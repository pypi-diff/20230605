# Comparing `tmp/scdeepinsight-0.1.8.tar.gz` & `tmp/scdeepinsight-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdeepinsight-0.1.8.tar", max compression
+gzip compressed data, was "scdeepinsight-0.1.9.tar", max compression
```

## Comparing `scdeepinsight-0.1.8.tar` & `scdeepinsight-0.1.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4090 2023-06-05 13:09:31.912356 scdeepinsight-0.1.8/README.md
--rw-r--r--   0        0        0      559 2023-06-05 15:15:49.155920 scdeepinsight-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4707 2023-06-05 15:14:58.450936 scdeepinsight-0.1.8/scdeepinsight.py
--rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 scdeepinsight-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     4090 2023-06-05 13:09:31.912356 scdeepinsight-0.1.9/README.md
+-rw-r--r--   0        0        0      559 2023-06-05 15:18:56.624164 scdeepinsight-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4707 2023-06-05 15:14:58.450936 scdeepinsight-0.1.9/scdeepinsight.py
+-rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 scdeepinsight-0.1.9/PKG-INFO
```

### Comparing `scdeepinsight-0.1.8/README.md` & `scdeepinsight-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `scdeepinsight-0.1.8/pyproject.toml` & `scdeepinsight-0.1.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scdeepinsight"
-version = "0.1.8"
+version = "0.1.9"
 description = "An automatic cell type annotation tool for PBMC scRNA-seq data."
 authors = ["Shangru JIA <jiashangru@g.ecc.u-tokyo.ac.jp>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `scdeepinsight-0.1.8/scdeepinsight.py` & `scdeepinsight-0.1.9/scdeepinsight.py`

 * *Files identical despite different names*

### Comparing `scdeepinsight-0.1.8/PKG-INFO` & `scdeepinsight-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdeepinsight
-Version: 0.1.8
+Version: 0.1.9
 Summary: An automatic cell type annotation tool for PBMC scRNA-seq data.
 License: MIT
 Author: Shangru JIA
 Author-email: jiashangru@g.ecc.u-tokyo.ac.jp
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

