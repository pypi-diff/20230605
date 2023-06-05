# Comparing `tmp/ngdataenginterface-0.1.0.tar.gz` & `tmp/ngdataenginterface-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataenginterface-0.1.0.tar", max compression
+gzip compressed data, was "ngdataenginterface-0.1.1.tar", max compression
```

## Comparing `ngdataenginterface-0.1.0.tar` & `ngdataenginterface-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2934 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/README.md
--rw-r--r--   0        0        0      348 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/__init__.py
--rw-r--r--   0        0        0     3808 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/analytical.py
--rw-r--r--   0        0        0     3392 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/aws_interface.py
--rw-r--r--   0        0        0     2704 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/process.py
--rw-r--r--   0        0        0      517 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/__init__.py
--rw-r--r--   0        0        0     2124 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/create_analytical_tables.py
--rw-r--r--   0        0        0     1516 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/landing_to_raw.py
--rw-r--r--   0        0        0     2015 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/raw_to_trusted.py
--rw-r--r--   0        0        0     1508 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/trusted_to_analytics.py
--rw-r--r--   0        0        0     1836 2023-05-29 19:16:09.083496 ngdataenginterface-0.1.0/ngdataenginterface/spark_manager.py
--rw-r--r--   0        0        0    13389 2023-05-29 19:16:09.083496 ngdataenginterface-0.1.0/ngdataenginterface/table.py
--rw-r--r--   0        0        0     2780 2023-05-29 19:16:09.083496 ngdataenginterface-0.1.0/ngdataenginterface/utils.py
--rw-r--r--   0        0        0      395 2023-05-29 19:16:09.083496 ngdataenginterface-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2934 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/README.md
+-rw-r--r--   0        0        0      348 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/__init__.py
+-rw-r--r--   0        0        0     3778 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/analytical.py
+-rw-r--r--   0        0        0     3392 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/aws_interface.py
+-rw-r--r--   0        0        0     2704 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/process.py
+-rw-r--r--   0        0        0      517 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/__init__.py
+-rw-r--r--   0        0        0     2124 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/create_analytical_tables.py
+-rw-r--r--   0        0        0     1516 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/landing_to_raw.py
+-rw-r--r--   0        0        0     2015 2023-06-05 14:05:20.107219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/raw_to_trusted.py
+-rw-r--r--   0        0        0     1508 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/ngdataenginterface/scripts/trusted_to_analytics.py
+-rw-r--r--   0        0        0     1836 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/ngdataenginterface/spark_manager.py
+-rw-r--r--   0        0        0    13379 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/ngdataenginterface/table.py
+-rw-r--r--   0        0        0     2720 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/ngdataenginterface/utils.py
+-rw-r--r--   0        0        0      395 2023-06-05 14:05:20.108219 ngdataenginterface-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.1.1/PKG-INFO
```

### Comparing `ngdataenginterface-0.1.0/README.md` & `ngdataenginterface-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/analytical.py` & `ngdataenginterface-0.1.1/ngdataenginterface/analytical.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     """
     Class Analytical encapsulates the functionality for table read and write operations,
     along with the execution of a specified aggregation function.
     """
 
     def __init__(
         self,
-        read_params: Dict[str, dict],
-        write_params: Dict[str, dict],
+        read_params: dict,
+        write_params: dict,
         aggregation_function,
         date: datetime,
         aws_interface: AWSInterface,
         spark_manager: SparkManager,
         overwrite: bool = False,
         log_level: int = logging.INFO,
     ) -> None:
@@ -34,28 +34,28 @@
             write_params, date, aws_interface, spark_manager, overwrite
         )
         self.aggregation_function = aggregation_function
         self.meta = {
             "spark": spark_manager.spark,
             "aws_interface": aws_interface,
             "date": date,
-            "session_name": "analytical_tables"
+            "session_name": "analytical_tables",
         }
         # Set up logging
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)  # Set the log level
 
     @staticmethod
     def _init_tables(
-        params: Dict[str, dict],
+        params: dict,
         date: datetime,
         aws_interface: AWSInterface,
         spark_manager: SparkManager,
         overwrite: bool,
-    ) -> Dict[str, Table]:
+    ) -> dict:
         """
         Initialize the tables for data read and write operations.
         """
         tables = {}
         print("\nparams: ", params, "\n")
         for table_name, table_params in params.items():
             path = PathParams.from_dict(table_params)
@@ -71,15 +71,16 @@
     def prepare_inputs(self) -> None:
         """
         Prepare the inputs by reading data from the tables.
         """
         self.logger.info("Preparing inputs...")
         try:
             self.inputs = {
-                table_name: {"df": table.read_table()} for table_name, table in self.read.items()
+                table_name: {"df": table.read_table()}
+                for table_name, table in self.read.items()
             }
             self.logger.debug(f"Prepared inputs: {self.inputs}")
         except Exception as e:
             self.logger.error(f"Failed to prepare inputs: {e}")
             raise e
         self.logger.info("Inputs prepared successfully.")
 
@@ -88,15 +89,15 @@
         Run the aggregation function and write the output back to the tables.
         """
         self.logger.info("Running the aggregation function...")
         try:
             self.prepare_inputs()
             # print("\ninputs: ", self.inputs, "\n")
             # print("\nagg:", self.aggregation_function, "\n")
-            self.output = self.aggregation_function(inputs=self.inputs, meta = self.meta)
+            self.output = self.aggregation_function(inputs=self.inputs, meta=self.meta)
             self.logger.debug(f"Aggregation output: {self.output}")
             # print("\noutput2: ", self.output, "\n")
             for table_name, table in self.write.items():
                 # print("\noutput: ", self.output[table_name], "\n")
                 table.write_table(self.output[table_name])
             self.logger.info(
                 "Successfully ran the aggregation function and wrote output to tables."
```

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/aws_interface.py` & `ngdataenginterface-0.1.1/ngdataenginterface/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/process.py` & `ngdataenginterface-0.1.1/ngdataenginterface/process.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/scripts/__init__.py` & `ngdataenginterface-0.1.1/ngdataenginterface/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/scripts/create_analytical_tables.py` & `ngdataenginterface-0.1.1/ngdataenginterface/scripts/create_analytical_tables.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/scripts/landing_to_raw.py` & `ngdataenginterface-0.1.1/ngdataenginterface/scripts/landing_to_raw.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/scripts/raw_to_trusted.py` & `ngdataenginterface-0.1.1/ngdataenginterface/scripts/raw_to_trusted.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/scripts/trusted_to_analytics.py` & `ngdataenginterface-0.1.1/ngdataenginterface/scripts/trusted_to_analytics.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/spark_manager.py` & `ngdataenginterface-0.1.1/ngdataenginterface/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/table.py` & `ngdataenginterface-0.1.1/ngdataenginterface/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         assert "file_type" in data.keys(), "Couldn`t find `file_type` in path input"
         if self.schema_path is not None:
             assert (
                 "schema_path" in data.keys()
             ), "Couldn't find `schema_path` in path input"
 
     @classmethod
-    def from_dict(cls, data: dict[str, str]):
+    def from_dict(cls, data: dict):
         instance = cls(
             env=data["env"],
             bucket_name=data["bucket_name"],
             object_path=data["object_path"],
             partition=data["partition"],
             file_type=data["file_type"],
             schema_path=data.get("schema_path"),
```

### Comparing `ngdataenginterface-0.1.0/ngdataenginterface/utils.py` & `ngdataenginterface-0.1.1/ngdataenginterface/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,28 +55,25 @@
 def handle_execution_date_args(dt: str):
     match = re.search(r"(?<=\.).+?(?=\:)", dt)
     if match:
         dt = dt.replace(f".{match.group()[:-3]}", "")
     return datetime.strptime("".join(dt.rsplit(":", 1)), "%Y-%m-%dT%H:%M:%S%z")
 
 
-def handle_input_api(env,read_params, ng_prefix = "ngcash"):
-        layer = read_params["layer"]
-        object_path = read_params["object_path"]
-        partition = read_params["partition"]
-        file_type = read_params["file_type"]
-        input_dict =  {
-            "env": env,
-            "bucket_name": f"{ng_prefix}-datalake-{env}-{layer}",
-            "object_path": object_path,
-            "partition": partition,
-            "file_type": file_type,
-        }
-        if read_params.get('schema_path') is not None:
-            input_dict['schema_path'] = {
+def handle_input_api(env, read_params, ng_prefix="ngcash"):
+    layer = read_params["layer"]
+    object_path = read_params["object_path"]
+    partition = read_params["partition"]
+    file_type = read_params["file_type"]
+    input_dict = {
+        "env": env,
+        "bucket_name": f"{ng_prefix}-datalake-{env}-{layer}",
+        "object_path": object_path,
+        "partition": partition,
+        "file_type": file_type,
+    }
+    if read_params.get("schema_path") is not None:
+        input_dict["schema_path"] = {
             "bucket_name": f"{ng_prefix}-datalake-{env}-repository",
-            "object_path": read_params['schema_path']
+            "object_path": read_params["schema_path"],
         }
-        return input_dict
-
-
-
+    return input_dict
```

### Comparing `ngdataenginterface-0.1.0/PKG-INFO` & `ngdataenginterface-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngdataenginterface
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for facilitating the development of data engineering pipelines
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

