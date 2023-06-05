# Comparing `tmp/pysofar-0.1.8.tar.gz` & `tmp/pysofar-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysofar-0.1.8.tar", last modified: Tue Jun  9 23:36:49 2020, max compression
+gzip compressed data, was "dist/pysofar-0.1.9.tar", last modified: Sat Sep 12 00:53:26 2020, max compression
```

## Comparing `pysofar-0.1.8.tar` & `pysofar-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mikesosa   (501) staff       (20)        0 2020-06-09 23:36:49.000000 pysofar-0.1.8/
--rw-r--r--   0 mikesosa   (501) staff       (20)     6616 2020-06-09 23:36:49.000000 pysofar-0.1.8/PKG-INFO
--rw-r--r--   0 mikesosa   (501) staff       (20)     4664 2020-01-08 19:58:25.000000 pysofar-0.1.8/README.md
--rw-r--r--   0 mikesosa   (501) staff       (20)       38 2020-06-09 23:36:49.000000 pysofar-0.1.8/setup.cfg
--rw-r--r--   0 mikesosa   (501) staff       (20)     1303 2020-06-09 23:35:41.000000 pysofar-0.1.8/setup.py
-drwxr-xr-x   0 mikesosa   (501) staff       (20)        0 2020-06-09 23:36:49.000000 pysofar-0.1.8/src/
-drwxr-xr-x   0 mikesosa   (501) staff       (20)        0 2020-06-09 23:36:49.000000 pysofar-0.1.8/src/pysofar/
--rw-r--r--   0 mikesosa   (501) staff       (20)     1832 2020-06-09 18:49:29.000000 pysofar-0.1.8/src/pysofar/__init__.py
--rw-r--r--   0 mikesosa   (501) staff       (20)    19893 2020-06-09 23:00:11.000000 pysofar-0.1.8/src/pysofar/sofar.py
--rw-r--r--   0 mikesosa   (501) staff       (20)     9531 2020-06-09 23:00:11.000000 pysofar-0.1.8/src/pysofar/spotter.py
--rw-r--r--   0 mikesosa   (501) staff       (20)     1515 2020-01-08 19:58:25.000000 pysofar-0.1.8/src/pysofar/tools.py
--rw-r--r--   0 mikesosa   (501) staff       (20)      437 2020-01-08 19:58:25.000000 pysofar-0.1.8/src/pysofar/wavefleet_exceptions.py
-drwxr-xr-x   0 mikesosa   (501) staff       (20)        0 2020-06-09 23:36:49.000000 pysofar-0.1.8/src/pysofar.egg-info/
--rw-r--r--   0 mikesosa   (501) staff       (20)     6616 2020-06-09 23:36:49.000000 pysofar-0.1.8/src/pysofar.egg-info/PKG-INFO
--rw-r--r--   0 mikesosa   (501) staff       (20)      317 2020-06-09 23:36:49.000000 pysofar-0.1.8/src/pysofar.egg-info/SOURCES.txt
--rw-r--r--   0 mikesosa   (501) staff       (20)        1 2020-06-09 23:36:49.000000 pysofar-0.1.8/src/pysofar.egg-info/dependency_links.txt
--rw-r--r--   0 mikesosa   (501) staff       (20)       23 2020-06-09 23:36:49.000000 pysofar-0.1.8/src/pysofar.egg-info/requires.txt
--rw-r--r--   0 mikesosa   (501) staff       (20)        8 2020-06-09 23:36:49.000000 pysofar-0.1.8/src/pysofar.egg-info/top_level.txt
+drwxr-xr-x   0 mikesosa   (501) staff       (20)        0 2020-09-12 00:53:26.000000 pysofar-0.1.9/
+-rw-r--r--   0 mikesosa   (501) staff       (20)     6616 2020-09-12 00:53:26.000000 pysofar-0.1.9/PKG-INFO
+-rw-r--r--   0 mikesosa   (501) staff       (20)     4664 2020-06-09 18:58:48.000000 pysofar-0.1.9/README.md
+-rw-r--r--   0 mikesosa   (501) staff       (20)       38 2020-09-12 00:53:26.000000 pysofar-0.1.9/setup.cfg
+-rw-r--r--   0 mikesosa   (501) staff       (20)     1303 2020-09-12 00:51:46.000000 pysofar-0.1.9/setup.py
+drwxr-xr-x   0 mikesosa   (501) staff       (20)        0 2020-09-12 00:53:26.000000 pysofar-0.1.9/src/
+drwxr-xr-x   0 mikesosa   (501) staff       (20)        0 2020-09-12 00:53:26.000000 pysofar-0.1.9/src/pysofar/
+-rw-r--r--   0 mikesosa   (501) staff       (20)     1867 2020-09-12 00:50:17.000000 pysofar-0.1.9/src/pysofar/__init__.py
+-rw-r--r--   0 mikesosa   (501) staff       (20)    19893 2020-09-11 18:05:44.000000 pysofar-0.1.9/src/pysofar/sofar.py
+-rw-r--r--   0 mikesosa   (501) staff       (20)     9531 2020-09-11 18:05:44.000000 pysofar-0.1.9/src/pysofar/spotter.py
+-rw-r--r--   0 mikesosa   (501) staff       (20)     1515 2020-06-09 18:58:48.000000 pysofar-0.1.9/src/pysofar/tools.py
+-rw-r--r--   0 mikesosa   (501) staff       (20)      437 2020-06-09 18:58:48.000000 pysofar-0.1.9/src/pysofar/wavefleet_exceptions.py
+drwxr-xr-x   0 mikesosa   (501) staff       (20)        0 2020-09-12 00:53:26.000000 pysofar-0.1.9/src/pysofar.egg-info/
+-rw-r--r--   0 mikesosa   (501) staff       (20)     6616 2020-09-12 00:53:26.000000 pysofar-0.1.9/src/pysofar.egg-info/PKG-INFO
+-rw-r--r--   0 mikesosa   (501) staff       (20)      317 2020-09-12 00:53:26.000000 pysofar-0.1.9/src/pysofar.egg-info/SOURCES.txt
+-rw-r--r--   0 mikesosa   (501) staff       (20)        1 2020-09-12 00:53:26.000000 pysofar-0.1.9/src/pysofar.egg-info/dependency_links.txt
+-rw-r--r--   0 mikesosa   (501) staff       (20)       23 2020-09-12 00:53:26.000000 pysofar-0.1.9/src/pysofar.egg-info/requires.txt
+-rw-r--r--   0 mikesosa   (501) staff       (20)        8 2020-09-12 00:53:26.000000 pysofar-0.1.9/src/pysofar.egg-info/top_level.txt
```

### Comparing `pysofar-0.1.8/PKG-INFO` & `pysofar-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysofar
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client for interfacing with the Sofar Wavefleet API to access Spotter Data
 Home-page: https://github.com/wavespotter/wavefleet-client-python
 Author: Rufus Sofar
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 Licesnse
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Project-URL: Spotter About, https://www.sofarocean.com/products/spotter
```

### Comparing `pysofar-0.1.8/README.md` & `pysofar-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pysofar-0.1.8/setup.py` & `pysofar-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     readme_contents = file.read()
 
 setuptools.setup(
     name='pysofar',
-    version='0.1.8',
+    version='0.1.9',
     license='Apache 2 Licesnse',
     install_requires=[
         'requests',
         'python-dotenv'
     ],
     description='Python client for interfacing with the Sofar Wavefleet API to access Spotter Data',
     long_description=readme_contents,
```

### Comparing `pysofar-0.1.8/src/pysofar/__init__.py` & `pysofar-0.1.9/src/pysofar/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 Authors: Mike Sosa
 """
 import os
 import dotenv
 import requests
 import json
 
-# config values
-userpath = os.path.expanduser("~")
-enviromentFile = os.path.join(userpath, 'sofar_api.env')
-dotenv.load_dotenv(enviromentFile)
-token = os.getenv('WF_API_TOKEN')
-
-_wavefleet_token = token
-_endpoint = os.getenv('WF_URL')
-if _endpoint is None:
-    _endpoint = 'https://wavefleet.spoondriftspotter.co/api'
-
 def get_token():
+    # config values
+    userpath = os.path.expanduser("~")
+    enviromentFile = os.path.join(userpath, 'sofar_api.env')
+    dotenv.load_dotenv(enviromentFile)
+    token = os.getenv('WF_API_TOKEN')
+    _wavefleet_token = token
+
     return _wavefleet_token
 
 
 def get_endpoint():
+    _endpoint = os.getenv('WF_URL')
+    if _endpoint is None:
+        _endpoint = 'https://wavefleet.spoondriftspotter.co/api'
     return _endpoint
 
 
 class SofarConnection:
     """
     Base Parent class for connections to the api
     Use SofarApi in sofar.py in practice
```

### Comparing `pysofar-0.1.8/src/pysofar/sofar.py` & `pysofar-0.1.9/src/pysofar/sofar.py`

 * *Files identical despite different names*

### Comparing `pysofar-0.1.8/src/pysofar/spotter.py` & `pysofar-0.1.9/src/pysofar/spotter.py`

 * *Files identical despite different names*

### Comparing `pysofar-0.1.8/src/pysofar/tools.py` & `pysofar-0.1.9/src/pysofar/tools.py`

 * *Files identical despite different names*

### Comparing `pysofar-0.1.8/src/pysofar.egg-info/PKG-INFO` & `pysofar-0.1.9/src/pysofar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysofar
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client for interfacing with the Sofar Wavefleet API to access Spotter Data
 Home-page: https://github.com/wavespotter/wavefleet-client-python
 Author: Rufus Sofar
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 Licesnse
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Project-URL: Spotter About, https://www.sofarocean.com/products/spotter
```

