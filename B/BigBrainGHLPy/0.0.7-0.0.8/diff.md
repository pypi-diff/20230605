# Comparing `tmp/BigBrainGHLPy-0.0.7.tar.gz` & `tmp/BigBrainGHLPy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BigBrainGHLPy-0.0.7.tar", last modified: Mon Jun  5 10:27:48 2023, max compression
+gzip compressed data, was "BigBrainGHLPy-0.0.8.tar", last modified: Mon Jun  5 11:52:52 2023, max compression
```

## Comparing `BigBrainGHLPy-0.0.7.tar` & `BigBrainGHLPy-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/BBGHL/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/BBGHL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/BBGHL/ghlFunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 10:27:48.000000 BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:27:48.394463 BigBrainGHLPy-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 10:27:38.000000 BigBrainGHLPy-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/BBGHL/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/BBGHL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/BBGHL/ghlFunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 11:52:52.000000 BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 11:52:52.264849 BigBrainGHLPy-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 11:52:42.000000 BigBrainGHLPy-0.0.8/setup.py
```

### Comparing `BigBrainGHLPy-0.0.7/BBGHL/ghlFunctions.py` & `BigBrainGHLPy-0.0.8/BBGHL/ghlFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,15 +308,15 @@
             response = requests.request("DELETE", url, headers=self.headers, data=payload)
             return response.json() 
 
         except Exception as e:
             return e 
 
     
-    def get_contacts(self, after: Optional[Union[int, datetime]], after_id: Optional[str]):
+    def get_contacts(self, after: Optional[Union[int, datetime]] = None, after_id: Optional[str] = None):
         '''
         Get all contacts
         :param after: - timestamp or datetime 
         :param after_id: - str Contact ID 
         :return: - list of GHL contacts. if no params are present - all contacts will be pulled
         '''
 
@@ -363,15 +363,15 @@
 
         try:
             response = requests.request(method='GET', url=url, headers=self.headers)
             return response.json() if not id_only else [x.get('id') for x in response.json().get('pipelines', {})]
         except Exception as e:
             return e
         
-    def get_opportunitiesByPipelline(self, pipeline_id: str, after: Optional[Union[int, datetime]], after_id: Optional[str]):
+    def get_opportunitiesByPipelline(self, pipeline_id: str, after: Optional[Union[int, datetime]] = None, after_id: Optional[str] = None):
         '''
         Get all opportunities for a pipeline 
         :param pipeline_id: - ID of the pipeline
         :param after: - timestamp or datetime 
         :param after_id: - str Opportunity ID 
         '''
```

### Comparing `BigBrainGHLPy-0.0.7/BigBrainGHLPy.egg-info/PKG-INFO` & `BigBrainGHLPy-0.0.8/BigBrainGHLPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BigBrainGHLPy
-Version: 0.0.7
+Version: 0.0.8
 Summary: A basic python wrapper for GoHighLevel
 Author: xtrakTD
 Author-email: <dmitry.m@bbdmgroup.com>
 Keywords: python,ghl,gohighlevel,api,wrapper
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BigBrainGHLPy-0.0.7/LICENSE` & `BigBrainGHLPy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `BigBrainGHLPy-0.0.7/PKG-INFO` & `BigBrainGHLPy-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BigBrainGHLPy
-Version: 0.0.7
+Version: 0.0.8
 Summary: A basic python wrapper for GoHighLevel
 Author: xtrakTD
 Author-email: <dmitry.m@bbdmgroup.com>
 Keywords: python,ghl,gohighlevel,api,wrapper
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BigBrainGHLPy-0.0.7/setup.py` & `BigBrainGHLPy-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'A basic python wrapper for GoHighLevel'
 
 
 # Setting up
 setup(
     name="BigBrainGHLPy",
     version=VERSION,
```

