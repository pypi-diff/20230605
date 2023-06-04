# Comparing `tmp/mlplatformutils-0.6.tar.gz` & `tmp/mlplatformutils-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.6.tar", last modified: Sun Jun  4 22:01:24 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.7.tar", last modified: Sun Jun  4 22:33:53 2023, max compression
```

## Comparing `mlplatformutils-0.6.tar` & `mlplatformutils-0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.385226 mlplatformutils-0.6/
--rw-rw-rw-   0        0        0     3625 2023-06-04 22:01:24.386211 mlplatformutils-0.6/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-06-04 02:08:17.000000 mlplatformutils-0.6/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-04 22:01:24.390744 mlplatformutils-0.6/setup.cfg
--rw-rw-rw-   0        0        0      536 2023-06-04 22:00:52.000000 mlplatformutils-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.153628 mlplatformutils-0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.191636 mlplatformutils-0.6/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.6/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.381209 mlplatformutils-0.6/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.6/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.6/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.6/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.6/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.6/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.6/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       19 2023-06-04 22:00:56.000000 mlplatformutils-0.6/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.272642 mlplatformutils-0.6/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3625 2023-06-04 22:01:23.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-04 22:01:24.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 22:01:23.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-04 22:01:23.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-04 22:01:23.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 22:33:53.504696 mlplatformutils-0.7/
+-rw-rw-rw-   0        0        0     3676 2023-06-04 22:33:53.505695 mlplatformutils-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.7/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-04 22:33:53.510696 mlplatformutils-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      654 2023-06-04 22:33:49.000000 mlplatformutils-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 22:33:53.397151 mlplatformutils-0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 22:33:53.420054 mlplatformutils-0.7/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.7/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 22:33:53.501697 mlplatformutils-0.7/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.7/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.7/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.7/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.7/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.7/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.7/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       19 2023-06-04 22:30:59.000000 mlplatformutils-0.7/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-04 22:33:53.461711 mlplatformutils-0.7/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3676 2023-06-04 22:33:53.000000 mlplatformutils-0.7/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-04 22:33:53.000000 mlplatformutils-0.7/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 22:33:53.000000 mlplatformutils-0.7/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-04 22:33:53.000000 mlplatformutils-0.7/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-04 22:33:53.000000 mlplatformutils-0.7/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.6/PKG-INFO` & `mlplatformutils-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.6
+Version: 0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Description: # mlplatformutils
         
@@ -89,8 +89,9 @@
         from mlplatformutils.core.app_insights_logger import telemetrylogger
         from mlplatformutils.core.lineagegraph import LineageGraph
         from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2
         import mlplatformutils.core.platformutils as mlpu
         mlpu.__version__
 Keywords: mlplatformutils
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.6/setup.py` & `mlplatformutils-0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from setuptools import setup, find_packages
+import os
+directory = os.getcwd()
 
-with open('README.md') as f:
+with open(directory+"/README.md") as f:
     long_description = f.read()
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.6',
+    version='0.7',
     license='MIT',
+    classifiers=[
+        'Programming Language :: Python :: 3.8'
+    ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     keywords='mlplatformutils',
     install_requires=[
           'applicationinsights','gremlinpython','azureml-core'
```

### Comparing `mlplatformutils-0.6/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.7/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.6/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.7/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.6/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.7/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.6/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.7/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.6/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.7/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.6/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.7/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.6
+Version: 0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Description: # mlplatformutils
         
@@ -89,8 +89,9 @@
         from mlplatformutils.core.app_insights_logger import telemetrylogger
         from mlplatformutils.core.lineagegraph import LineageGraph
         from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2
         import mlplatformutils.core.platformutils as mlpu
         mlpu.__version__
 Keywords: mlplatformutils
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.6/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.7/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

