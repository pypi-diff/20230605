# Comparing `tmp/mock_data_generator-1.0.1.tar.gz` & `tmp/mock_data_generator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.0.1.tar", max compression
+gzip compressed data, was "mock_data_generator-1.0.2.tar", max compression
```

## Comparing `mock_data_generator-1.0.1.tar` & `mock_data_generator-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.0.1/LICENSE
--rw-r--r--   0        0        0     1913 2023-06-05 06:20:40.916685 mock_data_generator-1.0.1/README.md
--rw-r--r--   0        0        0     1917 2023-06-05 04:47:23.541208 mock_data_generator-1.0.1/mock_data_generator/driver.py
--rw-r--r--   0        0        0      876 2023-06-05 06:59:01.159267 mock_data_generator-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 mock_data_generator-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1967 2023-06-05 08:17:54.096354 mock_data_generator-1.0.2/README.md
+-rw-r--r--   0        0        0     1917 2023-06-05 07:25:11.243942 mock_data_generator-1.0.2/mock_data_generator/driver.py
+-rw-r--r--   0        0        0      876 2023-06-05 08:18:18.623516 mock_data_generator-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 mock_data_generator-1.0.2/PKG-INFO
```

### Comparing `mock_data_generator-1.0.1/LICENSE` & `mock_data_generator-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.0.1/README.md` & `mock_data_generator-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Data Generator - WIP
 
 ## Overview
-During every data project I came across a very basic problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those has certain limitations on number of columns and rows. 
-Solve this, I invested some time to build a utility to generate the mock data based on the supplied json schema. 
-This utility is using Python Faker module to randomly generate the test data. 
+During every data project I came across a very basic problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those has certain limitations on number of columns and rows.
+Solve this, I invested some time to build a utility to generate the mock data based on the supplied json schema.
+This utility is using Python Faker module to randomly generate the test data.
 
 ## How to use
 Follow below step to run the utility. I am open to the suggestions, please add comment or mail me your suggestions.
-### Inputs
-- input_json_schema_path: Provide absolute path of the json schema file. The sample json schema file should be 
+### Inputs:
+Accepts below inputs as parameters.
+
+- --input_json_schema_path: Provide absolute path of the json schema file. The sample json schema file should look like below.
 ```json
 {
   "type": "object",
   "properties": {
     "price": { "type": "number" },
     "name": { "type": "string" },
     "a": { "type": "integer" },
@@ -21,28 +23,27 @@
     "dt": { "type": "date" },
     "ts": { "type": "timestamp" },
     "e": { "type": "boolean" }
   }
 }
 ```
 
-- output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
+- --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
-- output_path: Absolute path where the generated output should be stored
+- --output_path: Absolute path where the generated output should be stored
 
-- number_of_rows: Number of output rows to be generated
+- --number_of_rows: Number of output rows to be generated
 
 - Supported data types are: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP"`
 
 
-### Pre-requisites 
+### Pre-requisites
 1. Python 3.11.3
 2. Poetry 1.3.2
 
 ### Steps to execute the utility
-1. `clone the repo`
-2. `cd mock_data_generator`
-3. `poetry install`
-4. Sample command: `poetry run generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` : If output path does not exists, it will create it and store the data inside the directory into data.csv file
+1. pip install mock-data-generator
+2. specify the parameters mentioned above
+4. Sample command: `generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` : If output path does not exists, it will create it and store the data inside the directory into data.csv file
 
 ### Licensing
-Distributed under the MIT license. See ``LICENSE`` for more information.
+Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `mock_data_generator-1.0.1/mock_data_generator/driver.py` & `mock_data_generator-1.0.2/mock_data_generator/driver.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.0.1/pyproject.toml` & `mock_data_generator-1.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.0.1"
+version = "1.0.2"
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
-current_version = "1.0.1"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.0.1/PKG-INFO` & `mock_data_generator-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.11.3,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,22 +15,24 @@
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Data Generator - WIP
 
 ## Overview
-During every data project I came across a very basic problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those has certain limitations on number of columns and rows. 
-Solve this, I invested some time to build a utility to generate the mock data based on the supplied json schema. 
-This utility is using Python Faker module to randomly generate the test data. 
+During every data project I came across a very basic problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those has certain limitations on number of columns and rows.
+Solve this, I invested some time to build a utility to generate the mock data based on the supplied json schema.
+This utility is using Python Faker module to randomly generate the test data.
 
 ## How to use
 Follow below step to run the utility. I am open to the suggestions, please add comment or mail me your suggestions.
-### Inputs
-- input_json_schema_path: Provide absolute path of the json schema file. The sample json schema file should be 
+### Inputs:
+Accepts below inputs as parameters.
+
+- --input_json_schema_path: Provide absolute path of the json schema file. The sample json schema file should look like below.
 ```json
 {
   "type": "object",
   "properties": {
     "price": { "type": "number" },
     "name": { "type": "string" },
     "a": { "type": "integer" },
@@ -39,28 +41,28 @@
     "dt": { "type": "date" },
     "ts": { "type": "timestamp" },
     "e": { "type": "boolean" }
   }
 }
 ```
 
-- output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
+- --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
-- output_path: Absolute path where the generated output should be stored
+- --output_path: Absolute path where the generated output should be stored
 
-- number_of_rows: Number of output rows to be generated
+- --number_of_rows: Number of output rows to be generated
 
 - Supported data types are: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP"`
 
 
-### Pre-requisites 
+### Pre-requisites
 1. Python 3.11.3
 2. Poetry 1.3.2
 
 ### Steps to execute the utility
-1. `clone the repo`
-2. `cd mock_data_generator`
-3. `poetry install`
-4. Sample command: `poetry run generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` : If output path does not exists, it will create it and store the data inside the directory into data.csv file
+1. pip install mock-data-generator
+2. specify the parameters mentioned above
+4. Sample command: `generate --input_json_schema_path=resources/schema.json --output_file_format=csv --output_path=output_data --number_of_rows=10 ` : If output path does not exists, it will create it and store the data inside the directory into data.csv file
 
 ### Licensing
 Distributed under the MIT license. See ``LICENSE`` for more information.
+
```

