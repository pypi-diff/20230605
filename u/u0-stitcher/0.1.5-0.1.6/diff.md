# Comparing `tmp/u0_stitcher-0.1.5.tar.gz` & `tmp/u0_stitcher-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "u0_stitcher-0.1.5.tar", last modified: Mon May 29 09:34:58 2023, max compression
+gzip compressed data, was "u0_stitcher-0.1.6.tar", last modified: Mon Jun  5 02:06:54 2023, max compression
```

## Comparing `u0_stitcher-0.1.5.tar` & `u0_stitcher-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-29 09:34:58.805980 u0_stitcher-0.1.5/
--rw-r--r--   0 u03013112   (502) staff       (20)     3790 2023-05-29 09:34:58.805846 u0_stitcher-0.1.5/PKG-INFO
--rw-r--r--   0 u03013112   (502) staff       (20)     3167 2023-05-25 09:48:10.000000 u0_stitcher-0.1.5/README.md
--rw-r--r--   0 u03013112   (502) staff       (20)       38 2023-05-29 09:34:58.806022 u0_stitcher-0.1.5/setup.cfg
--rw-r--r--   0 u03013112   (502) staff       (20)      865 2023-05-29 09:33:23.000000 u0_stitcher-0.1.5/setup.py
-drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-29 09:34:58.804044 u0_stitcher-0.1.5/u0_stitcher/
--rw-r--r--   0 u03013112   (502) staff       (20)       46 2023-05-25 08:29:16.000000 u0_stitcher-0.1.5/u0_stitcher/__init__.py
--rw-r--r--   0 u03013112   (502) staff       (20)      163 2023-05-25 09:15:53.000000 u0_stitcher-0.1.5/u0_stitcher/errors.py
--rw-r--r--   0 u03013112   (502) staff       (20)     4466 2023-05-25 11:37:38.000000 u0_stitcher-0.1.5/u0_stitcher/fisheye2Equirectangular.py
--rw-r--r--   0 u03013112   (502) staff       (20)    10883 2023-05-29 08:50:20.000000 u0_stitcher-0.1.5/u0_stitcher/stitchEasy3.py
--rw-r--r--   0 u03013112   (502) staff       (20)    13180 2023-05-29 09:31:46.000000 u0_stitcher-0.1.5/u0_stitcher/stitcher.py
-drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-05-29 09:34:58.805619 u0_stitcher-0.1.5/u0_stitcher.egg-info/
--rw-r--r--   0 u03013112   (502) staff       (20)     3790 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 u03013112   (502) staff       (20)      328 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 u03013112   (502) staff       (20)        1 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 u03013112   (502) staff       (20)       20 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/requires.txt
--rw-r--r--   0 u03013112   (502) staff       (20)       12 2023-05-29 09:34:58.000000 u0_stitcher-0.1.5/u0_stitcher.egg-info/top_level.txt
+drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-06-05 02:06:54.944492 u0_stitcher-0.1.6/
+-rw-r--r--   0 u03013112   (502) staff       (20)     3790 2023-06-05 02:06:54.944284 u0_stitcher-0.1.6/PKG-INFO
+-rw-r--r--   0 u03013112   (502) staff       (20)     3167 2023-05-25 09:48:10.000000 u0_stitcher-0.1.6/README.md
+-rw-r--r--   0 u03013112   (502) staff       (20)       38 2023-06-05 02:06:54.944568 u0_stitcher-0.1.6/setup.cfg
+-rw-r--r--   0 u03013112   (502) staff       (20)      865 2023-06-05 02:06:51.000000 u0_stitcher-0.1.6/setup.py
+drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-06-05 02:06:54.943315 u0_stitcher-0.1.6/u0_stitcher/
+-rw-r--r--   0 u03013112   (502) staff       (20)       46 2023-05-25 08:29:16.000000 u0_stitcher-0.1.6/u0_stitcher/__init__.py
+-rw-r--r--   0 u03013112   (502) staff       (20)      163 2023-05-25 09:15:53.000000 u0_stitcher-0.1.6/u0_stitcher/errors.py
+-rw-r--r--   0 u03013112   (502) staff       (20)     4466 2023-06-01 06:07:50.000000 u0_stitcher-0.1.6/u0_stitcher/fisheye2Equirectangular.py
+-rw-r--r--   0 u03013112   (502) staff       (20)    10883 2023-05-29 08:50:20.000000 u0_stitcher-0.1.6/u0_stitcher/stitchEasy3.py
+-rw-r--r--   0 u03013112   (502) staff       (20)    13180 2023-05-29 09:31:46.000000 u0_stitcher-0.1.6/u0_stitcher/stitcher.py
+drwxr-xr-x   0 u03013112   (502) staff       (20)        0 2023-06-05 02:06:54.944087 u0_stitcher-0.1.6/u0_stitcher.egg-info/
+-rw-r--r--   0 u03013112   (502) staff       (20)     3790 2023-06-05 02:06:54.000000 u0_stitcher-0.1.6/u0_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 u03013112   (502) staff       (20)      328 2023-06-05 02:06:54.000000 u0_stitcher-0.1.6/u0_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 u03013112   (502) staff       (20)        1 2023-06-05 02:06:54.000000 u0_stitcher-0.1.6/u0_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 u03013112   (502) staff       (20)       20 2023-06-05 02:06:54.000000 u0_stitcher-0.1.6/u0_stitcher.egg-info/requires.txt
+-rw-r--r--   0 u03013112   (502) staff       (20)       12 2023-06-05 02:06:54.000000 u0_stitcher-0.1.6/u0_stitcher.egg-info/top_level.txt
```

### Comparing `u0_stitcher-0.1.5/PKG-INFO` & `u0_stitcher-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: u0_stitcher
-Version: 0.1.5
+Version: 0.1.6
 Summary: stitcher for two fisheye camera
 Home-page: https://github.com/u03013112/pano
 Author: u03013112
 Author-email: u03013112@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `u0_stitcher-0.1.5/README.md` & `u0_stitcher-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `u0_stitcher-0.1.5/setup.py` & `u0_stitcher-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="u0_stitcher",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'opencv-python',
     ],
     author="u03013112",
     author_email="u03013112@hotmail.com",
```

### Comparing `u0_stitcher-0.1.5/u0_stitcher/fisheye2Equirectangular.py` & `u0_stitcher-0.1.6/u0_stitcher/fisheye2Equirectangular.py`

 * *Files identical despite different names*

### Comparing `u0_stitcher-0.1.5/u0_stitcher/stitchEasy3.py` & `u0_stitcher-0.1.6/u0_stitcher/stitchEasy3.py`

 * *Files identical despite different names*

### Comparing `u0_stitcher-0.1.5/u0_stitcher/stitcher.py` & `u0_stitcher-0.1.6/u0_stitcher/stitcher.py`

 * *Files identical despite different names*

### Comparing `u0_stitcher-0.1.5/u0_stitcher.egg-info/PKG-INFO` & `u0_stitcher-0.1.6/u0_stitcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: u0-stitcher
-Version: 0.1.5
+Version: 0.1.6
 Summary: stitcher for two fisheye camera
 Home-page: https://github.com/u03013112/pano
 Author: u03013112
 Author-email: u03013112@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

