# Comparing `tmp/termux-api-1.2.4.tar.gz` & `tmp/termux-api-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termux-api-1.2.4.tar", last modified: Wed May 31 16:26:08 2023, max compression
+gzip compressed data, was "termux-api-1.2.5.tar", last modified: Mon Jun  5 17:51:01 2023, max compression
```

## Comparing `termux-api-1.2.4.tar` & `termux-api-1.2.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 16:26:08.644661 termux-api-1.2.4/
--rw-rw-rw-   0        0        0     1086 2022-06-29 16:50:48.000000 termux-api-1.2.4/LICENSE
--rw-rw-rw-   0        0        0     3621 2023-05-31 16:26:08.643661 termux-api-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3060 2022-06-30 07:05:02.000000 termux-api-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 16:26:08.644661 termux-api-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-05-31 16:21:50.000000 termux-api-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:26:08.637656 termux-api-1.2.4/termux/
--rw-rw-rw-   0        0        0     3513 2023-05-31 16:21:50.000000 termux-api-1.2.4/termux/API.py
--rw-rw-rw-   0        0        0      661 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Camera.py
--rw-rw-rw-   0        0        0      520 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Clipboard.py
--rw-rw-rw-   0        0        0     1269 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Media.py
--rw-rw-rw-   0        0        0     1293 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Microphone.py
--rw-rw-rw-   0        0        0     1237 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Notification.py
--rw-rw-rw-   0        0        0     2284 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Scheduler.py
--rw-rw-rw-   0        0        0     2241 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Sensors.py
--rw-rw-rw-   0        0        0     1105 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Share.py
--rw-rw-rw-   0        0        0     1112 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/TTS.py
--rw-rw-rw-   0        0        0      814 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Telephony.py
--rw-rw-rw-   0        0        0     4732 2023-05-31 16:21:50.000000 termux-api-1.2.4/termux/UI.py
--rw-rw-rw-   0        0        0      455 2023-05-31 16:21:50.000000 termux-api-1.2.4/termux/Wake.py
--rw-rw-rw-   0        0        0      638 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Wifi.py
--rw-rw-rw-   0        0        0      871 2023-05-31 16:21:50.000000 termux-api-1.2.4/termux/__init__.py
--rw-rw-rw-   0        0        0     1195 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/android.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:26:08.642661 termux-api-1.2.4/termux_api.egg-info/
--rw-rw-rw-   0        0        0     3621 2023-05-31 16:26:08.000000 termux-api-1.2.4/termux_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-05-31 16:26:08.000000 termux-api-1.2.4/termux_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 16:26:08.000000 termux-api-1.2.4/termux_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 16:26:08.000000 termux-api-1.2.4/termux_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 17:51:01.656473 termux-api-1.2.5/
+-rw-rw-rw-   0        0        0     1086 2022-06-29 16:50:48.000000 termux-api-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     3621 2023-06-05 17:51:01.655589 termux-api-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3060 2022-06-30 07:05:02.000000 termux-api-1.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 17:51:01.656473 termux-api-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-06-05 17:43:49.000000 termux-api-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:51:01.643820 termux-api-1.2.5/termux/
+-rw-rw-rw-   0        0        0     3513 2023-05-31 16:21:50.000000 termux-api-1.2.5/termux/API.py
+-rw-rw-rw-   0        0        0      661 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Camera.py
+-rw-rw-rw-   0        0        0      520 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Clipboard.py
+-rw-rw-rw-   0        0        0     1269 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Media.py
+-rw-rw-rw-   0        0        0     1293 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Microphone.py
+-rw-rw-rw-   0        0        0     1237 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Notification.py
+-rw-rw-rw-   0        0        0     1245 2023-06-05 17:35:36.000000 termux-api-1.2.5/termux/SMS.py
+-rw-rw-rw-   0        0        0     2284 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Scheduler.py
+-rw-rw-rw-   0        0        0     2241 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Sensors.py
+-rw-rw-rw-   0        0        0     1105 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Share.py
+-rw-rw-rw-   0        0        0     1112 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/TTS.py
+-rw-rw-rw-   0        0        0      814 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Telephony.py
+-rw-rw-rw-   0        0        0     4732 2023-05-31 16:21:50.000000 termux-api-1.2.5/termux/UI.py
+-rw-rw-rw-   0        0        0      455 2023-05-31 16:21:50.000000 termux-api-1.2.5/termux/Wake.py
+-rw-rw-rw-   0        0        0      638 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/Wifi.py
+-rw-rw-rw-   0        0        0      897 2023-06-05 16:34:04.000000 termux-api-1.2.5/termux/__init__.py
+-rw-rw-rw-   0        0        0     1195 2022-06-30 07:05:02.000000 termux-api-1.2.5/termux/android.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:51:01.653646 termux-api-1.2.5/termux_api.egg-info/
+-rw-rw-rw-   0        0        0     3621 2023-06-05 17:51:01.000000 termux-api-1.2.5/termux_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-06-05 17:51:01.000000 termux-api-1.2.5/termux_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:51:01.000000 termux-api-1.2.5/termux_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 17:51:01.000000 termux-api-1.2.5/termux_api.egg-info/top_level.txt
```

### Comparing `termux-api-1.2.4/LICENSE` & `termux-api-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/PKG-INFO` & `termux-api-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-api
-Version: 1.2.4
+Version: 1.2.5
 Summary: A package for accessing termux-api
 Home-page: https://github.com/shajul/termux-api.git
 Author: drshajul
 Author-email: drshajul@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: termux-api Version: 1.2.4 Summary: A package for
+Metadata-Version: 2.1 Name: termux-api Version: 1.2.5 Summary: A package for
 accessing termux-api Home-page: https://github.com/shajul/termux-api.git
 Author: drshajul Author-email: drshajul@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # termux-api [!
 [Build Status](http://img.shields.io/travis/badges/
 badgerbadgerbadger.svg?style=flat-square)](https://github.com/shajul/termux-
```

### Comparing `termux-api-1.2.4/README.md` & `termux-api-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/setup.py` & `termux-api-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="termux-api", 
-    version="1.2.4",
+    version="1.2.5",
     author="drshajul",
     author_email="drshajul@gmail.com",
     description="A package for accessing termux-api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shajul/termux-api.git",
     packages=setuptools.find_packages(),
```

### Comparing `termux-api-1.2.4/termux/API.py` & `termux-api-1.2.5/termux/API.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Camera.py` & `termux-api-1.2.5/termux/Camera.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Clipboard.py` & `termux-api-1.2.5/termux/Clipboard.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Media.py` & `termux-api-1.2.5/termux/Media.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Microphone.py` & `termux-api-1.2.5/termux/Microphone.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Notification.py` & `termux-api-1.2.5/termux/Notification.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Scheduler.py` & `termux-api-1.2.5/termux/Scheduler.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Sensors.py` & `termux-api-1.2.5/termux/Sensors.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Share.py` & `termux-api-1.2.5/termux/Share.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/TTS.py` & `termux-api-1.2.5/termux/TTS.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Telephony.py` & `termux-api-1.2.5/termux/Telephony.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/UI.py` & `termux-api-1.2.5/termux/UI.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/Wifi.py` & `termux-api-1.2.5/termux/Wifi.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux/__init__.py` & `termux-api-1.2.5/termux/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,22 +7,23 @@
   termux.Clipboard
   termux.Media - Playback and media scanner
   termux.Microphone
   termux.Notification
   termux.Scheduler - Job Scheduler
   termux.Sensors
   termux.Share
+  termux.SMS
   termux.Telephony - make call, info of device and network
   termux.TTS - Text to speech
   termux.UI - Dialog Widgets and Toast
   termux.Wifi
   termux.Wake
 
 For information about available methods, use
   help(termux.<modulename>)
 '''
 
-from . import API, Camera, Clipboard, Sensors, TTS, Wifi, Notification, Media, Microphone, Scheduler, Share, Telephony, UI, Wake
+from . import API, Camera, Clipboard, Sensors, TTS, Wifi, Notification, Media, Microphone, Scheduler, Share, Telephony, UI, Wake, SMS
 
 
 __all__ = sorted(["API", "Sensors", "Camera", "Clipboard", "TTS", "Wifi", "Notification",
-                  "Media", "Microphone", "Scheduler", "Share", "Telephony", "UI", "Wake"])
+                  "Media", "Microphone", "Scheduler", "Share", "Telephony", "UI", "Wake", "SMS"])
```

### Comparing `termux-api-1.2.4/termux/android.py` & `termux-api-1.2.5/termux/android.py`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.4/termux_api.egg-info/PKG-INFO` & `termux-api-1.2.5/termux_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-api
-Version: 1.2.4
+Version: 1.2.5
 Summary: A package for accessing termux-api
 Home-page: https://github.com/shajul/termux-api.git
 Author: drshajul
 Author-email: drshajul@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: termux-api Version: 1.2.4 Summary: A package for
+Metadata-Version: 2.1 Name: termux-api Version: 1.2.5 Summary: A package for
 accessing termux-api Home-page: https://github.com/shajul/termux-api.git
 Author: drshajul Author-email: drshajul@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # termux-api [!
 [Build Status](http://img.shields.io/travis/badges/
 badgerbadgerbadger.svg?style=flat-square)](https://github.com/shajul/termux-
```

