# Comparing `tmp/augratin-23.5.26.tar.gz` & `tmp/augratin-23.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augratin-23.5.26.tar", last modified: Fri May 26 15:52:55 2023, max compression
+gzip compressed data, was "augratin-23.6.4.tar", last modified: Mon Jun  5 04:01:29 2023, max compression
```

## Comparing `augratin-23.5.26.tar` & `augratin-23.6.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.631701 augratin-23.5.26/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.26/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5141 2023-05-26 15:52:55.629701 augratin-23.5.26/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4366 2023-05-26 15:51:22.000000 augratin-23.5.26/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.575701 augratin-23.5.26/augratin/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42152 2023-05-26 15:49:25.000000 augratin-23.5.26/augratin/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.613701 augratin-23.5.26/augratin/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27092 2023-05-17 23:53:10.000000 augratin-23.5.26/augratin/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/k6gte-augratin-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/k6gte-augratin-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/k6gte-augratin-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/k6gte-augratin.desktop
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.623701 augratin-23.5.26/augratin/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13852 2023-05-18 16:38:33.000000 augratin-23.5.26/augratin/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.26/augratin/lib/omnirig_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-26 15:49:50.000000 augratin-23.5.26/augratin/lib/version.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.591701 augratin-23.5.26/augratin.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5141 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1142 2023-05-26 15:50:00.000000 augratin-23.5.26/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-26 15:52:55.631701 augratin-23.5.26/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:01:29.728191 augratin-23.6.4/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.6.4/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5519 2023-06-05 04:01:29.725191 augratin-23.6.4/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4745 2023-06-05 03:42:32.000000 augratin-23.6.4/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:01:29.671190 augratin-23.6.4/augratin/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.6.4/augratin/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42515 2023-06-05 03:42:32.000000 augratin-23.6.4/augratin/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:01:29.706191 augratin-23.6.4/augratin/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.6.4/augratin/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27092 2023-05-17 23:53:10.000000 augratin-23.6.4/augratin/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.6.4/augratin/data/k6gte-augratin-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.6.4/augratin/data/k6gte-augratin-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.6.4/augratin/data/k6gte-augratin-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.6.4/augratin/data/k6gte-augratin.desktop
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:01:29.724191 augratin-23.6.4/augratin/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.6.4/augratin/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13852 2023-05-18 16:38:33.000000 augratin-23.6.4/augratin/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3303 2023-06-05 03:42:32.000000 augratin-23.6.4/augratin/lib/omnirig_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-05 03:47:00.000000 augratin-23.6.4/augratin/lib/version.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:01:29.688190 augratin-23.6.4/augratin.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5519 2023-06-05 04:01:29.000000 augratin-23.6.4/augratin.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-06-05 04:01:29.000000 augratin-23.6.4/augratin.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-05 04:01:29.000000 augratin-23.6.4/augratin.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-06-05 04:01:29.000000 augratin-23.6.4/augratin.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-06-05 04:01:29.000000 augratin-23.6.4/augratin.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-06-05 04:01:29.000000 augratin-23.6.4/augratin.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1141 2023-06-05 03:46:47.000000 augratin-23.6.4/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-05 04:01:29.728191 augratin-23.6.4/setup.cfg
```

### Comparing `augratin-23.5.26/LICENSE` & `augratin-23.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `augratin-23.5.26/PKG-INFO` & `augratin-23.6.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.26
+Version: 23.6.4
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,14 +27,15 @@
 - [AuGratin](#augratin)
   - [Why AuGratin](#why-augratin)
   - [What is AuGratin](#what-is-augratin)
   - [Recent changes](#recent-changes)
   - [Installing, Updating, Running, Removing](#installing-updating-running-removing)
   - [Features](#features)
   - [What to do if your map is blank](#what-to-do-if-your-map-is-blank)
+  - [What to do if omnirig fails to connect](#what-to-do-if-omnirig-fails-to-connect)
   - [CAT control](#cat-control)
 
 ## Why AuGratin
 
 AuGratin is an extension to an earlier program called POTAto. And since it's made from POTAto, I called it AuGratin.
 
 ## What is AuGratin
@@ -106,14 +107,18 @@
 #fedora
 sudo dnf install python3-qt5 python3-qt5-webengine
 
 #ubuntu
 sudo apt install python3-pyqt5 python3-pyqt5.qtwebengine
 ```
 
+## What to do if omnirig fails to connect
+
+On occasion the win32 cache files can get corrupted preventing connection to omnirig. If omnirig was previously working but the continues to fail try erasing the cache files located here: C:\Users\username*\AppData\Local\Temp\gen_py\python version*
+
 ## CAT control
 
 If no command line options are given, the program will check if either flrig, rigctld or OmniRig are running on the computer. It will setup CAT control to whichever it finds first.
 
 You can force it to use either with commandline options.
 
 `-r` will force rigctld with default host:port of localhost:4532.
```

### Comparing `augratin-23.5.26/README.md` & `augratin-23.6.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 - [AuGratin](#augratin)
   - [Why AuGratin](#why-augratin)
   - [What is AuGratin](#what-is-augratin)
   - [Recent changes](#recent-changes)
   - [Installing, Updating, Running, Removing](#installing-updating-running-removing)
   - [Features](#features)
   - [What to do if your map is blank](#what-to-do-if-your-map-is-blank)
+  - [What to do if omnirig fails to connect](#what-to-do-if-omnirig-fails-to-connect)
   - [CAT control](#cat-control)
 
 ## Why AuGratin
 
 AuGratin is an extension to an earlier program called POTAto. And since it's made from POTAto, I called it AuGratin.
 
 ## What is AuGratin
@@ -87,14 +88,18 @@
 #fedora
 sudo dnf install python3-qt5 python3-qt5-webengine
 
 #ubuntu
 sudo apt install python3-pyqt5 python3-pyqt5.qtwebengine
 ```
 
+## What to do if omnirig fails to connect
+
+On occasion the win32 cache files can get corrupted preventing connection to omnirig. If omnirig was previously working but the continues to fail try erasing the cache files located here: C:\Users\username*\AppData\Local\Temp\gen_py\python version*
+
 ## CAT control
 
 If no command line options are given, the program will check if either flrig, rigctld or OmniRig are running on the computer. It will setup CAT control to whichever it finds first.
 
 You can force it to use either with commandline options.
 
 `-r` will force rigctld with default host:port of localhost:4532.
```

### Comparing `augratin-23.5.26/augratin/__main__.py` & `augratin-23.6.4/augratin/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -842,16 +842,25 @@
         """bandwidth"""
         logger.debug("%s", f"mark:{currentPolygon} f:{freq} b:{self.bandwidth}")
         self.clear_freq_mark(currentPolygon)
         if freq < self.currentBand.start or freq > self.currentBand.end:
             return
         if freq and self.bandwidth:
             # color = QtGui.QColor(30, 30, 180)
-            bw_start = freq - ((self.bandwidth / 2) / 1000000)
-            bw_end = freq + ((self.bandwidth / 2) / 1000000)
+            mode = self.comboBox_mode.currentText()
+            if mode == "SSB":
+                if freq > 10:
+                    bw_start = freq
+                    bw_end = freq + ((self.bandwidth) / 1000000)
+                else:
+                    bw_start = freq 
+                    bw_end = freq - ((self.bandwidth) / 1000000)
+            else:
+                bw_start = freq - ((self.bandwidth / 2) / 1000000)
+                bw_end = freq + ((self.bandwidth / 2) / 1000000)
             logger.debug("%s", f"s:{bw_start} e:{bw_end}")
             Yposition_neg = self.Freq2ScenePos(bw_start).y()
             Yposition_pos = self.Freq2ScenePos(bw_end).y()
             poly = QtGui.QPolygonF()
             poly.append(QtCore.QPointF(175, Yposition_neg))
             poly.append(QtCore.QPointF(180, Yposition_neg))
             poly.append(QtCore.QPointF(180, Yposition_pos))
```

### Comparing `augratin-23.5.26/augratin/data/JetBrainsMono-Regular.ttf` & `augratin-23.6.4/augratin/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `augratin-23.5.26/augratin/data/dialog.ui` & `augratin-23.6.4/augratin/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `augratin-23.5.26/augratin/data/k6gte-augratin-128.png` & `augratin-23.6.4/augratin/data/k6gte-augratin-128.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.26/augratin/data/k6gte-augratin-32.png` & `augratin-23.6.4/augratin/data/k6gte-augratin-32.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.26/augratin/data/k6gte-augratin-64.png` & `augratin-23.6.4/augratin/data/k6gte-augratin-64.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.26/augratin/lib/cat_interface.py` & `augratin-23.6.4/augratin/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.26/augratin.egg-info/PKG-INFO` & `augratin-23.6.4/augratin.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.26
+Version: 23.6.4
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,14 +27,15 @@
 - [AuGratin](#augratin)
   - [Why AuGratin](#why-augratin)
   - [What is AuGratin](#what-is-augratin)
   - [Recent changes](#recent-changes)
   - [Installing, Updating, Running, Removing](#installing-updating-running-removing)
   - [Features](#features)
   - [What to do if your map is blank](#what-to-do-if-your-map-is-blank)
+  - [What to do if omnirig fails to connect](#what-to-do-if-omnirig-fails-to-connect)
   - [CAT control](#cat-control)
 
 ## Why AuGratin
 
 AuGratin is an extension to an earlier program called POTAto. And since it's made from POTAto, I called it AuGratin.
 
 ## What is AuGratin
@@ -106,14 +107,18 @@
 #fedora
 sudo dnf install python3-qt5 python3-qt5-webengine
 
 #ubuntu
 sudo apt install python3-pyqt5 python3-pyqt5.qtwebengine
 ```
 
+## What to do if omnirig fails to connect
+
+On occasion the win32 cache files can get corrupted preventing connection to omnirig. If omnirig was previously working but the continues to fail try erasing the cache files located here: C:\Users\username*\AppData\Local\Temp\gen_py\python version*
+
 ## CAT control
 
 If no command line options are given, the program will check if either flrig, rigctld or OmniRig are running on the computer. It will setup CAT control to whichever it finds first.
 
 You can force it to use either with commandline options.
 
 `-r` will force rigctld with default host:port of localhost:4532.
```

### Comparing `augratin-23.5.26/augratin.egg-info/SOURCES.txt` & `augratin-23.6.4/augratin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augratin-23.5.26/pyproject.toml` & `augratin-23.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "augratin" 
-version = "23.5.26"
+version = "23.6.4"
 description = "An aid for POTA hunters"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
```

