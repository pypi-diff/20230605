# Comparing `tmp/attrbox-0.1.2.tar.gz` & `tmp/attrbox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attrbox-0.1.2.tar", last modified: Thu Jun  1 05:06:42 2023, max compression
+gzip compressed data, was "attrbox-0.1.5.tar", last modified: Mon Jun  5 11:37:03 2023, max compression
```

## Comparing `attrbox-0.1.2.tar` & `attrbox-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.731005 attrbox-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-01 05:06:27.000000 attrbox-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-01 05:06:42.731005 attrbox-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-01 05:06:27.000000 attrbox-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-01 05:06:27.000000 attrbox-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 05:06:42.731005 attrbox-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.727005 attrbox-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.731005 attrbox-0.1.2/src/attrbox/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/attrdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/attrlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-01 05:06:27.000000 attrbox-0.1.2/src/attrbox/jsend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.731005 attrbox-0.1.2/src/attrbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 05:06:42.000000 attrbox-0.1.2/src/attrbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:06:42.731005 attrbox-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-01 05:06:27.000000 attrbox-0.1.2/test/test_attrdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-01 05:06:27.000000 attrbox-0.1.2/test/test_fn_set_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:37:03.840861 attrbox-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-05 11:36:46.000000 attrbox-0.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-05 11:37:03.840861 attrbox-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-05 11:36:46.000000 attrbox-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-05 11:36:46.000000 attrbox-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 11:37:03.840861 attrbox-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:37:03.832860 attrbox-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:37:03.836861 attrbox-0.1.5/src/attrbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-05 11:36:46.000000 attrbox-0.1.5/src/attrbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-05 11:36:46.000000 attrbox-0.1.5/src/attrbox/attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-05 11:36:46.000000 attrbox-0.1.5/src/attrbox/attrlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-05 11:36:46.000000 attrbox-0.1.5/src/attrbox/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-05 11:36:46.000000 attrbox-0.1.5/src/attrbox/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-05 11:36:46.000000 attrbox-0.1.5/src/attrbox/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-05 11:36:46.000000 attrbox-0.1.5/src/attrbox/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 11:36:46.000000 attrbox-0.1.5/src/attrbox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:37:03.840861 attrbox-0.1.5/src/attrbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-05 11:37:03.000000 attrbox-0.1.5/src/attrbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-05 11:37:03.000000 attrbox-0.1.5/src/attrbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:37:03.000000 attrbox-0.1.5/src/attrbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 11:37:03.000000 attrbox-0.1.5/src/attrbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 11:37:03.000000 attrbox-0.1.5/src/attrbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:37:03.840861 attrbox-0.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-05 11:36:46.000000 attrbox-0.1.5/test/test_attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-05 11:36:46.000000 attrbox-0.1.5/test/test_fn_set_path.py
```

### Comparing `attrbox-0.1.2/LICENSE.md` & `attrbox-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `attrbox-0.1.2/PKG-INFO` & `attrbox-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attrbox
-Version: 0.1.2
+Version: 0.1.5
 Summary: Attribute-based data structures.
 Author-email: Metaist LLC <metaist@metaist.com>
 License: MIT
 Project-URL: Homepage, https://github.com/metaist/attrbox
 Project-URL: Documentation, https://metaist.github.io/attrbox/
 Project-URL: Repository, https://github.com/metaist/attrbox.git
 Project-URL: Changelog, https://github.com/metaist/attrbox/blob/main/CHANGELOG.md
@@ -17,14 +17,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # attrbox
```

### Comparing `attrbox-0.1.2/README.md` & `attrbox-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `attrbox-0.1.2/pyproject.toml` & `attrbox-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["setuptools >= 40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools.package-data]
+attrbox = ["py.typed"]
+
 [tool.setuptools.dynamic]
 version = { attr = "attrbox.__version__" }
 
 [project.urls]
 Homepage = "https://github.com/metaist/attrbox"
 Documentation = "https://metaist.github.io/attrbox/"
 Repository = "https://github.com/metaist/attrbox.git"
@@ -18,30 +21,28 @@
 name = "attrbox"
 description = "Attribute-based data structures."
 keywords = ["attr", "attributes", "dict", "list"]
 
 dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
-  "docopt==0.6.2",  # TODO: vendorize
-  "tomli >= 1.1.0", # TODO 2026-10-04 [3.10 EOL]: remove
+  # lib => pinned range
+  "docopt==0.6.2", # TODO: vendorize
+  "tomli>=1.1.0",  # TODO 2026-10-04 [3.10 EOL]: remove
 ]
 optional-dependencies = { dev = [
-  # dev dependencies are latest
+  # dev => latest
   "black",
   "coverage",
   "mypy",
   "pdm",
   "pdoc3",
   "pytest-cov",
   "pytest",
   "ruff",
-
-  # for tests
-  "toml",
 ] }
 readme = "README.md"
 license = { text = "MIT" }
 authors = [{ name = "Metaist LLC", email = "metaist@metaist.com" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -51,14 +52,16 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Topic :: Software Development :: Libraries",
+  "Typing :: Typed",
 ]
 
 [tool.pdm.scripts]
 black = { shell = "black ." }
 ruff = { shell = "ruff ." }
 cspell = { shell = "cspell --gitignore '**/*.{py,txt,md,markdown}'" }
```

### Comparing `attrbox-0.1.2/src/attrbox/__init__.py` & `attrbox-0.1.5/src/attrbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .jsend import JSend
 
 from .env import load_env
 from .config import load_config
 from .config import parse_docopt
 
 
-__version__ = "0.1.2"
+__version__ = "0.1.5"
 __all__ = (
     "__version__",
     "AttrDict",
     "AttrList",
     "JSend",
     "load_env",
     "load_config",
```

### Comparing `attrbox-0.1.2/src/attrbox/attrdict.py` & `attrbox-0.1.5/src/attrbox/attrdict.py`

 * *Files identical despite different names*

### Comparing `attrbox-0.1.2/src/attrbox/attrlist.py` & `attrbox-0.1.5/src/attrbox/attrlist.py`

 * *Files identical despite different names*

### Comparing `attrbox-0.1.2/src/attrbox/config.py` & `attrbox-0.1.5/src/attrbox/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     doc: str,
     /,
     argv: Optional[Sequence[str]] = None,
     *,
     version: str = "1.0.0",
     options_first: bool = False,
     read_config: bool = True,
-) -> Dict[str, Any]:
+) -> AttrDict:
     """Parse docopt args and load config.
 
     Args:
         doc (str): docstring with description of command
 
         argv (Sequence[str], optional): arguments to parse against the
             doc. If `None`, will default to `sys.argv[1:]`. Defaults to `None`.
@@ -223,15 +223,15 @@
         options_first (bool): If `True`, options must come before positional
             arguments. Defaults to `False`.
 
         read_config (bool): If `True`, a `<config>` argument or `--config` option
             will be automatically loaded before args are parsed. Defaults to `True`.
 
     Returns:
-        Dict[str, Any]: mapping of options to values
+        AttrDict[str, Any]: mapping of options to values
 
     Examples:
         >>> usage = "Usage: test.py [--debug]"
         >>> parse_docopt(usage, argv=["--debug"])
         {'debug': True}
 
         >>> root = Path(__file__).parent.parent.parent
```

### Comparing `attrbox-0.1.2/src/attrbox/env.py` & `attrbox-0.1.5/src/attrbox/env.py`

 * *Files identical despite different names*

### Comparing `attrbox-0.1.2/src/attrbox/fn.py` & `attrbox-0.1.5/src/attrbox/fn.py`

 * *Files identical despite different names*

### Comparing `attrbox-0.1.2/src/attrbox/jsend.py` & `attrbox-0.1.5/src/attrbox/jsend.py`

 * *Files identical despite different names*

### Comparing `attrbox-0.1.2/src/attrbox.egg-info/PKG-INFO` & `attrbox-0.1.5/src/attrbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attrbox
-Version: 0.1.2
+Version: 0.1.5
 Summary: Attribute-based data structures.
 Author-email: Metaist LLC <metaist@metaist.com>
 License: MIT
 Project-URL: Homepage, https://github.com/metaist/attrbox
 Project-URL: Documentation, https://metaist.github.io/attrbox/
 Project-URL: Repository, https://github.com/metaist/attrbox.git
 Project-URL: Changelog, https://github.com/metaist/attrbox/blob/main/CHANGELOG.md
@@ -17,14 +17,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # attrbox
```

### Comparing `attrbox-0.1.2/test/test_attrdict.py` & `attrbox-0.1.5/test/test_attrdict.py`

 * *Files identical despite different names*

### Comparing `attrbox-0.1.2/test/test_fn_set_path.py` & `attrbox-0.1.5/test/test_fn_set_path.py`

 * *Files identical despite different names*

