# Comparing `tmp/scdeepinsight-0.1.6.tar.gz` & `tmp/scdeepinsight-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdeepinsight-0.1.6.tar", max compression
+gzip compressed data, was "scdeepinsight-0.1.7.tar", max compression
```

## Comparing `scdeepinsight-0.1.6.tar` & `scdeepinsight-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4090 2023-06-05 13:09:31.912356 scdeepinsight-0.1.6/README.md
--rw-r--r--   0        0        0      559 2023-06-05 15:05:10.408714 scdeepinsight-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2620 2023-06-05 14:56:20.540392 scdeepinsight-0.1.6/scdeepinsight/Annotate.py
--rw-r--r--   0        0        0     2196 2023-06-05 14:56:20.544392 scdeepinsight-0.1.6/scdeepinsight/ImageTransform.py
--rw-r--r--   0        0        0       37 2023-06-05 14:57:18.331227 scdeepinsight-0.1.6/scdeepinsight/__init__.py
--rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 scdeepinsight-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4090 2023-06-05 13:09:31.912356 scdeepinsight-0.1.7/README.md
+-rw-r--r--   0        0        0      559 2023-06-05 15:09:13.905838 scdeepinsight-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2620 2023-06-05 14:56:20.540392 scdeepinsight-0.1.7/scdeepinsight/Annotate.py
+-rw-r--r--   0        0        0     2196 2023-06-05 14:56:20.544392 scdeepinsight-0.1.7/scdeepinsight/ImageTransform.py
+-rw-r--r--   0        0        0       65 2023-06-05 15:09:18.082754 scdeepinsight-0.1.7/scdeepinsight/__init__.py
+-rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 scdeepinsight-0.1.7/PKG-INFO
```

### Comparing `scdeepinsight-0.1.6/README.md` & `scdeepinsight-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `scdeepinsight-0.1.6/pyproject.toml` & `scdeepinsight-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scdeepinsight"
-version = "0.1.6"
+version = "0.1.7"
 description = "An automatic cell type annotation tool for PBMC scRNA-seq data."
 authors = ["Shangru JIA <jiashangru@g.ecc.u-tokyo.ac.jp>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `scdeepinsight-0.1.6/scdeepinsight/Annotate.py` & `scdeepinsight-0.1.7/scdeepinsight/Annotate.py`

 * *Files identical despite different names*

### Comparing `scdeepinsight-0.1.6/scdeepinsight/ImageTransform.py` & `scdeepinsight-0.1.7/scdeepinsight/ImageTransform.py`

 * *Files identical despite different names*

### Comparing `scdeepinsight-0.1.6/PKG-INFO` & `scdeepinsight-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdeepinsight
-Version: 0.1.6
+Version: 0.1.7
 Summary: An automatic cell type annotation tool for PBMC scRNA-seq data.
 License: MIT
 Author: Shangru JIA
 Author-email: jiashangru@g.ecc.u-tokyo.ac.jp
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

