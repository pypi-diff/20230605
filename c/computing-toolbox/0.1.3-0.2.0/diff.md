# Comparing `tmp/computing-toolbox-0.1.3.tar.gz` & `tmp/computing-toolbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.1.3.tar", last modified: Sun Jun  4 07:55:26 2023, max compression
+gzip compressed data, was "computing-toolbox-0.2.0.tar", last modified: Mon Jun  5 06:06:28 2023, max compression
```

## Comparing `computing-toolbox-0.1.3.tar` & `computing-toolbox-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:26.928284 computing-toolbox-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-04 07:55:26.928284 computing-toolbox-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 07:55:26.928284 computing-toolbox-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:26.924284 computing-toolbox-0.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:26.924284 computing-toolbox-0.1.3/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:26.924284 computing-toolbox-0.1.3/src/computing_toolbox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/algorithms/split_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:26.924284 computing-toolbox-0.1.3/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:26.928284 computing-toolbox-0.1.3/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/utils/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-04 07:55:14.000000 computing-toolbox-0.1.3/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:55:26.924284 computing-toolbox-0.1.3/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-04 07:55:26.000000 computing-toolbox-0.1.3/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-04 07:55:26.000000 computing-toolbox-0.1.3/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 07:55:26.000000 computing-toolbox-0.1.3/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-04 07:55:26.000000 computing-toolbox-0.1.3/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-04 07:55:26.000000 computing-toolbox-0.1.3/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:28.391609 computing-toolbox-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-05 06:06:28.391609 computing-toolbox-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:06:28.391609 computing-toolbox-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:28.387609 computing-toolbox-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:28.387609 computing-toolbox-0.2.0/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:28.387609 computing-toolbox-0.2.0/src/computing_toolbox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/algorithms/split_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:28.387609 computing-toolbox-0.2.0/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:28.391609 computing-toolbox-0.2.0/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/utils/http_async_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/utils/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-05 06:06:08.000000 computing-toolbox-0.2.0/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:28.387609 computing-toolbox-0.2.0/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-05 06:06:28.000000 computing-toolbox-0.2.0/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-05 06:06:28.000000 computing-toolbox-0.2.0/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:06:28.000000 computing-toolbox-0.2.0/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-05 06:06:28.000000 computing-toolbox-0.2.0/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 06:06:28.000000 computing-toolbox-0.2.0/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.1.3/LICENSE` & `computing-toolbox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/PKG-INFO` & `computing-toolbox-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.1.3
+Version: 0.2.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.1.3/README.md` & `computing-toolbox-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/pyproject.toml` & `computing-toolbox-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "computing-toolbox"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
   { name="Pedro Mayorga", email="ppmayorga80@gmail.com" },
 ]
 description = "Computing Toolbox for daily computations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox/algorithms/split_range.py` & `computing-toolbox-0.2.0/src/computing_toolbox/algorithms/split_range.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.2.0/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.2.0/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.2.0/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-0.2.0/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-0.2.0/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-0.2.0/src/computing_toolbox/utils/http_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox/utils/jsonl.py` & `computing-toolbox-0.2.0/src/computing_toolbox/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.2.0/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.2.0/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.1.3
+Version: 0.2.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.1.3/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.2.0/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 src/computing_toolbox/algorithms/split_range.py
 src/computing_toolbox/gcp/__init__.py
 src/computing_toolbox/gcp/gs.py
 src/computing_toolbox/gcp/secret_manager.py
 src/computing_toolbox/utils/__init__.py
 src/computing_toolbox/utils/deep_get.py
 src/computing_toolbox/utils/es_long_search.py
+src/computing_toolbox/utils/http_async_request.py
 src/computing_toolbox/utils/http_fake_headers.py
 src/computing_toolbox/utils/http_request.py
 src/computing_toolbox/utils/jsonl.py
 src/computing_toolbox/utils/tictoc.py
```

