# Comparing `tmp/canonicalwebteam.http-1.0.3.tar.gz` & `tmp/canonicalwebteam.http-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/canonicalwebteam.http-1.0.3.tar", last modified: Fri Mar 27 12:30:49 2020, max compression
+gzip compressed data, was "canonicalwebteam.http-1.0.4.tar", last modified: Mon Jun  5 15:51:46 2023, max compression
```

## Comparing `canonicalwebteam.http-1.0.3.tar` & `canonicalwebteam.http-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/canonicalwebteam/
--rw-r--r--   0 runner    (1001) docker     (115)       65 2020-03-27 12:30:35.000000 canonicalwebteam.http-1.0.3/canonicalwebteam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/canonicalwebteam/http/
--rw-r--r--   0 runner    (1001) docker     (115)     2090 2020-03-27 12:30:35.000000 canonicalwebteam.http-1.0.3/canonicalwebteam/http/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (115)     5099 2020-03-27 12:30:35.000000 canonicalwebteam.http-1.0.3/canonicalwebteam/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/canonicalwebteam.http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/canonicalwebteam.http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)      122 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/canonicalwebteam.http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)     1166 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/canonicalwebteam.http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)       23 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/canonicalwebteam.http.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)      416 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/canonicalwebteam.http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)     1166 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)      664 2020-03-27 12:30:35.000000 canonicalwebteam.http-1.0.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (115)      767 2020-03-27 12:30:35.000000 canonicalwebteam.http-1.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (115)       19 2020-03-27 12:30:35.000000 canonicalwebteam.http-1.0.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-27 12:30:48.000000 canonicalwebteam.http-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-27 12:30:35.000000 canonicalwebteam.http-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1314 2020-03-27 12:30:35.000000 canonicalwebteam.http-1.0.3/tests/test_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (115)     8931 2020-03-27 12:30:35.000000 canonicalwebteam.http-1.0.3/tests/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:46.846217 canonicalwebteam.http-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 15:51:38.000000 canonicalwebteam.http-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-05 15:51:46.846217 canonicalwebteam.http-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-05 15:51:38.000000 canonicalwebteam.http-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:46.846217 canonicalwebteam.http-1.0.4/canonicalwebteam/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 15:51:38.000000 canonicalwebteam.http-1.0.4/canonicalwebteam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:46.846217 canonicalwebteam.http-1.0.4/canonicalwebteam/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-05 15:51:38.000000 canonicalwebteam.http-1.0.4/canonicalwebteam/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-05 15:51:38.000000 canonicalwebteam.http-1.0.4/canonicalwebteam/http/heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:46.846217 canonicalwebteam.http-1.0.4/canonicalwebteam.http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-05 15:51:46.000000 canonicalwebteam.http-1.0.4/canonicalwebteam.http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-05 15:51:46.000000 canonicalwebteam.http-1.0.4/canonicalwebteam.http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:51:46.000000 canonicalwebteam.http-1.0.4/canonicalwebteam.http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 15:51:46.000000 canonicalwebteam.http-1.0.4/canonicalwebteam.http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 15:51:46.000000 canonicalwebteam.http-1.0.4/canonicalwebteam.http.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:51:46.846217 canonicalwebteam.http-1.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-06-05 15:51:38.000000 canonicalwebteam.http-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:46.846217 canonicalwebteam.http-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:38.000000 canonicalwebteam.http-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-05 15:51:38.000000 canonicalwebteam.http-1.0.4/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-05 15:51:38.000000 canonicalwebteam.http-1.0.4/tests/test_heuristics.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `canonicalwebteam.http-1.0.3/canonicalwebteam/http/heuristics.py` & `canonicalwebteam.http-1.0.4/canonicalwebteam/http/heuristics.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.http-1.0.3/canonicalwebteam/http/__init__.py` & `canonicalwebteam.http-1.0.4/canonicalwebteam/http/__init__.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.http-1.0.3/canonicalwebteam.http.egg-info/PKG-INFO` & `canonicalwebteam.http-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam.http
-Version: 1.0.3
+Version: 1.0.4
 Summary: For making HTTP requests with helpful defaults for Canonical's webteam.
 Home-page: https://github.com/canonical-webteam/http
 Author: Canonical webteam
 Author-email: webteam@canonical.com
 License: UNKNOWN
-Description: # canonicalwebteam.http
-        
-        [![Tests status](https://github.com/canonical-web-and-design/canonicalwebteam.http/workflows/Tests/badge.svg)](https://github.com/canonical-web-and-design/canonicalwebteam.http/actions?query=workflow%3ATests)
-        
-        **NB: We are retiring this module and will be removing it from our codebases.**
-        
-        A Python library for making HTTP requests with sensible defaults.
-        
-        ## Installation
-        
-        This module is in PyPi as `canonicalwebteam.http`. You should be able to install it simply with:
-        
-        ``` bash
-        pip install canonicalwebteam.http
-        ```
-        
-        ## Tests
-        
-        Tests are located in the [tests](tests) directory and can be run with `python -m unittest discover tests/`.
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# canonicalwebteam.http
+
+[![Tests status](https://github.com/canonical-web-and-design/canonicalwebteam.http/workflows/Tests/badge.svg)](https://github.com/canonical-web-and-design/canonicalwebteam.http/actions?query=workflow%3ATests)
+
+**NB: We are retiring this module and will be removing it from our codebases.**
+
+A Python library for making HTTP requests with sensible defaults.
+
+## Installation
+
+This module is in PyPi as `canonicalwebteam.http`. You should be able to install it simply with:
+
+``` bash
+pip install canonicalwebteam.http
+```
+
+## Tests
+
+Tests are located in the [tests](tests) directory and can be run with `python -m unittest discover tests/`.
+
+
```

### Comparing `canonicalwebteam.http-1.0.3/PKG-INFO` & `canonicalwebteam.http-1.0.4/canonicalwebteam.http.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam.http
-Version: 1.0.3
+Version: 1.0.4
 Summary: For making HTTP requests with helpful defaults for Canonical's webteam.
 Home-page: https://github.com/canonical-webteam/http
 Author: Canonical webteam
 Author-email: webteam@canonical.com
 License: UNKNOWN
-Description: # canonicalwebteam.http
-        
-        [![Tests status](https://github.com/canonical-web-and-design/canonicalwebteam.http/workflows/Tests/badge.svg)](https://github.com/canonical-web-and-design/canonicalwebteam.http/actions?query=workflow%3ATests)
-        
-        **NB: We are retiring this module and will be removing it from our codebases.**
-        
-        A Python library for making HTTP requests with sensible defaults.
-        
-        ## Installation
-        
-        This module is in PyPi as `canonicalwebteam.http`. You should be able to install it simply with:
-        
-        ``` bash
-        pip install canonicalwebteam.http
-        ```
-        
-        ## Tests
-        
-        Tests are located in the [tests](tests) directory and can be run with `python -m unittest discover tests/`.
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# canonicalwebteam.http
+
+[![Tests status](https://github.com/canonical-web-and-design/canonicalwebteam.http/workflows/Tests/badge.svg)](https://github.com/canonical-web-and-design/canonicalwebteam.http/actions?query=workflow%3ATests)
+
+**NB: We are retiring this module and will be removing it from our codebases.**
+
+A Python library for making HTTP requests with sensible defaults.
+
+## Installation
+
+This module is in PyPi as `canonicalwebteam.http`. You should be able to install it simply with:
+
+``` bash
+pip install canonicalwebteam.http
+```
+
+## Tests
+
+Tests are located in the [tests](tests) directory and can be run with `python -m unittest discover tests/`.
+
+
```

### Comparing `canonicalwebteam.http-1.0.3/README.md` & `canonicalwebteam.http-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.http-1.0.3/setup.py` & `canonicalwebteam.http-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #! /usr/bin/env python3
 
 # Core
 from setuptools import setup, find_packages
 
 setup(
     name="canonicalwebteam.http",
-    version="1.0.3",
+    version="1.0.4",
     author="Canonical webteam",
     author_email="webteam@canonical.com",
     url="https://github.com/canonical-webteam/http",
     packages=find_packages(),
     description=(
         "For making HTTP requests "
         "with helpful defaults for Canonical's webteam."
     ),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=[
-        "CacheControl>=0.12.5",
+        "CacheControl[filecache]>=0.12.5",
         "freezegun>=0.3.11",
         "HTTPretty>=1.0.2",
         "lockfile>=0.12.2",
         "mockredispy>=2.9.3",
         "redis>=3.0.1",
         "requests>=2.21.0",
     ],
```

### Comparing `canonicalwebteam.http-1.0.3/tests/test_heuristics.py` & `canonicalwebteam.http-1.0.4/tests/test_heuristics.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.http-1.0.3/tests/test_cache.py` & `canonicalwebteam.http-1.0.4/tests/test_cache.py`

 * *Files identical despite different names*

