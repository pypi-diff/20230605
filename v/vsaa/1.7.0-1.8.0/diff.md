# Comparing `tmp/vsaa-1.7.0.tar.gz` & `tmp/vsaa-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsaa-1.7.0.tar", last modified: Thu May  4 21:58:48 2023, max compression
+gzip compressed data, was "vsaa-1.8.0.tar", last modified: Mon Jun  5 14:02:39 2023, max compression
```

## Comparing `vsaa-1.7.0.tar` & `vsaa-1.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:48.346152 vsaa-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 21:58:22.000000 vsaa-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-04 21:58:48.346152 vsaa-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-04 21:58:22.000000 vsaa-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:58:48.346152 vsaa-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-04 21:58:22.000000 vsaa-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:48.346152 vsaa-1.7.0/vsaa/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:48.346152 vsaa-1.7.0/vsaa/antialiasers/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/eedi2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/eedi3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/nnedi3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/sangnom.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:48.346152 vsaa-1.7.0/vsaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:39.465671 vsaa-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-05 14:02:15.000000 vsaa-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 14:02:39.465671 vsaa-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-05 14:02:15.000000 vsaa-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 14:02:39.465671 vsaa-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-05 14:02:15.000000 vsaa-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:39.461671 vsaa-1.8.0/vsaa/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:39.465671 vsaa-1.8.0/vsaa/antialiasers/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/antialiasers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/antialiasers/eedi2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/antialiasers/eedi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/antialiasers/nnedi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/antialiasers/sangnom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:15.000000 vsaa-1.8.0/vsaa/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:39.465671 vsaa-1.8.0/vsaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 14:02:39.000000 vsaa-1.8.0/vsaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-05 14:02:39.000000 vsaa-1.8.0/vsaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:02:39.000000 vsaa-1.8.0/vsaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-05 14:02:39.000000 vsaa-1.8.0/vsaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 14:02:39.000000 vsaa-1.8.0/vsaa.egg-info/top_level.txt
```

### Comparing `vsaa-1.7.0/LICENSE` & `vsaa-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsaa-1.7.0/PKG-INFO` & `vsaa-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsaa
-Version: 1.7.0
+Version: 1.8.0
 Summary: VapourSynth anti aliasing and scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-aa
 Project-URL: Documentation, https://vsaa.encode.moe/en/latest/
```

### Comparing `vsaa-1.7.0/setup.cfg` & `vsaa-1.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsaa-1.7.0/setup.py` & `vsaa-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.7.0/vsaa/abstract.py` & `vsaa-1.8.0/vsaa/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 
 
 @dataclass
 class _Antialiaser(_SingleInterpolate):
     field: int = dc_field(default=0, kw_only=True)
     drop_fields: bool = dc_field(default=True, kw_only=True)
     transpose_first: bool = dc_field(default=False, kw_only=True)
-    shifter: KernelT = dc_field(default=Catrom(), kw_only=True)
+    shifter: KernelT | None = dc_field(default=None, kw_only=True)
     scaler: ScalerT | None = dc_field(default=None, kw_only=True)
 
     def __post_init__(self) -> None:
         super().__post_init__()
 
-        self._shifter = Kernel.ensure_obj(self.shifter, self.__class__)
+        self._shifter = Kernel.ensure_obj(self.shifter or Catrom, self.__class__)
         self._scaler = None if self.scaler is None else Scaler.ensure_obj(self.scaler, self.__class__)
 
     def preprocess_clip(self, clip: vs.VideoNode) -> vs.VideoNode:
         return clip
 
     def get_aa_args(self, clip: vs.VideoNode, **kwargs: Any) -> dict[str, Any]:
         return {}
```

### Comparing `vsaa-1.7.0/vsaa/antialiasers/eedi2.py` & `vsaa-1.8.0/vsaa/antialiasers/eedi2.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.7.0/vsaa/antialiasers/eedi3.py` & `vsaa-1.8.0/vsaa/antialiasers/eedi3.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,15 @@
 
         if self._sclip_aa and ((('sclip' in kwargs) and not kwargs['sclip']) or 'sclip' not in kwargs):
             if self._sclip_aa is True:
                 if double_y:
                     raise CustomValueError("You can't pass sclip_aa=True when supersampling!", self.__class__)
                 aa_kwargs.update(sclip=clip)
             else:
-                sclip_args = self._sclip_aa.get_aa_args(
-                    clip, **(dict(mclip=kwargs.get('clip') if 'mclip' in kwargs else {}))
-                )
+                sclip_args = self._sclip_aa.get_aa_args(clip, **(dict(mclip=kwargs.get('mclip', None))))
 
                 if double_y:
                     sclip_args |= self._sclip_aa.get_ss_args(clip)
                 else:
                     sclip_args |= self._sclip_aa.get_sr_args(clip)
 
                 aa_kwargs.update(
```

### Comparing `vsaa-1.7.0/vsaa/antialiasers/nnedi3.py` & `vsaa-1.8.0/vsaa/antialiasers/nnedi3.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,24 @@
 class NNEDI3(_FullInterpolate, _Antialiaser):
     nsize: int = 0
     nns: int = 4
     qual: int = 2
     etype: int = 0
     pscrn: int = 1
 
-    opencl: bool = False
+    opencl: bool | None = None
+
+    def __post_init__(self) -> None:
+        super().__post_init__()
+
+        if self.opencl is None:
+            self.opencl = hasattr(core, 'sneedif')
 
     def is_full_interpolate_enabled(self, x: bool, y: bool) -> bool:
-        return self.opencl
+        return not not self.opencl
 
     def get_aa_args(self, clip: vs.VideoNode, **kwargs: Any) -> dict[str, Any]:
         assert clip.format
         is_float = clip.format.sample_type == vs.FLOAT
         pscrn = 1 if is_float else self.pscrn
         return dict(nsize=self.nsize, nns=self.nns, qual=self.qual, etype=self.etype, pscrn=pscrn)
 
@@ -37,15 +43,28 @@
         ).nnedi3(
             clip, self.field, double_y or not self.drop_fields, **kwargs
         )
 
         return self.shift_interpolate(clip, interpolated, double_y, **kwargs)
 
     def full_interpolate(self, clip: vs.VideoNode, double_y: bool, double_x: bool, **kwargs: Any) -> vs.VideoNode:
-        return core.nnedi3cl.NNEDI3CL(clip, self.field, double_y, double_x, **kwargs)
+        if hasattr(core, 'sneedif'):
+            clip = core.sneedif.NNEDI3(
+                clip, self.field, double_y, double_x, transpose_first=self.transpose_first, **kwargs
+            )
+        else:
+            if not self.transpose_first:
+                clip = clip.std.Transpose()
+
+            clip = core.nnedi3cl.NNEDI3CL(clip, self.field, double_y, double_x, **kwargs)
+
+            if not self.transpose_first:
+                clip = clip.std.Transpose()
+
+        return clip
 
     _shift = 0.5
 
 
 class Nnedi3SS(NNEDI3, SuperSampler):
     ...
```

### Comparing `vsaa-1.7.0/vsaa/antialiasers/sangnom.py` & `vsaa-1.8.0/vsaa/antialiasers/sangnom.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.7.0/vsaa/funcs.py` & `vsaa-1.8.0/vsaa/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     ssh = get_h(work_clip.width * rfactor, work_clip, 2)
     ssw = get_w(ssh, work_clip, 2)
 
     ssfunc = Scaler.ensure_obj(ssfunc, upscaled_sraa)
     downscaler = Scaler.ensure_obj(downscaler, upscaled_sraa)
 
     up = ssfunc.scale(work_clip, ssw, ssh)
-    up, *chroma = [up] if aa_chroma else (split(up) if scale_chroma else [up, *chroma])
+    up, *chroma = [up] if aa_chroma or scale_chroma else [up, *chroma]
 
     aa = aafunc.aa(up, *direction.to_yx())
 
     if downscaler:
         aa = downscaler.scale(aa, width, height)
 
     if not chroma:
```

### Comparing `vsaa-1.7.0/vsaa/mask.py` & `vsaa-1.8.0/vsaa/mask.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.7.0/vsaa.egg-info/PKG-INFO` & `vsaa-1.8.0/vsaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsaa
-Version: 1.7.0
+Version: 1.8.0
 Summary: VapourSynth anti aliasing and scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-aa
 Project-URL: Documentation, https://vsaa.encode.moe/en/latest/
```

