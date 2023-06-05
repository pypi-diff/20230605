# Comparing `tmp/vsdehalo-1.7.0.tar.gz` & `tmp/vsdehalo-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdehalo-1.7.0.tar", last modified: Thu May  4 21:59:26 2023, max compression
+gzip compressed data, was "vsdehalo-1.7.1.tar", last modified: Mon Jun  5 14:33:46 2023, max compression
```

## Comparing `vsdehalo-1.7.0.tar` & `vsdehalo-1.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/vsdehalo/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    31383 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/vine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-05-04 21:58:59.000000 vsdehalo-1.7.0/vsdehalo/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:26.015532 vsdehalo-1.7.0/vsdehalo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 21:59:26.000000 vsdehalo-1.7.0/vsdehalo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/vsdehalo/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/vine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-05 14:33:24.000000 vsdehalo-1.7.1/vsdehalo/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:33:46.603425 vsdehalo-1.7.1/vsdehalo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 14:33:46.000000 vsdehalo-1.7.1/vsdehalo.egg-info/top_level.txt
```

### Comparing `vsdehalo-1.7.0/LICENSE` & `vsdehalo-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.0/PKG-INFO` & `vsdehalo-1.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdehalo
-Version: 1.7.0
+Version: 1.7.1
 Summary: Collection of dehaloing VapourSynth functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-dehalo
 Project-URL: Documentation, https://vsdehalo.encode.moe/en/latest/
```

### Comparing `vsdehalo-1.7.0/setup.cfg` & `vsdehalo-1.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.0/setup.py` & `vsdehalo-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.0/vsdehalo/alpha.py` & `vsdehalo-1.7.1/vsdehalo/alpha.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,52 +647,52 @@
     if not chroma:
         return dehalo
 
     return join([dehalo, *chroma], clip.format.color_family)
 
 
 def dehalomicron(
-    clip: vs.VideoNode, brz: float = 0.75, sigma: float = 1.55, sigma0: float = 1.15, ss: float = 1.65,
+    clip: vs.VideoNode, brz: float = 0.075, sigma: float = 1.55, sigma0: float = 1.15, ss: float = 1.65,
     pre_ss: bool = True, dampen: float | list[float] | tuple[float | list[float], bool | None] = 0.65,
-    sigma_ref: float = 4.3333, planes: PlanesT = 0, fdhealo_kwargs: KwargsT | None = None, **kwargs: Any
+    sigma_ref: float = 4.3333, planes: PlanesT = 0, fdehalo_kwargs: KwargsT | None = None, **kwargs: Any
 ) -> vs.VideoNode:
     func = FunctionUtil(clip, dehalomicron, planes, (vs.GRAY, vs.YUV))
 
-    fdhealo_kwargs = KwargsT(edgeproc=0.5, ss=1.5 if pre_ss else 2.0) | (fdhealo_kwargs or {})
+    fdehalo_kwargs = KwargsT(edgeproc=0.5, ss=1.5 if pre_ss else 2.0) | (fdehalo_kwargs or {})
 
     y = get_y(func.work_clip)
 
     y_mask = retinex(y)
 
     dehalo_ref0 = dehalo_sigma(func.work_clip, sigma=sigma0, planes=planes)
     dehalo_ref0mask = dehalo_sigma(y_mask, sigma=sigma0 + sigma0 * 0.09)
 
     ymask_ref0 = gauss_blur(y_mask, sigma=sigma_ref)
 
     dehalo_mask = norm_expr([dehalo_ref0mask, y_mask], 'x y - abs 100 *')
     dehalo_mask = RemoveGrainMode.CIRCLE_BLUR(dehalo_mask)
     dehalo_mask = RemoveGrainMode.MINMAX_MEDIAN_OPP(dehalo_mask)
 
-    dmask_expr = 'x 2 *'
-
-    if brz != 0.0:
-        dmask_expr = f"x {scale_value(abs(brz) / 10, 32, y)} {'>' if brz < 0.0 else '>'} 0 {dmask_expr} ?"
+    if brz:
+        dmask_expr = f"x {scale_value(abs(brz), 32, y)} {'>' if brz < 0.0 else '>'} 0 x 2 * ?"
+    else:
+        dmask_expr = 'x 2 *'
 
     dehalo_mask = norm_expr(dehalo_mask, dmask_expr, func.norm_planes)
 
     fine_edge_mask = fine_dehalo.mask(norm_expr([y_mask, ymask_ref0], 'y x -'), planes=func.norm_planes)
     dehalo_mask = norm_expr(
         [dehalo_mask, y_mask, ymask_ref0, fine_edge_mask], 'y z + 2 / x < x and x abs a ?', func.norm_planes
     )
     dehalo_mask = RemoveGrainMode.EDGE_CLIP_STRONG(dehalo_mask)
 
     actual_dehalo = dehalo_sigma(
         func.work_clip, pre_ss=1 + pre_ss, sigma=sigma, ss=ss - 0.5 * pre_ss, planes=func.norm_planes, **kwargs
     )
-    dehalo_ref = fine_dehalo(func.work_clip, planes=func.norm_planes, **fdhealo_kwargs)
+    dehalo_ref = fine_dehalo(func.work_clip, planes=func.norm_planes, **fdehalo_kwargs)
 
     dehalo_min = ExprOp.MIN(actual_dehalo, dehalo_ref, planes=func.norm_planes)
 
     dehalo = limit_filter(actual_dehalo, func.work_clip, dehalo_ref, planes=func.norm_planes)
     dehalo = dehalo.std.MaskedMerge(dehalo_min, dehalo_mask, func.norm_planes)
 
     if isinstance(dampen, tuple):
```

### Comparing `vsdehalo-1.7.0/vsdehalo/denoise.py` & `vsdehalo-1.7.1/vsdehalo/denoise.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.0/vsdehalo/mask.py` & `vsdehalo-1.7.1/vsdehalo/mask.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.0/vsdehalo/vine.py` & `vsdehalo-1.7.1/vsdehalo/vine.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 """
 from __future__ import annotations
 
 from functools import partial
 from math import log
 from typing import Any
 
-from vsdenoise import CCDMode, CCDPoints, MotionMode, MVTools, PelType, Prefilter, SearchMode, ccd, nl_means
+from vsdenoise import (
+    CCDMode, CCDPoints, MotionMode, MVTools, PelType, Prefilter, SearchMode, ccd, frequency_merge, nl_means
+)
 from vsexprtools import ExprOp, norm_expr_planes
 from vskernels import Bicubic
 from vsmasktools import Morpho
-from vsrgtools import contrasharpening_dehalo, gauss_blur, gauss_fmtc_blur, lehmer_diff_merge
+from vsrgtools import contrasharpening_dehalo, gauss_blur, gauss_fmtc_blur
 from vstools import (
     CustomIndexError, CustomRuntimeError, MatrixT, PlanesT, ResampleUtil, check_ref_clip, check_variable, core, get_y,
     join, normalize_planes, split, vs
 )
 
 from .alpha import fine_dehalo
 
@@ -118,16 +120,16 @@
 
     if aggressive:
         clean = core.std.Expr(
             [blur_func(work_clip), clean, blur_func(clean)],
             norm_expr_planes(work_clip, 'y z - x +', planes)
         )
     else:
-        clean = lehmer_diff_merge(
-            gauss_blur(work_clip, 0.5), clean, blur_func, planes=planes  # type: ignore
+        clean = frequency_merge(
+            gauss_blur(work_clip, 0.5), clean, lowpass=blur_func, planes=planes  # type: ignore
         )
 
     diff = work_clip.std.MakeDiff(clean, planes)
 
     diff = nl_means(diff, h_smoothine, 0, sr, 1, planes=planes, rclip=clean)
 
     smooth = clean.std.MergeDiff(diff, planes)
```

### Comparing `vsdehalo-1.7.0/vsdehalo/warp.py` & `vsdehalo-1.7.1/vsdehalo/warp.py`

 * *Files identical despite different names*

### Comparing `vsdehalo-1.7.0/vsdehalo.egg-info/PKG-INFO` & `vsdehalo-1.7.1/vsdehalo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdehalo
-Version: 1.7.0
+Version: 1.7.1
 Summary: Collection of dehaloing VapourSynth functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-dehalo
 Project-URL: Documentation, https://vsdehalo.encode.moe/en/latest/
```

