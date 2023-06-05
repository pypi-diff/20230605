# Comparing `tmp/invoke-plugin-for-pylint-1.0.1.tar.gz` & `tmp/invoke-plugin-for-pylint-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoke-plugin-for-pylint-1.0.1.tar", last modified: Mon May  1 19:05:13 2023, max compression
+gzip compressed data, was "invoke-plugin-for-pylint-2.0.0.tar", last modified: Mon Jun  5 14:28:44 2023, max compression
```

## Comparing `invoke-plugin-for-pylint-1.0.1.tar` & `invoke-plugin-for-pylint-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:13.641551 invoke-plugin-for-pylint-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 19:04:43.000000 invoke-plugin-for-pylint-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-01 19:05:13.641551 invoke-plugin-for-pylint-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-01 19:04:43.000000 invoke-plugin-for-pylint-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:13.641551 invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-01 19:04:43.000000 invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-01 19:04:43.000000 invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint/_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:13.641551 invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-01 19:05:13.000000 invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-01 19:05:13.000000 invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:05:13.000000 invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-01 19:05:13.000000 invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 19:05:13.000000 invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-01 19:04:43.000000 invoke-plugin-for-pylint-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:05:13.641551 invoke-plugin-for-pylint-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:13.641551 invoke-plugin-for-pylint-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-01 19:04:43.000000 invoke-plugin-for-pylint-1.0.1/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:28:44.497503 invoke-plugin-for-pylint-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 14:28:19.000000 invoke-plugin-for-pylint-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-06-05 14:28:44.497503 invoke-plugin-for-pylint-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-05 14:28:19.000000 invoke-plugin-for-pylint-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:28:44.497503 invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-05 14:28:19.000000 invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-05 14:28:19.000000 invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint/_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:28:44.497503 invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-06-05 14:28:44.000000 invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-05 14:28:44.000000 invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:28:44.000000 invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-05 14:28:44.000000 invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 14:28:44.000000 invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-05 14:28:19.000000 invoke-plugin-for-pylint-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:28:44.501503 invoke-plugin-for-pylint-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:28:44.497503 invoke-plugin-for-pylint-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-05 14:28:19.000000 invoke-plugin-for-pylint-2.0.0/tests/test_plugin.py
```

### Comparing `invoke-plugin-for-pylint-1.0.1/LICENSE` & `invoke-plugin-for-pylint-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invoke-plugin-for-pylint-1.0.1/PKG-INFO` & `invoke-plugin-for-pylint-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoke-plugin-for-pylint
-Version: 1.0.1
+Version: 2.0.0
 Summary: Pylint plugin which disables checks for proper integration with invoke
 Author-email: Kai Mueller <kai.mueller01@sap.com>
 License: Apache-2.0
 Project-URL: Issue Tracker, https://github.com/SAP/invoke-plugin-for-pylint/issues
 Project-URL: Changelog, https://github.com/SAP/invoke-plugin-for-pylint/blob/main/CHANGELOG.md
 Keywords: pylint,invoke,plugin,inv,linter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `invoke-plugin-for-pylint-1.0.1/README.md` & `invoke-plugin-for-pylint-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint/_plugin.py` & `invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint/_plugin.py`

 * *Files identical despite different names*

### Comparing `invoke-plugin-for-pylint-1.0.1/invoke_plugin_for_pylint.egg-info/PKG-INFO` & `invoke-plugin-for-pylint-2.0.0/invoke_plugin_for_pylint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoke-plugin-for-pylint
-Version: 1.0.1
+Version: 2.0.0
 Summary: Pylint plugin which disables checks for proper integration with invoke
 Author-email: Kai Mueller <kai.mueller01@sap.com>
 License: Apache-2.0
 Project-URL: Issue Tracker, https://github.com/SAP/invoke-plugin-for-pylint/issues
 Project-URL: Changelog, https://github.com/SAP/invoke-plugin-for-pylint/blob/main/CHANGELOG.md
 Keywords: pylint,invoke,plugin,inv,linter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `invoke-plugin-for-pylint-1.0.1/pyproject.toml` & `invoke-plugin-for-pylint-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invoke-plugin-for-pylint"
-version = "1.0.1"
+version = "2.0.0"
 description = "Pylint plugin which disables checks for proper integration with invoke"
 authors = [{ name = "Kai Mueller", email = "kai.mueller01@sap.com"}]
 readme = "README.md"
 keywords = ["pylint", "invoke", "plugin", "inv", "linter"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
@@ -24,38 +24,38 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Quality Assurance",
     "Typing :: Typed"
 ]
 requires-python = ">=3.7,<4"
 dependencies = [
-    "invoke>=1.5,<3",
+    "invoke>=2,<3",
     "pylint~=2.11",
 ]
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Issue Tracker" = "https://github.com/SAP/invoke-plugin-for-pylint/issues"
 "Changelog" = "https://github.com/SAP/invoke-plugin-for-pylint/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit==2.21.0",
-    "pylint==2.17.2",
+    "pylint==2.17.4",
     "pytest==7.3.1",
     "pytest-mock==3.10.0",
-    "coverage[toml]==7.2.3",
+    "coverage[toml]==7.2.7",
     "diff-cover==7.5.0",
-    "pytest-cov==4.0.0",
+    "pytest-cov==4.1.0",
     "black==23.3.0",
     "isort==5.11.5",
-    "mypy==1.2.0",
-    "types-invoke==2.0.0.6",
+    "mypy==1.3.0",
+    "types-invoke==2.0.0.8",
 ]
 
 [tool.setuptools.packages.find]
 include = ["invoke_plugin_for_pylint"]
 
 [tool.setuptools.package-data]
 invoke_plugin_for_pylint = ["py.typed"]
```

### Comparing `invoke-plugin-for-pylint-1.0.1/tests/test_plugin.py` & `invoke-plugin-for-pylint-2.0.0/tests/test_plugin.py`

 * *Files identical despite different names*

