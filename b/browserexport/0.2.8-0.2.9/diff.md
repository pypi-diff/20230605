# Comparing `tmp/browserexport-0.2.8.tar.gz` & `tmp/browserexport-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserexport-0.2.8.tar", last modified: Sat Nov 12 20:05:16 2022, max compression
+gzip compressed data, was "browserexport-0.2.9.tar", last modified: Wed Dec 21 04:32:40 2022, max compression
```

## Comparing `browserexport-0.2.8.tar` & `browserexport-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2022-11-12 20:05:16.848971 browserexport-0.2.8/
--rw-r--r--   0 sean      (1000) sean      (1000)     1074 2020-08-29 02:15:53.000000 browserexport-0.2.8/LICENSE
--rw-r--r--   0 sean      (1000) sean      (1000)    13033 2022-11-12 20:05:16.848971 browserexport-0.2.8/PKG-INFO
--rw-r--r--   0 sean      (1000) sean      (1000)    12273 2022-11-12 20:03:33.000000 browserexport-0.2.8/README.md
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2022-11-12 20:05:16.848971 browserexport-0.2.8/browserexport/
--rw-r--r--   0 sean      (1000) sean      (1000)     4873 2022-05-02 20:57:32.000000 browserexport-0.2.8/browserexport/__main__.py
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2022-11-12 20:05:16.848971 browserexport-0.2.8/browserexport/browsers/
--rw-r--r--   0 sean      (1000) sean      (1000)     1314 2022-11-12 20:00:07.000000 browserexport-0.2.8/browserexport/browsers/all.py
--rw-r--r--   0 sean      (1000) sean      (1000)      486 2022-11-12 20:01:01.000000 browserexport-0.2.8/browserexport/browsers/arc.py
--rw-r--r--   0 sean      (1000) sean      (1000)      409 2022-05-02 20:02:05.000000 browserexport-0.2.8/browserexport/browsers/brave.py
--rw-r--r--   0 sean      (1000) sean      (1000)     1699 2022-05-02 20:02:05.000000 browserexport-0.2.8/browserexport/browsers/chrome.py
--rw-r--r--   0 sean      (1000) sean      (1000)      425 2022-05-02 20:02:05.000000 browserexport-0.2.8/browserexport/browsers/chromium.py
--rw-r--r--   0 sean      (1000) sean      (1000)     6469 2022-05-02 20:57:32.000000 browserexport-0.2.8/browserexport/browsers/common.py
--rw-r--r--   0 sean      (1000) sean      (1000)     2370 2022-05-02 20:57:32.000000 browserexport-0.2.8/browserexport/browsers/firefox.py
--rw-r--r--   0 sean      (1000) sean      (1000)     1127 2022-05-02 20:02:05.000000 browserexport-0.2.8/browserexport/browsers/firefox_mobile.py
--rw-r--r--   0 sean      (1000) sean      (1000)     1351 2022-05-02 20:02:05.000000 browserexport-0.2.8/browserexport/browsers/firefox_mobile_legacy.py
--rw-r--r--   0 sean      (1000) sean      (1000)     2623 2022-05-02 20:02:05.000000 browserexport-0.2.8/browserexport/browsers/palemoon.py
--rw-r--r--   0 sean      (1000) sean      (1000)     1672 2022-05-02 20:02:05.000000 browserexport-0.2.8/browserexport/browsers/safari.py
--rw-r--r--   0 sean      (1000) sean      (1000)      384 2022-05-02 20:02:05.000000 browserexport-0.2.8/browserexport/browsers/vivaldi.py
--rw-r--r--   0 sean      (1000) sean      (1000)      478 2022-05-02 20:02:05.000000 browserexport-0.2.8/browserexport/browsers/waterfox.py
--rw-r--r--   0 sean      (1000) sean      (1000)      587 2022-02-19 00:27:46.000000 browserexport-0.2.8/browserexport/common.py
--rw-r--r--   0 sean      (1000) sean      (1000)      319 2022-01-03 21:16:35.000000 browserexport-0.2.8/browserexport/demo.py
--rw-r--r--   0 sean      (1000) sean      (1000)      867 2022-02-02 16:07:21.000000 browserexport-0.2.8/browserexport/log.py
--rw-r--r--   0 sean      (1000) sean      (1000)     1743 2022-03-09 06:11:22.000000 browserexport-0.2.8/browserexport/merge.py
--rw-r--r--   0 sean      (1000) sean      (1000)     1800 2022-03-09 06:11:23.000000 browserexport-0.2.8/browserexport/model.py
--rw-r--r--   0 sean      (1000) sean      (1000)     1815 2022-08-30 09:29:14.000000 browserexport-0.2.8/browserexport/parse.py
--rw-r--r--   0 sean      (1000) sean      (1000)        0 2022-01-03 21:16:35.000000 browserexport-0.2.8/browserexport/py.typed
--rw-r--r--   0 sean      (1000) sean      (1000)     3267 2022-05-02 20:53:02.000000 browserexport-0.2.8/browserexport/save.py
--rw-r--r--   0 sean      (1000) sean      (1000)      962 2022-02-19 00:25:54.000000 browserexport-0.2.8/browserexport/sqlite.py
-drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2022-11-12 20:05:16.848971 browserexport-0.2.8/browserexport.egg-info/
--rw-r--r--   0 sean      (1000) sean      (1000)    13033 2022-11-12 20:05:16.000000 browserexport-0.2.8/browserexport.egg-info/PKG-INFO
--rw-r--r--   0 sean      (1000) sean      (1000)      944 2022-11-12 20:05:16.000000 browserexport-0.2.8/browserexport.egg-info/SOURCES.txt
--rw-r--r--   0 sean      (1000) sean      (1000)        1 2022-11-12 20:05:16.000000 browserexport-0.2.8/browserexport.egg-info/dependency_links.txt
--rw-r--r--   0 sean      (1000) sean      (1000)       61 2022-11-12 20:05:16.000000 browserexport-0.2.8/browserexport.egg-info/entry_points.txt
--rw-r--r--   0 sean      (1000) sean      (1000)       78 2022-11-12 20:05:16.000000 browserexport-0.2.8/browserexport.egg-info/requires.txt
--rw-r--r--   0 sean      (1000) sean      (1000)       14 2022-11-12 20:05:16.000000 browserexport-0.2.8/browserexport.egg-info/top_level.txt
--rw-r--r--   0 sean      (1000) sean      (1000)      564 2022-11-12 20:05:16.848971 browserexport-0.2.8/setup.cfg
--rw-r--r--   0 sean      (1000) sean      (1000)     1404 2022-11-12 20:04:16.000000 browserexport-0.2.8/setup.py
+drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2022-12-21 04:32:40.300040 browserexport-0.2.9/
+-rw-r--r--   0 sean      (1000) sean      (1000)     1074 2020-08-29 02:15:53.000000 browserexport-0.2.9/LICENSE
+-rw-r--r--   0 sean      (1000) sean      (1000)    13033 2022-12-21 04:32:40.300040 browserexport-0.2.9/PKG-INFO
+-rw-r--r--   0 sean      (1000) sean      (1000)    12273 2022-11-12 20:03:33.000000 browserexport-0.2.9/README.md
+drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2022-12-21 04:32:40.300040 browserexport-0.2.9/browserexport/
+-rw-r--r--   0 sean      (1000) sean      (1000)     4873 2022-05-02 20:57:32.000000 browserexport-0.2.9/browserexport/__main__.py
+drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2022-12-21 04:32:40.300040 browserexport-0.2.9/browserexport/browsers/
+-rw-r--r--   0 sean      (1000) sean      (1000)     1314 2022-11-12 20:00:07.000000 browserexport-0.2.9/browserexport/browsers/all.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      486 2022-11-12 20:01:01.000000 browserexport-0.2.9/browserexport/browsers/arc.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      409 2022-05-02 20:02:05.000000 browserexport-0.2.9/browserexport/browsers/brave.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     1699 2022-05-02 20:02:05.000000 browserexport-0.2.9/browserexport/browsers/chrome.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      425 2022-05-02 20:02:05.000000 browserexport-0.2.9/browserexport/browsers/chromium.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     6469 2022-05-02 20:57:32.000000 browserexport-0.2.9/browserexport/browsers/common.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     2370 2022-05-02 20:57:32.000000 browserexport-0.2.9/browserexport/browsers/firefox.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     1127 2022-05-02 20:02:05.000000 browserexport-0.2.9/browserexport/browsers/firefox_mobile.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     1351 2022-05-02 20:02:05.000000 browserexport-0.2.9/browserexport/browsers/firefox_mobile_legacy.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     2623 2022-05-02 20:02:05.000000 browserexport-0.2.9/browserexport/browsers/palemoon.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     1672 2022-05-02 20:02:05.000000 browserexport-0.2.9/browserexport/browsers/safari.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      384 2022-05-02 20:02:05.000000 browserexport-0.2.9/browserexport/browsers/vivaldi.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      478 2022-05-02 20:02:05.000000 browserexport-0.2.9/browserexport/browsers/waterfox.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      587 2022-02-19 00:27:46.000000 browserexport-0.2.9/browserexport/common.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      319 2022-01-03 21:16:35.000000 browserexport-0.2.9/browserexport/demo.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      867 2022-02-02 16:07:21.000000 browserexport-0.2.9/browserexport/log.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     1743 2022-03-09 06:11:22.000000 browserexport-0.2.9/browserexport/merge.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     1800 2022-03-09 06:11:23.000000 browserexport-0.2.9/browserexport/model.py
+-rw-r--r--   0 sean      (1000) sean      (1000)     1815 2022-08-30 09:29:14.000000 browserexport-0.2.9/browserexport/parse.py
+-rw-r--r--   0 sean      (1000) sean      (1000)        0 2022-01-03 21:16:35.000000 browserexport-0.2.9/browserexport/py.typed
+-rw-r--r--   0 sean      (1000) sean      (1000)     3267 2022-05-02 20:53:02.000000 browserexport-0.2.9/browserexport/save.py
+-rw-r--r--   0 sean      (1000) sean      (1000)      962 2022-02-19 00:25:54.000000 browserexport-0.2.9/browserexport/sqlite.py
+drwxr-xr-x   0 sean      (1000) sean      (1000)        0 2022-12-21 04:32:40.300040 browserexport-0.2.9/browserexport.egg-info/
+-rw-r--r--   0 sean      (1000) sean      (1000)    13033 2022-12-21 04:32:40.000000 browserexport-0.2.9/browserexport.egg-info/PKG-INFO
+-rw-r--r--   0 sean      (1000) sean      (1000)      944 2022-12-21 04:32:40.000000 browserexport-0.2.9/browserexport.egg-info/SOURCES.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)        1 2022-12-21 04:32:40.000000 browserexport-0.2.9/browserexport.egg-info/dependency_links.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)       61 2022-12-21 04:32:40.000000 browserexport-0.2.9/browserexport.egg-info/entry_points.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)       78 2022-12-21 04:32:40.000000 browserexport-0.2.9/browserexport.egg-info/requires.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)       14 2022-12-21 04:32:40.000000 browserexport-0.2.9/browserexport.egg-info/top_level.txt
+-rw-r--r--   0 sean      (1000) sean      (1000)      564 2022-12-21 04:32:40.300040 browserexport-0.2.9/setup.cfg
+-rw-r--r--   0 sean      (1000) sean      (1000)     1404 2022-12-21 04:30:56.000000 browserexport-0.2.9/setup.py
```

### Comparing `browserexport-0.2.8/LICENSE` & `browserexport-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/PKG-INFO` & `browserexport-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserexport
-Version: 0.2.8
+Version: 0.2.9
 Summary: save and merge browser history and metadata from different browsers
 Home-page: https://github.com/seanbreckenridge/browserexport
 Author: Sean Breckenridge
 Author-email: seanbrecke@gmail.com
 License: MIT
 Keywords: firefox history backup data
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: browserexport Version: 0.2.8 Summary: save and
+Metadata-Version: 2.1 Name: browserexport Version: 0.2.9 Summary: save and
 merge browser history and metadata from different browsers Home-page: https://
 github.com/seanbreckenridge/browserexport Author: Sean Breckenridge Author-
 email: seanbrecke@gmail.com License: MIT Keywords: firefox history backup data
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `browserexport-0.2.8/README.md` & `browserexport-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/__main__.py` & `browserexport-0.2.9/browserexport/__main__.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/browsers/all.py` & `browserexport-0.2.9/browserexport/browsers/all.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/browsers/chrome.py` & `browserexport-0.2.9/browserexport/browsers/chrome.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/browsers/common.py` & `browserexport-0.2.9/browserexport/browsers/common.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/browsers/firefox.py` & `browserexport-0.2.9/browserexport/browsers/firefox.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/browsers/firefox_mobile.py` & `browserexport-0.2.9/browserexport/browsers/firefox_mobile.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/browsers/firefox_mobile_legacy.py` & `browserexport-0.2.9/browserexport/browsers/firefox_mobile_legacy.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/browsers/palemoon.py` & `browserexport-0.2.9/browserexport/browsers/palemoon.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/browsers/safari.py` & `browserexport-0.2.9/browserexport/browsers/safari.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/common.py` & `browserexport-0.2.9/browserexport/common.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/log.py` & `browserexport-0.2.9/browserexport/log.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/merge.py` & `browserexport-0.2.9/browserexport/merge.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/model.py` & `browserexport-0.2.9/browserexport/model.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/parse.py` & `browserexport-0.2.9/browserexport/parse.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/save.py` & `browserexport-0.2.9/browserexport/save.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport/sqlite.py` & `browserexport-0.2.9/browserexport/sqlite.py`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/browserexport.egg-info/PKG-INFO` & `browserexport-0.2.9/browserexport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserexport
-Version: 0.2.8
+Version: 0.2.9
 Summary: save and merge browser history and metadata from different browsers
 Home-page: https://github.com/seanbreckenridge/browserexport
 Author: Sean Breckenridge
 Author-email: seanbrecke@gmail.com
 License: MIT
 Keywords: firefox history backup data
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: browserexport Version: 0.2.8 Summary: save and
+Metadata-Version: 2.1 Name: browserexport Version: 0.2.9 Summary: save and
 merge browser history and metadata from different browsers Home-page: https://
 github.com/seanbreckenridge/browserexport Author: Sean Breckenridge Author-
 email: seanbrecke@gmail.com License: MIT Keywords: firefox history backup data
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `browserexport-0.2.8/browserexport.egg-info/SOURCES.txt` & `browserexport-0.2.9/browserexport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/setup.cfg` & `browserexport-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `browserexport-0.2.8/setup.py` & `browserexport-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 long_description = Path("README.md").read_text()
 reqs = Path("requirements.txt").read_text().strip().splitlines()
 
 pkg = "browserexport"
 setup(
     name=pkg,
-    version="0.2.8",
+    version="0.2.9",
     url="https://github.com/seanbreckenridge/browserexport",
     author="Sean Breckenridge",
     author_email="seanbrecke@gmail.com",
     description=(
         """save and merge browser history and metadata from different browsers"""
     ),
     long_description=long_description,
```

