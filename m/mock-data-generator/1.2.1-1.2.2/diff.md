# Comparing `tmp/mock_data_generator-1.2.1.tar.gz` & `tmp/mock_data_generator-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.2.1.tar", max compression
+gzip compressed data, was "mock_data_generator-1.2.2.tar", max compression
```

## Comparing `mock_data_generator-1.2.1.tar` & `mock_data_generator-1.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.1/LICENSE
--rw-r--r--   0        0        0     2412 2023-06-05 13:02:32.422687 mock_data_generator-1.2.1/README.md
--rw-r--r--   0        0        0     1411 2023-06-05 12:29:43.508935 mock_data_generator-1.2.1/mock_data_generator/driver.py
--rw-r--r--   0        0        0      922 2023-06-05 13:13:15.915491 mock_data_generator-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 mock_data_generator-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2414 2023-06-05 13:18:09.875340 mock_data_generator-1.2.2/README.md
+-rw-r--r--   0        0        0     1411 2023-06-05 12:29:43.508935 mock_data_generator-1.2.2/mock_data_generator/driver.py
+-rw-r--r--   0        0        0      922 2023-06-05 13:37:14.890403 mock_data_generator-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 mock_data_generator-1.2.2/PKG-INFO
```

### Comparing `mock_data_generator-1.2.1/LICENSE` & `mock_data_generator-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.1/README.md` & `mock_data_generator-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
 - --output_path: Absolute path to store the generated mock dataset. If an output path does not exists, it will create it and store the data inside the directory into data file.
 
 - --number_of_rows: Number of output rows to be generated
 
 ### Pre-requisites
-1. Python ^3.10
+1. Python ~3.11.3
 
 
 ### Steps to execute the utility
 1. pip install mock-data-generator
 2. specify the parameters mentioned above
 4. Sample command: `generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` :
```

### Comparing `mock_data_generator-1.2.1/mock_data_generator/driver.py` & `mock_data_generator-1.2.2/mock_data_generator/driver.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.1/pyproject.toml` & `mock_data_generator-1.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.2.1"
+version = "1.2.2"
 description = "Generate mock data using json schema supplied."
 authors = ["Rahul Auti <rahulsmtauti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 generate = "mock_data_generator.driver:run"
@@ -31,13 +31,13 @@
 ]
 
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.bumpver]
-current_version = "1.2.1"
+current_version = "1.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.2.1/PKG-INFO` & `mock_data_generator-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.2.1
+Version: 1.2.2
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.11.3,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -66,15 +66,15 @@
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
 - --output_path: Absolute path to store the generated mock dataset. If an output path does not exists, it will create it and store the data inside the directory into data file.
 
 - --number_of_rows: Number of output rows to be generated
 
 ### Pre-requisites
-1. Python ^3.10
+1. Python ~3.11.3
 
 
 ### Steps to execute the utility
 1. pip install mock-data-generator
 2. specify the parameters mentioned above
 4. Sample command: `generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` :
```

