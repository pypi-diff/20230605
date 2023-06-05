# Comparing `tmp/ms_salesforce_api-0.0.40.tar.gz` & `tmp/ms_salesforce_api-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-0.0.40.tar", max compression
+gzip compressed data, was "ms_salesforce_api-0.0.41.tar", max compression
```

## Comparing `ms_salesforce_api-0.0.40.tar` & `ms_salesforce_api-0.0.41.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35149 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/LICENSE
--rw-r--r--   0        0        0     5635 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/README.md
--rw-r--r--   0        0        0        0 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2714 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2395 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3318 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15428 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     2082 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0     8063 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    12544 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0     5148 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    14583 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13715 2023-06-05 12:38:58.320893 ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0     1056 2023-06-05 12:38:58.324893 ms_salesforce_api-0.0.40/pyproject.toml
--rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 ms_salesforce_api-0.0.40/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/LICENSE
+-rw-r--r--   0        0        0     5635 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2714 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2395 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3318 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15428 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     2082 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0     8063 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-06-05 12:43:33.862832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:43:33.866832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    12544 2023-06-05 12:43:33.866832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0     5148 2023-06-05 12:43:33.866832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:43:33.866832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:43:33.866832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    14583 2023-06-05 12:43:33.866832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13715 2023-06-05 12:43:33.866832 ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0     1056 2023-06-05 12:43:33.866832 ms_salesforce_api-0.0.41/pyproject.toml
+-rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 ms_salesforce_api-0.0.41/PKG-INFO
```

### Comparing `ms_salesforce_api-0.0.40/LICENSE` & `ms_salesforce_api-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/README.md` & `ms_salesforce_api-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/constants.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-0.0.41/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-0.0.40/pyproject.toml` & `ms_salesforce_api-0.0.41/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "0.0.40"
+version = "0.0.41"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-0.0.40/PKG-INFO` & `ms_salesforce_api-0.0.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 0.0.40
+Version: 0.0.41
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
-Metadata-Version: 2.1 Name: ms-salesforce-api Version: 0.0.40 Summary: Python
+Metadata-Version: 2.1 Name: ms-salesforce-api Version: 0.0.41 Summary: Python
 library used to extract data from Salesforce API and migrate it to Bigquery and
 Postgres. Author: Making Science Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: gc-google-services-api (>=1.2.7,<2.0.0) Requires-Dist: isort
 (>=5.12.0,<6.0.0) Requires-Dist: pre-commit (>=3.1.1,<4.0.0) Requires-Dist:
```

