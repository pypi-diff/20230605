# Comparing `tmp/dartrig-0.1.7.tar.gz` & `tmp/dartrig-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.1.7.tar", last modified: Mon Jun  5 04:12:35 2023, max compression
+gzip compressed data, was "dist/dartrig-0.1.8.tar", last modified: Mon Jun  5 04:16:28 2023, max compression
```

## Comparing `dartrig-0.1.7.tar` & `dartrig-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:12:35.000000 dartrig-0.1.7/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:12:35.000000 dartrig-0.1.7/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.7/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.7/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-05 04:12:34.000000 dartrig-0.1.7/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    15575 2023-06-05 04:12:34.000000 dartrig-0.1.7/dartrig/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.7/dartrig/annotations.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/requires.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-05 04:12:35.000000 dartrig-0.1.7/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:16:28.000000 dartrig-0.1.8/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:16:28.000000 dartrig-0.1.8/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.8/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.8/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-05 04:16:27.000000 dartrig-0.1.8/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    15575 2023-06-05 04:12:34.000000 dartrig-0.1.8/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.8/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/requires.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-05 04:16:28.000000 dartrig-0.1.8/setup.cfg
```

### Comparing `dartrig-0.1.7/PKG-INFO` & `dartrig-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.7
+Version: 0.1.8
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dartrig-0.1.7/LICENSE` & `dartrig-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.7/README.md` & `dartrig-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.7/setup.py` & `dartrig-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.1.7",
+    version="0.1.8",
     install_requires=[
         'requests',
         'bs4',
-        'adt_cache==0.0.11'
+        'adt_cache==0.0.12'
     ],
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="dartrig api wrapper",
     long_description_content_type="text/markdown",
     long_description=open('README.md', "r").read(),
```

### Comparing `dartrig-0.1.7/dartrig/__init__.py` & `dartrig-0.1.8/dartrig/__init__.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.7/dartrig/annotations.py` & `dartrig-0.1.8/dartrig/annotations.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.7/dartrig.egg-info/PKG-INFO` & `dartrig-0.1.8/dartrig.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.7
+Version: 0.1.8
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

