# Comparing `tmp/tricycle-0.2.2.tar.gz` & `tmp/tricycle-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tricycle-0.2.2.tar", last modified: Wed Mar  1 08:38:36 2023, max compression
+gzip compressed data, was "tricycle-0.3.0.tar", last modified: Mon Jun  5 20:02:41 2023, max compression
```

## Comparing `tricycle-0.2.2.tar` & `tricycle-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 oremanj    (501) staff       (20)        0 2023-03-01 08:38:36.262630 tricycle-0.2.2/
--rw-r--r--   0 oremanj    (501) staff       (20)      134 2020-04-22 07:05:02.000000 tricycle-0.2.2/.coveragerc
--rw-r--r--   0 oremanj    (501) staff       (20)       98 2020-04-22 07:05:02.000000 tricycle-0.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 oremanj    (501) staff       (20)     1013 2020-04-28 22:57:59.000000 tricycle-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 oremanj    (501) staff       (20)      185 2020-04-22 07:05:02.000000 tricycle-0.2.2/LICENSE
--rw-r--r--   0 oremanj    (501) staff       (20)    11358 2020-04-22 07:05:02.000000 tricycle-0.2.2/LICENSE.APACHE2
--rw-r--r--   0 oremanj    (501) staff       (20)     1046 2020-04-22 07:05:02.000000 tricycle-0.2.2/LICENSE.MIT
--rw-r--r--   0 oremanj    (501) staff       (20)      177 2020-04-22 07:05:02.000000 tricycle-0.2.2/MANIFEST.in
--rw-r--r--   0 oremanj    (501) staff       (20)     3737 2023-03-01 08:38:36.262753 tricycle-0.2.2/PKG-INFO
--rw-r--r--   0 oremanj    (501) staff       (20)     2890 2020-04-28 22:52:40.000000 tricycle-0.2.2/README.rst
-drwxr-xr-x   0 oremanj    (501) staff       (20)        0 2023-03-01 08:38:36.255352 tricycle-0.2.2/docs/
--rw-r--r--   0 oremanj    (501) staff       (20)      610 2020-04-22 07:05:02.000000 tricycle-0.2.2/docs/Makefile
--rw-r--r--   0 oremanj    (501) staff       (20)      780 2020-04-22 07:05:02.000000 tricycle-0.2.2/docs/make.bat
-drwxr-xr-x   0 oremanj    (501) staff       (20)        0 2023-03-01 08:38:36.256864 tricycle-0.2.2/docs/source/
-drwxr-xr-x   0 oremanj    (501) staff       (20)        0 2023-03-01 08:38:36.257232 tricycle-0.2.2/docs/source/_static/
--rw-r--r--   0 oremanj    (501) staff       (20)        0 2020-04-22 07:05:02.000000 tricycle-0.2.2/docs/source/_static/.gitkeep
--rw-r--r--   0 oremanj    (501) staff       (20)     6270 2020-04-22 07:05:02.000000 tricycle-0.2.2/docs/source/conf.py
--rw-r--r--   0 oremanj    (501) staff       (20)      809 2023-03-01 08:09:34.000000 tricycle-0.2.2/docs/source/history.rst
--rw-r--r--   0 oremanj    (501) staff       (20)      804 2020-04-22 07:05:02.000000 tricycle-0.2.2/docs/source/index.rst
--rw-r--r--   0 oremanj    (501) staff       (20)     8430 2020-04-22 07:05:02.000000 tricycle-0.2.2/docs/source/reference.rst
--rw-r--r--   0 oremanj    (501) staff       (20)      215 2020-04-22 07:05:02.000000 tricycle-0.2.2/pyproject.toml
--rw-r--r--   0 oremanj    (501) staff       (20)       73 2023-03-01 08:38:36.263165 tricycle-0.2.2/setup.cfg
--rw-r--r--   0 oremanj    (501) staff       (20)     1153 2023-03-01 08:06:53.000000 tricycle-0.2.2/setup.py
--rw-r--r--   0 oremanj    (501) staff       (20)     1515 2023-03-01 08:32:00.000000 tricycle-0.2.2/test-requirements.txt
-drwxr-xr-x   0 oremanj    (501) staff       (20)        0 2023-03-01 08:38:36.259228 tricycle-0.2.2/tricycle/
--rw-r--r--   0 oremanj    (501) staff       (20)      583 2023-03-01 08:06:53.000000 tricycle-0.2.2/tricycle/__init__.py
--rw-r--r--   0 oremanj    (501) staff       (20)     6159 2023-03-01 08:33:54.000000 tricycle-0.2.2/tricycle/_meta.py
--rw-r--r--   0 oremanj    (501) staff       (20)     3445 2020-04-22 07:05:02.000000 tricycle-0.2.2/tricycle/_multi_cancel.py
--rw-r--r--   0 oremanj    (501) staff       (20)    11135 2020-10-01 07:08:46.000000 tricycle-0.2.2/tricycle/_rwlock.py
--rw-r--r--   0 oremanj    (501) staff       (20)     5770 2023-03-01 08:06:53.000000 tricycle-0.2.2/tricycle/_service_nursery.py
--rw-r--r--   0 oremanj    (501) staff       (20)    14908 2020-10-01 07:08:46.000000 tricycle-0.2.2/tricycle/_streams.py
-drwxr-xr-x   0 oremanj    (501) staff       (20)        0 2023-03-01 08:38:36.262390 tricycle-0.2.2/tricycle/_tests/
--rw-r--r--   0 oremanj    (501) staff       (20)        0 2020-04-22 07:05:02.000000 tricycle-0.2.2/tricycle/_tests/__init__.py
--rw-r--r--   0 oremanj    (501) staff       (20)       59 2020-04-22 07:05:02.000000 tricycle-0.2.2/tricycle/_tests/conftest.py
--rw-r--r--   0 oremanj    (501) staff       (20)     4328 2023-03-01 08:24:22.000000 tricycle-0.2.2/tricycle/_tests/test_meta.py
--rw-r--r--   0 oremanj    (501) staff       (20)     7198 2023-03-01 08:24:16.000000 tricycle-0.2.2/tricycle/_tests/test_multi_cancel.py
--rw-r--r--   0 oremanj    (501) staff       (20)     7877 2023-03-01 08:24:09.000000 tricycle-0.2.2/tricycle/_tests/test_rwlock.py
--rw-r--r--   0 oremanj    (501) staff       (20)     3725 2023-03-01 08:24:03.000000 tricycle-0.2.2/tricycle/_tests/test_service_nursery.py
--rw-r--r--   0 oremanj    (501) staff       (20)    13355 2023-03-01 08:23:44.000000 tricycle-0.2.2/tricycle/_tests/test_streams.py
--rw-r--r--   0 oremanj    (501) staff       (20)       22 2023-03-01 08:07:41.000000 tricycle-0.2.2/tricycle/_version.py
--rw-r--r--   0 oremanj    (501) staff       (20)        0 2020-04-22 07:05:02.000000 tricycle-0.2.2/tricycle/py.typed
-drwxr-xr-x   0 oremanj    (501) staff       (20)        0 2023-03-01 08:38:36.260615 tricycle-0.2.2/tricycle.egg-info/
--rw-r--r--   0 oremanj    (501) staff       (20)     3737 2023-03-01 08:38:36.000000 tricycle-0.2.2/tricycle.egg-info/PKG-INFO
--rw-r--r--   0 oremanj    (501) staff       (20)      868 2023-03-01 08:38:36.000000 tricycle-0.2.2/tricycle.egg-info/SOURCES.txt
--rw-r--r--   0 oremanj    (501) staff       (20)        1 2023-03-01 08:38:36.000000 tricycle-0.2.2/tricycle.egg-info/dependency_links.txt
--rw-r--r--   0 oremanj    (501) staff       (20)       32 2023-03-01 08:38:36.000000 tricycle-0.2.2/tricycle.egg-info/requires.txt
--rw-r--r--   0 oremanj    (501) staff       (20)        9 2023-03-01 08:38:36.000000 tricycle-0.2.2/tricycle.egg-info/top_level.txt
+drwxr-xr-x   0 oremanj    (503) staff       (20)        0 2023-06-05 20:02:41.867772 tricycle-0.3.0/
+-rw-r--r--   0 oremanj    (503) staff       (20)      146 2023-06-05 19:55:48.000000 tricycle-0.3.0/.coveragerc
+-rw-r--r--   0 oremanj    (503) staff       (20)       98 2023-06-05 16:41:43.000000 tricycle-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 oremanj    (503) staff       (20)     1013 2023-06-05 16:41:43.000000 tricycle-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 oremanj    (503) staff       (20)      185 2023-06-05 16:41:43.000000 tricycle-0.3.0/LICENSE
+-rw-r--r--   0 oremanj    (503) staff       (20)    11358 2023-06-05 16:41:43.000000 tricycle-0.3.0/LICENSE.APACHE2
+-rw-r--r--   0 oremanj    (503) staff       (20)     1046 2023-06-05 16:41:43.000000 tricycle-0.3.0/LICENSE.MIT
+-rw-r--r--   0 oremanj    (503) staff       (20)      177 2023-06-05 16:41:43.000000 tricycle-0.3.0/MANIFEST.in
+-rw-r--r--   0 oremanj    (503) staff       (20)     3773 2023-06-05 20:02:41.867629 tricycle-0.3.0/PKG-INFO
+-rw-r--r--   0 oremanj    (503) staff       (20)     2926 2023-06-05 19:55:48.000000 tricycle-0.3.0/README.rst
+drwxr-xr-x   0 oremanj    (503) staff       (20)        0 2023-06-05 20:02:41.861582 tricycle-0.3.0/docs/
+-rw-r--r--   0 oremanj    (503) staff       (20)      610 2023-06-05 16:41:43.000000 tricycle-0.3.0/docs/Makefile
+-rw-r--r--   0 oremanj    (503) staff       (20)      780 2023-06-05 16:41:43.000000 tricycle-0.3.0/docs/make.bat
+drwxr-xr-x   0 oremanj    (503) staff       (20)        0 2023-06-05 20:02:41.862563 tricycle-0.3.0/docs/source/
+drwxr-xr-x   0 oremanj    (503) staff       (20)        0 2023-06-05 20:02:41.862817 tricycle-0.3.0/docs/source/_static/
+-rw-r--r--   0 oremanj    (503) staff       (20)        0 2023-06-05 16:41:43.000000 tricycle-0.3.0/docs/source/_static/.gitkeep
+-rw-r--r--   0 oremanj    (503) staff       (20)     6850 2023-06-05 19:55:48.000000 tricycle-0.3.0/docs/source/conf.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     1328 2023-06-05 19:57:51.000000 tricycle-0.3.0/docs/source/history.rst
+-rw-r--r--   0 oremanj    (503) staff       (20)      804 2023-06-05 16:41:43.000000 tricycle-0.3.0/docs/source/index.rst
+-rw-r--r--   0 oremanj    (503) staff       (20)    11338 2023-06-05 19:55:48.000000 tricycle-0.3.0/docs/source/reference.rst
+-rw-r--r--   0 oremanj    (503) staff       (20)     1209 2023-06-05 17:21:59.000000 tricycle-0.3.0/pyproject.toml
+-rw-r--r--   0 oremanj    (503) staff       (20)       38 2023-06-05 20:02:41.867814 tricycle-0.3.0/setup.cfg
+-rw-r--r--   0 oremanj    (503) staff       (20)     1153 2023-06-05 17:21:59.000000 tricycle-0.3.0/setup.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     1639 2023-06-05 17:21:59.000000 tricycle-0.3.0/test-requirements.txt
+drwxr-xr-x   0 oremanj    (503) staff       (20)        0 2023-06-05 20:02:41.865000 tricycle-0.3.0/tricycle/
+-rw-r--r--   0 oremanj    (503) staff       (20)      655 2023-06-05 19:55:48.000000 tricycle-0.3.0/tricycle/__init__.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     6154 2023-06-05 17:21:59.000000 tricycle-0.3.0/tricycle/_meta.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     3445 2023-06-05 16:41:43.000000 tricycle-0.3.0/tricycle/_multi_cancel.py
+-rw-r--r--   0 oremanj    (503) staff       (20)    11130 2023-06-05 17:21:59.000000 tricycle-0.3.0/tricycle/_rwlock.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     5765 2023-06-05 17:21:59.000000 tricycle-0.3.0/tricycle/_service_nursery.py
+-rw-r--r--   0 oremanj    (503) staff       (20)    14908 2023-06-05 16:41:43.000000 tricycle-0.3.0/tricycle/_streams.py
+drwxr-xr-x   0 oremanj    (503) staff       (20)        0 2023-06-05 20:02:41.867379 tricycle-0.3.0/tricycle/_tests/
+-rw-r--r--   0 oremanj    (503) staff       (20)        0 2023-06-05 16:41:43.000000 tricycle-0.3.0/tricycle/_tests/__init__.py
+-rw-r--r--   0 oremanj    (503) staff       (20)       59 2023-06-05 16:41:43.000000 tricycle-0.3.0/tricycle/_tests/conftest.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     4323 2023-06-05 17:21:59.000000 tricycle-0.3.0/tricycle/_tests/test_meta.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     7198 2023-06-05 16:41:43.000000 tricycle-0.3.0/tricycle/_tests/test_multi_cancel.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     7877 2023-06-05 16:41:43.000000 tricycle-0.3.0/tricycle/_tests/test_rwlock.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     3725 2023-06-05 16:41:43.000000 tricycle-0.3.0/tricycle/_tests/test_service_nursery.py
+-rw-r--r--   0 oremanj    (503) staff       (20)    13325 2023-06-05 17:21:59.000000 tricycle-0.3.0/tricycle/_tests/test_streams.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     5509 2023-06-05 19:55:48.000000 tricycle-0.3.0/tricycle/_tests/test_tree_var.py
+-rw-r--r--   0 oremanj    (503) staff       (20)     8448 2023-06-05 19:55:48.000000 tricycle-0.3.0/tricycle/_tree_var.py
+-rw-r--r--   0 oremanj    (503) staff       (20)       22 2023-06-05 19:56:03.000000 tricycle-0.3.0/tricycle/_version.py
+-rw-r--r--   0 oremanj    (503) staff       (20)        0 2023-06-05 16:41:43.000000 tricycle-0.3.0/tricycle/py.typed
+drwxr-xr-x   0 oremanj    (503) staff       (20)        0 2023-06-05 20:02:41.865817 tricycle-0.3.0/tricycle.egg-info/
+-rw-r--r--   0 oremanj    (503) staff       (20)     3773 2023-06-05 20:02:41.000000 tricycle-0.3.0/tricycle.egg-info/PKG-INFO
+-rw-r--r--   0 oremanj    (503) staff       (20)      913 2023-06-05 20:02:41.000000 tricycle-0.3.0/tricycle.egg-info/SOURCES.txt
+-rw-r--r--   0 oremanj    (503) staff       (20)        1 2023-06-05 20:02:41.000000 tricycle-0.3.0/tricycle.egg-info/dependency_links.txt
+-rw-r--r--   0 oremanj    (503) staff       (20)       32 2023-06-05 20:02:41.000000 tricycle-0.3.0/tricycle.egg-info/requires.txt
+-rw-r--r--   0 oremanj    (503) staff       (20)        9 2023-06-05 20:02:41.000000 tricycle-0.3.0/tricycle.egg-info/top_level.txt
```

### Comparing `tricycle-0.2.2/CONTRIBUTING.md` & `tricycle-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/LICENSE.APACHE2` & `tricycle-0.3.0/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/LICENSE.MIT` & `tricycle-0.3.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/PKG-INFO` & `tricycle-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tricycle
-Version: 0.2.2
+Version: 0.3.0
 Summary: Experimental extensions for Trio, the friendly async I/O library
 Home-page: https://github.com/oremanj/tricycle
 Author: Joshua Oreman
 Author-email: oremanj@gmail.com
 License: MIT -or- Apache License 2.0
 Keywords: async,trio
 Classifier: License :: OSI Approved :: MIT License
@@ -12,34 +12,34 @@
 Classifier: Framework :: Trio
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 License-File: LICENSE.APACHE2
 License-File: LICENSE.MIT
 
 tricycle: experimental extensions for Trio
 ==========================================
 
 .. image:: https://img.shields.io/pypi/v/tricycle.svg
    :target: https://pypi.org/project/tricycle
    :alt: Latest PyPI version
 
+.. image:: https://github.com/oremanj/tricycle/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/oremanj/tricycle/actions/workflows/ci.yml
+   :alt: Automated test status
+
 .. image:: https://img.shields.io/badge/docs-read%20now-blue.svg
    :target: https://tricycle.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
-.. image:: https://travis-ci.org/oremanj/tricycle.svg?branch=master
-   :target: https://travis-ci.org/oremanj/tricycle
-   :alt: Automated test status
-
 .. image:: https://codecov.io/gh/oremanj/tricycle/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/oremanj/tricycle
    :alt: Test coverage
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/ambv/black
    :alt: Code style: black
@@ -55,15 +55,15 @@
 
 While we won't release known-broken code, and we strive for
 cleanliness and good test coverage, please be advised that
 ``tricycle`` is mostly one person's box of tools that seemed like a
 good idea at the time, and should be treated with according skepticism
 if you're contemplating using it in production. It hasn't necessarily
 been reviewed or tested to Trio's standards, it supports at minimum
-Python 3.6, and some features might not be available on PyPy or on
+Python 3.7, and some features might not be available on PyPy or on
 Windows.
 
 * If you find that it meets your needs, you're welcome to use it. We'll
   endeavor to provide a (short) deprecation period on API changes, but
   no guarantees on that yet.
 
 * If you find that it doesn't meet your needs, feel free to `let us know
```

### Comparing `tricycle-0.2.2/README.rst` & `tricycle-0.3.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 tricycle: experimental extensions for Trio
 ==========================================
 
 .. image:: https://img.shields.io/pypi/v/tricycle.svg
    :target: https://pypi.org/project/tricycle
    :alt: Latest PyPI version
 
+.. image:: https://github.com/oremanj/tricycle/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/oremanj/tricycle/actions/workflows/ci.yml
+   :alt: Automated test status
+
 .. image:: https://img.shields.io/badge/docs-read%20now-blue.svg
    :target: https://tricycle.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
-.. image:: https://travis-ci.org/oremanj/tricycle.svg?branch=master
-   :target: https://travis-ci.org/oremanj/tricycle
-   :alt: Automated test status
-
 .. image:: https://codecov.io/gh/oremanj/tricycle/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/oremanj/tricycle
    :alt: Test coverage
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/ambv/black
    :alt: Code style: black
@@ -32,15 +32,15 @@
 
 While we won't release known-broken code, and we strive for
 cleanliness and good test coverage, please be advised that
 ``tricycle`` is mostly one person's box of tools that seemed like a
 good idea at the time, and should be treated with according skepticism
 if you're contemplating using it in production. It hasn't necessarily
 been reviewed or tested to Trio's standards, it supports at minimum
-Python 3.6, and some features might not be available on PyPy or on
+Python 3.7, and some features might not be available on PyPy or on
 Windows.
 
 * If you find that it meets your needs, you're welcome to use it. We'll
   endeavor to provide a (short) deprecation period on API changes, but
   no guarantees on that yet.
 
 * If you find that it doesn't meet your needs, feel free to `let us know
```

### Comparing `tricycle-0.2.2/docs/Makefile` & `tricycle-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/docs/make.bat` & `tricycle-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/docs/source/conf.py` & `tricycle-0.3.0/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,41 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 # So autodoc can import our package
 sys.path.insert(0, os.path.abspath('../..'))
 
+# https://docs.readthedocs.io/en/stable/builds.html#build-environment
+if "READTHEDOCS" in os.environ:
+    import glob
+
+    if glob.glob("../../newsfragments/*.*.rst"):
+        print("-- Found newsfragments; running towncrier --", flush=True)
+        import subprocess
+
+        subprocess.run(
+            ["towncrier", "--yes", "--date", "not released yet"],
+            cwd="../..",
+            check=True,
+        )
+
 # Warn about all references to unknown targets
 nitpicky = True
 # Except for these ones, which we expect to point to unknown targets:
 nitpick_ignore = [
     # Format is ("sphinx reference type", "string"), e.g.:
     ("py:obj", "bytes-like"),
     ("py:class", "None"),
     ("py:exc", "Anything else"),
+    ("py:class", "tricycle._rwlock._RWLockStatistics"),
+    ("py:class", "tricycle._tree_var.T"),
+    ("py:class", "tricycle._tree_var.U"),
 ]
+default_role = "obj"
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
@@ -86,15 +104,15 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `tricycle-0.2.2/docs/source/index.rst` & `tricycle-0.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/setup.py` & `tricycle-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     author="Joshua Oreman",
     author_email="oremanj@gmail.com",
     license="MIT -or- Apache License 2.0",
     packages=find_packages(),
     include_package_data=True,
     install_requires=["trio >= 0.15.0", "trio-typing >= 0.5.0"],
     keywords=["async", "trio"],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "License :: OSI Approved :: Apache Software License",
         "Framework :: Trio",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `tricycle-0.2.2/test-requirements.txt` & `tricycle-0.3.0/test-requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,88 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile test-requirements.in
 #
+
 async-generator==1.10
     # via
     #   -r test-requirements.in
     #   trio
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   -r test-requirements.in
-    #   pytest
     #   trio
-black==23.1.0 ; implementation_name == "cpython"
+black==23.3.0 ; implementation_name == "cpython"
     # via -r test-requirements.in
 click==8.1.3
     # via black
-coverage[toml]==7.2.1
+coverage[toml]==7.2.7
     # via pytest-cov
+exceptiongroup==1.1.1
+    # via
+    #   pytest
+    #   trio
 flake8==5.0.4
     # via -r test-requirements.in
 idna==3.4
     # via trio
 iniconfig==2.0.0
     # via pytest
 mccabe==0.7.0
     # via flake8
-mypy==1.0.1 ; implementation_name == "cpython"
+mypy==1.3.0 ; implementation_name == "cpython"
     # via -r test-requirements.in
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
     #   trio-typing
 outcome==1.2.0
     # via
     #   pytest-trio
     #   trio
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   pytest
-pathspec==0.11.0
+pathspec==0.11.1
     # via black
-platformdirs==3.0.0
+platformdirs==3.5.1
     # via black
 pluggy==1.0.0
     # via pytest
 pycodestyle==2.9.1
     # via flake8
 pyflakes==2.5.0
     # via flake8
-pytest==7.2.1
+pytest==7.3.1
     # via
     #   -r test-requirements.in
     #   pytest-cov
     #   pytest-trio
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r test-requirements.in
 pytest-trio==0.8.0
     # via -r test-requirements.in
 sniffio==1.3.0
     # via trio
 sortedcontainers==2.4.0
     # via trio
+tomli==2.0.1
+    # via
+    #   black
+    #   mypy
+    #   pytest
 trio==0.22.0
     # via
     #   -r test-requirements.in
     #   pytest-trio
     #   trio-typing
-trio-typing==0.7.0
+trio-typing==0.8.0
     # via -r test-requirements.in
-typing-extensions==4.5.0
+typing-extensions==4.6.3
     # via
+    #   black
     #   mypy
     #   trio-typing
```

### Comparing `tricycle-0.2.2/tricycle/__init__.py` & `tricycle-0.3.0/tricycle/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ._streams import (
     BufferedReceiveStream as BufferedReceiveStream,
     TextReceiveStream as TextReceiveStream,
 )
 from ._multi_cancel import MultiCancelScope as MultiCancelScope
 from ._service_nursery import open_service_nursery as open_service_nursery
 from ._meta import ScopedObject as ScopedObject, BackgroundObject as BackgroundObject
+from ._tree_var import TreeVar as TreeVar, TreeVarToken as TreeVarToken
 
 # watch this space...
 
 _export = None
 for _export in globals().values():
     if hasattr(_export, "__module__"):
         _export.__module__ = __name__
```

### Comparing `tricycle-0.2.2/tricycle/_meta.py` & `tricycle-0.3.0/tricycle/_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 import functools
-from async_generator import asynccontextmanager
+from contextlib import asynccontextmanager
 from trio import Nursery
 from typing import (
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
     ClassVar,
```

### Comparing `tricycle-0.2.2/tricycle/_multi_cancel.py` & `tricycle-0.3.0/tricycle/_multi_cancel.py`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/tricycle/_rwlock.py` & `tricycle-0.3.0/tricycle/_rwlock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import attr
 import trio
-from async_generator import asynccontextmanager
+from contextlib import asynccontextmanager
 from collections import OrderedDict
 from typing import (
     AsyncIterator,
     FrozenSet,
     List,
     Optional,
     Sequence,
```

### Comparing `tricycle-0.2.2/tricycle/_service_nursery.py` & `tricycle-0.3.0/tricycle/_service_nursery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import attr
 import collections
 import trio
 from trio_typing import TaskStatus
 from functools import partial
-from async_generator import asynccontextmanager
+from contextlib import asynccontextmanager
 from typing import Any, AsyncIterator, Awaitable, Callable, Optional, overload
 from ._multi_cancel import MultiCancelScope
 
 
 def _get_coroutine_or_flag_problem(
     async_fn: Callable[..., Awaitable[Any]], *args: Any, **kwargs: Any
 ) -> Awaitable[Any]:
```

### Comparing `tricycle-0.2.2/tricycle/_streams.py` & `tricycle-0.3.0/tricycle/_streams.py`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/tricycle/_tests/test_meta.py` & `tricycle-0.3.0/tricycle/_tests/test_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import attr
 import pytest
 import types
 import trio
 import trio.testing
-from async_generator import asynccontextmanager
+from contextlib import asynccontextmanager
 from typing import Any, AsyncIterator, Coroutine, Iterator, List
 from trio_typing import TaskStatus
 
 from .. import ScopedObject, BackgroundObject
 
 
 def test_too_much_magic() -> None:
```

### Comparing `tricycle-0.2.2/tricycle/_tests/test_multi_cancel.py` & `tricycle-0.3.0/tricycle/_tests/test_multi_cancel.py`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/tricycle/_tests/test_rwlock.py` & `tricycle-0.3.0/tricycle/_tests/test_rwlock.py`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/tricycle/_tests/test_service_nursery.py` & `tricycle-0.3.0/tricycle/_tests/test_service_nursery.py`

 * *Files identical despite different names*

### Comparing `tricycle-0.2.2/tricycle/_tests/test_streams.py` & `tricycle-0.3.0/tricycle/_tests/test_streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pytest
 import locale
 import random
 import sys
 
 import trio
 import trio.testing
-from async_generator import asynccontextmanager
+from contextlib import asynccontextmanager
 from functools import partial
 from typing import (
+    AsyncContextManager,
     AsyncIterator,
     Awaitable,
     Callable,
     List,
     Optional,
     Sequence,
     Tuple,
     cast,
 )
-from typing_extensions import AsyncContextManager
 from .. import BufferedReceiveStream, TextReceiveStream
 
 
 async def test_buffered_receive(autojump_clock: trio.testing.MockClock) -> None:
     send_stream, receive_stream_raw = trio.testing.memory_stream_one_way_pair()
     receive_stream = BufferedReceiveStream(receive_stream_raw, chunk_size=8)
```

### Comparing `tricycle-0.2.2/tricycle.egg-info/PKG-INFO` & `tricycle-0.3.0/tricycle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tricycle
-Version: 0.2.2
+Version: 0.3.0
 Summary: Experimental extensions for Trio, the friendly async I/O library
 Home-page: https://github.com/oremanj/tricycle
 Author: Joshua Oreman
 Author-email: oremanj@gmail.com
 License: MIT -or- Apache License 2.0
 Keywords: async,trio
 Classifier: License :: OSI Approved :: MIT License
@@ -12,34 +12,34 @@
 Classifier: Framework :: Trio
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 License-File: LICENSE.APACHE2
 License-File: LICENSE.MIT
 
 tricycle: experimental extensions for Trio
 ==========================================
 
 .. image:: https://img.shields.io/pypi/v/tricycle.svg
    :target: https://pypi.org/project/tricycle
    :alt: Latest PyPI version
 
+.. image:: https://github.com/oremanj/tricycle/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/oremanj/tricycle/actions/workflows/ci.yml
+   :alt: Automated test status
+
 .. image:: https://img.shields.io/badge/docs-read%20now-blue.svg
    :target: https://tricycle.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
-.. image:: https://travis-ci.org/oremanj/tricycle.svg?branch=master
-   :target: https://travis-ci.org/oremanj/tricycle
-   :alt: Automated test status
-
 .. image:: https://codecov.io/gh/oremanj/tricycle/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/oremanj/tricycle
    :alt: Test coverage
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/ambv/black
    :alt: Code style: black
@@ -55,15 +55,15 @@
 
 While we won't release known-broken code, and we strive for
 cleanliness and good test coverage, please be advised that
 ``tricycle`` is mostly one person's box of tools that seemed like a
 good idea at the time, and should be treated with according skepticism
 if you're contemplating using it in production. It hasn't necessarily
 been reviewed or tested to Trio's standards, it supports at minimum
-Python 3.6, and some features might not be available on PyPy or on
+Python 3.7, and some features might not be available on PyPy or on
 Windows.
 
 * If you find that it meets your needs, you're welcome to use it. We'll
   endeavor to provide a (short) deprecation period on API changes, but
   no guarantees on that yet.
 
 * If you find that it doesn't meet your needs, feel free to `let us know
```

### Comparing `tricycle-0.2.2/tricycle.egg-info/SOURCES.txt` & `tricycle-0.3.0/tricycle.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 CONTRIBUTING.md
 LICENSE
 LICENSE.APACHE2
 LICENSE.MIT
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 test-requirements.txt
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/history.rst
 docs/source/index.rst
@@ -19,21 +18,23 @@
 docs/source/_static/.gitkeep
 tricycle/__init__.py
 tricycle/_meta.py
 tricycle/_multi_cancel.py
 tricycle/_rwlock.py
 tricycle/_service_nursery.py
 tricycle/_streams.py
+tricycle/_tree_var.py
 tricycle/_version.py
 tricycle/py.typed
 tricycle.egg-info/PKG-INFO
 tricycle.egg-info/SOURCES.txt
 tricycle.egg-info/dependency_links.txt
 tricycle.egg-info/requires.txt
 tricycle.egg-info/top_level.txt
 tricycle/_tests/__init__.py
 tricycle/_tests/conftest.py
 tricycle/_tests/test_meta.py
 tricycle/_tests/test_multi_cancel.py
 tricycle/_tests/test_rwlock.py
 tricycle/_tests/test_service_nursery.py
-tricycle/_tests/test_streams.py
+tricycle/_tests/test_streams.py
+tricycle/_tests/test_tree_var.py
```

