# Comparing `tmp/BigBrainGHLPy-0.0.4.tar.gz` & `tmp/BigBrainGHLPy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BigBrainGHLPy-0.0.4.tar", last modified: Mon Jun  5 08:37:19 2023, max compression
+gzip compressed data, was "BigBrainGHLPy-0.0.7.tar", last modified: Mon Jun  5 10:27:48 2023, max compression
```

## Comparing `BigBrainGHLPy-0.0.4.tar` & `BigBrainGHLPy-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:37:19.856901 BigBrainGHLPy-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:37:19.856901 BigBrainGHLPy-0.0.4/BigBrainGHLPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 08:37:19.000000 BigBrainGHLPy-0.0.4/BigBrainGHLPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-05 08:37:19.000000 BigBrainGHLPy-0.0.4/BigBrainGHLPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:37:19.000000 BigBrainGHLPy-0.0.4/BigBrainGHLPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 08:37:19.000000 BigBrainGHLPy-0.0.4/BigBrainGHLPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 08:37:19.000000 BigBrainGHLPy-0.0.4/BigBrainGHLPy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:37:19.856901 BigBrainGHLPy-0.0.4/GHL/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 08:37:10.000000 BigBrainGHLPy-0.0.4/GHL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-06-05 08:37:10.000000 BigBrainGHLPy-0.0.4/GHL/ghlFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 08:37:10.000000 BigBrainGHLPy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 08:37:19.856901 BigBrainGHLPy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 08:37:10.000000 BigBrainGHLPy-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 08:37:19.856901 BigBrainGHLPy-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 08:37:10.000000 BigBrainGHLPy-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/BBGHL/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/BBGHL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/BBGHL/ghlFunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/setup.py
```

### Comparing `BigBrainGHLPy-0.0.4/BigBrainGHLPy.egg-info/PKG-INFO` & `BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BigBrainGHLPy
-Version: 0.0.4
+Version: 0.0.7
 Summary: A basic python wrapper for GoHighLevel
 Author: xtrakTD
 Author-email: <dmitry.m@bbdmgroup.com>
 Keywords: python,ghl,gohighlevel,api,wrapper
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BigBrainGHLPy-0.0.4/GHL/ghlFunctions.py` & `BigBrainGHLPy-0.0.7/BBGHL/ghlFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from typing import Union, Optional
 from datetime import datetime
 from dateutil.tz import tzutc
 import json 
 
 
 
-class GHLPy:
+class GHL:
     
     """
     Class for GHL wrapper 
     """
 
 
     def __init__(self, token):
```

### Comparing `BigBrainGHLPy-0.0.4/LICENSE` & `BigBrainGHLPy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BigBrainGHLPy-0.0.4/PKG-INFO` & `BigBrainGHLPy-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BigBrainGHLPy
-Version: 0.0.4
+Version: 0.0.7
 Summary: A basic python wrapper for GoHighLevel
 Author: xtrakTD
 Author-email: <dmitry.m@bbdmgroup.com>
 Keywords: python,ghl,gohighlevel,api,wrapper
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BigBrainGHLPy-0.0.4/setup.py` & `BigBrainGHLPy-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.7'
 DESCRIPTION = 'A basic python wrapper for GoHighLevel'
 
 
 # Setting up
 setup(
     name="BigBrainGHLPy",
     version=VERSION,
```

