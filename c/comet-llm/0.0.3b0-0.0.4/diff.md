# Comparing `tmp/comet_llm-0.0.3b0.tar.gz` & `tmp/comet_llm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_llm-0.0.3b0.tar", last modified: Mon Jun  5 17:22:57 2023, max compression
+gzip compressed data, was "comet_llm-0.0.4.tar", last modified: Mon Jun  5 17:33:47 2023, max compression
```

## Comparing `comet_llm-0.0.3b0.tar` & `comet_llm-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:22:57.561817 comet_llm-0.0.3b0/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-05 17:22:57.557817 comet_llm-0.0.3b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:22:57.561817 comet_llm-0.0.3b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:22:57.557817 comet_llm-0.0.3b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:22:57.557817 comet_llm-0.0.3b0/src/comet_llm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:22:57.557817 comet_llm-0.0.3b0/src/comet_llm/experiment_api/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/experiment_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/experiment_api/comet_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/experiment_api/experiment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/experiment_api/request_exception_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/experiment_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-05 17:22:46.000000 comet_llm-0.0.3b0/src/comet_llm/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:22:57.557817 comet_llm-0.0.3b0/src/comet_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-05 17:22:57.000000 comet_llm-0.0.3b0/src/comet_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 17:22:57.000000 comet_llm-0.0.3b0/src/comet_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:22:57.000000 comet_llm-0.0.3b0/src/comet_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:22:57.000000 comet_llm-0.0.3b0/src/comet_llm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 17:22:57.000000 comet_llm-0.0.3b0/src/comet_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 17:22:57.000000 comet_llm-0.0.3b0/src/comet_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.685722 comet_llm-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 17:33:47.685722 comet_llm-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 17:33:30.000000 comet_llm-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:33:47.685722 comet_llm-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-05 17:33:30.000000 comet_llm-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.681722 comet_llm-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.681722 comet_llm-0.0.4/src/comet_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.685722 comet_llm-0.0.4/src/comet_llm/experiment_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_api/comet_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_api/experiment_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_api/request_exception_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.685722 comet_llm-0.0.4/src/comet_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/top_level.txt
```

### Comparing `comet_llm-0.0.3b0/PKG-INFO` & `comet_llm-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_llm
-Version: 0.0.3b0
+Version: 0.0.4
 Summary: Comet logger for LLM
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_llm-0.0.3b0/setup.py` & `comet_llm-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,11 +50,11 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="comet_llm",
     name="comet_llm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.ml",
-    version="0.0.3b",
+    version="0.0.4",
     zip_safe=False,
     license="Proprietary",
 )
```

### Comparing `comet_llm-0.0.3b0/src/comet_llm/__init__.py` & `comet_llm-0.0.4/src/comet_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/api.py` & `comet_llm-0.0.4/src/comet_llm/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/config.py` & `comet_llm-0.0.4/src/comet_llm/config.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/convert.py` & `comet_llm-0.0.4/src/comet_llm/convert.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/datetimes.py` & `comet_llm-0.0.4/src/comet_llm/datetimes.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/exceptions.py` & `comet_llm-0.0.4/src/comet_llm/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/experiment_api/__init__.py` & `comet_llm-0.0.4/src/comet_llm/experiment_api/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/experiment_api/comet_api_client.py` & `comet_llm-0.0.4/src/comet_llm/experiment_api/comet_api_client.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/experiment_api/experiment_api.py` & `comet_llm-0.0.4/src/comet_llm/experiment_api/experiment_api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/experiment_api/request_exception_wrapper.py` & `comet_llm-0.0.4/src/comet_llm/experiment_api/request_exception_wrapper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/experiment_info.py` & `comet_llm-0.0.4/src/comet_llm/experiment_info.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/preprocess.py` & `comet_llm-0.0.4/src/comet_llm/preprocess.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm/types.py` & `comet_llm-0.0.4/src/comet_llm/types.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.3b0/src/comet_llm.egg-info/PKG-INFO` & `comet_llm-0.0.4/src/comet_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet-llm
-Version: 0.0.3b0
+Version: 0.0.4
 Summary: Comet logger for LLM
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_llm-0.0.3b0/src/comet_llm.egg-info/SOURCES.txt` & `comet_llm-0.0.4/src/comet_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

