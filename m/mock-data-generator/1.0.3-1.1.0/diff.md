# Comparing `tmp/mock_data_generator-1.0.3.tar.gz` & `tmp/mock_data_generator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.0.3.tar", max compression
+gzip compressed data, was "mock_data_generator-1.1.0.tar", max compression
```

## Comparing `mock_data_generator-1.0.3.tar` & `mock_data_generator-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.0.3/LICENSE
--rw-r--r--   0        0        0     1967 2023-06-05 08:17:54.096354 mock_data_generator-1.0.3/README.md
--rw-r--r--   0        0        0     1917 2023-06-05 07:25:11.243942 mock_data_generator-1.0.3/mock_data_generator/driver.py
--rw-r--r--   0        0        0      876 2023-06-05 08:33:45.011141 mock_data_generator-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 mock_data_generator-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2413 2023-06-05 10:41:52.897881 mock_data_generator-1.1.0/README.md
+-rw-r--r--   0        0        0     1459 2023-06-05 10:54:16.975436 mock_data_generator-1.1.0/mock_data_generator/driver.py
+-rw-r--r--   0        0        0      876 2023-06-05 10:52:27.210959 mock_data_generator-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 mock_data_generator-1.1.0/PKG-INFO
```

### Comparing `mock_data_generator-1.0.3/LICENSE` & `mock_data_generator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.0.3/README.md` & `mock_data_generator-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,27 @@
 This utility is using Python Faker module to randomly generate the test data.
 
 ## How to use
 Follow below step to run the utility. I am open to the suggestions, please add comment or mail me your suggestions.
 ### Inputs:
 Accepts below inputs as parameters.
 
-- --input_json_schema_path: Provide absolute path of the json schema file. The sample json schema file should look like below.
+- --input_json_schema_path: Provide absolute path of the json schemas. It accepts folder with json schema files or absolute path of a json schema file. The sample json schema file should be in the below format.
+```json
+{
+  "type": "<object/record,etc>",
+  "properties": {
+    "<column_name>": { "type": "<data_type>" },
+    "<column_name>": { "type": "<data_type>" }
+  }
+}
+
+The sample json schema file would look like below.
+
+```
 ```json
 {
   "type": "object",
   "properties": {
     "price": { "type": "number" },
     "name": { "type": "string" },
     "a": { "type": "integer" },
@@ -22,14 +34,15 @@
     "c": { "type": "boolean" },
     "dt": { "type": "date" },
     "ts": { "type": "timestamp" },
     "e": { "type": "boolean" }
   }
 }
 ```
+If error occured while processing a schema file, that file would be skipped. Mock data would get generated for rest of the valid schema files.
 
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
 - --output_path: Absolute path where the generated output should be stored
 
 - --number_of_rows: Number of output rows to be generated
```

### Comparing `mock_data_generator-1.0.3/mock_data_generator/driver.py` & `mock_data_generator-1.1.0/mock_data_generator/driver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import argparse
-
+import os
 from generator.generate import runner
-from schema_handler.schema_validator import validate_and_read_json_as_object
 from utils.constants import FILE_FORMATS
-from utils.fileutils import make_path_if_not_exists, read_json_file_as_string
+from utils.fileutils import process
 
 
 def validate_file_format(value):
     if value.upper() not in FILE_FORMATS:
         raise argparse.ArgumentTypeError(
             f"Unsupported output file format {value} detected. Supported file formats are {FILE_FORMATS}"
         )
     return value
 
+
 def validate_num_rows(value):
     num_rows = int(value)
     if num_rows <= 0:
-        raise argparse.ArgumentTypeError("%s is an invalid number of rows. The value for number of rows should be positive integer" % value)
+        raise argparse.ArgumentTypeError(
+            "%s is an invalid number of rows. The value for number of rows should be positive integer"
+            % value
+        )
     return num_rows
 
 
-
 def run():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--input_json_schema_path",
-        help="Input absolute path of the schema json. e.g:/user/test/data/json_schema/schema.json",
+        help="Input absolute path of the schema json, schema file or schema folder",
         required=True,
     )
     parser.add_argument(
         "--output_file_format",
         type=validate_file_format,
         help="Expected output file format(csv,json,xml,excel,parquet)",
         required=True,
@@ -40,22 +42,12 @@
     parser.add_argument(
         "--number_of_rows",
         type=validate_num_rows,
         help="Number of mock records to be generated.",
         required=True,
     )
     args = parser.parse_args()
-
-    make_path_if_not_exists(args.output_path)
-    json_schema_string = read_json_file_as_string(args.input_json_schema_path)
-    json_schema = validate_and_read_json_as_object(json_schema=json_schema_string)
-
-    runner(
-        json_schema=json_schema,
-        num_of_rows=int(args.number_of_rows),
-        output_path=args.output_path,
-        file_format=args.output_file_format,
-    )
+    process(args=args)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `mock_data_generator-1.0.3/pyproject.toml` & `mock_data_generator-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.0.3"
+version = "1.1.0"
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
-current_version = "1.0.3"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.0.3/PKG-INFO` & `mock_data_generator-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.0.3
+Version: 1.1.0
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.11.3,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,27 @@
 This utility is using Python Faker module to randomly generate the test data.
 
 ## How to use
 Follow below step to run the utility. I am open to the suggestions, please add comment or mail me your suggestions.
 ### Inputs:
 Accepts below inputs as parameters.
 
-- --input_json_schema_path: Provide absolute path of the json schema file. The sample json schema file should look like below.
+- --input_json_schema_path: Provide absolute path of the json schemas. It accepts folder with json schema files or absolute path of a json schema file. The sample json schema file should be in the below format.
+```json
+{
+  "type": "<object/record,etc>",
+  "properties": {
+    "<column_name>": { "type": "<data_type>" },
+    "<column_name>": { "type": "<data_type>" }
+  }
+}
+
+The sample json schema file would look like below.
+
+```
 ```json
 {
   "type": "object",
   "properties": {
     "price": { "type": "number" },
     "name": { "type": "string" },
     "a": { "type": "integer" },
@@ -40,14 +52,15 @@
     "c": { "type": "boolean" },
     "dt": { "type": "date" },
     "ts": { "type": "timestamp" },
     "e": { "type": "boolean" }
   }
 }
 ```
+If error occured while processing a schema file, that file would be skipped. Mock data would get generated for rest of the valid schema files.
 
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
 - --output_path: Absolute path where the generated output should be stored
 
 - --number_of_rows: Number of output rows to be generated
```

