# Comparing `tmp/vsmuxtools-0.0.4.tar.gz` & `tmp/vsmuxtools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmuxtools-0.0.4.tar", last modified: Sun Jun  4 11:43:22 2023, max compression
+gzip compressed data, was "vsmuxtools-0.0.5.tar", last modified: Mon Jun  5 19:50:46 2023, max compression
```

## Comparing `vsmuxtools-0.0.4.tar` & `vsmuxtools-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.737438 vsmuxtools-0.0.4/
--rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      994 2023-06-04 11:43:22.737438 vsmuxtools-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-05-27 19:14:49.000000 vsmuxtools-0.0.4/README.md
--rw-rw-rw-   0        0        0     1078 2023-06-04 11:42:11.000000 vsmuxtools-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 11:43:22.737438 vsmuxtools-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.722896 vsmuxtools-0.0.4/vsmuxtools/
--rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.4/vsmuxtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.732410 vsmuxtools-0.0.4/vsmuxtools/extension/
--rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.4/vsmuxtools/extension/__init__.py
--rw-rw-rw-   0        0        0     2717 2023-05-31 21:39:04.000000 vsmuxtools-0.0.4/vsmuxtools/extension/audio.py
--rw-rw-rw-   0        0        0     1477 2023-06-04 11:42:52.000000 vsmuxtools-0.0.4/vsmuxtools/extension/chapters.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.734409 vsmuxtools-0.0.4/vsmuxtools/utils/
--rw-rw-rw-   0        0        0       84 2023-05-30 16:15:03.000000 vsmuxtools-0.0.4/vsmuxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     7915 2023-05-31 20:52:56.000000 vsmuxtools-0.0.4/vsmuxtools/utils/src.py
--rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.4/vsmuxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.736410 vsmuxtools-0.0.4/vsmuxtools/video/
--rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.4/vsmuxtools/video/__init__.py
--rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.4/vsmuxtools/video/encoders.py
--rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.4/vsmuxtools/video/resumable.py
--rw-rw-rw-   0        0        0     9999 2023-05-30 16:43:59.000000 vsmuxtools-0.0.4/vsmuxtools/video/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.730409 vsmuxtools-0.0.4/vsmuxtools.egg-info/
--rw-rw-rw-   0        0        0      994 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.089028 vsmuxtools-0.0.5/
+-rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      994 2023-06-05 19:50:46.089028 vsmuxtools-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-05-27 19:14:49.000000 vsmuxtools-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1078 2023-06-05 18:41:57.000000 vsmuxtools-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 19:50:46.089028 vsmuxtools-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.069854 vsmuxtools-0.0.5/vsmuxtools/
+-rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.5/vsmuxtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.083755 vsmuxtools-0.0.5/vsmuxtools/extension/
+-rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.5/vsmuxtools/extension/__init__.py
+-rw-rw-rw-   0        0        0     2717 2023-05-31 21:39:04.000000 vsmuxtools-0.0.5/vsmuxtools/extension/audio.py
+-rw-rw-rw-   0        0        0     1477 2023-06-04 11:42:52.000000 vsmuxtools-0.0.5/vsmuxtools/extension/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.085755 vsmuxtools-0.0.5/vsmuxtools/utils/
+-rw-rw-rw-   0        0        0       84 2023-05-30 16:15:03.000000 vsmuxtools-0.0.5/vsmuxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     7943 2023-06-04 12:11:30.000000 vsmuxtools-0.0.5/vsmuxtools/utils/src.py
+-rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.5/vsmuxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.088028 vsmuxtools-0.0.5/vsmuxtools/video/
+-rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.5/vsmuxtools/video/__init__.py
+-rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.5/vsmuxtools/video/encoders.py
+-rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.5/vsmuxtools/video/resumable.py
+-rw-rw-rw-   0        0        0    10096 2023-06-05 18:38:29.000000 vsmuxtools-0.0.5/vsmuxtools/video/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:50:46.081754 vsmuxtools-0.0.5/vsmuxtools.egg-info/
+-rw-rw-rw-   0        0        0      994 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 19:50:46.000000 vsmuxtools-0.0.5/vsmuxtools.egg-info/top_level.txt
```

### Comparing `vsmuxtools-0.0.4/LICENSE` & `vsmuxtools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.4/PKG-INFO` & `vsmuxtools-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.4
+Version: 0.0.5
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.4/pyproject.toml` & `vsmuxtools-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 [project]
 name = "vsmuxtools"
-version = "0.0.4"
+version = "0.0.5"
 description = "The extension to muxtools with vapoursynth and encoding stuff"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "vapoursynth>=60",
     "vstools>=1.6.2",
-    "muxtools>=0.0.3",
+    "muxtools>=0.0.5",
 ]
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
```

### Comparing `vsmuxtools-0.0.4/vsmuxtools/extension/audio.py` & `vsmuxtools-0.0.5/vsmuxtools/extension/audio.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.4/vsmuxtools/extension/chapters.py` & `vsmuxtools-0.0.5/vsmuxtools/extension/chapters.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.4/vsmuxtools/utils/src.py` & `vsmuxtools-0.0.5/vsmuxtools/utils/src.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,30 +63,30 @@
     @property
     def src_cut(self) -> vs.VideoNode:
         if not hasattr(self, "clip_cut"):
             self.__index_clip()
         return self.clip_cut
 
     @copy_signature(initialize_clip)
-    def init(self, **kwargs) -> vs.VideoNode:
+    def init(self, *args, **kwargs) -> vs.VideoNode:
         """
         Getter that calls `vstools.initialize_clip` on the src clip for convenience
 
         :param kwargs:      Any other args passed to initialize_clip
         """
-        return initialize_clip(self.src, **kwargs)
+        return initialize_clip(self.src, *args, **kwargs)
 
     @copy_signature(initialize_clip)
-    def init_cut(self, **kwargs) -> vs.VideoNode:
+    def init_cut(self, *args, **kwargs) -> vs.VideoNode:
         """
         Getter that calls `vstools.initialize_clip` on the src_cut clip for convenience
 
         :param kwargs:      Any other args passed to initialize_clip
         """
-        return initialize_clip(self.src_cut, **kwargs)
+        return initialize_clip(self.src_cut, *args, **kwargs)
 
     def get_audio(self, track: int = 0, **kwargs) -> vs.AudioNode:
         """
         Indexes the specified audio track from the input file.
         """
         args = dict(exact=True)
         args.update(**kwargs)
```

### Comparing `vsmuxtools-0.0.4/vsmuxtools/video/encoders.py` & `vsmuxtools-0.0.5/vsmuxtools/video/encoders.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.4/vsmuxtools/video/resumable.py` & `vsmuxtools-0.0.5/vsmuxtools/video/resumable.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.4/vsmuxtools/video/settings.py` & `vsmuxtools-0.0.5/vsmuxtools/video/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+from genericpath import isfile
 import re
+import os
 from tracemalloc import start
 from muxtools import error, PathLike, ensure_path, warn
 from vstools import vs, Matrix, Primaries, Transfer, ColorRange, ChromaLocation, get_prop, Colorspace
 from ..utils.types import Zone
 
 __all__ = ["settings_builder_x265", "settings_builder_x264", "sb", "sb265", "sb264"]
 
@@ -163,22 +165,22 @@
 sb265 = sb
 sb264 = settings_builder_x264
 
 
 def file_or_default(file: PathLike, default: str, no_warn: bool = False) -> tuple[str | list[str], bool]:
     if isinstance(file, list):
         return file, False
-    file = ensure_path(file, None)
-
-    if file.exists():
-        with open(file, "r") as r:
-            settings = str(r.read())
-            settings = settings.replace("\n", " ")
-            settings = re.sub(r"(?:-o|--output) {clip.+?}", "", settings, flags=re.I).strip()
-            return settings, True
+    if os.path.isfile(file):
+        file = ensure_path(file, None)
+        if file.exists():
+            with open(file, "r") as r:
+                settings = str(r.read())
+                settings = settings.replace("\n", " ")
+                settings = re.sub(r"(?:-o|--output) {clip.+?}", "", settings, flags=re.I).strip()
+                return settings, True
 
     if not no_warn:
         warn("Settings file wasn't found. Using default.", None, 3)
     return default, False
 
 
 def get_props(clip: vs.VideoNode, x265: bool) -> dict[str, str]:
```

### Comparing `vsmuxtools-0.0.4/vsmuxtools.egg-info/PKG-INFO` & `vsmuxtools-0.0.5/vsmuxtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.4
+Version: 0.0.5
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.4/vsmuxtools.egg-info/SOURCES.txt` & `vsmuxtools-0.0.5/vsmuxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

