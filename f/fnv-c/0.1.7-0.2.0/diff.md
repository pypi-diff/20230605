# Comparing `tmp/fnv-c-0.1.7.tar.gz` & `tmp/fnv-c-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fnv-c-0.1.7.tar", last modified: Wed May 31 13:08:08 2023, max compression
+gzip compressed data, was "dist/fnv-c-0.2.0.tar", last modified: Mon Jun  5 09:39:09 2023, max compression
```

## Comparing `fnv-c-0.1.7.tar` & `fnv-c-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:08:08.000000 fnv-c-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 13:07:57.000000 fnv-c-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-31 13:08:08.000000 fnv-c-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-31 13:07:57.000000 fnv-c-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:08:08.000000 fnv-c-0.1.7/fnv_c/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-31 13:07:57.000000 fnv-c-0.1.7/fnv_c/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:08:08.000000 fnv-c-0.1.7/fnv_c/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:07:57.000000 fnv-c-0.1.7/fnv_c/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-31 13:07:57.000000 fnv-c-0.1.7/fnv_c/ext/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 13:07:57.000000 fnv-c-0.1.7/fnv_c/ext/fnv.c
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-31 13:07:57.000000 fnv-c-0.1.7/fnv_c/ext/fnv.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:08:08.000000 fnv-c-0.1.7/fnv_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-31 13:08:08.000000 fnv-c-0.1.7/fnv_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 13:08:08.000000 fnv-c-0.1.7/fnv_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:08:08.000000 fnv-c-0.1.7/fnv_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 13:08:08.000000 fnv-c-0.1.7/fnv_c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 13:08:08.000000 fnv-c-0.1.7/fnv_c.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-31 13:07:57.000000 fnv-c-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:08:08.000000 fnv-c-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-31 13:08:08.000000 fnv-c-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:39:09.000000 fnv-c-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 09:38:51.000000 fnv-c-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-05 09:39:09.000000 fnv-c-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-05 09:38:51.000000 fnv-c-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:39:09.000000 fnv-c-0.2.0/fnv_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-05 09:38:51.000000 fnv-c-0.2.0/fnv_c/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:39:09.000000 fnv-c-0.2.0/fnv_c/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:38:51.000000 fnv-c-0.2.0/fnv_c/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-05 09:38:51.000000 fnv-c-0.2.0/fnv_c/ext/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-05 09:38:51.000000 fnv-c-0.2.0/fnv_c/ext/fnv.c
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-05 09:38:51.000000 fnv-c-0.2.0/fnv_c/ext/fnv.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:39:09.000000 fnv-c-0.2.0/fnv_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-05 09:39:09.000000 fnv-c-0.2.0/fnv_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-05 09:39:09.000000 fnv-c-0.2.0/fnv_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:39:09.000000 fnv-c-0.2.0/fnv_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 09:39:09.000000 fnv-c-0.2.0/fnv_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 09:39:09.000000 fnv-c-0.2.0/fnv_c.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-05 09:38:51.000000 fnv-c-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:39:09.000000 fnv-c-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-05 09:39:08.000000 fnv-c-0.2.0/setup.py
```

### Comparing `fnv-c-0.1.7/PKG-INFO` & `fnv-c-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,76 @@
-Metadata-Version: 2.1
-Name: fnv-c
-Version: 0.1.7
-Summary: Python 3.7+ FNV (fnv0, fnv1, fnv1a) non-cryptographic hash library implemented in C through libffi
-Home-page: https://github.com/botify-labs/fnv-c
-Author: Fabien MARTY
-Author-email: fabien.marty@botify.com
-License: UNKNOWN
-Description: # fnv-c
-        
-        [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/botify-labs/fnv-c/lint.yaml)](https://github.com/botify-labs/fnv-c/actions/workflows/lint.yaml)
-        [![Codecov](https://img.shields.io/codecov/c/github/botify-labs/fnv-c)](https://app.codecov.io/github/botify-labs/fnv-c)
-        [![pypi badge](https://img.shields.io/pypi/v/fnv-c?color=brightgreen)](https://pypi.org/project/fnv-c/)
-        
-        ## What is it?
-        
-        **fnv-c** is a Python 3.7+ FNV (`fnv0`, `fnv1`, `fnv1a`) **non-cryptographic** hash library implemented in C through libffi.
-        
-        FNV ("Fowler–Noll–Vo") is is a non-cryptographic hash function created by Glenn Fowler, Landon Curt Noll, and Kiem-Phong.
-        FNV is probably no the "best" non-cryptographic hash function but:
-        
-        - it has a reasonably good distribution
-        - it's very fast
-        - it's very easy to implement *(even in some exotic stored procedures for example)* so you can use it everywhere
-        
-        More details on [this Wikepedia article](https://en.wikipedia.org/wiki/Fowler%E2%80%93Noll%E2%80%93Vo_hash_function).
-        
-        ## Features
-        
-        - speed: **4 000%** faster than basic Python implementation, **40%** faster than `pyhash`
-        - portability:
-            - tested with recent Python versions (3.7+)
-            - compatible with ARM64 and avoid too agressive CPU optimizations for maximizing binary portability 
-            - compatible with PyPy
-        
-        ## Non features
-        
-        - other hash algorithms (this library is only about FNV algorithm)
-        
-        ## How to install/use it?
-        
-        ```
-        pip install fnv-c
-        ```
-        
-        ```python
-        import fnv_c
-        
-        print(fnv_c.fnv0_32(b"foo bar"))
-        print(fnv_c.fnv0_64(b"foo bar"))
-        print(fnv_c.fnv1_32(b"foo bar"))
-        print(fnv_c.fnv1_64(b"foo bar"))
-        print(fnv_c.fnv1a_32(b"foo bar"))
-        print(fnv_c.fnv1a_64(b"foo bar"))
-        ```
-        
-        ## Function signatures / API
-        
-        Full API doc is available at: [https://botify-labs.github.io/fnv-c/fnv_c/](https://botify-labs.github.io/fnv-c/fnv_c/)
-        
-        ## Dev
-        
-        See [this specific document](DEV.md)
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
+# fnv-c
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/botify-labs/fnv-c/lint.yaml)](https://github.com/botify-labs/fnv-c/actions/workflows/lint.yaml)
+[![Codecov](https://img.shields.io/codecov/c/github/botify-labs/fnv-c)](https://app.codecov.io/github/botify-labs/fnv-c)
+[![pypi badge](https://img.shields.io/pypi/v/fnv-c?color=brightgreen)](https://pypi.org/project/fnv-c/)
+
+## What is it?
+
+**fnv-c** is a Python 3.7+ FNV (`fnv0`, `fnv1`, `fnv1a`) **non-cryptographic** hash library implemented in C through libffi.
+
+FNV ("Fowler–Noll–Vo") is is a non-cryptographic hash function created by Glenn Fowler, Landon Curt Noll, and Kiem-Phong.
+FNV is probably no the "best" non-cryptographic hash function but:
+
+- it has a reasonably good distribution
+- it's very fast
+- it's very easy to implement *(even in some exotic stored procedures for example)* so you can use it everywhere
+
+More details on [this Wikepedia article](https://en.wikipedia.org/wiki/Fowler%E2%80%93Noll%E2%80%93Vo_hash_function).
+
+## Features
+
+- speed: 
+    - up to **800 MB/s** hashing speed *(on Macbook Pro M1 (2020) with `fnv0_64`)*
+    - **6 800%** faster than basic Python implementation, **70%** faster than `pyhash` *(when hashing 100 bytes with `fnv0_64` on a cloud VM)*
+- portability:
+    - tested with recent Python versions (3.7+)
+    - compatible with ARM64
+    - compatible (and tested) with PyPy
+
+## Non features
+
+- other hash algorithms *(this library is only about FNV algorithm)*
+- too agressive CPU optimizations *(we prefer maximizing binary portability)*
+
+## Benchmark
+
+You have a benchmark script [here](bench.py) to bench `fnv-c` by yourself and to compare it with:
+- [`fnvhash`](https://github.com/znerol/py-fnvhash) (pure python implementation)
+- [`pyhash`](https://github.com/flier/pyfasthash) (more general hashing library with C++ extension)
+
+### Comparisons with other libraries (`fnv0_64` on a cloud VM)
+
+Differences with `fnvhash` are huge (from **35%** for one byte hashing to **19 000%** for 1 000 bytes hashing with `fnv0_64`)
+
+Differences with `pyhash` (on `fnv0_64`) are shown with the following diagram:
+
+![](bench.png)
+
+### Influence of string size on `fnv-c` hashing speed (on a Macbook Pro M1 (2020) with `fnv0_64`)
+
+![](bench2.png)
+
+## How to install/use it?
+
+```
+pip install fnv-c
+```
+
+```python
+import fnv_c
+
+print(fnv_c.fnv0_32(b"foo bar"))
+print(fnv_c.fnv0_64(b"foo bar"))
+print(fnv_c.fnv1_32(b"foo bar"))
+print(fnv_c.fnv1_64(b"foo bar"))
+print(fnv_c.fnv1a_32(b"foo bar"))
+print(fnv_c.fnv1a_64(b"foo bar"))
+```
+
+## Function signatures / API
+
+Full API doc is available at: [https://botify-labs.github.io/fnv-c/fnv_c/](https://botify-labs.github.io/fnv-c/fnv_c/)
+
+## Dev
+
+See [this specific document](DEV.md)
```

### Comparing `fnv-c-0.1.7/fnv_c/__init__.py` & `fnv-c-0.2.0/fnv_c/__init__.py`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.7/fnv_c/ext/build.py` & `fnv-c-0.2.0/fnv_c/ext/build.py`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.7/fnv_c/ext/fnv.c` & `fnv-c-0.2.0/fnv_c/ext/fnv.c`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.7/fnv_c.egg-info/PKG-INFO` & `fnv-c-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnv-c
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python 3.7+ FNV (fnv0, fnv1, fnv1a) non-cryptographic hash library implemented in C through libffi
 Home-page: https://github.com/botify-labs/fnv-c
 Author: Fabien MARTY
 Author-email: fabien.marty@botify.com
 License: UNKNOWN
 Description: # fnv-c
         
@@ -23,23 +23,44 @@
         - it's very fast
         - it's very easy to implement *(even in some exotic stored procedures for example)* so you can use it everywhere
         
         More details on [this Wikepedia article](https://en.wikipedia.org/wiki/Fowler%E2%80%93Noll%E2%80%93Vo_hash_function).
         
         ## Features
         
-        - speed: **4 000%** faster than basic Python implementation, **40%** faster than `pyhash`
+        - speed: 
+            - up to **800 MB/s** hashing speed *(on Macbook Pro M1 (2020) with `fnv0_64`)*
+            - **6 800%** faster than basic Python implementation, **70%** faster than `pyhash` *(when hashing 100 bytes with `fnv0_64` on a cloud VM)*
         - portability:
             - tested with recent Python versions (3.7+)
-            - compatible with ARM64 and avoid too agressive CPU optimizations for maximizing binary portability 
-            - compatible with PyPy
+            - compatible with ARM64
+            - compatible (and tested) with PyPy
         
         ## Non features
         
-        - other hash algorithms (this library is only about FNV algorithm)
+        - other hash algorithms *(this library is only about FNV algorithm)*
+        - too agressive CPU optimizations *(we prefer maximizing binary portability)*
+        
+        ## Benchmark
+        
+        You have a benchmark script [here](bench.py) to bench `fnv-c` by yourself and to compare it with:
+        - [`fnvhash`](https://github.com/znerol/py-fnvhash) (pure python implementation)
+        - [`pyhash`](https://github.com/flier/pyfasthash) (more general hashing library with C++ extension)
+        
+        ### Comparisons with other libraries (`fnv0_64` on a cloud VM)
+        
+        Differences with `fnvhash` are huge (from **35%** for one byte hashing to **19 000%** for 1 000 bytes hashing with `fnv0_64`)
+        
+        Differences with `pyhash` (on `fnv0_64`) are shown with the following diagram:
+        
+        ![](bench.png)
+        
+        ### Influence of string size on `fnv-c` hashing speed (on a Macbook Pro M1 (2020) with `fnv0_64`)
+        
+        ![](bench2.png)
         
         ## How to install/use it?
         
         ```
         pip install fnv-c
         ```
         
@@ -57,13 +78,14 @@
         ## Function signatures / API
         
         Full API doc is available at: [https://botify-labs.github.io/fnv-c/fnv_c/](https://botify-labs.github.io/fnv-c/fnv_c/)
         
         ## Dev
         
         See [this specific document](DEV.md)
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `fnv-c-0.1.7/setup.py` & `fnv-c-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.1.7"
+VERSION = "0.2.0"
 
 DESCRIPTION = "Python 3.7+ FNV (fnv0, fnv1, fnv1a) non-cryptographic hash library implemented in C through libffi"
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 
 setup(
```

