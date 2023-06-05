# Comparing `tmp/test_graphql_sdk-0.0.5.tar.gz` & `tmp/test_graphql_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_graphql_sdk-0.0.5.tar", last modified: Mon Jun  5 12:51:19 2023, max compression
+gzip compressed data, was "test_graphql_sdk-0.0.6.tar", last modified: Mon Jun  5 12:53:40 2023, max compression
```

## Comparing `test_graphql_sdk-0.0.5.tar` & `test_graphql_sdk-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,18 @@
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:51:19.399716 test_graphql_sdk-0.0.5/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 12:51:19.399763 test_graphql_sdk-0.0.5/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)     2692 2023-06-05 12:41:34.000000 test_graphql_sdk-0.0.5/README.md
--rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-05-31 07:35:04.000000 test_graphql_sdk-0.0.5/pyproject.toml
--rw-r--r--   0 sarvesh    (501) staff       (20)      659 2023-06-05 12:51:19.399948 test_graphql_sdk-0.0.5/setup.cfg
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:51:19.398831 test_graphql_sdk-0.0.5/src/
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:51:19.399613 test_graphql_sdk-0.0.5/src/test_graphql_sdk.egg-info/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 12:51:19.000000 test_graphql_sdk-0.0.5/src/test_graphql_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)      210 2023-06-05 12:51:19.000000 test_graphql_sdk-0.0.5/src/test_graphql_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 12:51:19.000000 test_graphql_sdk-0.0.5/src/test_graphql_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 12:51:19.000000 test_graphql_sdk-0.0.5/src/test_graphql_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:40.940061 test_graphql_sdk-0.0.6/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 12:53:40.940112 test_graphql_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2692 2023-06-05 12:41:34.000000 test_graphql_sdk-0.0.6/README.md
+-rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-05-31 07:35:04.000000 test_graphql_sdk-0.0.6/pyproject.toml
+-rw-r--r--   0 sarvesh    (501) staff       (20)      659 2023-06-05 12:53:40.940316 test_graphql_sdk-0.0.6/setup.cfg
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:40.938317 test_graphql_sdk-0.0.6/src/
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:40.939475 test_graphql_sdk-0.0.6/src/airstack/
+-rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:03.000000 test_graphql_sdk-0.0.6/src/airstack/__init__.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)      210 2023-06-01 15:14:21.000000 test_graphql_sdk-0.0.6/src/airstack/constant.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2288 2023-06-05 11:32:00.000000 test_graphql_sdk-0.0.6/src/airstack/example.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     4831 2023-06-05 12:53:30.000000 test_graphql_sdk-0.0.6/src/airstack/execute_query.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     5723 2023-06-02 16:57:40.000000 test_graphql_sdk-0.0.6/src/airstack/generic.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     1802 2023-06-05 12:51:08.000000 test_graphql_sdk-0.0.6/src/airstack/send_request.py
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:40.939939 test_graphql_sdk-0.0.6/src/test_graphql_sdk.egg-info/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 12:53:40.000000 test_graphql_sdk-0.0.6/src/test_graphql_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)      367 2023-06-05 12:53:40.000000 test_graphql_sdk-0.0.6/src/test_graphql_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 12:53:40.000000 test_graphql_sdk-0.0.6/src/test_graphql_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-05 12:53:40.000000 test_graphql_sdk-0.0.6/src/test_graphql_sdk.egg-info/top_level.txt
```

### Comparing `test_graphql_sdk-0.0.5/PKG-INFO` & `test_graphql_sdk-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_graphql_sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_graphql_sdk-0.0.5/README.md` & `test_graphql_sdk-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `test_graphql_sdk-0.0.5/setup.cfg` & `test_graphql_sdk-0.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = test_graphql_sdk
-version = 0.0.5
+version = 0.0.6
 author = Sarvesh
 author_email = sarveshsingh.03@gmail.com
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls =
```

### Comparing `test_graphql_sdk-0.0.5/src/test_graphql_sdk.egg-info/PKG-INFO` & `test_graphql_sdk-0.0.6/src/test_graphql_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-graphql-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

