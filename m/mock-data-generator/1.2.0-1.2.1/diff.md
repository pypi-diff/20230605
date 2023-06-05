# Comparing `tmp/mock_data_generator-1.2.0.tar.gz` & `tmp/mock_data_generator-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.2.0.tar", max compression
+gzip compressed data, was "mock_data_generator-1.2.1.tar", max compression
```

## Comparing `mock_data_generator-1.2.0.tar` & `mock_data_generator-1.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.0/LICENSE
--rw-r--r--   0        0        0     2412 2023-06-05 13:02:32.422687 mock_data_generator-1.2.0/README.md
--rw-r--r--   0        0        0     1411 2023-06-05 12:29:43.508935 mock_data_generator-1.2.0/mock_data_generator/driver.py
--rw-r--r--   0        0        0      920 2023-06-05 13:03:33.607375 mock_data_generator-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3203 1970-01-01 00:00:00.000000 mock_data_generator-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2412 2023-06-05 13:02:32.422687 mock_data_generator-1.2.1/README.md
+-rw-r--r--   0        0        0     1411 2023-06-05 12:29:43.508935 mock_data_generator-1.2.1/mock_data_generator/driver.py
+-rw-r--r--   0        0        0      922 2023-06-05 13:13:15.915491 mock_data_generator-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 mock_data_generator-1.2.1/PKG-INFO
```

### Comparing `mock_data_generator-1.2.0/LICENSE` & `mock_data_generator-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.0/README.md` & `mock_data_generator-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.0/mock_data_generator/driver.py` & `mock_data_generator-1.2.1/mock_data_generator/driver.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.0/pyproject.toml` & `mock_data_generator-1.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.2.0"
+version = "1.2.1"
 description = "Generate mock data using json schema supplied."
 authors = ["Rahul Auti <rahulsmtauti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 generate = "mock_data_generator.driver:run"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "~3.11.3"
 faker = "^18.9.0"
 jsonschema = "^4.17.3"
 lxml = "^4.9.2"
 openpyxl = "^3.1.2"
 pandas = "^2.0.2"
 tqdm = "^4.65.0"
 pyarrow = "^12.0.0"
@@ -31,13 +31,13 @@
 ]
 
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.bumpver]
-current_version = "1.2.0"
+current_version = "1.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.2.0/PKG-INFO` & `mock_data_generator-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.2.0
+Version: 1.2.1
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11.3,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faker (>=18.9.0,<19.0.0)
 Requires-Dist: fastparquet (>=2023.4.0,<2024.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
```

