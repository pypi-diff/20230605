# Comparing `tmp/scdef-0.0.7.tar.gz` & `tmp/scdef-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdef-0.0.7.tar", max compression
+gzip compressed data, was "scdef-0.0.8.tar", max compression
```

## Comparing `scdef-0.0.7.tar` & `scdef-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      961 2023-06-05 12:00:48.737739 scdef-0.0.7/README.md
--rw-r--r--   0        0        0      641 2023-06-05 17:57:43.434967 scdef-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      141 2023-06-05 01:25:33.034355 scdef-0.0.7/scdef/__init__.py
--rw-r--r--   0        0        0    13737 2023-06-05 01:13:30.448424 scdef-0.0.7/scdef/bscdef.py
--rw-r--r--   0        0        0    10025 2023-06-05 01:13:30.354772 scdef-0.0.7/scdef/iscdef.py
--rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.7/scdef/main.py
--rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.7/scdef/models/integrated.py
--rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.7/scdef/models/joint.py
--rw-r--r--   0        0        0        0 2023-06-05 01:42:20.961736 scdef-0.0.7/scdef/models/single.py
--rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.7/scdef/models/spatial.py
--rw-r--r--   0        0        0    50586 2023-06-05 17:05:58.304170 scdef-0.0.7/scdef/scdef.py
--rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.7/scdef/util.py
--rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 scdef-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      961 2023-06-05 12:00:48.737739 scdef-0.0.8/README.md
+-rw-r--r--   0        0        0      660 2023-06-05 19:07:21.964725 scdef-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-06-05 01:25:33.034355 scdef-0.0.8/scdef/__init__.py
+-rw-r--r--   0        0        0    13737 2023-06-05 01:13:30.448424 scdef-0.0.8/scdef/bscdef.py
+-rw-r--r--   0        0        0    10025 2023-06-05 01:13:30.354772 scdef-0.0.8/scdef/iscdef.py
+-rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.8/scdef/main.py
+-rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.8/scdef/models/integrated.py
+-rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.8/scdef/models/joint.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:42:20.961736 scdef-0.0.8/scdef/models/single.py
+-rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.8/scdef/models/spatial.py
+-rw-r--r--   0        0        0    50586 2023-06-05 17:05:58.304170 scdef-0.0.8/scdef/scdef.py
+-rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.8/scdef/util.py
+-rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 scdef-0.0.8/PKG-INFO
```

### Comparing `scdef-0.0.7/README.md` & `scdef-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `scdef-0.0.7/pyproject.toml` & `scdef-0.0.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "scdef"
-version = "0.0.7"
+version = "0.0.8"
 description = "Extract hierarchical signatures of cell state from single-cell data."
 license = "MIT"
 authors = ["pedrofale <pedro.miguel.ferreira.pf@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/cbg-ethz/scdef"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 pandas = "^1.5.1"
 numpy = "^1.23.4"
-jax = "^0.3.20"
+jax = "^0.3.25"
+jaxlib = "^0.3.25"
 scanpy = "^1.9.3"
 anndata = "^0.9.1"
 click = "^8.0.1"
 tqdm = "^4.64.0"
 gseapy = "^1.0.4"
 graphviz = "^0.14.2"
 igraph = "^0.10.4"
```

### Comparing `scdef-0.0.7/scdef/bscdef.py` & `scdef-0.0.8/scdef/bscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.7/scdef/iscdef.py` & `scdef-0.0.8/scdef/iscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.7/scdef/main.py` & `scdef-0.0.8/scdef/main.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.7/scdef/models/integrated.py` & `scdef-0.0.8/scdef/models/integrated.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.7/scdef/models/joint.py` & `scdef-0.0.8/scdef/models/joint.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.7/scdef/models/spatial.py` & `scdef-0.0.8/scdef/models/spatial.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.7/scdef/scdef.py` & `scdef-0.0.8/scdef/scdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.7/scdef/util.py` & `scdef-0.0.8/scdef/util.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.7/PKG-INFO` & `scdef-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdef
-Version: 0.0.7
+Version: 0.0.8
 Summary: Extract hierarchical signatures of cell state from single-cell data.
 Home-page: https://github.com/cbg-ethz/scdef
 License: MIT
 Author: pedrofale
 Author-email: pedro.miguel.ferreira.pf@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anndata (>=0.9.1,<0.10.0)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: graphviz (>=0.14.2,<0.15.0)
 Requires-Dist: gseapy (>=1.0.4,<2.0.0)
 Requires-Dist: igraph (>=0.10.4,<0.11.0)
-Requires-Dist: jax (>=0.3.20,<0.4.0)
+Requires-Dist: jax (>=0.3.25,<0.4.0)
+Requires-Dist: jaxlib (>=0.3.25,<0.4.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: scanpy (>=1.9.3,<2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Project-URL: Repository, https://github.com/cbg-ethz/scdef
 Description-Content-Type: text/markdown
```

