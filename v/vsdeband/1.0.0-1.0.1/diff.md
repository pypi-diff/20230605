# Comparing `tmp/vsdeband-1.0.0.tar.gz` & `tmp/vsdeband-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdeband-1.0.0.tar", last modified: Thu May  4 21:59:35 2023, max compression
+gzip compressed data, was "vsdeband-1.0.1.tar", last modified: Mon Jun  5 14:34:30 2023, max compression
```

## Comparing `vsdeband-1.0.0.tar` & `vsdeband-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:35.128878 vsdeband-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 21:59:08.000000 vsdeband-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-04 21:59:35.128878 vsdeband-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 21:59:08.000000 vsdeband-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 21:59:35.128878 vsdeband-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-04 21:59:08.000000 vsdeband-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:35.124879 vsdeband-1.0.0/vsdeband/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/f3kdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/placebo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 21:59:08.000000 vsdeband-1.0.0/vsdeband/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:35.128878 vsdeband-1.0.0/vsdeband.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 21:59:35.000000 vsdeband-1.0.0/vsdeband.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:34:30.341065 vsdeband-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 14:34:04.000000 vsdeband-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 14:34:30.341065 vsdeband-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-05 14:34:04.000000 vsdeband-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-05 14:34:30.341065 vsdeband-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-05 14:34:04.000000 vsdeband-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:34:30.341065 vsdeband-1.0.1/vsdeband/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/f3kdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/placebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-05 14:34:04.000000 vsdeband-1.0.1/vsdeband/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:34:30.341065 vsdeband-1.0.1/vsdeband.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 14:34:30.000000 vsdeband-1.0.1/vsdeband.egg-info/top_level.txt
```

### Comparing `vsdeband-1.0.0/LICENSE` & `vsdeband-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.0/PKG-INFO` & `vsdeband-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdeband
-Version: 1.0.0
+Version: 1.0.1
 Summary: VapourSynth Debanding Functions Collection
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-deband
 Project-URL: Documentation, https://vsdeband.encode.moe/en/latest/
```

### Comparing `vsdeband-1.0.0/setup.cfg` & `vsdeband-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.0/setup.py` & `vsdeband-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.0/vsdeband/f3kdb.py` & `vsdeband-1.0.1/vsdeband/f3kdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             raise CustomRuntimeError('You are missing the neo_f3kdb plugin!', func.func)
 
         if 'y_2' not in core.neo_f3kdb.Deband.__signature__.parameters:  # type: ignore
             raise CustomRuntimeError('You are using an outdated version of neo_f3kdb, upgrade now!', func.func)
 
         radius = fallback(self.radius, radius)
 
-        y, cb, cr = func.norm_seq(fallback(self.thr, thr))
+        y, cb, cr = normalize_seq(fallback(self.thr, thr), 3)
         gry, grc = normalize_seq(fallback(self.grain, grain), 2)
 
         sample_mode = fallback(self.sample_mode, sample_mode)  # type: ignore
 
         color_range = ColorRange.from_param(
             color_range, self.deband
         ) or ColorRange.from_video(func.work_clip, func=func.func)
```

### Comparing `vsdeband-1.0.0/vsdeband/filters.py` & `vsdeband-1.0.1/vsdeband/filters.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.0/vsdeband/funcs.py` & `vsdeband-1.0.1/vsdeband/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     return depth(limit, bits)
 
 
 def masked_deband(
     clip: vs.VideoNode, radius: int = 16,
     thr: float | list[float] = 96, grain: float | list[float] = [0.23, 0],
     sigma: float = 1.25, rxsigma: list[int] = [50, 220, 300],
-    pf_sigma: float | None = 1.25, brz: tuple[int, int] = (0.38, 0.68),
+    pf_sigma: float | None = 1.25, brz: tuple[float, float] = (0.038, 0.068),
     rg_mode: RemoveGrainModeT = RemoveGrainMode.MINMAX_MEDIAN_OPP,
     debander: type[Debander] | Debander = F3kdb, **kwargs: Any
 ) -> vs.VideoNode:
     clip, bits = expect_bits(clip, 16)
 
     if not isinstance(debander, Debander):
         debander = debander()
```

### Comparing `vsdeband-1.0.0/vsdeband/mask.py` & `vsdeband-1.0.1/vsdeband/mask.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 __all__ = [
     'deband_detail_mask'
 ]
 
 
 def deband_detail_mask(
     clip: vs.VideoNode, sigma: float = 1.0, rxsigma: list[int] = [50, 200, 350],
-    pf_sigma: float | None = 1.0, brz: tuple[float, float] = (0.38, 0.68),
+    pf_sigma: float | None = 1.0, brz: tuple[float, float] = (0.038, 0.068),
     rg_mode: RemoveGrainModeT = RemoveGrainMode.MINMAX_MEDIAN_OPP
 ) -> vs.VideoNode:
     clip_y = get_y(clip)
 
     ret = retinex(
         clip_y if pf_sigma is None else gauss_blur(clip_y, pf_sigma), rxsigma, upper_thr=0.005
     )
 
-    brz0, brz1 = (br / 10 for br in brz)
+    brz0, brz1 = brz
 
     blur_ret = gauss_blur(ret, sigma)
     blur_ret_diff = Morpho.deflate(ExprOp.SUB(blur_ret, ret))
 
     blur_ret_brz = Morpho.inflate(blur_ret_diff, 4)
     blur_ret_brz = Morpho.closing(Morpho.binarize(blur_ret_brz, brz0), coords=8)
```

### Comparing `vsdeband-1.0.0/vsdeband/noise.py` & `vsdeband-1.0.1/vsdeband/noise.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.0/vsdeband/placebo.py` & `vsdeband-1.0.1/vsdeband/placebo.py`

 * *Files identical despite different names*

### Comparing `vsdeband-1.0.0/vsdeband.egg-info/PKG-INFO` & `vsdeband-1.0.1/vsdeband.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdeband
-Version: 1.0.0
+Version: 1.0.1
 Summary: VapourSynth Debanding Functions Collection
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Irrational Encoding Wizardry
 Maintainer-email: wizards@encode.moe
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-deband
 Project-URL: Documentation, https://vsdeband.encode.moe/en/latest/
```

