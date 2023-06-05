# Comparing `tmp/lecore-0.1.1.tar.gz` & `tmp/lecore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\work\gitlab\le-py-core\package-lecore\dist\.tmp-dtqaohth\lecore-0.1.1.tar", last modified: Mon Jun  5 14:43:16 2023, max compression
+gzip compressed data, was "D:\work\gitlab\le-py-core\package-lecore\dist\.tmp-wyf9qem3\lecore-0.1.2.tar", last modified: Mon Jun  5 14:47:10 2023, max compression
```

## Comparing `lecore-0.1.1.tar` & `lecore-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 14:43:16.000000 lecore-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-03-24 15:23:12.000000 lecore-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1558 2023-06-05 14:43:16.000000 lecore-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-03-27 13:17:27.000000 lecore-0.1.1/README.md
--rw-rw-rw-   0        0        0      685 2023-06-05 14:40:21.000000 lecore-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 14:43:16.000000 lecore-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-05 14:43:16.000000 lecore-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 14:43:16.000000 lecore-0.1.1/src/lecore/
-drwxrwxrwx   0        0        0        0 2023-06-05 14:43:16.000000 lecore-0.1.1/src/lecore/LeBin/
--rw-rw-rw-   0        0        0    12112 2023-01-16 14:47:23.000000 lecore-0.1.1/src/lecore/LeBin/RegisterMap.py
--rw-rw-rw-   0        0        0     4563 2021-08-12 11:01:11.000000 lecore-0.1.1/src/lecore/LeBin/SerialCom.py
--rw-rw-rw-   0        0        0     2933 2020-11-27 14:22:56.000000 lecore-0.1.1/src/lecore/LeBin/UpgradeFirmware.py
--rw-rw-rw-   0        0        0     5339 2021-06-08 08:56:52.000000 lecore-0.1.1/src/lecore/LeBin/VisualLeBin.py
--rw-rw-rw-   0        0        0        0 2023-06-05 14:27:54.000000 lecore-0.1.1/src/lecore/LeBin/__init__.py
--rw-rw-rw-   0        0        0     4973 2023-06-05 14:39:42.000000 lecore-0.1.1/src/lecore/Looger.py
--rw-rw-rw-   0        0        0       32 2023-03-27 11:54:46.000000 lecore-0.1.1/src/lecore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:43:16.000000 lecore-0.1.1/src/lecore.egg-info/
--rw-rw-rw-   0        0        0     1558 2023-06-05 14:43:16.000000 lecore-0.1.1/src/lecore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-06-05 14:43:16.000000 lecore-0.1.1/src/lecore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 14:43:16.000000 lecore-0.1.1/src/lecore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 14:43:16.000000 lecore-0.1.1/src/lecore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 14:43:16.000000 lecore-0.1.1/src/lecore.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 14:43:16.000000 lecore-0.1.1/tests/
--rw-rw-rw-   0        0        0     1456 2023-03-27 13:17:27.000000 lecore-0.1.1/tests/test_looger.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:47:10.000000 lecore-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-03-24 15:23:12.000000 lecore-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1558 2023-06-05 14:47:10.000000 lecore-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-03-27 13:17:27.000000 lecore-0.1.2/README.md
+-rw-rw-rw-   0        0        0      685 2023-06-05 14:46:56.000000 lecore-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 14:47:10.000000 lecore-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 14:47:10.000000 lecore-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 14:47:10.000000 lecore-0.1.2/src/lecore/
+drwxrwxrwx   0        0        0        0 2023-06-05 14:47:10.000000 lecore-0.1.2/src/lecore/LeBin/
+-rw-rw-rw-   0        0        0    12112 2023-01-16 14:47:23.000000 lecore-0.1.2/src/lecore/LeBin/RegisterMap.py
+-rw-rw-rw-   0        0        0     4563 2021-08-12 11:01:11.000000 lecore-0.1.2/src/lecore/LeBin/SerialCom.py
+-rw-rw-rw-   0        0        0     2933 2020-11-27 14:22:56.000000 lecore-0.1.2/src/lecore/LeBin/UpgradeFirmware.py
+-rw-rw-rw-   0        0        0     5339 2021-06-08 08:56:52.000000 lecore-0.1.2/src/lecore/LeBin/VisualLeBin.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:27:54.000000 lecore-0.1.2/src/lecore/LeBin/__init__.py
+-rw-rw-rw-   0        0        0     4973 2023-06-05 14:39:42.000000 lecore-0.1.2/src/lecore/Looger.py
+-rw-rw-rw-   0        0        0       28 2023-06-05 14:45:48.000000 lecore-0.1.2/src/lecore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:47:10.000000 lecore-0.1.2/src/lecore.egg-info/
+-rw-rw-rw-   0        0        0     1558 2023-06-05 14:47:10.000000 lecore-0.1.2/src/lecore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-06-05 14:47:10.000000 lecore-0.1.2/src/lecore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 14:47:10.000000 lecore-0.1.2/src/lecore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 14:47:10.000000 lecore-0.1.2/src/lecore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 14:47:10.000000 lecore-0.1.2/src/lecore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 14:47:10.000000 lecore-0.1.2/tests/
+-rw-rw-rw-   0        0        0     1456 2023-03-27 13:17:27.000000 lecore-0.1.2/tests/test_looger.py
```

### Comparing `lecore-0.1.1/LICENSE` & `lecore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lecore-0.1.1/PKG-INFO` & `lecore-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Logic Elements core utilities
 Author-email: Jan Bartovský <jan.bartovsky@logicelements.cz>
 Project-URL: Homepage, http://www.logicelements.cz
 Keywords: logicelements,looger,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecore-0.1.1/README.md` & `lecore-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lecore-0.1.1/pyproject.toml` & `lecore-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lecore"
 description = "Logic Elements core utilities"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Jan Bartovský", email="jan.bartovsky@logicelements.cz" },
 ]
 readme = "README.md"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `lecore-0.1.1/src/lecore/LeBin/RegisterMap.py` & `lecore-0.1.2/src/lecore/LeBin/RegisterMap.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.1/src/lecore/LeBin/SerialCom.py` & `lecore-0.1.2/src/lecore/LeBin/SerialCom.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.1/src/lecore/LeBin/UpgradeFirmware.py` & `lecore-0.1.2/src/lecore/LeBin/UpgradeFirmware.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.1/src/lecore/LeBin/VisualLeBin.py` & `lecore-0.1.2/src/lecore/LeBin/VisualLeBin.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.1/src/lecore/Looger.py` & `lecore-0.1.2/src/lecore/Looger.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.1/src/lecore.egg-info/PKG-INFO` & `lecore-0.1.2/src/lecore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Logic Elements core utilities
 Author-email: Jan Bartovský <jan.bartovsky@logicelements.cz>
 Project-URL: Homepage, http://www.logicelements.cz
 Keywords: logicelements,looger,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecore-0.1.1/tests/test_looger.py` & `lecore-0.1.2/tests/test_looger.py`

 * *Files identical despite different names*

