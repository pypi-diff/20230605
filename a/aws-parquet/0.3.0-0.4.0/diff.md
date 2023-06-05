# Comparing `tmp/aws_parquet-0.3.0.tar.gz` & `tmp/aws_parquet-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_parquet-0.3.0.tar", max compression
+gzip compressed data, was "aws_parquet-0.4.0.tar", max compression
```

## Comparing `aws_parquet-0.3.0.tar` & `aws_parquet-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-06-05 14:51:18.420536 aws_parquet-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     4985 2023-06-05 15:28:20.043606 aws_parquet-0.3.0/README.md
--rw-r--r--   0        0        0     1836 2023-06-05 15:28:24.824272 aws_parquet-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      341 2023-05-31 17:25:56.938752 aws_parquet-0.3.0/src/aws_parquet/__init__.py
--rw-r--r--   0        0        0      315 2023-05-29 14:23:51.668665 aws_parquet-0.3.0/src/aws_parquet/_types.py
--rw-r--r--   0        0        0    15941 2023-05-31 17:53:36.675601 aws_parquet-0.3.0/src/aws_parquet/dataset.py
--rw-r--r--   0        0        0     2473 2023-05-29 14:23:51.710022 aws_parquet-0.3.0/src/aws_parquet/interface.py
--rw-r--r--   0        0        0        0 2023-05-27 12:44:13.338464 aws_parquet-0.3.0/src/aws_parquet/py.typed
--rw-r--r--   0        0        0     5957 1970-01-01 00:00:00.000000 aws_parquet-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-05 14:51:18.420536 aws_parquet-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     4985 2023-06-05 15:28:20.043606 aws_parquet-0.4.0/README.md
+-rw-r--r--   0        0        0     1836 2023-06-05 21:24:28.387499 aws_parquet-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-05-31 17:25:56.938752 aws_parquet-0.4.0/src/aws_parquet/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-29 14:23:51.668665 aws_parquet-0.4.0/src/aws_parquet/_types.py
+-rw-r--r--   0        0        0    15941 2023-05-31 17:53:36.675601 aws_parquet-0.4.0/src/aws_parquet/dataset.py
+-rw-r--r--   0        0        0     2473 2023-05-29 14:23:51.710022 aws_parquet-0.4.0/src/aws_parquet/interface.py
+-rw-r--r--   0        0        0        0 2023-05-27 12:44:13.338464 aws_parquet-0.4.0/src/aws_parquet/py.typed
+-rw-r--r--   0        0        0     5957 1970-01-01 00:00:00.000000 aws_parquet-0.4.0/PKG-INFO
```

### Comparing `aws_parquet-0.3.0/LICENSE.txt` & `aws_parquet-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_parquet-0.3.0/README.md` & `aws_parquet-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_parquet-0.3.0/pyproject.toml` & `aws_parquet-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws_parquet"
-version = "0.3.0"
+version = "0.4.0"
 description = "An object-oriented interface for defining parquet datasets for AWS built on top of awswrangler and pandera"
 packages = [{ include = "aws_parquet", from = "src" }]
 authors = ["Marwan Sarieddine <sarieddine.marwan@gmail.com>"]
 license = "MIT"
 
 readme = "README.md"
 include = ["README.md", "LICENSE.txt", "src/aws_parquet/py.typed"]
```

### Comparing `aws_parquet-0.3.0/src/aws_parquet/dataset.py` & `aws_parquet-0.4.0/src/aws_parquet/dataset.py`

 * *Files identical despite different names*

### Comparing `aws_parquet-0.3.0/src/aws_parquet/interface.py` & `aws_parquet-0.4.0/src/aws_parquet/interface.py`

 * *Files identical despite different names*

### Comparing `aws_parquet-0.3.0/PKG-INFO` & `aws_parquet-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parquet
-Version: 0.3.0
+Version: 0.4.0
 Summary: An object-oriented interface for defining parquet datasets for AWS built on top of awswrangler and pandera
 Home-page: https://github.com/marwan116/aws-parquet/
 License: MIT
 Keywords: pandas,aws,parquet
 Author: Marwan Sarieddine
 Author-email: sarieddine.marwan@gmail.com
 Requires-Python: >=3.8,<=3.11
```

