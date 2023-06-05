# Comparing `tmp/bipl-0.2.1.tar.gz` & `tmp/bipl-0.2.2.tar.gz`

## Comparing `bipl-0.2.1.tar` & `bipl-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    14285 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.2.1/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.2.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.2.1/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.2.1/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.2.1/hatch_build.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bipl-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 bipl-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.2.2/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.2.2/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.2.2/hatch_build.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bipl-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 bipl-0.2.2/PKG-INFO
```

### Comparing `bipl-0.2.1/src/bipl/io/__init__.py` & `bipl-0.2.2/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/src/bipl/io/_dzi.py` & `bipl-0.2.2/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/src/bipl/io/_libs.py` & `bipl-0.2.2/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/src/bipl/io/_openslide.py` & `bipl-0.2.2/src/bipl/io/_openslide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/src/bipl/io/_slide.py` & `bipl-0.2.2/src/bipl/io/_slide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/src/bipl/io/_slide_bases.py` & `bipl-0.2.2/src/bipl/io/_slide_bases.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/src/bipl/io/_tiff.py` & `bipl-0.2.2/src/bipl/io/_tiff.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/src/bipl/ops/_mosaic.py` & `bipl-0.2.2/src/bipl/ops/_mosaic.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,16 @@
 
         ih, iw = self.ishape
         step = self.m.step // scale
         pad = self.m.overlap // (scale * 2)
 
         mh, mw = (ih * step), (iw * step)
         if mask.shape[:2] != (mh, mw):
-            mask_pad = [(0, s1 - s0) for s0, s1 in zip(mask.shape, (mh, mw))]
+            mask_pad = [(0, max(0, s1 - s0))
+                        for s0, s1 in zip(mask.shape, (mh, mw))]
             mask = np.pad(mask, mask_pad)[:mh, :mw]
 
         if self.m.overlap:
             kernel = np.ones((3, 3), dtype='u1')
             mask = cv2.dilate(mask, kernel, iterations=pad)
 
         if pad:
```

### Comparing `bipl-0.2.1/src/bipl/ops/_util.py` & `bipl-0.2.2/src/bipl/ops/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/LICENSE` & `bipl-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/README.md` & `bipl-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/hatch_build.py` & `bipl-0.2.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.2.1/pyproject.toml` & `bipl-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.2.1"
+version = "0.2.2"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
```

### Comparing `bipl-0.2.1/PKG-INFO` & `bipl-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.2.1
+Version: 0.2.2
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
```

