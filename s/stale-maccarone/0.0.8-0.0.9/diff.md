# Comparing `tmp/stale_maccarone-0.0.8.tar.gz` & `tmp/stale_maccarone-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stale_maccarone-0.0.8.tar", last modified: Mon May 29 18:45:15 2023, max compression
+gzip compressed data, was "stale_maccarone-0.0.9.tar", last modified: Thu Jun  1 17:08:40 2023, max compression
```

## Comparing `stale_maccarone-0.0.8.tar` & `stale_maccarone-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/src/stale_maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/src/stale_maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/scripts/preprocess.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/src/stale_maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.893379 stale_maccarone-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.893379 stale_maccarone-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/src/stale_maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/loader.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/src/stale_maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/scripts/preprocess.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/src/stale_maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-01 17:08:32.000000 stale_maccarone-0.0.9/src/stale_maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/src/stale_maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-01 17:08:40.000000 stale_maccarone-0.0.9/src/stale_maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-01 17:08:40.000000 stale_maccarone-0.0.9/src/stale_maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:08:40.000000 stale_maccarone-0.0.9/src/stale_maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-01 17:08:40.000000 stale_maccarone-0.0.9/src/stale_maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 17:08:40.000000 stale_maccarone-0.0.9/src/stale_maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 17:08:40.000000 stale_maccarone-0.0.9/src/stale_maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:40.897379 stale_maccarone-0.0.9/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-01 17:08:05.000000 stale_maccarone-0.0.9/support/rename_to_stale.sh
```

### Comparing `stale_maccarone-0.0.8/.github/workflows/publish-to-pypi-stale.yml` & `stale_maccarone-0.0.9/.github/workflows/publish-to-pypi-stale.yml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.8/.github/workflows/publish-to-pypi.yml` & `stale_maccarone-0.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.8/.gitignore` & `stale_maccarone-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.8/LICENSE` & `stale_maccarone-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.8/dev-requirements.txt` & `stale_maccarone-0.0.9/dev-requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -49,15 +49,17 @@
 matplotlib-inline==0.1.6
     # via ipython
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 openai==0.27.7
-    # via maccarone (pyproject.toml)
+    # via
+    #   maccarone (pyproject.toml)
+    #   stale-maccarone
 packaging==23.1
     # via
     #   build
     #   pytest
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
@@ -78,22 +80,27 @@
     # via ipython
 pyproject-hooks==1.0.0
     # via build
 pytest==7.3.1
     # via
     #   maccarone (pyproject.toml)
     #   pytest-asyncio
+    #   stale-maccarone
 pytest-asyncio==0.21.0
-    # via maccarone (pyproject.toml)
+    # via
+    #   maccarone (pyproject.toml)
+    #   stale-maccarone
 requests==2.30.0
     # via openai
 six==1.16.0
     # via asttokens
 stack-data==0.6.2
     # via ipython
+stale-maccarone==0.0.8
+    # via maccarone (pyproject.toml)
 tomli==2.0.1
     # via
     #   build
     #   pyproject-hooks
     #   pytest
 tqdm==4.65.0
     # via openai
```

### Comparing `stale_maccarone-0.0.8/pyproject.toml` & `stale_maccarone-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 "Homepage" = "https://github.com/bsilverthorn/maccarone"
 "Repository" = "https://github.com/bsilverthorn/maccarone"
 
 [project.optional-dependencies]
 dev = [
     "ipython",
     "pip-tools",
-    "stale_maccarone==0.0.4",
+    "stale_maccarone==0.0.8",
 ]
 
 [project.scripts]
 stale_maccarone = "stale_maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
```

### Comparing `stale_maccarone-0.0.8/src/stale_maccarone/caching.py` & `stale_maccarone-0.0.9/src/stale_maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.8/src/stale_maccarone/enable.py` & `stale_maccarone-0.0.9/src/stale_maccarone/loader.mn.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import os
-import re
 import sys
 import logging
-import importlib.abc
-import importlib.machinery
 
-from enum import Enum
 from importlib.abc import (
     MetaPathFinder,
     SourceLoader,
 )
 from importlib.machinery import ModuleSpec
+from fnmatch import fnmatchcase
 
 from stale_maccarone.preprocessor import preprocess_maccarone
 
-enable_py_string_matching = True
-fullname_pattern: str | None = None
-
 class ImportFinder(MetaPathFinder):
+    def __init__(
+            self,
+            py_string_matching: bool,
+            include_pattern: str | None,
+            exclude_pattern: str | None,
+        ) -> None:
+        self.py_string_matching = py_string_matching
+        self.include_pattern = include_pattern
+        self.exclude_pattern = exclude_pattern
+
     def find_spec(self, fullname, path, target=None):
-        # check against module name pattern, if configured
-        if fullname_pattern is not None:
-            if re.match(fullname_pattern, fullname) is None:
+        # check against module name patterns, if configured
+        if self.exclude_pattern is not None:
+            if fnmatchcase(fullname, self.exclude_pattern) is not None:
+                return None
+
+        if self.include_pattern is not None:
+            if fnmatchcase(fullname, self.include_pattern) is None:
                 return None
 
         # module name looks ok; check for maccarone snippets
         def make_modulespec(filename):
             return ModuleSpec(
                 fullname,
                 ImportLoader(fullname, filename),
@@ -42,15 +50,15 @@
             package_path = parts[1:-1]
             base_filename = os.path.join(entry, *package_path, basename)
             py_filename = base_filename + '.py'
             mn_filename = base_filename + '.mn.py'
 
             if os.path.exists(mn_filename):
                 return make_modulespec(mn_filename)
-            elif enable_py_string_matching and os.path.exists(py_filename):
+            elif self.py_string_matching and os.path.exists(py_filename):
                 with open(py_filename, "rt") as file:
                     if "#<<" in file.read():
                         return make_modulespec(py_filename)
 
         return None  # we don't know how to import this
 
 class ImportLoader(SourceLoader):
@@ -63,11 +71,24 @@
 
     def get_data(self, filename):
         with open(self.path, 'r') as file:
             in_source = file.read()
 
         return preprocess_maccarone(in_source)
 
-sys.meta_path.insert(0, ImportFinder())
+def enable(
+        py_string_matching=True,
+        include_pattern=None,
+        exclude_pattern=None,
+    ):
+    """Exclude patterns take precedence over include patterns."""
+
+    import_finder = ImportFinder(
+        py_string_matching=py_string_matching,
+        include_pattern=include_pattern,
+        exclude_pattern=exclude_pattern,
+    )
+
+    sys.meta_path.insert(0, import_finder)
 
-if os.environ.get("MACCARONE_LOGGING", False):
-    logging.basicConfig(level=logging.DEBUG)
+    if os.environ.get("MACCARONE_LOGGING", False):
+        logging.basicConfig(level=logging.DEBUG)
```

### Comparing `stale_maccarone-0.0.8/src/stale_maccarone/openai.py` & `stale_maccarone-0.0.9/src/stale_maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.8/src/stale_maccarone/preprocessor.py` & `stale_maccarone-0.0.9/src/stale_maccarone/preprocessor.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,29 +57,41 @@
 
     logger.debug("tagged input ↓\n%s", tag_source)
 
     return tag_source
 
 def tagged_input_to_tagged_output(tagged_input: str) -> str:
     system_prompt = """
-You are an expert programmer working on contract. Your client has written a partial program, but left pieces for you to complete. They have marked those with `<write_this>` tags inside Python comments, e.g.
+You are an expert programmer working on contract. Your client has written a partial program, but left pieces for you to complete. They have marked those with `<write_this>` tags inside Python comments, e.g.:
 
 ```
 def add_two_numbers(x, y):
     # <write_this id="0">
     # add the two numbers
     # </>
+
+# <write_this id="1">
+# add two numbers from command line args, using argparse
+# </>
 ```
 
-which should result in:
+You should produce a document that provides a `<completed>` tag for each missing piece, e.g.:
 
 ```
 <completed id="0">
 return x + y
 </>
+<completed id="1">
+import argparse
+parser = argparse.ArgumentParser()
+parser.add_argument("x", type=int)
+parser.add_argument("y", type=int)
+args = parser.parse_args()
+return add_two_numbers(args.x, args.y)
+</>
 ```
 
 This formatting is very important. The client uses a custom tool to process your work product, and their tool requires this format. Follow this format exactly and do not copy anything outside a `<write_this>` tag.
 """
     chat_messages = [
         {"role": "system", "content": system_prompt},
         {"role": "user", "content": tagged_input},
```

### Comparing `stale_maccarone-0.0.8/src/stale_maccarone/scripts/preprocess.mn.py` & `stale_maccarone-0.0.9/src/stale_maccarone/scripts/preprocess.mn.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,17 +29,15 @@
 def main(root_path: str):
     """Preprocess maccarone files into Python."""
 
     for path in glob.glob(root_path + "/**/*.mn.py", recursive=True):
         preprocess(path)
 
 def parse_args() -> Namespace:
-    #<<
-    # use argparse to support `script ROOT_PATH`
-    #>>
+    #<<use argparse to handle `script ROOT_PATH`>>
 
 def script_main():
     logging.basicConfig(level=logging.INFO)
 
     return main(**vars(parse_args()))
 
 if __name__ == "__main__":
```

### Comparing `stale_maccarone-0.0.8/src/stale_maccarone/scripts/preprocess.py` & `stale_maccarone-0.0.9/src/stale_maccarone/scripts/preprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,17 +30,16 @@
     """Preprocess maccarone files into Python."""
 
     for path in glob.glob(root_path + "/**/*.mn.py", recursive=True):
         preprocess(path)
 
 def parse_args() -> Namespace:
     parser = ArgumentParser(description="Preprocess maccarone files into Python.")
-    parser.add_argument("root_path", help="Root path to search for .mn.py files.")
-    args = parser.parse_args()
-    return args
+    parser.add_argument("root_path", help="The root path to search for maccarone files.")
+    return parser.parse_args()
 
 
 def script_main():
     logging.basicConfig(level=logging.INFO)
 
     return main(**vars(parse_args()))
```

### Comparing `stale_maccarone-0.0.8/src/stale_maccarone/test/test_caching.py` & `stale_maccarone-0.0.9/src/stale_maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.8/src/stale_maccarone/test/test_preprocessor.py` & `stale_maccarone-0.0.9/src/stale_maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.8/src/stale_maccarone.egg-info/SOURCES.txt` & `stale_maccarone-0.0.9/src/stale_maccarone.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 .gitignore
 LICENSE
+README.md
 dev-requirements.txt
 local-dev-requirements.txt
 pyproject.toml
 .github/workflows/publish-to-pypi-stale.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/run-pytest.yml
 examples/__init__.py
 examples/add.mn.py
 examples/fizzbuzz.mn.py
 examples/todo.mn.py
 src/stale_maccarone/__init__.py
 src/stale_maccarone/caching.py
-src/stale_maccarone/enable.py
+src/stale_maccarone/loader.mn.py
+src/stale_maccarone/loader.py
 src/stale_maccarone/openai.py
 src/stale_maccarone/preprocessor.py
 src/stale_maccarone.egg-info/PKG-INFO
 src/stale_maccarone.egg-info/SOURCES.txt
 src/stale_maccarone.egg-info/dependency_links.txt
 src/stale_maccarone.egg-info/entry_points.txt
 src/stale_maccarone.egg-info/requires.txt
```

### Comparing `stale_maccarone-0.0.8/support/rename_to_stale.sh` & `stale_maccarone-0.0.9/support/rename_to_stale.sh`

 * *Files identical despite different names*

