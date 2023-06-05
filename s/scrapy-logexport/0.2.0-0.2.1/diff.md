# Comparing `tmp/scrapy_logexport-0.2.0.tar.gz` & `tmp/scrapy_logexport-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_logexport-0.2.0.tar", max compression
+gzip compressed data, was "scrapy_logexport-0.2.1.tar", max compression
```

## Comparing `scrapy_logexport-0.2.0.tar` & `scrapy_logexport-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.239068 scrapy_logexport-0.2.0/LICENSE
--rw-r--r--   0        0        0     4828 2023-06-05 10:32:39.055671 scrapy_logexport-0.2.0/README.md
--rw-r--r--   0        0        0      723 2023-06-05 10:37:36.308697 scrapy_logexport-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       36 2023-06-05 03:22:25.491386 scrapy_logexport-0.2.0/scrapy_logexport/__init__.py
--rw-r--r--   0        0        0     4672 2023-06-05 09:25:31.901599 scrapy_logexport-0.2.0/scrapy_logexport/extension.py
--rw-r--r--   0        0        0     5615 1970-01-01 00:00:00.000000 scrapy_logexport-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.239068 scrapy_logexport-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4293 2023-06-05 10:44:48.446982 scrapy_logexport-0.2.1/README.md
+-rw-r--r--   0        0        0      723 2023-06-05 10:45:46.403432 scrapy_logexport-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-05 03:22:25.491386 scrapy_logexport-0.2.1/scrapy_logexport/__init__.py
+-rw-r--r--   0        0        0     4672 2023-06-05 09:25:31.901599 scrapy_logexport-0.2.1/scrapy_logexport/extension.py
+-rw-r--r--   0        0        0     5080 1970-01-01 00:00:00.000000 scrapy_logexport-0.2.1/PKG-INFO
```

### Comparing `scrapy_logexport-0.2.0/LICENSE` & `scrapy_logexport-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_logexport-0.2.0/README.md` & `scrapy_logexport-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,29 @@
+Metadata-Version: 2.1
+Name: scrapy-logexport
+Version: 0.2.1
+Summary: Upload scrapy logs to cloud storage
+Home-page: https://github.com/nicholas-mischke/scrapy-logexport
+License: MIT
+Author: Nicholas Mischke
+Author-email: nmischkework@proton.me
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: botocore (>=1.29.143,<2.0.0)
+Project-URL: Repository, https://github.com/nicholas-mischke/scrapy-logexport
+Description-Content-Type: text/markdown
 
-# Scrapy Log Export
 
-[![Build Status](https://travis-ci.org/TeamHG-Memex/scrapy-logexporter.svg?branch=master)](https://travis-ci.org/TeamHG-Memex/scrapy-logexporter)
-[![codecov](https://codecov.io/gh/TeamHG-Memex/scrapy-logexporter/branch/master/graph/badge.svg)](https://codecov.io/gh/TeamHG-Memex/scrapy-logexporter)
-[![PyPI](https://img.shields.io/pypi/v/scrapy-logexporter.svg)](https://pypi.python.org/pypi/scrapy-logexporter)
-[![PyPI](https://img.shields.io/pypi/pyversions/scrapy-logexporter.svg)](https://pypi.python.org/pypi/scrapy-logexporter)
+# Scrapy Log Export
 
 ## Description
 A scrapy extension that allows for a LOG_URI setting, similar to a FEED_URI setting.
 The same FEED_STORAGE classes that are used in the feedexport extensions are used here.
 
 This extension is useful if you're running scrapy in a container and want to store your logs with a cloud service provider.
 
@@ -125,8 +140,8 @@
 GCS_PROJECT_ID # Overridden by LOG_STORAGE_GCS_PROJECT_ID
 FEED_EXPORT_GCS_ACL # Overridden by LOG_STORAGE_GCS_ACL
 
 # FTPFeedStorage settings
 FEED_STORAGE_FTP_ACTIVE # Overridden by LOG_STORAGE_FTP_ACTIVE
 
 FEED_TEMPDIR # Not used by logexport directly
-```
+```
```

### Comparing `scrapy_logexport-0.2.0/pyproject.toml` & `scrapy_logexport-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapy-logexport"
-version = "0.2.0"
+version = "0.2.1"
 description = "Upload scrapy logs to cloud storage"
 authors = ["Nicholas Mischke <nmischkework@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "scrapy_logexport"}]
 repository = "https://github.com/nicholas-mischke/scrapy-logexport"
```

### Comparing `scrapy_logexport-0.2.0/scrapy_logexport/extension.py` & `scrapy_logexport-0.2.1/scrapy_logexport/extension.py`

 * *Files identical despite different names*

