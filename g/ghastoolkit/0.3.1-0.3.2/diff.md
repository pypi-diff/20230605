# Comparing `tmp/ghastoolkit-0.3.1.tar.gz` & `tmp/ghastoolkit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.3.1.tar", last modified: Mon May 22 15:12:35 2023, max compression
+gzip compressed data, was "ghastoolkit-0.3.2.tar", last modified: Mon Jun  5 18:46:12 2023, max compression
```

## Comparing `ghastoolkit-0.3.1.tar` & `ghastoolkit-0.3.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:35.947193 ghastoolkit-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-22 15:12:35.947193 ghastoolkit-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:12:35.947193 ghastoolkit-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:35.935192 ghastoolkit-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:35.939192 ghastoolkit-0.3.1/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:35.943192 ghastoolkit-0.3.1/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/codeql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/codeql/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:35.947193 ghastoolkit-0.3.1/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:35.947193 ghastoolkit-0.3.1/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:35.947193 ghastoolkit-0.3.1/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:35.939192 ghastoolkit-0.3.1/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-22 15:12:35.000000 ghastoolkit-0.3.1/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-22 15:12:35.000000 ghastoolkit-0.3.1/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:12:35.000000 ghastoolkit-0.3.1/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 15:12:35.000000 ghastoolkit-0.3.1/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 15:12:35.000000 ghastoolkit-0.3.1/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:12:35.947193 ghastoolkit-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-22 15:12:03.000000 ghastoolkit-0.3.1/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.849889 ghastoolkit-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.849889 ghastoolkit-0.3.2/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.849889 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.3.1/LICENSE` & `ghastoolkit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/PKG-INFO` & `ghastoolkit-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.3.1/README.md` & `ghastoolkit-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/pyproject.toml` & `ghastoolkit-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -17,16 +17,16 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "certifi==2023.5.7",
     "charset-normalizer==3.1.0",
     "idna==3.4",
     "PyYAML==6.0",
-    "requests==2.30.0",
     "ratelimit==2.2.1",
+    "requests==2.31.0",
     "urllib3==2.0.2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/GeekMasher/ghastoolkit"
 "Bug Tracker" = "https://github.com/GeekMasher/ghastoolkit/issues"
```

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/__init__.py` & `ghastoolkit-0.3.2/src/ghastoolkit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
@@ -13,19 +13,19 @@
 __license__ = "MIT License"
 __copyright__ = "Copyright (c) 2023, GeekMasher"
 
 __author__ = "GeekMasher"
 
 __banner__ = f"""\
  _____  _   _   ___   _____ _____           _ _    _ _   
-|  __ \| | | | / _ \ /  ___|_   _|         | | |  (_) |  
-| |  \/| |_| |/ /_\ \\\\ `--.  | | ___   ___ | | | ___| |_ 
-| | __ |  _  ||  _  | `--. \ | |/ _ \ / _ \| | |/ / | __|
-| |_\ \| | | || | | |/\__/ / | | (_) | (_) | |   <| | |_ 
- \____/\_| |_/\_| |_/\____/  \_/\___/ \___/|_|_|\_\_|\__| v{__version__} 
+|  __ \\| | | | / _ \\ /  ___|_   _|         | | |  (_) |  
+| |  \\/| |_| |/ /_\\ \\\\ `--.  | | ___   ___ | | | ___| |_ 
+| | __ |  _  ||  _  | `--. \\ | |/ _ \\ / _ \\| | |/ / | __|
+| |_\\ \\| | | || | | |/\\__/ / | | (_) | (_) | |   <| | |_ 
+ \\____/\\_| |_/\\_| |_/\\____/  \\_/\\___/ \\___/|_|_|\\_\\_|\\__| v{__version__} 
 """
 
 
 # Octokit
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.octokit.octokit import Octokit, RestRequest, GraphQLRequest
 from ghastoolkit.octokit.codescanning import CodeScanning, CodeAlert
```

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/__main__.py` & `ghastoolkit-0.3.2/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.3.2/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.3.2/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.3.2/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.3.2/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.3.2/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.3.2/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.3.2/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.3.2/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.3.2/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.3.2/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.3.2/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.3.2/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.3.2/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.3.2/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.3.1/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.3.2/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/tests/test_codeqldb.py` & `ghastoolkit-0.3.2/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/tests/test_codescanning.py` & `ghastoolkit-0.3.2/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/tests/test_default.py` & `ghastoolkit-0.3.2/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/tests/test_dependencies.py` & `ghastoolkit-0.3.2/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/tests/test_depgraph.py` & `ghastoolkit-0.3.2/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/tests/test_github.py` & `ghastoolkit-0.3.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/tests/test_licenses.py` & `ghastoolkit-0.3.2/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/tests/test_octokit.py` & `ghastoolkit-0.3.2/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.1/tests/test_secretscanning.py` & `ghastoolkit-0.3.2/tests/test_secretscanning.py`

 * *Files identical despite different names*

