# Comparing `tmp/bnipython-0.6.4.tar.gz` & `tmp/bnipython-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-jehf8h1b/bnipython-0.6.4.tar", last modified: Tue May  9 06:44:45 2023, max compression
+gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-hns9_lgu/bnipython-0.6.5.tar", last modified: Mon Jun  5 03:00:44 2023, max compression
```

## Comparing `bnipython-0.6.4.tar` & `bnipython-0.6.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.198294 bnipython-0.6.4/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.4/LICENSE
--rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-05-09 06:44:45.196762 bnipython-0.6.4/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)    11599 2023-04-18 07:38:12.000000 bnipython-0.6.4/README.md
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.157608 bnipython-0.6.4/bnipython/
--rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.4/bnipython/__init__.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.170124 bnipython-0.6.4/bnipython/lib/
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.173490 bnipython-0.6.4/bnipython/lib/api/
--rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-18 07:21:08.000000 bnipython-0.6.4/bnipython/lib/api/oneGatePayment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.4/bnipython/lib/api/snapBI.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1140 2023-04-18 06:59:40.000000 bnipython-0.6.4/bnipython/lib/bniClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.176941 bnipython-0.6.4/bnipython/lib/net/
--rw-r--r--   0 ikowirya   (501) staff       (20)     3284 2023-05-05 03:23:06.000000 bnipython-0.6.4/bnipython/lib/net/httpClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.185860 bnipython-0.6.4/bnipython/lib/util/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1312 2023-04-18 04:24:59.000000 bnipython-0.6.4/bnipython/lib/util/constants.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1255 2023-04-18 07:30:10.000000 bnipython-0.6.4/bnipython/lib/util/response.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     2448 2023-05-05 03:25:19.000000 bnipython-0.6.4/bnipython/lib/util/utils.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.168767 bnipython-0.6.4/bnipython.egg-info/
--rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/SOURCES.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/dependency_links.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/requires.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/top_level.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-05-09 06:44:45.198708 bnipython-0.6.4/setup.cfg
--rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-05-09 06:40:06.000000 bnipython-0.6.4/setup.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.193564 bnipython-0.6.4/tests/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-18 06:59:40.000000 bnipython-0.6.4/tests/test_bni_client.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    10315 2023-04-18 07:37:16.000000 bnipython-0.6.4/tests/test_one_gate_payment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-05-05 03:44:48.000000 bnipython-0.6.4/tests/test_snap_bi.py
--rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.4/tests/test_util.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-06-05 03:00:44.476366 bnipython-0.6.5/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.5/LICENSE
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-06-05 03:00:44.475103 bnipython-0.6.5/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)    11599 2023-04-18 07:38:12.000000 bnipython-0.6.5/README.md
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-06-05 03:00:44.453411 bnipython-0.6.5/bnipython/
+-rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.5/bnipython/__init__.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-06-05 03:00:44.457566 bnipython-0.6.5/bnipython/lib/
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-06-05 03:00:44.460819 bnipython-0.6.5/bnipython/lib/api/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-18 07:21:08.000000 bnipython-0.6.5/bnipython/lib/api/oneGatePayment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.5/bnipython/lib/api/snapBI.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1140 2023-04-18 06:59:40.000000 bnipython-0.6.5/bnipython/lib/bniClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-06-05 03:00:44.463288 bnipython-0.6.5/bnipython/lib/net/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     3284 2023-05-05 03:23:06.000000 bnipython-0.6.5/bnipython/lib/net/httpClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-06-05 03:00:44.467219 bnipython-0.6.5/bnipython/lib/util/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1308 2023-06-05 03:00:11.000000 bnipython-0.6.5/bnipython/lib/util/constants.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1255 2023-04-18 07:30:10.000000 bnipython-0.6.5/bnipython/lib/util/response.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     2448 2023-05-05 03:25:19.000000 bnipython-0.6.5/bnipython/lib/util/utils.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-06-05 03:00:44.456966 bnipython-0.6.5/bnipython.egg-info/
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-06-05 03:00:44.000000 bnipython-0.6.5/bnipython.egg-info/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-06-05 03:00:44.000000 bnipython-0.6.5/bnipython.egg-info/SOURCES.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-06-05 03:00:44.000000 bnipython-0.6.5/bnipython.egg-info/dependency_links.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-06-05 03:00:44.000000 bnipython-0.6.5/bnipython.egg-info/requires.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-06-05 03:00:44.000000 bnipython-0.6.5/bnipython.egg-info/top_level.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-06-05 03:00:44.476723 bnipython-0.6.5/setup.cfg
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-06-05 02:54:40.000000 bnipython-0.6.5/setup.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-06-05 03:00:44.472735 bnipython-0.6.5/tests/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-18 06:59:40.000000 bnipython-0.6.5/tests/test_bni_client.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    10315 2023-04-18 07:37:16.000000 bnipython-0.6.5/tests/test_one_gate_payment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-05-05 03:44:48.000000 bnipython-0.6.5/tests/test_snap_bi.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.5/tests/test_util.py
```

### Comparing `bnipython-0.6.4/LICENSE` & `bnipython-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/PKG-INFO` & `bnipython-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.4
+Version: 0.6.5
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bnipython-0.6.4/README.md` & `bnipython-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/bnipython/lib/api/oneGatePayment.py` & `bnipython-0.6.5/bnipython/lib/api/oneGatePayment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/bnipython/lib/api/snapBI.py` & `bnipython-0.6.5/bnipython/lib/api/snapBI.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/bnipython/lib/bniClient.py` & `bnipython-0.6.5/bnipython/lib/bniClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/bnipython/lib/net/httpClient.py` & `bnipython-0.6.5/bnipython/lib/net/httpClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/bnipython/lib/util/constants.py` & `bnipython-0.6.5/bnipython/lib/util/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 DEV_BASE_URL = 'https://newapidev.bni.co.id:8066';
 UAT_BASE_URL = 'https://newapidev.bni.co.id:8065';
 SANDBOX_BASE_URL = 'https://sandbox.bni.co.id';
-SANDBOX_DEV_BASE_URL = 'https://sb-dev.harismawan.com';
+SANDBOX_DEV_BASE_URL = 'https://sandbox.dglapm.id';
 PRODUCTION_BASE_URL = 'https://api.bni.co.id';
 # DEV_OGP_URL = 'https://sandbox.harismawan.com'
 # DEV_SNAP_BI = 'https://dev.harismawan.com'
 TOKEN_JWT = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjbGllbnRJZCI6IklEQk5JVkdWemRDQkJVRkE9IiwiYWNjb3VudE5vIjoiMDExNTQ3NjExNyJ9.ljWtFHL0dHhLPw97U8SVWsFV3fRIJItHlQ-HPqCRUwc'
 APP_NAME = 'Test APP'
 APP_NAME_TEST = 'Test Wawat'
```

### Comparing `bnipython-0.6.4/bnipython/lib/util/response.py` & `bnipython-0.6.5/bnipython/lib/util/response.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/bnipython/lib/util/utils.py` & `bnipython-0.6.5/bnipython/lib/util/utils.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/bnipython.egg-info/PKG-INFO` & `bnipython-0.6.5/bnipython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.4
+Version: 0.6.5
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bnipython-0.6.4/bnipython.egg-info/SOURCES.txt` & `bnipython-0.6.5/bnipython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/setup.py` & `bnipython-0.6.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 test_req = pkg_req + [
     'pytest>=3.0.6'
 ]
 
 setup(
     name="bnipython",
-    version="0.6.4",
+    version="0.6.5",
     author="BNI API",
     author_email="",
     license='MIT',
     description="Official  BNI API SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bni-api/bni-python/",
```

### Comparing `bnipython-0.6.4/tests/test_bni_client.py` & `bnipython-0.6.5/tests/test_bni_client.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/tests/test_one_gate_payment.py` & `bnipython-0.6.5/tests/test_one_gate_payment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/tests/test_snap_bi.py` & `bnipython-0.6.5/tests/test_snap_bi.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.4/tests/test_util.py` & `bnipython-0.6.5/tests/test_util.py`

 * *Files identical despite different names*

