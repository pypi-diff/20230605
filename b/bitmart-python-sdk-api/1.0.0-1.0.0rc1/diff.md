# Comparing `tmp/bitmart-python-sdk-api-1.0.0.tar.gz` & `tmp/bitmart-python-sdk-api-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmart-python-sdk-api-1.0.0.tar", last modified: Mon Jun  5 10:38:42 2023, max compression
+gzip compressed data, was "bitmart-python-sdk-api-1.0.0rc1.tar", last modified: Mon Jun  5 10:28:46 2023, max compression
```

## Comparing `bitmart-python-sdk-api-1.0.0.tar` & `bitmart-python-sdk-api-1.0.0rc1.tar`

### file list

```diff
@@ -1,32 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:42.192257 bitmart-python-sdk-api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-06-05 10:38:42.192257 bitmart-python-sdk-api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:42.192257 bitmart-python-sdk-api-1.0.0/bitmart/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/api_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/api_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/api_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/api_margin_loan.py
--rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/api_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/api_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:42.192257 bitmart-python-sdk-api-1.0.0/bitmart/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_ws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_ws_contract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/ws_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/bitmart/ws_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:42.192257 bitmart-python-sdk-api-1.0.0/bitmart_python_sdk_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-06-05 10:38:42.000000 bitmart-python-sdk-api-1.0.0/bitmart_python_sdk_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-05 10:38:42.000000 bitmart-python-sdk-api-1.0.0/bitmart_python_sdk_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:38:42.000000 bitmart-python-sdk-api-1.0.0/bitmart_python_sdk_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 10:38:42.000000 bitmart-python-sdk-api-1.0.0/bitmart_python_sdk_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 10:38:42.000000 bitmart-python-sdk-api-1.0.0/bitmart_python_sdk_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 10:38:42.192257 bitmart-python-sdk-api-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-05 10:38:39.000000 bitmart-python-sdk-api-1.0.0/setup.py
+drwxr-xr-x   0 zengningzhong   (501) staff       (20)        0 2023-06-05 10:28:46.938706 bitmart-python-sdk-api-1.0.0rc1/
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     1068 2023-05-31 07:51:47.000000 bitmart-python-sdk-api-1.0.0rc1/LICENSE.md
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     8628 2023-06-05 10:28:46.938968 bitmart-python-sdk-api-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     7873 2023-06-05 09:48:40.000000 bitmart-python-sdk-api-1.0.0rc1/README.md
+drwxr-xr-x   0 zengningzhong   (501) staff       (20)        0 2023-06-05 10:28:46.914584 bitmart-python-sdk-api-1.0.0rc1/bitmart/
+-rw-r--r--   0 zengningzhong   (501) staff       (20)       94 2020-05-25 08:18:02.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/__init__.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)       26 2023-06-05 10:28:28.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/__version__.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     6514 2023-06-05 03:27:54.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/api_account.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     1045 2023-06-05 03:27:54.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/api_broker.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)    13449 2023-06-05 03:27:54.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/api_contract.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     4868 2023-06-05 03:27:54.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/api_margin_loan.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)    15806 2023-06-05 03:27:54.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/api_spot.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)      863 2023-06-05 03:27:54.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/api_system.py
+drwxr-xr-x   0 zengningzhong   (501) staff       (20)        0 2023-06-05 10:28:46.924158 bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/
+-rw-r--r--   0 zengningzhong   (501) staff       (20)        0 2023-06-01 08:34:10.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/__init__.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     3130 2023-06-01 08:44:22.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_client.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     5833 2023-06-03 06:02:13.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_consts.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)      628 2020-12-30 07:21:33.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_exceptions.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)      636 2020-07-16 12:17:54.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_log.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     1028 2023-06-03 05:43:02.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_utils.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     2584 2023-06-05 04:20:59.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_ws_client.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     2076 2023-06-05 04:20:59.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_ws_contract_client.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     4739 2023-06-02 13:16:44.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/ws_contract.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     4666 2023-06-02 13:16:44.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart/ws_spot.py
+drwxr-xr-x   0 zengningzhong   (501) staff       (20)        0 2023-06-05 10:28:46.929002 bitmart-python-sdk-api-1.0.0rc1/bitmart_python_sdk_api.egg-info/
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     8628 2023-06-05 10:28:46.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart_python_sdk_api.egg-info/PKG-INFO
+-rw-r--r--   0 zengningzhong   (501) staff       (20)      930 2023-06-05 10:28:46.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart_python_sdk_api.egg-info/SOURCES.txt
+-rw-r--r--   0 zengningzhong   (501) staff       (20)        1 2023-06-05 10:28:46.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart_python_sdk_api.egg-info/dependency_links.txt
+-rw-r--r--   0 zengningzhong   (501) staff       (20)       33 2023-06-05 10:28:46.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart_python_sdk_api.egg-info/requires.txt
+-rw-r--r--   0 zengningzhong   (501) staff       (20)        8 2023-06-05 10:28:46.000000 bitmart-python-sdk-api-1.0.0rc1/bitmart_python_sdk_api.egg-info/top_level.txt
+-rw-r--r--   0 zengningzhong   (501) staff       (20)      207 2023-06-05 10:28:46.940615 bitmart-python-sdk-api-1.0.0rc1/setup.cfg
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     1545 2023-06-03 04:27:21.000000 bitmart-python-sdk-api-1.0.0rc1/setup.py
+drwxr-xr-x   0 zengningzhong   (501) staff       (20)        0 2023-06-05 10:28:46.937472 bitmart-python-sdk-api-1.0.0rc1/tests/
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     2640 2023-06-03 05:59:22.000000 bitmart-python-sdk-api-1.0.0rc1/tests/test_api_account.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)      615 2023-02-25 06:21:32.000000 bitmart-python-sdk-api-1.0.0rc1/tests/test_api_broker.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     4370 2023-06-05 04:27:48.000000 bitmart-python-sdk-api-1.0.0rc1/tests/test_api_contract.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     2178 2023-06-03 06:18:15.000000 bitmart-python-sdk-api-1.0.0rc1/tests/test_api_margin_loan.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     4915 2023-06-05 03:21:33.000000 bitmart-python-sdk-api-1.0.0rc1/tests/test_api_spot.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)      445 2020-07-16 12:17:54.000000 bitmart-python-sdk-api-1.0.0rc1/tests/test_api_system.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     1539 2023-06-05 04:27:48.000000 bitmart-python-sdk-api-1.0.0rc1/tests/test_ws_contract.py
+-rw-r--r--   0 zengningzhong   (501) staff       (20)     1490 2023-06-05 04:27:48.000000 bitmart-python-sdk-api-1.0.0rc1/tests/test_ws_spot.py
```

### Comparing `bitmart-python-sdk-api-1.0.0/LICENSE.md` & `bitmart-python-sdk-api-1.0.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/PKG-INFO` & `bitmart-python-sdk-api-1.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmart-python-sdk-api
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: BitMart Exchange official(https://bitmart.com) Python client for the BitMart Cloud API
 Home-page: https://github.com/bitmartexchange/bitmart-python-sdk-api
 License: MIT
 Keywords: BitMart Exchange,BitMart API,BitMart Websocket
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bitmart-python-sdk-api-1.0.0/README.md` & `bitmart-python-sdk-api-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/api_account.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/api_account.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/api_broker.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/api_broker.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/api_contract.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/api_contract.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/api_margin_loan.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/api_margin_loan.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/api_spot.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/api_spot.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/api_system.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/api_system.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_client.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_client.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_consts.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_consts.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_exceptions.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_exceptions.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_log.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_log.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_utils.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_utils.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_ws_client.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_ws_client.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/lib/cloud_ws_contract_client.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/lib/cloud_ws_contract_client.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/ws_contract.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/ws_contract.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart/ws_spot.py` & `bitmart-python-sdk-api-1.0.0rc1/bitmart/ws_spot.py`

 * *Files identical despite different names*

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart_python_sdk_api.egg-info/PKG-INFO` & `bitmart-python-sdk-api-1.0.0rc1/bitmart_python_sdk_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmart-python-sdk-api
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: BitMart Exchange official(https://bitmart.com) Python client for the BitMart Cloud API
 Home-page: https://github.com/bitmartexchange/bitmart-python-sdk-api
 License: MIT
 Keywords: BitMart Exchange,BitMart API,BitMart Websocket
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bitmart-python-sdk-api-1.0.0/bitmart_python_sdk_api.egg-info/SOURCES.txt` & `bitmart-python-sdk-api-1.0.0rc1/bitmart_python_sdk_api.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,16 @@
 bitmart/lib/cloud_utils.py
 bitmart/lib/cloud_ws_client.py
 bitmart/lib/cloud_ws_contract_client.py
 bitmart_python_sdk_api.egg-info/PKG-INFO
 bitmart_python_sdk_api.egg-info/SOURCES.txt
 bitmart_python_sdk_api.egg-info/dependency_links.txt
 bitmart_python_sdk_api.egg-info/requires.txt
-bitmart_python_sdk_api.egg-info/top_level.txt
+bitmart_python_sdk_api.egg-info/top_level.txt
+tests/test_api_account.py
+tests/test_api_broker.py
+tests/test_api_contract.py
+tests/test_api_margin_loan.py
+tests/test_api_spot.py
+tests/test_api_system.py
+tests/test_ws_contract.py
+tests/test_ws_spot.py
```

### Comparing `bitmart-python-sdk-api-1.0.0/setup.py` & `bitmart-python-sdk-api-1.0.0rc1/setup.py`

 * *Files identical despite different names*

