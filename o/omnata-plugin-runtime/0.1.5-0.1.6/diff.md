# Comparing `tmp/omnata_plugin_runtime-0.1.5.tar.gz` & `tmp/omnata_plugin_runtime-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_plugin_runtime-0.1.5.tar", max compression
+gzip compressed data, was "omnata_plugin_runtime-0.1.6.tar", max compression
```

## Comparing `omnata_plugin_runtime-0.1.5.tar` & `omnata_plugin_runtime-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    26526 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/LICENSE
--rw-r--r--   0        0        0      296 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/README.md
--rw-r--r--   0        0        0      826 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1213 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/__init__.py
--rw-r--r--   0        0        0     3277 2023-06-05 01:51:08.807662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/api.py
--rw-r--r--   0        0        0    29524 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/configuration.py
--rw-r--r--   0        0        0    12646 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/forms.py
--rw-r--r--   0        0        0     3985 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/logging.py
--rw-r--r--   0        0        0    64614 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/omnata_plugin.py
--rw-r--r--   0        0        0    18397 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/plugin_entrypoints.py
--rw-r--r--   0        0        0    10078 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/rate_limiting.py
--rw-r--r--   0        0        0     2611 2023-06-05 01:51:08.811662 omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/record_transformer.py
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-05 02:56:10.903714 omnata_plugin_runtime-0.1.6/LICENSE
+-rw-r--r--   0        0        0      296 2023-06-05 02:56:10.903714 omnata_plugin_runtime-0.1.6/README.md
+-rw-r--r--   0        0        0      826 2023-06-05 02:56:10.903714 omnata_plugin_runtime-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1213 2023-06-05 02:56:10.907714 omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/__init__.py
+-rw-r--r--   0        0        0     3277 2023-06-05 02:56:10.907714 omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/api.py
+-rw-r--r--   0        0        0    29524 2023-06-05 02:56:10.907714 omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/configuration.py
+-rw-r--r--   0        0        0    12646 2023-06-05 02:56:10.907714 omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/forms.py
+-rw-r--r--   0        0        0     4387 2023-06-05 02:56:10.907714 omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/logging.py
+-rw-r--r--   0        0        0    64614 2023-06-05 02:56:10.907714 omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/omnata_plugin.py
+-rw-r--r--   0        0        0    18397 2023-06-05 02:56:10.907714 omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/plugin_entrypoints.py
+-rw-r--r--   0        0        0    10078 2023-06-05 02:56:10.907714 omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/rate_limiting.py
+-rw-r--r--   0        0        0     2611 2023-06-05 02:56:10.907714 omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/record_transformer.py
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.6/PKG-INFO
```

### Comparing `omnata_plugin_runtime-0.1.5/LICENSE` & `omnata_plugin_runtime-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.5/pyproject.toml` & `omnata_plugin_runtime-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnata-plugin-runtime"
-version = "0.1.5"
+version = "0.1.6"
 description = "A development kit to assist with building, testing and publishing Omnata Plugins"
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_plugin_runtime", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/__init__.py` & `omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/api.py` & `omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/api.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/configuration.py` & `omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/configuration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/forms.py` & `omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/forms.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/logging.py` & `omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     """
     Custom logger that can handle pydantic validation errors.
     Without this, you get "Object of type ErrorWrapper is not JSON serializable"
     when logging the exception.
     """
     def error(self, msg, *args, **kwargs):
         if isinstance(msg, ValidationError):
-            msg = msg.errors()
+            # If the exc_info or stack_info flags are set, unset them and manually
+            # add the error information to the log message.
+            exc_info = kwargs.pop('exc_info', False)
+            stack_info = kwargs.pop('stack_info', False)
+            if exc_info or stack_info:
+                msg = f"{msg.errors()} (originally raised at {msg.__traceback__.tb_frame.f_code.co_filename}:{msg.__traceback__.tb_lineno})"
         super().error(msg, *args, **kwargs)
 
 class OmnataPluginLogHandler(logging.handlers.BufferingHandler):
     """
     A logging handler to ship logs back into Omnata Snowflake tables. It uses a combination
     of time and capacity to flush the buffer.
     Additional information about the current sync and run is included, so that logs can be filtered easily.
```

### Comparing `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/omnata_plugin.py` & `omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/omnata_plugin.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/plugin_entrypoints.py` & `omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/plugin_entrypoints.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/rate_limiting.py` & `omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.5/src/omnata_plugin_runtime/record_transformer.py` & `omnata_plugin_runtime-0.1.6/src/omnata_plugin_runtime/record_transformer.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.5/PKG-INFO` & `omnata_plugin_runtime-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnata-plugin-runtime
-Version: 0.1.5
+Version: 0.1.6
 Summary: A development kit to assist with building, testing and publishing Omnata Plugins
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

