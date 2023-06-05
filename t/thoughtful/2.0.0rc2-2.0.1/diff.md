# Comparing `tmp/thoughtful-2.0.0rc2.tar.gz` & `tmp/thoughtful-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-2.0.0rc2.tar", max compression
+gzip compressed data, was "thoughtful-2.0.1.tar", max compression
```

## Comparing `thoughtful-2.0.0rc2.tar` & `thoughtful-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0    11358 2022-12-14 17:25:44.942523 thoughtful-2.0.0rc2/LICENSE
--rw-r--r--   0        0        0     2992 2023-03-22 17:30:28.308693 thoughtful-2.0.0rc2/README.md
--rw-r--r--   0        0        0     1949 2023-05-31 17:45:48.486059 thoughtful-2.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0      222 2023-03-07 23:35:15.321689 thoughtful-2.0.0rc2/thoughtful/__init__.py
--rw-r--r--   0        0        0       57 2023-05-31 17:45:58.271778 thoughtful-2.0.0rc2/thoughtful/__version__.py
--rw-r--r--   0        0        0     1070 2023-05-31 17:32:30.137953 thoughtful-2.0.0rc2/thoughtful/environment_variables.py
--rw-r--r--   0        0        0      143 2022-12-14 17:25:44.949518 thoughtful-2.0.0rc2/thoughtful/supervisor/__init__.py
--rw-r--r--   0        0        0     4466 2023-05-31 17:33:24.495974 thoughtful-2.0.0rc2/thoughtful/supervisor/default_instances.py
--rw-r--r--   0        0        0     8580 2023-05-31 17:32:30.138562 thoughtful-2.0.0rc2/thoughtful/supervisor/main_context.py
--rw-r--r--   0        0        0    10567 2022-12-14 17:25:44.949966 thoughtful-2.0.0rc2/thoughtful/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2022-12-14 17:25:44.949991 thoughtful-2.0.0rc2/thoughtful/supervisor/py.typed
--rw-r--r--   0        0        0        0 2022-12-14 17:25:44.950159 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     2872 2023-05-31 17:32:30.139057 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/record.py
--rw-r--r--   0        0        0     1189 2023-05-31 17:32:30.139326 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/record_report.py
--rw-r--r--   0        0        0     2066 2023-05-31 17:32:30.139588 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/report.py
--rw-r--r--   0        0        0    10118 2023-05-31 17:32:30.139842 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      660 2023-05-31 17:32:30.140233 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/status.py
--rw-r--r--   0        0        0      876 2023-05-31 17:32:30.140535 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2022-12-14 17:25:44.951007 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1754 2023-05-31 17:32:30.140774 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     7609 2023-05-31 17:33:24.496190 thoughtful-2.0.0rc2/thoughtful/supervisor/step_context.py
--rw-r--r--   0        0        0     7435 2023-05-31 17:33:24.496425 thoughtful-2.0.0rc2/thoughtful/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0        0 2023-01-30 21:43:52.785761 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/__init__.py
--rw-r--r--   0        0        0      736 2023-04-06 19:41:20.157278 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/action.py
--rw-r--r--   0        0        0     1347 2023-05-31 17:32:30.141532 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/jwt_auth.py
--rw-r--r--   0        0        0     3935 2023-05-31 17:32:30.141687 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/notifier.py
--rw-r--r--   0        0        0     3184 2023-05-24 14:48:54.311303 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/payloads.py
--rw-r--r--   0        0        0     1352 2023-05-31 17:32:30.141964 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/token.py
--rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc2/setup.py
--rw-r--r--   0        0        0     4592 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-05 20:17:30.549384 thoughtful-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2992 2023-06-05 20:17:30.549384 thoughtful-2.0.1/README.md
+-rw-r--r--   0        0        0     1935 2023-06-05 20:17:30.549384 thoughtful-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/__version__.py
+-rw-r--r--   0        0        0     1070 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/environment_variables.py
+-rw-r--r--   0        0        0      143 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/__init__.py
+-rw-r--r--   0        0        0     4466 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/default_instances.py
+-rw-r--r--   0        0        0     8580 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/main_context.py
+-rw-r--r--   0        0        0    10567 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/py.typed
+-rw-r--r--   0        0        0        0 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     2872 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     1189 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/record_report.py
+-rw-r--r--   0        0        0     2066 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/report.py
+-rw-r--r--   0        0        0    10118 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      660 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/status.py
+-rw-r--r--   0        0        0      876 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1754 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     7609 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/step_context.py
+-rw-r--r--   0        0        0     7435 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/__init__.py
+-rw-r--r--   0        0        0      736 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/action.py
+-rw-r--r--   0        0        0     1347 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/jwt_auth.py
+-rw-r--r--   0        0        0     3935 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/notifier.py
+-rw-r--r--   0        0        0     3184 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/payloads.py
+-rw-r--r--   0        0        0     1352 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/token.py
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-2.0.1/PKG-INFO
```

### Comparing `thoughtful-2.0.0rc2/LICENSE` & `thoughtful-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/README.md` & `thoughtful-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/pyproject.toml` & `thoughtful-2.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "thoughtful"
-version = "2.0.0rc2"
+version = "2.0.1"
 description = "Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor"
-authors = ["Thoughtful Automation <engineering@thoughtfulautomation.com>"]
+authors = ["Thoughtful Automation <care@thoughtful.ai>"]
 license = "Apache-2.0"
 readme = 'README.md'
-homepage = "https://thoughtfulautomation.com"
+homepage = "https://thoughtful.ai"
 repository = "https://github.com/thoughtful-automation/thoughtful"
-documentation = "https://readthedocs.com/projects/thoughtful-supervisor/"
+documentation = "https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/index.html"
 
 keywords = ['rpa', 'robot-framework', 'robocorp', 'automation']
 
 classifiers = [
   "Topic :: Security :: Cryptography",
   "License :: OSI Approved :: Apache Software License",
   "Framework :: Robot Framework",
```

### Comparing `thoughtful-2.0.0rc2/thoughtful/environment_variables.py` & `thoughtful-2.0.1/thoughtful/environment_variables.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/default_instances.py` & `thoughtful-2.0.1/thoughtful/supervisor/default_instances.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/main_context.py` & `thoughtful-2.0.1/thoughtful/supervisor/main_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/manifest.py` & `thoughtful-2.0.1/thoughtful/supervisor/manifest.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/record.py` & `thoughtful-2.0.1/thoughtful/supervisor/reporting/record.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/record_report.py` & `thoughtful-2.0.1/thoughtful/supervisor/reporting/record_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/report.py` & `thoughtful-2.0.1/thoughtful/supervisor/reporting/report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/report_builder.py` & `thoughtful-2.0.1/thoughtful/supervisor/reporting/report_builder.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/status.py` & `thoughtful-2.0.1/thoughtful/supervisor/reporting/status.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/step_report.py` & `thoughtful-2.0.1/thoughtful/supervisor/reporting/step_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/timed_report.py` & `thoughtful-2.0.1/thoughtful/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/timer.py` & `thoughtful-2.0.1/thoughtful/supervisor/reporting/timer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/step_context.py` & `thoughtful-2.0.1/thoughtful/supervisor/step_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/step_decorator_factory.py` & `thoughtful-2.0.1/thoughtful/supervisor/step_decorator_factory.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/action.py` & `thoughtful-2.0.1/thoughtful/supervisor/streaming/action.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/jwt_auth.py` & `thoughtful-2.0.1/thoughtful/supervisor/streaming/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/notifier.py` & `thoughtful-2.0.1/thoughtful/supervisor/streaming/notifier.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/payloads.py` & `thoughtful-2.0.1/thoughtful/supervisor/streaming/payloads.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/token.py` & `thoughtful-2.0.1/thoughtful/supervisor/streaming/token.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc2/PKG-INFO` & `thoughtful-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thoughtful
-Version: 2.0.0rc2
+Version: 2.0.1
 Summary: Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor
-Home-page: https://thoughtfulautomation.com
+Home-page: https://thoughtful.ai
 License: Apache-2.0
 Keywords: rpa,robot-framework,robocorp,automation
 Author: Thoughtful Automation
-Author-email: engineering@thoughtfulautomation.com
+Author-email: care@thoughtful.ai
 Requires-Python: >=3.8,<3.12
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -26,15 +26,15 @@
 Requires-Dist: pre-commit (>=2.17.0,<3.0.0)
 Requires-Dist: pyconfs (>=0.5.5,<0.6.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pydantic-yaml (>=0.6.3,<0.7.0)
 Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
 Requires-Dist: pyyaml (>=5.4.1)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Project-URL: Documentation, https://readthedocs.com/projects/thoughtful-supervisor/
+Project-URL: Documentation, https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/index.html
 Project-URL: Repository, https://github.com/thoughtful-automation/thoughtful
 Description-Content-Type: text/markdown
 
 **thoughtful** is a collection of open-source libraries and tools for Robot Process
 Automation (RPA) development. The goal of this project is to provide a set of
 for supervising bot execution, and enabling these bots to do more.
```

