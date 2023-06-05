# Comparing `tmp/scdeepinsight-0.1.4.tar.gz` & `tmp/scdeepinsight-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdeepinsight-0.1.4.tar", max compression
+gzip compressed data, was "scdeepinsight-0.1.5.tar", max compression
```

## Comparing `scdeepinsight-0.1.4.tar` & `scdeepinsight-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0     4090 2023-06-05 13:09:31.912356 scdeepinsight-0.1.4/README.md
--rw-r--r--   0        0        0      558 2023-06-05 14:34:09.479233 scdeepinsight-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4706 2023-06-05 14:30:51.640224 scdeepinsight-0.1.4/scdeepinsight.py
--rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 scdeepinsight-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4090 2023-06-05 13:09:31.912356 scdeepinsight-0.1.5/README.md
+-rw-r--r--   0        0        0      559 2023-06-05 14:58:45.770465 scdeepinsight-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2620 2023-06-05 14:56:20.540392 scdeepinsight-0.1.5/scdeepinsight/Annotate.py
+-rw-r--r--   0        0        0     2196 2023-06-05 14:56:20.544392 scdeepinsight-0.1.5/scdeepinsight/ImageTransform.py
+-rw-r--r--   0        0        0       37 2023-06-05 14:57:18.331227 scdeepinsight-0.1.5/scdeepinsight/__init__.py
+-rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 scdeepinsight-0.1.5/PKG-INFO
```

### Comparing `scdeepinsight-0.1.4/README.md` & `scdeepinsight-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `scdeepinsight-0.1.4/pyproject.toml` & `scdeepinsight-0.1.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "scdeepinsight"
-version = "0.1.4"
+version = "0.1.5"
 description = "An automatic cell type annotation tool for PBMC scRNA-seq data."
 authors = ["Shangru JIA <jiashangru@g.ecc.u-tokyo.ac.jp>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 efficientnet-pytorch = "^0.7.1"
 pandas = "^2.0.2"
 numpy = "^1.24.3"
 anndata = "^0.9.1"
 pathlib = "^1.0.1"
 scikit-learn = "^1.1.1"
-torch = "^2.0.1"
+torch = "^1.11.0"
 torchvision = "^0.15.2"
 scanpy = "^1.9.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `scdeepinsight-0.1.4/PKG-INFO` & `scdeepinsight-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdeepinsight
-Version: 0.1.4
+Version: 0.1.5
 Summary: An automatic cell type annotation tool for PBMC scRNA-seq data.
 License: MIT
 Author: Shangru JIA
 Author-email: jiashangru@g.ecc.u-tokyo.ac.jp
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Requires-Dist: anndata (>=0.9.1,<0.10.0)
 Requires-Dist: efficientnet-pytorch (>=0.7.1,<0.8.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: scanpy (>=1.9.3,<2.0.0)
 Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: torch (>=1.11.0,<2.0.0)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Description-Content-Type: text/markdown
 
 # scDeepInsight
 - A supervised single-cell annotation method
 - The paper of scDeepInsight has been uploaded to bioRxiv: [scDeepInsight: a supervised cell-type identification method for scRNA-seq data with deep learning](https://www.biorxiv.org/content/10.1101/2023.03.09.531861v1)
```

