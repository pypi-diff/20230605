# Comparing `tmp/vsrgtools-1.4.4.tar.gz` & `tmp/vsrgtools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsrgtools-1.4.4.tar", last modified: Thu May  4 21:57:54 2023, max compression
+gzip compressed data, was "vsrgtools-1.5.0.tar", last modified: Mon Jun  5 14:00:51 2023, max compression
```

## Comparing `vsrgtools-1.4.4.tar` & `vsrgtools-1.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/vsrgtools/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/vsrgtools/aka_expr/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/aka_expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/aka_expr/_rg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/aka_expr/_rp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/bilateral.cu
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/contra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/freqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/rgtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/sharp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/vsrgtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/vsrgtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/vsrgtools/aka_expr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/aka_expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/aka_expr/_rg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/aka_expr/_rp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/bilateral.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/contra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/freqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/rgtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/sharp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-05 14:00:30.000000 vsrgtools-1.5.0/vsrgtools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:51.233498 vsrgtools-1.5.0/vsrgtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 14:00:51.000000 vsrgtools-1.5.0/vsrgtools.egg-info/top_level.txt
```

### Comparing `vsrgtools-1.4.4/LICENSE` & `vsrgtools-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/PKG-INFO` & `vsrgtools-1.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsrgtools
-Version: 1.4.4
+Version: 1.5.0
 Summary: Wrapper for RGVS, RGSF, and various other functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-rgtools
 Project-URL: Documentation, https://vsrgtools.encode.moe/en/latest/
```

### Comparing `vsrgtools-1.4.4/setup.cfg` & `vsrgtools-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/setup.py` & `vsrgtools-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/vsrgtools/aka_expr/__init__.py` & `vsrgtools-1.5.0/vsrgtools/aka_expr/__init__.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/vsrgtools/aka_expr/_rg.py` & `vsrgtools-1.5.0/vsrgtools/aka_expr/_rg.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/vsrgtools/aka_expr/_rp.py` & `vsrgtools-1.5.0/vsrgtools/aka_expr/_rp.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/vsrgtools/bilateral.cu` & `vsrgtools-1.5.0/vsrgtools/bilateral.cu`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/vsrgtools/blur.py` & `vsrgtools-1.5.0/vsrgtools/blur.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,33 +5,30 @@
 from math import e, log, log2, sqrt
 from typing import Any
 
 from vsexprtools import ExprOp, ExprVars, complexpr_available, norm_expr
 from vspyplugin import FilterMode, ProcessMode, PyPluginCuda
 from vstools import (
     ConvMode, CustomNotImplementedError, CustomOverflowError, CustomValueError, FuncExceptT, FunctionUtil,
-    NotFoundEnumValue, PlanesT, StrList, check_variable, core, depth, disallow_variable_format,
-    disallow_variable_resolution, fallback, get_depth, get_neutral_value, join, normalize_planes, normalize_seq, split,
-    to_arr, vs
+    NotFoundEnumValue, PlanesT, StrList, check_variable, core, depth, fallback, get_depth, get_neutral_value, join,
+    normalize_planes, normalize_seq, split, to_arr, vs
 )
 
 from .enum import BlurMatrix, LimitFilterMode
 from .limit import limit_filter
 from .util import normalize_radius
 
 __all__ = [
     'blur', 'box_blur', 'side_box_blur',
     'gauss_blur', 'gauss_fmtc_blur',
     'min_blur', 'sbr', 'median_blur',
     'bilateral'
 ]
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def blur(
     clip: vs.VideoNode, radius: int | list[int] = 1, mode: ConvMode = ConvMode.SQUARE, planes: PlanesT = None
 ) -> vs.VideoNode:
     assert check_variable(clip, blur)
 
     planes = normalize_planes(clip, planes)
 
@@ -55,47 +52,46 @@
         matrix = matrix3
     else:
         raise CustomNotImplementedError('This radius isn\'t supported!', blur)
 
     return clip.std.Convolution(matrix, planes=planes, mode=mode)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def box_blur(clip: vs.VideoNode, radius: int | list[int] = 1, passes: int = 1, planes: PlanesT = None) -> vs.VideoNode:
     assert check_variable(clip, box_blur)
 
     planes = normalize_planes(clip, planes)
 
     if isinstance(radius, list):
         return normalize_radius(clip, box_blur, radius, planes, passes=passes)
 
+    if not radius:
+        return clip
+
     if radius > 12:
         blurred = clip.std.BoxBlur(planes, radius, passes, radius, passes)
     else:
         matrix_size = radius * 2 | 1
         blurred = clip
         for _ in range(passes):
             blurred = blurred.std.Convolution(
                 [1] * matrix_size, planes=planes, mode=ConvMode.SQUARE
             )
 
     return blurred
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def side_box_blur(
     clip: vs.VideoNode, radius: int | list[int] = 1, planes: PlanesT = None,
-    inverse: bool = False, expr: bool | None = None
+    inverse: bool = False
 ) -> vs.VideoNode:
     planes = normalize_planes(clip, planes)
 
     if isinstance(radius, list):
-        return normalize_radius(clip, side_box_blur, radius, planes, inverse=inverse, expr=expr)
+        return normalize_radius(clip, side_box_blur, radius, planes, inverse=inverse)
 
     half_kernel = [(1 if i <= 0 else 0) for i in range(-radius, radius + 1)]
 
     conv_m1 = partial(core.std.Convolution, matrix=half_kernel, planes=planes)
     conv_m2 = partial(core.std.Convolution, matrix=half_kernel[::-1], planes=planes)
     blur_pt = partial(core.std.BoxBlur, planes=planes)
 
@@ -113,15 +109,15 @@
         hrz_flt(vrt_intermediate)
         for i, vrt_intermediate in enumerate(vrt_intermediates)
         for j, hrz_flt in enumerate(hrz_filters) if not i == j == 2
     )
 
     comp_blur = None if inverse else box_blur(clip, radius, 1, planes)
 
-    if complexpr_available if expr is None else expr:
+    if complexpr_available:
         template = '{cum} x - abs {new} x - abs < {cum} {new} ?'
 
         cum_expr, cumc = '', 'y'
         n_inter = len(intermediates)
 
         for i, newc, var in zip(count(), ExprVars[2:26], ExprVars[4:26]):
             if i == n_inter - 1:
@@ -165,16 +161,14 @@
 
     if sigma >= min(clip.width, clip.height):
         raise CustomOverflowError("Sigma can't be bigger or equal than the smaller size of the clip!", func)
 
     return sigma
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def gauss_blur(
     clip: vs.VideoNode,
     sigma: float | list[float] | None = 0.5, sharp: float | list[float] | None = None,
     mode: ConvMode = ConvMode.SQUARE, planes: PlanesT = None
 ) -> vs.VideoNode:
     assert check_variable(clip, gauss_blur)
 
@@ -192,16 +186,14 @@
 
     if sigma <= 4.333:
         return BlurMatrix.gauss(sigma)(clip, planes, mode)
 
     return gauss_fmtc_blur(clip, sigma, sharp, True, mode, planes)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def gauss_fmtc_blur(
     clip: vs.VideoNode,
     sigma: float | list[float] | None = 0.5, sharp: float | list[float] | None = None,
     strict: bool = True, mode: ConvMode = ConvMode.SQUARE, planes: PlanesT = None
 ) -> vs.VideoNode:
     assert check_variable(clip, gauss_fmtc_blur)
 
@@ -236,25 +228,23 @@
             down = clip.fmtc.resample(
                 clip.width * 2, clip.height * 2, kernel='gauss', a1=sharp
             )
             down = down.fmtc.resample(clip.width, clip.height, kernel='gauss', a1=sigma)
 
             return depth(down, clip)
 
-    if not {*range(clip.format.num_planes)} - {*planes}:  # type: ignore
+    if not {*range(clip.format.num_planes)} - {*planes}:
         return _fmtc_blur(clip)
 
     return join([
-        _fmtc_blur(p) if i in planes else p  # type: ignore
+        _fmtc_blur(p) if i in planes else p
         for i, p in enumerate(split(clip))
     ])
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def min_blur(clip: vs.VideoNode, radius: int | list[int] = 1, planes: PlanesT = None) -> vs.VideoNode:
     """
     MinBlur by Didée (http://avisynth.nl/index.php/MinBlur)
     Nifty Gauss/Median combination
     """
     assert check_variable(clip, min_blur)
 
@@ -272,16 +262,14 @@
         weighted = blur(clip, radius)
     else:
         weighted = sbr(clip, planes=planes)
 
     return limit_filter(weighted, clip, median, LimitFilterMode.DIFF_MIN, planes)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def sbr(
     clip: vs.VideoNode,
     radius: int | list[int] = 1, mode: ConvMode = ConvMode.SQUARE,
     planes: PlanesT = None
 ) -> vs.VideoNode:
     assert check_variable(clip, sbr)
```

### Comparing `vsrgtools-1.4.4/vsrgtools/contra.py` & `vsrgtools-1.5.0/vsrgtools/contra.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 
 from functools import partial
 from inspect import Signature
 from typing import Callable
 
 from vsexprtools import complexpr_available, norm_expr
 from vstools import (
-    CustomValueError, GenericVSFunction, PlanesT, check_ref_clip, check_variable, clamp_arr, disallow_variable_format,
-    disallow_variable_resolution, get_neutral_value, iterate, normalize_planes, to_arr, vs
+    CustomValueError, GenericVSFunction, PlanesT, check_ref_clip, check_variable, clamp_arr, get_neutral_value, iterate,
+    normalize_planes, to_arr, vs
 )
 
-from .blur import blur, box_blur, min_blur, median_blur
-from .enum import RemoveGrainMode, RemoveGrainModeT, RepairMode, RepairModeT, BlurMatrix
+from .blur import blur, box_blur, median_blur, min_blur
+from .enum import BlurMatrix, RemoveGrainMode, RemoveGrainModeT, RepairMode, RepairModeT
 from .rgtools import removegrain, repair
 from .util import norm_rmode_planes
 
 __all__ = [
     'contrasharpening', 'contra',
     'contrasharpening_dehalo', 'contra_dehalo',
     'contrasharpening_median', 'contra_median',
     'fine_contra'
 ]
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def contrasharpening(
-    flt: vs.VideoNode, src: vs.VideoNode, radius: int | list[int] | None = None,
+    flt: vs.VideoNode, src: vs.VideoNode, radius: int | list[int] = 1,
     mode: RepairModeT = RepairMode.MINMAX_SQUARE3, planes: PlanesT = 0
 ) -> vs.VideoNode:
     """
     contra-sharpening: sharpen the denoised clip, but don't add more to any pixel than what was previously removed.
     Script by Didée, at the VERY GRAINY thread (http://forum.doom9.org/showthread.php?p=1076491#post1076491)
     :param flt:         Filtered clip
     :param src:         Source clip
@@ -48,15 +46,17 @@
         neutral = [get_neutral_value(flt), get_neutral_value(flt, True)]
     else:
         neutral = [0.0]
 
     planes = normalize_planes(flt, planes)
 
     if radius is None:
-        radius = 2 if flt.width > 1024 or flt.height > 576 else 1
+        import warnings  # type: ignore
+        warnings.warn('contrasharpening: radius=None is deprecated! The function will always default to 1.')
+        radius = 1
 
     # Damp down remaining spots of the denoised clip
     mblur = min_blur(flt, radius, planes)
 
     rg11 = blur(mblur, radius, planes=planes)
 
     # Difference of a simple kernel blur
@@ -74,16 +74,14 @@
         expr = 'x {mid} - LD! y {mid} - BD! LD@ abs BD@ abs < LD@ BD@ ? z +'
     else:
         expr = 'x {mid} - abs y {mid} - abs < x y ? {mid} - z +'
 
     return norm_expr([limit, diff_blur, flt], expr, planes, mid=neutral)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def contrasharpening_dehalo(
     flt: vs.VideoNode, src: vs.VideoNode, level: float = 1.4, alpha: float = 2.49, planes: PlanesT = 0
 ) -> vs.VideoNode:
     """
     :param dehaloed:    Dehaloed clip
     :param src:         Source clip
     :param level:       Strength level
@@ -111,16 +109,14 @@
 
         clips = [diff, src, flt]
         expr = 'x {mid} - y z - xor 0 x {mid} - abs y z - abs < x {mid} - y z - ? ? z +'
 
     return norm_expr(clips, expr, planes, mid=neutral)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def contrasharpening_median(
     flt: vs.VideoNode, src: vs.VideoNode,
     mode: RemoveGrainModeT | Callable[..., vs.VideoNode] = box_blur,
     planes: PlanesT = 0
 ) -> vs.VideoNode:
     """
     :param flt:         Filtered clip
@@ -146,19 +142,17 @@
         expr = 'x dup + z - D! x y < D@ x y clamp D@ y x clamp ?'
     else:
         expr = 'x dup + z - x y min max x y max min'
 
     return norm_expr([flt, src, repaired], expr, planes)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def fine_contra(
     flt: vs.VideoNode, src: vs.VideoNode, sharp: float | list[float] | range = 0.75,
-    radius: int | list[int] | None = None, merge_func: GenericVSFunction | None = None,
+    radius: int | list[int] = 1, merge_func: GenericVSFunction | None = None,
     mode: RepairModeT = RepairMode.MINMAX_SQUARE_REF3, planes: PlanesT = 0
 ) -> vs.VideoNode:
     """
     :param flt:         Filtered clip.
     :param src:         Source clip.
     :param sharp:       Contrast Adaptive Sharpening's sharpening strength.
                         If it's a list, depending on ``merge_func`` being ``None``,
@@ -178,15 +172,17 @@
         neutral = [get_neutral_value(flt), get_neutral_value(flt, True)]
     else:
         neutral = [0.0]
 
     planes = normalize_planes(flt, planes)
 
     if radius is None:
-        radius = 2 if flt.width > 1024 or flt.height > 576 else 1
+        import warnings  # type: ignore
+        warnings.warn('fine_contra: radius=None is deprecated! The function will always default to 1.')
+        radius = 1
 
     mblur = min_blur(flt, radius, planes)
 
     sharp = [1.0 / x for x in sharp if x] if isinstance(sharp, range) else to_arr(sharp)
     sharp = clamp_arr(sharp, 0.0, 1.0)
 
     if merge_func is None:
```

### Comparing `vsrgtools-1.4.4/vsrgtools/enum.py` & `vsrgtools-1.5.0/vsrgtools/enum.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/vsrgtools/func.py` & `vsrgtools-1.5.0/vsrgtools/func.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from __future__ import annotations
 
 from typing import Iterable
 
 from vsexprtools import ExprOp, ExprVars, complexpr_available, norm_expr
 from vstools import (
-    CustomIndexError, CustomOverflowError, PlanesT, VSFunction, check_variable, core, disallow_variable_format,
-    disallow_variable_resolution, fallback, flatten, get_neutral_value, normalize_planes, vs
+    CustomIndexError, CustomOverflowError, PlanesT, VSFunction, check_variable, core, fallback, flatten,
+    get_neutral_value, normalize_planes, vs
 )
 
 from .enum import LimitFilterMode
 from .limit import limit_filter
 
 __all__ = [
     'minimum_diff', 'median_diff',
     'median_clips',
     'flux_smooth'
 ]
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def minimum_diff(
     clip: vs.VideoNode,
     clip_func: VSFunction, diff_func: VSFunction | None = None,
     diff: bool | None = None, planes: PlanesT = None
 ) -> vs.VideoNode:
     planes = normalize_planes(clip, planes)
 
@@ -39,32 +37,28 @@
     diffa = core.std.MakeDiff(clip, filtered, planes)
 
     diffb = diff_func(diffa)
 
     return median_diff(clip, diffa, diffb, planes)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def median_diff(clip: vs.VideoNode, diffa: vs.VideoNode, diffb: vs.VideoNode, planes: PlanesT = None) -> vs.VideoNode:
     assert check_variable(clip, median_diff)
 
     planes = normalize_planes(clip, planes)
     neutral = [get_neutral_value(clip), get_neutral_value(clip, True)]
 
     if complexpr_available:
         expr = 'y z - D! x D@ y {mid} clamp D@ {mid} y clamp - -'
     else:
         expr = 'x y z - y min {mid} max y z - {mid} min y max - -'
 
     return norm_expr([clip, diffa, diffb], expr, planes, mid=neutral)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def median_clips(*_clips: vs.VideoNode | Iterable[vs.VideoNode], planes: PlanesT = None) -> vs.VideoNode:
     clips = list[vs.VideoNode](flatten(_clips))  # type: ignore
     n_clips = len(clips)
 
     if not complexpr_available and n_clips > 26:
         raise CustomOverflowError('You can pass only up to 26 clips without akarin Expr!', median_clips, reason=n_clips)
     elif n_clips < 3:
@@ -87,25 +81,23 @@
         yzmin, yzmax = 'YZMIN@', 'YZMAX@'
 
     expr = f'{header} x {yzmin} min x = {yzmin} x {yzmax} max x = {yzmax} x ? ?'
 
     return norm_expr(clips, expr, planes)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def flux_smooth(
     clip: vs.VideoNode, radius: int = 2, threshold: int = 7, scenechange: int = 24, planes: PlanesT = None
 ) -> vs.VideoNode:
     assert check_variable(clip, flux_smooth)
 
     if radius < 1 or radius > 7:
         raise CustomIndexError('Radius must be between 1 and 7 (inclusive)!', flux_smooth, reason=radius)
 
-    planes = normalize_planes(clip, planes, False)
+    planes = normalize_planes(clip, planes)
 
     threshold = threshold << clip.format.bits_per_sample - 8
 
     cthreshold = threshold if (1 in planes or 2 in planes) else 0
 
     median = clip.tmedian.TemporalMedian(radius, planes)  # type: ignore
     average = clip.focus2.TemporalSoften2(  # type: ignore
```

### Comparing `vsrgtools-1.4.4/vsrgtools/limit.py` & `vsrgtools-1.5.0/vsrgtools/limit.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/vsrgtools/rgtools.py` & `vsrgtools-1.5.0/vsrgtools/rgtools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from __future__ import annotations
 
 from vsexprtools import complexpr_available, expr_func
-from vstools import (
-    NotFoundEnumValue, PlanesT, check_variable, core, disallow_variable_format, disallow_variable_resolution,
-    normalize_seq, pick_func_stype, vs
-)
+from vstools import NotFoundEnumValue, PlanesT, check_variable, core, normalize_seq, pick_func_stype, vs
 
 from .aka_expr import (
     aka_removegrain_expr_11_12, aka_removegrain_expr_19, aka_removegrain_expr_20, aka_removegrain_expr_23,
     aka_removegrain_expr_24, removegrain_aka_exprs, repair_aka_exprs
 )
-from .enum import RemoveGrainMode, RemoveGrainModeT, RepairMode, RepairModeT, VerticalCleanerModeT, BlurMatrix
+from .enum import BlurMatrix, RemoveGrainMode, RemoveGrainModeT, RepairMode, RepairModeT, VerticalCleanerModeT
 
 __all__ = [
     'repair', 'removegrain',
     'clense', 'backward_clense', 'forward_clense',
     'vertical_cleaner', 'horizontal_cleaner'
 ]
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def repair(clip: vs.VideoNode, repairclip: vs.VideoNode, mode: RepairModeT) -> vs.VideoNode:
     assert check_variable(clip, repair)
     assert check_variable(repairclip, repair)
 
     is_float = clip.format.sample_type == vs.FLOAT
     mode = normalize_seq(mode, clip.format.num_planes)
 
@@ -40,16 +35,14 @@
         return pick_func_stype(clip, core.rgvs.Repair, core.rgsf.Repair)(clip, repairclip, mode)
 
     return core.akarin.Expr(
         [clip, repairclip], [repair_aka_exprs[m]() for m in mode], clip.format.id, True
     )
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def removegrain(clip: vs.VideoNode, mode: RemoveGrainModeT) -> vs.VideoNode:
     assert check_variable(clip, removegrain)
 
     mode = normalize_seq(mode, clip.format.num_planes)
     mode = list(map(RemoveGrainMode, mode))
 
     if not sum(mode):
@@ -84,39 +77,29 @@
             expr.append(aka_removegrain_expr_24(0 if idx == 0 else -0.5))
         else:
             expr.append(removegrain_aka_exprs[m]())
 
     return expr_func(clip, expr, opt=True)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def clense(
     clip: vs.VideoNode,
     previous_clip: vs.VideoNode | None = None, next_clip: vs.VideoNode | None = None,
     planes: PlanesT = None
 ) -> vs.VideoNode:
     return pick_func_stype(clip, clip.rgvs.Clense, clip.rgsf.Clense)(previous_clip, next_clip, planes)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def forward_clense(clip: vs.VideoNode, planes: PlanesT = None) -> vs.VideoNode:
     return pick_func_stype(clip, clip.rgvs.ForwardClense, clip.rgsf.ForwardClense)(planes)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def backward_clense(clip: vs.VideoNode, planes: PlanesT = None) -> vs.VideoNode:
     return pick_func_stype(clip, clip.rgvs.BackwardClense, clip.rgsf.BackwardClense)(planes)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def vertical_cleaner(clip: vs.VideoNode, mode: VerticalCleanerModeT) -> vs.VideoNode:
     return pick_func_stype(clip, clip.rgvs.VerticalCleaner, clip.rgsf.VerticalCleaner)(mode)
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def horizontal_cleaner(clip: vs.VideoNode, mode: VerticalCleanerModeT) -> vs.VideoNode:
     return vertical_cleaner(clip.std.Transpose(), mode).std.Transpose()
```

### Comparing `vsrgtools-1.4.4/vsrgtools/sharp.py` & `vsrgtools-1.5.0/vsrgtools/sharp.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/vsrgtools/util.py` & `vsrgtools-1.5.0/vsrgtools/util.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.4/vsrgtools.egg-info/PKG-INFO` & `vsrgtools-1.5.0/vsrgtools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsrgtools
-Version: 1.4.4
+Version: 1.5.0
 Summary: Wrapper for RGVS, RGSF, and various other functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-rgtools
 Project-URL: Documentation, https://vsrgtools.encode.moe/en/latest/
```

### Comparing `vsrgtools-1.4.4/vsrgtools.egg-info/SOURCES.txt` & `vsrgtools-1.5.0/vsrgtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

