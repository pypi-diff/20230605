# Comparing `tmp/mock_data_generator-1.1.1.tar.gz` & `tmp/mock_data_generator-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.1.1.tar", max compression
+gzip compressed data, was "mock_data_generator-1.1.2.tar", max compression
```

## Comparing `mock_data_generator-1.1.1.tar` & `mock_data_generator-1.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.1.1/LICENSE
--rw-r--r--   0        0        0     2428 2023-06-05 11:16:03.210516 mock_data_generator-1.1.1/README.md
--rw-r--r--   0        0        0     1459 2023-06-05 10:54:16.975436 mock_data_generator-1.1.1/mock_data_generator/driver.py
--rw-r--r--   0        0        0      876 2023-06-05 11:00:16.827498 mock_data_generator-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 mock_data_generator-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2428 2023-06-05 11:16:03.210516 mock_data_generator-1.1.2/README.md
+-rw-r--r--   0        0        0     1411 2023-06-05 12:29:43.508935 mock_data_generator-1.1.2/mock_data_generator/driver.py
+-rw-r--r--   0        0        0      876 2023-06-05 12:31:42.475076 mock_data_generator-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 mock_data_generator-1.1.2/PKG-INFO
```

### Comparing `mock_data_generator-1.1.1/LICENSE` & `mock_data_generator-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.1.1/README.md` & `mock_data_generator-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.1.1/mock_data_generator/driver.py` & `mock_data_generator-1.1.2/mock_data_generator/driver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import argparse
-import os
-from generator.generate import runner
 from utils.constants import FILE_FORMATS
-from utils.fileutils import process
+from utils.fileutils import proceed
 
 
 def validate_file_format(value):
     if value.upper() not in FILE_FORMATS:
         raise argparse.ArgumentTypeError(
             f"Unsupported output file format {value} detected. Supported file formats are {FILE_FORMATS}"
         )
@@ -42,12 +40,12 @@
     parser.add_argument(
         "--number_of_rows",
         type=validate_num_rows,
         help="Number of mock records to be generated.",
         required=True,
     )
     args = parser.parse_args()
-    process(args=args)
+    proceed(args=args)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `mock_data_generator-1.1.1/pyproject.toml` & `mock_data_generator-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.1.1"
+version = "1.1.2"
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
-current_version = "1.1.1"
+current_version = "1.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.1.1/PKG-INFO` & `mock_data_generator-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.1.1
+Version: 1.1.2
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.11.3,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

