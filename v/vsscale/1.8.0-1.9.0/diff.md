# Comparing `tmp/vsscale-1.8.0.tar.gz` & `tmp/vsscale-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsscale-1.8.0.tar", last modified: Thu May  4 21:58:58 2023, max compression
+gzip compressed data, was "vsscale-1.9.0.tar", last modified: Mon Jun  5 14:03:02 2023, max compression
```

## Comparing `vsscale-1.8.0.tar` & `vsscale-1.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:58.075980 vsscale-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 21:58:30.000000 vsscale-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 21:58:58.075980 vsscale-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-04 21:58:30.000000 vsscale-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:58:58.079980 vsscale-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-04 21:58:30.000000 vsscale-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:58.075980 vsscale-1.8.0/vsscale/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/descale.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:58.075980 vsscale-1.8.0/vsscale/shaders/
--rw-r--r--   0 runner    (1001) docker     (123)   246177 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl
--rw-r--r--   0 runner    (1001) docker     (123)   362441 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl
--rw-r--r--   0 runner    (1001) docker     (123)    70598 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/SSimDownscaler.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/SSimSuperRes.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:58.075980 vsscale-1.8.0/vsscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:02.544036 vsscale-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-05 14:02:41.000000 vsscale-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-05 14:03:02.544036 vsscale-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-05 14:02:41.000000 vsscale-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 14:03:02.544036 vsscale-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-05 14:02:41.000000 vsscale-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:02.540036 vsscale-1.9.0/vsscale/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/descale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13814 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:02.544036 vsscale-1.9.0/vsscale/shaders/
+-rw-r--r--   0 runner    (1001) docker     (123)   246177 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)   362441 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)    70598 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/SSimDownscaler.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders/SSimSuperRes.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-05 14:02:41.000000 vsscale-1.9.0/vsscale/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:03:02.544036 vsscale-1.9.0/vsscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:03:02.000000 vsscale-1.9.0/vsscale.egg-info/top_level.txt
```

### Comparing `vsscale-1.8.0/LICENSE` & `vsscale-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/PKG-INFO` & `vsscale-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsscale
-Version: 1.8.0
+Version: 1.9.0
 Summary: VapourSynth (de)scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-scale
 Project-URL: Documentation, https://vsscale.encode.moe/en/latest/
```

### Comparing `vsscale-1.8.0/setup.cfg` & `vsscale-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/setup.py` & `vsscale-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/base.py` & `vsscale-1.9.0/vsscale/base.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/descale.py` & `vsscale-1.9.0/vsscale/descale.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/exceptions.py` & `vsscale-1.9.0/vsscale/exceptions.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/funcs.py` & `vsscale-1.9.0/vsscale/funcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,18 +64,16 @@
                 ]
         else:
             weight = 1.0 / len(scalers)
 
             norm_scalers = [(scaler, weight) for scaler in scalers]  # type: ignore
 
         self.scalers = [
-            (
-                Scaler.ensure_obj(scaler, self.__class__),
-                float(weight if weight else 0)
-            ) for scaler, weight in norm_scalers
+            (self.ensure_scaler(scaler), float(weight if weight else 0))
+            for scaler, weight in norm_scalers
         ]
 
     def scale(  # type: ignore
         self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0), **kwargs: Any
     ) -> vs.VideoNode:
         scalers, weights = cast(tuple[list[Scaler], list[float]], zip(*self.scalers))
 
@@ -106,15 +104,15 @@
 
     operator: Literal[ExprOp.MAX, ExprOp.MIN] | None = ExprOp.MIN
     """Whether to take the brightest or darkest pixels in the merge."""
 
     masked: bool = True
     """Whether to mask with a ringing mask or not."""
 
-    reference: ScalerT | vs.VideoNode = field(default_factory=lambda: Nnedi3(0, opencl=None))
+    reference: ScalerT | vs.VideoNode = Nnedi3
     """Reference Scaler used to clamp ref_scaler"""
 
     range_out: ColorRange | None = None
     """Range out for clamping the output. If None it will be fetched from the VideoNode."""
 
     def __post_init__(self) -> None:
         super().__post_init__()
@@ -125,32 +123,30 @@
             raise CustomOverflowError('strength can\'t be less or equal to 0!', self.__class__)
 
         if self.overshoot is None:
             self.overshoot = self.strength / 100
         if self.undershoot is None:
             self.undershoot = self.overshoot
 
-        self._ref_scaler = Scaler.ensure_obj(self.ref_scaler, self.__class__)
-
     @inject_self
     def scale(  # type: ignore
         self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0),
         *, smooth: vs.VideoNode | None = None, **kwargs: Any
     ) -> vs.VideoNode:
         assert (self.undershoot or self.undershoot == 0) and (self.overshoot or self.overshoot == 0)
 
-        ref = self._ref_scaler.scale(clip, width, height, shift, **kwargs)
+        ref = self.ensure_scaler(self.ref_scaler).scale(clip, width, height, shift, **kwargs)
 
         if isinstance(self.reference, vs.VideoNode):
             smooth = self.reference  # type: ignore
 
             if shift != (0, 0):
                 smooth = self._kernel.shift(smooth, shift)  # type: ignore
         else:
-            smooth = Scaler.ensure_obj(self.reference, self.__class__).scale(clip, width, height, shift)  # type: ignore
+            smooth = self.ensure_scaler(self.reference).scale(clip, width, height, shift)  # type: ignore
 
         assert smooth
 
         check_ref_clip(ref, smooth)
 
         range_out = ColorRange.from_video(clip, False) if self.range_out is None else self.range_out
 
@@ -213,15 +209,15 @@
         """
 
         self.unsharp_func = unsharp_func
 
         self.merge_mode = merge_mode
 
         self.reference = reference
-        self.ref_scaler = Scaler.ensure_obj(ref_scaler, self.__class__)
+        self.ref_scaler = self.ensure_scaler(ref_scaler)
 
         self.args = args
         self.kwargs = kwargs
 
     @inject_self
     def scale(  # type: ignore
         self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0),
@@ -231,15 +227,15 @@
 
         if isinstance(self.reference, vs.VideoNode):
             smooth = self.reference  # type: ignore
 
             if shift != (0, 0):
                 smooth = self._kernel.shift(smooth, shift)  # type: ignore
         else:
-            smooth = Scaler.ensure_obj(self.reference, self.__class__).scale(clip, width, height, shift)  # type: ignore
+            smooth = self.ensure_scaler(self.reference).scale(clip, width, height, shift)  # type: ignore
 
         assert smooth
 
         check_ref_clip(fsrcnnx, smooth)
 
         smooth_sharp = self.unsharp_func(smooth, *self.args, **self.kwargs)
```

### Comparing `vsscale-1.8.0/vsscale/gamma.py` & `vsscale-1.9.0/vsscale/gamma.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/helpers.py` & `vsscale-1.9.0/vsscale/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from functools import partial
+from math import ceil, floor
 from typing import Any, Callable, Protocol
 
 from vsaa import Nnedi3
 from vskernels import Catrom, Kernel, KernelT, Scaler, ScalerT
-from vstools import F_VD, MatrixT, get_w, plane, vs
+from vstools import F_VD, KwargsT, MatrixT, fallback, get_w, mod2, plane, vs
 
 from .types import Resolution
 
 __all__ = [
     'GenericScaler',
-    'scale_var_clip'
+    'scale_var_clip',
+    'fdescale_args'
 ]
 
 
 class _GeneriScaleNoShift(Protocol):
     def __call__(self, clip: vs.VideoNode, width: int, height: int, *args: Any, **kwds: Any) -> vs.VideoNode:
         ...
 
@@ -34,28 +36,28 @@
     """
     Generic Scaler base class.
     Inherit from this to create more complex scalers with built-in utils.
     Instantiate with a callable taking at least a VideoNode, width, and height
     to use that as a Scaler in functions taking that.
     """
 
-    kernel: KernelT = field(default_factory=lambda: Catrom, kw_only=True)
+    kernel: KernelT | None = field(default=None, kw_only=True)
     """
     Base kernel to be used for certain scaling/shifting/resampling operations.
     Must be specified and defaults to catrom
     """
 
     scaler: ScalerT | None = field(default=None, kw_only=True)
     """Scaler used for scaling operations. Defaults to kernel."""
 
     shifter: KernelT | None = field(default=None, kw_only=True)
     """Kernel used for shifting operations. Defaults to kernel."""
 
     def __post_init__(self) -> None:
-        self._kernel = Kernel.ensure_obj(self.kernel, self.__class__)
+        self._kernel = Kernel.ensure_obj(self.kernel or Catrom, self.__class__)
         self._scaler = Scaler.ensure_obj(self.scaler or self._kernel, self.__class__)
         self._shifter = Kernel.ensure_obj(
             self.shifter or (self._scaler if isinstance(self._scaler, Kernel) else Catrom), self.__class__
         )
 
     def __init__(
         self, func: _GeneriScaleNoShift | _GeneriScaleWithShift | F_VD, **kwargs: Any
@@ -109,14 +111,35 @@
             clip = self._kernel.resample(clip, input_clip, matrix)
 
         if copy_props:
             return clip.std.CopyFrameProps(input_clip)
 
         return clip
 
+    def ensure_scaler(self, scaler: ScalerT) -> Scaler:
+        from dataclasses import is_dataclass, replace
+
+        scaler_obj = Scaler.ensure_obj(scaler, self.__class__)
+
+        if is_dataclass(scaler_obj):
+            kwargs = dict()
+
+            if hasattr(scaler_obj, 'kernel'):
+                kwargs.update(kernel=self.kernel or scaler_obj.kernel)
+
+            if hasattr(scaler_obj, 'scaler'):
+                kwargs.update(scaler=self.scaler or scaler_obj.scaler)
+
+            if hasattr(scaler_obj, 'shifter'):
+                kwargs.update(shifter=self.shifter or scaler_obj.shifter)
+
+            scaler_obj = replace(scaler_obj, **kwargs)
+
+        return scaler_obj
+
 
 def scale_var_clip(
     clip: vs.VideoNode,
     width: int | Callable[[Resolution], int] | None, height: int | Callable[[Resolution], int],
     shift: tuple[float, float] | Callable[[Resolution], tuple[float, float]] = (0, 0),
     scaler: Scaler | Callable[[Resolution], Scaler] = Nnedi3(), debug: bool = False
 ) -> vs.VideoNode:
@@ -172,7 +195,44 @@
 
     if callable(width) or callable(height):
         out_clip = clip
     else:
         out_clip = clip.std.BlankClip(width, height)
 
     return out_clip.std.FrameEval(_eval_scale, clip, clip)
+
+
+def fdescale_args(
+    clip: vs.VideoNode, src_height: float,
+    base_height: int | None = None, base_width: int | None = None,
+    src_top: float | None = None, src_left: float | None = None,
+    src_width: float | None = None, mode: str = 'hw', up_rate: float = 2.0
+) -> tuple[KwargsT, KwargsT]:
+    base_height = fallback(base_height, mod2(ceil(src_height)))
+    base_width = fallback(base_width, get_w(base_height, clip, 2))
+
+    src_width = fallback(src_width, src_height * clip.width / clip.height)
+
+    cropped_width = base_width - 2 * floor((base_width - src_width) / 2)
+    cropped_height = base_height - 2 * floor((base_height - src_height) / 2)
+
+    do_h, do_w = 'h' in mode.lower(), 'w' in mode.lower()
+
+    de_args = dict(
+        width=cropped_width if do_w else clip.width,
+        height=cropped_height if do_h else clip.height
+    )
+
+    up_args = dict()
+
+    src_top = fallback(src_top, (cropped_height - src_height) / 2)
+    src_left = fallback(src_left, (cropped_width - src_width) / 2)
+
+    if do_h:
+        de_args.update(src_height=src_height, src_top=src_top)
+        up_args.update(src_height=src_height * up_rate, src_top=src_top * up_rate)
+
+    if do_w:
+        de_args.update(src_width=src_width, src_left=src_left)
+        up_args.update(src_width=src_width * up_rate, src_left=src_left * up_rate)
+
+    return de_args, up_args
```

### Comparing `vsscale-1.8.0/vsscale/mask.py` & `vsscale-1.9.0/vsscale/mask.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
-from vsexprtools import ExprOp, average_merge, combine, norm_expr
+from vsexprtools import ExprOp, average_merge, norm_expr
 from vskernels import Catrom
 from vsmasktools import Morpho, XxpandMode
 from vsrgtools import box_blur, gauss_blur
-from vstools import (
-    core, get_depth, get_neutral_value, get_peak_value, get_y, iterate, scale_value, shift_clip_multi, split, vs
-)
+from vstools import core, get_y, iterate, shift_clip_multi, split, vs
 
 __all__ = [
     'descale_detail_mask', 'descale_error_mask'
 ]
 
 
 def descale_detail_mask(
@@ -33,15 +31,15 @@
                         The first ``Maximum`` is done before inflating, the second after.
                         Default: 4 times pre-inflating, 0 times post-inflating.
 
     :return:            Mask containing all the native FHD detail.
     """
     mask = norm_expr([get_y(clip), get_y(rescaled)], 'x y - abs')
 
-    mask = mask.std.Binarize(thr * get_peak_value(mask))
+    mask = Morpho.binarize(mask, thr)
 
     if xxpand[0]:
         mask = iterate(mask, core.std.Maximum if xxpand[0] > 0 else core.std.Minimum, xxpand[0])
 
     if inflate:
         mask = iterate(mask, core.std.Inflate, inflate)
 
@@ -49,15 +47,15 @@
         mask = iterate(mask, core.std.Maximum if xxpand[1] > 0 else core.std.Minimum, xxpand[1])
 
     return mask.std.Limiter()
 
 
 def descale_error_mask(
     clip: vs.VideoNode, rescaled: vs.VideoNode,
-    thr: float | list[float] = 0.38,
+    thr: float | list[float] = 0.038,
     expands: int | tuple[int, int, int] = (2, 2, 3),
     blur: int | float = 3, bwbias: int = 1, tr: int = 1
 ) -> vs.VideoNode:
     """
     Create an error mask from the original and rescaled clip.
 
     :param clip:        Original clip.
@@ -70,63 +68,51 @@
 
     :return:            Descale error mask.
     """
     assert clip.format and rescaled.format
 
     y, *chroma = split(clip)
 
-    bit_depth = get_depth(clip)
-    neutral = get_neutral_value(clip)
-
     error = norm_expr([y, rescaled], 'x y - abs')
 
     if bwbias > 1 and chroma:
-        chroma_abs = norm_expr(chroma, f'x {neutral} - abs y {neutral} - abs max')
-        chroma_abs = Catrom().scale(chroma_abs, y.width, y.height)
+        chroma_abs = norm_expr(chroma, 'x range_half - abs y range_half - abs max')
+        chroma_abs = Catrom.scale(chroma_abs, y.width, y.height)
 
-        tv_low, tv_high = scale_value(16, 8, bit_depth), scale_value(235, 8, bit_depth)
-        bias = norm_expr([y, chroma_abs], f'x {tv_high} >= x {tv_low} <= or y 0 = and {bwbias} 1 ?')
+        bias = norm_expr([y, chroma_abs], f'x ymax >= x ymin <= or y 0 = and {bwbias} 1 ?')
         bias = Morpho.expand(bias, 2)
 
-        error = norm_expr([error, bias], 'x y *')
+        error = ExprOp.MUL(error, bias)
 
     if isinstance(expands, int):
         exp1 = exp2 = exp3 = expands
     else:
         exp1, exp2, exp3 = expands
 
-    assert exp1
-
-    error = Morpho.expand(error, exp1)
+    if exp1:
+        error = Morpho.expand(error, exp1)
 
     if exp2:
         error = Morpho.expand(error, exp2, mode=XxpandMode.ELLIPSE)
 
-    scaled_thrs = [
-        scale_value(val / 10, 32, bit_depth)
-        for val in ([thr] if isinstance(thr, float) else thr)
-    ]
+    thrs = [thr] if isinstance(thr, float) else thr
 
-    error = error.std.Binarize(scaled_thrs[0])
+    error = Morpho.binarize(error, thrs[0])
 
-    for scaled_thr in scaled_thrs[1:]:
-        bin2 = error.std.Binarize(scaled_thr)
+    for scaled_thr in thrs[1:]:
+        bin2 = Morpho.binarize(error, scaled_thr)
         error = bin2.misc.Hysteresis(error)
 
     if exp3:
         error = Morpho.expand(error, exp2, mode=XxpandMode.ELLIPSE)
 
     if tr > 1:
-        avg = average_merge(*shift_clip_multi(error, (-tr, tr))).std.Binarize(neutral)
-
-        _error = combine([error, avg], ExprOp.MIN)
-        shifted = shift_clip_multi(_error, (-tr, tr))
-        _error = combine(shifted, ExprOp.MAX)
+        avg = Morpho.binarize(average_merge(*shift_clip_multi(error, (-tr, tr))), 0.5)
 
-        error = combine([error, _error], ExprOp.MIN)
+        error = ExprOp.MIN(error, ExprOp.MAX(shift_clip_multi(ExprOp.MIN(error, avg), (-tr, tr))))
 
     if isinstance(blur, int):
         error = box_blur(error, blur)
     else:
         error = gauss_blur(error, blur)
 
     return error.std.Limiter()
```

### Comparing `vsscale-1.8.0/vsscale/scale.py` & `vsscale-1.9.0/vsscale/scale.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dataclasses import dataclass, field
 from functools import partial
 from math import ceil, floor, log2
 from typing import Any, Literal
 
 from vsexprtools import complexpr_available, expr_func, norm_expr
-from vskernels import Scaler, ScalerT, SetsuCubic, ZewiaCubic
+from vskernels import ScalerT, SetsuCubic, ZewiaCubic
 from vsrgtools import box_blur, gauss_blur
 from vstools import (
     DependencyNotFoundError, KwargsT, Matrix, MatrixT, PlanesT, Transfer, VSFunction, check_ref_clip, check_variable,
     core, depth, fallback, get_depth, get_nvidia_version, inject_self, padder, vs
 )
 
 from .gamma import gamma2linear, linear2gamma
@@ -46,17 +46,17 @@
         self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0), **kwargs: Any
     ) -> vs.VideoNode:
         ref = clip
 
         if isinstance(self.ref, vs.VideoNode):
             check_ref_clip(clip, self.ref)  # type: ignore
             ref = self.ref  # type: ignore
-            scaler = Scaler.ensure_obj(self.scaler, self.__class__)
+            scaler = self.ensure_scaler(self.scaler)
         else:
-            scaler = Scaler.ensure_obj(self.ref, self.__class__)  # type: ignore
+            scaler = self.ensure_scaler(self.ref)  # type: ignore
 
         if (ref.width, ref.height) != (width, height):
             ref = scaler.scale(ref, width, height)
 
         kwargs |= {
             'lambda_': self.sigma, 'planes': self.planes,
             'src_left': shift[1], 'src_top': shift[0]
@@ -275,14 +275,16 @@
                 core.log_message(
                     vs.MESSAGE_TYPE_DEBUG,
                     f'Selected [{data.get("name", b"<unknown>").decode("utf8")}] '
                     f'with {f"{(memory / (1 << 30))}GiB" if memory else "<unknown>"} of VRAM, '
                     f'num_streams={def_num_streams} ({streams_info})'
                 )
             except Exception:
+                self.fp16 = False
+                bkwargs['fp16'] = False
                 cuda = get_nvidia_version() is not None
 
         if bkwargs.get('num_streams', None) is None:
             bkwargs.update(num_streams=fallback(self.num_streams, 1))
 
         if cuda is True:
             if hasattr(core, 'ort'):
```

### Comparing `vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl` & `vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl` & `vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl` & `vsscale-1.9.0/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/shaders/SSimDownscaler.glsl` & `vsscale-1.9.0/vsscale/shaders/SSimDownscaler.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/shaders/SSimSuperRes.glsl` & `vsscale-1.9.0/vsscale/shaders/SSimSuperRes.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/shaders.py` & `vsscale-1.9.0/vsscale/shaders.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale/types.py` & `vsscale-1.9.0/vsscale/types.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.8.0/vsscale.egg-info/PKG-INFO` & `vsscale-1.9.0/vsscale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsscale
-Version: 1.8.0
+Version: 1.9.0
 Summary: VapourSynth (de)scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-scale
 Project-URL: Documentation, https://vsscale.encode.moe/en/latest/
```

### Comparing `vsscale-1.8.0/vsscale.egg-info/SOURCES.txt` & `vsscale-1.9.0/vsscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

