# Comparing `tmp/autosrt-1.3.3.tar.gz` & `tmp/autosrt-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.3.3.tar", last modified: Sun Jun  4 20:45:44 2023, max compression
+gzip compressed data, was "autosrt-1.3.4.tar", last modified: Mon Jun  5 01:31:00 2023, max compression
```

## Comparing `autosrt-1.3.3.tar` & `autosrt-1.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 20:45:44.870473 autosrt-1.3.3/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.3/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-04 20:45:44.871217 autosrt-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 20:45:44.820269 autosrt-1.3.3/autosrt/
--rw-rw-rw-   0        0        0    15610 2023-06-04 20:19:47.000000 autosrt-1.3.3/autosrt/__init__.py
--rw-rw-rw-   0        0        0    71573 2023-06-04 20:45:08.000000 autosrt-1.3.3/autosrt/autosrt.py
-drwxrwxrwx   0        0        0        0 2023-06-04 20:45:44.854735 autosrt-1.3.3/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-04 20:45:44.000000 autosrt-1.3.3/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-06-04 20:45:44.000000 autosrt-1.3.3/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 20:45:44.000000 autosrt-1.3.3/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-04 20:45:44.000000 autosrt-1.3.3/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-04 20:45:44.000000 autosrt-1.3.3/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-04 20:45:44.000000 autosrt-1.3.3/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-04 20:45:44.874962 autosrt-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 20:45:44.867469 autosrt-1.3.3/test/
--rw-rw-rw-   0        0        0     7362 2023-05-03 15:20:29.000000 autosrt-1.3.3/test/test1.py
--rw-rw-rw-   0        0        0     4465 2023-05-02 21:51:09.000000 autosrt-1.3.3/test/test2.py
--rw-rw-rw-   0        0        0     9939 2023-05-03 13:45:31.000000 autosrt-1.3.3/test/test3.py
--rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.3/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:31:00.878979 autosrt-1.3.4/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-06-05 01:31:00.878979 autosrt-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 01:31:00.837025 autosrt-1.3.4/autosrt/
+-rw-rw-rw-   0        0        0    16163 2023-06-05 01:30:32.000000 autosrt-1.3.4/autosrt/__init__.py
+-rw-rw-rw-   0        0        0    71573 2023-06-05 01:26:11.000000 autosrt-1.3.4/autosrt/autosrt.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:31:00.858751 autosrt-1.3.4/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 01:31:00.000000 autosrt-1.3.4/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-05 01:31:00.883475 autosrt-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:31:00.875983 autosrt-1.3.4/test/
+-rw-rw-rw-   0        0        0     7362 2023-05-03 15:20:29.000000 autosrt-1.3.4/test/test1.py
+-rw-rw-rw-   0        0        0     4465 2023-05-02 21:51:09.000000 autosrt-1.3.4/test/test2.py
+-rw-rw-rw-   0        0        0     9939 2023-05-03 13:45:31.000000 autosrt-1.3.4/test/test3.py
+-rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.4/test/test4.py
```

### Comparing `autosrt-1.3.3/LICENSE` & `autosrt-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.3/PKG-INFO` & `autosrt-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.3
+Version: 1.3.4
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.3/README.md` & `autosrt-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.3/autosrt/__init__.py` & `autosrt-1.3.4/autosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,42 @@
 import sys
 import multiprocessing
 from glob import glob, escape
 from progressbar import ProgressBar, Percentage, Bar, ETA
 import time
 from datetime import datetime, timedelta
 from pathlib import Path
+import subprocess
 
 from .autosrt import VERSION, Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
     SubtitleFormatter,  SubtitleWriter, MediaSubtitleRenderer, stop_ffmpeg_windows, stop_ffmpeg_linux, remove_temp_files, \
     is_same_language, check_file_type
 
+def has_subtitles(media_filepath):
+    if "\\" in media_filepath:
+        media_filepath = media_filepath.replace("\\", "/")
+
+    ffmpeg_cmd = [
+        "ffmpeg",
+        "-y",
+        "-i", media_filepath,
+        "-map", "0:s:0",
+        "-f", "srt",
+        "-"
+    ]
+
+    result = subprocess.run(ffmpeg_cmd, capture_output=True, text=True)
+    #print(result.stdout)
+    #print(result.stderr)
+
+    if result.stdout:
+        return True  # Subtitles detected
+    else:
+        return False  # No subtitles detected
+
 def show_progress(media_filepath, progress):
     global pbar
     pbar.update(progress)
 
 def show_error_messages(messages):
     print(messages)
 
@@ -168,15 +191,15 @@
 
     transcribe_end_time = None
     transcribe_elapsed_time = None
     transcribe_start_time = time.time()
     rendered_media_filepath = None
 
     for media_filepath in media_filepaths:
-        if ".rendered." in str(media_filepath):
+        if has_subtitles(media_filepath):
             media_filepaths.remove(media_filepath)
 
     for media_filepath in media_filepaths:
         print("Processing {}".format(media_filepath))
 
         try:
             widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
```

### Comparing `autosrt-1.3.3/autosrt/autosrt.py` & `autosrt-1.3.4/autosrt/autosrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 except ImportError:
     JSONDecodeError = ValueError
 from progressbar import ProgressBar, Percentage, Bar, ETA
 import pysrt
 import six
 import shlex
 
-VERSION = "1.3.3"
+VERSION = "1.3.4"
 
 
 #======================================================== ffmpeg_progress_yield ========================================================#
 
 
 import re
 #import subprocess
```

### Comparing `autosrt-1.3.3/autosrt.egg-info/PKG-INFO` & `autosrt-1.3.4/autosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.3
+Version: 1.3.4
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.3/setup.py` & `autosrt-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.3/test/test1.py` & `autosrt-1.3.4/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.3/test/test2.py` & `autosrt-1.3.4/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.3/test/test3.py` & `autosrt-1.3.4/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.3/test/test4.py` & `autosrt-1.3.4/test/test4.py`

 * *Files identical despite different names*

