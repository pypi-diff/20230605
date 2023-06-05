# Comparing `tmp/pydantic_zarr-0.1.2.tar.gz` & `tmp/pydantic_zarr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_zarr-0.1.2.tar", max compression
+gzip compressed data, was "pydantic_zarr-0.1.3.tar", max compression
```

## Comparing `pydantic_zarr-0.1.2.tar` & `pydantic_zarr-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.1.2/LICENSE
--rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.1.2/README.md
--rw-r--r--   0        0        0      489 2023-06-01 19:07:18.430532 pydantic_zarr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 17:37:02.193613 pydantic_zarr-0.1.2/src/pydantic_zarr/__init__.py
--rw-r--r--   0        0        0     8330 2023-06-01 19:05:25.338950 pydantic_zarr-0.1.2/src/pydantic_zarr/core.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.1.3/LICENSE
+-rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.1.3/README.md
+-rw-r--r--   0        0        0      489 2023-06-05 13:59:26.020614 pydantic_zarr-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-06-03 15:04:37.431488 pydantic_zarr-0.1.3/src/pydantic_zarr/__init__.py
+-rw-r--r--   0        0        0     9934 2023-06-05 13:57:00.113260 pydantic_zarr-0.1.3/src/pydantic_zarr/core.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.1.3/PKG-INFO
```

### Comparing `pydantic_zarr-0.1.2/LICENSE` & `pydantic_zarr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_zarr-0.1.2/src/pydantic_zarr/core.py` & `pydantic_zarr-0.1.3/src/pydantic_zarr/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
 from typing import (
     Any,
     Generic,
     Literal,
+    Mapping,
     Optional,
     TypeVar,
     Union,
 )
+from pydantic import root_validator, validator
 
 from pydantic.generics import GenericModel
 from zarr.storage import init_group, BaseStore
 import numcodecs
 import zarr
 import os
+import numpy as np
 
-TAttrs = TypeVar("TAttrs", bound=dict[str, Any])
-TItem = TypeVar("TItem", bound=Union["ArraySpec", "GroupSpec"])
+TAttrs = TypeVar("TAttrs", bound=Mapping[str, Any])
+TItem = TypeVar("TItem", bound=Union["GroupSpec", "ArraySpec"])
 
 DimensionSeparator = Union[Literal["."], Literal["/"]]
 ZarrVersion = Union[Literal[2], Literal[3]]
 ArrayOrder = Union[Literal["C"], Literal["F"]]
 
 
 class NodeSpec(GenericModel, Generic[TAttrs]):
@@ -36,26 +39,45 @@
         extra = "forbid"
 
 
 class ArraySpec(NodeSpec, Generic[TAttrs]):
     """
     This pydantic model represents the structural properties of a zarr array.
     It does not represent the data contained in the array. It is generic with respect to
-    to the type of attrs.
+    the type of attrs.
     """
 
     shape: tuple[int, ...]
     chunks: tuple[int, ...]
     dtype: str
     fill_value: Union[None, int, float] = 0
     order: ArrayOrder = "C"
     filters: Optional[list[dict[str, Any]]] = None
     dimension_separator: DimensionSeparator = "/"
     compressor: Optional[dict[str, Any]] = None
 
+    @validator("dtype", pre=True)
+    def stringify_dtype(cls, v):
+        """
+        Convert a np.dtype object into a string
+        """
+        if isinstance(v, np.dtype):
+            return str(v)
+        return v
+
+    @root_validator
+    def check_ndim(cls, values):
+        if (lshape := len(values["shape"])) != (lchunks := len(values["chunks"])):
+            msg = f"""
+            Length of shape must match length of chunks. Got {lshape} elements
+            for shape and {lchunks} elements for chunks.
+            """
+            raise ValueError(msg)
+        return values
+
     @classmethod
     def from_zarr(cls, zarray: zarr.Array):
         """
         Create an ArraySpec from a zarr array.
 
         Parameters
         ----------
@@ -83,40 +105,47 @@
             order=zarray.order,
             filters=filters,
             dimension_separator=zarray._dimension_separator,
             compressor=compressor,
             attrs=dict(zarray.attrs),
         )
 
-    def to_zarr(self, store: BaseStore, path: str) -> zarr.Array:
+    def to_zarr(
+        self, store: BaseStore, path: str, overwrite: bool = False
+    ) -> zarr.Array:
         """
         Serialize an ArraySpec to a zarr array at a specific path in a zarr store.
 
         Parameters
         ----------
         store : instance of zarr.BaseStore
             The storage backend that will manifest the array.
 
         path : str
             The location of the array inside the store.
 
+        overwrite : bool
+            Whether to overwrite an existing array or group at the path. If overwrite is
+            False and an array or group already exists at the path, an exception will be
+            raised. Defaults to False.
+
         Returns
         -------
         A zarr array that is structurally identical to the ArraySpec.
         This operation will create metadata documents in the store.
         """
         spec_dict = self.dict()
         attrs = spec_dict.pop("attrs")
         if self.compressor is not None:
             spec_dict["compressor"] = numcodecs.get_codec(spec_dict["compressor"])
         if self.filters is not None:
             spec_dict["filters"] = [
                 numcodecs.get_codec(f) for f in spec_dict["filters"]
             ]
-        result = zarr.create(store=store, path=path, **spec_dict)
+        result = zarr.create(store=store, path=path, **spec_dict, overwrite=overwrite)
         result.attrs.put(attrs)
         return result
 
 
 class GroupSpec(NodeSpec, Generic[TAttrs, TItem]):
     items: dict[str, TItem] = {}
 
@@ -151,43 +180,49 @@
                 """
                 raise ValueError(msg)
             items[name] = _item
 
         result = GroupSpec(attrs=dict(zgroup.attrs), items=items)
         return result
 
-    def to_zarr(self, store: BaseStore, path: str):
+    def to_zarr(self, store: BaseStore, path: str, overwrite: bool = False):
         """
         Serialize a GroupSpec to a zarr group at a specific path in a zarr store.
 
         Parameters
         ----------
         store : instance of zarr.BaseStore
             The storage backend that will manifest the group and its contents.
 
         path : str
             The location of the group inside the store.
 
+        overwrite : bool
+            Whether to overwrite an existing array or group at the path. If overwrite is
+            False and an array or group already exists at the path, an exception will be
+            raised. Defaults to False.
+
         Returns
         -------
         A zarr group that is structurally identical to the GroupSpec.
         This operation will create metadata documents in the store.
         """
         spec_dict = self.dict()
         # pop items because it's not a valid kwarg for init_group
         spec_dict.pop("items")
         # pop attrs because it's not a valid kwarg for init_group
         attrs = spec_dict.pop("attrs")
-        # needing to call init_group, then zarr.group is not ergonomic
-        init_group(store=store, path=path)
-        result = zarr.group(store=store, path=path, **spec_dict)
+        # weird that we have to call init_group before creating the group
+        init_group(store, overwrite=overwrite, path=path)
+        result = zarr.group(store=store, path=path, **spec_dict, overwrite=overwrite)
         result.attrs.put(attrs)
         for name, item in self.items.items():
             subpath = os.path.join(path, name)
-            item.to_zarr(store, subpath)
+            item.to_zarr(store, subpath, overwrite=overwrite)
+
         return result
 
 
 def from_zarr(element: Union[zarr.Array, zarr.Group]) -> Union[ArraySpec, GroupSpec]:
     """
     Recursively parse a Zarr group or Zarr array into an ArraySpec or GroupSpec.
 
@@ -227,15 +262,18 @@
         GroupLike protocols.
         """
         raise ValueError(msg)
     return result
 
 
 def to_zarr(
-    spec: Union[ArraySpec, GroupSpec], store: BaseStore, path: str
+    spec: Union[ArraySpec, GroupSpec],
+    store: BaseStore,
+    path: str,
+    overwrite: bool = False,
 ) -> Union[zarr.Array, zarr.Group]:
     """
     Serialize a GroupSpec or ArraySpec to a zarr group or array at a specific path in
     a zarr store.
 
     Parameters
     ----------
@@ -244,24 +282,29 @@
 
     store : instance of zarr.BaseStore
         The storage backend that will manifest the group or array.
 
     path : str
         The location of the group or array inside the store.
 
+    overwrite : bool
+       Whether to overwrite an existing array or group at the path. If overwrite is
+        False and an array or group already exists at the path, an exception will be
+        raised. Defaults to False.
+
     Returns
     -------
     A zarr Group or Array that is structurally identical to the spec object.
     This operation will create metadata documents in the store.
 
     """
     if isinstance(spec, ArraySpec):
-        result = spec.to_zarr(store, path)
+        result = spec.to_zarr(store, path, overwrite=overwrite)
     elif isinstance(spec, GroupSpec):
-        result = spec.to_zarr(store, path)
+        result = spec.to_zarr(store, path, overwrite=overwrite)
     else:
         msg = f"""
         Invalid argument for spec. Expected an instance of GroupSpec or ArraySpec, got
         {type(spec)} instead.
         """
         raise ValueError(msg)
```

### Comparing `pydantic_zarr-0.1.2/PKG-INFO` & `pydantic_zarr-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-zarr
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

