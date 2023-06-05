# Comparing `tmp/scrapy_s3logstorage-0.1.0.tar.gz` & `tmp/scrapy_s3logstorage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_s3logstorage-0.1.0.tar", max compression
+gzip compressed data, was "scrapy_s3logstorage-0.1.1.tar", max compression
```

## Comparing `scrapy_s3logstorage-0.1.0.tar` & `scrapy_s3logstorage-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.239068 scrapy_s3logstorage-0.1.0/LICENSE
--rw-r--r--   0        0        0     1659 2023-06-01 04:36:26.605823 scrapy_s3logstorage-0.1.0/README.md
--rw-r--r--   0        0        0      488 2023-06-01 04:13:34.464653 scrapy_s3logstorage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       36 2023-05-31 06:58:44.235695 scrapy_s3logstorage-0.1.0/scrapy_s3logstorage/__init__.py
--rw-r--r--   0        0        0     3354 2023-06-01 04:05:43.400431 scrapy_s3logstorage-0.1.0/scrapy_s3logstorage/extension.py
--rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 scrapy_s3logstorage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.239068 scrapy_s3logstorage-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1790 2023-06-05 10:55:17.651054 scrapy_s3logstorage-0.1.1/README.md
+-rw-r--r--   0        0        0      488 2023-06-05 10:54:30.402792 scrapy_s3logstorage-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-05 10:50:57.177543 scrapy_s3logstorage-0.1.1/scrapy_s3logstorage/__init__.py
+-rw-r--r--   0        0        0     3354 2023-06-05 10:50:57.177543 scrapy_s3logstorage-0.1.1/scrapy_s3logstorage/extension.py
+-rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 scrapy_s3logstorage-0.1.1/PKG-INFO
```

### Comparing `scrapy_s3logstorage-0.1.0/LICENSE` & `scrapy_s3logstorage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_s3logstorage-0.1.0/README.md` & `scrapy_s3logstorage-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 
 # Scrapy S3 Log Storage
 
+# **DEPRECATED**
+
+This package is deprecated. Please use [scrapy-logexport](https://pypi.org/project/scrapy-logexport/) instead.
+
+
 ## Description
 A Scrapy extension to upload log files to S3.
 
 If you're already exporting your feeds to S3 this extension uses many of the same settings. After adding this extension to your `EXTENSIONS` setting, just set the `LOG_FILE`, `S3_LOG_BUCKET` and an optional `S3_LOG_ACL`settings and you're good to go.
 
 ## Installation
 You can install scrapy-s3logstorage using pip:
```

### Comparing `scrapy_s3logstorage-0.1.0/scrapy_s3logstorage/extension.py` & `scrapy_s3logstorage-0.1.1/scrapy_s3logstorage/extension.py`

 * *Files identical despite different names*

### Comparing `scrapy_s3logstorage-0.1.0/PKG-INFO` & `scrapy_s3logstorage-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-s3logstorage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Upload scrapy logs to S3
 Author: Nicholas Mischke
 Author-email: nmischkework@proton.me
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,14 +15,19 @@
 Requires-Dist: environs (>=9.5.0,<10.0.0)
 Requires-Dist: scrapy (>=2.9.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 
 # Scrapy S3 Log Storage
 
+# **DEPRECATED**
+
+This package is deprecated. Please use [scrapy-logexport](https://pypi.org/project/scrapy-logexport/) instead.
+
+
 ## Description
 A Scrapy extension to upload log files to S3.
 
 If you're already exporting your feeds to S3 this extension uses many of the same settings. After adding this extension to your `EXTENSIONS` setting, just set the `LOG_FILE`, `S3_LOG_BUCKET` and an optional `S3_LOG_ACL`settings and you're good to go.
 
 ## Installation
 You can install scrapy-s3logstorage using pip:
```

