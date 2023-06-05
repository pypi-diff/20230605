# Comparing `tmp/generalimport-0.5.0.tar.gz` & `tmp/generalimport-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalimport-0.5.0.tar", last modified: Fri Jun  2 21:27:33 2023, max compression
+gzip compressed data, was "generalimport-0.5.1.tar", last modified: Mon Jun  5 09:31:03 2023, max compression
```

## Comparing `generalimport-0.5.0.tar` & `generalimport-0.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.632518 generalimport-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 21:27:04.000000 generalimport-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 21:27:04.000000 generalimport-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-06-02 21:27:33.632518 generalimport-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-02 21:27:06.000000 generalimport-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.628518 generalimport-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-02 21:25:00.000000 generalimport-0.5.0/examples/1minimal_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-02 21:25:00.000000 generalimport-0.5.0/examples/2tests_showcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-02 21:25:00.000000 generalimport-0.5.0/examples/3recommended_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-02 21:25:00.000000 generalimport-0.5.0/examples/4how_it_works.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.628518 generalimport-0.5.0/generalimport/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/dunders.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/fake_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/general_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/generalimport_bottom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/import_catcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/min.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.628518 generalimport-0.5.0/generalimport/test/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_generalimport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.632518 generalimport-0.5.0/generalimport/test/test_usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/top.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.628518 generalimport-0.5.0/generalimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-06-02 21:27:33.000000 generalimport-0.5.0/generalimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-02 21:27:33.000000 generalimport-0.5.0/generalimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:27:33.000000 generalimport-0.5.0/generalimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 21:27:33.000000 generalimport-0.5.0/generalimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-02 21:27:04.000000 generalimport-0.5.0/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:27:33.632518 generalimport-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-02 21:27:06.000000 generalimport-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:03.395982 generalimport-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 09:30:30.000000 generalimport-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 09:30:30.000000 generalimport-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-06-05 09:31:03.395982 generalimport-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-05 09:30:32.000000 generalimport-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:03.391982 generalimport-0.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-05 09:27:46.000000 generalimport-0.5.1/examples/1minimal_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-05 09:27:46.000000 generalimport-0.5.1/examples/2tests_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-05 09:27:46.000000 generalimport-0.5.1/examples/3recommended_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-05 09:27:46.000000 generalimport-0.5.1/examples/4how_it_works.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:03.391982 generalimport-0.5.1/generalimport/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/dunders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/fake_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/general_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/generalimport_bottom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/import_catcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/min.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:03.395982 generalimport-0.5.1/generalimport/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_generalimport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:03.395982 generalimport-0.5.1/generalimport/test/test_usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/test/test_usage/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-05 09:27:46.000000 generalimport-0.5.1/generalimport/top.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:03.395982 generalimport-0.5.1/generalimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-06-05 09:31:03.000000 generalimport-0.5.1/generalimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-05 09:31:03.000000 generalimport-0.5.1/generalimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:31:03.000000 generalimport-0.5.1/generalimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 09:31:03.000000 generalimport-0.5.1/generalimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-05 09:30:30.000000 generalimport-0.5.1/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:31:03.395982 generalimport-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-05 09:30:32.000000 generalimport-0.5.1/setup.py
```

### Comparing `generalimport-0.5.0/LICENSE` & `generalimport-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/PKG-INFO` & `generalimport-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generalimport
-Version: 0.5.0
+Version: 0.5.1
 Summary: Handle all your optional dependencies with a single call!
 Home-page: https://github.com/ManderaGeneral/generalimport
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -41,21 +41,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-2([library]) --> 5([packager])
 2([library]) --> 4([vector])
-3([file]) --> 5([packager])
-0([import]) --> 3([file])
 1([tool]) --> 2([library])
-0([import]) --> 2([library])
+3([file]) --> 5([packager])
 2([library]) --> 3([file])
+0([import]) --> 2([library])
+0([import]) --> 3([file])
+2([library]) --> 5([packager])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 0 fill:#482
@@ -73,15 +73,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                          | Ver                                              | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:-----------------------------------------------------------------|:-------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.5.0](https://pypi.org/project/generalimport/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 97.0 %  |
+| [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.5.1](https://pypi.org/project/generalimport/) | 2023-06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 97.2 %  |
 </details>
 
 
 <details open>
 <summary><h2>Examples</h2></summary>
 
 
@@ -197,15 +197,15 @@
 │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L25'>Method: catch</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L49'>Method: create_module</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L52'>Method: exec_module</a>
 │  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L33'>Method: find_spec</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L8'>Class: ImportCatcher</a>
 │  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L24'>Method: handle</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L30'>Class: MissingDependencyException</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L34'>Function: MissingOptionalDependency</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L34'>Class: MissingOptionalDependency</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L63'>Function: fake_module_check</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L16'>Function: generalimport</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L12'>Function: get_importer</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L8'>Function: get_installed_modules_names</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L42'>Function: get_spec</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L29'>Function: import_module</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L43'>Function: is_imported</a>
@@ -223,11 +223,11 @@
 
 Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 
 <sup>
-Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/master'>master</a>.
+Generated 2023-06-05 11:30 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/master'>master</a>.
 </sup>
 </details>
```

### Comparing `generalimport-0.5.0/README.md` & `generalimport-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-2([library]) --> 5([packager])
 2([library]) --> 4([vector])
-3([file]) --> 5([packager])
-0([import]) --> 3([file])
 1([tool]) --> 2([library])
-0([import]) --> 2([library])
+3([file]) --> 5([packager])
 2([library]) --> 3([file])
+0([import]) --> 2([library])
+0([import]) --> 3([file])
+2([library]) --> 5([packager])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 0 fill:#482
@@ -55,15 +55,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                          | Ver                                              | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:-----------------------------------------------------------------|:-------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.5.0](https://pypi.org/project/generalimport/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 97.0 %  |
+| [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.5.1](https://pypi.org/project/generalimport/) | 2023-06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 97.2 %  |
 </details>
 
 
 <details open>
 <summary><h2>Examples</h2></summary>
 
 
@@ -179,15 +179,15 @@
 │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L25'>Method: catch</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L49'>Method: create_module</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L52'>Method: exec_module</a>
 │  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L33'>Method: find_spec</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L8'>Class: ImportCatcher</a>
 │  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L24'>Method: handle</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L30'>Class: MissingDependencyException</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L34'>Function: MissingOptionalDependency</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L34'>Class: MissingOptionalDependency</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L63'>Function: fake_module_check</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L16'>Function: generalimport</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L12'>Function: get_importer</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L8'>Function: get_installed_modules_names</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L42'>Function: get_spec</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L29'>Function: import_module</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L43'>Function: is_imported</a>
@@ -205,11 +205,11 @@
 
 Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 
 <sup>
-Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/master'>master</a>.
+Generated 2023-06-05 11:30 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/master'>master</a>.
 </sup>
 </details>
```

### Comparing `generalimport-0.5.0/examples/1minimal_example.py` & `generalimport-0.5.1/examples/1minimal_example.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/examples/2tests_showcase.py` & `generalimport-0.5.1/examples/2tests_showcase.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/examples/4how_it_works.py` & `generalimport-0.5.1/examples/4how_it_works.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/__init__.py` & `generalimport-0.5.1/generalimport/__init__.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/dunders.py` & `generalimport-0.5.1/generalimport/dunders.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/exception.py` & `generalimport-0.5.1/generalimport/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,17 +27,21 @@
         return self.msg
 
 
 class MissingDependencyException(SkipTestException):
     pass
 
 
-def MissingOptionalDependency(*args, **kwargs):
-    warnings.warn("MissingOptionalDependency has been changed to MissingDependencyException", DeprecationWarning, stacklevel=2)
-    return MissingDependencyException(*args, **kwargs)
+class MissingOptionalDependency(SkipTestException):
+    """ MissingOptionalDependency is deprecated, use MissingDependencyException """
+    pass
+
+# def MissingOptionalDependency(*args, **kwargs):
+#     warnings.warn("MissingOptionalDependency has been changed to MissingDependencyException", DeprecationWarning, stacklevel=2)
+#     return MissingDependencyException(*args, **kwargs)
```

### Comparing `generalimport-0.5.0/generalimport/fake_module.py` & `generalimport-0.5.1/generalimport/fake_module.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/general_importer.py` & `generalimport-0.5.1/generalimport/general_importer.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/generalimport_bottom.py` & `generalimport-0.5.1/generalimport/generalimport_bottom.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/import_catcher.py` & `generalimport-0.5.1/generalimport/import_catcher.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/min.py` & `generalimport-0.5.1/generalimport/min.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_generalimport.py` & `generalimport-0.5.1/generalimport/test/test_generalimport.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_binary.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_binary.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_callable.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_callable.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_cast.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_cast.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_compare.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_compare.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_context.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_context.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_delete.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_delete.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_info.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_info.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_iterable.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_iterable.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_logic.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_logic.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_lookup.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_lookup.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_math.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_math.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_matrix.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_matrix.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_raise.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_raise.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_string.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_string.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_thread.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_thread.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/test/test_usage/test_typing.py` & `generalimport-0.5.1/generalimport/test/test_usage/test_typing.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport/top.py` & `generalimport-0.5.1/generalimport/top.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/generalimport.egg-info/PKG-INFO` & `generalimport-0.5.1/generalimport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generalimport
-Version: 0.5.0
+Version: 0.5.1
 Summary: Handle all your optional dependencies with a single call!
 Home-page: https://github.com/ManderaGeneral/generalimport
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -41,21 +41,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-2([library]) --> 5([packager])
 2([library]) --> 4([vector])
-3([file]) --> 5([packager])
-0([import]) --> 3([file])
 1([tool]) --> 2([library])
-0([import]) --> 2([library])
+3([file]) --> 5([packager])
 2([library]) --> 3([file])
+0([import]) --> 2([library])
+0([import]) --> 3([file])
+2([library]) --> 5([packager])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 0 fill:#482
@@ -73,15 +73,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                          | Ver                                              | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:-----------------------------------------------------------------|:-------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.5.0](https://pypi.org/project/generalimport/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 97.0 %  |
+| [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.5.1](https://pypi.org/project/generalimport/) | 2023-06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 97.2 %  |
 </details>
 
 
 <details open>
 <summary><h2>Examples</h2></summary>
 
 
@@ -197,15 +197,15 @@
 │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L25'>Method: catch</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L49'>Method: create_module</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L52'>Method: exec_module</a>
 │  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L33'>Method: find_spec</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L8'>Class: ImportCatcher</a>
 │  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L24'>Method: handle</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L30'>Class: MissingDependencyException</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L34'>Function: MissingOptionalDependency</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L34'>Class: MissingOptionalDependency</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L63'>Function: fake_module_check</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L16'>Function: generalimport</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L12'>Function: get_importer</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L8'>Function: get_installed_modules_names</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L42'>Function: get_spec</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L29'>Function: import_module</a>
 ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L43'>Function: is_imported</a>
@@ -223,11 +223,11 @@
 
 Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 
 <sup>
-Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/master'>master</a>.
+Generated 2023-06-05 11:30 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/master'>master</a>.
 </sup>
 </details>
```

### Comparing `generalimport-0.5.0/generalimport.egg-info/SOURCES.txt` & `generalimport-0.5.1/generalimport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generalimport-0.5.0/setup.py` & `generalimport-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 except FileNotFoundError:
     long_description = 'Readme missing'
 
 setup(
     name="generalimport",
     author='Rickard "Mandera" Abraham',
     author_email="rickard.abraham@gmail.com",
-    version="0.5.0",
+    version="0.5.1",
     description="Handle all your optional dependencies with a single call!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/ManderaGeneral/generalimport",
     license="mit",
     packages=find_namespace_packages(exclude=("build*", "dist*")),
```

