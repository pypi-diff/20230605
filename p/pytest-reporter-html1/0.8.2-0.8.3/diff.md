# Comparing `tmp/pytest-reporter-html1-0.8.2.tar.gz` & `tmp/pytest-reporter-html1-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reporter-html1-0.8.2.tar", last modified: Tue Jun  8 18:09:43 2021, max compression
+gzip compressed data, was "/Users/crille/Projects/pytest-reporter-project/pytest-reporter-html1/dist/.tmp-dx59qs4l/pytest-reporter-html1-0.8.3.tar", last modified: Mon Jun  5 08:37:36 2023, max compression
```

## Comparing `pytest-reporter-html1-0.8.2.tar` & `pytest-reporter-html1-0.8.3.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.402249 pytest-reporter-html1-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (121)      865 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      911 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4894 2021-06-08 18:09:43.402249 pytest-reporter-html1-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3286 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/pytest_reporter_html1/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6338 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/icons/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/icons/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/icons/nok.svg
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/icons/ok.svg
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/icons/skip.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      984 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/module.html
--rw-r--r--   0 runner    (1001) docker     (121)     6138 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/normalize.css
--rw-r--r--   0 runner    (1001) docker     (121)     7584 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/style.css
--rw-r--r--   0 runner    (1001) docker     (121)     3791 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/test.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/pytest_reporter_html1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4894 2021-06-08 18:09:43.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2021-06-08 18:09:43.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-08 18:09:43.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-06-08 18:09:43.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-06-08 18:09:43.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-06-08 18:09:43.000000 pytest-reporter-html1-0.8.2/pytest_reporter_html1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    79876 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-08 18:09:43.402249 pytest-reporter-html1-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/tests/report/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/report/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 18:09:43.398249 pytest-reporter-html1-0.8.2/tests/samples/
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/samples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/samples/sample_capturing.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/samples/sample_class.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/samples/sample_extra.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/samples/sample_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/samples/sample_reruns.py
--rw-r--r--   0 runner    (1001) docker     (121)      892 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/samples/sample_test_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/samples/sample_unittest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-06-08 18:09:35.000000 pytest-reporter-html1-0.8.2/tox.ini
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.382317 pytest-reporter-html1-0.8.3/
+-rw-r--r--   0 crille     (501) staff       (20)       18 2020-05-14 22:30:22.000000 pytest-reporter-html1-0.8.3/.gitattributes
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.262433 pytest-reporter-html1-0.8.3/.github/
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.284948 pytest-reporter-html1-0.8.3/.github/workflows/
+-rw-r--r--   0 crille     (501) staff       (20)     1265 2020-08-02 18:30:25.000000 pytest-reporter-html1-0.8.3/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 crille     (501) staff       (20)      865 2020-05-14 22:35:45.000000 pytest-reporter-html1-0.8.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 crille     (501) staff       (20)      911 2020-04-20 18:40:32.000000 pytest-reporter-html1-0.8.3/.gitignore
+-rw-r--r--   0 crille     (501) staff       (20)     1086 2020-04-20 18:40:42.000000 pytest-reporter-html1-0.8.3/LICENSE
+-rw-r--r--   0 crille     (501) staff       (20)      141 2020-05-14 22:30:22.000000 pytest-reporter-html1-0.8.3/MANIFEST.in
+-rw-r--r--   0 crille     (501) staff       (20)     4037 2023-06-05 08:37:36.381423 pytest-reporter-html1-0.8.3/PKG-INFO
+-rw-r--r--   0 crille     (501) staff       (20)     3286 2020-08-17 18:04:37.000000 pytest-reporter-html1-0.8.3/README.rst
+-rw-r--r--   0 crille     (501) staff       (20)      100 2021-06-08 18:01:01.000000 pytest-reporter-html1-0.8.3/pyproject.toml
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.293573 pytest-reporter-html1-0.8.3/pytest_reporter_html1/
+-rw-r--r--   0 crille     (501) staff       (20)      282 2020-05-14 22:35:45.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/__init__.py
+-rw-r--r--   0 crille     (501) staff       (20)     6565 2023-06-05 08:19:03.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/plugin.py
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.263313 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.321991 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/
+-rw-r--r--   0 crille     (501) staff       (20)     1049 2020-08-17 18:04:37.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/base.html
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.346979 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/icons/
+-rw-r--r--   0 crille     (501) staff       (20)      177 2020-07-12 14:30:04.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/icons/arrow.svg
+-rw-r--r--   0 crille     (501) staff       (20)      266 2020-07-12 12:50:53.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/icons/nok.svg
+-rw-r--r--   0 crille     (501) staff       (20)      177 2020-07-12 14:30:04.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/icons/ok.svg
+-rw-r--r--   0 crille     (501) staff       (20)      168 2020-08-17 18:04:37.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/icons/skip.svg
+-rw-r--r--   0 crille     (501) staff       (20)     4798 2023-06-05 08:19:30.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/index.html
+-rw-r--r--   0 crille     (501) staff       (20)      984 2020-08-17 18:04:37.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/module.html
+-rw-r--r--   0 crille     (501) staff       (20)     6138 2020-05-19 17:39:35.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/normalize.css
+-rw-r--r--   0 crille     (501) staff       (20)     7584 2023-06-05 07:58:18.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/style.css
+-rw-r--r--   0 crille     (501) staff       (20)     3791 2021-02-04 19:50:34.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/test.html
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.305776 pytest-reporter-html1-0.8.3/pytest_reporter_html1.egg-info/
+-rw-r--r--   0 crille     (501) staff       (20)     4037 2023-06-05 08:37:36.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1.egg-info/PKG-INFO
+-rw-r--r--   0 crille     (501) staff       (20)     1349 2023-06-05 08:37:36.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1.egg-info/SOURCES.txt
+-rw-r--r--   0 crille     (501) staff       (20)        1 2023-06-05 08:37:36.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1.egg-info/dependency_links.txt
+-rw-r--r--   0 crille     (501) staff       (20)       57 2023-06-05 08:37:36.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1.egg-info/entry_points.txt
+-rw-r--r--   0 crille     (501) staff       (20)       64 2023-06-05 08:37:36.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1.egg-info/requires.txt
+-rw-r--r--   0 crille     (501) staff       (20)       22 2023-06-05 08:37:36.000000 pytest-reporter-html1-0.8.3/pytest_reporter_html1.egg-info/top_level.txt
+-rw-r--r--   0 crille     (501) staff       (20)       72 2023-06-05 07:58:18.000000 pytest-reporter-html1-0.8.3/requirements.txt
+-rw-r--r--   0 crille     (501) staff       (20)    79876 2020-08-02 18:34:35.000000 pytest-reporter-html1-0.8.3/screenshot.png
+-rw-r--r--   0 crille     (501) staff       (20)       38 2023-06-05 08:37:36.382562 pytest-reporter-html1-0.8.3/setup.cfg
+-rw-r--r--   0 crille     (501) staff       (20)     1530 2020-08-17 18:04:37.000000 pytest-reporter-html1-0.8.3/setup.py
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.350552 pytest-reporter-html1-0.8.3/tests/
+-rw-r--r--   0 crille     (501) staff       (20)       34 2020-05-14 22:35:45.000000 pytest-reporter-html1-0.8.3/tests/pytest.ini
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.353808 pytest-reporter-html1-0.8.3/tests/report/
+-rw-r--r--   0 crille     (501) staff       (20)        2 2020-05-14 22:35:45.000000 pytest-reporter-html1-0.8.3/tests/report/.gitignore
+drwxr-xr-x   0 crille     (501) staff       (20)        0 2023-06-05 08:37:36.380015 pytest-reporter-html1-0.8.3/tests/samples/
+-rw-r--r--   0 crille     (501) staff       (20)     1349 2020-07-15 12:08:25.000000 pytest-reporter-html1-0.8.3/tests/samples/conftest.py
+-rw-r--r--   0 crille     (501) staff       (20)      386 2020-07-12 12:50:53.000000 pytest-reporter-html1-0.8.3/tests/samples/sample_capturing.py
+-rw-r--r--   0 crille     (501) staff       (20)       62 2020-07-12 12:50:53.000000 pytest-reporter-html1-0.8.3/tests/samples/sample_class.py
+-rw-r--r--   0 crille     (501) staff       (20)       78 2020-07-15 10:59:06.000000 pytest-reporter-html1-0.8.3/tests/samples/sample_extra.py
+-rw-r--r--   0 crille     (501) staff       (20)      424 2020-08-11 19:47:01.000000 pytest-reporter-html1-0.8.3/tests/samples/sample_outcomes.py
+-rw-r--r--   0 crille     (501) staff       (20)      156 2020-07-12 13:09:48.000000 pytest-reporter-html1-0.8.3/tests/samples/sample_reruns.py
+-rw-r--r--   0 crille     (501) staff       (20)      892 2021-02-04 19:49:47.000000 pytest-reporter-html1-0.8.3/tests/samples/sample_test_info.py
+-rw-r--r--   0 crille     (501) staff       (20)      370 2023-06-05 07:58:18.000000 pytest-reporter-html1-0.8.3/tests/samples/sample_unittest.py
+-rw-r--r--   0 crille     (501) staff       (20)     1253 2021-02-04 19:49:47.000000 pytest-reporter-html1-0.8.3/tests/test_samples.py
+-rw-r--r--   0 crille     (501) staff       (20)      277 2020-08-02 16:46:33.000000 pytest-reporter-html1-0.8.3/tox.ini
```

### Comparing `pytest-reporter-html1-0.8.2/.github/workflows/pythonpackage.yml` & `pytest-reporter-html1-0.8.3/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/.github/workflows/pythonpublish.yml` & `pytest-reporter-html1-0.8.3/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/.gitignore` & `pytest-reporter-html1-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/LICENSE` & `pytest-reporter-html1-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/PKG-INFO` & `pytest-reporter-html1-0.8.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-reporter-html1
-Version: 0.8.2
+Version: 0.8.3
 Summary: A basic HTML report template for Pytest
 Home-page: https://github.com/christiansandberg/pytest-reporter-html1
 Author: Christian Sandberg
 Author-email: christiansandberg@me.com
 Maintainer: Christian Sandberg
 Maintainer-email: christiansandberg@me.com
 License: MIT
-Description: =====================
-        pytest-reporter-html1
-        =====================
-        
-        .. image:: https://img.shields.io/pypi/v/pytest-reporter-html1.svg
-            :target: https://pypi.org/project/pytest-reporter-html1
-            :alt: PyPI version
-        
-        A basic HTML report for `pytest`_ using `Jinja2`_ template engine.
-        Based on `pytest-reporter`_ which provides the data to the template.
-        
-        
-        Features
-        --------
-        
-        * Overview of files, tests, and phases with expandable sections
-        * Includes information about tests such as documentation, markers, and fixtures
-        * Fairly mobile friendly
-        * Complies with Jenkins default CSP policy (with ``--split-report``)
-        * Support for `pytest-metadata`_ and `pytest-rerunfailures`_
-        * May be used as a base template for customization
-        
-        .. image:: https://raw.githubusercontent.com/christiansandberg/pytest-reporter-html1/master/screenshot.png
-            :alt: Screenshot
-        
-        
-        Installation
-        ------------
-        
-        You can install "pytest-reporter-html1" via `pip`_ from `PyPI`_::
-        
-            $ pip install pytest-reporter-html1
-        
-        
-        Usage
-        -----
-        
-        Specify the html1 template and the output path of the report::
-        
-            $ pytest --template=html1/index.html --report=report.html
-        
-        By default the report is self-contained, but you can separate CSS, images,
-        and JavaScript by specifying the ``--split-report`` option.
-        
-        
-        Customization
-        -------------
-        
-        You can inherit this template in your own to tailor parts of it to your own needs.
-        It defines various blocks which you can override using `template inheritance`_.
-        
-        .. code:: html
-        
-            {% extends "html1/index.html" %}
-            {% block style %}
-                {{ super() }}
-                header {
-                    background-color: black;
-                }
-            {% endblock %}
-        
-        Some additional filters are available for templates to use:
-        
-        ``asset(path_or_content, extension)``
-            Takes a path to a local file or a raw bytes object and either returns a
-            base64 encoded URL or a new relative URL to a copy depending on if the
-            report is self-contained or not.
-        
-            .. code:: html
-        
-                <img src="{{ 'path/to/image.png'|asset }}">
-                <img src="{{ raw_byte_data|asset('png') }}">
-        
-        ``ansi(s)``
-            Convert ANSI color codes to HTML.
-        
-        ``strftime(value, format)``
-            Format a Unix timestamp using `datetime.strftime`_.
-        
-            .. code:: html
-        
-                Started: {{ started|strftime('%Y-%m-%d %H:%M:%S') }}
-        
-        ``timedelta(value)``
-            Convert a time in seconds to a `timedelta`_ object.
-        
-        ``rst(s)``
-            Convert reStructuredText to HTML.
-        
-        
-        Issues
-        ------
-        
-        If you encounter any problems, please `file an issue`_ along with a detailed description.
-        
-        .. _`Jinja2`: https://jinja.palletsprojects.com/
-        .. _`template inheritance`: https://jinja.palletsprojects.com/en/master/templates/#template-inheritance
-        .. _`file an issue`: https://github.com/christiansandberg/pytest-reporter-html1/issues
-        .. _`pytest`: https://github.com/pytest-dev/pytest
-        .. _`pytest-reporter`: https://github.com/christiansandberg/pytest-reporter
-        .. _`pytest-metadata`: https://github.com/pytest-dev/pytest-metadata
-        .. _`pytest-rerunfailures`: https://github.com/pytest-dev/pytest-rerunfailures
-        .. _`pip`: https://pypi.org/project/pip/
-        .. _`PyPI`: https://pypi.org/project
-        .. _`datetime.strftime`: https://docs.python.org/3/library/datetime.html#datetime.datetime.strftime
-        .. _`timedelta`: https://docs.python.org/3/library/datetime.html#timedelta-objects
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
+License-File: LICENSE
+
+=====================
+pytest-reporter-html1
+=====================
+
+.. image:: https://img.shields.io/pypi/v/pytest-reporter-html1.svg
+    :target: https://pypi.org/project/pytest-reporter-html1
+    :alt: PyPI version
+
+A basic HTML report for `pytest`_ using `Jinja2`_ template engine.
+Based on `pytest-reporter`_ which provides the data to the template.
+
+
+Features
+--------
+
+* Overview of files, tests, and phases with expandable sections
+* Includes information about tests such as documentation, markers, and fixtures
+* Fairly mobile friendly
+* Complies with Jenkins default CSP policy (with ``--split-report``)
+* Support for `pytest-metadata`_ and `pytest-rerunfailures`_
+* May be used as a base template for customization
+
+.. image:: https://raw.githubusercontent.com/christiansandberg/pytest-reporter-html1/master/screenshot.png
+    :alt: Screenshot
+
+
+Installation
+------------
+
+You can install "pytest-reporter-html1" via `pip`_ from `PyPI`_::
+
+    $ pip install pytest-reporter-html1
+
+
+Usage
+-----
+
+Specify the html1 template and the output path of the report::
+
+    $ pytest --template=html1/index.html --report=report.html
+
+By default the report is self-contained, but you can separate CSS, images,
+and JavaScript by specifying the ``--split-report`` option.
+
+
+Customization
+-------------
+
+You can inherit this template in your own to tailor parts of it to your own needs.
+It defines various blocks which you can override using `template inheritance`_.
+
+.. code:: html
+
+    {% extends "html1/index.html" %}
+    {% block style %}
+        {{ super() }}
+        header {
+            background-color: black;
+        }
+    {% endblock %}
+
+Some additional filters are available for templates to use:
+
+``asset(path_or_content, extension)``
+    Takes a path to a local file or a raw bytes object and either returns a
+    base64 encoded URL or a new relative URL to a copy depending on if the
+    report is self-contained or not.
+
+    .. code:: html
+
+        <img src="{{ 'path/to/image.png'|asset }}">
+        <img src="{{ raw_byte_data|asset('png') }}">
+
+``ansi(s)``
+    Convert ANSI color codes to HTML.
+
+``strftime(value, format)``
+    Format a Unix timestamp using `datetime.strftime`_.
+
+    .. code:: html
+
+        Started: {{ started|strftime('%Y-%m-%d %H:%M:%S') }}
+
+``timedelta(value)``
+    Convert a time in seconds to a `timedelta`_ object.
+
+``rst(s)``
+    Convert reStructuredText to HTML.
+
+
+Issues
+------
+
+If you encounter any problems, please `file an issue`_ along with a detailed description.
+
+.. _`Jinja2`: https://jinja.palletsprojects.com/
+.. _`template inheritance`: https://jinja.palletsprojects.com/en/master/templates/#template-inheritance
+.. _`file an issue`: https://github.com/christiansandberg/pytest-reporter-html1/issues
+.. _`pytest`: https://github.com/pytest-dev/pytest
+.. _`pytest-reporter`: https://github.com/christiansandberg/pytest-reporter
+.. _`pytest-metadata`: https://github.com/pytest-dev/pytest-metadata
+.. _`pytest-rerunfailures`: https://github.com/pytest-dev/pytest-rerunfailures
+.. _`pip`: https://pypi.org/project/pip/
+.. _`PyPI`: https://pypi.org/project
+.. _`datetime.strftime`: https://docs.python.org/3/library/datetime.html#datetime.datetime.strftime
+.. _`timedelta`: https://docs.python.org/3/library/datetime.html#timedelta-objects
```

### Comparing `pytest-reporter-html1-0.8.2/README.rst` & `pytest-reporter-html1-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/pytest_reporter_html1/plugin.py` & `pytest-reporter-html1-0.8.3/pytest_reporter_html1/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,20 @@
         env.filters["rst"] = lambda s: publish_parts(source=s, writer_name="html5")["body"]
         env.filters["css_minify"] = css_minify
         return env
 
     def pytest_reporter_context(self, context, config):
         context.setdefault("colors", COLORS)
         context.setdefault("time_format", "%Y-%m-%d %H:%M:%S")
+        metadata = context.setdefault("metadata", {})
+
+        if config.pluginmanager.getplugin("metadata"):
+            from pytest_metadata.plugin import metadata_key
+
+            metadata.update(config.stash[metadata_key])
 
     def _cssfilter(self, css):
         if self.self_contained:
             return Markup("<style>") + css + Markup("</style>")
         else:
             self._css = css
             return Markup('<link rel="stylesheet" type="text/css" href="style.css">')
```

### Comparing `pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/base.html` & `pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/base.html`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/index.html` & `pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,28 @@
             <td>{{ duration|timedelta }}</td>
           </tr>
         {% endif %}
         <tr>
           <th>Total run time</th>
           <td>{{ tests|map(attribute='phases')|map('sum', 'report.duration')|sum|timedelta }}</td>
         </tr>
-        {% if config._metadata %}
-          {% for key, value in config._metadata.items() %}
-            <tr>
-              <th>{{ key }}</th>
-              <td>
-                {% if value is mapping %}
-                  {% for key, value in value.items() %}
-                    {{ key }}: {{ value }}<br>
-                  {% endfor %}
-                {% else %}
-                  {{ value|urlize }}
-                {% endif %}
-              </td>
-            </tr>
-            {% endfor %}
-        {% endif %}
+        {% for key, value in metadata.items() %}
+          <tr>
+            <th>{{ key }}</th>
+            <td>
+              {% if value is mapping %}
+                {% for key, value in value.items() %}
+                  {{ key }}: {{ value }}<br>
+                {% endfor %}
+              {% else %}
+                {{ value|urlize }}
+              {% endif %}
+            </td>
+          </tr>
+          {% endfor %}
         {% endblock %}
       </table>
     </div>
     <div class="graph">
       {% set tests_by_category = tests|groupby('status.category') %}
       {% set nodes_run = tests|map(attribute='item.nodeid')|list %}
       {% set nof_nodes_not_run = session.items|rejectattr('nodeid', 'in', nodes_run)|list|count %}
```

### Comparing `pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/module.html` & `pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/module.html`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/normalize.css` & `pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/normalize.css`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/style.css` & `pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/style.css`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/pytest_reporter_html1/templates/html1/test.html` & `pytest-reporter-html1-0.8.3/pytest_reporter_html1/templates/html1/test.html`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/pytest_reporter_html1.egg-info/PKG-INFO` & `pytest-reporter-html1-0.8.3/pytest_reporter_html1.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-reporter-html1
-Version: 0.8.2
+Version: 0.8.3
 Summary: A basic HTML report template for Pytest
 Home-page: https://github.com/christiansandberg/pytest-reporter-html1
 Author: Christian Sandberg
 Author-email: christiansandberg@me.com
 Maintainer: Christian Sandberg
 Maintainer-email: christiansandberg@me.com
 License: MIT
-Description: =====================
-        pytest-reporter-html1
-        =====================
-        
-        .. image:: https://img.shields.io/pypi/v/pytest-reporter-html1.svg
-            :target: https://pypi.org/project/pytest-reporter-html1
-            :alt: PyPI version
-        
-        A basic HTML report for `pytest`_ using `Jinja2`_ template engine.
-        Based on `pytest-reporter`_ which provides the data to the template.
-        
-        
-        Features
-        --------
-        
-        * Overview of files, tests, and phases with expandable sections
-        * Includes information about tests such as documentation, markers, and fixtures
-        * Fairly mobile friendly
-        * Complies with Jenkins default CSP policy (with ``--split-report``)
-        * Support for `pytest-metadata`_ and `pytest-rerunfailures`_
-        * May be used as a base template for customization
-        
-        .. image:: https://raw.githubusercontent.com/christiansandberg/pytest-reporter-html1/master/screenshot.png
-            :alt: Screenshot
-        
-        
-        Installation
-        ------------
-        
-        You can install "pytest-reporter-html1" via `pip`_ from `PyPI`_::
-        
-            $ pip install pytest-reporter-html1
-        
-        
-        Usage
-        -----
-        
-        Specify the html1 template and the output path of the report::
-        
-            $ pytest --template=html1/index.html --report=report.html
-        
-        By default the report is self-contained, but you can separate CSS, images,
-        and JavaScript by specifying the ``--split-report`` option.
-        
-        
-        Customization
-        -------------
-        
-        You can inherit this template in your own to tailor parts of it to your own needs.
-        It defines various blocks which you can override using `template inheritance`_.
-        
-        .. code:: html
-        
-            {% extends "html1/index.html" %}
-            {% block style %}
-                {{ super() }}
-                header {
-                    background-color: black;
-                }
-            {% endblock %}
-        
-        Some additional filters are available for templates to use:
-        
-        ``asset(path_or_content, extension)``
-            Takes a path to a local file or a raw bytes object and either returns a
-            base64 encoded URL or a new relative URL to a copy depending on if the
-            report is self-contained or not.
-        
-            .. code:: html
-        
-                <img src="{{ 'path/to/image.png'|asset }}">
-                <img src="{{ raw_byte_data|asset('png') }}">
-        
-        ``ansi(s)``
-            Convert ANSI color codes to HTML.
-        
-        ``strftime(value, format)``
-            Format a Unix timestamp using `datetime.strftime`_.
-        
-            .. code:: html
-        
-                Started: {{ started|strftime('%Y-%m-%d %H:%M:%S') }}
-        
-        ``timedelta(value)``
-            Convert a time in seconds to a `timedelta`_ object.
-        
-        ``rst(s)``
-            Convert reStructuredText to HTML.
-        
-        
-        Issues
-        ------
-        
-        If you encounter any problems, please `file an issue`_ along with a detailed description.
-        
-        .. _`Jinja2`: https://jinja.palletsprojects.com/
-        .. _`template inheritance`: https://jinja.palletsprojects.com/en/master/templates/#template-inheritance
-        .. _`file an issue`: https://github.com/christiansandberg/pytest-reporter-html1/issues
-        .. _`pytest`: https://github.com/pytest-dev/pytest
-        .. _`pytest-reporter`: https://github.com/christiansandberg/pytest-reporter
-        .. _`pytest-metadata`: https://github.com/pytest-dev/pytest-metadata
-        .. _`pytest-rerunfailures`: https://github.com/pytest-dev/pytest-rerunfailures
-        .. _`pip`: https://pypi.org/project/pip/
-        .. _`PyPI`: https://pypi.org/project
-        .. _`datetime.strftime`: https://docs.python.org/3/library/datetime.html#datetime.datetime.strftime
-        .. _`timedelta`: https://docs.python.org/3/library/datetime.html#timedelta-objects
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
+License-File: LICENSE
+
+=====================
+pytest-reporter-html1
+=====================
+
+.. image:: https://img.shields.io/pypi/v/pytest-reporter-html1.svg
+    :target: https://pypi.org/project/pytest-reporter-html1
+    :alt: PyPI version
+
+A basic HTML report for `pytest`_ using `Jinja2`_ template engine.
+Based on `pytest-reporter`_ which provides the data to the template.
+
+
+Features
+--------
+
+* Overview of files, tests, and phases with expandable sections
+* Includes information about tests such as documentation, markers, and fixtures
+* Fairly mobile friendly
+* Complies with Jenkins default CSP policy (with ``--split-report``)
+* Support for `pytest-metadata`_ and `pytest-rerunfailures`_
+* May be used as a base template for customization
+
+.. image:: https://raw.githubusercontent.com/christiansandberg/pytest-reporter-html1/master/screenshot.png
+    :alt: Screenshot
+
+
+Installation
+------------
+
+You can install "pytest-reporter-html1" via `pip`_ from `PyPI`_::
+
+    $ pip install pytest-reporter-html1
+
+
+Usage
+-----
+
+Specify the html1 template and the output path of the report::
+
+    $ pytest --template=html1/index.html --report=report.html
+
+By default the report is self-contained, but you can separate CSS, images,
+and JavaScript by specifying the ``--split-report`` option.
+
+
+Customization
+-------------
+
+You can inherit this template in your own to tailor parts of it to your own needs.
+It defines various blocks which you can override using `template inheritance`_.
+
+.. code:: html
+
+    {% extends "html1/index.html" %}
+    {% block style %}
+        {{ super() }}
+        header {
+            background-color: black;
+        }
+    {% endblock %}
+
+Some additional filters are available for templates to use:
+
+``asset(path_or_content, extension)``
+    Takes a path to a local file or a raw bytes object and either returns a
+    base64 encoded URL or a new relative URL to a copy depending on if the
+    report is self-contained or not.
+
+    .. code:: html
+
+        <img src="{{ 'path/to/image.png'|asset }}">
+        <img src="{{ raw_byte_data|asset('png') }}">
+
+``ansi(s)``
+    Convert ANSI color codes to HTML.
+
+``strftime(value, format)``
+    Format a Unix timestamp using `datetime.strftime`_.
+
+    .. code:: html
+
+        Started: {{ started|strftime('%Y-%m-%d %H:%M:%S') }}
+
+``timedelta(value)``
+    Convert a time in seconds to a `timedelta`_ object.
+
+``rst(s)``
+    Convert reStructuredText to HTML.
+
+
+Issues
+------
+
+If you encounter any problems, please `file an issue`_ along with a detailed description.
+
+.. _`Jinja2`: https://jinja.palletsprojects.com/
+.. _`template inheritance`: https://jinja.palletsprojects.com/en/master/templates/#template-inheritance
+.. _`file an issue`: https://github.com/christiansandberg/pytest-reporter-html1/issues
+.. _`pytest`: https://github.com/pytest-dev/pytest
+.. _`pytest-reporter`: https://github.com/christiansandberg/pytest-reporter
+.. _`pytest-metadata`: https://github.com/pytest-dev/pytest-metadata
+.. _`pytest-rerunfailures`: https://github.com/pytest-dev/pytest-rerunfailures
+.. _`pip`: https://pypi.org/project/pip/
+.. _`PyPI`: https://pypi.org/project
+.. _`datetime.strftime`: https://docs.python.org/3/library/datetime.html#datetime.datetime.strftime
+.. _`timedelta`: https://docs.python.org/3/library/datetime.html#timedelta-objects
```

### Comparing `pytest-reporter-html1-0.8.2/pytest_reporter_html1.egg-info/SOURCES.txt` & `pytest-reporter-html1-0.8.3/pytest_reporter_html1.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitattributes
 .gitignore
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 requirements.txt
 screenshot.png
 setup.py
 tox.ini
 .github/workflows/pythonpackage.yml
 .github/workflows/pythonpublish.yml
 pytest_reporter_html1/__init__.py
```

### Comparing `pytest-reporter-html1-0.8.2/screenshot.png` & `pytest-reporter-html1-0.8.3/screenshot.png`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/setup.py` & `pytest-reporter-html1-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/tests/samples/conftest.py` & `pytest-reporter-html1-0.8.3/tests/samples/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/tests/samples/sample_test_info.py` & `pytest-reporter-html1-0.8.3/tests/samples/sample_test_info.py`

 * *Files identical despite different names*

### Comparing `pytest-reporter-html1-0.8.2/tests/test_samples.py` & `pytest-reporter-html1-0.8.3/tests/test_samples.py`

 * *Files identical despite different names*

