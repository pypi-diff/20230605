# Comparing `tmp/permutate-0.0.7.tar.gz` & `tmp/permutate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permutate-0.0.7.tar", max compression
+gzip compressed data, was "permutate-0.0.9.tar", max compression
```

## Comparing `permutate-0.0.7.tar` & `permutate-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     8712 2023-06-01 20:24:56.599704 permutate-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-05-31 14:00:12.890922 permutate-0.0.7/permutate/__init__.py
--rw-r--r--   0        0        0       48 2023-05-31 17:06:56.770244 permutate-0.0.7/permutate/__main__.py
--rw-r--r--   0        0        0     2354 2023-06-01 16:23:45.772329 permutate-0.0.7/permutate/job_request_schema.py
--rw-r--r--   0        0        0    10079 2023-05-31 17:06:56.771081 permutate-0.0.7/permutate/job_response_schema.py
--rw-r--r--   0        0        0     1153 2023-05-31 17:06:56.771661 permutate-0.0.7/permutate/logger.py
--rw-r--r--   0        0        0     2357 2023-05-31 17:06:56.771839 permutate-0.0.7/permutate/main.py
--rw-r--r--   0        0        0     7518 2023-06-01 19:41:00.861159 permutate-0.0.7/permutate/runner.py
--rw-r--r--   0        0        0      559 2023-05-25 17:31:15.484872 permutate-0.0.7/permutate/singleton.py
--rw-r--r--   0        0        0     3436 2023-05-31 17:06:56.772174 permutate-0.0.7/permutate/templates/job_result_template.html
--rw-r--r--   0        0        0     2032 2023-06-01 16:38:51.520700 permutate-0.0.7/permutate/workspace/plugin_test.yaml
--rw-r--r--   0        0        0      602 2023-06-01 21:33:39.569472 permutate-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     9458 1970-01-01 00:00:00.000000 permutate-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     8939 2023-06-05 16:22:27.278398 permutate-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/__main__.py
+-rw-r--r--   0        0        0     2354 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/job_request_schema.py
+-rw-r--r--   0        0        0    10079 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/job_response_schema.py
+-rw-r--r--   0        0        0     1153 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/logger.py
+-rw-r--r--   0        0        0     2357 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/main.py
+-rw-r--r--   0        0        0     7553 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/runner.py
+-rw-r--r--   0        0        0      559 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/singleton.py
+-rw-r--r--   0        0        0     3436 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/templates/job_result_template.html
+-rw-r--r--   0        0        0     2032 2023-06-05 16:22:27.282398 permutate-0.0.9/permutate/workspace/plugin_test.yaml
+-rw-r--r--   0        0        0      602 2023-06-05 16:22:27.286398 permutate-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     9685 1970-01-01 00:00:00.000000 permutate-0.0.9/PKG-INFO
```

### Comparing `permutate-0.0.7/README.md` & `permutate-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -192,14 +192,19 @@
 
 This command will run the tests on a sample test file provided in the package and save the results to an html file. This command can be used to see the sample output.
 
 ```sh
 permutate run
 ```
 
+#### Docker
+```shell
+docker run -v /LOCALPATH/plugin_test.yaml:/usr/app/plugin_test.yaml -e "OPENAI_KEY=your-key" -e "COHERE_API_KEY=your-key" -e "GOOGLE_APPLICATION_CREDENTIALS=your-file-path" shrikant14/permutate:latest
+```
+
 ##### Output
 You can save your permutate run output to: 
 1. HTML Report:
 
     You can save your permutation run output to an HTML Report that presents the results of the permutation run in a structured and visually appealing format.
 
    Sample report: https://raw.githubusercontent.com/LegendaryAI/permutate/main/docs/sample_result.html
```

### Comparing `permutate-0.0.7/permutate/job_request_schema.py` & `permutate-0.0.9/permutate/job_request_schema.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.7/permutate/job_response_schema.py` & `permutate-0.0.9/permutate/job_response_schema.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.7/permutate/logger.py` & `permutate-0.0.9/permutate/logger.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.7/permutate/main.py` & `permutate-0.0.9/permutate/main.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.7/permutate/runner.py` & `permutate-0.0.9/permutate/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         if config.use_openplugin_library:
             try:
                 response_json = run_plugin_selector(payload)
                 if response_json is None:
                     passed = False
             except Exception as e:
                 print(e)
+                response_json=None
                 passed = False
         else:
             if permutation.tool_selector.get("provider") == "Imprompt":
                 url = config.imprompt_tool_selector
             elif permutation.tool_selector.get("provider") == "Langchain":
                 url = config.langchain_tool_selector
             else:
```

### Comparing `permutate-0.0.7/permutate/singleton.py` & `permutate-0.0.9/permutate/singleton.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.7/permutate/templates/job_result_template.html` & `permutate-0.0.9/permutate/templates/job_result_template.html`

 * *Files identical despite different names*

### Comparing `permutate-0.0.7/permutate/workspace/plugin_test.yaml` & `permutate-0.0.9/permutate/workspace/plugin_test.yaml`

 * *Files identical despite different names*

### Comparing `permutate-0.0.7/pyproject.toml` & `permutate-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "permutate"
-version = "0.0.7"
+version = "0.0.9"
 description = "Testing framework for LLM Plugins"
 authors = ["shrikant <shrikant.pm14@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "2.29.0"
```

### Comparing `permutate-0.0.7/PKG-INFO` & `permutate-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permutate
-Version: 0.0.7
+Version: 0.0.9
 Summary: Testing framework for LLM Plugins
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -213,14 +213,19 @@
 
 This command will run the tests on a sample test file provided in the package and save the results to an html file. This command can be used to see the sample output.
 
 ```sh
 permutate run
 ```
 
+#### Docker
+```shell
+docker run -v /LOCALPATH/plugin_test.yaml:/usr/app/plugin_test.yaml -e "OPENAI_KEY=your-key" -e "COHERE_API_KEY=your-key" -e "GOOGLE_APPLICATION_CREDENTIALS=your-file-path" shrikant14/permutate:latest
+```
+
 ##### Output
 You can save your permutate run output to: 
 1. HTML Report:
 
     You can save your permutation run output to an HTML Report that presents the results of the permutation run in a structured and visually appealing format.
 
    Sample report: https://raw.githubusercontent.com/LegendaryAI/permutate/main/docs/sample_result.html
```

