# Comparing `tmp/aiodbm-0.2.0b1.tar.gz` & `tmp/aiodbm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodbm-0.2.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodbm-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodbm-0.2.0b1.tar` & `aiodbm-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,7 @@
--rw-r--r--   0        0        0      221 2023-05-31 12:59:34.028365 aiodbm-0.2.0b1/.coveragerc
--rw-r--r--   0        0        0      964 2023-06-01 00:00:49.918153 aiodbm-0.2.0b1/.github/workflows/main.yml
--rw-r--r--   0        0        0      798 2023-06-01 00:00:49.918153 aiodbm-0.2.0b1/.github/workflows/release.yml
--rw-r--r--   0        0        0      110 2023-05-31 01:31:26.803876 aiodbm-0.2.0b1/.gitignore
--rw-r--r--   0        0        0      477 2023-05-31 13:13:07.581265 aiodbm-0.2.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-06-02 17:34:44.178645 aiodbm-0.2.0b1/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-31 00:53:23.248884 aiodbm-0.2.0b1/LICENSE
--rw-r--r--   0        0        0      121 2023-05-31 13:00:10.815989 aiodbm-0.2.0b1/Makefile
--rw-r--r--   0        0        0     3771 2023-06-03 11:55:58.452751 aiodbm-0.2.0b1/README.rst
--rw-r--r--   0        0        0      634 2023-06-02 17:04:23.375256 aiodbm-0.2.0b1/docs/Makefile
--rw-r--r--   0        0        0       37 2023-06-02 17:04:23.375256 aiodbm-0.2.0b1/docs/_static/custom.css
--rw-r--r--   0        0        0       97 2023-06-02 17:31:54.543635 aiodbm-0.2.0b1/docs/api.rst
--rw-r--r--   0        0        0     1856 2023-06-02 17:19:55.420980 aiodbm-0.2.0b1/docs/conf.py
--rw-r--r--   0        0        0      347 2023-06-02 17:04:23.375256 aiodbm-0.2.0b1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-06-02 17:04:23.375256 aiodbm-0.2.0b1/docs/make.bat
--rw-r--r--   0        0        0      378 2023-06-01 00:51:11.106230 aiodbm-0.2.0b1/examples/basic_usage.py
--rw-r--r--   0        0        0      795 2023-06-02 17:51:19.099511 aiodbm-0.2.0b1/pyproject.toml
--rw-r--r--   0        0        0      144 2023-06-03 11:55:22.932910 aiodbm-0.2.0b1/src/aiodbm/__init__.py
--rw-r--r--   0        0        0     8179 2023-06-03 10:28:02.047201 aiodbm-0.2.0b1/src/aiodbm/core.py
--rw-r--r--   0        0        0        0 2023-05-31 00:55:46.532853 aiodbm-0.2.0b1/tests/__init__.py
--rw-r--r--   0        0        0     2044 2023-06-02 17:03:15.638929 aiodbm-0.2.0b1/tests/measurements.py
--rw-r--r--   0        0        0     9197 2023-06-03 10:44:24.394360 aiodbm-0.2.0b1/tests/test_core.py
--rw-r--r--   0        0        0      397 2023-05-31 12:58:42.736904 aiodbm-0.2.0b1/tox.ini
--rw-r--r--   0        0        0     4465 1970-01-01 00:00:00.000000 aiodbm-0.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-05 18:14:10.939963 aiodbm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3725 2023-06-05 18:14:10.939963 aiodbm-0.3.0/README.rst
+-rw-r--r--   0        0        0      795 2023-06-05 18:14:10.939963 aiodbm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-06-05 18:14:10.939963 aiodbm-0.3.0/src/aiodbm/__init__.py
+-rw-r--r--   0        0        0     5819 2023-06-05 18:14:10.939963 aiodbm-0.3.0/src/aiodbm/core.py
+-rw-r--r--   0        0        0     3103 2023-06-05 18:14:10.939963 aiodbm-0.3.0/src/aiodbm/threads.py
+-rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 aiodbm-0.3.0/PKG-INFO
```

### Comparing `aiodbm-0.2.0b1/LICENSE` & `aiodbm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodbm-0.2.0b1/README.rst` & `aiodbm-0.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 Description
 -----------
 
 aiodbm is a library that allows you to use DBM in asyncio code.
 
 * Full coverage of Python's DBM and GDBM API
-* Shared single thread implementation for best asyncio performance
 * Typing support
 * Docstrings and documentation
 * Fully tested
 
 Why use DBM?
 ------------
 
@@ -68,14 +67,17 @@
 
 .. code:: shell
 
     pip install aiodbm
 
 ------------
 
+Reference
+---------
+
 .. [1] Python's DBM module: https://docs.python.org/3/library/dbm.html
 .. [2] The newer DBM variants GDBM or NDBM are preinstalled on most Linux/Unix systems: https://en.wikipedia.org/wiki/DBM_(computing)#Availability
 .. [3] Python benchmark with DBM, Sqlite and other embedded databases: https://charlesleifer.com/blog/completely-un-scientific-benchmarks-of-some-embedded-databases-with-python/
 
 .. _DBM: https://en.wikipedia.org/wiki/DBM_(computing)
 .. _benchmark: https://charlesleifer.com/blog/completely-un-scientific-benchmarks-of-some-embedded-databases-with-python/
```

### Comparing `aiodbm-0.2.0b1/pyproject.toml` & `aiodbm-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodbm-0.2.0b1/PKG-INFO` & `aiodbm-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodbm
-Version: 0.2.0b1
+Version: 0.3.0
 Summary: An AsyncIO bridge for DBM.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -25,15 +25,14 @@
 
 Description
 -----------
 
 aiodbm is a library that allows you to use DBM in asyncio code.
 
 * Full coverage of Python's DBM and GDBM API
-* Shared single thread implementation for best asyncio performance
 * Typing support
 * Docstrings and documentation
 * Fully tested
 
 Why use DBM?
 ------------
 
@@ -85,14 +84,17 @@
 
 .. code:: shell
 
     pip install aiodbm
 
 ------------
 
+Reference
+---------
+
 .. [1] Python's DBM module: https://docs.python.org/3/library/dbm.html
 .. [2] The newer DBM variants GDBM or NDBM are preinstalled on most Linux/Unix systems: https://en.wikipedia.org/wiki/DBM_(computing)#Availability
 .. [3] Python benchmark with DBM, Sqlite and other embedded databases: https://charlesleifer.com/blog/completely-un-scientific-benchmarks-of-some-embedded-databases-with-python/
 
 .. _DBM: https://en.wikipedia.org/wiki/DBM_(computing)
 .. _benchmark: https://charlesleifer.com/blog/completely-un-scientific-benchmarks-of-some-embedded-databases-with-python/
```

