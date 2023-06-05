# Comparing `tmp/vsmasktools-1.0.0.tar.gz` & `tmp/vsmasktools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmasktools-1.0.0.tar", last modified: Thu May  4 22:00:45 2023, max compression
+gzip compressed data, was "vsmasktools-1.1.0.tar", last modified: Mon Jun  5 14:01:29 2023, max compression
```

## Comparing `vsmasktools-1.0.0.tar` & `vsmasktools-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:45.262222 vsmasktools-1.0.0/vsmasktools/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/vsmasktools/edge/
--rw-r--r--   0 runner    (1001) docker     (123)    30484 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_2x2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_3x3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_5x5.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge/_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/edge_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/hardsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/morpho.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/spat_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-04 22:00:18.000000 vsmasktools-1.0.0/vsmasktools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:45.266222 vsmasktools-1.0.0/vsmasktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 22:00:45.000000 vsmasktools-1.0.0/vsmasktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:01:29.874000 vsmasktools-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-05 14:01:29.874000 vsmasktools-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 14:01:29.874000 vsmasktools-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:01:29.874000 vsmasktools-1.1.0/vsmasktools/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:01:29.874000 vsmasktools-1.1.0/vsmasktools/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)    30484 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/edge/_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/edge/_2x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/edge/_3x3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/edge/_5x5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/edge/_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/edge_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/hardsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/morpho.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/spat_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-06-05 14:01:06.000000 vsmasktools-1.1.0/vsmasktools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:01:29.874000 vsmasktools-1.1.0/vsmasktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-05 14:01:29.000000 vsmasktools-1.1.0/vsmasktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 14:01:29.000000 vsmasktools-1.1.0/vsmasktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:01:29.000000 vsmasktools-1.1.0/vsmasktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 14:01:29.000000 vsmasktools-1.1.0/vsmasktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 14:01:29.000000 vsmasktools-1.1.0/vsmasktools.egg-info/top_level.txt
```

### Comparing `vsmasktools-1.0.0/LICENSE` & `vsmasktools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/PKG-INFO` & `vsmasktools-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmasktools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Various masking tools for VapourSynth
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-masktools
 Project-URL: Documentation, https://vsmasktools.encode.moe/en/latest/
```

### Comparing `vsmasktools-1.0.0/README.md` & `vsmasktools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/setup.cfg` & `vsmasktools-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/setup.py` & `vsmasktools-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/__init__.py` & `vsmasktools-1.1.0/vsmasktools/__init__.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/abstract.py` & `vsmasktools-1.1.0/vsmasktools/abstract.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/details.py` & `vsmasktools-1.1.0/vsmasktools/details.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/diff.py` & `vsmasktools-1.1.0/vsmasktools/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     mask = Morpho.expand(mask, 2 + expand, mode=XxpandMode.ELLIPSE).std.Deflate()
 
     return depth(mask, bits)
 
 
 def diff_creditless(
-    credit_clip: vs.VideoNode, nc_clip: vs.VideoNode, thr: float = 0.1,
+    credit_clip: vs.VideoNode, nc_clip: vs.VideoNode, thr: float = 0.01,
     start_frame: int = 0, expand: int = 2, *, prefilter: bool | int = False,
     ep_clip: vs.VideoNode | None = None, func: FuncExceptT | None = None, **kwargs: Any
 ) -> vs.VideoNode:
     func = func or diff_creditless
 
     assert check_variable(credit_clip, func)
 
@@ -68,15 +68,15 @@
     diff_fmt = dst_fmt.replace(color_family=vs.GRAY)
 
     diff = ExprOp.mae(dst_fmt)(
         (Bicubic.resample(c, dst_fmt) for c in clips),
         format=diff_fmt, split_planes=True
     )
 
-    mask = Morpho.binarize(ExLaplacian4.edgemask(diff), thr / 10)
+    mask = ExLaplacian4.edgemask(diff, lthr=thr, hthr=thr)
     mask = Morpho.expand(mask, 2 + expand, mode=XxpandMode.ELLIPSE)
 
     if not ep_clip or ep_clip.num_frames == mask.num_frames:
         return mask
 
     blank = ep_clip.std.BlankClip(format=diff_fmt.id, keep=True)
```

### Comparing `vsmasktools-1.0.0/vsmasktools/edge/_1d.py` & `vsmasktools-1.1.0/vsmasktools/edge/_1d.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/edge/_3x3.py` & `vsmasktools-1.1.0/vsmasktools/edge/_3x3.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/edge/_5x5.py` & `vsmasktools-1.1.0/vsmasktools/edge/_5x5.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/edge/_abstract.py` & `vsmasktools-1.1.0/vsmasktools/edge/_abstract.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/edge_funcs.py` & `vsmasktools-1.1.0/vsmasktools/edge_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,31 +128,31 @@
     def _prefilter(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
         if self is self.RETINEX:  # type: ignore
             sigmas = kwargs.get('sigmas', [50, 200, 350])
 
             return retinex(clip, sigmas, 0.001, 0.005)
 
         if self is self.CLAHE:  # type: ignore
-            limit, tile = kwargs.get('limit', 0.305), kwargs.get('tile', 5)
+            limit, tile = kwargs.get('limit', 0.0305), kwargs.get('tile', 5)
 
-            return depth(depth(clip, 16).ehist.CLAHE(scale_value(limit / 10, 32, 16), tile), clip)
+            return depth(depth(clip, 16).ehist.CLAHE(scale_value(limit, 32, 16), tile), clip)
 
         return clip
 
     @overload
     def __call__(  # type: ignore
         self: Literal[RETINEX], src: vs.VideoNode, tsigma: float = 1, brz: float = 0.122,
         *, sigmas: Sequence[float] = [50, 200, 350]
     ) -> vs.VideoNode:
         ...
 
     @overload
     def __call__(  # type: ignore
         self: Literal[CLAHE], src: vs.VideoNode, tsigma: float = 1, brz: float = 0.122,
-        *, limit: float = 0.305, tile: int = 5
+        *, limit: float = 0.0305, tile: int = 5
     ) -> vs.VideoNode:
         ...
 
     def __call__(self, src: vs.VideoNode, tsigma: float = 1, brz: float = 0.122, **kwargs: Any) -> vs.VideoNode:
         luma = get_y(src)
 
         dreluma = self._prefilter(luma, **kwargs)
```

### Comparing `vsmasktools-1.0.0/vsmasktools/exceptions.py` & `vsmasktools-1.1.0/vsmasktools/exceptions.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/hardsub.py` & `vsmasktools-1.1.0/vsmasktools/hardsub.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/masks.py` & `vsmasktools-1.1.0/vsmasktools/masks.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/morpho.py` & `vsmasktools-1.1.0/vsmasktools/morpho.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/spat_funcs.py` & `vsmasktools-1.1.0/vsmasktools/spat_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     return norm_expr(
         msr_stats, expr_balance, None, y,
         ymin=get_lowest_value(y, False, ColorRange.LIMITED),
         ymax=get_peak_value(y, False, ColorRange.LIMITED)
     )
 
 
-def flat_mask(src: vs.VideoNode, radius: int = 5, thr: float = 0.11, gauss: bool = False) -> vs.VideoNode:
+def flat_mask(src: vs.VideoNode, radius: int = 5, thr: float = 0.011, gauss: bool = False) -> vs.VideoNode:
     luma = get_y(src)
 
     blur = gauss_blur(luma, radius * 0.361083333) if gauss else box_blur(luma, radius)
 
-    mask = depth(luma, 8).abrz.AdaptiveBinarize(depth(blur, 8), scale_value(thr / 10, 32, 8))
+    mask = depth(luma, 8).abrz.AdaptiveBinarize(depth(blur, 8), scale_value(thr, 32, 8))
 
     return depth(mask, luma, dither_type=DitherType.NONE, range_in=ColorRange.FULL, range_out=ColorRange.FULL)
```

### Comparing `vsmasktools-1.0.0/vsmasktools/types.py` & `vsmasktools-1.1.0/vsmasktools/types.py`

 * *Files identical despite different names*

### Comparing `vsmasktools-1.0.0/vsmasktools/utils.py` & `vsmasktools-1.1.0/vsmasktools/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,17 +167,14 @@
     """
     func = func or replace_squaremask
 
     assert check_variable(clipa, func) and check_variable(clipb, func)
 
     mask = squaremask(clipb[0], *mask_params, invert, func)
 
-    if ranges is None:
-        ranges = [(None, None)]
-
     if isinstance(blur_sigma, int):
         mask = box_blur(mask, blur_sigma)
     elif isinstance(blur_sigma, float):
         mask = gauss_blur(mask, blur_sigma)
 
     mask = mask.std.Loop(clipa.num_frames)
```

### Comparing `vsmasktools-1.0.0/vsmasktools.egg-info/PKG-INFO` & `vsmasktools-1.1.0/vsmasktools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmasktools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Various masking tools for VapourSynth
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-masktools
 Project-URL: Documentation, https://vsmasktools.encode.moe/en/latest/
```

### Comparing `vsmasktools-1.0.0/vsmasktools.egg-info/SOURCES.txt` & `vsmasktools-1.1.0/vsmasktools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

