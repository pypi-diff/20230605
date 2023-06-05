# Comparing `tmp/vsdenoise-2.2.0.tar.gz` & `tmp/vsdenoise-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdenoise-2.2.0.tar", last modified: Thu May  4 21:59:13 2023, max compression
+gzip compressed data, was "vsdenoise-2.3.0.tar", last modified: Mon Jun  5 14:32:33 2023, max compression
```

## Comparing `vsdenoise-2.2.0.tar` & `vsdenoise-2.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:13.583131 vsdenoise-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 21:59:13.583131 vsdenoise-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 21:59:13.583131 vsdenoise-2.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1507 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:13.579131 vsdenoise-2.2.0/vsdenoise/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/blockmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/bm3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/deblock.py
--rw-r--r--   0 runner    (1001) docker     (123)    22664 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/knlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/limit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:13.583131 vsdenoise-2.2.0/vsdenoise/mvtools/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/mvtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/mvtools/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/mvtools/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    42255 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/mvtools/mvtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/mvtools/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/mvtools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    41360 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/prefilters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/regress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-04 21:58:45.000000 vsdenoise-2.2.0/vsdenoise/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:13.583131 vsdenoise-2.2.0/vsdenoise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 21:59:13.000000 vsdenoise-2.2.0/vsdenoise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-04 21:59:13.000000 vsdenoise-2.2.0/vsdenoise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:59:13.000000 vsdenoise-2.2.0/vsdenoise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-04 21:59:13.000000 vsdenoise-2.2.0/vsdenoise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 21:59:13.000000 vsdenoise-2.2.0/vsdenoise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:33.118652 vsdenoise-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-05 14:32:33.118652 vsdenoise-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-05 14:32:33.118652 vsdenoise-2.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1507 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:33.114652 vsdenoise-2.3.0/vsdenoise/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/blockmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/bm3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/deblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23153 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/freqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/limit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:33.118652 vsdenoise-2.3.0/vsdenoise/mvtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46432 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/mvtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/mvtools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/nlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41315 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/prefilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/regress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-05 14:32:08.000000 vsdenoise-2.3.0/vsdenoise/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:33.114652 vsdenoise-2.3.0/vsdenoise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 14:32:33.000000 vsdenoise-2.3.0/vsdenoise.egg-info/top_level.txt
```

### Comparing `vsdenoise-2.2.0/LICENSE` & `vsdenoise-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/PKG-INFO` & `vsdenoise-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdenoise
-Version: 2.2.0
+Version: 2.3.0
 Summary: VapourSynth denoising functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-denoise
 Project-URL: Documentation, https://vsdenoise.encode.moe/en/latest/
@@ -34,8 +34,31 @@
 ```
 
 Or if you want the latest git version, install it with this command:
 
 ```sh
 $ pip install git+https://github.com/Irrational-Encoding-Wizardry/vs-denoise.git
 ```
-<br>
+<br><br>
+
+## Example usage
+```py
+from vsdenoise import MVTools, SADMode, MotionMode, Prefilter, BM3DCuda, Profile, nl_means
+
+clip = ...
+
+ref = MVTools.denoise(
+    clip, thSAD=100, block_size=32, overlap=16,
+    motion=MotionMode.HIGH_SAD,
+    prefilter=Prefilter.DFTTEST,
+    sad_mode=(
+        SADMode.ADAPTIVE_SPATIAL_MIXED,
+        SADMode.ADAPTIVE_SATD_MIXED,
+    )
+)
+
+denoise = BM3DCuda.denoise(
+    clip, sigma=0.8, tr=2, profile=Profile.NORMAL, ref=ref, planes=0
+)
+
+denoise = nl_means(denoise, tr=2, strength=0.6, ref=ref, planes=[1, 2])
+```
```

### Comparing `vsdenoise-2.2.0/setup.cfg` & `vsdenoise-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/setup.py` & `vsdenoise-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/vsdenoise/bm3d.py` & `vsdenoise-2.3.0/vsdenoise/bm3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,29 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Literal, NamedTuple, final, overload
 
 from vstools import (
-    ColorRange, ColorRangeT, Colorspace, ConstantFormatVideoNode, CustomIndexError, CustomStrEnum, CustomValueError,
-    DitherType, FuncExceptT, KwargsT, Matrix, MatrixT, Self, SingleOrArr, check_variable, core, depth, get_video_format,
-    join, normalize_seq, vs, vs_object
+    MISSING, ColorRange, ColorRangeT, Colorspace, ConstantFormatVideoNode, CustomIndexError, CustomRuntimeError,
+    CustomStrEnum, CustomValueError, DitherType, FuncExceptT, FunctionUtil, KwargsT, Matrix, MatrixT, MissingT, PlanesT,
+    Self, SingleOrArr, check_variable, core, depth, get_video_format, get_y, join, normalize_seq, vs, vs_object
 )
 
 from .types import _Plugin_bm3dcpu_Core_Bound, _Plugin_bm3dcuda_Core_Bound, _Plugin_bm3dcuda_rtc_Core_Bound
 
 __all__ = [
     'Profile',
-    'BM3D', 'BM3DCuda', 'BM3DCudaRTC', 'BM3DCPU'
+
+    'BM3D',
+
+    'BM3DMawen',
+
+    'BM3DCuda', 'BM3DCudaRTC', 'BM3DCPU'
 ]
 
 
 @dataclass
 class BM3DColorspaceConfig:
     csp: Colorspace
     clip: ConstantFormatVideoNode
@@ -277,15 +282,15 @@
 
 class AbstractBM3D(vs_object):
     """Abstract BM3D-based denoiser interface."""
 
     wclip: vs.VideoNode
 
     sigma: _Sigma
-    radius: _Radius
+    tr: _TemporalRadius
     profile: Profile.Config
 
     ref: vs.VideoNode | None
 
     refine: int
 
     cspconfig: BM3DColorspaceConfig
@@ -297,28 +302,28 @@
     """Custom kwargs passed to bm3d for the :py:attr:`final` clip."""
 
     class _Sigma(NamedTuple):
         y: float
         u: float
         v: float
 
-    class _Radius(NamedTuple):
+    class _TemporalRadius(NamedTuple):
         basic: int
         final: int
 
     def __init__(
-        self, clip: vs.VideoNode, sigma: SingleOrArr[float], radius: SingleOrArr[int] | None = None,
+        self, clip: vs.VideoNode, sigma: SingleOrArr[float] = 0.5, tr: SingleOrArr[int] | None = None,
         profile: Profile | Profile.Config = Profile.FAST, ref: vs.VideoNode | None = None, refine: int = 1,
         matrix: MatrixT | None = None, range_in: ColorRangeT | None = None,
-        colorspace: Colorspace | None = None, fp32: bool = True
+        colorspace: Colorspace | None = None, fp32: bool = True, *, radius: SingleOrArr[int] | MissingT = MISSING
     ) -> None:
         """
         :param clip:            Source clip.
         :param sigma:           Strength of denoising, valid range is [0, +inf].
-        :param radius:          Temporal radius, valid range is [1, 16].
+        :param tr:              Temporal radius, valid range is [1, 16].
         :param profile:         Preset profile. See :py:attr:`vsdenoise.bm3d.Profile`.
                                 Default: Profile.FAST.
         :param ref:             Reference clip used in block-matching, replacing the basic estimation.
                                 If not specified, the input clip is used instead.
                                 Default: None.
         :param refine:          The number of times to refine the estimation.
                                  * 1 means basic estimate with one final estimate.
@@ -332,16 +337,21 @@
         :param range_in:        Enum for the color range of the input clip.
                                 See :py:attr:`vstools.enums.ColorRange` for more info.
                                 If not specified, gets the color from the "_ColorRange" prop of the clip.
                                 This check is not performed if the input clip is float.
         """
         assert check_variable(clip, self.__class__)
 
+        if radius is not MISSING:
+            import warnings
+            warnings.warn(f'{self.__class__.__name__}: radius is deprecated and will be removed. Use tr')
+            tr = radius
+
         self.sigma = self._Sigma(*normalize_seq(sigma, 3))
-        self.radius = self._Radius(*normalize_seq(radius or 0, 2))
+        self.tr = self._TemporalRadius(*normalize_seq(tr or 0, 2))
 
         _is_gray = clip.format.color_family == vs.GRAY
 
         if _is_gray:
             self.sigma = self.sigma._replace(u=0, v=0)
         elif sum(self.sigma[1:]) == 0:
             _is_gray = True
@@ -393,60 +403,77 @@
         :param ref:     Reference clip used for weight calculations.
 
         :return:        Final, refined, denoised clip.
         """
 
     @classmethod
     def denoise(
-        cls, clip: vs.VideoNode, sigma: SingleOrArr[float], radius: SingleOrArr[int] | None = None,
+        cls, clip: vs.VideoNode, sigma: SingleOrArr[float] = 0.5, tr: SingleOrArr[int] | None = None,
         refine: int = 1, profile: Profile | Profile.Config = Profile.FAST, ref: vs.VideoNode | None = None,
         matrix: MatrixT | None = None, range_in: ColorRangeT | None = None,
-        colorspace: Colorspace | None = None, fp32: bool = True
+        colorspace: Colorspace | None = None, fp32: bool = True, planes: PlanesT = None, **kwargs: Any
     ) -> vs.VideoNode:
-        return cls(clip, sigma, radius, profile, ref, refine, matrix, range_in, colorspace, fp32).final()
+        func = FunctionUtil(clip, cls.denoise, planes)
+
+        sigma = func.norm_seq(sigma)
+
+        ref = get_y(ref) if func.luma_only and ref else ref
+
+        bm3d = cls(func.work_clip, sigma, tr, profile, ref, refine, matrix, range_in, colorspace, fp32, **kwargs)
+
+        if refine:
+            denoise = bm3d.final()
+        else:
+            denoise = bm3d.basic(
+                bm3d.cspconfig.get_clip(bm3d.cspconfig.clip, bm3d._pre_clip, None)
+            )
+
+        return func.return_clip(denoise)
 
     def __post_init__(self) -> None:
+        super().__post_init__()
+
         self._pre_clip = self.cspconfig.prepare_clip(self.cspconfig.clip)
         self._pre_ref = self.cspconfig.prepare_clip(self.ref)
 
-        return super().__post_init__()
-
     def __vs_del__(self, core_id: int) -> None:
         del self.cspconfig, self.ref
+
         self.basic_args.clear()
         self.final_args.clear()
 
 
-class BM3D(AbstractBM3D):
+class BM3DMawen(AbstractBM3D):
     """BM3D implementation by mawen1250."""
 
     def __init__(
-        self, clip: vs.VideoNode, sigma: SingleOrArr[float], radius: SingleOrArr[int] | None = None,
+        self, clip: vs.VideoNode, sigma: SingleOrArr[float] = 0.5, tr: SingleOrArr[int] | None = None,
         profile: Profile | Profile.Config = Profile.FAST, pre: vs.VideoNode | None = None,
         ref: vs.VideoNode | None = None, refine: int = 1, matrix: MatrixT | None = None,
-        range_in: ColorRangeT | None = None, colorspace: Colorspace | None = None, fp32: bool = True
+        range_in: ColorRangeT | None = None, colorspace: Colorspace | None = None, fp32: bool = True,
+        *, radius: SingleOrArr[int] | MissingT = MISSING
     ) -> None:
-        self.pre = pre and self.cspconfig.check_clip(pre, matrix, range_in, self.__class__)
+        super().__init__(clip, sigma, tr, profile, ref, refine, matrix, range_in, colorspace, fp32, radius=radius)
 
-        super().__init__(clip, sigma, radius, profile, ref, refine, matrix, range_in, colorspace, fp32)
+        self.pre = pre and self.cspconfig.check_clip(pre, matrix, range_in, self.__class__)
 
     def __post_init__(self) -> None:
-        self._pre_pre = self.cspconfig.prepare_clip(self.pre)
+        super().__post_init__()
 
-        return super().__post_init__()
+        self._pre_pre = self.cspconfig.prepare_clip(self.pre)
 
     def basic(self, clip: vs.VideoNode | None = None, opp: bool = False) -> vs.VideoNode:
         clip = self.cspconfig.get_clip(self.cspconfig.clip, self._pre_clip, clip)
 
         kwargs = KwargsT(ref=self.pre, sigma=self.sigma, matrix=100, args=self.basic_args)
 
-        if self.radius.basic:
-            clip = clip.bm3d.VBasic(**self.profile.as_dict(**kwargs, radius=self.radius.basic))  # type: ignore
+        if self.tr.basic:
+            clip = clip.bm3d.VBasic(**self.profile.as_dict(**kwargs, radius=self.tr.basic))  # type: ignore
 
-            clip = clip.bm3d.VAggregate(self.radius.basic, self.cspconfig.fp32)
+            clip = clip.bm3d.VAggregate(self.tr.basic, self.cspconfig.fp32)
         else:
             clip = clip.bm3d.Basic(**self.profile.as_dict(**kwargs))  # type: ignore
 
         return clip if opp else self.cspconfig.post_processing(clip)
 
     def final(
         self, clip: vs.VideoNode | None = None, ref: vs.VideoNode | None = None, refine: int | None = None
@@ -457,17 +484,17 @@
             ref = self.cspconfig.get_clip(self.ref, self._pre_ref, ref)
         else:
             ref = self.basic(clip, True)
 
         kwargs = KwargsT(ref=ref, sigma=self.sigma, matrix=100, args=self.final_args)
 
         for _ in range(refine or self.refine):
-            if self.radius.final:
-                clip = clip.bm3d.VFinal(**self.profile.as_dict(**kwargs, radius=self.radius.final))  # type: ignore
-                clip = clip.bm3d.VAggregate(self.radius.final, self.cspconfig.fp32)
+            if self.tr.final:
+                clip = clip.bm3d.VFinal(**self.profile.as_dict(**kwargs, radius=self.tr.final))  # type: ignore
+                clip = clip.bm3d.VAggregate(self.tr.final, self.cspconfig.fp32)
             else:
                 clip = clip.bm3d.Final(**self.profile.as_dict(**kwargs))  # type: ignore
 
         return self.cspconfig.post_processing(clip)
 
 
 class AbstractBM3DCudaMeta(ABCMeta):
@@ -484,57 +511,80 @@
 
     plugin: _Plugin_bm3dcuda_Core_Bound | _Plugin_bm3dcuda_rtc_Core_Bound | _Plugin_bm3dcpu_Core_Bound
 
     def basic(self, clip: vs.VideoNode | None = None, opp: bool = False) -> vs.VideoNode:
         clip = self.cspconfig.get_clip(self.cspconfig.clip, self._pre_clip, clip)
 
         kwargs = self.profile.as_dict(
-            self.plugin, True, False, self.basic_args, sigma=self.sigma, radius=self.radius.basic
+            self.plugin, True, False, self.basic_args, sigma=self.sigma, radius=self.tr.basic
         )
 
         if hasattr(self.plugin, 'BM3Dv2'):
             clip = self.plugin.BM3Dv2(clip, **kwargs)
         else:
             clip = self.plugin.BM3D(clip, **kwargs)
 
-            if self.radius.basic:
-                clip = clip.bm3d.VAggregate(self.radius.basic, self.cspconfig.fp32)
+            if self.tr.basic:
+                clip = clip.bm3d.VAggregate(self.tr.basic, self.cspconfig.fp32)
 
         return clip if opp else self.cspconfig.post_processing(clip)
 
     def final(
         self, clip: vs.VideoNode | None = None, ref: vs.VideoNode | None = None, refine: int | None = None
     ) -> vs.VideoNode:
         clip = self.cspconfig.get_clip(self.cspconfig.clip, self._pre_clip, clip)
 
         if self.ref and self._pre_ref:
             ref = self.cspconfig.get_clip(self.ref, self._pre_ref, ref)
         else:
             ref = self.basic(clip, True)
 
         kwargs = self.profile.as_dict(
-            self.plugin, False, True, self.final_args, sigma=self.sigma, radius=self.radius.final
+            self.plugin, False, True, self.final_args, sigma=self.sigma, radius=self.tr.final
         )
 
         if hasattr(self.plugin, 'BM3Dv2'):
             for _ in range(refine or self.refine):
                 clip = self.plugin.BM3Dv2(clip, ref, **kwargs)
         else:
             for _ in range(refine or self.refine):
                 clip = self.plugin.BM3D(clip, ref, **kwargs)
 
-                if self.radius.final:
-                    clip = clip.bm3d.VAggregate(self.radius.final, self.cspconfig.fp32)
+                if self.tr.final:
+                    clip = clip.bm3d.VAggregate(self.tr.final, self.cspconfig.fp32)
 
         return self.cspconfig.post_processing(clip)
 
 
 class BM3DCuda(AbstractBM3DCuda, plugin=core.lazy.bm3dcuda):
     ...
 
 
 class BM3DCudaRTC(AbstractBM3DCuda, plugin=core.lazy.bm3dcuda_rtc):
     ...
 
 
 class BM3DCPU(AbstractBM3DCuda, plugin=core.lazy.bm3dcpu):
     ...
+
+
+class AutoBM3DMeta(ABCMeta):
+    def __new__(
+        __mcls: type[Self], __name: str, __bases: tuple[type, ...], __namespace: dict[str, Any], **kwargs: Any
+    ) -> type[AbstractBM3D]:
+        if hasattr(core, 'bm3dcuda_rtc'):
+            return BM3DCudaRTC
+
+        if hasattr(core, 'bm3dcuda'):
+            return BM3DCuda
+
+        if hasattr(core, 'bm3dcpu'):
+            return BM3DCPU
+
+        if hasattr(core, 'bm3d'):
+            return BM3DMawen
+
+        raise CustomRuntimeError('You have no bm3d plugin installed!')
+
+
+class BM3D(AbstractBM3D, metaclass=AutoBM3DMeta):
+    ...
```

### Comparing `vsdenoise-2.2.0/vsdenoise/ccd.py` & `vsdenoise-2.3.0/vsdenoise/ccd.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/vsdenoise/deblock.py` & `vsdenoise-2.3.0/vsdenoise/deblock.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Literal, SupportsFloat, cast
+from typing import Any, Literal, SupportsFloat, cast
 
 from vsexprtools import expr_func, norm_expr
 from vskernels import Catrom, Kernel, KernelT, Point
+from vsmasktools import FDoG, GenericMaskT, adg_mask, normalize_mask
+from vsrgtools import gauss_blur
 from vstools import (
-    CustomStrEnum, DependencyNotFoundError, DitherType, FrameRangeN, FrameRangesN, InvalidColorFamilyError, KwargsT,
-    LengthMismatchError, Matrix, MatrixT, UnsupportedVideoFormatError, check_variable, core, depth, fallback, get_depth,
-    get_nvidia_version, get_y, join, replace_ranges, vs
+    ColorRange, CustomStrEnum, DependencyNotFoundError, DitherType, FrameRangeN, FrameRangesN, InvalidColorFamilyError,
+    KwargsT, LengthMismatchError, Matrix, MatrixT, UnsupportedVideoFormatError, check_variable, core, depth, fallback,
+    get_depth, get_nvidia_version, get_y, join, replace_ranges, vs
 )
 
 __all__ = [
-    'dpir',
+    'dpir', 'dpir_mask'
 ]
 
 
 class _dpir(CustomStrEnum):
     DEBLOCK = 'deblock'
     DENOISE = 'denoise'
 
     def __call__(
         self, clip: vs.VideoNode, strength: SupportsFloat | vs.VideoNode | None | tuple[
             SupportsFloat | vs.VideoNode | None, SupportsFloat | vs.VideoNode | None
         ] = 10, matrix: MatrixT | None = None, cuda: bool | Literal['trt'] | None = None, i444: bool = False,
         tiles: int | tuple[int, int] | None = None, overlap: int | tuple[int, int] | None = 8,
         zones: list[tuple[FrameRangeN | FrameRangesN | None, SupportsFloat | vs.VideoNode | None]] | None = None,
-        fp16: bool | None = None, num_streams: int | None = None, device_id: int = 0, kernel: KernelT = Catrom
+        fp16: bool | None = None, num_streams: int | None = None, device_id: int = 0, kernel: KernelT = Catrom,
+        **kwargs: Any
     ) -> vs.VideoNode:
         func = 'dpir'
 
         try:
             from vsmlrt import Backend, DPIRModel, backendT, calc_tilesize, inference, models_path  # type: ignore
         except ModuleNotFoundError as e:
             raise DependencyNotFoundError(func, e)
@@ -220,15 +223,15 @@
                             return dpir_ranges_zones[ranges]
 
                     return strength_clip
 
                 zoned_strength_clip = strength_clip.std.FrameEval(_select_sclip)
 
         backend: backendT
-        bkwargs = KwargsT(fp16=fp16, device_id=device_id)
+        bkwargs = kwargs | KwargsT(fp16=fp16, device_id=device_id)
 
         # All this will eventually be in vs-nn
         if cuda is None or trt_available:
             try:
                 data: KwargsT = core.trt.DeviceProperties(device_id)  # type: ignore
                 memory = data.get('total_global_memory', 0)
                 def_num_streams = data.get('async_engine_count', 1)
@@ -293,7 +296,34 @@
         if is_rgb or is_gray:
             return depth(run_dpir, bit_depth)
 
         return kernel.resample(run_dpir, targ_format, targ_matrix)
 
 
 dpir = _dpir.DEBLOCK
+
+
+def dpir_mask(
+    clip: vs.VideoNode, low: float = 5, high: float = 10, lines: float | None = None,
+    luma_scaling: float = 12, linemask: GenericMaskT | bool = True, relative: bool = False
+) -> vs.VideoNode:
+    y = depth(get_y(clip), 32, range_out=ColorRange.FULL)
+
+    if linemask is True:
+        linemask = FDoG
+
+    mask = adg_mask(y, luma_scaling, relative, func=dpir_mask)
+
+    if relative:
+        mask = gauss_blur(mask, 1.5)
+
+    mask = norm_expr(mask, f'{high} 255 / x {low} 255 / * -')
+
+    if linemask:
+        lines = fallback(lines, high)
+        linemask = normalize_mask(linemask, y)
+
+        lines_clip = mask.std.BlankClip(color=lines / 255)
+
+        mask = mask.std.MaskedMerge(lines_clip, linemask)
+
+    return mask
```

### Comparing `vsdenoise-2.2.0/vsdenoise/fft.py` & `vsdenoise-2.3.0/vsdenoise/fft.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 ]
 
 Frequency: TypeAlias = float
 Sigma: TypeAlias = float
 
 
 class SInterMode(CustomEnum):
+    """SLocation interpolation mode."""
+
     LINEAR = 'linear'
     SPLINE = 1
     SPLINE_LINEAR = 'slinear'
     QUADRATIC = 'quadratic'
     CUBIC = 'cubic'
     NEAREST = 'nearest'
     NEAREST_UP = 'nearest-up'
@@ -61,14 +63,16 @@
         if len(locations) == 1:
             return SLocation.from_param(locations[0]).interpolate(self, res, digits)
 
         return SLocation.MultiDim(*(self(x, res, digits) for x in locations))
 
 
 class SLocation:
+    """Specify a range of frequencies to target."""
+
     frequencies: tuple[float, ...]
     sigmas: tuple[float, ...]
 
     NoProcess: SLocation
 
     @classmethod
     def boundsCheck(
@@ -210,19 +214,30 @@
 
 
 class FilterTypeWithInfo(KwargsT):
     ...
 
 
 class FilterType(CustomIntEnum):
+    """Filtering types for DFTTest."""
+
     WIENER = 0
+    """mult = max((psd - sigma) / psd, 0) ^ f0beta"""
+
     THR = 1
+    """mult = psd < sigma ? 0.0 : 1.0"""
+
     MULT = 2
+    """mult = sigma"""
+
     MULT_PSD = 3
+    """mult = (psd >= pmin && psd <= pmax) ? sigma : sigma2"""
+
     MULT_RANGE = 4
+    """mult = sigma * sqrt((psd * pmax) / ((psd + pmin) * (psd + pmax)))"""
 
     if TYPE_CHECKING:
         from .fft import FilterType
 
         @overload
         def __call__(  # type: ignore[misc]
             self: Literal[FilterType.WIENER], *, sigma: float = 8.0, beta: float = 1.0,
@@ -288,14 +303,16 @@
 
         value[f'{otype}win'] = value.pop('win')
 
         return value
 
 
 class SynthesisType(CustomIntEnum):
+    """Synthesis type for spatial processing."""
+
     HANNING = 0
     HAMMING = 1
     NUTTALL = 10
     BLACKMAN = 2
     BLACKMAN_NUTTALL = 11
     BLACKMAN_HARRIS_4TERM = 3
     BLACKMAN_HARRIS_7TERM = 5
@@ -478,14 +495,16 @@
 
         raise CustomRuntimeError(
             'No implementation of DFTTest could be found, please install one. dfttest2 is recommended.', self.__class__
         )
 
 
 class DFTTest:
+    """2D/3D frequency domain denoiser."""
+
     default_args: KwargsT
     default_slocation: SLocation | SLocation.MultiDim | None
 
     class Backend(CustomIntEnum):
         AUTO = auto()
         OLD = auto()
         NEO = auto()
```

### Comparing `vsdenoise-2.2.0/vsdenoise/funcs.py` & `vsdenoise-2.3.0/vsdenoise/funcs.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,37 @@
 
 from __future__ import annotations
 
 from itertools import count, zip_longest
 from typing import Any, Callable, Iterable, cast
 
 from vskernels import Bilinear, Catrom, Scaler, ScalerT
-from vsrgtools import RemoveGrainMode, contrasharpening, contrasharpening_dehalo, removegrain
+from vsrgtools import RemoveGrainMode, RepairMode, contrasharpening, contrasharpening_dehalo, removegrain
 from vsrgtools.util import norm_rmode_planes
 from vstools import (
-    FunctionUtil, KwargsT, PlanesT, VSFunction, depth, expect_bits, fallback, get_h, get_w, normalize_planes, vs
+    ColorRangeT, FunctionUtil, KwargsT, MatrixT, PlanesT, SingleOrArr, VSFunction, depth, expect_bits, fallback, get_h,
+    get_w, join, normalize_planes, to_arr, vs
 )
 
+from .blockmatch import bmdegrain
+from .bm3d import BM3D, Profile
 from .limit import TemporalLimiter, TemporalLimiterConfig
-from .mvtools import MotionMode, MVTools, MVToolsPresets, SADMode, SearchMode
+from .mvtools import MotionMode, MVTools, MVToolsPreset, MVToolsPresets, SADMode, SearchMode
 from .mvtools.enums import SearchModeBase
 from .mvtools.utils import normalize_thscd
+from .nlm import WeightMode, WeightModeAndRef, nl_means
 from .postprocess import PostProcess, PostProcessConfig
 from .prefilters import PelType, Prefilter
 
 __all__ = [
     'mlm_degrain',
 
-    'temporal_degrain'
+    'temporal_degrain',
+
+    'schizo_denoise'
 ]
 
 
 def mlm_degrain(
     clip: vs.VideoNode, tr: int = 3, refine: int = 3, thSAD: int | tuple[int, int] = 200,
     factors: Iterable[float] | range = [1 / 3, 2 / 3],
     scaler: ScalerT = Bilinear, downscaler: ScalerT = Catrom,
@@ -275,18 +281,83 @@
     else:
         dnWindow = postConf(NR2)
 
     if contra:
         if contra is True:
             contra = 3
 
-        if isinstance(contra, int):
-            sharpened = contrasharpening(dnWindow, func.work_clip, contra, 13, func.norm_planes)
-        else:
+        if isinstance(contra, float):
             sharpened = contrasharpening_dehalo(dnWindow, func.work_clip, contra, 2.5, func.norm_planes)
+        else:
+            sharpened = contrasharpening(dnWindow, func.work_clip, contra, 13, func.norm_planes)
     else:
         sharpened = dnWindow
 
     if postConf.tr > 0 and postConf.merge_strength:
         sharpened = func.work_clip.std.Merge(sharpened, postConf.merge_strength / 100)
 
     return func.return_clip(sharpened)
+
+
+def schizo_denoise(
+    src: vs.VideoNode, sigma: SingleOrArr[float] = [0.8, 0.3], thSAD: int = 60,
+    tr: SingleOrArr[int] = 2, sr: SingleOrArr[int] = 2, block_size: int = 32,
+    profile: Profile | Profile.Config = Profile.FAST(bm_range=9),
+    preset: MVToolsPreset = MVToolsPresets.FAST,
+    prefilter: vs.VideoNode | Prefilter = Prefilter.DFTTEST,
+    smooth: bool | tuple[bool | int, bool | int] = True,
+    wmode: WeightMode | WeightModeAndRef = WeightMode.WELSCH,
+    contra: int | float | bool = False, aggressive: vs.VideoNode | Prefilter | bool = False,
+    matrix: MatrixT | None = None, range_in: ColorRangeT | None = None,
+    nlm_ref: vs.VideoNode | bool | None = None, **kwargs: Any
+) -> vs.VideoNode:
+    func = FunctionUtil(
+        src, schizo_denoise, None, vs.YUV, range(16, 32), True, matrix=matrix, range_in=range_in
+    )
+
+    ref_smooth, out_smooth = smooth if isinstance(smooth, tuple) else (smooth, False)
+
+    luma_ref = MVTools.denoise(
+        func.work_clip, **preset(
+            thSAD=thSAD, prefilter=prefilter, block_size=block_size, planes=0,
+            overlap=block_size // 2, **kwargs
+        ), range_in=func.color_range
+    )
+
+    if isinstance(aggressive, vs.VideoNode):
+        main_clip, main_ref = luma_ref, aggressive
+    elif isinstance(aggressive, Prefilter):
+        main_clip, main_ref = luma_ref, aggressive(func.work_clip)
+    elif aggressive:
+        main_clip, main_ref = luma_ref, bmdegrain(
+            func.work_clip, [x * 3 for x in to_arr(sigma)], 1, 2,
+            block_size=block_size // 2, self_refine=True
+        )
+    else:
+        main_clip, main_ref = func.work_clip, luma_ref
+
+    chroma_ref = nl_means(
+        func.work_clip, sigma, tr, [0, *to_arr(sr)], wmode=wmode, planes=[1, 2],
+        ref=nlm_ref if isinstance(nlm_ref, vs.VideoNode) else (main_ref if nlm_ref else None)  # type: ignore
+    )
+
+    main_clip, main_ref = join(main_clip, chroma_ref), join(main_ref, chroma_ref)
+
+    if ref_smooth:
+        main_ref = main_ref.ttmpsm.TTempSmooth(maxr=1, thresh=1, mdiff=0, strength=ref_smooth, planes=0)
+
+    main = BM3D.denoise(
+        main_clip, sigma, tr, 1, profile, main_ref, matrix, range_in, planes=0
+    )
+
+    if out_smooth:
+        main = main.ttmpsm.TTempSmooth(maxr=1, thresh=1, mdiff=0, strength=out_smooth, planes=0)
+
+    if not contra:
+        return main
+
+    if isinstance(contra, float):
+        return contrasharpening_dehalo(main, func.work_clip, contra, planes=0)
+
+    return contrasharpening(
+        main, func.work_clip, contra, RepairMode(3 if contra is True else contra), planes=0
+    )
```

### Comparing `vsdenoise-2.2.0/vsdenoise/knlm.py` & `vsdenoise-2.3.0/vsdenoise/nlm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-This module implements a wrapper for KNLMeansCL
+This module implements a wrapper for non local means denoisers
 """
 
 from __future__ import annotations
 
 import warnings
 from enum import auto
-from typing import TYPE_CHECKING, Any, Literal, Sequence, overload
+from typing import TYPE_CHECKING, Any, Literal, NamedTuple, Sequence, overload
 
 from vstools import (
-    CustomEnum, CustomValueError, KwargsT, PlanesT, check_variable, core, join, normalize_planes, normalize_seq, to_arr,
-    vs
+    CustomEnum, CustomIntEnum, CustomValueError, KwargsT, PlanesT, check_variable, core, join, normalize_planes,
+    normalize_seq, to_arr, vs
 )
 
 __all__ = [
-    'ChannelMode', 'DeviceType',
+    'ChannelMode', 'DeviceType', 'WeightMode',
 
     'nl_means'
 ]
 
 
 class ChannelMode(CustomEnum):
     """Enum representing the NLMeans channel operation mode."""
@@ -87,15 +87,15 @@
 
     def __new__(cls, val: str, **kwargs: Any) -> DeviceTypeWithInfo:
         self = super().__new__(cls, val)
         self.kwargs = kwargs
         return self
 
     if TYPE_CHECKING:
-        from .knlm import DeviceType
+        from .nlm import DeviceType
 
         @overload  # type: ignore
         def __call__(
             self: Literal[DeviceType.CUDA], *, device_id: int | None = None, num_streams: int | None = None
         ) -> DeviceType:
             ...
 
@@ -119,27 +119,27 @@
         def __call__(self, **kwargs: Any) -> DeviceTypeWithInfo:
             return DeviceTypeWithInfo(str(self), **kwargs)
 
     def NLMeans(
         self: DeviceTypeWithInfo | DeviceType, clip: vs.VideoNode,
         h: float | None = None, d: int | None = None, a: int | None = None, s: int | None = None,
         channels: str | None = None, wmode: int | None = None, wref: float | None = None,
-        rclip: vs.VideoNode | None = None, **kwargs: Any
+        ref: vs.VideoNode | None = None, **kwargs: Any
     ) -> vs.VideoNode:
         if self == DeviceType.AUTO and hasattr(core, 'nlm_cuda'):
             self = DeviceType.CUDA
         elif self == DeviceType.CUDA and not hasattr(core, 'nlm_cuda'):
             raise CustomValueError("You can't use cuda device type, you are missing the nlm_cuda plugin!")
 
         if self == DeviceType.CUDA:
             return core.nlm_cuda.NLMeans(  # type: ignore
-                clip, d, a, s, h, channels, wmode, wref, rclip, **(self.kwargs | kwargs)
+                clip, d, a, s, h, channels, wmode, wref, ref, **(self.kwargs | kwargs)
             )
 
-        return core.knlm.KNLMeansCL(clip, d, a, s, h, channels, wmode, wref, rclip, **(self.kwargs | kwargs))
+        return core.knlm.KNLMeansCL(clip, d, a, s, h, channels, wmode, wref, ref, **(self.kwargs | kwargs))
 
 
 class DeviceType(DeviceTypeWithInfo, CustomEnum):
     """Enum representing available OpenCL device on which to run the plugin."""
 
     ACCELERATOR = 'accelerator'
     """Dedicated OpenCL accelerators."""
@@ -157,21 +157,58 @@
     """Automatically detect device. Priority is "cuda" -> "accelerator" -> "gpu" -> "cpu"."""
 
     if not TYPE_CHECKING:
         def __call__(self, **kwargs: Any) -> DeviceTypeWithInfo:
             return DeviceTypeWithInfo(str(self), **kwargs)
 
 
-DEVICETYPE = Literal['accelerator', 'cpu', 'gpu', 'auto']
+class WeightMode(CustomIntEnum):
+    WELSCH = 0
+    """
+    Welsch weighting function has a faster decay, but still assigns positive weights to dissimilar blocks.
+    Original Non-local means denoising weighting function.
+    """
+
+    BISQUARE_LR = 1
+    """
+    Modified Bisquare weighting function to be less robust.
+    """
+
+    BISQUARE_THR = 2
+    """
+    Bisquare weighting function use a soft threshold to compare neighbourhoods.
+    The weight is 0 as soon as a given threshold is exceeded.
+    """
+
+    BISQUARE_HR = 3
+    """
+    Modified Bisquare weighting function to be even more robust.
+    """
+
+    def __call__(self, weight_ref: float = 1.0) -> WeightModeAndRef:
+        """
+        :param weight_ref:  Amount of original pixel to contribute to the filter output,
+                            relative to the weight of the most similar pixel found.
+
+        :return:            Config with weight mode and ref.
+        """
+        return WeightModeAndRef(self, weight_ref)
+
+
+class WeightModeAndRef(NamedTuple):
+    weight_mode: WeightMode
+    weight_ref: float
 
 
 def nl_means(
     clip: vs.VideoNode, strength: float | Sequence[float] = 1.2,
     tr: int | Sequence[int] = 1, sr: int | Sequence[int] = 2, simr: int | Sequence[int] = 4,
-    device_type: DeviceType = DeviceType.AUTO, planes: PlanesT = None, **kwargs: Any
+    device_type: DeviceType = DeviceType.AUTO, ref: vs.VideoNode | None = None,
+    wmode: WeightMode | WeightModeAndRef = WeightMode.WELSCH, planes: PlanesT = None,
+    **kwargs: Any
 ) -> vs.VideoNode:
     """
     Convenience wrapper for NLMeans implementations.
 
     :param clip:            Source clip.
     :param strength:        Controls the strength of the filtering.\n
                             Larger values will remove more noise.
@@ -182,14 +219,16 @@
     :param sr:              Search Radius. Spatial size = `(2 * sr + 1)^2`.\n
                             Sets the radius of the search window.\n
                             sr=1 uses 9 pixel, while sr=2 uses 25 pixels and so on.\n
                             Usually, larger values result in better denoising.
     :param simr:            Similarity Radius. Similarity neighbourhood size = `(2 * simr + 1) ** 2`.\n
                             Sets the radius of the similarity neighbourhood window.\n
                             The impact on performance is low, therefore it depends on the nature of the noise.
+    :param ref:             Reference clip to do weighting calculation.
+    :param wmode:           Weighting function to use.
     :param planes:          Set the clip planes to be processed.
     :param device_type:     Set the device to use for processing. The fastest device will be used by default.
     :param kwargs:          Additional arguments passed to the plugin.
 
     :return:                Denoised clip.
     """
 
@@ -198,14 +237,18 @@
     planes = normalize_planes(clip, planes)
 
     if planes == []:
         return clip
 
     nstrength, ntr, nsr, nsimr = to_arr(strength), to_arr(tr), to_arr(sr), to_arr(simr)
 
+    wmoder, wref = wmode if isinstance(wmode, WeightModeAndRef) else wmode()
+
+    kwargs.update(ref=ref, wmode=wmoder.value, wref=wref)
+
     params = dict[str, list[float] | list[int]](strength=nstrength, tr=ntr, sr=nsr, simr=nsimr)
 
     def _nl_means(i: int, channels: str) -> vs.VideoNode:
         return device_type.NLMeans(clip, nstrength[i], ntr[i], nsr[i], nsimr[i], channels, **kwargs)
 
     if clip.format.color_family in {vs.GRAY, vs.RGB}:
         for doc, p in params.items():
```

### Comparing `vsdenoise-2.2.0/vsdenoise/limit.py` & `vsdenoise-2.3.0/vsdenoise/limit.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/vsdenoise/mvtools/enums.py` & `vsdenoise-2.3.0/vsdenoise/mvtools/enums.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/vsdenoise/mvtools/motion.py` & `vsdenoise-2.3.0/vsdenoise/mvtools/motion.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/vsdenoise/mvtools/mvtools.py` & `vsdenoise-2.3.0/vsdenoise/mvtools/mvtools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from itertools import chain
 from math import exp
-from typing import Any, Sequence
+from typing import Any, Callable, Concatenate, Sequence, Union, overload
 
 from vstools import (
     ColorRange, ConstantFormatVideoNode, CustomOverflowError, CustomRuntimeError, FieldBased, FieldBasedT, FuncExceptT,
-    GenericVSFunction, InvalidColorFamilyError, KwargsT, PlanesT, check_ref_clip, check_variable, clamp, core, depth,
+    InvalidColorFamilyError, KwargsT, P, PlanesT, check_ref_clip, check_variable, clamp, core, depth,
     disallow_variable_format, disallow_variable_resolution, fallback, kwargs_fallback, normalize_planes, normalize_seq,
     scale_value, vs
 )
 
 from ..prefilters import PelType, Prefilter, prefilter_to_full_range
 from .enums import MotionMode, MVDirection, MVToolsPlugin, SADMode, SearchMode
 from .motion import MotionVectors, SuperClips
@@ -304,15 +304,15 @@
         ) | self.super_args
         super_render_args = common_args | dict(levels=1, hpad=self.hpad, vpad=self.vpad, chroma=not self.is_gray)
 
         if pelclip or pelclip2:
             common_args |= dict(pelclip=pelclip)
             super_render_args |= dict(pelclip=pelclip2)
 
-        super_render = self.mvtools.Super(self.workclip, **super_render_args)
+        super_render = self.mvtools.Super(ref if inplace else self.workclip, **super_render_args)
         super_search = self.mvtools.Super(ref, **(dict(rfilter=rfilter) | common_args))
         super_recalc = self.refine and self.mvtools.Super(prefilter, **(dict(levels=1) | common_args)) or super_render
 
         supers = SuperClips(ref, super_render, super_search, super_recalc)
 
         if not inplace:
             self.supers = supers
@@ -392,15 +392,15 @@
         vectors = MotionVectors() if inplace else self.vectors
 
         if isinstance(sad_mode, tuple):
             sad_mode, recalc_sad_mode = sad_mode
         else:
             sad_mode, recalc_sad_mode = sad_mode, SADMode.SATD
 
-        supers = supers or self.get_supers(ref)
+        supers = supers or self.get_supers(ref, inplace=inplace)
 
         if self.params_curve:
             thSAD_recalc = round(exp(-101. / (thSAD * 0.83)) * 360)
         else:
             thSAD_recalc = thSAD
 
         t2 = (self.tr * 2 if self.tr > 1 else self.tr) if self.source_type.is_inter else self.tr
@@ -476,15 +476,15 @@
 
         recalc_args = KwargsT(
             search=search.recalc_mode, dct=sad_mode, thsad=thSAD, blksize=halfblocksize,
             overlap=overlap, truemotion=motion.truemotion, searchparam=search.param_recalc,
             chroma=self.chroma, pnew=motion.pnew, lambda_=motion.block_coherence(halfblocksize)
         ) | self.recalculate_args
 
-        supers = supers or self.get_supers(ref)
+        supers = supers or self.get_supers(ref, inplace=True)
 
         if self.mvtools is MVToolsPlugin.FLOAT_NEW:
             for i in range(refine):
                 recalc_blksize = clamp(blocksize / 2 ** i, 4, 128)
 
                 vectors.vmulti = self.mvtools.Recalculate(
                     supers.recalculate, vectors=vectors.vmulti, **(recalc_args | dict(
@@ -503,63 +503,121 @@
                     vectors.calculate_vectors(
                         i, self.mvtools, supers, True, **(recalc_args | dict(
                             blksize=recalc_blksize, overlap=recalc_blksize // 2,
                             lambda_=motion.block_coherence(recalc_blksize)
                         ))
                     )
 
-    def compensate(
-        self, func: GenericVSFunction, thSAD: int = 150,
-        thSCD: int | tuple[int | None, int | None] | None = (None, 51),
-        supers: SuperClips | None = None, *, ref: vs.VideoNode | None = None, **kwargs: Any
+    @overload
+    def compensate(  # type: ignore
+        self, func: Union[
+            Callable[Concatenate[vs.VideoNode, P], vs.VideoNode],
+            Callable[Concatenate[list[vs.VideoNode], P], vs.VideoNode]
+        ], thSAD: int = 150, thSCD: int | tuple[int | None, int | None] | None = (None, 51),
+        supers: SuperClips | None = None, *args: P.args, ref: vs.VideoNode | None = None,
+        **kwargs: P.kwargs
     ) -> vs.VideoNode:
         """
         At compensation stage, the plugin client functions read the motion vectors and use them to move blocks
         and form a motion compensated frame (or realize some other full- or partial motion compensation or
         interpolation function).
 
         Every block in this fully-compensated frame is placed in the same position as this block in current frame.
 
         So, we may (for example) use strong temporal denoising even for quite fast moving objects without producing
         annoying artefactes and ghosting (object's features and edges coincide if compensation is perfect).
 
         This function is for using compensated and original frames to create an interleaved clip,
         denoising it with the external temporal filter `func`, and select central cleaned original frames for output.
 
-        :param func:     Temporal function to motion compensate.
-        :param thSAD:    This is the SAD threshold for safe (dummy) compensation.\n
-                         If block SAD is above thSAD, the block is bad, and we use source block
-                         instead of the compensated block.
-        :param thSCD:    The first value is a threshold for whether a block has changed
-                         between the previous frame and the current one.\n
-                         When a block has changed, it means that motion estimation for it isn't relevant.
-                         It, for example, occurs at scene changes, and is one of the thresholds used to
-                         tweak the scene changes detection engine.\n
-                         Raising it will lower the number of blocks detected as changed.\n
-                         It may be useful for noisy or flickered video. This threshold is compared to the SAD value.\n
-                         For exactly identical blocks we have SAD = 0, but real blocks are always different
-                         because of objects complex movement (zoom, rotation, deformation),
-                         discrete pixels sampling, and noise.\n
-                         Suppose we have two compared 8×8 blocks with every pixel different by 5.\n
-                         It this case SAD will be 8×8×5 = 320 (block will not detected as changed for thSCD1 = 400).\n
-                         Actually this parameter is scaled internally in MVTools,
-                         and it is always relative to 8x8 block size.\n
-                         The second value is a threshold of the percentage of how many blocks have to change for
-                         the frame to be considered as a scene change. It ranges from 0 to 100 %.
-        :param supers:   Custom super clips to be used for compensating.
-        :param ref:      Reference clip to use instead of main clip.
-        :param kwargs:   Keyword arguments passed to `func` to avoid using `partial`.
+        :param func:    Temporal function to motion compensate.
+        :param thSAD:   This is the SAD threshold for safe (dummy) compensation.\n
+                        If block SAD is above thSAD, the block is bad, and we use source block
+                        instead of the compensated block.
+        :param thSCD:   The first value is a threshold for whether a block has changed
+                        between the previous frame and the current one.\n
+                        When a block has changed, it means that motion estimation for it isn't relevant.
+                        It, for example, occurs at scene changes, and is one of the thresholds used to
+                        tweak the scene changes detection engine.\n
+                        Raising it will lower the number of blocks detected as changed.\n
+                        It may be useful for noisy or flickered video. This threshold is compared to the SAD value.\n
+                        For exactly identical blocks we have SAD = 0, but real blocks are always different
+                        because of objects complex movement (zoom, rotation, deformation),
+                        discrete pixels sampling, and noise.\n
+                        Suppose we have two compared 8×8 blocks with every pixel different by 5.\n
+                        It this case SAD will be 8×8×5 = 320 (block will not detected as changed for thSCD1 = 400).\n
+                        Actually this parameter is scaled internally in MVTools,
+                        and it is always relative to 8x8 block size.\n
+                        The second value is a threshold of the percentage of how many blocks have to change for
+                        the frame to be considered as a scene change. It ranges from 0 to 100 %.
+        :param supers:  Custom super clips to be used for compensating.
+        :param wargs:   Arguments passed to `func` to avoid using `partial`.
+        :param ref:     Reference clip to use instead of main clip.
+        :param kwargs:  Keyword arguments passed to `func` to avoid using `partial`.
+
+        :return:        Motion compensated output of `func`.
+        """
+
+    @overload
+    def compensate(
+        self, func: None,
+        thSAD: int = 150, thSCD: int | tuple[int | None, int | None] | None = (None, 51),
+        supers: SuperClips | None = None, ref: vs.VideoNode | None = None
+    ) -> tuple[vs.VideoNode, tuple[int, int]]:
+        """
+        At compensation stage, the plugin client functions read the motion vectors and use them to move blocks
+        and form a motion compensated frame (or realize some other full- or partial motion compensation or
+        interpolation function).
+
+        Every block in this fully-compensated frame is placed in the same position as this block in current frame.
+
+        So, we may (for example) use strong temporal denoising even for quite fast moving objects without producing
+        annoying artefactes and ghosting (object's features and edges coincide if compensation is perfect).
+
+        This function is for using compensated and original frames to create an interleaved clip,
+        denoising it with the external temporal filter `func`, and select central cleaned original frames for output.
+
+        :param thSAD:   This is the SAD threshold for safe (dummy) compensation.\n
+                        If block SAD is above thSAD, the block is bad, and we use source block
+                        instead of the compensated block.
+        :param thSCD:   The first value is a threshold for whether a block has changed
+                        between the previous frame and the current one.\n
+                        When a block has changed, it means that motion estimation for it isn't relevant.
+                        It, for example, occurs at scene changes, and is one of the thresholds used to
+                        tweak the scene changes detection engine.\n
+                        Raising it will lower the number of blocks detected as changed.\n
+                        It may be useful for noisy or flickered video. This threshold is compared to the SAD value.\n
+                        For exactly identical blocks we have SAD = 0, but real blocks are always different
+                        because of objects complex movement (zoom, rotation, deformation),
+                        discrete pixels sampling, and noise.\n
+                        Suppose we have two compared 8×8 blocks with every pixel different by 5.\n
+                        It this case SAD will be 8×8×5 = 320 (block will not detected as changed for thSCD1 = 400).\n
+                        Actually this parameter is scaled internally in MVTools,
+                        and it is always relative to 8x8 block size.\n
+                        The second value is a threshold of the percentage of how many blocks have to change for
+                        the frame to be considered as a scene change. It ranges from 0 to 100 %.
+        :param supers:  Custom super clips to be used for compensating.
+        :param ref:     Reference clip to use instead of main clip.
 
-        :return:         Motion compensated output of `func`.
+        :return:        A tuple of motion compensated clip, then a tuple of (cycle, offset) so that
+                        compensated.std.SelectEvery(cycle, offsets) will give the original clip.
         """
 
+    def compensate(  # type: ignore
+        self, func: Union[
+            Callable[Concatenate[vs.VideoNode, P], vs.VideoNode],
+            Callable[Concatenate[list[vs.VideoNode], P], vs.VideoNode]
+        ] | None, thSAD: int = 150, thSCD: int | tuple[int | None, int | None] | None = (None, 51),
+        supers: SuperClips | None = None, *args: P.args, ref: vs.VideoNode | None = None,
+        **kwargs: P.kwargs
+    ) -> vs.VideoNode | tuple[vs.VideoNode, tuple[int, int]]:
         ref = self.get_ref_clip(ref, self.compensate)
 
         thSCD1, thSCD2 = self.normalize_thscd(thSCD, thSAD, self.compensate)
-        supers = supers or self.get_supers(ref)
+        supers = supers or self.get_supers(ref, inplace=True)
 
         vect_b, vect_f = self.get_vectors_bf(self.vectors)
 
         compensate_args = dict(
             super=supers.render, thsad=thSAD,
             thscd1=thSCD1, thscd2=thSCD2,
             tff=self.source_type.is_inter and self.source_type.value or None
@@ -568,20 +626,27 @@
         comp_back, comp_forw = [
             [self.mvtools.Compensate(ref, vectors=vect, **compensate_args) for vect in vectors]
             for vectors in (reversed(vect_b), vect_f)
         ]
 
         comp_clips = [*comp_forw, ref, *comp_back]
         n_clips = len(comp_clips)
+        offset = (n_clips - 1) // 2
 
         interleaved = core.std.Interleave(comp_clips)
 
-        processed = func(interleaved, **kwargs)
+        if func:
+            try:
+                processed = func(interleaved, *args, **kwargs)  # type: ignore
+
+                return processed.std.SelectEvery(n_clips, offset)
+            except Exception:
+                return func(comp_clips, *args, **kwargs)  # type: ignore
 
-        return processed.std.SelectEvery(cycle=n_clips, offsets=(n_clips - 1) // 2)
+        return interleaved, (n_clips, offset)
 
     def degrain(
         self,
         thSAD: int | tuple[int | None, int | None] | None = None,
         limit: int | tuple[int, int] = 255,
         thSCD: int | tuple[int | None, int | None] | None = (None, 51),
         supers: SuperClips | None = None,
@@ -631,15 +696,15 @@
 
         if isinstance(vectors, MVTools):
             vectors = vectors.vectors
         elif vectors is None:
             vectors = self.vectors
 
         vect_b, vect_f = self.get_vectors_bf(vectors, supers=supers, ref=ref)
-        supers = supers or self.get_supers(ref)
+        supers = supers or self.get_supers(ref, inplace=True)
 
         thSAD, thSADC = (thSAD if isinstance(thSAD, tuple) else (thSAD, None))
 
         thSAD = kwargs_fallback(thSAD, (vectors.kwargs, 'thSAD'), 300)
         thSADC = fallback(thSADC, round(thSAD * 0.18875 * exp(2 * 0.693)) if self.params_curve else thSAD // 2)
 
         limit, limitC = normalize_seq(limit, 2)
@@ -683,18 +748,15 @@
 
         :return:            SuperClips tuple.
         """
 
         if self.supers and self.supers.base == ref:
             return self.supers
 
-        supers = self.super(ref=ref)
-
-        if not inplace:
-            self.supers = supers
+        supers = self.super(ref=ref, inplace=inplace)
 
         return supers
 
     def get_vectors_bf(
         self, vectors: MotionVectors, *, supers: SuperClips | None = None,
         ref: vs.VideoNode | None = None, inplace: bool = False
     ) -> tuple[list[vs.VideoNode], list[vs.VideoNode]]:
```

### Comparing `vsdenoise-2.2.0/vsdenoise/mvtools/presets.py` & `vsdenoise-2.3.0/vsdenoise/mvtools/presets.py`

 * *Files 10% similar despite different names*

```diff
@@ -127,7 +127,22 @@
         pel=1, prefilter=Prefilter.NONE, params_curve=False, sharp=2, rfilter=4,
         block_size=32, overlap=16, thSAD=200, sad_mode=SADMode.SPATIAL.same_recalc,
         motion=MotionMode.HIGH_SAD, search=SearchMode.HEXAGON.defaults,
         hpad=property(fget=lambda x: x.block_size), vpad=property(fget=lambda x: x.block_size),
         range_conversion=1.0
     )
     """CMDegrain from EoE."""
+
+    FAST = MVToolsPreset(
+        pel=1, prefilter=Prefilter.MINBLUR3, thSAD=60, block_size=32,
+        overlap=property(fget=lambda x: x.block_size // 2),
+        sad_mode=SADMode.SPATIAL.same_recalc, search=SearchMode.DIAMOND,
+        motion=MotionMode.HIGH_SAD, pel_type=PelType.BICUBIC, rfilter=2, sharp=2
+    )
+    """Fast preset"""
+
+    NOISY = MVToolsPreset(
+        pel=2, thSAD=100, block_size=32, overlap=property(fget=lambda x: x.block_size // 2),
+        motion=MotionMode.HIGH_SAD, prefilter=Prefilter.DFTTEST,
+        sad_mode=(SADMode.ADAPTIVE_SPATIAL_MIXED, SADMode.ADAPTIVE_SATD_MIXED)
+    )
+    """Preset for accurate estimation"""
```

### Comparing `vsdenoise-2.2.0/vsdenoise/mvtools/utils.py` & `vsdenoise-2.3.0/vsdenoise/mvtools/utils.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/vsdenoise/prefilters.py` & `vsdenoise-2.3.0/vsdenoise/prefilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     disallow_variable_resolution, fallback, get_depth, get_neutral_value, get_peak_value, get_y, join, normalize_planes,
     normalize_seq, scale_8bit, scale_value, split, vs
 )
 
 from .bm3d import BM3D as BM3DM
 from .bm3d import BM3DCPU, AbstractBM3D, BM3DCuda, BM3DCudaRTC, Profile
 from .fft import DFTTest
-from .knlm import DEVICETYPE, DeviceType, nl_means
+from .nlm import DeviceType, nl_means
 
 __all__ = [
     'Prefilter', 'prefilter_to_full_range',
     'MultiPrefilter',
     'PelType'
 ]
 
@@ -128,17 +128,17 @@
             elif bm3d_arch in (BM3DCuda, BM3DCudaRTC):
                 sigma, profile = 8, Profile.NORMAL
             else:
                 raise ValueError
 
             sigmas = kwargs.pop('sigma', [sigma if 0 in planes else 0, sigma if (1 in planes or 2 in planes) else 0])
 
-            bm3d_args = dict[str, Any](sigma=sigmas, radius=1, profile=profile) | kwargs
+            bm3d_args = dict[str, Any](sigma=sigmas, tr=1, profile=profile) | kwargs
 
-            return bm3d_arch(clip, **bm3d_args).final()
+            return bm3d_arch.denoise(clip, **bm3d_args)
 
         if pref_type == Prefilter.SCALEDBLUR:
             scale = kwargs.pop('scale', 2)
             downscaler = Scaler.ensure_obj(kwargs.pop('downscaler', Bilinear))
             upscaler = downscaler.ensure_obj(kwargs.pop('upscaler', downscaler))
 
             downscale = downscaler.scale(clip, clip.width // scale, clip.height // scale)
@@ -209,15 +209,15 @@
         if pref_type is Prefilter.BMLATERAL:
             sigma = kwargs.pop('sigma', 1.5)
             tr = kwargs.pop('tr', 2)
             radius = kwargs.pop('radius', 7)
             cuda = kwargs.pop('gpu', hasattr(core, 'bm3dcuda'))
 
             den = Prefilter.BM3D(
-                clip, planes, sigma=[10.0, 8.0] if cuda else [8.0, 6.4], radius=tr, gpu=cuda, **kwargs
+                clip, planes, sigma=[10.0, 8.0] if cuda else [8.0, 6.4], tr=tr, gpu=cuda, **kwargs
             )
 
             return Prefilter.BILATERAL(den, planes, sigmaS=[sigma, sigma / 3], sigmaR=radius / 255)
 
 
 class Prefilter(PrefilterBase):
     """
@@ -320,15 +320,15 @@
         ) -> vs.VideoNode:
             ...
 
         @overload
         def __call__(  # type: ignore
             self: Literal[Prefilter.NLMEANS], clip: vs.VideoNode, /, planes: PlanesT = None,
             *, strength: SingleOrArr[float] = 7.0, tr: SingleOrArr[int] = 1, sr: SingleOrArr[int] = 2,
-            simr: SingleOrArr[int] = 2, device_type: DEVICETYPE | DeviceType = DeviceType.AUTO, **kwargs: Any
+            simr: SingleOrArr[int] = 2, device_type: DeviceType = DeviceType.AUTO, **kwargs: Any
         ) -> vs.VideoNode:
             """
             Denoising with NLMeans, then postprocessed to remove low frequencies.
 
             :param clip:            Source clip.
             :param strength:        Controls the strength of the filtering.\n
                                     Larger values will remove more noise.
@@ -349,24 +349,24 @@
 
             :return:                Denoised clip.
             """
 
         @overload
         def __call__(  # type: ignore
             self: Literal[Prefilter.BM3D], clip: vs.VideoNode, /, planes: PlanesT = None,
-            *, arch: type[AbstractBM3D] = ..., gpu: bool = False,
-            sigma: SingleOrArr[float] = ..., radius: SingleOrArr[int] = 1,
+            *, arch: type[AbstractBM3D] = ..., gpu: bool | None = None,
+            sigma: SingleOrArr[float] = ..., tr: SingleOrArr[int] = 1,
             profile: Profile = ..., ref: vs.VideoNode | None = None, refine: int = 1
         ) -> vs.VideoNode:
             """
             Normal spatio-temporal denoising using BM3D.
 
             :param clip:        Clip to be preprocessed.
             :param sigma:       Strength of denoising, valid range is [0, +inf].
-            :param radius:      Temporal radius, valid range is [1, 16].
+            :param tr:          Temporal radius, valid range is [1, 16].
             :param profile:     See :py:attr:`vsdenoise.bm3d.Profile`.
             :param ref:         Reference clip used in block-matching, replacing the basic estimation.
                                 If not specified, the input clip is used instead.
             :param refine:      Times to refine the estimation.
                                 * 0 means basic estimate only.
                                 * 1 means basic estimate with one final estimate.
                                 * n means basic estimate refined with final estimate for n times.
@@ -547,15 +547,15 @@
         ) -> PrefilterPartial:
             ...
 
         @overload
         def __call__(  # type: ignore
             self: Literal[Prefilter.NLMEANS], *, planes: PlanesT = None,
             strength: SingleOrArr[float] = 7.0, tr: SingleOrArr[int] = 1, sr: SingleOrArr[int] = 2,
-            simr: SingleOrArr[int] = 2, device_type: DEVICETYPE | DeviceType = DeviceType.AUTO, **kwargs: Any
+            simr: SingleOrArr[int] = 2, device_type: DeviceType = DeviceType.AUTO, **kwargs: Any
         ) -> PrefilterPartial:
             """
             Denoising with NLMeans, then postprocessed to remove low frequencies.
 
             :param planes:          Set the clip planes to be processed.
             :param strength:        Controls the strength of the filtering.\n
                                     Larger values will remove more noise.
```

### Comparing `vsdenoise-2.2.0/vsdenoise/regress.py` & `vsdenoise-2.3.0/vsdenoise/regress.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/vsdenoise/types.py` & `vsdenoise-2.3.0/vsdenoise/types.py`

 * *Files identical despite different names*

### Comparing `vsdenoise-2.2.0/vsdenoise.egg-info/PKG-INFO` & `vsdenoise-2.3.0/vsdenoise.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdenoise
-Version: 2.2.0
+Version: 2.3.0
 Summary: VapourSynth denoising functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-denoise
 Project-URL: Documentation, https://vsdenoise.encode.moe/en/latest/
@@ -34,8 +34,31 @@
 ```
 
 Or if you want the latest git version, install it with this command:
 
 ```sh
 $ pip install git+https://github.com/Irrational-Encoding-Wizardry/vs-denoise.git
 ```
-<br>
+<br><br>
+
+## Example usage
+```py
+from vsdenoise import MVTools, SADMode, MotionMode, Prefilter, BM3DCuda, Profile, nl_means
+
+clip = ...
+
+ref = MVTools.denoise(
+    clip, thSAD=100, block_size=32, overlap=16,
+    motion=MotionMode.HIGH_SAD,
+    prefilter=Prefilter.DFTTEST,
+    sad_mode=(
+        SADMode.ADAPTIVE_SPATIAL_MIXED,
+        SADMode.ADAPTIVE_SATD_MIXED,
+    )
+)
+
+denoise = BM3DCuda.denoise(
+    clip, sigma=0.8, tr=2, profile=Profile.NORMAL, ref=ref, planes=0
+)
+
+denoise = nl_means(denoise, tr=2, strength=0.6, ref=ref, planes=[1, 2])
+```
```

### Comparing `vsdenoise-2.2.0/vsdenoise.egg-info/SOURCES.txt` & `vsdenoise-2.3.0/vsdenoise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 vsdenoise/__init__.py
 vsdenoise/_metadata.py
 vsdenoise/blockmatch.py
 vsdenoise/bm3d.py
 vsdenoise/ccd.py
 vsdenoise/deblock.py
 vsdenoise/fft.py
+vsdenoise/freqs.py
 vsdenoise/funcs.py
-vsdenoise/knlm.py
 vsdenoise/limit.py
+vsdenoise/nlm.py
 vsdenoise/postprocess.py
 vsdenoise/prefilters.py
 vsdenoise/py.typed
 vsdenoise/regress.py
 vsdenoise/types.py
 vsdenoise.egg-info/PKG-INFO
 vsdenoise.egg-info/SOURCES.txt
```

