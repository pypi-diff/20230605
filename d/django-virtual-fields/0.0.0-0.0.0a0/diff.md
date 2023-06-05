# Comparing `tmp/django_virtual_fields-0.0.0.tar.gz` & `tmp/django_virtual_fields-0.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_virtual_fields-0.0.0.tar", max compression
+gzip compressed data, was "django_virtual_fields-0.0.0a0.tar", max compression
```

## Comparing `django_virtual_fields-0.0.0.tar` & `django_virtual_fields-0.0.0a0.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0     2028 2023-06-05 04:30:49.281789 django_virtual_fields-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 04:30:49.281789 django_virtual_fields-0.0.0/virtual_fields/__init__.py
--rw-r--r--   0        0        0      102 2023-06-05 04:30:49.281789 django_virtual_fields-0.0.0/virtual_fields/apps.py
--rw-r--r--   0        0        0      106 2023-06-05 04:30:49.281789 django_virtual_fields-0.0.0/virtual_fields/models/__init__.py
--rw-r--r--   0        0        0      160 2023-06-05 04:30:49.281789 django_virtual_fields-0.0.0/virtual_fields/models/__init__.pyi
--rw-r--r--   0        0        0     2034 2023-06-05 04:30:49.281789 django_virtual_fields-0.0.0/virtual_fields/models/_compat.py
--rw-r--r--   0        0        0     8464 2023-06-05 04:30:49.281789 django_virtual_fields-0.0.0/virtual_fields/models/fields.py
--rw-r--r--   0        0        0      452 2023-06-05 04:30:49.281789 django_virtual_fields-0.0.0/virtual_fields/testing.py
--rw-r--r--   0        0        0      569 2023-06-05 04:30:49.281789 django_virtual_fields-0.0.0/virtual_fields/utils.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 django_virtual_fields-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1940 2023-05-07 03:46:27.106727 django_virtual_fields-0.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 02:29:50.554439 django_virtual_fields-0.0.0a0/virtual_fields/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-07 03:38:06.810711 django_virtual_fields-0.0.0a0/virtual_fields/apps.py
+-rw-r--r--   0        0        0      569 2023-05-07 03:36:01.336635 django_virtual_fields-0.0.0a0/virtual_fields/utils.py
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 django_virtual_fields-0.0.0a0/setup.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 django_virtual_fields-0.0.0a0/PKG-INFO
```

### Comparing `django_virtual_fields-0.0.0/pyproject.toml` & `django_virtual_fields-0.0.0a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Django-Virtual-Fields"
-version = "0.0.0"
+version = "0.0.0a0"
 description = "Virtual `django` fields."
 authors = ["David Kyalo <davidmkyalo@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
@@ -33,15 +33,14 @@
 [tool.poetry.group.dev.dependencies]
 black = "*"
 ipython = "^8.10.0"
 django-polymorphic = "^3.1.0"
 tox = "^4.4.8"
 psycopg = "^3.1.8"
 mysqlclient = "^2.1.1"
-django-debug-toolbar = "^4.1.0"
 
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
@@ -67,23 +66,22 @@
 
 [tool.mypy]
 python_version = "3.10"
 ignore_missing_imports = "True"
 
 
 [tool.pytest.ini_options]
-addopts = "--reuse-db --showlocals --cov=virtual_fields --cov-report html --cov-config pyproject.toml"
+addopts = "--showlocals --cov=virtual_fields --cov-report html --cov-config pyproject.toml"
 asyncio_mode="auto"
 xfail_strict= "True"
 log_level = "DEBUG"
 python_files = "tests.py test.py test_*.py"
 python_classes = "test_* Test_*"
 python_functions = "test_* test"
-# DJANGO_SETTINGS_MODULE = "tests.app.settings"
-DJANGO_SETTINGS_MODULE = "examples.settings"
+DJANGO_SETTINGS_MODULE = "tests.app.settings"
 
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "^\\s*pass\\s*$",
     "^\\s*\\.\\.\\.\\s*$",
```

### Comparing `django_virtual_fields-0.0.0/virtual_fields/utils.py` & `django_virtual_fields-0.0.0a0/virtual_fields/utils.py`

 * *Files identical despite different names*

### Comparing `django_virtual_fields-0.0.0/PKG-INFO` & `django_virtual_fields-0.0.0a0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: django-virtual-fields
-Version: 0.0.0
+Version: 0.0.0a0
 Summary: Virtual `django` fields.
 License: MIT
 Author: David Kyalo
 Author-email: davidmkyalo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=3.2.0)
 Requires-Dist: typing-extensions (>=4.4.0)
 Requires-Dist: zana (>=0.2.0a4,<0.3.0)
```

