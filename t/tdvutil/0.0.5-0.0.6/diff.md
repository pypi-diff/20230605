# Comparing `tmp/tdvutil-0.0.5.tar.gz` & `tmp/tdvutil-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdvutil-0.0.5.tar", last modified: Tue Dec  6 19:54:51 2022, max compression
+gzip compressed data, was "tdvutil-0.0.6.tar", last modified: Mon Jun  5 20:26:38 2023, max compression
```

## Comparing `tdvutil-0.0.5.tar` & `tdvutil-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2022-12-06 19:54:51.740591 tdvutil-0.0.5/
--rw-r--r--   0 jg         (502) _lpoperator   (100)     1283 2022-09-16 20:02:50.000000 tdvutil-0.0.5/.gitignore
--rw-r--r--   0 jg         (502) _lpoperator   (100)      996 2022-09-16 20:02:50.000000 tdvutil-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 jg         (502) _lpoperator   (100)    35149 2022-09-16 20:02:50.000000 tdvutil-0.0.5/LICENSE.txt
--rw-r--r--   0 jg         (502) _lpoperator   (100)     1227 2022-09-16 20:02:50.000000 tdvutil-0.0.5/Makefile
--rw-r--r--   0 jg         (502) _lpoperator   (100)    41276 2022-12-06 19:54:51.741083 tdvutil-0.0.5/PKG-INFO
--rw-r--r--   0 jg         (502) _lpoperator   (100)        0 2022-09-16 20:02:50.000000 tdvutil-0.0.5/README.md
-drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2022-12-06 19:54:51.733039 tdvutil-0.0.5/docs/
--rw-r--r--   0 jg         (502) _lpoperator   (100)     1154 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/Makefile
-drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2022-12-06 19:54:51.733403 tdvutil-0.0.5/docs/_static/
--rw-r--r--   0 jg         (502) _lpoperator   (100)       18 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/_static/.gitignore
-drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2022-12-06 19:54:51.734070 tdvutil-0.0.5/docs/api/
--rw-r--r--   0 jg         (502) _lpoperator   (100)       58 2022-09-16 20:10:36.000000 tdvutil-0.0.5/docs/api/modules.rst
--rw-r--r--   0 jg         (502) _lpoperator   (100)      144 2022-09-16 20:10:36.000000 tdvutil-0.0.5/docs/api/tdvutil.rst
--rw-r--r--   0 jg         (502) _lpoperator   (100)      130 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/authors.rst
--rw-r--r--   0 jg         (502) _lpoperator   (100)      151 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/changelog.rst
--rw-r--r--   0 jg         (502) _lpoperator   (100)     9797 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/conf.py
--rw-r--r--   0 jg         (502) _lpoperator   (100)     9728 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/conf.py.orig
--rw-r--r--   0 jg         (502) _lpoperator   (100)     2274 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/index.rst
--rw-r--r--   0 jg         (502) _lpoperator   (100)       74 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/license.rst
--rw-r--r--   0 jg         (502) _lpoperator   (100)     1557 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/readme.rst
--rw-r--r--   0 jg         (502) _lpoperator   (100)      250 2022-09-16 20:02:50.000000 tdvutil-0.0.5/docs/requirements.txt
--rw-r--r--   0 jg         (502) _lpoperator   (100)     2264 2022-12-06 19:52:31.000000 tdvutil-0.0.5/pyproject.toml
--rw-r--r--   0 jg         (502) _lpoperator   (100)       38 2022-12-06 19:54:51.741732 tdvutil-0.0.5/setup.cfg
-drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2022-12-06 19:54:51.726398 tdvutil-0.0.5/src/
-drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2022-12-06 19:54:51.737765 tdvutil-0.0.5/src/_tdvutil/
--rw-r--r--   0 jg         (502) _lpoperator   (100)      129 2022-09-16 20:02:50.000000 tdvutil-0.0.5/src/_tdvutil/__init__.py
--rw-r--r--   0 jg         (502) _lpoperator   (100)      176 2022-12-06 19:54:51.000000 tdvutil-0.0.5/src/_tdvutil/_version.py
--rw-r--r--   0 jg         (502) _lpoperator   (100)     7442 2022-09-16 20:02:50.000000 tdvutil-0.0.5/src/_tdvutil/alintrospect.py
--rw-r--r--   0 jg         (502) _lpoperator   (100)     1663 2022-09-16 22:45:04.000000 tdvutil-0.0.5/src/_tdvutil/argparse.py
--rw-r--r--   0 jg         (502) _lpoperator   (100)      415 2022-11-30 22:36:03.000000 tdvutil-0.0.5/src/_tdvutil/now.py
--rw-r--r--   0 jg         (502) _lpoperator   (100)     2357 2022-09-16 20:02:50.000000 tdvutil-0.0.5/src/_tdvutil/pathfix.py
--rw-r--r--   0 jg         (502) _lpoperator   (100)    10233 2022-09-16 20:02:50.000000 tdvutil-0.0.5/src/_tdvutil/ppretty.py
--rw-r--r--   0 jg         (502) _lpoperator   (100)     1084 2022-09-16 20:02:50.000000 tdvutil-0.0.5/src/_tdvutil/ppretty.pyi
--rw-r--r--   0 jg         (502) _lpoperator   (100)        0 2022-09-16 20:02:50.000000 tdvutil-0.0.5/src/_tdvutil/py.typed
--rw-r--r--   0 jg         (502) _lpoperator   (100)     2514 2022-12-06 19:53:23.000000 tdvutil-0.0.5/src/_tdvutil/timefmt.py
-drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2022-12-06 19:54:51.738414 tdvutil-0.0.5/src/tdvutil/
--rw-r--r--   0 jg         (502) _lpoperator   (100)      446 2022-12-06 19:45:54.000000 tdvutil-0.0.5/src/tdvutil/__init__.py
-drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2022-12-06 19:54:51.740280 tdvutil-0.0.5/src/tdvutil/argparse/
--rw-r--r--   0 jg         (502) _lpoperator   (100)      106 2022-09-16 22:42:40.000000 tdvutil-0.0.5/src/tdvutil/argparse/__init__.py
--rw-r--r--   0 jg         (502) _lpoperator   (100)        0 2022-09-16 20:02:50.000000 tdvutil-0.0.5/src/tdvutil/py.typed
-drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2022-12-06 19:54:51.739869 tdvutil-0.0.5/src/tdvutil.egg-info/
--rw-r--r--   0 jg         (502) _lpoperator   (100)    41276 2022-12-06 19:54:51.000000 tdvutil-0.0.5/src/tdvutil.egg-info/PKG-INFO
--rw-r--r--   0 jg         (502) _lpoperator   (100)      768 2022-12-06 19:54:51.000000 tdvutil-0.0.5/src/tdvutil.egg-info/SOURCES.txt
--rw-r--r--   0 jg         (502) _lpoperator   (100)        1 2022-12-06 19:54:51.000000 tdvutil-0.0.5/src/tdvutil.egg-info/dependency_links.txt
--rw-r--r--   0 jg         (502) _lpoperator   (100)       17 2022-12-06 19:54:51.000000 tdvutil-0.0.5/src/tdvutil.egg-info/top_level.txt
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.369832 tdvutil-0.0.6/
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     1283 2022-09-16 20:02:50.000000 tdvutil-0.0.6/.gitignore
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      996 2022-09-16 20:02:50.000000 tdvutil-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 jg         (502) _lpoperator   (100)    35149 2022-09-16 20:02:50.000000 tdvutil-0.0.6/LICENSE.txt
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     1255 2023-05-30 21:40:41.000000 tdvutil-0.0.6/Makefile
+-rw-r--r--   0 jg         (502) _lpoperator   (100)    41298 2023-06-05 20:26:38.370278 tdvutil-0.0.6/PKG-INFO
+-rw-r--r--   0 jg         (502) _lpoperator   (100)        0 2022-09-16 20:02:50.000000 tdvutil-0.0.6/README.md
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      408 2023-05-30 20:42:47.000000 tdvutil-0.0.6/conftest.py
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.363736 tdvutil-0.0.6/docs/
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     1154 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/Makefile
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.364016 tdvutil-0.0.6/docs/_static/
+-rw-r--r--   0 jg         (502) _lpoperator   (100)       18 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/_static/.gitignore
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.364547 tdvutil-0.0.6/docs/api/
+-rw-r--r--   0 jg         (502) _lpoperator   (100)       58 2022-09-16 20:10:36.000000 tdvutil-0.0.6/docs/api/modules.rst
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      144 2022-09-16 20:10:36.000000 tdvutil-0.0.6/docs/api/tdvutil.rst
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      130 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/authors.rst
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      151 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/changelog.rst
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     9797 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/conf.py
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     9728 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/conf.py.orig
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     2274 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/index.rst
+-rw-r--r--   0 jg         (502) _lpoperator   (100)       74 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/license.rst
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     1557 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/readme.rst
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      250 2022-09-16 20:02:50.000000 tdvutil-0.0.6/docs/requirements.txt
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     3409 2023-05-30 21:39:24.000000 tdvutil-0.0.6/pyproject.toml
+-rw-r--r--   0 jg         (502) _lpoperator   (100)       38 2023-06-05 20:26:38.370824 tdvutil-0.0.6/setup.cfg
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.358310 tdvutil-0.0.6/src/
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.367141 tdvutil-0.0.6/src/_tdvutil/
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      129 2022-09-16 20:02:50.000000 tdvutil-0.0.6/src/_tdvutil/__init__.py
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      176 2023-06-05 20:26:37.000000 tdvutil-0.0.6/src/_tdvutil/_version.py
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     7442 2022-09-16 20:02:50.000000 tdvutil-0.0.6/src/_tdvutil/alintrospect.py
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     1663 2022-09-16 22:45:04.000000 tdvutil-0.0.6/src/_tdvutil/argparse.py
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      415 2022-11-30 22:36:03.000000 tdvutil-0.0.6/src/_tdvutil/now.py
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     2357 2022-09-16 20:02:50.000000 tdvutil-0.0.6/src/_tdvutil/pathfix.py
+-rw-r--r--   0 jg         (502) _lpoperator   (100)    10233 2022-09-16 20:02:50.000000 tdvutil-0.0.6/src/_tdvutil/ppretty.py
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     1084 2022-09-16 20:02:50.000000 tdvutil-0.0.6/src/_tdvutil/ppretty.pyi
+-rw-r--r--   0 jg         (502) _lpoperator   (100)        0 2022-09-16 20:02:50.000000 tdvutil-0.0.6/src/_tdvutil/py.typed
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     2581 2023-05-30 21:38:55.000000 tdvutil-0.0.6/src/_tdvutil/timefmt.py
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.367644 tdvutil-0.0.6/src/tdvutil/
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      446 2022-12-06 19:45:54.000000 tdvutil-0.0.6/src/tdvutil/__init__.py
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.369285 tdvutil-0.0.6/src/tdvutil/argparse/
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      106 2022-09-16 22:42:40.000000 tdvutil-0.0.6/src/tdvutil/argparse/__init__.py
+-rw-r--r--   0 jg         (502) _lpoperator   (100)        0 2022-09-16 20:02:50.000000 tdvutil-0.0.6/src/tdvutil/py.typed
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.368972 tdvutil-0.0.6/src/tdvutil.egg-info/
+-rw-r--r--   0 jg         (502) _lpoperator   (100)    41298 2023-06-05 20:26:38.000000 tdvutil-0.0.6/src/tdvutil.egg-info/PKG-INFO
+-rw-r--r--   0 jg         (502) _lpoperator   (100)      836 2023-06-05 20:26:38.000000 tdvutil-0.0.6/src/tdvutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jg         (502) _lpoperator   (100)        1 2023-06-05 20:26:38.000000 tdvutil-0.0.6/src/tdvutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jg         (502) _lpoperator   (100)       32 2023-06-05 20:26:38.000000 tdvutil-0.0.6/src/tdvutil.egg-info/requires.txt
+-rw-r--r--   0 jg         (502) _lpoperator   (100)       17 2023-06-05 20:26:38.000000 tdvutil-0.0.6/src/tdvutil.egg-info/top_level.txt
+drwxr-xr-x   0 jg         (502) _lpoperator   (100)        0 2023-06-05 20:26:38.369586 tdvutil-0.0.6/tests/
+-rw-r--r--   0 jg         (502) _lpoperator   (100)     1222 2023-05-30 21:41:54.000000 tdvutil-0.0.6/tests/test_timefmt.py
```

### Comparing `tdvutil-0.0.5/.gitignore` & `tdvutil-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/.pre-commit-config.yaml` & `tdvutil-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/LICENSE.txt` & `tdvutil-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/Makefile` & `tdvutil-0.0.6/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
 
 .PHONY: localdev
 localdev:
 	$(PIP_BIN) install --editable .
 
 
+.PHONY: test
+test:
+	@pytest
 # .PHONY: clean
 # clean:
 # 	rm -rf ./$(OUTDIR)/* ./$(WOWDUMP_OUTDIR)/* ./$(DEPS_DIR)/*.*P ./$(DEPS_DIR)/*.d
 
 # .PHONY: realclean
 # realclean: clean
 # 	rm -rf dist build */*.egg-info *.egg-info
```

### Comparing `tdvutil-0.0.5/PKG-INFO` & `tdvutil-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdvutil
-Version: 0.0.5
+Version: 0.0.6
 Summary: A few simple helper classes used by TDV Alinsa
 Author-email: TDV Alinsa <alinsa-github@lupine.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,8 +684,9 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE.txt
```

### Comparing `tdvutil-0.0.5/docs/Makefile` & `tdvutil-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/docs/conf.py` & `tdvutil-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/docs/conf.py.orig` & `tdvutil-0.0.6/docs/conf.py.orig`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/docs/index.rst` & `tdvutil-0.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/docs/readme.rst` & `tdvutil-0.0.6/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/pyproject.toml` & `tdvutil-0.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -22,20 +22,29 @@
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries",
 ]
 
-dependencies = []
+dependencies = [  ]
 
 # for e.g. "pip install mything[dev]"
 # [project.optional-dependencies]
 # dev = ["check-manifest"]
 
+[project.optional-dependencies]
+tests = [
+    'pytest>=7.0',
+    'pytest-cov',
+    # 'pytest-html',
+    # 'pytest-order',
+    # 'pytest-benchmark[histogram]>=3.2.1',
+    # 'responses',
+]
 
 [project.urls]
 "Homepage" = "https://github.com/alinsavix/python-tdvutil"
 "Bug Reports" = "https://github.com/alinsavix/python-tdvutil/issues"
 "Source" = "https://github.com/alinsavix/python-tdvutil"
 
 
@@ -81,7 +90,47 @@
 disallow_incomplete_defs = true
 check_untyped_defs = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
+
+
+[tool.isort]
+sections = [ "FUTURE", "STDLIB", "FIRSTPARTY", "THIRDPARTY", "LOCALFOLDER" ]
+
+
+[tool.pytest.ini_options]
+log_cli = true
+
+addopts = [
+    "--tb=short",
+    "--strict-markers",
+    # "--html=@rootdir@/tests/report.html",
+    # "--css=@rootdir@/tests/report.css",
+    # "--self-contained-html",
+    # "--cov=wowdump",
+    # "--cov-report=html:@rootdir@/tests/htmlcov",
+    "--import-mode=importlib",
+
+]
+
+pythonpath = [ "src" ]
+
+console_output_style = "count"
+log_auto_indent = true
+norecursedirs = [ "*" ]
+python_files = [ "test_*.py", "check_*.py", "example_*.py" ]
+testpaths = [ "tests" ]
+
+required_plugins = [
+    # "pytest-html >=3.1",
+    "pytest-cov >=2.12",
+    # "pytest-order >=1.0",
+]
+
+filterwarnings = [
+    # hopefully the pytest folks will give us a better way to do this at
+    # some point so we don't have to use `pytest_cmdline_preparse` at all
+    'ignore:The pytest_cmdline_preparse hook is deprecated:DeprecationWarning',
+]
```

### Comparing `tdvutil-0.0.5/src/_tdvutil/alintrospect.py` & `tdvutil-0.0.6/src/_tdvutil/alintrospect.py`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/src/_tdvutil/argparse.py` & `tdvutil-0.0.6/src/_tdvutil/argparse.py`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/src/_tdvutil/pathfix.py` & `tdvutil-0.0.6/src/_tdvutil/pathfix.py`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/src/_tdvutil/ppretty.py` & `tdvutil-0.0.6/src/_tdvutil/ppretty.py`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/src/_tdvutil/ppretty.pyi` & `tdvutil-0.0.6/src/_tdvutil/ppretty.pyi`

 * *Files identical despite different names*

### Comparing `tdvutil-0.0.5/src/_tdvutil/timefmt.py` & `tdvutil-0.0.6/src/_tdvutil/timefmt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-import time
-
-
 # Convert seconds to HH:MM:SS.SSS format. Sure, this could use strftime
 # or datetime.timedelta, but both of those have their own issues when
 # you want a consistent format involving milliseconds.
-def sec_to_hms(secs: float) -> str:
+def sec_to_hms(secs: float, use_ms: bool = True, use_hours: bool = True) -> str:
     """
     Simple conversion from a time in seconds, to hh:mm:ss.sss format
 
     :param secs: A length of time to convert, in seconds
     :type secs: float
+    :param use_ms: include milliseconds in the output
+    :type use_ms: bool
+    :param use_hours: include hours digits in the output, even if zero
+    :type use_hours: bool
 
-    :return: A string in the format of hh:mm:ss.sss
+    :return: A string in the format of [hh]:mm:ss[.sss]
     :rtype: str
     """
     hours = int(secs // (60 * 60))
     secs %= (60 * 60)
 
     minutes = int(secs // 60)
     secs %= 60
 
     ms = int((secs % 1) * 1000)
     secs = int(secs)
 
-    return f"{hours:02d}:{minutes:02d}:{secs:02d}.{ms:03d}"
+    ms_str = f".{ms:03d}" if use_ms else ""
+    hour_str = f"{hours:02d}:" if (use_hours or hours > 0) else ""
+
+    return f"{hour_str}{minutes:02d}:{secs:02d}{ms_str}"
 
 
 # Convert seconds to a compressed string, e.g. 1h15m6s
 def sec_to_shortstr(secs: float) -> str:
     """
     Simple conversion from a time in seconds, to a compressd string format
 
@@ -77,21 +81,9 @@
         m, s = timesplit
     elif len(timesplit) == 1:
         h = "0"
         m = "0"
         s = timesplit[0]
     else:
         raise ValueError(f"too many fields ({len(timesplit)}) in hh:mm:ss string 'hms'")
-        sys.exit(1)
 
     return (int(h) * 60 * 60) + (int(m) * 60) + float(s)
-
-
-if __name__ == '__main__':
-    sec = 18231
-    hms = sec_to_hms(sec)
-    hms_short = sec_to_shortstr(sec)
-    sec = hms_to_sec(hms)
-
-    print(f"{sec}s -> {hms}")
-    print(f"{sec}s -> {hms_short}")
-    print(f"{hms} -> {sec}s")
```

### Comparing `tdvutil-0.0.5/src/tdvutil.egg-info/PKG-INFO` & `tdvutil-0.0.6/src/tdvutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdvutil
-Version: 0.0.5
+Version: 0.0.6
 Summary: A few simple helper classes used by TDV Alinsa
 Author-email: TDV Alinsa <alinsa-github@lupine.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,8 +684,9 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE.txt
```

