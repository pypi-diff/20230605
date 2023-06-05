# Comparing `tmp/nemo_library-1.0.6.tar.gz` & `tmp/nemo_library-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo_library-1.0.6.tar", last modified: Sat Jun  3 19:49:11 2023, max compression
+gzip compressed data, was "nemo_library-1.0.7.tar", last modified: Mon Jun  5 20:58:58 2023, max compression
```

## Comparing `nemo_library-1.0.6.tar` & `nemo_library-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:49:11.795197 nemo_library-1.0.6/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-03 19:49:11.794929 nemo_library-1.0.6/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)     1887 2023-06-03 19:14:26.000000 nemo_library-1.0.6/README.md
--rw-r--r--   0 schuglocal   (503) staff       (20)     1971 2023-06-03 19:49:11.000000 nemo_library-1.0.6/README.rst
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:49:11.792436 nemo_library-1.0.6/nemo_library/
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.6/nemo_library/__init__.py
--rw-r--r--   0 schuglocal   (503) staff       (20)    10897 2023-06-03 19:48:41.000000 nemo_library-1.0.6/nemo_library/nemo_library.py
--rw-r--r--   0 schuglocal   (503) staff       (20)      873 2023-06-03 18:41:10.000000 nemo_library-1.0.6/nemo_library/symbols.py
-drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-03 19:49:11.794512 nemo_library-1.0.6/nemo_library.egg-info/
--rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/PKG-INFO
--rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/SOURCES.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/dependency_links.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/requires.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-03 19:49:11.000000 nemo_library-1.0.6/nemo_library.egg-info/top_level.txt
--rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 19:49:11.795255 nemo_library-1.0.6/setup.cfg
--rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-03 19:49:03.000000 nemo_library-1.0.6/setup.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 20:58:58.109400 nemo_library-1.0.7/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-05 20:58:58.109049 nemo_library-1.0.7/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)     1887 2023-06-03 19:14:26.000000 nemo_library-1.0.7/README.md
+-rw-r--r--   0 schuglocal   (503) staff       (20)     1971 2023-06-05 20:58:57.000000 nemo_library-1.0.7/README.rst
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 20:58:58.105550 nemo_library-1.0.7/nemo_library/
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-03 04:48:05.000000 nemo_library-1.0.7/nemo_library/__init__.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)    11883 2023-06-05 20:58:00.000000 nemo_library-1.0.7/nemo_library/nemo_library.py
+-rw-r--r--   0 schuglocal   (503) staff       (20)      680 2023-06-05 20:55:34.000000 nemo_library-1.0.7/nemo_library/symbols.py
+drwxr-xr-x   0 schuglocal   (503) staff       (20)        0 2023-06-05 20:58:58.108231 nemo_library-1.0.7/nemo_library.egg-info/
+-rw-r--r--   0 schuglocal   (503) staff       (20)     2265 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/PKG-INFO
+-rw-r--r--   0 schuglocal   (503) staff       (20)      286 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/SOURCES.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)        1 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/dependency_links.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       16 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/requires.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       13 2023-06-05 20:58:58.000000 nemo_library-1.0.7/nemo_library.egg-info/top_level.txt
+-rw-r--r--   0 schuglocal   (503) staff       (20)       38 2023-06-05 20:58:58.109463 nemo_library-1.0.7/setup.cfg
+-rw-r--r--   0 schuglocal   (503) staff       (20)      534 2023-06-05 20:52:25.000000 nemo_library-1.0.7/setup.py
```

### Comparing `nemo_library-1.0.6/PKG-INFO` & `nemo_library-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo_library
-Version: 1.0.6
+Version: 1.0.7
 Summary: A library for uploading data to and downloading reports from NEMO cloud solution
 Author: Gunnar Schug
 Author-email: GunnarSchug81@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 NEMO Library
```

### Comparing `nemo_library-1.0.6/README.md` & `nemo_library-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.6/README.rst` & `nemo_library-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `nemo_library-1.0.6/nemo_library/nemo_library.py` & `nemo_library-1.0.7/nemo_library/nemo_library.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 import math
 import os
 
 import pandas as pd
 import requests
 
 from nemo_library.symbols import (
-    COGNITO_APPCLIENTID,
-    COGNITO_AUTHFLOW,
-    COGNITO_URL,
     ENDPOINT_URL_PROJECT_FILE_RE_UPLOAD_ABORT,
     ENDPOINT_URL_PROJECT_FILE_RE_UPLOAD_FINALIZE,
     ENDPOINT_URL_PROJECT_FILE_RE_UPLOAD_INITIALIZE,
     ENDPOINT_URL_PROJECT_FILE_RE_UPLOAD_KEEP_ALIVE,
     ENDPOINT_URL_PROJECT_PROPERTIES,
     ENDPOINT_URL_PROJECTS,
     ENDPOINT_URL_REPORT_RESULT,
@@ -25,40 +22,57 @@
 
 class NemoLibrary:
     #################################################################################################################################################################
 
     def __init__(self):
         config = configparser.ConfigParser()
         config.read("config.ini")
+        self._environment_ = config["nemo_library"]["environment"]
         self._userid_ = config["nemo_library"]["userid"]
         self._password_ = config["nemo_library"]["password"]
         self._nemo_url_ = config["nemo_library"]["nemo_url"]
 
+        match self._environment_:
+            case "demo":
+                self._cognito_url_ = 'https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_1ZbUITj21'
+                self._cognito_appclientid = '7tvfugcnunac7id3ebgns6n66u'
+                self._cognito_authflow_ = 'USER_PASSWORD_AUTH'
+            case "dev":
+                self._cognito_url_ = 'https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_778axETqE'
+                self._cognito_appclientid = '4lr89aas81m844o0admv3pfcrp'
+                self._cognito_authflow_ = 'USER_PASSWORD_AUTH'
+            case "prod":
+                self._cognito_url_ = 'https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_1oayObkcF'
+                self._cognito_appclientid = '8t32vcmmdvmva4qvb79gpfhdn'
+                self._cognito_authflow_ = 'USER_PASSWORD_AUTH'
+            case _:
+                raise Exception(f"unknown environment '{self._environment_}' provided")
+            
         super().__init__()
 
     #################################################################################################################################################################
 
     def _login(self):
         headers = {
             "X-Amz-Target": "AWSCognitoIdentityProviderService.InitiateAuth",
             "Content-Type": "application/x-amz-json-1.1",
         }
 
         authparams = {"USERNAME": self._userid_, "PASSWORD": self._password_}
 
         data = {
             "AuthParameters": authparams,
-            "AuthFlow": COGNITO_AUTHFLOW,
-            "ClientId": COGNITO_APPCLIENTID,
+            "AuthFlow": self._cognito_authflow_,
+            "ClientId": self._cognito_appclientid,
         }
 
         # login and get tokenb
 
         response_auth = requests.post(
-            COGNITO_URL, headers=headers, data=json.dumps(data)
+            self._cognito_url_, headers=headers, data=json.dumps(data)
         )
         if response_auth.status_code != 200:
             raise Exception(
                 f"request failed. Status: {response_auth.status_code}, error: {response_auth.text}"
             )
         tokens = json.loads(response_auth.text)
         return tokens["AuthenticationResult"]["IdToken"]
```

### Comparing `nemo_library-1.0.6/nemo_library.egg-info/PKG-INFO` & `nemo_library-1.0.7/nemo_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemo-library
-Version: 1.0.6
+Version: 1.0.7
 Summary: A library for uploading data to and downloading reports from NEMO cloud solution
 Author: Gunnar Schug
 Author-email: GunnarSchug81@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 NEMO Library
```

### Comparing `nemo_library-1.0.6/setup.py` & `nemo_library-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nemo_library',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     install_requires=[
         'requests','pandas'
     ],
     author='Gunnar Schug',
     author_email='GunnarSchug81@gmail.com',
     description='A library for uploading data to and downloading reports from NEMO cloud solution',
```

