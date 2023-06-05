# Comparing `tmp/omnata_plugin_runtime-0.1.4.tar.gz` & `tmp/omnata_plugin_runtime-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_plugin_runtime-0.1.4.tar", max compression
+gzip compressed data, was "omnata_plugin_runtime-0.1.5.tar", max compression
```

## Comparing `omnata_plugin_runtime-0.1.4.tar` & `omnata_plugin_runtime-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    26526 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/LICENSE
--rw-r--r--   0        0        0      296 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/README.md
--rw-r--r--   0        0        0      826 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1213 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/__init__.py
--rw-r--r--   0        0        0     3277 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/api.py
--rw-r--r--   0        0        0    29524 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/configuration.py
--rw-r--r--   0        0        0    12646 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/forms.py
--rw-r--r--   0        0        0     3975 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/logging.py
--rw-r--r--   0        0        0    64614 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/omnata_plugin.py
--rw-r--r--   0        0        0    18397 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/plugin_entrypoints.py
--rw-r--r--   0        0        0    10078 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/rate_limiting.py
--rw-r--r--   0        0        0     2611 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/record_transformer.py
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/LICENSE
+-rw-r--r--   0        0        0      296 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/README.md
+-rw-r--r--   0        0        0      826 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1213 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/__init__.py
+-rw-r--r--   0        0        0     3277 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/api.py
+-rw-r--r--   0        0        0    29524 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/configuration.py
+-rw-r--r--   0        0        0    12646 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/forms.py
+-rw-r--r--   0        0        0     3985 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/logging.py
+-rw-r--r--   0        0        0    64614 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/omnata_plugin.py
+-rw-r--r--   0        0        0    18397 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/plugin_entrypoints.py
+-rw-r--r--   0        0        0    10078 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/rate_limiting.py
+-rw-r--r--   0        0        0     2611 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/record_transformer.py
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.5/PKG-INFO
```

### Comparing `omnata_plugin_runtime-0.1.4/LICENSE` & `omnata_plugin_runtime-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.4/pyproject.toml` & `omnata_plugin_runtime-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnata-plugin-runtime"
-version = "0.1.4"
+version = "0.1.5"
 description = "A development kit to assist with building, testing and publishing Omnata Plugins"
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_plugin_runtime", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/__init__.py` & `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/api.py` & `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/api.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/configuration.py` & `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/configuration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/forms.py` & `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/forms.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/logging.py` & `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import logging.handlers
 from typing import List
 import pandas
 from snowflake.snowpark import Session
 from pydantic import ValidationError
 
-class CustomLogger(logging.Logger):
+class CustomLogger(logging.getLoggerClass()):
     """
     Custom logger that can handle pydantic validation errors.
     Without this, you get "Object of type ErrorWrapper is not JSON serializable"
     when logging the exception.
     """
     def error(self, msg, *args, **kwargs):
         if isinstance(msg, ValidationError):
```

### Comparing `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/omnata_plugin.py` & `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/omnata_plugin.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/plugin_entrypoints.py` & `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/plugin_entrypoints.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/rate_limiting.py` & `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/record_transformer.py` & `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/record_transformer.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.4/PKG-INFO` & `omnata_plugin_runtime-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnata-plugin-runtime
-Version: 0.1.4
+Version: 0.1.5
 Summary: A development kit to assist with building, testing and publishing Omnata Plugins
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

