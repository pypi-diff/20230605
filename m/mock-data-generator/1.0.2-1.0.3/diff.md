# Comparing `tmp/mock_data_generator-1.0.2.tar.gz` & `tmp/mock_data_generator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.0.2.tar", max compression
+gzip compressed data, was "mock_data_generator-1.0.3.tar", max compression
```

## Comparing `mock_data_generator-1.0.2.tar` & `mock_data_generator-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.0.2/LICENSE
--rw-r--r--   0        0        0     1967 2023-06-05 08:17:54.096354 mock_data_generator-1.0.2/README.md
--rw-r--r--   0        0        0     1917 2023-06-05 07:25:11.243942 mock_data_generator-1.0.2/mock_data_generator/driver.py
--rw-r--r--   0        0        0      876 2023-06-05 08:18:18.623516 mock_data_generator-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 mock_data_generator-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1967 2023-06-05 08:17:54.096354 mock_data_generator-1.0.3/README.md
+-rw-r--r--   0        0        0     1917 2023-06-05 07:25:11.243942 mock_data_generator-1.0.3/mock_data_generator/driver.py
+-rw-r--r--   0        0        0      876 2023-06-05 08:33:45.011141 mock_data_generator-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 mock_data_generator-1.0.3/PKG-INFO
```

### Comparing `mock_data_generator-1.0.2/LICENSE` & `mock_data_generator-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.0.2/README.md` & `mock_data_generator-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.0.2/mock_data_generator/driver.py` & `mock_data_generator-1.0.3/mock_data_generator/driver.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.0.2/pyproject.toml` & `mock_data_generator-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.0.2"
+version = "1.0.3"
 description = "Generate mock data using json schema supplied."
 authors = ["Rahul Auti <rahulsmtauti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 generate = "mock_data_generator.driver:run"
@@ -29,13 +29,13 @@
 ]
 
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.bumpver]
-current_version = "1.0.2"
+current_version = "1.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.0.2/PKG-INFO` & `mock_data_generator-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.11.3,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

