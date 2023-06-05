# Comparing `tmp/vskernels-2.4.0.tar.gz` & `tmp/vskernels-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vskernels-2.4.0.tar", last modified: Thu May  4 22:00:14 2023, max compression
+gzip compressed data, was "vskernels-2.4.1.tar", last modified: Mon Jun  5 13:58:43 2023, max compression
```

## Comparing `vskernels-2.4.0.tar` & `vskernels-2.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:14.525055 vskernels-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 21:59:44.000000 vskernels-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-04 22:00:14.525055 vskernels-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-04 21:59:44.000000 vskernels-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 22:00:14.525055 vskernels-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-04 21:59:44.000000 vskernels-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:14.521055 vskernels-2.4.0/vskernels/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:14.525055 vskernels-2.4.0/vskernels/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/bicubic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/fmtconv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/impulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/placebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/kernels/various.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-04 21:59:44.000000 vskernels-2.4.0/vskernels/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:14.525055 vskernels-2.4.0/vskernels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 22:00:14.000000 vskernels-2.4.0/vskernels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:43.740913 vskernels-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 13:58:06.000000 vskernels-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-05 13:58:43.740913 vskernels-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-05 13:58:06.000000 vskernels-2.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-05 13:58:43.740913 vskernels-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-05 13:58:06.000000 vskernels-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:43.736913 vskernels-2.4.1/vskernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:43.740913 vskernels-2.4.1/vskernels/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/bicubic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/fmtconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/placebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/kernels/various.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-05 13:58:06.000000 vskernels-2.4.1/vskernels/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:43.736913 vskernels-2.4.1/vskernels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-05 13:58:43.000000 vskernels-2.4.1/vskernels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-05 13:58:43.000000 vskernels-2.4.1/vskernels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:58:43.000000 vskernels-2.4.1/vskernels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 13:58:43.000000 vskernels-2.4.1/vskernels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 13:58:43.000000 vskernels-2.4.1/vskernels.egg-info/top_level.txt
```

### Comparing `vskernels-2.4.0/LICENSE` & `vskernels-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/PKG-INFO` & `vskernels-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vskernels
-Version: 2.4.0
+Version: 2.4.1
 Summary: Kernel objects for scaling and format conversion within VapourSynth
 Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-kernels
 Project-URL: Documentation, https://vskernels.encode.moe/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vskernels Version: 2.4.0 Summary: Kernel objects
+Metadata-Version: 2.1 Name: vskernels Version: 2.4.1 Summary: Kernel objects
 for scaling and format conversion within VapourSynth Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev Project-URL: Source Code, https://
 github.com/Irrational-Encoding-Wizardry/vs-kernels Project-URL: Documentation,
 https://vskernels.encode.moe/en/latest/ Project-URL: Contact, https://
 discord.gg/qxTxVJGtst Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Other Audience
```

### Comparing `vskernels-2.4.0/README.md` & `vskernels-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/setup.cfg` & `vskernels-2.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/setup.py` & `vskernels-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/__init__.py` & `vskernels-2.4.1/vskernels/__init__.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/exceptions.py` & `vskernels-2.4.1/vskernels/exceptions.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/kernels/abstract.py` & `vskernels-2.4.1/vskernels/kernels/abstract.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/kernels/bicubic.py` & `vskernels-2.4.1/vskernels/kernels/bicubic.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/kernels/docs.py` & `vskernels-2.4.1/vskernels/kernels/docs.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/kernels/fmtconv.py` & `vskernels-2.4.1/vskernels/kernels/fmtconv.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     * fmtconv
     """
 
     def scale_function(self, clip: vs.VideoNode, **kwargs: Any) -> vs.VideoNode:
         assert clip.format
 
-        def _check_fmt(fmt: int | vs.PresetFormat | vs.VideoFormat) -> tuple[vs.VideoFormat, bool]:
+        def _check_fmt(fmt: int | VideoFormatT) -> tuple[vs.VideoFormat, bool]:
             fmt = core.get_video_format(fmt)
 
             return fmt, ((
                 fmt.bits_per_sample == 32 and fmt.sample_type == vs.FLOAT
             ) or (
                 fmt.bits_per_sample == 16 and fmt.sample_type == vs.INTEGER
             ))
```

### Comparing `vskernels-2.4.0/vskernels/kernels/impulse.py` & `vskernels-2.4.1/vskernels/kernels/impulse.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/kernels/placebo.py` & `vskernels-2.4.1/vskernels/kernels/placebo.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/kernels/resize.py` & `vskernels-2.4.1/vskernels/kernels/resize.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/kernels/spline.py` & `vskernels-2.4.1/vskernels/kernels/spline.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/kernels/various.py` & `vskernels-2.4.1/vskernels/kernels/various.py`

 * *Files identical despite different names*

### Comparing `vskernels-2.4.0/vskernels/util.py` & `vskernels-2.4.1/vskernels/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,22 +75,22 @@
     ) -> vs.VideoNode:
         try:
             return super().scale(clip, clip.width, clip.height, shift, **kwargs)  # type: ignore
         except Exception:
             return clip
 
 
-class NoScale(Bicubic, NoScaleBase):  # type: ignore
+class NoScale(NoScaleBase, Bicubic):  # type: ignore
     def __class_getitem__(cls, kernel: KernelT) -> type[Kernel]:
         return cls.from_kernel(kernel)
 
     @staticmethod
     def from_kernel(kernel: KernelT) -> type[Kernel]:
         kernel_t = Kernel.from_param(kernel)
 
-        class inner_no_shift(NoScaleBase, kernel_t):  # type: ignore
+        class inner_no_scale(kernel_t, NoScaleBase):  # type: ignore
             ...
 
-        return inner_no_shift
+        return inner_no_scale
 
 
 excluded_kernels = [Kernel, FmtConv, Example, Impulse, Placebo, NoShiftBase, NoScaleBase]
```

### Comparing `vskernels-2.4.0/vskernels.egg-info/PKG-INFO` & `vskernels-2.4.1/vskernels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vskernels
-Version: 2.4.0
+Version: 2.4.1
 Summary: Kernel objects for scaling and format conversion within VapourSynth
 Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-kernels
 Project-URL: Documentation, https://vskernels.encode.moe/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vskernels Version: 2.4.0 Summary: Kernel objects
+Metadata-Version: 2.1 Name: vskernels Version: 2.4.1 Summary: Kernel objects
 for scaling and format conversion within VapourSynth Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev Project-URL: Source Code, https://
 github.com/Irrational-Encoding-Wizardry/vs-kernels Project-URL: Documentation,
 https://vskernels.encode.moe/en/latest/ Project-URL: Contact, https://
 discord.gg/qxTxVJGtst Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Other Audience
```

### Comparing `vskernels-2.4.0/vskernels.egg-info/SOURCES.txt` & `vskernels-2.4.1/vskernels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

