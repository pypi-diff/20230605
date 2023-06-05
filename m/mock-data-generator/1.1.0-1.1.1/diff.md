# Comparing `tmp/mock_data_generator-1.1.0.tar.gz` & `tmp/mock_data_generator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.1.0.tar", max compression
+gzip compressed data, was "mock_data_generator-1.1.1.tar", max compression
```

## Comparing `mock_data_generator-1.1.0.tar` & `mock_data_generator-1.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.1.0/LICENSE
--rw-r--r--   0        0        0     2413 2023-06-05 10:41:52.897881 mock_data_generator-1.1.0/README.md
--rw-r--r--   0        0        0     1459 2023-06-05 10:54:16.975436 mock_data_generator-1.1.0/mock_data_generator/driver.py
--rw-r--r--   0        0        0      876 2023-06-05 10:52:27.210959 mock_data_generator-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 mock_data_generator-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2428 2023-06-05 11:16:03.210516 mock_data_generator-1.1.1/README.md
+-rw-r--r--   0        0        0     1459 2023-06-05 10:54:16.975436 mock_data_generator-1.1.1/mock_data_generator/driver.py
+-rw-r--r--   0        0        0      876 2023-06-05 11:00:16.827498 mock_data_generator-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 mock_data_generator-1.1.1/PKG-INFO
```

### Comparing `mock_data_generator-1.1.0/LICENSE` & `mock_data_generator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.1.0/README.md` & `mock_data_generator-1.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # Data Generator - WIP
 
 ## Overview
-During every data project I came across a very basic problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those has certain limitations on number of columns and rows.
-Solve this, I invested some time to build a utility to generate the mock data based on the supplied json schema.
+During every data project I came across a very basic problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those have certain limitations on the number of columns and rows.
+To solve this, I’ve built a utility to generate the mock data based on the supplied json schema.
 This utility is using Python Faker module to randomly generate the test data.
 
 ## How to use
-Follow below step to run the utility. I am open to the suggestions, please add comment or mail me your suggestions.
-### Inputs:
-Accepts below inputs as parameters.
+Follow below steps to run the utility. I am open to your suggestions, please add comments or mail me your suggestions.
 
-- --input_json_schema_path: Provide absolute path of the json schemas. It accepts folder with json schema files or absolute path of a json schema file. The sample json schema file should be in the below format.
+### Inputs
+It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP"`
+#### Supported Input Parameters
+
+- --input_json_schema_path: Provide absolute path of the json schema file/folder. It accepts folders(that contains valid json schema files) or absolute path of a json schema file.
+
+> Json schema file format.
 ```json
 {
   "type": "<object/record,etc>",
   "properties": {
     "<column_name>": { "type": "<data_type>" },
     "<column_name>": { "type": "<data_type>" }
   }
 }
 
-The sample json schema file would look like below.
-
 ```
+> The sample json schema file would look like below.
 ```json
 {
   "type": "object",
   "properties": {
     "price": { "type": "number" },
     "name": { "type": "string" },
     "a": { "type": "integer" },
@@ -34,29 +37,26 @@
     "c": { "type": "boolean" },
     "dt": { "type": "date" },
     "ts": { "type": "timestamp" },
     "e": { "type": "boolean" }
   }
 }
 ```
-If error occured while processing a schema file, that file would be skipped. Mock data would get generated for rest of the valid schema files.
+The generator will skip the current json schema file if an error occurred. Mock data would get generated for rest of the valid schema files.
 
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
-- --output_path: Absolute path where the generated output should be stored
+- --output_path: Absolute path to store the generated mock dataset. If an output path does not exists, it will create it and store the data inside the directory into data file.
 
 - --number_of_rows: Number of output rows to be generated
 
-- Supported data types are: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP"`
-
-
 ### Pre-requisites
 1. Python 3.11.3
 2. Poetry 1.3.2
 
 ### Steps to execute the utility
 1. pip install mock-data-generator
 2. specify the parameters mentioned above
-4. Sample command: `generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` : If output path does not exists, it will create it and store the data inside the directory into data.csv file
+4. Sample command: `generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` :
 
 ### Licensing
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mock_data_generator-1.1.0/mock_data_generator/driver.py` & `mock_data_generator-1.1.1/mock_data_generator/driver.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.1.0/pyproject.toml` & `mock_data_generator-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.1.0"
+version = "1.1.1"
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
-current_version = "1.1.0"
+current_version = "1.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.1.0/PKG-INFO` & `mock_data_generator-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.11.3,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,36 +15,39 @@
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Data Generator - WIP
 
 ## Overview
-During every data project I came across a very basic problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those has certain limitations on number of columns and rows.
-Solve this, I invested some time to build a utility to generate the mock data based on the supplied json schema.
+During every data project I came across a very basic problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those have certain limitations on the number of columns and rows.
+To solve this, I’ve built a utility to generate the mock data based on the supplied json schema.
 This utility is using Python Faker module to randomly generate the test data.
 
 ## How to use
-Follow below step to run the utility. I am open to the suggestions, please add comment or mail me your suggestions.
-### Inputs:
-Accepts below inputs as parameters.
+Follow below steps to run the utility. I am open to your suggestions, please add comments or mail me your suggestions.
 
-- --input_json_schema_path: Provide absolute path of the json schemas. It accepts folder with json schema files or absolute path of a json schema file. The sample json schema file should be in the below format.
+### Inputs
+It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP"`
+#### Supported Input Parameters
+
+- --input_json_schema_path: Provide absolute path of the json schema file/folder. It accepts folders(that contains valid json schema files) or absolute path of a json schema file.
+
+> Json schema file format.
 ```json
 {
   "type": "<object/record,etc>",
   "properties": {
     "<column_name>": { "type": "<data_type>" },
     "<column_name>": { "type": "<data_type>" }
   }
 }
 
-The sample json schema file would look like below.
-
 ```
+> The sample json schema file would look like below.
 ```json
 {
   "type": "object",
   "properties": {
     "price": { "type": "number" },
     "name": { "type": "string" },
     "a": { "type": "integer" },
@@ -52,30 +55,27 @@
     "c": { "type": "boolean" },
     "dt": { "type": "date" },
     "ts": { "type": "timestamp" },
     "e": { "type": "boolean" }
   }
 }
 ```
-If error occured while processing a schema file, that file would be skipped. Mock data would get generated for rest of the valid schema files.
+The generator will skip the current json schema file if an error occurred. Mock data would get generated for rest of the valid schema files.
 
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
-- --output_path: Absolute path where the generated output should be stored
+- --output_path: Absolute path to store the generated mock dataset. If an output path does not exists, it will create it and store the data inside the directory into data file.
 
 - --number_of_rows: Number of output rows to be generated
 
-- Supported data types are: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP"`
-
-
 ### Pre-requisites
 1. Python 3.11.3
 2. Poetry 1.3.2
 
 ### Steps to execute the utility
 1. pip install mock-data-generator
 2. specify the parameters mentioned above
-4. Sample command: `generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` : If output path does not exists, it will create it and store the data inside the directory into data.csv file
+4. Sample command: `generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` :
 
 ### Licensing
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

