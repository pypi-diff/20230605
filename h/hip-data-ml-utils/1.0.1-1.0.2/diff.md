# Comparing `tmp/hip_data_ml_utils-1.0.1.tar.gz` & `tmp/hip_data_ml_utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hip_data_ml_utils-1.0.1.tar", max compression
+gzip compressed data, was "hip_data_ml_utils-1.0.2.tar", max compression
```

## Comparing `hip_data_ml_utils-1.0.1.tar` & `hip_data_ml_utils-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1085 2023-06-05 06:59:18.756911 hip_data_ml_utils-1.0.1/LICENSE.txt
--rwxr-xr-x   0        0        0     1548 2023-06-05 06:59:18.756911 hip_data_ml_utils-1.0.1/README.md
--rwxr-xr-x   0        0        0        0 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/core/__init__.py
--rwxr-xr-x   0        0        0      642 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/core/config.py
--rw-r--r--   0        0        0     2158 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/core/databricks_utils.py
--rw-r--r--   0        0        0     3119 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/core/pyathena_utils.py
--rwxr-xr-x   0        0        0        0 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/mlflow_databricks/__init__.py
--rw-r--r--   0        0        0     7529 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py
--rw-r--r--   0        0        0     2578 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py
--rw-r--r--   0        0        0     6370 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py
--rw-r--r--   0        0        0     4470 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py
--rwxr-xr-x   0        0        0        0 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/pyathena_client/__init__.py
--rw-r--r--   0        0        0     4368 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/hip_data_ml_utils/pyathena_client/client.py
--rw-r--r--   0        0        0     1404 2023-06-05 06:59:18.764911 hip_data_ml_utils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3928 1970-01-01 00:00:00.000000 hip_data_ml_utils-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-05 08:19:39.988757 hip_data_ml_utils-1.0.2/LICENSE.txt
+-rwxr-xr-x   0        0        0     1548 2023-06-05 08:19:39.988757 hip_data_ml_utils-1.0.2/README.md
+-rwxr-xr-x   0        0        0        0 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/__init__.py
+-rwxr-xr-x   0        0        0      642 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/config.py
+-rw-r--r--   0        0        0     2158 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/databricks_utils.py
+-rw-r--r--   0        0        0     3119 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/pyathena_utils.py
+-rwxr-xr-x   0        0        0        0 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/__init__.py
+-rw-r--r--   0        0        0     7529 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py
+-rw-r--r--   0        0        0     2578 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py
+-rw-r--r--   0        0        0     6370 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py
+-rw-r--r--   0        0        0     4470 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py
+-rwxr-xr-x   0        0        0        0 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/pyathena_client/__init__.py
+-rw-r--r--   0        0        0     4368 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/pyathena_client/client.py
+-rw-r--r--   0        0        0     1404 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3928 1970-01-01 00:00:00.000000 hip_data_ml_utils-1.0.2/PKG-INFO
```

### Comparing `hip_data_ml_utils-1.0.1/LICENSE.txt` & `hip_data_ml_utils-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/README.md` & `hip_data_ml_utils-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/hip_data_ml_utils/core/config.py` & `hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/config.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/hip_data_ml_utils/core/databricks_utils.py` & `hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/hip_data_ml_utils/core/pyathena_utils.py` & `hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/pyathena_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py` & `hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py` & `hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py` & `hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py` & `hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/hip_data_ml_utils/pyathena_client/client.py` & `hip_data_ml_utils-1.0.2/hip_data_ml_utils/pyathena_client/client.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.1/pyproject.toml` & `hip_data_ml_utils-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hip_data_ml_utils"
-version = "1.0.1"
+version = "1.0.2"
 description = "Common Python tools and utilities for Hipages ML work"
 authors = ["Hipages Data Team <datascience@hipagesgroup.com.au>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
@@ -26,15 +26,15 @@
 joblib= "1.2.0"
 mccabe = "0.6.1"
 mock = "^4.0.3"
 moto = "^3.1.5"
 mypy-extensions = "0.4.3"
 nodeenv = "1.5.0"
 numpy = "1.21.5"
-packaging = "^21.3"
+packaging = "^23.1"
 pandas = "1.4.4"
 pluggy = "1.0.0"
 polling = "0.3.2"
 pre-commit = "2.10.0"
 py = "1.10.0"
 pyarrow = "8.0.0"
 pyathena = "^2.13.0"
```

### Comparing `hip_data_ml_utils-1.0.1/PKG-INFO` & `hip_data_ml_utils-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hip-data-ml-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Common Python tools and utilities for Hipages ML work
 License: MIT
 Author: Hipages Data Team
 Author-email: datascience@hipagesgroup.com.au
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
 Requires-Dist: mccabe (==0.6.1)
 Requires-Dist: mlflow-skinny (>=2.3.2,<3.0.0)
 Requires-Dist: mock (>=4.0.3,<5.0.0)
 Requires-Dist: moto (>=3.1.5,<4.0.0)
 Requires-Dist: mypy-extensions (==0.4.3)
 Requires-Dist: nodeenv (==1.5.0)
 Requires-Dist: numpy (==1.21.5)
-Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pandas (==1.4.4)
 Requires-Dist: platformdirs (==2.5.2)
 Requires-Dist: pluggy (==1.0.0)
 Requires-Dist: polling (==0.3.2)
 Requires-Dist: pre-commit (==2.10.0)
 Requires-Dist: py (==1.10.0)
 Requires-Dist: pyarrow (==8.0.0)
```

