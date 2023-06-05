# Comparing `tmp/generalvector-1.5.8.tar.gz` & `tmp/generalvector-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalvector-1.5.8.tar", last modified: Fri Feb 26 14:48:50 2021, max compression
+gzip compressed data, was "generalvector-1.5.9.tar", last modified: Sat Apr 10 12:44:30 2021, max compression
```

## Comparing `generalvector-1.5.8.tar` & `generalvector-1.5.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 14:48:50.144915 generalvector-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-02-26 14:46:19.000000 generalvector-1.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7841 2021-02-26 14:48:50.144915 generalvector-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6683 2021-02-26 14:48:44.000000 generalvector-1.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 14:48:50.144915 generalvector-1.5.8/generalvector/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-02-26 14:44:44.000000 generalvector-1.5.8/generalvector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2021-02-26 14:44:44.000000 generalvector-1.5.8/generalvector/general.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 14:48:50.144915 generalvector-1.5.8/generalvector/test/
--rw-r--r--   0 runner    (1001) docker     (121)    12766 2021-02-26 14:44:44.000000 generalvector-1.5.8/generalvector/test/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (121)    10881 2021-02-26 14:44:44.000000 generalvector-1.5.8/generalvector/test/test_vector2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5622 2021-02-26 14:44:44.000000 generalvector-1.5.8/generalvector/vector.py
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2021-02-26 14:44:44.000000 generalvector-1.5.8/generalvector/vector2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-26 14:48:50.144915 generalvector-1.5.8/generalvector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7841 2021-02-26 14:48:50.000000 generalvector-1.5.8/generalvector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      397 2021-02-26 14:48:50.000000 generalvector-1.5.8/generalvector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-26 14:48:50.000000 generalvector-1.5.8/generalvector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-02-26 14:48:50.000000 generalvector-1.5.8/generalvector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-02-26 14:48:50.000000 generalvector-1.5.8/generalvector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-02-26 14:44:48.000000 generalvector-1.5.8/metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-26 14:48:50.144915 generalvector-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      969 2021-02-26 14:46:21.000000 generalvector-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-10 12:44:30.059452 generalvector-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-04-10 12:43:23.000000 generalvector-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6997 2021-04-10 12:44:30.059452 generalvector-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5887 2021-04-10 12:44:25.000000 generalvector-1.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-10 12:44:30.055452 generalvector-1.5.9/generalvector/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-04-10 12:43:14.000000 generalvector-1.5.9/generalvector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3638 2021-04-10 12:43:14.000000 generalvector-1.5.9/generalvector/general.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-10 12:44:30.059452 generalvector-1.5.9/generalvector/test/
+-rw-r--r--   0 runner    (1001) docker     (121)    12766 2021-04-10 12:43:14.000000 generalvector-1.5.9/generalvector/test/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10881 2021-04-10 12:43:14.000000 generalvector-1.5.9/generalvector/test/test_vector2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5622 2021-04-10 12:43:14.000000 generalvector-1.5.9/generalvector/vector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5083 2021-04-10 12:43:14.000000 generalvector-1.5.9/generalvector/vector2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-10 12:44:30.055452 generalvector-1.5.9/generalvector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6997 2021-04-10 12:44:29.000000 generalvector-1.5.9/generalvector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2021-04-10 12:44:29.000000 generalvector-1.5.9/generalvector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-10 12:44:29.000000 generalvector-1.5.9/generalvector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-04-10 12:44:29.000000 generalvector-1.5.9/generalvector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-04-10 12:44:29.000000 generalvector-1.5.9/generalvector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-04-10 12:43:14.000000 generalvector-1.5.9/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-10 12:44:30.059452 generalvector-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      969 2021-04-10 12:43:24.000000 generalvector-1.5.9/setup.py
```

### Comparing `generalvector-1.5.8/PKG-INFO` & `generalvector-1.5.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: generalvector
-Version: 1.5.8
+Version: 1.5.9
 Summary: Simple immutable vectors.
 Home-page: https://github.com/ManderaGeneral/generalvector
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Description: # generalvector
         Simple immutable vectors.
         
         This package and 3 other make up [ManderaGeneral](https://github.com/Mandera).
         
         ## Information
-        | Package                                                          | Ver                                              | Latest Release       | Python                                                                                                                   | Platform        |   Lvl | Todo                                                      | Tests   |
-        |:-----------------------------------------------------------------|:-------------------------------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:----------------------------------------------------------|:--------|
-        | [generalvector](https://github.com/ManderaGeneral/generalvector) | [1.5.8](https://pypi.org/project/generalvector/) | 2021-02-26 15:48 CET | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     1 | [1](https://github.com/ManderaGeneral/generalvector#Todo) | 100.0 % |
+        | Package                                                          | Ver                                              | Latest Release        | Python                                                                                                                   | Platform        |   Lvl | Todo                                                      | Tests   |
+        |:-----------------------------------------------------------------|:-------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:----------------------------------------------------------|:--------|
+        | [generalvector](https://github.com/ManderaGeneral/generalvector) | [1.5.9](https://pypi.org/project/generalvector/) | 2021-04-10 14:44 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     1 | [1](https://github.com/ManderaGeneral/generalvector#Todo) | 100.0 % |
         
         ## Contents
         <pre>
         <a href='#generalvector'>generalvector</a>
         ├─ <a href='#Information'>Information</a>
         ├─ <a href='#Contents'>Contents</a>
         ├─ <a href='#Installation'>Installation</a>
@@ -29,53 +29,47 @@
         ## Installation
         | Command                     | <a href='https://pypi.org/project/generallibrary'>generallibrary</a>   |
         |:----------------------------|:-----------------------------------------------------------------------|
         | `pip install generalvector` | Yes                                                                    |
         
         ## Attributes
         <pre>
-        <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/__init__.py#L1'>Module: generalvector</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L10'>Class: Vec</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L92'>Method: absolute</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L122'>Method: clamp</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L77'>Method: confineTo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L168'>Method: distance</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L142'>Method: hex</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L133'>Method: inrange</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L67'>Method: length</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L113'>Method: max</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L104'>Method: min</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L73'>Method: normalized</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L88'>Method: random</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L149'>Method: range</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L82'>Method: round</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L40'>Method: sanitize</a>
-        └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L9'>Class: Vec2</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L92'>Method: absolute</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L122'>Method: clamp</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L77'>Method: confineTo</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L161'>Method: distance</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L132'>Method: inrange</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L67'>Method: length</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L113'>Method: max</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L104'>Method: min</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L73'>Method: normalized</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L88'>Method: random</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L143'>Method: range</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L82'>Method: round</a>
-           └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L40'>Method: sanitize</a>
+        <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/__init__.py#L1'>Module: generalvector</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L10'>Class: Vec</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L122'>Method: clamp</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L168'>Method: distance</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L142'>Method: hex</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L133'>Method: inrange</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L67'>Method: length</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L113'>Method: max</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L104'>Method: min</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L73'>Method: normalized</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L88'>Method: random</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L149'>Method: range</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L82'>Method: round</a>
+        └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L9'>Class: Vec2</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L122'>Method: clamp</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L161'>Method: distance</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L132'>Method: inrange</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L67'>Method: length</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L113'>Method: max</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L104'>Method: min</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L73'>Method: normalized</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L88'>Method: random</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L143'>Method: range</a>
+           └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L82'>Method: round</a>
         </pre>
         
         ## Todo
-        | Module                                                                                                            | Message                                                                                                                                     |
-        |:------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------|
-        | <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L1'>general.py</a> | <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L7'>Move most methods to _GeneralVector.</a> |
+        | Module                                                                                                           | Message                                                                                                                                    |
+        |:-----------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------|
+        | <a href='https://github.com/ManderaGeneral/generalvector/blob/master/generalvector/general.py#L1'>general.py</a> | <a href='https://github.com/ManderaGeneral/generalvector/blob/master/generalvector/general.py#L7'>Move most methods to _GeneralVector.</a> |
         
         <sup>
-        Generated 2021-02-26 15:48 CET for commit <a href='https://github.com/ManderaGeneral/generalvector/commit/c269098'>c269098</a>.
+        Generated 2021-04-10 14:44 CEST for commit <a href='https://github.com/ManderaGeneral/generalvector/commit/f4087ba'>f4087ba</a>.
         </sup>
         
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,65 +1,59 @@
-Metadata-Version: 2.1 Name: generalvector Version: 1.5.8 Summary: Simple
+Metadata-Version: 2.1 Name: generalvector Version: 1.5.9 Summary: Simple
 immutable vectors. Home-page: https://github.com/ManderaGeneral/generalvector
 Author: Rickard "Mandera" Abraham Author-email: rickard.abraham@gmail.com
 License: mit Description: # generalvector Simple immutable vectors. This
 package and 3 other make up [ManderaGeneral](https://github.com/Mandera). ##
 Information | Package | Ver | Latest Release | Python | Platform | Lvl | Todo |
 Tests | |:-----------------------------------------------------------------|:--
------------------------------------------------|:---------------------|:-------
+-----------------------------------------------|:----------------------|:------
 -------------------------------------------------------------------------------
------------------------------------|:----------------|------:|:----------------
-------------------------------------------|:--------| | [generalvector](https:/
-/github.com/ManderaGeneral/generalvector) | [1.5.8](https://pypi.org/project/
-generalvector/) | 2021-02-26 15:48 CET | [3.8](https://www.python.org/
+------------------------------------|:----------------|------:|:---------------
+-------------------------------------------|:--------| | [generalvector](https:
+//github.com/ManderaGeneral/generalvector) | [1.5.9](https://pypi.org/project/
+generalvector/) | 2021-04-10 14:44 CEST | [3.8](https://www.python.org/
 downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/
 python-390/) | Windows, Ubuntu | 1 | [1](https://github.com/ManderaGeneral/
 generalvector#Todo) | 100.0 % | ## Contents
         generalvector
         ââ Information
         ââ Contents
         ââ Installation
         ââ Attributes
         ââ Todo
 ## Installation | Command | generallibrary | |:----------------------------|:--
 ---------------------------------------------------------------------| | `pip
 install generalvector` | Yes | ## Attributes
         Module:_generalvector
         ââ Class:_Vec
-        â  ââ Method:_absolute
         â  ââ Method:_clamp
-        â  ââ Method:_confineTo
         â  ââ Method:_distance
         â  ââ Method:_hex
         â  ââ Method:_inrange
         â  ââ Method:_length
         â  ââ Method:_max
         â  ââ Method:_min
         â  ââ Method:_normalized
         â  ââ Method:_random
         â  ââ Method:_range
-        â  ââ Method:_round
-        â  ââ Method:_sanitize
+        â  ââ Method:_round
         ââ Class:_Vec2
-           ââ Method:_absolute
            ââ Method:_clamp
-           ââ Method:_confineTo
            ââ Method:_distance
            ââ Method:_inrange
            ââ Method:_length
            ââ Method:_max
            ââ Method:_min
            ââ Method:_normalized
            ââ Method:_random
            ââ Method:_range
-           ââ Method:_round
-           ââ Method:_sanitize
+           ââ Method:_round
 ## Todo | Module | Message | |:------------------------------------------------
-------------------------------------------------------------------|:-----------
+-----------------------------------------------------------------|:------------
 -------------------------------------------------------------------------------
---------------------------------------------------| | general.py | Move_most
-methods_to__GeneralVector. | Generated 2021-02-26 15:48 CET for commit c269098.
-Platform: UNKNOWN Classifier: Topic :: Utilities Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8, <3.10 Description-Content-Type: text/markdown
+------------------------------------------------| | general.py | Move_most
+methods_to__GeneralVector. | Generated 2021-04-10 14:44 CEST for commit
+f4087ba. Platform: UNKNOWN Classifier: Topic :: Utilities Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
+:: Linux Requires-Python: >=3.8, <3.10 Description-Content-Type: text/markdown
```

### Comparing `generalvector-1.5.8/README.md` & `generalvector-1.5.9/generalvector.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,79 @@
-# generalvector
-Simple immutable vectors.
-
-This package and 3 other make up [ManderaGeneral](https://github.com/Mandera).
-
-## Information
-| Package                                                          | Ver                                              | Latest Release       | Python                                                                                                                   | Platform        |   Lvl | Todo                                                      | Tests   |
-|:-----------------------------------------------------------------|:-------------------------------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:----------------------------------------------------------|:--------|
-| [generalvector](https://github.com/ManderaGeneral/generalvector) | [1.5.8](https://pypi.org/project/generalvector/) | 2021-02-26 15:48 CET | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     1 | [1](https://github.com/ManderaGeneral/generalvector#Todo) | 100.0 % |
-
-## Contents
-<pre>
-<a href='#generalvector'>generalvector</a>
-├─ <a href='#Information'>Information</a>
-├─ <a href='#Contents'>Contents</a>
-├─ <a href='#Installation'>Installation</a>
-├─ <a href='#Attributes'>Attributes</a>
-└─ <a href='#Todo'>Todo</a>
-</pre>
-
-## Installation
-| Command                     | <a href='https://pypi.org/project/generallibrary'>generallibrary</a>   |
-|:----------------------------|:-----------------------------------------------------------------------|
-| `pip install generalvector` | Yes                                                                    |
-
-## Attributes
-<pre>
-<a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/__init__.py#L1'>Module: generalvector</a>
-├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L10'>Class: Vec</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L92'>Method: absolute</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L122'>Method: clamp</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L77'>Method: confineTo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L168'>Method: distance</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L142'>Method: hex</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L133'>Method: inrange</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L67'>Method: length</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L113'>Method: max</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L104'>Method: min</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L73'>Method: normalized</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L88'>Method: random</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L149'>Method: range</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L82'>Method: round</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L40'>Method: sanitize</a>
-└─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L9'>Class: Vec2</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L92'>Method: absolute</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L122'>Method: clamp</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L77'>Method: confineTo</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L161'>Method: distance</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L132'>Method: inrange</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L67'>Method: length</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L113'>Method: max</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L104'>Method: min</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L73'>Method: normalized</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L88'>Method: random</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L143'>Method: range</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L82'>Method: round</a>
-   └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L40'>Method: sanitize</a>
-</pre>
-
-## Todo
-| Module                                                                                                            | Message                                                                                                                                     |
-|:------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------|
-| <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L1'>general.py</a> | <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L7'>Move most methods to _GeneralVector.</a> |
-
-<sup>
-Generated 2021-02-26 15:48 CET for commit <a href='https://github.com/ManderaGeneral/generalvector/commit/c269098'>c269098</a>.
-</sup>
+Metadata-Version: 2.1
+Name: generalvector
+Version: 1.5.9
+Summary: Simple immutable vectors.
+Home-page: https://github.com/ManderaGeneral/generalvector
+Author: Rickard "Mandera" Abraham
+Author-email: rickard.abraham@gmail.com
+License: mit
+Description: # generalvector
+        Simple immutable vectors.
+        
+        This package and 3 other make up [ManderaGeneral](https://github.com/Mandera).
+        
+        ## Information
+        | Package                                                          | Ver                                              | Latest Release        | Python                                                                                                                   | Platform        |   Lvl | Todo                                                      | Tests   |
+        |:-----------------------------------------------------------------|:-------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:----------------------------------------------------------|:--------|
+        | [generalvector](https://github.com/ManderaGeneral/generalvector) | [1.5.9](https://pypi.org/project/generalvector/) | 2021-04-10 14:44 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     1 | [1](https://github.com/ManderaGeneral/generalvector#Todo) | 100.0 % |
+        
+        ## Contents
+        <pre>
+        <a href='#generalvector'>generalvector</a>
+        ├─ <a href='#Information'>Information</a>
+        ├─ <a href='#Contents'>Contents</a>
+        ├─ <a href='#Installation'>Installation</a>
+        ├─ <a href='#Attributes'>Attributes</a>
+        └─ <a href='#Todo'>Todo</a>
+        </pre>
+        
+        ## Installation
+        | Command                     | <a href='https://pypi.org/project/generallibrary'>generallibrary</a>   |
+        |:----------------------------|:-----------------------------------------------------------------------|
+        | `pip install generalvector` | Yes                                                                    |
+        
+        ## Attributes
+        <pre>
+        <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/__init__.py#L1'>Module: generalvector</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L10'>Class: Vec</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L122'>Method: clamp</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L168'>Method: distance</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L142'>Method: hex</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L133'>Method: inrange</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L67'>Method: length</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L113'>Method: max</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L104'>Method: min</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L73'>Method: normalized</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L88'>Method: random</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L149'>Method: range</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L82'>Method: round</a>
+        └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L9'>Class: Vec2</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L122'>Method: clamp</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L161'>Method: distance</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L132'>Method: inrange</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L67'>Method: length</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L113'>Method: max</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L104'>Method: min</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L73'>Method: normalized</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L88'>Method: random</a>
+           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L143'>Method: range</a>
+           └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L82'>Method: round</a>
+        </pre>
+        
+        ## Todo
+        | Module                                                                                                           | Message                                                                                                                                    |
+        |:-----------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------|
+        | <a href='https://github.com/ManderaGeneral/generalvector/blob/master/generalvector/general.py#L1'>general.py</a> | <a href='https://github.com/ManderaGeneral/generalvector/blob/master/generalvector/general.py#L7'>Move most methods to _GeneralVector.</a> |
+        
+        <sup>
+        Generated 2021-04-10 14:44 CEST for commit <a href='https://github.com/ManderaGeneral/generalvector/commit/f4087ba'>f4087ba</a>.
+        </sup>
+        
+Platform: UNKNOWN
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8, <3.10
+Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,57 +1,59 @@
-# generalvector Simple immutable vectors. This package and 3 other make up
-[ManderaGeneral](https://github.com/Mandera). ## Information | Package | Ver |
-Latest Release | Python | Platform | Lvl | Todo | Tests | |:-------------------
-----------------------------------------------|:-------------------------------
-------------------|:---------------------|:------------------------------------
+Metadata-Version: 2.1 Name: generalvector Version: 1.5.9 Summary: Simple
+immutable vectors. Home-page: https://github.com/ManderaGeneral/generalvector
+Author: Rickard "Mandera" Abraham Author-email: rickard.abraham@gmail.com
+License: mit Description: # generalvector Simple immutable vectors. This
+package and 3 other make up [ManderaGeneral](https://github.com/Mandera). ##
+Information | Package | Ver | Latest Release | Python | Platform | Lvl | Todo |
+Tests | |:-----------------------------------------------------------------|:--
+-----------------------------------------------|:----------------------|:------
 -------------------------------------------------------------------------------
-------|:----------------|------:|:---------------------------------------------
--------------|:--------| | [generalvector](https://github.com/ManderaGeneral/
-generalvector) | [1.5.8](https://pypi.org/project/generalvector/) | 2021-02-26
-15:48 CET | [3.8](https://www.python.org/downloads/release/python-380/), [3.9]
-(https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu | 1 |
-[1](https://github.com/ManderaGeneral/generalvector#Todo) | 100.0 % | ##
-Contents
-generalvector
-ââ Information
-ââ Contents
-ââ Installation
-ââ Attributes
-ââ Todo
+------------------------------------|:----------------|------:|:---------------
+-------------------------------------------|:--------| | [generalvector](https:
+//github.com/ManderaGeneral/generalvector) | [1.5.9](https://pypi.org/project/
+generalvector/) | 2021-04-10 14:44 CEST | [3.8](https://www.python.org/
+downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/
+python-390/) | Windows, Ubuntu | 1 | [1](https://github.com/ManderaGeneral/
+generalvector#Todo) | 100.0 % | ## Contents
+        generalvector
+        ââ Information
+        ââ Contents
+        ââ Installation
+        ââ Attributes
+        ââ Todo
 ## Installation | Command | generallibrary | |:----------------------------|:--
 ---------------------------------------------------------------------| | `pip
 install generalvector` | Yes | ## Attributes
-Module:_generalvector
-ââ Class:_Vec
-â  ââ Method:_absolute
-â  ââ Method:_clamp
-â  ââ Method:_confineTo
-â  ââ Method:_distance
-â  ââ Method:_hex
-â  ââ Method:_inrange
-â  ââ Method:_length
-â  ââ Method:_max
-â  ââ Method:_min
-â  ââ Method:_normalized
-â  ââ Method:_random
-â  ââ Method:_range
-â  ââ Method:_round
-â  ââ Method:_sanitize
-ââ Class:_Vec2
-   ââ Method:_absolute
-   ââ Method:_clamp
-   ââ Method:_confineTo
-   ââ Method:_distance
-   ââ Method:_inrange
-   ââ Method:_length
-   ââ Method:_max
-   ââ Method:_min
-   ââ Method:_normalized
-   ââ Method:_random
-   ââ Method:_range
-   ââ Method:_round
-   ââ Method:_sanitize
+        Module:_generalvector
+        ââ Class:_Vec
+        â  ââ Method:_clamp
+        â  ââ Method:_distance
+        â  ââ Method:_hex
+        â  ââ Method:_inrange
+        â  ââ Method:_length
+        â  ââ Method:_max
+        â  ââ Method:_min
+        â  ââ Method:_normalized
+        â  ââ Method:_random
+        â  ââ Method:_range
+        â  ââ Method:_round
+        ââ Class:_Vec2
+           ââ Method:_clamp
+           ââ Method:_distance
+           ââ Method:_inrange
+           ââ Method:_length
+           ââ Method:_max
+           ââ Method:_min
+           ââ Method:_normalized
+           ââ Method:_random
+           ââ Method:_range
+           ââ Method:_round
 ## Todo | Module | Message | |:------------------------------------------------
-------------------------------------------------------------------|:-----------
+-----------------------------------------------------------------|:------------
 -------------------------------------------------------------------------------
---------------------------------------------------| | general.py | Move_most
-methods_to__GeneralVector. | Generated 2021-02-26 15:48 CET for commit c269098.
+------------------------------------------------| | general.py | Move_most
+methods_to__GeneralVector. | Generated 2021-04-10 14:44 CEST for commit
+f4087ba. Platform: UNKNOWN Classifier: Topic :: Utilities Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
+:: Linux Requires-Python: >=3.8, <3.10 Description-Content-Type: text/markdown
```

### Comparing `generalvector-1.5.8/generalvector/general.py` & `generalvector-1.5.9/generalvector/general.py`

 * *Files identical despite different names*

### Comparing `generalvector-1.5.8/generalvector/test/test_vector.py` & `generalvector-1.5.9/generalvector/test/test_vector.py`

 * *Files identical despite different names*

### Comparing `generalvector-1.5.8/generalvector/test/test_vector2.py` & `generalvector-1.5.9/generalvector/test/test_vector2.py`

 * *Files identical despite different names*

### Comparing `generalvector-1.5.8/generalvector/vector.py` & `generalvector-1.5.9/generalvector/vector.py`

 * *Files identical despite different names*

### Comparing `generalvector-1.5.8/generalvector/vector2.py` & `generalvector-1.5.9/generalvector/vector2.py`

 * *Files identical despite different names*

### Comparing `generalvector-1.5.8/generalvector.egg-info/PKG-INFO` & `generalvector-1.5.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,61 @@
-Metadata-Version: 2.1
-Name: generalvector
-Version: 1.5.8
-Summary: Simple immutable vectors.
-Home-page: https://github.com/ManderaGeneral/generalvector
-Author: Rickard "Mandera" Abraham
-Author-email: rickard.abraham@gmail.com
-License: mit
-Description: # generalvector
-        Simple immutable vectors.
-        
-        This package and 3 other make up [ManderaGeneral](https://github.com/Mandera).
-        
-        ## Information
-        | Package                                                          | Ver                                              | Latest Release       | Python                                                                                                                   | Platform        |   Lvl | Todo                                                      | Tests   |
-        |:-----------------------------------------------------------------|:-------------------------------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:----------------------------------------------------------|:--------|
-        | [generalvector](https://github.com/ManderaGeneral/generalvector) | [1.5.8](https://pypi.org/project/generalvector/) | 2021-02-26 15:48 CET | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     1 | [1](https://github.com/ManderaGeneral/generalvector#Todo) | 100.0 % |
-        
-        ## Contents
-        <pre>
-        <a href='#generalvector'>generalvector</a>
-        ├─ <a href='#Information'>Information</a>
-        ├─ <a href='#Contents'>Contents</a>
-        ├─ <a href='#Installation'>Installation</a>
-        ├─ <a href='#Attributes'>Attributes</a>
-        └─ <a href='#Todo'>Todo</a>
-        </pre>
-        
-        ## Installation
-        | Command                     | <a href='https://pypi.org/project/generallibrary'>generallibrary</a>   |
-        |:----------------------------|:-----------------------------------------------------------------------|
-        | `pip install generalvector` | Yes                                                                    |
-        
-        ## Attributes
-        <pre>
-        <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/__init__.py#L1'>Module: generalvector</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L10'>Class: Vec</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L92'>Method: absolute</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L122'>Method: clamp</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L77'>Method: confineTo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L168'>Method: distance</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L142'>Method: hex</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L133'>Method: inrange</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L67'>Method: length</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L113'>Method: max</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L104'>Method: min</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L73'>Method: normalized</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L88'>Method: random</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L149'>Method: range</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector.py#L82'>Method: round</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L40'>Method: sanitize</a>
-        └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L9'>Class: Vec2</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L92'>Method: absolute</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L122'>Method: clamp</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L77'>Method: confineTo</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L161'>Method: distance</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L132'>Method: inrange</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L67'>Method: length</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L113'>Method: max</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L104'>Method: min</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L73'>Method: normalized</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L88'>Method: random</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L143'>Method: range</a>
-           ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/vector2.py#L82'>Method: round</a>
-           └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L40'>Method: sanitize</a>
-        </pre>
-        
-        ## Todo
-        | Module                                                                                                            | Message                                                                                                                                     |
-        |:------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------|
-        | <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L1'>general.py</a> | <a href='https://github.com/ManderaGeneral/generalvector/blob/c269098/generalvector/general.py#L7'>Move most methods to _GeneralVector.</a> |
-        
-        <sup>
-        Generated 2021-02-26 15:48 CET for commit <a href='https://github.com/ManderaGeneral/generalvector/commit/c269098'>c269098</a>.
-        </sup>
-        
-Platform: UNKNOWN
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8, <3.10
-Description-Content-Type: text/markdown
+# generalvector
+Simple immutable vectors.
+
+This package and 3 other make up [ManderaGeneral](https://github.com/Mandera).
+
+## Information
+| Package                                                          | Ver                                              | Latest Release        | Python                                                                                                                   | Platform        |   Lvl | Todo                                                      | Tests   |
+|:-----------------------------------------------------------------|:-------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:----------------------------------------------------------|:--------|
+| [generalvector](https://github.com/ManderaGeneral/generalvector) | [1.5.9](https://pypi.org/project/generalvector/) | 2021-04-10 14:44 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu |     1 | [1](https://github.com/ManderaGeneral/generalvector#Todo) | 100.0 % |
+
+## Contents
+<pre>
+<a href='#generalvector'>generalvector</a>
+├─ <a href='#Information'>Information</a>
+├─ <a href='#Contents'>Contents</a>
+├─ <a href='#Installation'>Installation</a>
+├─ <a href='#Attributes'>Attributes</a>
+└─ <a href='#Todo'>Todo</a>
+</pre>
+
+## Installation
+| Command                     | <a href='https://pypi.org/project/generallibrary'>generallibrary</a>   |
+|:----------------------------|:-----------------------------------------------------------------------|
+| `pip install generalvector` | Yes                                                                    |
+
+## Attributes
+<pre>
+<a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/__init__.py#L1'>Module: generalvector</a>
+├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L10'>Class: Vec</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L122'>Method: clamp</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L168'>Method: distance</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L142'>Method: hex</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L133'>Method: inrange</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L67'>Method: length</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L113'>Method: max</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L104'>Method: min</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L73'>Method: normalized</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L88'>Method: random</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L149'>Method: range</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector.py#L82'>Method: round</a>
+└─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L9'>Class: Vec2</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L122'>Method: clamp</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L161'>Method: distance</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L132'>Method: inrange</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L67'>Method: length</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L113'>Method: max</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L104'>Method: min</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L73'>Method: normalized</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L88'>Method: random</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L143'>Method: range</a>
+   └─ <a href='https://github.com/ManderaGeneral/generalvector/blob/f4087ba/generalvector/vector2.py#L82'>Method: round</a>
+</pre>
+
+## Todo
+| Module                                                                                                           | Message                                                                                                                                    |
+|:-----------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------|
+| <a href='https://github.com/ManderaGeneral/generalvector/blob/master/generalvector/general.py#L1'>general.py</a> | <a href='https://github.com/ManderaGeneral/generalvector/blob/master/generalvector/general.py#L7'>Move most methods to _GeneralVector.</a> |
+
+<sup>
+Generated 2021-04-10 14:44 CEST for commit <a href='https://github.com/ManderaGeneral/generalvector/commit/f4087ba'>f4087ba</a>.
+</sup>
```

#### html2text {}

```diff
@@ -1,65 +1,52 @@
-Metadata-Version: 2.1 Name: generalvector Version: 1.5.8 Summary: Simple
-immutable vectors. Home-page: https://github.com/ManderaGeneral/generalvector
-Author: Rickard "Mandera" Abraham Author-email: rickard.abraham@gmail.com
-License: mit Description: # generalvector Simple immutable vectors. This
-package and 3 other make up [ManderaGeneral](https://github.com/Mandera). ##
-Information | Package | Ver | Latest Release | Python | Platform | Lvl | Todo |
-Tests | |:-----------------------------------------------------------------|:--
------------------------------------------------|:---------------------|:-------
+# generalvector Simple immutable vectors. This package and 3 other make up
+[ManderaGeneral](https://github.com/Mandera). ## Information | Package | Ver |
+Latest Release | Python | Platform | Lvl | Todo | Tests | |:-------------------
+----------------------------------------------|:-------------------------------
+------------------|:----------------------|:-----------------------------------
 -------------------------------------------------------------------------------
------------------------------------|:----------------|------:|:----------------
-------------------------------------------|:--------| | [generalvector](https:/
-/github.com/ManderaGeneral/generalvector) | [1.5.8](https://pypi.org/project/
-generalvector/) | 2021-02-26 15:48 CET | [3.8](https://www.python.org/
-downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/
-python-390/) | Windows, Ubuntu | 1 | [1](https://github.com/ManderaGeneral/
-generalvector#Todo) | 100.0 % | ## Contents
-        generalvector
-        ââ Information
-        ââ Contents
-        ââ Installation
-        ââ Attributes
-        ââ Todo
+-------|:----------------|------:|:--------------------------------------------
+--------------|:--------| | [generalvector](https://github.com/ManderaGeneral/
+generalvector) | [1.5.9](https://pypi.org/project/generalvector/) | 2021-04-10
+14:44 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9]
+(https://www.python.org/downloads/release/python-390/) | Windows, Ubuntu | 1 |
+[1](https://github.com/ManderaGeneral/generalvector#Todo) | 100.0 % | ##
+Contents
+generalvector
+ââ Information
+ââ Contents
+ââ Installation
+ââ Attributes
+ââ Todo
 ## Installation | Command | generallibrary | |:----------------------------|:--
 ---------------------------------------------------------------------| | `pip
 install generalvector` | Yes | ## Attributes
-        Module:_generalvector
-        ââ Class:_Vec
-        â  ââ Method:_absolute
-        â  ââ Method:_clamp
-        â  ââ Method:_confineTo
-        â  ââ Method:_distance
-        â  ââ Method:_hex
-        â  ââ Method:_inrange
-        â  ââ Method:_length
-        â  ââ Method:_max
-        â  ââ Method:_min
-        â  ââ Method:_normalized
-        â  ââ Method:_random
-        â  ââ Method:_range
-        â  ââ Method:_round
-        â  ââ Method:_sanitize
-        ââ Class:_Vec2
-           ââ Method:_absolute
-           ââ Method:_clamp
-           ââ Method:_confineTo
-           ââ Method:_distance
-           ââ Method:_inrange
-           ââ Method:_length
-           ââ Method:_max
-           ââ Method:_min
-           ââ Method:_normalized
-           ââ Method:_random
-           ââ Method:_range
-           ââ Method:_round
-           ââ Method:_sanitize
+Module:_generalvector
+ââ Class:_Vec
+â  ââ Method:_clamp
+â  ââ Method:_distance
+â  ââ Method:_hex
+â  ââ Method:_inrange
+â  ââ Method:_length
+â  ââ Method:_max
+â  ââ Method:_min
+â  ââ Method:_normalized
+â  ââ Method:_random
+â  ââ Method:_range
+â  ââ Method:_round
+ââ Class:_Vec2
+   ââ Method:_clamp
+   ââ Method:_distance
+   ââ Method:_inrange
+   ââ Method:_length
+   ââ Method:_max
+   ââ Method:_min
+   ââ Method:_normalized
+   ââ Method:_random
+   ââ Method:_range
+   ââ Method:_round
 ## Todo | Module | Message | |:------------------------------------------------
-------------------------------------------------------------------|:-----------
+-----------------------------------------------------------------|:------------
 -------------------------------------------------------------------------------
---------------------------------------------------| | general.py | Move_most
-methods_to__GeneralVector. | Generated 2021-02-26 15:48 CET for commit c269098.
-Platform: UNKNOWN Classifier: Topic :: Utilities Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8, <3.10 Description-Content-Type: text/markdown
+------------------------------------------------| | general.py | Move_most
+methods_to__GeneralVector. | Generated 2021-04-10 14:44 CEST for commit
+f4087ba.
```

### Comparing `generalvector-1.5.8/setup.py` & `generalvector-1.5.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_namespace_packages
 from pathlib import Path
 
 setup(
     name="generalvector",
     author='Rickard "Mandera" Abraham',
     author_email="rickard.abraham@gmail.com",
-    version="1.5.8",
+    version="1.5.9",
     description="Simple immutable vectors.",
     long_description=(Path(__file__).parent / 'README.md').read_text(encoding='utf-8'),
     long_description_content_type="text/markdown",
     install_requires=[
         'generallibrary',
     ],
     url="https://github.com/ManderaGeneral/generalvector",
```

