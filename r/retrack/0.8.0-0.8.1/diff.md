# Comparing `tmp/retrack-0.8.0.tar.gz` & `tmp/retrack-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrack-0.8.0.tar", max compression
+gzip compressed data, was "retrack-0.8.1.tar", max compression
```

## Comparing `retrack-0.8.0.tar` & `retrack-0.8.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-05-30 21:12:39.357809 retrack-0.8.0/LICENSE
--rw-r--r--   0        0        0     4914 2023-05-30 21:12:39.357809 retrack-0.8.0/README.md
--rw-r--r--   0        0        0     2117 2023-05-30 21:12:39.357809 retrack-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      366 2023-05-30 21:12:39.357809 retrack-0.8.0/retrack/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 21:12:39.357809 retrack-0.8.0/retrack/engine/__init__.py
--rw-r--r--   0        0        0     6986 2023-05-30 21:12:39.357809 retrack-0.8.0/retrack/engine/parser.py
--rw-r--r--   0        0        0     2907 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/engine/request_manager.py
--rw-r--r--   0        0        0     6850 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/engine/runner.py
--rw-r--r--   0        0        0     1614 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/__init__.py
--rw-r--r--   0        0        0     1800 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/base.py
--rw-r--r--   0        0        0     2574 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/check.py
--rw-r--r--   0        0        0     2234 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/constants.py
--rw-r--r--   0        0        0      873 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/contains.py
--rw-r--r--   0        0        0      951 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/datetime.py
--rw-r--r--   0        0        0      543 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/dynamic/__init__.py
--rw-r--r--   0        0        0      813 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/dynamic/base.py
--rw-r--r--   0        0        0     2607 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/dynamic/csv_table.py
--rw-r--r--   0        0        0      910 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/endswith.py
--rw-r--r--   0        0        0      941 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/endswithany.py
--rw-r--r--   0        0        0     1009 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/inputs.py
--rw-r--r--   0        0        0     1606 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/logic.py
--rw-r--r--   0        0        0     1056 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/match.py
--rw-r--r--   0        0        0     2623 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/math.py
--rw-r--r--   0        0        0     1085 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/outputs.py
--rw-r--r--   0        0        0      581 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/start.py
--rw-r--r--   0        0        0      926 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/startswith.py
--rw-r--r--   0        0        0      957 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/nodes/startswithany.py
--rw-r--r--   0        0        0        0 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/utils/__init__.py
--rw-r--r--   0        0        0      197 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/utils/constants.py
--rw-r--r--   0        0        0     1324 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/utils/registry.py
--rw-r--r--   0        0        0      154 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/utils/transformers.py
--rw-r--r--   0        0        0      594 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/validators/__init__.py
--rw-r--r--   0        0        0      267 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/validators/base.py
--rw-r--r--   0        0        0      407 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/validators/check_is_dag.py
--rw-r--r--   0        0        0     1296 2023-05-30 21:12:39.361809 retrack-0.8.0/retrack/validators/node_exists.py
--rw-r--r--   0        0        0     6021 1970-01-01 00:00:00.000000 retrack-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-05 17:17:53.309099 retrack-0.8.1/LICENSE
+-rw-r--r--   0        0        0     5095 2023-06-05 17:17:53.309099 retrack-0.8.1/README.md
+-rw-r--r--   0        0        0     2119 2023-06-05 17:17:53.309099 retrack-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/engine/__init__.py
+-rw-r--r--   0        0        0     6986 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/engine/parser.py
+-rw-r--r--   0        0        0     2907 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/engine/request_manager.py
+-rw-r--r--   0        0        0     6850 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/engine/runner.py
+-rw-r--r--   0        0        0     1614 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/nodes/__init__.py
+-rw-r--r--   0        0        0     1800 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/nodes/base.py
+-rw-r--r--   0        0        0     2574 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/nodes/check.py
+-rw-r--r--   0        0        0     2234 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/nodes/constants.py
+-rw-r--r--   0        0        0      873 2023-06-05 17:17:53.309099 retrack-0.8.1/retrack/nodes/contains.py
+-rw-r--r--   0        0        0      951 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/datetime.py
+-rw-r--r--   0        0        0      543 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/dynamic/__init__.py
+-rw-r--r--   0        0        0      813 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/dynamic/base.py
+-rw-r--r--   0        0        0     2607 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/dynamic/csv_table.py
+-rw-r--r--   0        0        0      910 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/endswith.py
+-rw-r--r--   0        0        0      941 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/endswithany.py
+-rw-r--r--   0        0        0     1009 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/inputs.py
+-rw-r--r--   0        0        0     1606 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/logic.py
+-rw-r--r--   0        0        0     1056 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/match.py
+-rw-r--r--   0        0        0     2623 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/math.py
+-rw-r--r--   0        0        0     1085 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/outputs.py
+-rw-r--r--   0        0        0      581 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/start.py
+-rw-r--r--   0        0        0      926 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/startswith.py
+-rw-r--r--   0        0        0      957 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/nodes/startswithany.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/utils/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/utils/constants.py
+-rw-r--r--   0        0        0     1324 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/utils/registry.py
+-rw-r--r--   0        0        0      154 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/utils/transformers.py
+-rw-r--r--   0        0        0      594 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/validators/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/validators/base.py
+-rw-r--r--   0        0        0      407 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/validators/check_is_dag.py
+-rw-r--r--   0        0        0     1296 2023-06-05 17:17:53.313099 retrack-0.8.1/retrack/validators/node_exists.py
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 retrack-0.8.1/PKG-INFO
```

### Comparing `retrack-0.8.0/LICENSE` & `retrack-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/README.md` & `retrack-0.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,24 @@
 ```
 
 ## Usage
 
 ```python
 import retrack
 
+runner = retrack.Runner.from_json("your-rule.json")
+
+response = runner.execute(input_data)
+```
+
+Or, if you want to create the parser and runner manually:
+
+```python
+import retrack
+
 # Parse the rule/model
 parser = retrack.Parser(rule)
 
 # Create a runner
 runner = retrack.Runner(parser)
 
 # Run the rule/model passing the data
```

### Comparing `retrack-0.8.0/pyproject.toml` & `retrack-0.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "retrack"
-version = "0.8.0"
+version = "0.8.1"
 description = "A business rules engine"
 authors = ["Gabriel Guarisa <gabrielguarisa@gmail.com>", "Nathalia Trotte <nathaliatrotte@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gabrielguarisa/retrack"
 homepage = "https://github.com/gabrielguarisa/retrack"
 keywords = ["rules", "models", "business", "node", "graph"]
 
 [tool.poetry.dependencies]
 python = "^3.7.16"
 pandas = [
   { version = "1.2.0", python = "<3.8" },
-  { version = "^1.5.2", python = ">=3.8" }
+  { version = "^1.2.0", python = ">=3.8" }
 ]
 numpy = [
   { version = "1.19.5", python = "<3.8" },
-  { version = "^1.24.0", python = ">=3.8" }
+  { version = "^1.19.5", python = ">=3.8" }
 ]
 pydantic = "^1.10.4"
 networkx = [
   { version = "2.6.3", python = "<3.8" },
-  { version = "^3.0", python = ">=3.8" }
+  { version = "^2.6.3", python = ">=3.8" }
 ]
 
 [tool.poetry.dev-dependencies]
 pytest = [
   { version = "6.2.2", python = "<3.8" },
   { version = "^6.2.4", python = ">=3.8" }
 ]
```

### Comparing `retrack-0.8.0/retrack/engine/parser.py` & `retrack-0.8.1/retrack/engine/parser.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/engine/request_manager.py` & `retrack-0.8.1/retrack/engine/request_manager.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/engine/runner.py` & `retrack-0.8.1/retrack/engine/runner.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/__init__.py` & `retrack-0.8.1/retrack/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/base.py` & `retrack-0.8.1/retrack/nodes/base.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/check.py` & `retrack-0.8.1/retrack/nodes/check.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/constants.py` & `retrack-0.8.1/retrack/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/contains.py` & `retrack-0.8.1/retrack/nodes/contains.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/datetime.py` & `retrack-0.8.1/retrack/nodes/datetime.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/dynamic/__init__.py` & `retrack-0.8.1/retrack/nodes/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/dynamic/base.py` & `retrack-0.8.1/retrack/nodes/dynamic/base.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/dynamic/csv_table.py` & `retrack-0.8.1/retrack/nodes/dynamic/csv_table.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/endswith.py` & `retrack-0.8.1/retrack/nodes/endswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/endswithany.py` & `retrack-0.8.1/retrack/nodes/endswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/inputs.py` & `retrack-0.8.1/retrack/nodes/inputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/logic.py` & `retrack-0.8.1/retrack/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/match.py` & `retrack-0.8.1/retrack/nodes/match.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/math.py` & `retrack-0.8.1/retrack/nodes/math.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/outputs.py` & `retrack-0.8.1/retrack/nodes/outputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/start.py` & `retrack-0.8.1/retrack/nodes/start.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/startswith.py` & `retrack-0.8.1/retrack/nodes/startswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/nodes/startswithany.py` & `retrack-0.8.1/retrack/nodes/startswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/utils/registry.py` & `retrack-0.8.1/retrack/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/validators/__init__.py` & `retrack-0.8.1/retrack/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/retrack/validators/node_exists.py` & `retrack-0.8.1/retrack/validators/node_exists.py`

 * *Files identical despite different names*

### Comparing `retrack-0.8.0/PKG-INFO` & `retrack-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: retrack
-Version: 0.8.0
+Version: 0.8.1
 Summary: A business rules engine
 Home-page: https://github.com/gabrielguarisa/retrack
 License: MIT
 Keywords: rules,models,business,node,graph
 Author: Gabriel Guarisa
 Author-email: gabrielguarisa@gmail.com
 Requires-Python: >=3.7.16,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: networkx (==2.6.3) ; python_version < "3.8"
-Requires-Dist: networkx (>=3.0,<4.0) ; python_version >= "3.8"
+Requires-Dist: networkx (>=2.6.3,<3.0.0) ; python_version >= "3.8"
 Requires-Dist: numpy (==1.19.5) ; python_version < "3.8"
-Requires-Dist: numpy (>=1.24.0,<2.0.0) ; python_version >= "3.8"
+Requires-Dist: numpy (>=1.19.5,<2.0.0) ; python_version >= "3.8"
 Requires-Dist: pandas (==1.2.0) ; python_version < "3.8"
-Requires-Dist: pandas (>=1.5.2,<2.0.0) ; python_version >= "3.8"
+Requires-Dist: pandas (>=1.2.0,<2.0.0) ; python_version >= "3.8"
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Project-URL: Repository, https://github.com/gabrielguarisa/retrack
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://github.com/gabrielguarisa/retrack"><img src="https://raw.githubusercontent.com/gabrielguarisa/retrack/main/logo.png" alt="retrack"></a>
 </p>
@@ -48,14 +48,24 @@
 ```
 
 ## Usage
 
 ```python
 import retrack
 
+runner = retrack.Runner.from_json("your-rule.json")
+
+response = runner.execute(input_data)
+```
+
+Or, if you want to create the parser and runner manually:
+
+```python
+import retrack
+
 # Parse the rule/model
 parser = retrack.Parser(rule)
 
 # Create a runner
 runner = retrack.Runner(parser)
 
 # Run the rule/model passing the data
```

