# Comparing `tmp/test_graphql_sdk-0.0.2.tar.gz` & `tmp/test_graphql_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_graphql_sdk-0.0.2.tar", last modified: Mon Jun  5 11:38:26 2023, max compression
+gzip compressed data, was "test_graphql_sdk-0.0.3.tar", last modified: Mon Jun  5 12:22:42 2023, max compression
```

## Comparing `test_graphql_sdk-0.0.2.tar` & `test_graphql_sdk-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 11:38:26.930473 test_graphql_sdk-0.0.2/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3180 2023-06-05 11:38:26.930527 test_graphql_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)     2668 2023-06-05 11:24:49.000000 test_graphql_sdk-0.0.2/README.md
--rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-05-31 07:35:04.000000 test_graphql_sdk-0.0.2/pyproject.toml
--rw-r--r--   0 sarvesh    (501) staff       (20)      659 2023-06-05 11:38:26.930721 test_graphql_sdk-0.0.2/setup.cfg
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 11:38:26.929561 test_graphql_sdk-0.0.2/src/
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 11:38:26.930359 test_graphql_sdk-0.0.2/src/test_graphql_sdk.egg-info/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3180 2023-06-05 11:38:26.000000 test_graphql_sdk-0.0.2/src/test_graphql_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)      210 2023-06-05 11:38:26.000000 test_graphql_sdk-0.0.2/src/test_graphql_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 11:38:26.000000 test_graphql_sdk-0.0.2/src/test_graphql_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 11:38:26.000000 test_graphql_sdk-0.0.2/src/test_graphql_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:22:42.226733 test_graphql_sdk-0.0.3/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3180 2023-06-05 12:22:42.226783 test_graphql_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2668 2023-06-05 11:24:49.000000 test_graphql_sdk-0.0.3/README.md
+-rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-05-31 07:35:04.000000 test_graphql_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 sarvesh    (501) staff       (20)      659 2023-06-05 12:22:42.226974 test_graphql_sdk-0.0.3/setup.cfg
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:22:42.225774 test_graphql_sdk-0.0.3/src/
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:22:42.226630 test_graphql_sdk-0.0.3/src/test_graphql_sdk.egg-info/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3180 2023-06-05 12:22:42.000000 test_graphql_sdk-0.0.3/src/test_graphql_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)      210 2023-06-05 12:22:42.000000 test_graphql_sdk-0.0.3/src/test_graphql_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 12:22:42.000000 test_graphql_sdk-0.0.3/src/test_graphql_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 12:22:42.000000 test_graphql_sdk-0.0.3/src/test_graphql_sdk.egg-info/top_level.txt
```

### Comparing `test_graphql_sdk-0.0.2/PKG-INFO` & `test_graphql_sdk-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_graphql_sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_graphql_sdk-0.0.2/README.md` & `test_graphql_sdk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `test_graphql_sdk-0.0.2/setup.cfg` & `test_graphql_sdk-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = test_graphql_sdk
-version = 0.0.2
+version = 0.0.3
 author = Sarvesh
 author_email = sarveshsingh.03@gmail.com
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls =
```

### Comparing `test_graphql_sdk-0.0.2/src/test_graphql_sdk.egg-info/PKG-INFO` & `test_graphql_sdk-0.0.3/src/test_graphql_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-graphql-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

