# Comparing `tmp/vssource-0.9.2.tar.gz` & `tmp/vssource-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vssource-0.9.2.tar", last modified: Wed May 24 17:09:45 2023, max compression
+gzip compressed data, was "vssource-0.9.3.tar", last modified: Mon Jun  5 20:25:30 2023, max compression
```

## Comparing `vssource-0.9.2.tar` & `vssource-0.9.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:45.495139 vssource-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 17:09:18.000000 vssource-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-24 17:09:45.495139 vssource-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-24 17:09:18.000000 vssource-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-24 17:09:45.495139 vssource-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-24 17:09:18.000000 vssource-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:45.491138 vssource-0.9.2/vssource/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/dataclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:45.491138 vssource-0.9.2/vssource/formats/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:45.491138 vssource-0.9.2/vssource/formats/bd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/formats/bd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:45.495139 vssource-0.9.2/vssource/formats/dvd/
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/formats/dvd/IsoFile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/formats/dvd/IsoFileCore.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/formats/dvd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:45.495139 vssource-0.9.2/vssource/formats/dvd/parsedvd/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/formats/dvd/parsedvd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/formats/dvd/parsedvd/sector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/formats/dvd/parsedvd/vts_pgci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:45.495139 vssource-0.9.2/vssource/indexers/
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/indexers/D2VWitch.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/indexers/DGIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/indexers/DGIndexNV.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/indexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/indexers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/indexers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 17:09:18.000000 vssource-0.9.2/vssource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:45.491138 vssource-0.9.2/vssource.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-24 17:09:45.000000 vssource-0.9.2/vssource.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-24 17:09:45.000000 vssource-0.9.2/vssource.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:09:45.000000 vssource-0.9.2/vssource.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 17:09:45.000000 vssource-0.9.2/vssource.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 17:09:45.000000 vssource-0.9.2/vssource.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.884524 vssource-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 20:25:06.000000 vssource-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-05 20:25:30.884524 vssource-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-05 20:25:06.000000 vssource-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-05 20:25:30.884524 vssource-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-05 20:25:06.000000 vssource-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/dataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource/formats/bd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/bd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource/formats/dvd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/IsoFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/IsoFileCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.884524 vssource-0.9.3/vssource/formats/dvd/parsedvd/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/parsedvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/parsedvd/sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/formats/dvd/parsedvd/vts_pgci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.884524 vssource-0.9.3/vssource/indexers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/D2VWitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/DGIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/DGIndexNV.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/indexers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-05 20:25:06.000000 vssource-0.9.3/vssource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:25:30.880524 vssource-0.9.3/vssource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 20:25:30.000000 vssource-0.9.3/vssource.egg-info/top_level.txt
```

### Comparing `vssource-0.9.2/LICENSE` & `vssource-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/PKG-INFO` & `vssource-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vssource
-Version: 0.9.2
+Version: 0.9.3
 Summary: Vapoursynth Wrapper for DVDs stuff
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-source
 Project-URL: Documentation, https://vssource.encode.moe/en/latest/
```

### Comparing `vssource-0.9.2/README.md` & `vssource-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/setup.cfg` & `vssource-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/setup.py` & `vssource-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/vssource/dataclasses.py` & `vssource-0.9.3/vssource/dataclasses.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/vssource/formats/dvd/IsoFile.py` & `vssource-0.9.3/vssource/formats/dvd/IsoFile.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/vssource/formats/dvd/IsoFileCore.py` & `vssource-0.9.3/vssource/formats/dvd/IsoFileCore.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/vssource/formats/dvd/parsedvd/sector.py` & `vssource-0.9.3/vssource/formats/dvd/parsedvd/sector.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/vssource/formats/dvd/parsedvd/vts_pgci.py` & `vssource-0.9.3/vssource/formats/dvd/parsedvd/vts_pgci.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/vssource/indexers/D2VWitch.py` & `vssource-0.9.3/vssource/indexers/D2VWitch.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/vssource/indexers/DGIndex.py` & `vssource-0.9.3/vssource/indexers/DGIndex.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/vssource/indexers/DGIndexNV.py` & `vssource-0.9.3/vssource/indexers/DGIndexNV.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import subprocess
 from fractions import Fraction
 from functools import lru_cache, reduce
 from typing import Sequence
 
 from vstools import SPath, core
 
 from ..dataclasses import DGIndexFileInfo, DGIndexFooter, DGIndexFrameData, DGIndexHeader, IndexFileVideo
```

### Comparing `vssource-0.9.2/vssource/indexers/base.py` & `vssource-0.9.3/vssource/indexers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,17 +49,29 @@
 
     @classmethod
     def get_videos_hash(cls, files: list[SPath]) -> str:
         lenght = sum(file.stat().st_size for file in files)
         to_hash = lenght.to_bytes(32, 'little') + cls.get_joined_names(files).encode()
         return md5(to_hash).hexdigest()
 
-    @property
-    def source_func(self) -> VSSourceFunc:
-        return self._source_func
+    @classmethod
+    def source_func(self, path: DataType | SPathLike, *args: Any, **kwargs: Any) -> vs.VideoNode:
+        return self._source_func(str(path), *args, **kwargs)
+
+    @classmethod
+    def normalize_filenames(cls, file: SPathLike | Sequence[SPathLike]) -> list[SPath]:
+        files = list[SPath]()
+
+        for f in to_arr(file):  # type: ignore
+            if str(f).startswith('file:///'):
+                f = str(f)[8::]  # type: ignore
+
+            files.append(SPath(f))
+
+        return files
 
     def _source(
         self, clips: Iterable[vs.VideoNode],
         bits: int | None = None,
         matrix: MatrixT | None = None,
         transfer: TransferT | None = None,
         primaries: PrimariesT | None = None,
@@ -87,15 +99,15 @@
         primaries: PrimariesT | None = None,
         chroma_location: ChromaLocationT | None = None,
         color_range: ColorRangeT | None = None,
         field_based: FieldBasedT | None = None,
         **kwargs: Any
     ) -> vs.VideoNode:
         return self._source(
-            [self.source_func(SPath(f).to_str(), **kwargs) for f in to_arr(file)],  # type: ignore
+            [self.source_func(f.to_str(), **kwargs) for f in self.normalize_filenames(file)],
             bits, matrix, transfer, primaries, chroma_location, color_range, field_based
         )
 
 
 class ExternalIndexer(Indexer):
     _bin_path: ClassVar[str]
     _ext: ClassVar[str]
@@ -245,13 +257,13 @@
         transfer: TransferT | None = None,
         primaries: PrimariesT | None = None,
         chroma_location: ChromaLocationT | None = None,
         color_range: ColorRangeT | None = None,
         field_based: FieldBasedT | None = None,
         **kwargs: Any
     ) -> vs.VideoNode:
-        index_files = self.index([SPath(f) for f in to_arr(file)])  # type: ignore
+        index_files = self.index(self.normalize_filenames(file))
 
         return self._source(
             (self.source_func(idx_filename.to_str(), **kwargs) for idx_filename in index_files),
             bits, matrix, transfer, primaries, chroma_location, color_range, field_based
         )
```

### Comparing `vssource-0.9.2/vssource/utils.py` & `vssource-0.9.3/vssource/utils.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.2/vssource.egg-info/PKG-INFO` & `vssource-0.9.3/vssource.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vssource
-Version: 0.9.2
+Version: 0.9.3
 Summary: Vapoursynth Wrapper for DVDs stuff
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-source
 Project-URL: Documentation, https://vssource.encode.moe/en/latest/
```

### Comparing `vssource-0.9.2/vssource.egg-info/SOURCES.txt` & `vssource-0.9.3/vssource.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 vssource/__init__.py
 vssource/_metadata.py
 vssource/dataclasses.py
+vssource/funcs.py
 vssource/py.typed
 vssource/utils.py
 vssource.egg-info/PKG-INFO
 vssource.egg-info/SOURCES.txt
 vssource.egg-info/dependency_links.txt
 vssource.egg-info/requires.txt
 vssource.egg-info/top_level.txt
```

