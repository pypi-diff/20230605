# Comparing `tmp/aws_parquet-0.2.0.tar.gz` & `tmp/aws_parquet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_parquet-0.2.0.tar", max compression
+gzip compressed data, was "aws_parquet-0.3.0.tar", max compression
```

## Comparing `aws_parquet-0.2.0.tar` & `aws_parquet-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1176 2023-05-31 17:58:47.653187 aws_parquet-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      341 2023-05-31 17:25:56.938752 aws_parquet-0.2.0/src/aws_parquet/__init__.py
--rw-r--r--   0        0        0      315 2023-05-29 14:23:51.668665 aws_parquet-0.2.0/src/aws_parquet/_types.py
--rw-r--r--   0        0        0    15941 2023-05-31 17:53:36.675601 aws_parquet-0.2.0/src/aws_parquet/dataset.py
--rw-r--r--   0        0        0     2473 2023-05-29 14:23:51.710022 aws_parquet-0.2.0/src/aws_parquet/interface.py
--rw-r--r--   0        0        0        0 2023-05-27 12:44:13.338464 aws_parquet-0.2.0/src/aws_parquet/py.typed
--rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 aws_parquet-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-05 14:51:18.420536 aws_parquet-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     4985 2023-06-05 15:28:20.043606 aws_parquet-0.3.0/README.md
+-rw-r--r--   0        0        0     1836 2023-06-05 15:28:24.824272 aws_parquet-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-05-31 17:25:56.938752 aws_parquet-0.3.0/src/aws_parquet/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-29 14:23:51.668665 aws_parquet-0.3.0/src/aws_parquet/_types.py
+-rw-r--r--   0        0        0    15941 2023-05-31 17:53:36.675601 aws_parquet-0.3.0/src/aws_parquet/dataset.py
+-rw-r--r--   0        0        0     2473 2023-05-29 14:23:51.710022 aws_parquet-0.3.0/src/aws_parquet/interface.py
+-rw-r--r--   0        0        0        0 2023-05-27 12:44:13.338464 aws_parquet-0.3.0/src/aws_parquet/py.typed
+-rw-r--r--   0        0        0     5957 1970-01-01 00:00:00.000000 aws_parquet-0.3.0/PKG-INFO
```

### Comparing `aws_parquet-0.2.0/src/aws_parquet/dataset.py` & `aws_parquet-0.3.0/src/aws_parquet/dataset.py`

 * *Files identical despite different names*

### Comparing `aws_parquet-0.2.0/src/aws_parquet/interface.py` & `aws_parquet-0.3.0/src/aws_parquet/interface.py`

 * *Files identical despite different names*

