# Comparing `tmp/ms_salesforce_api-0.0.38.tar.gz` & `tmp/ms_salesforce_api-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-0.0.38.tar", max compression
+gzip compressed data, was "ms_salesforce_api-0.0.39.tar", max compression
```

## Comparing `ms_salesforce_api-0.0.38.tar` & `ms_salesforce_api-0.0.39.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35149 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/LICENSE
--rw-r--r--   0        0        0     5635 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/README.md
--rw-r--r--   0        0        0        0 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2714 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2395 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3318 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15428 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     2082 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0     8063 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    12544 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0     5148 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    14583 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13715 2023-06-05 12:30:58.671883 ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0     1046 2023-06-05 12:30:58.675884 ms_salesforce_api-0.0.38/pyproject.toml
--rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 ms_salesforce_api-0.0.38/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/LICENSE
+-rw-r--r--   0        0        0     5635 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2714 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2395 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3318 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15428 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     2082 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0     8063 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    12544 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0     5148 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    14583 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13715 2023-06-05 12:33:28.654386 ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0     1056 2023-06-05 12:33:28.658386 ms_salesforce_api-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 ms_salesforce_api-0.0.39/PKG-INFO
```

### Comparing `ms_salesforce_api-0.0.38/LICENSE` & `ms_salesforce_api-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/README.md` & `ms_salesforce_api-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/constants.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-0.0.39/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.38/pyproject.toml` & `ms_salesforce_api-0.0.39/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "0.0.38"
+version = "0.0.39"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
@@ -30,12 +30,12 @@
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 79
 
-[[tool.poetry.source]]
-name = "syscorp-librarian"
-url = "https://europe-west1-python.pkg.dev/ms--tiber-com-lib--pro--8bd7/syscorp-librarian/simple/"
-default = false
-secondary = true
+# [[tool.poetry.source]]
+# name = "syscorp-librarian"
+# url = "https://europe-west1-python.pkg.dev/ms--tiber-com-lib--pro--8bd7/syscorp-librarian/simple/"
+# default = false
+# secondary = true
```

### Comparing `ms_salesforce_api-0.0.38/PKG-INFO` & `ms_salesforce_api-0.0.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 0.0.38
+Version: 0.0.39
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ms-salesforce-api Version: 0.0.38 Summary: Python
+Metadata-Version: 2.1 Name: ms-salesforce-api Version: 0.0.39 Summary: Python
 library used to extract data from Salesforce API and migrate it to Bigquery and
 Postgres. Author: Making Science Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: gc-google-services-api (>=1.2.7,<2.0.0) Requires-Dist: isort
 (>=5.12.0,<6.0.0) Requires-Dist: pre-commit (>=3.1.1,<4.0.0) Requires-Dist:
```

