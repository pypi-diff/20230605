# Comparing `tmp/func_adl-3.2.5a1.tar.gz` & `tmp/func_adl-3.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/func_adl-3.2.5a1.tar", last modified: Mon Jun  5 17:54:50 2023, max compression
+gzip compressed data, was "dist/func_adl-3.2b1.tar", last modified: Sun Feb 12 10:04:09 2023, max compression
```

## Comparing `func_adl-3.2.5a1.tar` & `func_adl-3.2b1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/func_adl/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/func_adl/ast/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/ast/aggregate_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/ast/ast_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/ast/call_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/ast/func_adl_ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20316 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/ast/function_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/ast/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/ast/syntatic_sugar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/object_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    35230 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)    24078 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/util_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/func_adl/util_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/func_adl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/func_adl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/func_adl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/func_adl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/func_adl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/func_adl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:54:50.000000 func_adl-3.2.5a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/tests/test_event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/tests/test_object_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    28551 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/tests/test_type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/tests/test_type_based_replacement_py310.py
--rw-r--r--   0 runner    (1001) docker     (123)    20902 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/tests/test_util_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-05 17:54:44.000000 func_adl-3.2.5a1/tests/test_util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-02-12 10:04:09.000000 func_adl-3.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-02-12 10:04:06.000000 func_adl-3.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl/ast/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/aggregate_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/ast_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/call_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/func_adl_ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20316 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/function_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/syntatic_sugar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35230 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23874 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-12 10:04:06.000000 func_adl-3.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 10:04:09.000000 func_adl-3.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-02-12 10:04:06.000000 func_adl-3.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28551 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_type_based_replacement_py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_util_types.py
```

### Comparing `func_adl-3.2.5a1/PKG-INFO` & `func_adl-3.2b1/func_adl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
-Name: func_adl
-Version: 3.2.5a1
+Name: func-adl
+Version: 3.2b1
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
-License: MIT
+License: TBD
 Platform: Any
-Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: complete
```

### Comparing `func_adl-3.2.5a1/README.md` & `func_adl-3.2b1/README.md`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/ast/aggregate_shortcuts.py` & `func_adl-3.2b1/func_adl/ast/aggregate_shortcuts.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/ast/call_stack.py` & `func_adl-3.2b1/func_adl/ast/call_stack.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/ast/func_adl_ast_utils.py` & `func_adl-3.2b1/func_adl/ast/func_adl_ast_utils.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/ast/function_simplifier.py` & `func_adl-3.2b1/func_adl/ast/function_simplifier.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/ast/meta_data.py` & `func_adl-3.2b1/func_adl/ast/meta_data.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/ast/syntatic_sugar.py` & `func_adl-3.2b1/func_adl/ast/syntatic_sugar.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/event_dataset.py` & `func_adl-3.2b1/func_adl/event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/functions.py` & `func_adl-3.2b1/func_adl/functions.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/object_stream.py` & `func_adl-3.2b1/func_adl/object_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
 
 import ast
-import copy
 import logging
-import typing
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     Generic,
     Iterable,
@@ -85,20 +83,14 @@
         """Return the query `ast` that this `ObjectStream` represents
 
         Returns:
             ast.AST: The python `ast` that is represented by this query
         """
         return self._q_ast
 
-    def clone_with_new_ast(self, new_ast: ast.AST, new_type: typing.Any):
-        clone = copy.deepcopy(self)
-        clone._q_ast = new_ast
-        clone._item_type = new_type
-        return clone
-
     def SelectMany(
         self, func: Union[str, ast.Lambda, Callable[[T], Iterable[S]]]
     ) -> ObjectStream[S]:
         r"""
         Given the current stream's object type is an array or other iterable, return
         the items in this objects type, one-by-one. This has the effect of flattening a
         nested array.
@@ -114,20 +106,20 @@
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         from func_adl.type_based_replacement import remap_from_lambda
 
         n_stream, n_ast, rtn_type = remap_from_lambda(
-            self, _local_simplification(parse_as_ast(func, "SelectMany"))
+            self, _local_simplification(parse_as_ast(func))
         )
-
-        return self.clone_with_new_ast(
+        return ObjectStream[S](
             function_call("SelectMany", [n_stream.query_ast, cast(ast.AST, n_ast)]),
-            unwrap_iterable(rtn_type))
+            unwrap_iterable(rtn_type),
+        )
 
     def Select(self, f: Union[str, ast.Lambda, Callable[[T], S]]) -> ObjectStream[S]:
         r"""
         Apply a transformation function to each object in the stream, yielding a new type of
         object. There is a one-to-one correspondence between the input objects and output objects.
 
         Arguments:
@@ -140,18 +132,16 @@
 
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         from func_adl.type_based_replacement import remap_from_lambda
 
-        n_stream, n_ast, rtn_type = remap_from_lambda(
-            self, _local_simplification(parse_as_ast(f, "Select"))
-        )
-        return self.clone_with_new_ast(
+        n_stream, n_ast, rtn_type = remap_from_lambda(self, _local_simplification(parse_as_ast(f)))
+        return ObjectStream[S](
             function_call("Select", [n_stream.query_ast, cast(ast.AST, n_ast)]), rtn_type
         )
 
     def Where(self, filter: Union[str, ast.Lambda, Callable[[T], bool]]) -> ObjectStream[T]:
         r"""
         Filter the object stream, allowing only items for which `filter` evaluates as true through.
 
@@ -166,30 +156,30 @@
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         from func_adl.type_based_replacement import remap_from_lambda
 
         n_stream, n_ast, rtn_type = remap_from_lambda(
-            self, _local_simplification(parse_as_ast(filter, "Where"))
+            self, _local_simplification(parse_as_ast(filter))
         )
         if rtn_type != bool:
             raise ValueError(f"The Where filter must return a boolean (not {rtn_type})")
-        return self.clone_with_new_ast(
+        return ObjectStream[T](
             function_call("Where", [n_stream.query_ast, cast(ast.AST, n_ast)]), self.item_type
         )
 
     def MetaData(self, metadata: Dict[str, Any]) -> ObjectStream[T]:
         """Add metadata to the current object stream. The metadata is an arbitrary set of string
         key-value pairs. The backend must be able to properly interpret the metadata.
 
         Returns:
             ObjectStream: A new stream, of the same type and contents, but with metadata added.
         """
-        return self.clone_with_new_ast(
+        return ObjectStream[T](
             function_call("MetaData", [self._q_ast, as_ast(metadata)]), self.item_type
         )
 
     def QMetaData(self, metadata: Dict[str, Any]) -> ObjectStream[T]:
         """Add query metadata to the current object stream.
 
         - Metadata is never transmitted to any back end
@@ -220,15 +210,15 @@
             if add_md:
                 if first:
                     first = False
                     base_ast = self.MetaData({}).query_ast
                     base_ast._q_metadata = {}  # type: ignore
                 base_ast._q_metadata[k] = v  # type: ignore
 
-        return self.clone_with_new_ast(base_ast, self.item_type)
+        return ObjectStream[T](base_ast, self.item_type)
 
     def AsPandasDF(
         self, columns: Union[str, List[str]] = []
     ) -> ObjectStream[ReturnedDataPlaceHolder]:
         r"""
         Return a pandas stream that contains one item, an pandas `DataFrame`.
         This `DataFrame` will contain all the data fed to it. Only non-array datatypes are
@@ -244,14 +234,16 @@
         if isinstance(columns, str):
             columns = [columns]
 
         return ObjectStream[ReturnedDataPlaceHolder](
             function_call("ResultPandasDF", [self._q_ast, as_ast(columns)])
         )
 
+    as_pandas = AsPandasDF
+
     def AsROOTTTree(
         self, filename: str, treename: str, columns: Union[str, List[str]] = []
     ) -> ObjectStream[ReturnedDataPlaceHolder]:
         r"""
         Return the sequence of items as a ROOT TTree. Each item in the ObjectStream
         will get one entry in the file. The items must be of types that the infrastructure
         can work with:
```

### Comparing `func_adl-3.2.5a1/func_adl/type_based_replacement.py` & `func_adl-3.2b1/func_adl/type_based_replacement.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/func_adl/util_ast.py` & `func_adl-3.2b1/func_adl/util_ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,22 +643,18 @@
         if len(good_lambdas) == 0:
             raise ValueError(
                 f"Internal Error - Found no lambda in source with the arguments {caller_arg_list}"
             )
 
         if len(good_lambdas) > 1:
             raise ValueError(
-                "Found multiple calls on same line"
+                "Found multiple calls to on same line"
                 + ("" if caller_name is None else f" for {caller_name}")
                 + " - split the calls across "
-                """lines or change lambda argument names so they are different. For example change:
-                    df.Select(lambda x: x + 1).Select(lambda x: x + 2)
-                    to:
-                    df.Select(lambda x: x + 1).Select(lambda y: y + 2)
-                """
+                "lines or change lambda argument names so they are different."
             )
 
         lda = good_lambdas[0]
 
     return lda
```

### Comparing `func_adl-3.2.5a1/func_adl/util_types.py` & `func_adl-3.2b1/func_adl/util_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import inspect
 import sys
-import typing
 from typing import Any, Dict, Optional, Tuple, Type, TypeVar
 
 if sys.version_info >= (3, 8):
     from typing import get_args, get_origin
 else:  # pragma: no cover
     # TODO: Remove this when we drop support for 3.7
     def get_args(tp):
@@ -22,15 +21,17 @@
         t = get_inherited(t)
 
     return t is not Any
 
 
 def _is_iterable_direct(t: Type) -> bool:
     "Is this type iterable?"
-    return getattr(t, "_name", None) == "Iterable" or getattr(t, "__name__", None) == "Iterable"
+    if getattr(t, "_name", None) == "Iterable":
+        return True
+    return False
 
 
 def get_inherited(t: Type) -> Type:
     """Returns the inherited type of `t`
 
     Notes:
     * This works for 3.7 forward (but not back!)
@@ -49,26 +50,15 @@
         return Any
 
     r = base_classes[0]  # type: ignore
 
     g_args = get_args(t)
     if len(g_args) > 0:
         mapping = {a.__name__: v for a, v in zip(r.__parameters__, g_args)}
-
-        r_base = get_origin(r)
-        assert r_base is not None, "Internal error"
-
-        # Get us back to typing if this is a common interface.
-        # This is not needed in python 3.11 and forward, where
-        # collections.abc.X can are all be parameterized.
-        if r_base.__name__ in typing.__dict__:
-            r_base = typing.__dict__[r_base.__name__]
-
-        # Re-parameterize the type with the information e have from this parameterization.
-        r = r_base[tuple(_resolve_type(t_arg, mapping) for t_arg in get_args(r))]
+        r.__args__ = tuple(_resolve_type(t_arg, mapping) for t_arg in get_args(r))
 
     return r
 
 
 def unwrap_iterable(t: Type) -> Type:
     "Unwrap an iterable type"
     # Try to find an iterable in the history somehow
@@ -123,15 +113,15 @@
     Args:
         t (Type): The type to resolve
         parameters (Dict[str, Type]): The dict of types to resolve
 
     Returns:
         None if `t` is parameterized by unknown type var's
         The resolved type (a copy leaving `t` untouched) if TypeVar's are filled in
-        The type if no substitution is required.
+        The type if no substition is required.
     """
     if isinstance(t, TypeVar):
         if t.__name__ in parameters:
             return parameters[t.__name__]
         return None
 
     template_params = getattr(t, "__parameters__", None)
```

### Comparing `func_adl-3.2.5a1/func_adl.egg-info/PKG-INFO` & `func_adl-3.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
-Name: func-adl
-Version: 3.2.5a1
+Name: func_adl
+Version: 3.2b1
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
-License: MIT
+License: TBD
 Platform: Any
-Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: complete
```

### Comparing `func_adl-3.2.5a1/func_adl.egg-info/SOURCES.txt` & `func_adl-3.2b1/func_adl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/setup.py` & `func_adl-3.2b1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 extras_require["complete"] = sorted(set(sum(extras_require.values(), [])))
 
 version = os.getenv("func_adl_version")
 if version is None:
     import logging
 
     logging.error("func_adl_version environment variable not set")
-    version = "3.2"
+    version = "0.0.1a1"
 version = version.split("/")[-1]
 
 setup(
     name="func_adl",
     version=version,
     packages=["func_adl", "func_adl/ast"],
     scripts=[],
@@ -43,34 +43,35 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="G. Watts (IRIS-HEP/UW Seattle)",
     author_email="gwatts@uw.edu",
     maintainer="Gordon Watts (IRIS-HEP/UW Seattle)",
     maintainer_email="gwatts@uw.edu",
     url="https://github.com/iris-hep/func_adl",
-    license="MIT",
+    license="TBD",
     test_suite="tests",
     install_requires=["make-it-sync"],
     setup_requires=["pytest-runner"],
     tests_require=["pytest>=3.9"],
     extras_require=extras_require,
     classifiers=[
         # "Development Status :: 3 - Alpha",
         # "Development Status :: 4 - Beta",
-        "Development Status :: 5 - Production/Stable",
+        # "Development Status :: 5 - Production/Stable",
         # "Development Status :: 6 - Mature",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.6",
         "Topic :: Software Development",
         "Topic :: Utilities",
     ],
     data_files=[],
     python_requires=">=3.6, <3.12",
     platforms="Any",
 )
```

### Comparing `func_adl-3.2.5a1/tests/test_event_dataset.py` & `func_adl-3.2b1/tests/test_event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/tests/test_object_stream.py` & `func_adl-3.2b1/tests/test_object_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,14 @@
         .Select("lambda j: j.pT()")
         .AsROOTTTree("junk.root", "analysis", "jetPT")
         .value()
     )
     assert isinstance(r, ast.AST)
 
 
-def test_simple_query_one_line():
-    """Make sure we parse 2 functions on one line correctly"""
-    r = my_event().Select(lambda e: e.met).Where(lambda e: e > 10).value()
-    assert isinstance(r, ast.AST)
-
-
 def test_two_simple_query():
     r1 = (
         my_event()
         .SelectMany("lambda e: e.jets()")
         .Select("lambda j: j.pT()")
         .AsROOTTTree("junk.root", "analysis", "jetPT")
         .value()
```

### Comparing `func_adl-3.2.5a1/tests/test_type_based_replacement.py` & `func_adl-3.2b1/tests/test_type_based_replacement.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/tests/test_type_based_replacement_py310.py` & `func_adl-3.2b1/tests/test_type_based_replacement_py310.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.5a1/tests/test_util_ast.py` & `func_adl-3.2b1/tests/test_util_ast.py`

 * *Files 3% similar despite different names*

```diff
@@ -678,46 +678,14 @@
         .value()
     )
     # fmt: on
     assert jets_pflow is not None  # Just to keep flake8 happy without adding a noqa above.
     assert "uncalibrated_collection" in ast.dump(found[0])
 
 
-def test_parse_select_where():
-    "Common lambas with different parent functions on one line - found in wild"
-
-    found = []
-
-    class my_obj:
-        def Where(self, x: Callable):
-            found.append(parse_as_ast(x, "Where"))
-            return self
-
-        def Select(self, x: Callable):
-            found.append(parse_as_ast(x, "Select"))
-            return self
-
-        def AsAwkwardArray(self, stuff: str):
-            return self
-
-        def value(self):
-            return self
-
-    jets_pflow_name = "hi"
-    ds_dijet = my_obj()
-
-    # fmt: off
-    jets_pflow = (
-        ds_dijet.Select(lambda e: e.met).Where(lambda e: e > 100)
-    )
-    # fmt: on
-    assert jets_pflow is not None  # Just to keep flake8 happy without adding a noqa above.
-    assert "met" in ast.dump(found[0])
-
-
 def test_parse_multiline_lambda_ok_with_one_as_arg():
     "Make sure we can properly parse a multi-line lambda - but now with argument"
 
     found = []
 
     class my_obj:
         def do_it(self, x: Callable, counter: int):
```

### Comparing `func_adl-3.2.5a1/tests/test_util_types.py` & `func_adl-3.2b1/tests/test_util_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     T = TypeVar("T")
 
     class bogus(Iterable[T]):
         pass
 
     myc = bogus[int]
 
-    assert get_inherited(myc) == Iterable[int]  # type: ignore
+    assert get_inherited(myc) == Iterable[int]
 
 
 def test_get_inherited_two_levels():
     T = TypeVar("T")
     U = TypeVar("U")
 
     class bogus(Generic[T]):
@@ -102,27 +102,14 @@
     class bogus2(bogus[Iterable[U]]):
         pass
 
     myc = bogus2[int]
     assert get_inherited(myc) == bogus[Iterable[int]]
 
 
-def test_get_inherited_generic_twice():
-    T = TypeVar("T")
-
-    class bogus(Iterable[T]):
-        pass
-
-    myc = bogus[int]
-    assert get_inherited(myc) == Iterable[int]  # type: ignore
-
-    myd = bogus[float]
-    assert get_inherited(myd) == Iterable[float]  # type: ignore
-
-
 def test_build_type_int():
     assert build_type_dict_from_type(int) == {}
 
 
 def test_build_type_generic():
     T = TypeVar("T")
```

