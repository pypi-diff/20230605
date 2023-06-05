# Comparing `tmp/bpc-walrus-0.1.5.tar.gz` & `tmp/bpc-walrus-0.1.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bpc-walrus-0.1.5.tar", last modified: Mon Jun  5 10:08:45 2023, max compression
+gzip compressed data, was "bpc-walrus-0.1.5rc1.tar", last modified: Thu Aug  4 23:33:30 2022, max compression
```

## Comparing `bpc-walrus-0.1.5.tar` & `bpc-walrus-0.1.5rc1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1099 2021-04-05 09:04:49.000000 bpc-walrus-0.1.5/LICENSE
--rw-r--r--   0 jarryshaw   (501) staff       (20)       32 2021-04-02 14:53:19.000000 bpc-walrus-0.1.5/MANIFEST.in
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3234 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/PKG-INFO
--rw-r--r--   0 jarryshaw   (501) staff       (20)     2077 2021-04-05 09:04:49.000000 bpc-walrus-0.1.5/README.md
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/bpc_walrus.egg-info/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3234 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/bpc_walrus.egg-info/PKG-INFO
--rw-r--r--   0 jarryshaw   (501) staff       (20)      337 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/bpc_walrus.egg-info/SOURCES.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)        1 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/bpc_walrus.egg-info/dependency_links.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)       39 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/bpc_walrus.egg-info/entry_points.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)      306 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/bpc_walrus.egg-info/requires.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)        7 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/bpc_walrus.egg-info/top_level.txt
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/docs/
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/docs/source/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3744 2021-04-05 09:04:49.000000 bpc-walrus-0.1.5/docs/source/conf.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      233 2020-11-22 15:08:09.000000 bpc-walrus-0.1.5/pyproject.toml
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/scripts/
--rw-r--r--   0 jarryshaw   (501) staff       (20)      497 2021-04-02 14:50:42.000000 bpc-walrus-0.1.5/scripts/find_version.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      102 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/setup.cfg
--rw-r--r--   0 jarryshaw   (501) staff       (20)     2574 2023-06-05 10:08:20.000000 bpc-walrus-0.1.5/setup.py
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2023-06-05 10:08:45.000000 bpc-walrus-0.1.5/tests/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     6723 2020-11-22 15:08:09.000000 bpc-walrus-0.1.5/tests/test.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    80335 2023-06-05 10:08:20.000000 bpc-walrus-0.1.5/walrus.py
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-08-04 23:33:30.179967 bpc-walrus-0.1.5rc1/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     1099 2021-04-05 09:04:49.000000 bpc-walrus-0.1.5rc1/LICENSE
+-rw-r--r--   0 jarryshaw   (501) staff       (20)       32 2021-04-02 14:53:19.000000 bpc-walrus-0.1.5rc1/MANIFEST.in
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3237 2022-08-04 23:33:30.180117 bpc-walrus-0.1.5rc1/PKG-INFO
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2077 2021-04-05 09:04:49.000000 bpc-walrus-0.1.5rc1/README.md
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-08-04 23:33:30.178926 bpc-walrus-0.1.5rc1/bpc_walrus.egg-info/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3237 2022-08-04 23:33:29.000000 bpc-walrus-0.1.5rc1/bpc_walrus.egg-info/PKG-INFO
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      323 2022-08-04 23:33:30.000000 bpc-walrus-0.1.5rc1/bpc_walrus.egg-info/SOURCES.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        1 2022-08-04 23:33:29.000000 bpc-walrus-0.1.5rc1/bpc_walrus.egg-info/dependency_links.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)       39 2022-08-04 23:33:29.000000 bpc-walrus-0.1.5rc1/bpc_walrus.egg-info/entry_points.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      302 2022-08-04 23:33:29.000000 bpc-walrus-0.1.5rc1/bpc_walrus.egg-info/requires.txt
+-rw-r--r--   0 jarryshaw   (501) staff       (20)        7 2022-08-04 23:33:30.000000 bpc-walrus-0.1.5rc1/bpc_walrus.egg-info/top_level.txt
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-08-04 23:33:30.174539 bpc-walrus-0.1.5rc1/docs/
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-08-04 23:33:30.179361 bpc-walrus-0.1.5rc1/docs/source/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     3744 2021-04-05 09:04:49.000000 bpc-walrus-0.1.5rc1/docs/source/conf.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      233 2020-11-22 15:08:09.000000 bpc-walrus-0.1.5rc1/pyproject.toml
+drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-08-04 23:33:30.179683 bpc-walrus-0.1.5rc1/scripts/
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      497 2021-04-02 14:50:42.000000 bpc-walrus-0.1.5rc1/scripts/find_version.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)      102 2022-08-04 23:33:30.180585 bpc-walrus-0.1.5rc1/setup.cfg
+-rw-r--r--   0 jarryshaw   (501) staff       (20)     2574 2021-04-05 09:04:49.000000 bpc-walrus-0.1.5rc1/setup.py
+-rw-r--r--   0 jarryshaw   (501) staff       (20)    80338 2021-03-25 14:53:08.000000 bpc-walrus-0.1.5rc1/walrus.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bpc-walrus-0.1.5/LICENSE` & `bpc-walrus-0.1.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `bpc-walrus-0.1.5/PKG-INFO` & `bpc-walrus-0.1.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpc-walrus
-Version: 0.1.5
+Version: 0.1.5rc1
 Summary: Backport compiler for Python 3.8 assignment expressions.
 Home-page: https://github.com/pybpc/walrus
 Author: Jarry Shaw
 Author-email: jarryshaw@icloud.com
 License: MIT
 Keywords: walrus operator,assignment expression,back-port compiler
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bpc-walrus-0.1.5/README.md` & `bpc-walrus-0.1.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `bpc-walrus-0.1.5/bpc_walrus.egg-info/PKG-INFO` & `bpc-walrus-0.1.5rc1/bpc_walrus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpc-walrus
-Version: 0.1.5
+Version: 0.1.5rc1
 Summary: Backport compiler for Python 3.8 assignment expressions.
 Home-page: https://github.com/pybpc/walrus
 Author: Jarry Shaw
 Author-email: jarryshaw@icloud.com
 License: MIT
 Keywords: walrus operator,assignment expression,back-port compiler
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bpc-walrus-0.1.5/docs/source/conf.py` & `bpc-walrus-0.1.5rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bpc-walrus-0.1.5/setup.py` & `bpc-walrus-0.1.5rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ],
     keywords=['walrus operator', 'assignment expression', 'back-port compiler'],
     py_modules=[module_name],
     python_requires='>=3.4',
     install_requires=[
         'parso>=0.6.0',         # universal AST support
         'tbtrim>=0.2.1',        # traceback trim support
-        'bpc-f2format',         # bpc-f2format
+        'f2format',             # bpc-f2format
         'bpc-utils~=0.10.0',    # utility library
         'typing;python_version<"3.5"',
         'typing_extensions',
     ],
     extras_require={
         'lint': [
             'flake8',
```

### Comparing `bpc-walrus-0.1.5/walrus.py` & `bpc-walrus-0.1.5rc1/walrus.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                        recover_files)
 from bpc_utils import Linesep
 from typing_extensions import Literal, TypedDict, final
 
 __all__ = ['main', 'walrus', 'convert']
 
 # version string
-__version__ = '0.1.5'
+__version__ = '0.1.5rc1'
 
 ###############################################################################
 # Types for annotation
 
 ScopeKeyword = Literal['global', 'nonlocal']
```

