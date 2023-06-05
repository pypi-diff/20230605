# Comparing `tmp/openplugin-0.0.8.tar.gz` & `tmp/openplugin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-0.0.8.tar", max compression
+gzip compressed data, was "openplugin-0.0.9.tar", max compression
```

## Comparing `openplugin-0.0.8.tar` & `openplugin-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.8/README.md
--rw-r--r--   0        0        0      754 2023-06-01 14:53:19.914449 openplugin-0.0.8/openplugin/__init__.py
--rw-r--r--   0        0        0       49 2023-05-31 18:34:59.726797 openplugin-0.0.8/openplugin/__main__.py
--rw-r--r--   0        0        0      855 2023-05-31 17:18:40.367458 openplugin-0.0.8/openplugin/api/__init__.py
--rw-r--r--   0        0        0      277 2023-05-23 18:12:55.625523 openplugin-0.0.8/openplugin/api/http_error.py
--rw-r--r--   0        0        0      874 2023-06-01 14:05:00.648019 openplugin-0.0.8/openplugin/api/imprompt.py
--rw-r--r--   0        0        0      857 2023-05-31 17:18:40.370699 openplugin-0.0.8/openplugin/api/langchain.py
--rw-r--r--   0        0        0     8094 2023-06-01 15:09:41.946666 openplugin-0.0.8/openplugin/bindings/imprompt/imprompt_plugin_selector.py
--rw-r--r--   0        0        0     5322 2023-06-01 15:09:41.949092 openplugin-0.0.8/openplugin/bindings/langchain/langchain_plugin_selector.py
--rw-r--r--   0        0        0     7329 2023-05-30 21:50:10.184387 openplugin-0.0.8/openplugin/interfaces/plugin_selector.py
--rw-r--r--   0        0        0      561 2023-06-01 15:09:41.950905 openplugin-0.0.8/openplugin/main.py
--rw-r--r--   0        0        0     1055 2023-06-01 15:13:37.221779 openplugin-0.0.8/openplugin/utils/run_plugin_selector.py
--rw-r--r--   0        0        0      521 2023-06-01 15:13:43.522364 openplugin-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7160 1970-01-01 00:00:00.000000 openplugin-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6436 2023-05-25 20:33:57.756239 openplugin-0.0.9/README.md
+-rw-r--r--   0        0        0      754 2023-06-01 14:53:19.914449 openplugin-0.0.9/openplugin/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-31 18:34:59.726797 openplugin-0.0.9/openplugin/__main__.py
+-rw-r--r--   0        0        0      855 2023-05-31 17:18:40.367458 openplugin-0.0.9/openplugin/api/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-23 18:12:55.625523 openplugin-0.0.9/openplugin/api/http_error.py
+-rw-r--r--   0        0        0      874 2023-06-01 14:05:00.648019 openplugin-0.0.9/openplugin/api/imprompt.py
+-rw-r--r--   0        0        0      857 2023-05-31 17:18:40.370699 openplugin-0.0.9/openplugin/api/langchain.py
+-rw-r--r--   0        0        0     8094 2023-06-01 15:09:41.946666 openplugin-0.0.9/openplugin/bindings/imprompt/imprompt_plugin_selector.py
+-rw-r--r--   0        0        0     5322 2023-06-01 15:09:41.949092 openplugin-0.0.9/openplugin/bindings/langchain/langchain_plugin_selector.py
+-rw-r--r--   0        0        0     7329 2023-05-30 21:50:10.184387 openplugin-0.0.9/openplugin/interfaces/plugin_selector.py
+-rw-r--r--   0        0        0      561 2023-06-01 15:09:41.950905 openplugin-0.0.9/openplugin/main.py
+-rw-r--r--   0        0        0     1055 2023-06-01 15:13:37.221779 openplugin-0.0.9/openplugin/utils/run_plugin_selector.py
+-rw-r--r--   0        0        0      521 2023-06-01 15:25:32.438354 openplugin-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7160 1970-01-01 00:00:00.000000 openplugin-0.0.9/PKG-INFO
```

### Comparing `openplugin-0.0.8/README.md` & `openplugin-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/openplugin/__init__.py` & `openplugin-0.0.9/openplugin/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/openplugin/api/__init__.py` & `openplugin-0.0.9/openplugin/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/openplugin/api/imprompt.py` & `openplugin-0.0.9/openplugin/api/imprompt.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/openplugin/api/langchain.py` & `openplugin-0.0.9/openplugin/api/langchain.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/openplugin/bindings/imprompt/imprompt_plugin_selector.py` & `openplugin-0.0.9/openplugin/bindings/imprompt/imprompt_plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/openplugin/bindings/langchain/langchain_plugin_selector.py` & `openplugin-0.0.9/openplugin/bindings/langchain/langchain_plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/openplugin/interfaces/plugin_selector.py` & `openplugin-0.0.9/openplugin/interfaces/plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/openplugin/main.py` & `openplugin-0.0.9/openplugin/main.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/openplugin/utils/run_plugin_selector.py` & `openplugin-0.0.9/openplugin/utils/run_plugin_selector.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.8/pyproject.toml` & `openplugin-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openplugin"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["shrikant <shrikant.pm14@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 langchain = "^0.0.178"
```

### Comparing `openplugin-0.0.8/PKG-INFO` & `openplugin-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

