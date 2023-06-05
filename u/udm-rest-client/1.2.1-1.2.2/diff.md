# Comparing `tmp/udm-rest-client-1.2.1.tar.gz` & `tmp/udm-rest-client-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udm-rest-client-1.2.1.tar", last modified: Wed Feb 15 12:13:24 2023, max compression
+gzip compressed data, was "udm-rest-client-1.2.2.tar", last modified: Mon Jun  5 13:08:48 2023, max compression
```

## Comparing `udm-rest-client-1.2.1.tar` & `udm-rest-client-1.2.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-02-15 12:13:24.377787 udm-rest-client-1.2.1/
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     4556 2022-11-29 07:28:13.000000 udm-rest-client-1.2.1/CONTRIBUTING.rst
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)     3754 2023-02-15 12:11:58.000000 udm-rest-client-1.2.1/HISTORY.rst
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     1147 2023-02-15 11:29:41.000000 udm-rest-client-1.2.1/LICENSE
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      218 2019-11-13 22:29:06.000000 udm-rest-client-1.2.1/MANIFEST.in
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)    12624 2023-02-15 12:13:24.377787 udm-rest-client-1.2.1/PKG-INFO
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     7714 2023-02-15 11:26:11.000000 udm-rest-client-1.2.1/README.rst
-drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-02-15 12:13:24.377787 udm-rest-client-1.2.1/docs/
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      617 2019-09-30 05:43:41.000000 udm-rest-client-1.2.1/docs/Makefile
--rwxr-xr-x   0 dtroeder  (2311) dtroeder  (1001)     5714 2023-02-15 11:29:14.000000 udm-rest-client-1.2.1/docs/conf.py
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)       33 2019-09-06 03:21:51.000000 udm-rest-client-1.2.1/docs/contributing.rst
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)       28 2019-09-06 03:21:51.000000 udm-rest-client-1.2.1/docs/history.rst
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      320 2019-09-25 13:30:52.000000 udm-rest-client-1.2.1/docs/index.rst
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     1252 2022-11-29 07:29:12.000000 udm-rest-client-1.2.1/docs/installation.rst
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      814 2019-09-30 05:43:49.000000 udm-rest-client-1.2.1/docs/make.bat
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)       82 2019-11-24 06:47:05.000000 udm-rest-client-1.2.1/docs/modules.rst
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)       27 2019-09-06 03:21:51.000000 udm-rest-client-1.2.1/docs/readme.rst
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      840 2019-11-24 06:47:05.000000 udm-rest-client-1.2.1/docs/udm_rest_client.rst
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     6382 2022-11-09 15:12:58.000000 udm-rest-client-1.2.1/docs/usage.rst
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)       92 2022-01-18 08:33:00.000000 udm-rest-client-1.2.1/requirements.txt
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      137 2022-01-03 07:09:54.000000 udm-rest-client-1.2.1/requirements_dev.txt
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      205 2022-01-03 07:10:55.000000 udm-rest-client-1.2.1/requirements_test.txt
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      719 2023-02-15 12:13:24.381787 udm-rest-client-1.2.1/setup.cfg
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)     2034 2023-02-15 11:28:06.000000 udm-rest-client-1.2.1/setup.py
-drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-02-15 12:13:24.377787 udm-rest-client-1.2.1/tests/
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)    17049 2022-10-19 06:23:07.000000 udm-rest-client-1.2.1/tests/conftest.py
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     4830 2021-01-29 20:55:57.000000 udm-rest-client-1.2.1/tests/test_base.py
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)    43665 2023-01-16 17:33:54.000000 udm-rest-client-1.2.1/tests/test_base_http.py
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      194 2023-02-15 11:44:07.000000 udm-rest-client-1.2.1/tests/test_server.yaml
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      122 2021-01-29 16:19:28.000000 udm-rest-client-1.2.1/tests/test_server.yaml_10.200.3.152
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      121 2021-12-13 21:58:47.000000 udm-rest-client-1.2.1/tests/test_server.yaml_10.200.3.31
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      120 2021-12-13 21:54:06.000000 udm-rest-client-1.2.1/tests/test_server.yaml_10.9.165.5
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      130 2021-12-09 19:30:01.000000 udm-rest-client-1.2.1/tests/test_server.yaml_172.17.0.2
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)      187 2023-02-15 11:21:09.000000 udm-rest-client-1.2.1/tests/test_server_example.yaml
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     1377 2021-12-23 08:37:56.000000 udm-rest-client-1.2.1/tests/test_test.py
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     4101 2022-10-19 06:23:07.000000 udm-rest-client-1.2.1/tests/test_udm.py
-drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-02-15 12:13:24.377787 udm-rest-client-1.2.1/udm_rest_client/
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)      769 2023-02-15 11:28:13.000000 udm-rest-client-1.2.1/udm_rest_client/__init__.py
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)    12359 2023-02-15 11:29:41.000000 udm-rest-client-1.2.1/udm_rest_client/base.py
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)    50617 2023-02-15 11:29:41.000000 udm-rest-client-1.2.1/udm_rest_client/base_http.py
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     3458 2023-02-15 11:29:41.000000 udm-rest-client-1.2.1/udm_rest_client/exceptions.py
--rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)    10023 2023-02-15 11:29:41.000000 udm-rest-client-1.2.1/udm_rest_client/udm.py
-drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-02-15 12:13:24.377787 udm-rest-client-1.2.1/udm_rest_client.egg-info/
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)    12624 2023-02-15 12:13:24.000000 udm-rest-client-1.2.1/udm_rest_client.egg-info/PKG-INFO
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)     1007 2023-02-15 12:13:24.000000 udm-rest-client-1.2.1/udm_rest_client.egg-info/SOURCES.txt
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)        1 2023-02-15 12:13:24.000000 udm-rest-client-1.2.1/udm_rest_client.egg-info/dependency_links.txt
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)        1 2023-02-15 12:13:24.000000 udm-rest-client-1.2.1/udm_rest_client.egg-info/not-zip-safe
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)       92 2023-02-15 12:13:24.000000 udm-rest-client-1.2.1/udm_rest_client.egg-info/requires.txt
--rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)       16 2023-02-15 12:13:24.000000 udm-rest-client-1.2.1/udm_rest_client.egg-info/top_level.txt
--rwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)    11001 2023-02-15 12:05:23.000000 udm-rest-client-1.2.1/update_openapi_client
+drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-06-05 13:08:48.740331 udm-rest-client-1.2.2/
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     4556 2022-11-29 07:28:13.000000 udm-rest-client-1.2.2/CONTRIBUTING.rst
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)     3949 2023-06-05 13:06:57.000000 udm-rest-client-1.2.2/HISTORY.rst
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     1147 2023-02-15 11:29:41.000000 udm-rest-client-1.2.2/LICENSE
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      218 2019-11-13 22:29:06.000000 udm-rest-client-1.2.2/MANIFEST.in
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)    12819 2023-06-05 13:08:48.740331 udm-rest-client-1.2.2/PKG-INFO
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     7714 2023-02-15 11:26:11.000000 udm-rest-client-1.2.2/README.rst
+drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-06-05 13:08:48.736331 udm-rest-client-1.2.2/docs/
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      617 2019-09-30 05:43:41.000000 udm-rest-client-1.2.2/docs/Makefile
+-rwxr-xr-x   0 dtroeder  (2311) dtroeder  (1001)     5714 2023-02-15 11:29:14.000000 udm-rest-client-1.2.2/docs/conf.py
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)       33 2019-09-06 03:21:51.000000 udm-rest-client-1.2.2/docs/contributing.rst
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)       28 2019-09-06 03:21:51.000000 udm-rest-client-1.2.2/docs/history.rst
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      320 2019-09-25 13:30:52.000000 udm-rest-client-1.2.2/docs/index.rst
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     1252 2022-11-29 07:29:12.000000 udm-rest-client-1.2.2/docs/installation.rst
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      814 2019-09-30 05:43:49.000000 udm-rest-client-1.2.2/docs/make.bat
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)       82 2019-11-24 06:47:05.000000 udm-rest-client-1.2.2/docs/modules.rst
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)       27 2019-09-06 03:21:51.000000 udm-rest-client-1.2.2/docs/readme.rst
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      840 2019-11-24 06:47:05.000000 udm-rest-client-1.2.2/docs/udm_rest_client.rst
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     6382 2022-11-09 15:12:58.000000 udm-rest-client-1.2.2/docs/usage.rst
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)       92 2023-06-01 06:28:49.000000 udm-rest-client-1.2.2/requirements.txt
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      137 2022-01-03 07:09:54.000000 udm-rest-client-1.2.2/requirements_dev.txt
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      205 2022-01-03 07:10:55.000000 udm-rest-client-1.2.2/requirements_test.txt
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      719 2023-06-05 13:08:48.740331 udm-rest-client-1.2.2/setup.cfg
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)     2034 2023-06-05 13:06:04.000000 udm-rest-client-1.2.2/setup.py
+drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-06-05 13:08:48.736331 udm-rest-client-1.2.2/tests/
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)    17140 2023-06-01 12:36:14.000000 udm-rest-client-1.2.2/tests/conftest.py
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     4811 2023-06-01 07:34:50.000000 udm-rest-client-1.2.2/tests/test_base.py
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)    44282 2023-06-05 13:00:54.000000 udm-rest-client-1.2.2/tests/test_base_http.py
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      194 2023-02-15 11:44:07.000000 udm-rest-client-1.2.2/tests/test_server.yaml
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      122 2021-01-29 16:19:28.000000 udm-rest-client-1.2.2/tests/test_server.yaml_10.200.3.152
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      121 2021-12-13 21:58:47.000000 udm-rest-client-1.2.2/tests/test_server.yaml_10.200.3.31
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      120 2021-12-13 21:54:06.000000 udm-rest-client-1.2.2/tests/test_server.yaml_10.9.165.5
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)      130 2021-12-09 19:30:01.000000 udm-rest-client-1.2.2/tests/test_server.yaml_172.17.0.2
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)      187 2023-06-01 06:27:44.000000 udm-rest-client-1.2.2/tests/test_server_example.yaml
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     1377 2021-12-23 08:37:56.000000 udm-rest-client-1.2.2/tests/test_test.py
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     4101 2022-10-19 06:23:07.000000 udm-rest-client-1.2.2/tests/test_udm.py
+drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-06-05 13:08:48.740331 udm-rest-client-1.2.2/udm_rest_client/
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)      769 2023-06-05 13:01:49.000000 udm-rest-client-1.2.2/udm_rest_client/__init__.py
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)    12359 2023-02-15 11:29:41.000000 udm-rest-client-1.2.2/udm_rest_client/base.py
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)    50483 2023-06-01 12:26:03.000000 udm-rest-client-1.2.2/udm_rest_client/base_http.py
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)     3458 2023-02-15 11:29:41.000000 udm-rest-client-1.2.2/udm_rest_client/exceptions.py
+-rw-r--r--   0 dtroeder  (2311) dtroeder  (1001)    10023 2023-02-15 11:29:41.000000 udm-rest-client-1.2.2/udm_rest_client/udm.py
+drwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)        0 2023-06-05 13:08:48.740331 udm-rest-client-1.2.2/udm_rest_client.egg-info/
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)    12819 2023-06-05 13:08:48.000000 udm-rest-client-1.2.2/udm_rest_client.egg-info/PKG-INFO
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)     1007 2023-06-05 13:08:48.000000 udm-rest-client-1.2.2/udm_rest_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)        1 2023-06-05 13:08:48.000000 udm-rest-client-1.2.2/udm_rest_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)        1 2023-06-05 13:08:48.000000 udm-rest-client-1.2.2/udm_rest_client.egg-info/not-zip-safe
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)       92 2023-06-05 13:08:48.000000 udm-rest-client-1.2.2/udm_rest_client.egg-info/requires.txt
+-rw-rw-r--   0 dtroeder  (2311) dtroeder  (1001)       16 2023-06-05 13:08:48.000000 udm-rest-client-1.2.2/udm_rest_client.egg-info/top_level.txt
+-rwxrwxr-x   0 dtroeder  (2311) dtroeder  (1001)    11001 2023-02-15 12:05:23.000000 udm-rest-client-1.2.2/update_openapi_client
```

### Comparing `udm-rest-client-1.2.1/CONTRIBUTING.rst` & `udm-rest-client-1.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/HISTORY.rst` & `udm-rest-client-1.2.2/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+1.2.2 (2023-06-05)
+-------------------
+
+* Fix ``update_openapi_client`` crashing with newer versions of the Python Docker client and ``requests`` (Issue #10).
+* Testing fixes (Issues #5 and #9)
+
 1.2.1 (2023-02-15)
 -------------------
 
 * Update OpenAPI client library generator (openapitools/openapi-generator-cli) to version ``5.4.0`` to support Python 3.11..
 
 1.1.1 (2023-01-16)
 -------------------
```

### Comparing `udm-rest-client-1.2.1/LICENSE` & `udm-rest-client-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/PKG-INFO` & `udm-rest-client-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udm-rest-client
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python library to interact with the Univention UDM REST API. Implements the simple Python UDM API.
 Home-page: https://github.com/univention/python-udm-rest-api-client
 Author: Daniel Troeder
 Author-email: troeder@univention.de
 License: GNU Affero General Public License v3
 Keywords: Univention UCS UDM REST
 Classifier: Development Status :: 4 - Beta
@@ -199,14 +199,20 @@
     :target: https://github.com/univention/python-udm-rest-api-client/actions?query=workflow%3A%22Integration+tests%22
 
 
 =======
 History
 =======
 
+1.2.2 (2023-06-05)
+-------------------
+
+* Fix ``update_openapi_client`` crashing with newer versions of the Python Docker client and ``requests`` (Issue #10).
+* Testing fixes (Issues #5 and #9)
+
 1.2.1 (2023-02-15)
 -------------------
 
 * Update OpenAPI client library generator (openapitools/openapi-generator-cli) to version ``5.4.0`` to support Python 3.11..
 
 1.1.1 (2023-01-16)
 -------------------
```

### Comparing `udm-rest-client-1.2.1/README.rst` & `udm-rest-client-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/docs/Makefile` & `udm-rest-client-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/docs/conf.py` & `udm-rest-client-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/docs/installation.rst` & `udm-rest-client-1.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/docs/make.bat` & `udm-rest-client-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/docs/udm_rest_client.rst` & `udm-rest-client-1.2.2/docs/udm_rest_client.rst`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/docs/usage.rst` & `udm-rest-client-1.2.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/setup.cfg` & `udm-rest-client-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/setup.py` & `udm-rest-client-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     install_requires=requirements,
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     python_requires=">=3.6",
     scripts=["update_openapi_client"],
     url="https://github.com/univention/python-udm-rest-api-client",
-    version="1.2.1",
+    version="1.2.2",
     zip_safe=False,
 )
```

### Comparing `udm-rest-client-1.2.1/tests/conftest.py` & `udm-rest-client-1.2.2/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             user_dn=os.environ["UCS_USERDN"],
             password=os.environ["UCS_PASSWORD"],
         )
         _test_a_server_configuration(res)
     except (IndexError, KeyError):
         print("Test server config not found in environment.")
     except LDAPInvalidDnError as exc:
-        raise BadTestServerConfig(f"Invalid DN in environment variable 'UCS_USERDN': {exc!s}")
+        raise BadTestServerConfig(f"Invalid DN in environment variable 'UCS_USERDN': {exc!s}") from exc
     except udm_rest_client.exceptions.APICommunicationError as exc:
         raise BadTestServerConfig(
             f"Error connecting to test server using credentials from the "
             f"environment: [{exc.status}] {exc.reason}"
         ) from exc
     else:
         return res
@@ -293,15 +293,15 @@
     res = {
         "username": test_server_configuration.username,
         "password": test_server_configuration.password,
         "url": f"https://{test_server_configuration.host}/univention/udm",
         "safe_chars_for_path_param": "/",
         "ssl_ca_cert": str(ucs_ca_file_path(test_server_configuration.host)),
     }
-    if not any(c in string.ascii_letters for c in test_server_configuration.host):
+    if all(c not in string.ascii_letters for c in test_server_configuration.host):
         # it's an IP address, don't try to verify the certificate even if we have the CA
         res["verify_ssl"] = False
     return res
 
 
 @pytest.fixture(scope="session")
 def ldap_connection_credentials(test_server_configuration) -> Dict[str, Any]:
@@ -373,16 +373,17 @@
 
 @pytest.fixture(scope="session")
 def http_headers_write():
     return {"Accept": "application/json", "Content-Type": "application/json"}
 
 
 @pytest.fixture
-def user_created_via_http(http_headers_write, udm_kwargs, user_resource_kwargs, delete_user_via_http):
-    created_user_dns = []
+def user_created_via_http(
+    http_headers_write, udm_kwargs, user_resource_kwargs, schedule_delete_object_via_http
+):
     auth = (udm_kwargs["username"], udm_kwargs["password"])
     url = f"{udm_kwargs['url']}/users/user/"
     if udm_kwargs.get("verify_ssl", True):
         verify_ssl = udm_kwargs.get("ssl_ca_cert", False)  # pragma: no cover
     else:
         verify_ssl = False
 
@@ -392,139 +393,144 @@
 
         resp = requests.post(url, headers=http_headers_write, json=data, auth=auth, verify=verify_ssl)
         print(resp.reason)
         try:
             print(resp.json())
         except (AttributeError, ValueError):  # pragma: no cover
             print(resp.text)
-        assert resp.status_code in (201, 204)
+        assert resp.status_code in {201, 204}
         obj_url = resp.headers["Location"]
         dn = unquote(obj_url.rsplit("/", 1)[-1])
-        created_user_dns.append(dn)
+        schedule_delete_object_via_http("users/user", dn)
         return dn, obj_url, data
 
-    yield _func
-
-    for dn in created_user_dns:
-        delete_user_via_http(dn)
+    return _func
 
 
 @pytest.fixture
 def modify_user_via_http(base_dn, http_headers_write, udm_kwargs):
     auth = (udm_kwargs["username"], udm_kwargs["password"])
 
     def _func(dn: str, user: User) -> None:
         url = f"{udm_kwargs['url']}/users/user/{dn}"
-        data = dict((k, v) for k, v in attr.asdict(user).items() if v and k not in ("dn", "uri", "uuid"))
+        data = {k: v for k, v in attr.asdict(user).items() if v and k not in ("dn", "uri", "uuid")}
         properties = data.pop("props", {})
-        data["properties"] = dict((k, v) for k, v in properties.items() if v)
+        data["properties"] = {k: v for k, v in properties.items() if v}
         if udm_kwargs.get("verify_ssl", True):
             verify_ssl = udm_kwargs.get("ssl_ca_cert", False)  # pragma: no cover
         else:
             verify_ssl = False
 
         resp = requests.patch(url, headers=http_headers_write, json=data, auth=auth, verify=verify_ssl)
         assert resp.status_code == 204
 
     return _func
 
 
 @pytest.fixture
-def delete_user_via_http(base_dn, http_headers_read, udm_kwargs):
+def delete_object_via_http(http_headers_read, udm_kwargs) -> Callable[[str, str], None]:
     auth = (udm_kwargs["username"], udm_kwargs["password"])
     if udm_kwargs.get("verify_ssl", True):
         verify_ssl = udm_kwargs.get("ssl_ca_cert", False)  # pragma: no cover
     else:
         verify_ssl = False
 
-    def _func(dn: str) -> None:
-        url = f"{udm_kwargs['url']}/users/user/{dn}"
+    def _delete_object_via_http(udm_module: str, dn: str) -> None:
+        url = f"{udm_kwargs['url']}/{udm_module}/{dn}"
         resp = requests.delete(url, headers=http_headers_read, auth=auth, verify=verify_ssl)
-        assert resp.status_code in (204, 404)
+        assert resp.status_code in {204, 404}
 
-    return _func
+    return _delete_object_via_http
+
+
+@pytest.fixture
+def schedule_delete_object_via_http(delete_object_via_http) -> Callable[[str, str], None]:
+    objects: List[Tuple[str, str]] = []
+
+    def _schedule_delete_object_via_http(udm_module: str, dn: str) -> None:
+        objects.append((udm_module, dn))
+
+    yield _schedule_delete_object_via_http
+
+    for udm_module, dn in objects:
+        delete_object_via_http(udm_module, dn)
 
 
 def pytest_generate_tests(metafunc):
-    if "serialize_obj_data" in metafunc.fixturenames:
-        an_int = fake.pyint()
-        a_float = fake.pyfloat()
-        a_date: datetime.date = fake.date_object()
-        a_dict: Dict[str, Any] = fake.pydict(10, True, int, str, bool, float)
-        a_dict["dict"] = {"nested_bool": fake.pybool(), "nested_int": fake.pyint()}
-        a_dict["date"] = fake.date_object()
-        a_dict["none"] = None
-        a_dict["_ignoreme"] = fake.pyint()
-        a_dict_exp = copy.deepcopy(a_dict)
-        a_dict_exp["date"] = a_dict_exp["date"].strftime("%Y-%m-%d")
-        del a_dict_exp["_ignoreme"]
-        a_list: List[Any] = fake.pylist(10, True, int, str, bool, float)
-        a_list.insert(2, fake.date_object())
-        a_list_exp = copy.deepcopy(a_list)
-        a_list_exp[2] = a_list_exp[2].strftime("%Y-%m-%d")
-        a_tuple = fake.pytuple(10, True, int, str, bool, float)
-        user = UserFactory()
-        user.position = user.position.format(base_dn="dc=base,dc=dn")
-        user.dn = f"uid={user.props.username},{user.position}"
-        a_udm_obj = UsersUserUdmObjectFactory(user_data=user)
-        an_api_obj = openapi_client_udm.models.users_user.UsersUser(
-            dn=f"uid={fake.user_name()},{user.position}",
-            object_type="users/user",
-            properties={fake.first_name(): fake.last_name()},
-            uri=fake.url(),
-            uuid=fake.uuid4(),
-        )
-        test_data = [
-            (None, None),
-            (False, False),
-            (True, True),
-            (an_int, an_int),
-            (a_float, a_float),
-            (a_date, a_date.strftime("%Y-%m-%d")),
-            (a_dict, a_dict_exp),
-            (a_list, a_list_exp),
-            (a_tuple, list(a_tuple)),
-            (a_udm_obj, a_udm_obj.uri),
-            (an_api_obj, an_api_obj.to_dict()),
-            (Path("/tmp"), ValueError),
-        ]
-        random.shuffle(test_data)
-        ids = [
-            f"bool ({val_in})" if type(val_in) is bool else type(val_in).__name__
-            for val_in, val_out in test_data
-        ]
-        metafunc.parametrize("serialize_obj_data", test_data, ids=ids)
+    if "serialize_obj_data" not in metafunc.fixturenames:
+        return
+    an_int = fake.pyint()
+    a_float = fake.pyfloat()
+    a_date: datetime.date = fake.date_object()
+    a_dict: Dict[str, Any] = fake.pydict(10, True, int, str, bool, float)
+    a_dict["dict"] = {"nested_bool": fake.pybool(), "nested_int": fake.pyint()}
+    a_dict["date"] = fake.date_object()
+    a_dict["none"] = None
+    a_dict["_ignoreme"] = fake.pyint()
+    a_dict_exp = copy.deepcopy(a_dict)
+    a_dict_exp["date"] = a_dict_exp["date"].strftime("%Y-%m-%d")
+    del a_dict_exp["_ignoreme"]
+    a_list: List[Any] = fake.pylist(10, True, int, str, bool, float)
+    a_list.insert(2, fake.date_object())
+    a_list_exp = copy.deepcopy(a_list)
+    a_list_exp[2] = a_list_exp[2].strftime("%Y-%m-%d")
+    a_tuple = fake.pytuple(10, True, int, str, bool, float)
+    user = UserFactory()
+    user.position = user.position.format(base_dn="dc=base,dc=dn")
+    user.dn = f"uid={user.props.username},{user.position}"
+    a_udm_obj = UsersUserUdmObjectFactory(user_data=user)
+    an_api_obj = openapi_client_udm.models.users_user.UsersUser(
+        dn=f"uid={fake.user_name()},{user.position}",
+        object_type="users/user",
+        properties={fake.first_name(): fake.last_name()},
+        uri=fake.url(),
+        uuid=fake.uuid4(),
+    )
+    test_data = [
+        (None, None),
+        (False, False),
+        (True, True),
+        (an_int, an_int),
+        (a_float, a_float),
+        (a_date, a_date.strftime("%Y-%m-%d")),
+        (a_dict, a_dict_exp),
+        (a_list, a_list_exp),
+        (a_tuple, list(a_tuple)),
+        (a_udm_obj, a_udm_obj.uri),
+        (an_api_obj, an_api_obj.to_dict()),
+        (Path("/tmp"), ValueError),
+    ]
+    random.shuffle(test_data)
+    ids = [
+        f"bool ({val_in})" if type(val_in) is bool else type(val_in).__name__
+        for val_in, val_out in test_data
+    ]
+    metafunc.parametrize("serialize_obj_data", test_data, ids=ids)
 
 
 @pytest.fixture
-def new_cn(base_dn, http_headers_read, http_headers_write, udm_kwargs):
+def new_cn(base_dn, http_headers_read, http_headers_write, schedule_delete_object_via_http, udm_kwargs):
     """Create a new container"""
-    created_cn_dns = []
     auth = (udm_kwargs["username"], udm_kwargs["password"])
     url = f"{udm_kwargs['url']}/container/cn/"
     if udm_kwargs.get("verify_ssl", True):
         verify_ssl = udm_kwargs.get("ssl_ca_cert", False)  # pragma: no cover
     else:
         verify_ssl = False
 
-    def _func(**cn_kwargs) -> Tuple[str, str, Dict[str, str]]:
+    def _new_cn(**cn_kwargs) -> Tuple[str, str, Dict[str, str]]:
         data = {"properties": {"name": fake.city()}, "position": base_dn}
         data.update(cn_kwargs)
         resp = requests.post(url, headers=http_headers_write, json=data, auth=auth, verify=verify_ssl)
         print(resp.reason)
         try:
             print(resp.json())
         except (AttributeError, ValueError):  # pragma: no cover
             print(resp.text)
-        assert resp.status_code in (201, 204)
+        assert resp.status_code in {201, 204}
         obj_url = resp.headers["Location"]
         dn = unquote(obj_url.rsplit("/", 1)[-1])
-        created_cn_dns.append(dn)
+        schedule_delete_object_via_http("container/cn", dn)
         assert dn == f"cn={data['properties']['name']},{data['position']}"
         return dn, obj_url, data
 
-    yield _func
-
-    for dn in created_cn_dns:
-        url = f"{url}{dn}"
-        resp = requests.delete(url, headers=http_headers_read, auth=auth, verify=verify_ssl)
-        assert resp.status_code in (204, 404)
+    return _new_cn
```

### Comparing `udm-rest-client-1.2.1/tests/test_base.py` & `udm-rest-client-1.2.2/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     dn, url, user = user_created_via_http()
 
     async with UDM(**udm_kwargs) as udm:
         mod = udm.get("users/user")
         obj = await mod.get(dn)
     keys_exp = [k for k in obj.props.__dict__.keys() if not k.startswith("_")]
     assert set(keys_exp) == set(obj.props.keys())  # keys
-    assert set(keys_exp) == set(k for k in obj.props)  # iter
+    assert set(keys_exp) == set(obj.props)
     assert len(keys_exp) == len(obj.props)  # len
     for k in keys_exp:
         assert getattr(obj.props, k) in obj.props.values()  # values
         assert (k, getattr(obj.props, k)) in obj.props.items()  # items
 
 
 @pytest.mark.asyncio
```

### Comparing `udm-rest-client-1.2.1/tests/test_base_http.py` & `udm-rest-client-1.2.2/tests/test_base_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         assert obj.dn is None
         assert obj.uri == ""
         with pytest.raises(NotYetSavedError):
             await obj.reload()
 
 
 @pytest.mark.asyncio
-async def test_create_user(fake_user, udm_kwargs):
+async def test_create_user(fake_user, schedule_delete_object_via_http, udm_kwargs):
     user_data = fake_user()
     async with UDM(**udm_kwargs) as udm:
         mod = udm.get("users/user")
         obj = await mod.new()
         obj.policies = user_data.policies
         obj.superordinate = user_data.superordinate
         obj.position = user_data.position
@@ -371,27 +371,26 @@
         for k, v in attr.asdict(user_data.props).items():
             setattr(obj.props, k, v)
         assert obj.dn is None
         assert obj.uri == ""
 
         res = await obj.save()
 
+        schedule_delete_object_via_http("users/user", res.dn)
         assert res is obj
         assert obj.dn not in (None, "")
         assert obj.uri not in (None, "")
 
         obj_new = await mod.get(obj.dn)
         assert obj_new.dn == obj.dn
         assert obj_new.position == obj.position
         assert obj_new.props.firstname == obj.props.firstname
         assert obj_new.props.lastname == obj.props.lastname
         assert obj_new.props.birthday == obj.props.birthday
 
-        await obj.delete()
-
 
 @pytest.mark.asyncio
 async def test_creating_obj_with_bad_property_value(faker, fake_user, udm_kwargs):
     user_data = fake_user()
     async with UDM(**udm_kwargs) as udm:
         mod = udm.get("users/user")
         obj = await mod.new()
@@ -448,25 +447,25 @@
             if k == "password":
                 v = None
             assert getattr(obj_new.props, k) == v
 
 
 @pytest.mark.asyncio
 async def test_add_attribute_of_previously_deactivated_option(
-    faker, http_headers_write, test_server_configuration, udm_kwargs
+    faker, http_headers_write, schedule_delete_object_via_http, test_server_configuration, udm_kwargs
 ):
-    # TODO: ensure deletion of share using a fixture
     async with UDM(**udm_kwargs) as udm:
         mod = udm.get("shares/share")
         obj = await mod.new()
         obj.options = {"samba": True}
         obj.props.name = faker.unique.user_name()
         obj.props.host = "file.example.com"
         obj.props.path = f"/home/share{faker.first_name()}"
         await obj.save()
+        schedule_delete_object_via_http("shares/share", obj.dn)
 
         obj_new = await mod.get(obj.dn)
         assert obj_new.props.name == obj.props.name
         if obj.options.get("nfs") is True:
             # handle http://forge.univention.org/bugzilla/show_bug.cgi?id=50974
             print("NFS enabled by default :/")
             import requests
@@ -484,46 +483,47 @@
                 json={"options": {"samba": True, "nfs": False}},
             )
             print(resp.reason)
             try:
                 print(resp.json())
             except (AttributeError, ValueError):  # pragma: no cover
                 print(resp.text)
-            assert resp.status_code in (201, 204)
+            assert resp.status_code in {201, 204}
             obj_new = await mod.get(obj.dn)
         assert obj_new.options.get("samba") is True
         assert obj_new.options.get("nfs") is False
         assert not hasattr(obj_new.props, "root_squash")
 
         obj_new.options["nfs"] = True
         obj_new.props.root_squash = True
         await obj_new.save()
 
         obj_new2 = await mod.get(obj_new.dn)
         assert obj_new2.options.get("nfs") is True
         assert hasattr(obj_new2.props, "root_squash")
         assert obj.props.root_squash is True
 
-        await obj_new2.delete()
-
 
 @pytest.mark.asyncio
-async def test_move_user_no_props_changed(new_cn, user_created_via_http, udm_kwargs):
+async def test_move_user_no_props_changed(
+    new_cn, schedule_delete_object_via_http, user_created_via_http, udm_kwargs
+):
     old_user_dn, old_user_url, old_user_data = user_created_via_http()
     cn_dn, cn_obj_url, cn_data = new_cn()
     async with UDM(**udm_kwargs) as udm:
         mod = udm.get("users/user")
         obj = await mod.get(old_user_dn)
         assert obj.dn == old_user_dn
         assert obj.uri == old_user_url
         assert obj.position == old_user_data["position"]
         assert obj.props.firstname == old_user_data["properties"]["firstname"]
 
         obj.position = cn_dn
         res = await obj.save()
+        schedule_delete_object_via_http("users/user", obj.dn)
         assert res is obj
         assert obj.dn != old_user_dn
         assert obj.dn == f"uid={obj.props.username},{cn_dn}"
         assert obj.uri != old_user_url
 
         assert unquote(obj.uri) == old_user_url.rsplit("/", 1)[0] + "/" + obj.dn
 
@@ -531,15 +531,17 @@
         assert obj_new.dn == obj.dn
         assert obj_new.uri == obj.uri
         assert obj_new.position == cn_dn
         assert obj.props.firstname == old_user_data["properties"]["firstname"]
 
 
 @pytest.mark.asyncio
-async def test_move_and_modify_user(faker, new_cn, user_created_via_http, udm_kwargs):
+async def test_move_and_modify_user(
+    faker, new_cn, schedule_delete_object_via_http, user_created_via_http, udm_kwargs
+):
     old_user_dn, old_user_url, old_user_data = user_created_via_http()
     cn_dn, cn_obj_url, cn_data = new_cn()
     async with UDM(**udm_kwargs) as udm:
         mod = udm.get("users/user")
         obj = await mod.get(old_user_dn)
         assert obj.dn == old_user_dn
         assert obj.uri == old_user_url
@@ -548,14 +550,15 @@
 
         obj.position = cn_dn
         new_description = faker.text(max_nb_chars=50)
         obj.props.description = new_description
         new_lastname = faker.unique.last_name()
         obj.props.lastname = new_lastname
         res = await obj.save()
+        schedule_delete_object_via_http("users/user", obj.dn)
         assert res is obj
         assert obj.dn != old_user_dn
         assert obj.dn == f"uid={obj.props.username},{cn_dn}"
         assert obj.uri != old_user_url
 
         assert unquote(obj.uri) == old_user_url.rsplit("/", 1)[0] + "/" + obj.dn
 
@@ -565,15 +568,17 @@
         assert obj_new.position == cn_dn
         assert obj.props.firstname == old_user_data["properties"]["firstname"]
         assert obj.props.lastname == new_lastname
         assert obj.props.description == new_description
 
 
 @pytest.mark.asyncio
-async def test_move_multiple_objects(base_dn, new_cn, user_created_via_http, udm_kwargs):
+async def test_move_multiple_objects(
+    base_dn, new_cn, schedule_delete_object_via_http, user_created_via_http, udm_kwargs
+):
     top_cn_dn, top_cn_obj_url, top_cn_data = new_cn()
     old_cn_dn, old_cn_obj_url, old_cn_data = new_cn(position=top_cn_dn)
     cn_name = old_cn_data["properties"]["name"]
     users = {num: user_created_via_http(position=old_cn_dn) for num in range(20)}
     with patch.object(base_http, "MIN_FOLLOW_REDIRECT_SLEEP_TIME", 3.0):
         async with UDM(**udm_kwargs) as udm:
             mod_user = udm.get("users/user")
@@ -582,18 +587,23 @@
                 assert user_obj.position == old_cn_dn
             mod_cn = udm.get("container/cn")
             cn_obj = await mod_cn.get(old_cn_dn)
             assert cn_obj.dn == old_cn_dn
             assert cn_obj.dn != base_dn
             cn_obj.position = base_dn
             await cn_obj.save()
+            schedule_delete_object_via_http("container/cn", cn_obj.dn)
             assert cn_obj.dn == f"cn={cn_name},{base_dn}"
             for dn, url, data in users.values():
                 query = dn.split(",", 1)[0]
+                objs = []  # schedule deletion for all objects before testing them
                 async for obj in mod_user.search(query):
+                    schedule_delete_object_via_http("users/user", obj.dn)
+                    objs.append(obj)
+                for obj in objs:
                     assert old_cn_dn not in obj.dn
                     assert obj.position == cn_obj.dn
                     assert obj.dn == f"uid={data['properties']['username']},{cn_obj.dn}"
 
 
 @pytest.mark.asyncio
 async def test_move_error(base_dn, random_name, user_created_via_http, udm_kwargs):
```

### Comparing `udm-rest-client-1.2.1/tests/test_test.py` & `udm-rest-client-1.2.2/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/tests/test_udm.py` & `udm-rest-client-1.2.2/tests/test_udm.py`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/udm_rest_client/__init__.py` & `udm-rest-client-1.2.2/udm_rest_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for Python UDM REST Client."""
 __author__ = """Daniel Troeder"""
 __email__ = "troeder@univention.de"
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 from .base_http import UdmModule, UdmObject
 from .exceptions import (
     APICommunicationError,
     ConfigurationError,
     CreateError,
     DeletedError,
```

### Comparing `udm-rest-client-1.2.1/udm_rest_client/base.py` & `udm-rest-client-1.2.2/udm_rest_client/base.py`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/udm_rest_client/base_http.py` & `udm-rest-client-1.2.2/udm_rest_client/base_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -594,18 +594,15 @@
             memo[id_self]._api_obj = self._api_obj.__class__(**obj_dump)
             # _udm_module must be set in the current session
         return memo[id_self]
 
     def __eq__(self, other: "UdmObject") -> bool:
         if not super().__eq__(other):
             return False
-        for attr in ("uri", "uuid"):
-            if getattr(self, attr) != getattr(other, attr):
-                return False
-        return True
+        return all(getattr(self, attr) == getattr(other, attr) for attr in ("uri", "uuid"))
 
     async def reload(self, language: str = None) -> "UdmObject":
         """
         Refresh object from LDAP.
 
         :param str language: Language used in the "Accept-Language" header for this
             request (optional)
@@ -620,15 +617,17 @@
             )
         if not self.dn or not self._api_obj:
             raise NotYetSavedError(module_name=self._udm_module.name)
         api_obj = await self._udm_module._get_api_object(self.dn, language=language)
         self._api_obj = api_obj
         if api_obj.object_type != self._udm_module.name:
             # probably only happens with users/self
-            self._udm_module = UdmModule(api_obj.object_type, self._udm_module.session)
+            self._udm_module = UdmModule(  # pragma: no cover
+                api_obj.object_type, self._udm_module.session
+            )
         await self._copy_from_api_instance_obj(api_obj)
         return self
 
     async def save(self, language: str = None) -> "UdmObject":  # noqa: C901
         """
         Save object to LDAP (via UDM REST API).
 
@@ -679,30 +678,28 @@
                     attribute_map: Dict[str, str] = self._api_obj.policies.attribute_map
                     old_policies = {
                         attribute_map[k]: v for k, v in self._api_obj.policies.to_dict().items()
                     }
                 else:
                     old_policies = self._api_obj.policies
                 # v is Dict[str, List[str]], compare as Dict[str, Set[str]]
-                if {diff_k: set(diff_v) for diff_k, diff_v in v.items()} == {
+                if {diff_k: set(diff_v) for diff_k, diff_v in v.items()} != {
                     new_k: set(new_v) for new_k, new_v in old_policies.items()
                 }:
-                    continue
-                diff_dict[k] = v
+                    diff_dict[k] = v
             elif k == "position" and v:
                 diff_dict[k] = v  # always set position
-            else:
-                if v != old_obj[k]:
-                    diff_dict[k] = v
+            elif v != old_obj[k]:
+                diff_dict[k] = v
         for k in ("options", "policies", "props", "superordinate"):
             if not diff_dict.get(k):
                 diff_dict.pop(k, None)
         if self.dn:
             # 'move' as a separate step before 'modify'
-            if self.dn and self._api_obj.position and self._api_obj.position != self.position:
+            if self._api_obj.position and self._api_obj.position != self.position:
                 # TODO: handle base64 encoded DNs
                 logger.info("Moving {!r} to new position {!r}.".format(self, self.position))
                 api_obj = await self._move(self.position, language=language)
                 await self._copy_from_api_instance_obj(api_obj)
                 logger.info("Finished moving object, new DN: %r", self.dn)
 
             # position is always set, ignore if unchanged
@@ -720,37 +717,36 @@
         kwargs = {
             "udm_module_name": self._udm_module.name,
             "operation": operation,
             "dn": dn,
             "api_model_obj": diff_dict,
         }
         _, status, header = await self._udm_module.session.call_openapi(language=language, **kwargs)
-        if status in (201, 204):
-            new_module_name, new_dn = _uri2module_dn(header["Location"])
-            if new_module_name != self._udm_module.name:  # pragma: no cover
-                if not (self._udm_module.name == "users/self" and new_module_name == "users/user"):
-                    logger.warning(
-                        "UDM REST API redirected to an object of a different "
-                        "module. %r of %r returned the 'Location' %r which was"
-                        " decoded to module %r and DN %r. Arguments were: %r ",
-                        operation,
-                        self._udm_module.name,
-                        header["Location"],
-                        new_module_name,
-                        new_dn,
-                        kwargs,
-                    )
-                self._udm_module = UdmModule(new_module_name, self._udm_module.session)
-            self.dn = new_dn
-        else:  # pragma: no cover
+        if status not in {201, 204}:
             # TODO: wrap in {Create/Modify/Move/Delete}Exception
-            raise ApiException(
+            raise ApiException(  # pragma: no cover
                 f"UDM REST API returned status {status}, header: {header!r} "
                 f"for {operation!r} of {self._udm_module.name!r} {dn!r}."
             )
+        new_module_name, new_dn = _uri2module_dn(header["Location"])
+        if new_module_name != self._udm_module.name:  # pragma: no cover
+            if self._udm_module.name != "users/self" or new_module_name != "users/user":
+                logger.warning(
+                    "UDM REST API redirected to an object of a different "
+                    "module. %r of %r returned the 'Location' %r which was"
+                    " decoded to module %r and DN %r. Arguments were: %r ",
+                    operation,
+                    self._udm_module.name,
+                    header["Location"],
+                    new_module_name,
+                    new_dn,
+                    kwargs,
+                )
+            self._udm_module = UdmModule(new_module_name, self._udm_module.session)
+        self.dn = new_dn
         self._fresh = False
         await self.reload(language=language)
         return self
 
     async def delete(self, language=None) -> None:
         """
         Remove the object from the LDAP database.
@@ -820,15 +816,15 @@
             elif (
                 isinstance(v, list)  # flake8 doesn't like the way black splits this:
                 and v  # noqa: 503
                 and all(isinstance(x, str) for x in v)  # noqa: 503
                 and all(dn_regex.match(x) for x in v)  # noqa: 503
             ):
                 v = [DnPropertyEncoder(k, dn, self._udm_module.session).decode() for dn in v]
-            elif isinstance(v, MutableSequence) or isinstance(v, MutableMapping):
+            elif isinstance(v, (MutableSequence, MutableMapping)):
                 # changing obj.property.x should not change obj._api_obj.property.x
                 v = copy.deepcopy(v)
             setattr(self.props, k, v)
         superordinate: str = getattr(api_model_obj, "superordinate", None)
         if (
             superordinate
             and isinstance(superordinate, str)  # noqa: 503
@@ -877,15 +873,15 @@
                 self._udm_module.name,
                 "modify",
                 dn=self.dn,
                 api_model_obj=self._api_obj,
                 language=language,
             )
         except APICommunicationError as exc:
-            raise MoveError(f"Error moving {self} to {position!r}: [{exc.status}] {exc.reason}")
+            raise MoveError(f"Error moving {self} to {position!r}: [{exc.status}] {exc.reason}") from exc
         if status not in (200, 201, 202):  # pragma: no cover
             raise MoveError(
                 f"Error moving {self} to {position!r}:\nHTTP [{status}]\n"
                 f"response: {new_api_obj!r}\nheader: {header!r}'",
                 dn=self.dn,
                 module_name=self._udm_module.name,
             )
@@ -1149,15 +1145,15 @@
         :param str dn: the DN of the object to load, '' to load a template object
         :param str language: Language used in the "Accept-Language" header for this
             request (optional)
         :return: a ApiModel object
         :rtype: ApiModel
         :raises udm_rest_client.NoObject: if no object is found for `dn`
         """
-        if dn == "":
+        if not dn:
             operation = "new"
             dn = None
         else:
             operation = "get"
         api_model_obj, status, header = await self.session.call_openapi(
             self.name, operation, dn=dn, language=language
         )
@@ -1185,15 +1181,15 @@
                 raise ValueError("Either 'dn' or 'api_obj' must be not be None.")
             api_obj = await self._get_api_object(dn, language=language)
 
         if api_obj.object_type == self.name:
             udm_module = self
         else:
             # probably only happens with users/self
-            udm_module = UdmModule(api_obj.object_type, self.session)
+            udm_module = UdmModule(api_obj.object_type, self.session)  # pragma: no cover
 
         return await self._udm_object_class._new_from_api_object(api_obj=api_obj, udm_module=udm_module)
 
 
 class DnPropertyEncoder:
     """
     Given a DN, return a string object with the DN and an additional member
```

### Comparing `udm-rest-client-1.2.1/udm_rest_client/exceptions.py` & `udm-rest-client-1.2.2/udm_rest_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/udm_rest_client/udm.py` & `udm-rest-client-1.2.2/udm_rest_client/udm.py`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/udm_rest_client.egg-info/PKG-INFO` & `udm-rest-client-1.2.2/udm_rest_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udm-rest-client
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python library to interact with the Univention UDM REST API. Implements the simple Python UDM API.
 Home-page: https://github.com/univention/python-udm-rest-api-client
 Author: Daniel Troeder
 Author-email: troeder@univention.de
 License: GNU Affero General Public License v3
 Keywords: Univention UCS UDM REST
 Classifier: Development Status :: 4 - Beta
@@ -199,14 +199,20 @@
     :target: https://github.com/univention/python-udm-rest-api-client/actions?query=workflow%3A%22Integration+tests%22
 
 
 =======
 History
 =======
 
+1.2.2 (2023-06-05)
+-------------------
+
+* Fix ``update_openapi_client`` crashing with newer versions of the Python Docker client and ``requests`` (Issue #10).
+* Testing fixes (Issues #5 and #9)
+
 1.2.1 (2023-02-15)
 -------------------
 
 * Update OpenAPI client library generator (openapitools/openapi-generator-cli) to version ``5.4.0`` to support Python 3.11..
 
 1.1.1 (2023-01-16)
 -------------------
```

### Comparing `udm-rest-client-1.2.1/udm_rest_client.egg-info/SOURCES.txt` & `udm-rest-client-1.2.2/udm_rest_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `udm-rest-client-1.2.1/update_openapi_client` & `udm-rest-client-1.2.2/update_openapi_client`

 * *Files identical despite different names*

