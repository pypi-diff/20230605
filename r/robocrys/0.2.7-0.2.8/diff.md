# Comparing `tmp/robocrys-0.2.7.tar.gz` & `tmp/robocrys-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocrys-0.2.7.tar", last modified: Thu Jul  1 18:20:33 2021, max compression
+gzip compressed data, was "robocrys-0.2.8.tar", last modified: Mon Jun  5 14:21:18 2023, max compression
```

## Comparing `robocrys-0.2.7.tar` & `robocrys-0.2.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 18:20:33.792998 robocrys-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)     3461 2021-07-01 18:15:33.000000 robocrys-0.2.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2021-07-01 18:15:33.000000 robocrys-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8289 2021-07-01 18:20:33.792998 robocrys-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5979 2021-07-01 18:15:33.000000 robocrys-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 18:20:33.784998 robocrys-0.2.7/robocrys/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5167 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7475 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 18:20:33.792998 robocrys-0.2.7/robocrys/condense/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24425 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/component.py
--rw-r--r--   0 runner    (1001) docker     (121)    13315 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/condenser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4508 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (121)   565274 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/formula_db.json.gz
--rw-r--r--   0 runner    (1001) docker     (121)    10620 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/mineral.py
--rw-r--r--   0 runner    (1001) docker     (121)   155577 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/mineral_db.json.gz
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/molecule.py
--rw-r--r--   0 runner    (1001) docker     (121)  3041331 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/molecule_db.json.gz
--rw-r--r--   0 runner    (1001) docker     (121)    33621 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/site.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 18:20:33.792998 robocrys-0.2.7/robocrys/condense/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11349 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/tests/test_component.py
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/tests/test_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3387 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/tests/test_mineral.py
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/tests/test_molecule.py
--rw-r--r--   0 runner    (1001) docker     (121)    10981 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/tests/test_site.py
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/condense/tests/test_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 18:20:33.792998 robocrys-0.2.7/robocrys/describe/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/describe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13794 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/describe/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)    30337 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/describe/describer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 18:20:33.792998 robocrys-0.2.7/robocrys/describe/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/describe/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5858 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/describe/tests/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/describe/tests/test_description.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 18:20:33.792998 robocrys-0.2.7/robocrys/featurize/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/featurize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10108 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/featurize/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5798 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/featurize/featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 18:20:33.792998 robocrys-0.2.7/robocrys/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/tests/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     8519 2021-07-01 18:15:33.000000 robocrys-0.2.7/robocrys/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 18:20:33.784998 robocrys-0.2.7/robocrys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8289 2021-07-01 18:20:33.000000 robocrys-0.2.7/robocrys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2021-07-01 18:20:33.000000 robocrys-0.2.7/robocrys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-01 18:20:33.000000 robocrys-0.2.7/robocrys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-07-01 18:20:33.000000 robocrys-0.2.7/robocrys.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-07-01 18:20:33.000000 robocrys-0.2.7/robocrys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-01 18:20:33.000000 robocrys-0.2.7/robocrys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-01 18:20:33.792998 robocrys-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2021-07-01 18:15:33.000000 robocrys-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.693198 robocrys-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-05 14:16:31.000000 robocrys-0.2.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-05 14:16:31.000000 robocrys-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-05 14:21:18.693198 robocrys-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-05 14:16:31.000000 robocrys-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.677197 robocrys-0.2.8/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.685198 robocrys-0.2.8/robocrys/condense/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24397 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/condenser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)   565274 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/formula_db.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/mineral.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155577 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/mineral_db.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)  3041331 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/molecule_db.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    33461 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.689198 robocrys-0.2.8/robocrys/condense/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_mineral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.689198 robocrys-0.2.8/robocrys/describe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/describer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.689198 robocrys-0.2.8/robocrys/describe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/tests/test_description.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.689198 robocrys-0.2.8/robocrys/featurize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/featurize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/featurize/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/featurize/featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.693198 robocrys-0.2.8/robocrys/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/tests/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.681198 robocrys-0.2.8/robocrys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:21:18.693198 robocrys-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-05 14:16:31.000000 robocrys-0.2.8/setup.py
```

### Comparing `robocrys-0.2.7/CONTRIBUTING.rst` & `robocrys-0.2.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.7/LICENSE` & `robocrys-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.7/README.md` & `robocrys-0.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <p align="center">
   <img alt="robocrystallographer logo" src="https://raw.githubusercontent.com/hackingmaterials/robocrystallographer/master/docs/src/_static/logo-01.png" height="200px">
 </p>
 
 <p align="center">
   <a href="https://pypi.org/project/robocrys/"><img alt="PyPI version" src="https://img.shields.io/pypi/v/robocrys.svg?colorB=blue"> </a>
-  <a href="https://www.codacy.com/app/utf/robocrystallographer"><img alt="Codacy Grade" src="https://img.shields.io/codacy/grade/47f851408d364efa9a8cdf0ed844cd8b.svg"> </a>
-  <a href="https://www.codacy.com/app/utf/robocrystallographer"><img alt="Codacy Coverage" src="https://img.shields.io/codacy/coverage/47f851408d364efa9a8cdf0ed844cd8b.svg?colorB=brightgreen"> </a>
-  <a href="https://github.com/hackingmaterials/robocrystallographer/actions?query=workflow%3A%22Run+tests%22"><img alt="CircleCI" src="https://img.shields.io/github/workflow/status/hackingmaterials/robocrystallographer/Run%20tests"> </a>
+  <a href="https://github.com/hackingmaterials/robocrystallographer/actions?query=workflow%3A%22Run+tests%22"><img alt="CircleCI" src="https://img.shields.io/github/actions/workflow/status/hackingmaterials/robocrystallographer/tests.yml?branch=main"> </a>
 </p>
 
 
+
+
 Robocrystallographer is a tool to generate text descriptions of crystal
 structures. Similar to how a real-life crystallographer would analyse a
 structure, robocrystallographer looks at the symmetry, local environment, and
 extended connectivity when generating a description. The package includes
 utilities for identifying molecule names, component orientations,
 heterostructure information, and more...
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                           [robocrystallographer logo]
-          [PyPI_version] [Codacy_Grade] [Codacy_Coverage] [CircleCI]
+                           [PyPI_version] [CircleCI]
 Robocrystallographer is a tool to generate text descriptions of crystal
 structures. Similar to how a real-life crystallographer would analyse a
 structure, robocrystallographer looks at the symmetry, local environment, and
 extended connectivity when generating a description. The package includes
 utilities for identifying molecule names, component orientations,
 heterostructure information, and more... ## Usage Robocrystallographer can be
 used from the command-line or from a python API. The package integrates with
```

### Comparing `robocrys-0.2.7/robocrys/adapter.py` & `robocrys-0.2.8/robocrys/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""
-This module implements a class to resolve the symbolic references in condensed
+"""This module implements a class to resolve the symbolic references in condensed
 structure data.
 """
+from __future__ import annotations
 
-from typing import Any, Dict, List, Union
+from typing import Any
 
 
 class BaseAdapter:
     """Base adapter class for facilitating access to condensed structure data.
 
     Attributes:
         elements: The site elements.
 
     Args:
         condensed_structure: The condensed structure data, formatted as produced
             by :meth:`robocrys.condense.StructureCondenser.condense_structure`.
     """
 
-    def __init__(self, condensed_structure: Dict[str, Any]):
+    def __init__(self, condensed_structure: dict[str, Any]):
         self._condensed_structure = condensed_structure
         self.elements = {
             site_index: site_data["element"]
             for site_index, site_data in self.sites.items()
         }
 
     def get_distance_details(
-        self, from_site: int, to_sites: Union[int, List[int]]
-    ) -> List[float]:
+        self, from_site: int, to_sites: int | list[int]
+    ) -> list[float]:
         """Gets the bond lengths between two sets of sites.
 
         Args:
             from_site: An inequivalent site index.
-            to_sites: One ore more inequivalent site indices.
+            to_sites: One or more inequivalent site indices.
 
         Returns:
             The distances between the sites.
         """
         if isinstance(to_sites, int):
             # If only one to_site is provided turn it into a list
             to_sites = [to_sites]
@@ -43,21 +43,21 @@
         return [
             distance
             for to_site in to_sites
             for distance in self.distances[from_site][to_site]
         ]
 
     def get_angle_details(
-        self, from_site: int, to_sites: Union[int, List[int]], connectivity: str
-    ) -> List[float]:
+        self, from_site: int, to_sites: int | list[int], connectivity: str
+    ) -> list[float]:
         """Gets the connectivity angles between two sets of sites.
 
         Args:
             from_site: An inequivalent site index.
-            to_sites: One ore more inequivalent site indices.
+            to_sites: One or more inequivalent site indices.
             connectivity: The site connectivity type. I.e. "corner", "edge", or
                 "face".
 
         Returns:
             The distances between the sites.
         """
         if isinstance(to_sites, int):
@@ -67,15 +67,15 @@
         return [
             angle
             for to_site in to_sites
             for angle in self.angles[from_site][to_site][connectivity]
         ]
 
     @property
-    def mineral(self) -> Dict[str, Union[str, int, bool]]:
+    def mineral(self) -> dict[str, str | int | bool]:
         """The mineral data.
 
         See :meth:`robocrys.condense.StructureCondenser.condense_structure` for
         more details.
         """
         return self._condensed_structure["mineral"]
 
@@ -112,51 +112,51 @@
 
         See :meth:`robocrys.condense.StructureCondenser.condense_structure` for
         more details.
         """
         return self._condensed_structure["dimensionality"]
 
     @property
-    def sites(self) -> Dict[int, Dict[str, Any]]:
+    def sites(self) -> dict[int, dict[str, Any]]:
         """The site data.
 
         See :meth:`robocrys.condense.StructureCondenser.condense_structure` for
         more details.
         """
         return self._condensed_structure["sites"]
 
     @property
-    def distances(self) -> Dict[int, Dict[int, List[float]]]:
+    def distances(self) -> dict[int, dict[int, list[float]]]:
         """The distance data.
 
         See :meth:`robocrys.condense.StructureCondenser.condense_structure` for
         more details.
         """
         return self._condensed_structure["distances"]
 
     @property
-    def angles(self) -> Dict[int, Dict[int, Dict[str, List[float]]]]:
+    def angles(self) -> dict[int, dict[int, dict[str, list[float]]]]:
         """The angle data.
 
         See :meth:`robocrys.condense.StructureCondenser.condense_structure` for
         more details.
         """
         return self._condensed_structure["angles"]
 
     @property
-    def components(self) -> Dict[int, Dict[str, Any]]:
+    def components(self) -> dict[int, dict[str, Any]]:
         """The component data.
 
         See :meth:`robocrys.condense.StructureCondenser.condense_structure` for
         more details.
         """
         return self._condensed_structure["components"]
 
     @property
-    def component_makeup(self) -> List[int]:
+    def component_makeup(self) -> list[int]:
         """The component makeup of the structure.
 
         See :meth:`robocrys.condense.StructureCondenser.condense_structure` for
         more details.
         """
         return self._condensed_structure["component_makeup"]
```

### Comparing `robocrys-0.2.7/robocrys/cli.py` & `robocrys-0.2.8/robocrys/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-"""
-This module contains a script for using robocrys from the command line.
-"""
+"""This module contains a script for using robocrys from the command line."""
+from __future__ import annotations
 
 import argparse
 import sys
 import warnings
-from typing import Optional
 
 from pymatgen.core.structure import Structure
 from pymatgen.ext.matproj import MPRestError
 
 from robocrys import StructureCondenser, StructureDescriber, __version__
 
 __author__ = "Alex Ganose"
 __maintainer__ = "Alex Ganose"
 __email__ = "aganose@lbl.gov"
 __date__ = "December 17, 2018"
 
 
 def robocrystallographer(
     structure: Structure,
-    condenser_kwargs: Optional[dict] = None,
-    describer_kwargs: Optional[dict] = None,
+    condenser_kwargs: dict | None = None,
+    describer_kwargs: dict | None = None,
 ) -> str:
     """Gets the robocrystallographer description of a structure.
 
     Args:
         structure: A structure.
         condenser_kwargs: Keyword arguments that will be passed to
             :obj:`robocrys.condense.StructureCondenser`.
@@ -37,15 +35,15 @@
     """
     condenser_kwargs = condenser_kwargs if condenser_kwargs else {}
     describer_kwargs = describer_kwargs if describer_kwargs else {}
 
     sc = StructureCondenser(**condenser_kwargs)
     describer = StructureDescriber(**describer_kwargs)
 
-    if not any([hasattr(s, "oxi_state") for s in structure.composition.elements]):
+    if not any(hasattr(s, "oxi_state") for s in structure.composition.elements):
         try:
             structure.add_oxidation_state_by_guess(max_sites=-80)
         except ValueError:
             warnings.warn("Could not add oxidation states!")
 
     condensed_structure = sc.condense_structure(structure)
     description = describer.describe(condensed_structure)
@@ -162,15 +160,15 @@
         action="store_false",
         help="describe bond lengths for each site",
     )
     parser.add_argument(
         "--format",
         dest="fmt",
         default="unicode",
-        help="how to format the description (unicode [default]," " html, latex, raw)",
+        help="how to format the description (unicode [default], html, latex, raw)",
     )
     parser.add_argument(
         "--api-key",
         help="set the materials project API key. See: "
         "https://materialsproject.org/docs/api",
     )
     return parser
```

### Comparing `robocrys-0.2.7/robocrys/condense/component.py` & `robocrys-0.2.8/robocrys/condense/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-"""
-This module implements functions for handling structure components.
-"""
+"""This module implements functions for handling structure components."""
+from __future__ import annotations
+
 from copy import deepcopy
-from typing import Any, Dict, List, Tuple
+from typing import TYPE_CHECKING, Any
 
 import networkx as nx
 import numpy as np
 from monty.fractions import gcd
 from pymatgen.analysis.structure_matcher import StructureMatcher
 from pymatgen.core.composition import Composition
 from pymatgen.core.periodic_table import get_el_sp
 from pymatgen.core.structure import PeriodicSite, Structure
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.util.string import formula_double_format
 
-from robocrys import common_formulas
 from robocrys.condense.fingerprint import get_structure_fingerprint
+from robocrys.util import common_formulas
 
-Component = Dict[str, Any]
+if TYPE_CHECKING:
+    Component = dict[str, Any]
 
 
 def get_structure_inequiv_components(
-    components: List[Component],
+    components: list[Component],
     use_structure_graph: bool = False,
-    fingerprint_tol: int = 0.01,
-) -> List[Component]:
+    fingerprint_tol: float = 0.01,
+) -> list[Component]:
     """Gets and counts the structurally inequivalent components.
 
     Supports matching through StructureMatcher or by a combined structure graph/
     site fingerprint approach. For the latter method, the component data has to
     have been generated with ``inc_graph=True``.
 
     Args:
@@ -129,16 +130,15 @@
 
     def node_match(n1, n2):
         return n1["specie"] == n2["specie"]
 
     def edge_match(e1, e2):
         if use_weights:
             return e1["weight"] == e2["weight"]
-        else:
-            return True
+        return True
 
     graph_a = component_a["structure_graph"].graph
     graph_b = component_b["structure_graph"].graph
 
     species_a = {
         n: {"specie": str(component_a["structure_graph"].structure[n].specie)}
         for n in graph_a
@@ -153,16 +153,16 @@
 
     return nx.is_isomorphic(
         graph_a, graph_b, node_match=node_match, edge_match=edge_match
     )
 
 
 def get_sym_inequiv_components(
-    components: List[Component], spg_analyzer: SpacegroupAnalyzer
-) -> List[Component]:
+    components: list[Component], spg_analyzer: SpacegroupAnalyzer
+) -> list[Component]:
     """Gets and counts the symmetrically inequivalent components.
 
     Component data has to have been generated with ``inc_site_ids=True``.
 
     Args:
         components: A list of structure components, generated using
             :obj:`pymatgen.analysis.dimensionality.get_structure_components`,
@@ -197,18 +197,18 @@
         component["count"] = 1
         sym_inequiv_components[sym_indices] = component
 
     return list(sym_inequiv_components.values())
 
 
 def get_formula_inequiv_components(
-    components: List[Component],
+    components: list[Component],
     use_iupac_formula: bool = True,
     use_common_formulas: bool = True,
-) -> List[Component]:
+) -> list[Component]:
     """Gets and counts the inequivalent components based on their formuula.
 
     Note that the counting of compounds is different to in
     ``get_sym_inequiv_equivalent``. I.e. the count is not the number of
     components with the same formula. For example, the count of the formula
     "GaAs" in a system with two Ga2As2 components would be 4.
 
@@ -260,16 +260,16 @@
 
         inequiv_components[formula] = component
 
     return list(inequiv_components.values())
 
 
 def filter_molecular_components(
-    components: List[Component],
-) -> Tuple[List[Component], List[Component]]:
+    components: list[Component],
+) -> tuple[list[Component], list[Component]]:
     """Separate list of components into molecular and non-molecular components.
 
     Args:
         components: A list of structure components, generated using
             :obj:`pymatgen.analysis.dimensionality.get_structure_components`.
 
     Returns:
@@ -279,15 +279,15 @@
     molecular_components = [c for c in components if c["dimensionality"] == 0]
     other_components = [c for c in components if c["dimensionality"] != 0]
 
     return molecular_components, other_components
 
 
 def get_reconstructed_structure(
-    components: List[Component], simplify_molecules: bool = True
+    components: list[Component], simplify_molecules: bool = True
 ) -> Structure:
     """Reconstructs a structure from a list of components.
 
     Has the option to simplify molecular components into a single site
     positioned at the centre of mass of the molecular. If using this option,
     the components must have been generated with ``inc_molecule_graph=True``.
 
@@ -328,15 +328,15 @@
     return Structure.from_sites(other_sites + mol_sites)
 
 
 def get_component_formula_and_factor(
     component: Component,
     use_iupac_formula: bool = True,
     use_common_formulas: bool = True,
-) -> Tuple[str, int]:
+) -> tuple[str, int]:
     """Gets the reduced formula and factor of a single component.
 
     Args:
         component: A structure component, generated using
             :obj:`pymatgen.analysis.dimensionality.get_structure_components`.
         use_iupac_formula (bool, optional): Whether to order formulas by the
             iupac "electronegativity" series, defined in Table VI of
@@ -392,15 +392,15 @@
         component,
         use_iupac_formula=use_iupac_formula,
         use_common_formulas=use_common_formulas,
     )[0]
 
 
 def get_formula_from_components(
-    components: List[Component],
+    components: list[Component],
     molecules_first: bool = False,
     use_iupac_formula: bool = True,
     use_common_formulas: bool = True,
 ) -> str:
     """Reconstructs a chemical formula from structure components.
 
     The chemical formulas for the individual components will be grouped
@@ -429,16 +429,15 @@
 
     def order(comp_formula):
         composition = Composition(comp_formula)
         if use_iupac_formula:
             return sum(
                 [get_el_sp(s).iupac_ordering for s in composition.elements]
             ) / len(composition.elements)
-        else:
-            return composition.average_electroneg
+        return composition.average_electroneg
 
     components = get_formula_inequiv_components(
         components,
         use_iupac_formula=use_iupac_formula,
         use_common_formulas=use_common_formulas,
     )
 
@@ -461,51 +460,48 @@
     # the following is based on ``pymatgen.core.composition.reduce_formula``
     num_comps = len(formulas)
     factor = abs(gcd(*(form_count_dict.values())))
 
     reduced_form = []
     for i in range(0, num_comps):
         formula = formulas[i]
-        normamt = form_count_dict[formula] * 1.0 / factor
-        formatted_formula = formula if normamt == 1 else f"({formula})"
+        norm_amt = form_count_dict[formula] * 1.0 / factor
+        formatted_formula = formula if norm_amt == 1 else f"({formula})"
         reduced_form.append(formatted_formula)
-        reduced_form.append(formula_double_format(normamt))
+        reduced_form.append(str(formula_double_format(norm_amt)))
 
     reduced_form = "".join(reduced_form)
     return reduced_form
 
 
-def components_are_vdw_heterostructure(components: List[Component]) -> bool:
+def components_are_vdw_heterostructure(components: list[Component]) -> bool:
     """Whether a list of components form a van der Waals heterostructure.
 
     A heterostructure is defined here as a structure with more than one
     formula inequivalent 2D component.
 
     Args:
         components: A list of structure components, generated using
             :obj:`pymatgen.analysis.dimensionality.get_structure_components`.
 
     Returns:
         Whether the list of components from a heterostructure.
     """
     components = get_formula_inequiv_components(components)
 
-    if len([c for c in components if c["dimensionality"] == 2]):
-        return True
-    else:
-        return False
+    return bool(len([c for c in components if c["dimensionality"] == 2]))
 
 
 def get_vdw_heterostructure_information(
-    components: List[Component],
+    components: list[Component],
     use_iupac_formula: bool = True,
     use_common_formulas: bool = True,
     inc_ordered_components: bool = False,
     inc_intercalants: bool = False,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """Gets information about ordering of components in a vdw heterostructure.
 
     Args:
         components: A list of structure components, generated using
             :obj:`pymatgen.analysis.dimensionality.get_structure_components`
             with ``inc_orientation=True``.
         use_iupac_formula (bool, optional): Whether to order formulas by the
@@ -543,19 +539,20 @@
           :obj:`List` of intercalated components.
     """
     if not components_are_vdw_heterostructure(components):
         raise ValueError("Components do not form a heterostructure.")
 
     try:
         millers = {c["orientation"] for c in components if c["dimensionality"] == 2}
-    except KeyError as e:
-        if "orientation" in str(e):
-            raise KeyError("Components not generated with inc_orientation=True")
-        else:
-            raise e
+    except KeyError as exc:
+        if "orientation" in str(exc):
+            raise KeyError(
+                "Components not generated with inc_orientation=True"
+            ) from exc
+        raise exc
 
     if len(millers) != 1:
         raise ValueError("2D components don't all have the same orientation.")
 
     cart_miller = (
         components[0]["structure_graph"]
         .structure.lattice.get_cartesian_coords(millers.pop())
@@ -596,18 +593,16 @@
     # number of repetitions that can occur. To avoid unnecessary work we start
     # from this number of repetitions and move to 1 repetition (e.g. no
     # repetition)
     max_repetitions = int(np.floor(len(ordered_layers) / num_layer_formulas))
     for n in range(max_repetitions, 0, -1):
         if (
             all(
-                [
-                    len(set(ordered_layers_formula[i::num_layer_formulas])) == 1
-                    for i in range(n)
-                ]
+                len(set(ordered_layers_formula[i::num_layer_formulas])) == 1
+                for i in range(n)
             )
             and len(ordered_layers) % n == 0
         ):
             repeating_formula = ordered_layers_formula[: int(len(ordered_layers) / n)]
             num_repetitions = n
             break
```

### Comparing `robocrys-0.2.7/robocrys/condense/condenser.py` & `robocrys-0.2.8/robocrys/condense/condenser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-"""
-This module defines a class for condensing structures into dict representations.
-"""
+"""This module defines a class for condensing structures into dict representations."""
+from __future__ import annotations
 
-from typing import Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any
 
 from pymatgen.analysis.dimensionality import get_structure_components
 from pymatgen.analysis.local_env import CrystalNN, NearNeighbors
 from pymatgen.core.structure import Structure
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
-from robocrys import common_formulas
 from robocrys.condense.component import (
-    Component,
     components_are_vdw_heterostructure,
     get_component_formula,
     get_formula_from_components,
     get_reconstructed_structure,
     get_structure_inequiv_components,
     get_sym_inequiv_components,
     get_vdw_heterostructure_information,
 )
 from robocrys.condense.mineral import MineralMatcher
 from robocrys.condense.molecule import MoleculeNamer
 from robocrys.condense.site import SiteAnalyzer
+from robocrys.util import common_formulas
+
+if TYPE_CHECKING:
+    from robocrys.condense.component import Component
 
 
 class StructureCondenser:
     """Class to transform a structure into an intermediate dict representation.
 
     Args:
         use_conventional_cell: Whether to always use the convention cell
@@ -58,16 +59,16 @@
             The common formula will be used preferentially to the iupac or
             reduced formula.
     """
 
     def __init__(
         self,
         use_conventional_cell: bool = True,
-        near_neighbors: Optional[NearNeighbors] = None,
-        mineral_matcher: Optional[MineralMatcher] = None,
+        near_neighbors: NearNeighbors | None = None,
+        mineral_matcher: MineralMatcher | None = None,
         use_symmetry_equivalent_sites: bool = False,
         symprec: float = 0.01,
         simplify_molecules: bool = True,
         use_iupac_formula: bool = True,
         use_common_formulas: bool = True,
     ):
         if not near_neighbors:
@@ -81,15 +82,15 @@
         self.mineral_matcher = mineral_matcher
         self.use_symmetry_equivalent_sites = use_symmetry_equivalent_sites
         self.symprec = symprec
         self.simplify_molecules = simplify_molecules
         self.use_common_formulas = use_common_formulas
         self.use_iupac_formula = use_iupac_formula
 
-    def condense_structure(self, structure: Structure) -> Dict[str, Any]:
+    def condense_structure(self, structure: Structure) -> dict[str, Any]:
         """Condenses the structure into an intermediate dict representation.
 
         Args:
             structure: A pymatgen structure object.
 
         Returns:
             The condensed structure information. The data is formatted as a
@@ -157,16 +158,16 @@
             hs_info = None
 
         structure_data["vdw_heterostructure_info"] = hs_info
 
         return structure_data
 
     def _condense_mineral(
-        self, structure: Structure, components: List[Component]
-    ) -> Dict[str, Any]:
+        self, structure: Structure, components: list[Component]
+    ) -> dict[str, Any]:
         """Condenses the mineral data.
 
         Initially the original structure will be matched against a library
         of known minerals. If no match is found, the structure will be
         reconstructed, with all zero-dimensional components replaced by single
         atoms at their centre of mass, and the matching performed again.
         This allows for matching of systems with molecular substituents in
@@ -192,15 +193,14 @@
             correspond to the mineral name (e.g. Perovskite), the fingerprint
             distance between the prototype and known mineral, and whether the
             number of species types in the structure matches the number in the
             known prototype. If no mineral match is determined, the mineral type
             will be ``None``. If an exact mineral match is found the distance
             will be set to ``-1``.
         """
-
         if not self.mineral_matcher:
             return {
                 "type": None,
                 "distance": -1,
                 "n_species_type_match": True,
                 "simplified": False,
             }
@@ -215,15 +215,15 @@
             mineral["simplified"] = True
         else:
             mineral["simplified"] = False
 
         return mineral
 
     def _condense_formula(
-        self, structure: Structure, components: List[Component]
+        self, structure: Structure, components: list[Component]
     ) -> str:
         """Condenses the structure formula.
 
         If :attr:`StructureCondenser.use_common_formulas` is ``True`` and the
         formula is found in a database of 100,000 known formulas we
         preferentially use the known formula, otherwise we reconstruct the
         formula from the structure components.
@@ -244,18 +244,18 @@
             formula = get_formula_from_components(
                 components, use_common_formulas=self.use_common_formulas
             )
         return formula
 
     def _condense_components(
         self,
-        components: List[Component],
+        components: list[Component],
         spacegroup_analyzer: SpacegroupAnalyzer,
         site_analyzer: SiteAnalyzer,
-    ) -> Tuple[Dict[int, Any], List[int]]:
+    ) -> tuple[dict[int, Any], list[int]]:
         """Condenses the component data.
 
         Args:
             components: A list of structure components, generated using
                 :obj:`pymatgen.analysis.dimensionality.get_structure_components`
             site_analyzer: A site analyzer object for the structure containing
                 the components.
```

### Comparing `robocrys-0.2.7/robocrys/condense/fingerprint.py` & `robocrys-0.2.8/robocrys/condense/fingerprint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Dict, Iterable, List, Optional, Tuple, Union
+from __future__ import annotations
+
+from collections.abc import Iterable
 
 import numpy as np
 from matminer.featurizers.site import CrystalNNFingerprint
 from matminer.featurizers.structure import SiteStatsFingerprint
 from pymatgen.core.structure import IStructure
 
 
 def get_site_fingerprints(
     structure: IStructure,
     as_dict: bool = True,
     preset: str = "CrystalNNFingerprint_ops",
-) -> Union[List[Dict[str, int]], np.ndarray]:
+) -> list[dict[str, int]] | np.ndarray:
     """Gets the fingerprint for all sites in a structure.
 
     Args:
         structure: A structure.
         as_dict: Whether to return the fingerprints as a dictionary of
             ``{'op': val}``. Defaults to ``True``.
         preset: The preset to use when calculating the fingerprint. See
@@ -44,15 +46,15 @@
 
     return site_fingerprints
 
 
 def get_structure_fingerprint(
     structure: IStructure,
     preset: str = "CrystalNNFingerprint_ops",
-    stats: Optional[Tuple[str]] = ("mean", "std_dev"),
+    stats: tuple[str] | None = ("mean", "std_dev"),
     prototype_match: bool = False,
 ) -> np.ndarray:
     """Gets the fingerprint for a structure.
 
     Args:
         structure: A structure.
         preset: The preset to use when calculating the fingerprint. See
@@ -81,15 +83,15 @@
         ssf = SiteStatsFingerprint(
             CrystalNNFingerprint.from_preset("ops", cation_anion=False), stats=stats
         )
     return np.array(ssf.featurize(structure))
 
 
 def get_fingerprint_distance(
-    structure_a: Union[IStructure, Iterable], structure_b: Union[IStructure, Iterable]
+    structure_a: IStructure | Iterable, structure_b: IStructure | Iterable
 ) -> float:
     """Gets the euclidean distance between the fingerprints of two structures.
 
     Args:
         structure_a: The first structure or fingerprint. Can be provided as a
             structure or a fingerprint. If provided as a structure, the
             fingerprint will be calculated first, so generally it is quicker
@@ -110,9 +112,8 @@
         fingerprint_a = np.array(structure_a)
 
     if issubclass(type(structure_b), IStructure):
         fingerprint_b = get_structure_fingerprint(structure_b)
     else:
         fingerprint_b = np.array(structure_b)
 
-    dist = np.linalg.norm(fingerprint_a - fingerprint_b)
-    return dist
+    return np.linalg.norm(fingerprint_a - fingerprint_b)
```

### Comparing `robocrys-0.2.7/robocrys/condense/formula_db.json.gz` & `robocrys-0.2.8/robocrys/condense/formula_db.json.gz`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.7/robocrys/condense/mineral.py` & `robocrys-0.2.8/robocrys/condense/mineral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""
-This module provides tools for matching structures to known mineral class.
-"""
+"""This module provides tools for matching structures to known mineral class."""
+from __future__ import annotations
 
 from itertools import islice
-from typing import Any, Dict, List, Optional
+from typing import Any
 
 import numpy as np
 from matminer.utils.io import load_dataframe_from_json
 from pkg_resources import resource_filename
 from pymatgen.analysis.prototypes import AflowPrototypeMatcher
 from pymatgen.core.structure import IStructure
 
@@ -57,15 +56,15 @@
         self.initial_stol = initial_stol
         self.initial_angle_tol = initial_angle_tol
         self.fingerprint_distance_cutoff = fingerprint_distance_cutoff
         self.use_fingerprint_matching = use_fingerprint_matching
         self._structure = None
         self._mineral_db = None
 
-    def get_best_mineral_name(self, structure: IStructure) -> Dict[str, Any]:
+    def get_best_mineral_name(self, structure: IStructure) -> dict[str, Any]:
         """Gets the "best" mineral name for a structure.
 
         Uses a combination of AFLOW prototype matching and fingerprinting to
         get the best mineral name.
 
         The AFLOW structure prototypes are detailed in reference [aflow]_.
 
@@ -124,15 +123,15 @@
             "distance": distance,
             "n_species_type_match": n_species_types_match,
         }
 
     def get_aflow_matches(
         self,
         structure: IStructure,
-    ) -> Optional[List[Dict[str, Any]]]:
+    ) -> list[dict[str, Any]] | None:
         """Gets minerals for a structure by matching to AFLOW prototypes.
 
         Overrides
         :class:`pymatgen.analysis.aflow_prototypes.AflowPrototypeMatcher` to
         only return matches to prototypes with known mineral names.
 
         The AFLOW tolerance parameters (defined in the init method) are passed
@@ -176,18 +175,18 @@
         matcher._match_prototype = _match_prototype
 
         return matcher.get_prototypes(structure)
 
     def get_fingerprint_matches(
         self,
         structure: IStructure,
-        max_n_matches: Optional[int] = None,
+        max_n_matches: int | None = None,
         match_n_sp: bool = True,
-        mineral_name_constraint: Optional[str] = None,
-    ) -> Optional[List[Dict[str, Any]]]:
+        mineral_name_constraint: str | None = None,
+    ) -> list[dict[str, Any]] | None:
         """Gets minerals for a structure by matching to AFLOW fingerprints.
 
         Only AFLOW prototypes with mineral names are considered. The AFLOW
         structure prototypes are detailed in reference [aflow]_.
 
         Args:
             structure: A structure to match.
@@ -255,14 +254,14 @@
             lambda x: get_fingerprint_distance(x, fingerprint)
         )
 
         self._mineral_db = data.sort_values(by="distance")
         self._structure = structure
 
 
-def _get_row_data(row: Dict) -> Dict[str, Any]:
+def _get_row_data(row: dict) -> dict[str, Any]:
     """Utility function to extract mineral data from pandas `DataFrame` row."""
     return {
         "type": row["mineral"],
         "distance": row["distance"],
         "structure": row["structure"],
     }
```

### Comparing `robocrys-0.2.7/robocrys/condense/mineral_db.json.gz` & `robocrys-0.2.8/robocrys/condense/mineral_db.json.gz`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.7/robocrys/condense/molecule.py` & `robocrys-0.2.8/robocrys/condense/molecule.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,56 @@
-"""
-This module implements a class to match molecule graphs to molecule names.
+"""This module implements a class to match molecule graphs to molecule names.
 
 Some functionality relies on having a working internet connection.
 """
+from __future__ import annotations
 
 import warnings
-from typing import Optional, Tuple
 
 from monty.serialization import loadfn
 from pkg_resources import resource_filename
 from pubchempy import BadRequestError, get_compounds
 from pymatgen.analysis.graphs import MoleculeGraph
 from pymatgen.io.babel import BabelMolAdaptor
 
 
 class MoleculeNamer:
     name_sources = ("traditional", "iupac")
 
     def __init__(
         self,
         use_online_pubchem: bool = True,
-        name_preference: Tuple[str] = name_sources,
+        name_preference: tuple[str] = name_sources,
     ):
         """Class to match molecule graphs to known molecule names.
 
         Args:
             use_online_pubchem: Whether to try using the Pubchem website for
                 matching molecules if a match is not found in the offline
                 database. Defaults to ``True``. Requires a working internet
                 connection and for the ``pubchempy`` package to be installed.
             name_preference: The order of preference for determining compound
                 names. Options are "traditional", and "iupac". If the
                 first option is not available, the subsequent options will be
                 used. Should be provided as a tuple of options, from 1st choice
                 to last.
         """
-
         db_file = resource_filename("robocrys.condense", "molecule_db.json.gz")
         self.molecule_db = loadfn(db_file)
         self.matched_molecules = {}
         self.use_online_pubchem = use_online_pubchem
 
         # append the sources list to the end in case the user only supplies
         # a single preference
         self.name_preference = tuple(list(name_preference) + list(self.name_sources))
 
     def get_name_from_molecule_graph(
         self,
         molecule_graph: MoleculeGraph,
-    ) -> Optional[str]:
+    ) -> str | None:
         """Gets the name of a molecule from a molecule graph object.
 
         Args:
             molecule_graph: A molecule graph.
 
         Returns:
             The molecule name if a match is found else ``None``.
@@ -63,30 +61,29 @@
             return None
 
         match = None
         if smiles in self.matched_molecules:
             match = self.matched_molecules[smiles]
 
         elif smiles in self.molecule_db:
-
             # we should use the first preference for which there is a match
             for source in self.name_preference:
                 if (
                     source in self.molecule_db[smiles]
                     and self.molecule_db[source][smiles]
                 ):
                     match = self.molecule_db[smiles][source]
                     break
 
         if not match and self.use_online_pubchem:
             match = self.get_name_from_pubchem(smiles)
 
         return self._process_match(smiles, match)
 
-    def get_name_from_pubchem(self, smiles: str) -> Optional[str]:
+    def get_name_from_pubchem(self, smiles: str) -> str | None:
         """Tries to get the name of a molecule from the Pubchem website.
 
         Args:
             smiles: A SMILES string.
 
         Returns:
             The molecule name if a match is found else ``None``.
@@ -108,15 +105,15 @@
 
         if isinstance(match, str):
             match = match.lower()
 
         return self._process_match(smiles, match)
 
     @staticmethod
-    def molecule_graph_to_smiles(molecule_graph: MoleculeGraph) -> Optional[str]:
+    def molecule_graph_to_smiles(molecule_graph: MoleculeGraph) -> str | None:
         """Converts a molecule graph to SMILES string.
 
         Args:
             molecule_graph: A molecule graph.
 
         Returns:
             The SMILES representation of the molecule.
@@ -124,20 +121,19 @@
         try:
             bma = BabelMolAdaptor.from_molecule_graph(molecule_graph)
             pbmol = bma.pybel_mol
             return pbmol.write("smi").split()[0]
         except RuntimeError:
             warnings.warn(
                 "Molecule naming requires openbabel to be installed "
-                "with Python bindings. Please get it at "
-                "http://openbabel.org."
+                "with Python bindings. Please get it at http://openbabel.org.",
+                RuntimeWarning,
             )
             return None
 
-    def _process_match(self, smiles: str, match: Optional[str]) -> Optional[str]:
+    def _process_match(self, smiles: str, match: str | None) -> str | None:
         """Utility function to store and process match."""
         if isinstance(match, str):
             match = match.lower()
             self.matched_molecules[smiles] = match
             return self.matched_molecules[smiles]
-        else:
-            return match
+        return match
```

### Comparing `robocrys-0.2.7/robocrys/condense/molecule_db.json.gz` & `robocrys-0.2.8/robocrys/condense/molecule_db.json.gz`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.7/robocrys/condense/site.py` & `robocrys-0.2.8/robocrys/condense/site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""
-This module provides a class to extract geometry and neighbor information.
+"""This module provides a class to extract geometry and neighbor information.
 
-TODO:
+Todo:
     * distortion of geometry e.g. elongated along an axis
 """
+from __future__ import annotations
 
 from collections import defaultdict
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any
 
 import numpy as np
 from pymatgen.analysis.graphs import StructureGraph
 from pymatgen.core.composition import Composition
 from pymatgen.core.periodic_table import get_el_sp
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.util.coord import get_angle
@@ -74,15 +74,15 @@
         if use_symmetry_equivalent_sites:
             self.equivalent_sites = list(equivalent_sites)
         else:
             self.equivalent_sites = self._calculate_equivalent_sites()
 
         self.symmetry_labels = self._calculate_symmetry_labels(equivalent_sites)
 
-    def get_site_geometry(self, site_index: int) -> Dict[str, Union[str, float]]:
+    def get_site_geometry(self, site_index: int) -> dict[str, str | float]:
         """Gets the bonding geometry of a site.
 
         For example, "octahedral" or "square-planar".
 
         Args:
             site_index: The site index (zero based).
 
@@ -96,15 +96,15 @@
             :obj:`float` indicating whether how close the geometry is to the
             perfect geometry. If the largest geometrical order parameter falls
             beneath :attr:`robocrys.site.SiteAnalyzer.minimum_geometry_op`, the
             geometry type will be returned as "X-coordinate", where X is the
             coordination number.
         """
         # get fingerprint as a list of tuples, e.g. [("op name", val), ...]
-        site_fingerprint: List[Tuple[str, int]] = list(
+        site_fingerprint: list[tuple[str, int]] = list(
             self.site_fingerprints[site_index].items()
         )
 
         # get coordination number with largest weight, ignore op names with
         # just the coordination number weight (e.g. containing "wt")
         parameter = max(site_fingerprint, key=lambda x: x[1] if "wt" not in x[0] else 0)
 
@@ -126,19 +126,18 @@
             geometry = "single-bond" if geometry == "sgl_bd" else geometry
             likeness = parameter[1]
 
         return {"type": geometry, "likeness": likeness}
 
     def get_nearest_neighbors(
         self, site_index: int, inc_inequivalent_site_index: bool = True
-    ) -> List[Dict[str, Any]]:
+    ) -> list[dict[str, Any]]:
         """Gets information about the bonded nearest neighbors.
 
         Args:
-
             site_index: The site index (zero based).
             inc_inequivalent_site_index: Whether to include the inequivalent
                 site indices in the nearest neighbor information.
 
         Returns:
             For each site bonded to ``site_index``, returns a :obj:`dict`
             with the format::
@@ -147,35 +146,32 @@
 
             If ``inc_inequivalent_site_index=True``, the data will have an
             additional key ``'inequiv_index'`` corresponding to the inequivalent
             site index. E.g. if two sites are structurally/symmetrically
             equivalent (depending on the value of ``self.use_symmetry_equivalent_sites`` then
             they will have the same ``inequiv_index``.
         """
-
         nn_sites = self.bonded_structure.get_connected_sites(site_index)
 
         if inc_inequivalent_site_index:
             return [
                 {
                     "element": str(site.site.specie),
                     "inequiv_index": self.equivalent_sites[site.index],
                     "dist": site.dist,
                 }
                 for site in nn_sites
             ]
-        else:
-            return [
-                {"element": str(site.site.specie), "dist": site.dist}
-                for site in nn_sites
-            ]
+        return [
+            {"element": str(site.site.specie), "dist": site.dist} for site in nn_sites
+        ]
 
     def get_next_nearest_neighbors(
         self, site_index: int, inc_inequivalent_site_index: bool = True
-    ) -> List[Dict[str, Any]]:
+    ) -> list[dict[str, Any]]:
         """Gets information about the bonded next nearest neighbors.
 
         Args:
             site_index: The site index (zero based).
             inc_inequivalent_site_index: Whether to include the inequivalent
                 site indices.
 
@@ -279,15 +275,15 @@
             if inc_inequivalent_site_index:
                 summary["inequiv_index"] = self.equivalent_sites[nnn_site.index]
 
             next_nn_summary.append(summary)
 
         return next_nn_summary
 
-    def get_site_summary(self, site_index: int) -> Dict[str, Any]:
+    def get_site_summary(self, site_index: int) -> dict[str, Any]:
         """Gets a summary of the site information.
 
         Args:
             site_index: The site index (zero based).
 
         Returns:
             A summary of the site information, formatted as::
@@ -353,15 +349,15 @@
             "geometry": geometry,
             "nn": nn_indices,
             "nnn": nnn,
             "poly_formula": poly_formula,
             "sym_labels": sym_labels,
         }
 
-    def get_bond_distance_summary(self, site_index: int) -> Dict[int, List[float]]:
+    def get_bond_distance_summary(self, site_index: int) -> dict[int, list[float]]:
         """Gets the bond distance summary for a site.
 
         Args:
             site_index: The site index (zero based).
 
         Returns:
             The bonding data for the site, formatted as::
@@ -376,15 +372,15 @@
             to_site = nn_site["inequiv_index"]
             bonds[to_site].append(nn_site["dist"])
 
         return defaultdict_to_dict(bonds)
 
     def get_connectivity_angle_summary(
         self, site_index: int
-    ) -> Dict[int, Dict[str, List[float]]]:
+    ) -> dict[int, dict[str, list[float]]]:
         """Gets the connectivity angle summary for a site.
 
         The connectivity angles are the angles between a site and its
         next nearest neighbors.
 
         Args:
             site_index: The site index (zero based).
@@ -414,15 +410,15 @@
             connectivity = nnn_site["connectivity"]
             connectivities[to_site][connectivity].extend(nnn_site["angles"])
 
         return defaultdict_to_dict(connectivities)
 
     def get_nnn_distance_summary(
         self, site_index: int
-    ) -> Dict[int, Dict[str, List[float]]]:
+    ) -> dict[int, dict[str, list[float]]]:
         """Gets the next nearest neighbor distance summary for a site.
 
         Args:
             site_index: The site index (zero based).
 
         Returns:
             The connectivity distance data for the site, formatted as::
@@ -464,15 +460,15 @@
             Where ``site_summary`` has the same format as produced by
             :meth:`SiteAnalyzer.get_site_summary`.
         """
         return {
             site: self.get_site_summary(site) for site in set(self.equivalent_sites)
         }
 
-    def get_all_bond_distance_summaries(self) -> Dict[int, Dict[int, List[float]]]:
+    def get_all_bond_distance_summaries(self) -> dict[int, dict[int, list[float]]]:
         """Gets the bond distance summaries for all sites.
 
         Returns:
             The bond distance summaries for all sites, formatted as::
 
                 {
                     from_site: {
@@ -486,15 +482,15 @@
         return {
             from_site: self.get_bond_distance_summary(from_site)
             for from_site in set(self.equivalent_sites)
         }
 
     def get_all_connectivity_angle_summaries(
         self,
-    ) -> Dict[int, Dict[int, Dict[str, List[float]]]]:
+    ) -> dict[int, dict[int, dict[str, list[float]]]]:
         """Gets the connectivity angle summaries for all sites.
 
         The connectivity angles are the angles between a site and its
         next nearest neighbors.
 
         Returns:
             The connectivity angle summaries for all sites, formatted as::
@@ -515,15 +511,15 @@
         return {
             from_site: self.get_connectivity_angle_summary(from_site)
             for from_site in set(self.equivalent_sites)
         }
 
     def get_all_nnn_distance_summaries(
         self,
-    ) -> Dict[int, Dict[int, Dict[str, List[float]]]]:
+    ) -> dict[int, dict[int, dict[str, list[float]]]]:
         """Gets the next nearest neighbor distance summaries for all sites.
 
         Returns:
             The next nearest neighbor distance summaries for all sites,
             formatted as::
 
                 {
@@ -540,36 +536,36 @@
             :obj:`float` of distances.
         """
         return {
             from_site: self.get_nnn_distance_summary(from_site)
             for from_site in set(self.equivalent_sites)
         }
 
-    def get_inequivalent_site_indices(self, site_indices: List[int]) -> List[int]:
+    def get_inequivalent_site_indices(self, site_indices: list[int]) -> list[int]:
         """Gets the inequivalent site indices from a list of site indices.
 
         Args:
             site_indices: The site indices.
 
         Returns:
             The inequivalent site indices. For example, if a structure has 4
             sites where the first two are equivalent and the last two are
             inequivalent. If  ``site_indices=[0, 1, 2, 3]`` the output will be::
 
                 [0, 0, 2, 3]
 
         """
-        return list(self.equivalent_sites[i] for i in site_indices)
+        return [self.equivalent_sites[i] for i in site_indices]
 
     def _calculate_equivalent_sites(
         self,
         likeness_tol: float = 0.001,
         bond_dist_tol: float = 0.01,
         bond_angle_tol: float = 0.1,
-    ) -> List[int]:
+    ) -> list[int]:
         """Determines the indices of the structurally inequivalent sites.
 
         Args:
             likeness_tol: The tolerance used to determine if two likeness
                 parameters are the same.
             bond_dist_tol: The tolerance used to determine if two bond lengths
                 are the same.
@@ -629,15 +625,15 @@
                     "nn_sites": nn_sites,
                     "nnn_sites": nnn_sites,
                 }
                 inequiv_sites[site_index] = site_data
 
         return equivalent_sites
 
-    def _calculate_symmetry_labels(self, sym_equivalent_atoms: List[int]) -> List[int]:
+    def _calculate_symmetry_labels(self, sym_equivalent_atoms: list[int]) -> list[int]:
         """Calculates the symmetry labels for all sites in the structure.
 
         The symmetry labels number the sites in the structure. If two sites
         are symmetrically equivalent they share the same symmetry label. The
         numbering begins at 1 for each element in the structure.
 
         Args:
@@ -669,18 +665,18 @@
                     symmetry_labels[el_index] = count
                     count += 1
 
         return [symmetry_labels[i] for i in sorted(symmetry_labels.keys())]
 
     def _get_poly_formula(
         self,
-        geometry: Dict[str, Any],
-        nn_sites: List[Dict[str, Any]],
-        nnn_sites: List[Dict[str, Any]],
-    ) -> Optional[str]:
+        geometry: dict[str, Any],
+        nn_sites: list[dict[str, Any]],
+        nnn_sites: list[dict[str, Any]],
+    ) -> str | None:
         """Gets the polyhedra formula of the nearest neighbor atoms.
 
         The polyhedral formula is effectively the sorted nearest neighbor
         atoms in a reduced format. For example, if the nearest neighbors are
         3 I atoms, 2 Br atoms and 1 Cl atom, the polyhedral formula will be
         "I3Br2Cl". The polyhedral formula will be ``None`` if the site geometry
         is not in :data:`robocrys.util.connected_geometries`.
@@ -697,40 +693,37 @@
             The polyhedral formula if the site geometry is in
             :data:`robocrys.util.connected_geometries` else ``None``.
         """
 
         def order_elements(el):
             if self.use_iupac_formula:
                 return [get_el_sp(el).X, el]
-            else:
-                return [get_el_sp(el).iupac_ordering, el]
+            return [get_el_sp(el).iupac_ordering, el]
 
         nnn_geometries = [nnn_site["geometry"] for nnn_site in nnn_sites]
 
         poly_formula = None
         if geometry["type"] in connected_geometries and any(
-            [
-                nnn_geometry["type"] in connected_geometries
-                for nnn_geometry in nnn_geometries
-            ]
+            nnn_geometry["type"] in connected_geometries
+            for nnn_geometry in nnn_geometries
         ):
             nn_els = [get_el(nn_site["element"]) for nn_site in nn_sites]
             comp = Composition("".join(nn_els))
             el_amt_dict = comp.get_el_amt_dict()
 
             poly_formula = ""
             for e in sorted(el_amt_dict.keys(), key=order_elements):
                 poly_formula += e
-                poly_formula += formula_double_format(el_amt_dict[e])
+                poly_formula += str(formula_double_format(el_amt_dict[e]))
 
         return poly_formula
 
 
 def geometries_match(
-    geometry_a: Dict[str, Any], geometry_b: Dict[str, Any], likeness_tol: float = 0.001
+    geometry_a: dict[str, Any], geometry_b: dict[str, Any], likeness_tol: float = 0.001
 ) -> bool:
     """Determine whether two site geometries match.
 
     Geometry data should be formatted the same as produced by
     :meth:`robocrys.site.SiteAnalyzer.get_site_geometry`.
 
     Args:
@@ -745,16 +738,16 @@
     return (
         geometry_a["type"] == geometry_b["type"]
         and abs(geometry_a["likeness"] - geometry_b["likeness"]) < likeness_tol
     )
 
 
 def nn_summaries_match(
-    nn_sites_a: List[Dict[str, Union[int, str]]],
-    nn_sites_b: List[Dict[str, Union[int, str]]],
+    nn_sites_a: list[dict[str, int | str]],
+    nn_sites_b: list[dict[str, int | str]],
     bond_dist_tol: float = 0.01,
     match_bond_dists: bool = True,
 ) -> bool:
     """Determine whether two sets of nearest neighbors match.
 
     Nearest neighbor data should be formatted the same as produced by
     :meth:`robocrys.site.SiteAnalyzer.get_nearest_neighbors`.
@@ -790,16 +783,16 @@
         for site_a, site_b in zip(nn_sites_a, nn_sites_b)
     ]
 
     return all(d and e for d, e in zip(dists_match, elements_match))
 
 
 def nnn_summaries_match(
-    nnn_sites_a: List[Dict[str, Any]],
-    nnn_sites_b: List[Dict[str, Any]],
+    nnn_sites_a: list[dict[str, Any]],
+    nnn_sites_b: list[dict[str, Any]],
     likeness_tol: float = 0.001,
     bond_angle_tol: float = 0.1,
     match_bond_angles: bool = True,
 ):
     """Determine whether two sets of next nearest neighbors match.
 
     Next nearest neighbor data should be formatted the same as produced by
@@ -844,18 +837,16 @@
         geometries_match(
             site_a["geometry"], site_b["geometry"], likeness_tol=likeness_tol
         )
         for site_a, site_b in zip(nnn_sites_a, nnn_sites_b)
     ]
     angles_match = [
         all(
-            [
-                abs(a_a - a_b) < bond_angle_tol
-                for a_a, a_b in zip(sorted(site_a["angles"]), sorted(site_b["angles"]))
-            ]
+            abs(a_a - a_b) < bond_angle_tol
+            for a_a, a_b in zip(sorted(site_a["angles"]), sorted(site_b["angles"]))
         )
         if match_bond_angles
         else True
         for site_a, site_b in zip(nnn_sites_a, nnn_sites_b)
     ]
 
     return all(
```

### Comparing `robocrys-0.2.7/robocrys/condense/tests/test_component.py` & `robocrys-0.2.8/robocrys/condense/tests/test_component.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import os
 
 from pymatgen.analysis.dimensionality import get_structure_components
 from pymatgen.analysis.local_env import CrystalNN
 from pymatgen.analysis.structure_matcher import StructureMatcher
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
+from pytest import approx
 
 from robocrys.condense.component import (
     components_are_isomorphic,
     components_are_vdw_heterostructure,
     filter_molecular_components,
     get_component_formula,
     get_component_formula_and_factor,
@@ -43,120 +46,119 @@
         )
 
     def test_get_component_formula_and_factor(self):
         """Test getting the component formula and factor."""
         formula, factor = get_component_formula_and_factor(
             self.mapi_components[0], use_common_formulas=True, use_iupac_formula=True
         )
-        self.assertEqual(formula, "CH3NH3")
-        self.assertEqual(factor, 1)
+        assert formula == "CH3NH3"
+        assert factor == 1
 
         formula, factor = get_component_formula_and_factor(
             self.mapi_components[4], use_common_formulas=True, use_iupac_formula=True
         )
-        self.assertEqual(formula, "PbI3")
-        self.assertEqual(factor, 4)
+        assert formula == "PbI3"
+        assert factor == 4
 
         # test without common formulas
         formula, factor = get_component_formula_and_factor(
             self.mapi_components[0], use_common_formulas=False, use_iupac_formula=True
         )
-        self.assertEqual(formula, "CNH6")
-        self.assertEqual(factor, 1)
+        assert formula == "CNH6"
+        assert factor == 1
 
         # test without common formulas and without iupac formula
         formula, factor = get_component_formula_and_factor(
             self.mapi_components[0], use_common_formulas=False, use_iupac_formula=False
         )
-        self.assertEqual(formula, "H6CN")
-        self.assertEqual(factor, 1)
+        assert formula == "H6CN"
+        assert factor == 1
 
     def test_get_component_formula(self):
         """Test getting the component formula."""
         formula = get_component_formula(
             self.mapi_components[0], use_common_formulas=True, use_iupac_formula=True
         )
-        self.assertEqual(formula, "CH3NH3")
+        assert formula == "CH3NH3"
 
         formula = get_component_formula(
             self.mapi_components[4], use_common_formulas=True, use_iupac_formula=True
         )
-        self.assertEqual(formula, "PbI3")
+        assert formula == "PbI3"
 
         # test without common formulas
         formula = get_component_formula(
             self.mapi_components[0], use_common_formulas=False, use_iupac_formula=True
         )
-        self.assertEqual(formula, "CNH6")
+        assert formula == "CNH6"
 
         # test without common formulas and without iupac formula
         formula = get_component_formula(
             self.mapi_components[0], use_common_formulas=False, use_iupac_formula=False
         )
-        self.assertEqual(formula, "H6CN")
+        assert formula == "H6CN"
 
     def test_get_sym_inequiv_components(self):
         """Test getting symmetrically inequivalent structure components."""
         sga = SpacegroupAnalyzer(self.mapi.structure, symprec=0.01)
 
         inequiv_comp = get_sym_inequiv_components(self.mapi_components, sga)
 
-        self.assertEqual(len(inequiv_comp), 2)
-        self.assertEqual(inequiv_comp[0]["count"], 4)
-        self.assertEqual(inequiv_comp[1]["count"], 1)
+        assert len(inequiv_comp) == 2
+        assert inequiv_comp[0]["count"] == 4
+        assert inequiv_comp[1]["count"] == 1
 
     def test_get_comp_inequiv_components(self):
         """Test getting compositionally inequivalent structure components."""
-
         inequiv_comp = get_formula_inequiv_components(self.mapi_components)
 
-        self.assertEqual(len(inequiv_comp), 2)
-        self.assertEqual(inequiv_comp[0]["count"], 4)
-        self.assertEqual(inequiv_comp[0]["formula"], "CH3NH3")
-        self.assertEqual(inequiv_comp[1]["count"], 4)
-        self.assertEqual(inequiv_comp[1]["formula"], "PbI3")
+        assert len(inequiv_comp) == 2
+        assert inequiv_comp[0]["count"] == 4
+        assert inequiv_comp[0]["formula"] == "CH3NH3"
+        assert inequiv_comp[1]["count"] == 4
+        assert inequiv_comp[1]["formula"] == "PbI3"
 
         # Test not using common_formulas but with iupac formula
         inequiv_comp = get_formula_inequiv_components(
             self.mapi_components, use_iupac_formula=True, use_common_formulas=False
         )
-        self.assertEqual(inequiv_comp[0]["count"], 4)
-        self.assertEqual(inequiv_comp[0]["formula"], "CNH6")
+        assert inequiv_comp[0]["count"] == 4
+        assert inequiv_comp[0]["formula"] == "CNH6"
 
         # test non-iupac formula
         inequiv_comp = get_formula_inequiv_components(
             self.mapi_components, use_iupac_formula=False, use_common_formulas=False
         )
-        self.assertEqual(inequiv_comp[0]["count"], 4)
-        self.assertEqual(inequiv_comp[0]["formula"], "H6CN")
+        assert inequiv_comp[0]["count"] == 4
+        assert inequiv_comp[0]["formula"] == "H6CN"
 
     def test_filter_molecular_components(self):
         """Test filtering of molecular components."""
         mol_comps, comps = filter_molecular_components(self.mapi_components)
         mol_dimen = list({c["dimensionality"] for c in mol_comps})
         other_dimen = list({c["dimensionality"] for c in comps})
 
-        self.assertEqual(len(mol_comps), 4)
-        self.assertEqual(len(mol_dimen), 1)
-        self.assertEqual(mol_dimen[0], 0)
+        assert len(mol_comps) == 4
+        assert len(mol_dimen) == 1
+        assert mol_dimen[0] == 0
 
-        self.assertEqual(len(comps), 1)
-        self.assertTrue(0 not in other_dimen)
+        assert len(comps) == 1
+        assert 0 not in other_dimen
 
     def test_get_reconstructed_structure(self):
         structure = get_reconstructed_structure(
             self.mapi_components, simplify_molecules=False
         )
 
         # check the reconstructred structure matches the original using
         # pymatgen's structure matcher.
         sm = StructureMatcher(
             scale=False, primitive_cell=False, ltol=1e-4, stol=1e-4, angle_tol=1e-4
         )
-        self.assertTrue(sm.fit(structure, self.mapi.structure))
+        assert sm.fit(structure, self.mapi.structure)
 
         # Test the structure matches when we simplify molecules.
         # To do this we ignore all C, H, and N atoms.
         structure = get_reconstructed_structure(
             self.mapi_components, simplify_molecules=True
         )
 
@@ -164,90 +166,84 @@
             scale=False,
             primitive_cell=False,
             ltol=1e-4,
             stol=1e-4,
             angle_tol=1e-4,
             ignored_species=["C", "H", "N"],
         )
-        self.assertTrue(sm.fit(structure, self.mapi.structure))
+        assert sm.fit(structure, self.mapi.structure)
 
     def test_get_formula_from_components(self):
         formula = get_formula_from_components(
             self.mapi_components, use_common_formulas=True, use_iupac_formula=True
         )
-        self.assertTrue(formula, "CH3NH3PbI3")
+        assert formula, "CH3NH3PbI3"
 
         # check not using common formulas
         formula = get_formula_from_components(
             self.mapi_components, use_common_formulas=False, use_iupac_formula=True
         )
-        self.assertTrue(formula, "CNH6PbI3")
+        assert formula, "CNH6PbI3"
 
         # check non-iupac ordering works
         formula = get_formula_from_components(
             self.mapi_components, use_iupac_formula=False, use_common_formulas=False
         )
-        self.assertEqual(formula, "H6CNPbI3")
+        assert formula == "H6CNPbI3"
 
         # test multiple groups of different numbers of compositions
         s = CrystalNN().get_bonded_structure(self.get_structure("CuH8CN5Cl3"))
         comps = get_structure_components(s)
         formula = get_formula_from_components(
             comps, use_iupac_formula=True, use_common_formulas=True
         )
-        self.assertEqual(formula, "(CuCN4HCl)2(NH2)2(H2)3(HCl)4")
+        assert formula == "(CuCN4HCl)2(NH2)2(H2)3(HCl)4"
 
         # test putting molecules first
         s = CrystalNN().get_bonded_structure(self.get_structure("ZrCuH8C2NCl6"))
         comps = get_structure_components(s)
         formula = get_formula_from_components(
             comps,
             molecules_first=False,
             use_iupac_formula=True,
             use_common_formulas=True,
         )
-        self.assertEqual(formula, "ZrCuCl6(CH3)2NH2")
+        assert formula == "ZrCuCl6(CH3)2NH2"
 
         formula = get_formula_from_components(
             comps,
             molecules_first=True,
             use_iupac_formula=True,
             use_common_formulas=True,
         )
-        self.assertEqual(formula, "(CH3)2NH2ZrCuCl6")
+        assert formula == "(CH3)2NH2ZrCuCl6"
 
     def test_components_are_vdw_heterostructure(self):
         result = components_are_vdw_heterostructure(self.vdw_hetero_components)
-        self.assertTrue(result)
+        assert result
 
         result = components_are_vdw_heterostructure(self.mapi_components)
-        self.assertFalse(result)
+        assert not result
 
     def test_get_vdw_heterostructure_information(self):
         data = get_vdw_heterostructure_information(
             self.vdw_hetero_components,
             inc_ordered_components=True,
             inc_intercalants=True,
         )
-        self.assertEqual(len(data["ordered_components"]), 4)
-        self.assertAlmostEqual(
-            data["ordered_components"][0]["structure_graph"].structure.frac_coords[0][
-                0
-            ],
-            0.33330876,
-        )
-        self.assertAlmostEqual(
-            data["ordered_components"][3]["structure_graph"].structure.frac_coords[0][
-                0
-            ],
-            0.6666924,
-        )
-        self.assertEqual(data["repeating_unit"], ["MoS2", "WS2"])
-        self.assertEqual(data["num_repetitions"], 2)
-        self.assertEqual(data["intercalants"], [])
+        assert len(data["ordered_components"]) == 4
+        assert data["ordered_components"][0]["structure_graph"].structure.frac_coords[
+            0
+        ][0] == approx(0.33330876)
+        assert data["ordered_components"][3]["structure_graph"].structure.frac_coords[
+            0
+        ][0] == approx(0.6666924)
+        assert data["repeating_unit"] == ["MoS2", "WS2"]
+        assert data["num_repetitions"] == 2
+        assert data["intercalants"] == []
 
         # test error catching
         self.assertRaises(
             ValueError, get_vdw_heterostructure_information, self.mapi_components
         )
         self.assertRaises(
             KeyError,
@@ -256,43 +252,43 @@
         )
 
     def test_components_are_isomorphic(self):
         # check two CH3NH3 components are isomorphic
         result = components_are_isomorphic(
             self.mapi_components[0], self.mapi_components[1]
         )
-        self.assertTrue(result)
+        assert result
 
         # check CH3NH3 and PbI3 are not isomorphic
         result = components_are_isomorphic(
             self.mapi_components[0], self.mapi_components[4]
         )
-        self.assertFalse(result)
+        assert not result
 
     def test_get_structure_inequiv_components(self):
         inequiv_comp = get_structure_inequiv_components(
             self.mapi_components, use_structure_graph=False
         )
 
-        self.assertEqual(len(inequiv_comp), 2)
-        self.assertEqual(inequiv_comp[0]["count"], 4)
+        assert len(inequiv_comp) == 2
+        assert inequiv_comp[0]["count"] == 4
         # TODO: Uncomment out inequivalent ids when functionality implemented
         # self.assertEqual(inequiv_comp[0]['inequivalent_ids'],
         #                  (0, 8, 12, 44, 20, 28))
 
-        self.assertEqual(inequiv_comp[1]["count"], 1)
+        assert inequiv_comp[1]["count"] == 1
         # self.assertEqual(inequiv_comp[1]['inequivalent_ids'],
         #                  (32, 24, 36))
 
         # test using graph/fingerprint matching
         inequiv_comp = get_structure_inequiv_components(
             self.mapi_components, use_structure_graph=True
         )
 
-        self.assertEqual(len(inequiv_comp), 2)
-        self.assertEqual(inequiv_comp[0]["count"], 4)
+        assert len(inequiv_comp) == 2
+        assert inequiv_comp[0]["count"] == 4
         # self.assertEqual(inequiv_comp[0]['inequivalent_ids'],
         #                  (0, 8, 12, 44, 20, 28))
 
-        self.assertEqual(inequiv_comp[1]["count"], 1)
+        assert inequiv_comp[1]["count"] == 1
         # self.assertEqual(inequiv_comp[1]['inequivalent_ids'],
         #                  (32, 24, 36))
```

### Comparing `robocrys-0.2.7/robocrys/condense/tests/test_fingerprint.py` & `robocrys-0.2.8/robocrys/condense/tests/test_fingerprint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from __future__ import annotations
+
+from pytest import approx
+
 from robocrys.condense.fingerprint import (
     get_fingerprint_distance,
     get_site_fingerprints,
     get_structure_fingerprint,
 )
 from robocrys.tests import RobocrysTest
 
@@ -11,42 +15,43 @@
 
     def setUp(self):
         self.fe = self.get_structure("iron")
 
     def test_get_site_fingerprints(self):
         """Test to check site fingerprinting."""
         finger = get_site_fingerprints(self.fe)[0]
-        self.assertAlmostEqual(finger["body-centered cubic CN_8"], 0.576950507)
+        assert finger["body-centered cubic CN_8"] == approx(0.576950507)
 
         # check as_dict option
         finger = get_site_fingerprints(self.fe, as_dict=False)[0]
-        self.assertAlmostEqual(finger[30], 0.576950507)
+        assert finger[30] == approx(0.576950507)
 
     def test_get_structure_fingerprint(self):
         """Test to check structure fingerprinting."""
         fingerprint = get_structure_fingerprint(self.fe)
-        self.assertAlmostEqual(fingerprint[4], 1.98432036e-03)
+        assert fingerprint[4] == approx(1.98432036e-03)
 
         # test stats option
         fingerprint = get_structure_fingerprint(self.fe, stats=("mean",))
-        self.assertAlmostEqual(fingerprint[31], 2.51322893e-01)
+        assert fingerprint[31] == approx(2.51322893e-01)
 
-        # test preset options – reenable once fixed
+        # test preset options - re-enable once fixed
         # fingerprint = get_structure_fingerprint(
-        #     self.fe, preset='CrystalNNFingerprint_cn')
-        # self.assertAlmostEqual(fingerprint[2], 1.98432036e-03)
+        #     self.fe, preset="CrystalNNFingerprint_cn"
+        # )
+        # assert fingerprint[2] == approx(1.98432036e-03)
 
     def test_get_fingerprint_distance(self):
         """Tests to check getting fingerprint distance."""
         finger_1 = [0, 0, 0, 1]
         finger_2 = [1, 0, 0, 0]
         dist = get_fingerprint_distance(finger_1, finger_2)
-        self.assertAlmostEqual(dist, 1.4142135623730951)
+        assert dist == approx(1.4142135623730951)
 
         # test automatic conversion from structure to fingerprint
         dist = get_fingerprint_distance(self.fe, self.fe)
-        self.assertAlmostEqual(dist, 0.0)
+        assert dist == approx(0.0)
 
         # test one structure one fingerprint
         finger_1 = get_structure_fingerprint(self.fe)
         dist = get_fingerprint_distance(self.fe, finger_1)
-        self.assertAlmostEqual(dist, 0.0)
+        assert dist == approx(0.0)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `robocrys-0.2.7/robocrys/condense/tests/test_molecule.py` & `robocrys-0.2.8/robocrys/condense/tests/test_molecule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 
 from pymatgen.analysis.dimensionality import get_structure_components
 from pymatgen.analysis.local_env import CrystalNN
 
 from robocrys.condense.component import filter_molecular_components
 from robocrys.condense.molecule import MoleculeNamer
@@ -20,33 +22,33 @@
         mapi_components = get_structure_components(mapi, inc_molecule_graph=True)
         mol_components, _ = filter_molecular_components(mapi_components)
         self.methylammonium = mol_components[0]["molecule_graph"]
 
     def test_init(self):
         """Test initialising MoleculeNamer."""
         mn = MoleculeNamer()
-        self.assertTrue(mn)
+        assert mn
 
         mn = MoleculeNamer(use_online_pubchem=False)
-        self.assertTrue(mn)
+        assert mn
 
     def test_molecule_graph_to_smiles(self):
         """Test converting a molecule graph to SMILES string."""
         smiles = MoleculeNamer.molecule_graph_to_smiles(self.methylammonium)
-        self.assertEqual(smiles, "C[NH3]")
+        assert smiles == "C[NH3]"
 
     def test_get_name_from_pubchem(self):
         """Test downloading the molecule name from Pubchem."""
         mn = MoleculeNamer()
         name = mn.get_name_from_pubchem("C[NH3]")
-        self.assertEqual(name, "methylammonium")
+        assert name == "methylammonium"
 
     def test_get_name_from_molecule_graph(self):
         """Test getting a molecule name from the molecule graph."""
         mn = MoleculeNamer()
         name = mn.get_name_from_molecule_graph(self.methylammonium)
-        self.assertEqual(name, "methylammonium")
+        assert name == "methylammonium"
 
         # test iupac naming source
         mn = MoleculeNamer(name_preference=("iupac",))
         name = mn.get_name_from_molecule_graph(self.methylammonium)
-        self.assertEqual(name, "methylazanium")
+        assert name == "methylazanium"
```

### Comparing `robocrys-0.2.7/robocrys/condense/tests/test_site.py` & `robocrys-0.2.8/robocrys/condense/tests/test_site.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from __future__ import annotations
+
 from pymatgen.analysis.local_env import CrystalNN
+from pytest import approx
 
 from robocrys.condense.site import (
     SiteAnalyzer,
     geometries_match,
     nn_summaries_match,
     nnn_summaries_match,
 )
@@ -14,242 +17,240 @@
 
     def setUp(self):
         cnn = CrystalNN()
         self.tin_dioxide = cnn.get_bonded_structure(self.get_structure("SnO2"))
         self.ba_n = cnn.get_bonded_structure(self.get_structure("BaN2"))
 
     def test_init(self):
-        """Test to check SiteDescriber can be initialised"""
+        """Test to check SiteDescriber can be initialised."""
         sa = SiteAnalyzer(self.tin_dioxide)
-        self.assertNotEqual(sa, None, msg="tin dioxide site analyzer could not be init")
+        assert sa is not None, "tin dioxide site analyzer could not be init"
 
         # check different structure
         sa = SiteAnalyzer(self.ba_n)
-        self.assertNotEqual(sa, None, msg="BaN2 site analyzer could not be initialized")
+        assert sa is not None, "BaN2 site analyzer could not be initialized"
 
     def test_equivalent_sites(self):
         """Check equivalent sites instance variable set correctly."""
         sa = SiteAnalyzer(self.ba_n, use_symmetry_equivalent_sites=False)
-        self.assertEqual(sa.equivalent_sites, [0, 0, 0, 0, 4, 4])
+        assert sa.equivalent_sites == [0, 0, 0, 0, 4, 4]
 
         # test using symmetry to determine equivalent sites
         sa = SiteAnalyzer(self.ba_n, use_symmetry_equivalent_sites=True)
-        self.assertIsInstance(sa.equivalent_sites, list)
-        self.assertEqual(sa.equivalent_sites, [0, 0, 0, 0, 4, 4])
+        assert isinstance(sa.equivalent_sites, list)
+        assert sa.equivalent_sites == [0, 0, 0, 0, 4, 4]
 
         # test symprec option works
         sa = SiteAnalyzer(self.ba_n, use_symmetry_equivalent_sites=True, symprec=0.0001)
-        self.assertEqual(sa.equivalent_sites, [0, 1, 1, 0, 4, 4])
+        assert sa.equivalent_sites == [0, 1, 1, 0, 4, 4]
 
     def test_symmetry_labels(self):
         """Check equivalent sites instance variable set correctly."""
         sa = SiteAnalyzer(self.ba_n, use_symmetry_equivalent_sites=False)
-        self.assertEqual(sa.symmetry_labels, [1, 1, 1, 1, 1, 1])
+        assert sa.symmetry_labels == [1, 1, 1, 1, 1, 1]
 
     def test_get_site_geometry(self):
         """Test site geometry description."""
         sa = SiteAnalyzer(self.tin_dioxide)
         geom_data = sa.get_site_geometry(0)
-        self.assertEqual(geom_data["type"], "octahedral")
-        self.assertAlmostEqual(geom_data["likeness"], 0.9349776258427136)
+        assert geom_data["type"] == "octahedral"
+        assert geom_data["likeness"] == approx(0.9349776258427136)
 
         geom_data = sa.get_site_geometry(4)
-        self.assertEqual(geom_data["type"], "trigonal planar")
-        self.assertAlmostEqual(geom_data["likeness"], 0.6050243049545359)
+        assert geom_data["type"] == "trigonal planar"
+        assert geom_data["likeness"] == approx(0.6050243049545359)
 
         # check different structure
 
         sa = SiteAnalyzer(self.ba_n)
         geom_data = sa.get_site_geometry(0)
-        self.assertEqual(geom_data["type"], "6-coordinate")
-        self.assertAlmostEqual(geom_data["likeness"], 1)
+        assert geom_data["type"] == "6-coordinate"
+        assert geom_data["likeness"] == 1
 
     def test_get_nearest_neighbors(self):
         """Check getting nearest neighbors."""
         sa = SiteAnalyzer(self.tin_dioxide)
         info = sa.get_nearest_neighbors(4)
 
-        self.assertEqual(len(info), 3)
-        self.assertEqual(info[0]["element"], "Sn4+")
-        self.assertEqual(info[0]["inequiv_index"], 0)
-        self.assertAlmostEqual(info[0]["dist"], 2.0922101061490546)
+        assert len(info) == 3
+        assert info[0]["element"] == "Sn4+"
+        assert info[0]["inequiv_index"] == 0
+        assert info[0]["dist"] == approx(2.0922101061490546)
 
         info = sa.get_nearest_neighbors(0, inc_inequivalent_site_index=False)
-        self.assertTrue("inequiv_index" not in info[0])
+        assert "inequiv_index" not in info[0]
 
         # check different structure without oxi state
         sa = SiteAnalyzer(self.ba_n)
         info = sa.get_nearest_neighbors(0)
-        self.assertEqual(len(info), 6)
-        self.assertEqual(info[0]["element"], "N")
-        self.assertEqual(info[0]["inequiv_index"], 0)
-        self.assertAlmostEqual(info[0]["dist"], 1.2619877178483)
+        assert len(info) == 6
+        assert info[0]["element"] == "N"
+        assert info[0]["inequiv_index"] == 0
+        assert info[0]["dist"] == approx(1.2619877178483)
 
     def test_get_next_nearest_neighbors(self):
         """Check getting next nearest neighbors."""
         sa = SiteAnalyzer(self.tin_dioxide)
         info = sa.get_next_nearest_neighbors(5)
 
-        self.assertEqual(len(info), 14)
+        assert len(info) == 14
         idx = [i for i, s in enumerate(info) if s["connectivity"] == "edge"][0]
-        self.assertEqual(info[idx]["element"], "O2-")
-        self.assertEqual(info[idx]["connectivity"], "edge")
-        self.assertEqual(info[idx]["geometry"]["type"], "trigonal planar")
-        self.assertEqual(info[idx]["inequiv_index"], 2)
+        assert info[idx]["element"] == "O2-"
+        assert info[idx]["connectivity"] == "edge"
+        assert info[idx]["geometry"]["type"] == "trigonal planar"
+        assert info[idx]["inequiv_index"] == 2
 
         info = sa.get_next_nearest_neighbors(0, inc_inequivalent_site_index=False)
-        self.assertTrue("inequiv_index" not in info[0])
+        assert "inequiv_index" not in info[0]
 
         info = sa.get_next_nearest_neighbors(0)
-        self.assertEqual(info[0]["element"], "Sn4+")
-        self.assertEqual(info[0]["connectivity"], "edge")
-        self.assertEqual(info[0]["geometry"]["type"], "octahedral")
-        self.assertEqual(len(info[0]["angles"]), 2)
-        self.assertAlmostEqual(info[0]["angles"][0], 101.62287790513848)
-        self.assertAlmostEqual(info[0]["distance"], 3.24322132)
+        assert info[0]["element"] == "Sn4+"
+        assert info[0]["connectivity"] == "edge"
+        assert info[0]["geometry"]["type"] == "octahedral"
+        assert len(info[0]["angles"]) == 2
+        assert info[0]["angles"][0] == approx(101.62287790513848)
+        assert info[0]["distance"] == approx(3.24322132)
 
         # check different structure without oxi state
         sa = SiteAnalyzer(self.ba_n)
         info = sa.get_next_nearest_neighbors(0)
-        self.assertEqual(len(info), 36)
-        self.assertEqual(info[5]["element"], "N")
-        self.assertEqual(info[5]["connectivity"], "edge")
-        self.assertEqual(info[5]["geometry"]["type"], "6-coordinate")
-        self.assertEqual(len(info[5]["angles"]), 2)
-        self.assertAlmostEqual(info[5]["angles"][0], 83.91397867959587)
-        self.assertAlmostEqual(info[5]["distance"], 3.549136232944574)
+        assert len(info) == 36
+        assert info[5]["element"] == "N"
+        assert info[5]["connectivity"] == "edge"
+        assert info[5]["geometry"]["type"] == "6-coordinate"
+        assert len(info[5]["angles"]) == 2
+        assert info[5]["angles"][0] == approx(83.91397867959587)
+        assert info[5]["distance"] == approx(3.549136232944574)
 
     def test_get_site_summary(self):
-        """Test getting the site summary"""
+        """Test getting the site summary."""
         sa = SiteAnalyzer(self.tin_dioxide)
         data = sa.get_site_summary(0)
-        self.assertEqual(data["element"], "Sn4+")
-        self.assertEqual(data["geometry"]["type"], "octahedral")
-        self.assertAlmostEqual(data["geometry"]["likeness"], 0.9349776258427136)
-        self.assertEqual(len(data["nn"]), 6)
-        self.assertEqual(len(data["nnn"]["corner"]), 8)
-        self.assertEqual(len(data["nnn"]["edge"]), 2)
-        self.assertEqual(data["poly_formula"], "O6")
-        self.assertEqual(data["sym_labels"], (1,))
+        assert data["element"] == "Sn4+"
+        assert data["geometry"]["type"] == "octahedral"
+        assert data["geometry"]["likeness"] == approx(0.9349776258427136)
+        assert len(data["nn"]) == 6
+        assert len(data["nnn"]["corner"]) == 8
+        assert len(data["nnn"]["edge"]) == 2
+        assert data["poly_formula"] == "O6"
+        assert data["sym_labels"] == (1,)
 
     def test_get_bond_distance_summary(self):
-        """Test getting the bond distance summary"""
+        """Test getting the bond distance summary."""
         sa = SiteAnalyzer(self.tin_dioxide)
         data = sa.get_bond_distance_summary(0)
 
-        self.assertEqual(len(data[2]), 6)
-        self.assertAlmostEqual(data[2][0], 2.0922101061490546)
+        assert len(data[2]) == 6
+        assert data[2][0] == approx(2.0922101061490546)
 
     def test_connectivity_angle_summary(self):
-        """Test getting the connectivity angle summary"""
+        """Test getting the connectivity angle summary."""
         sa = SiteAnalyzer(self.tin_dioxide)
         data = sa.get_connectivity_angle_summary(0)
 
-        self.assertEqual(len(data[0]["corner"]), 8)
-        self.assertEqual(len(data[0]["edge"]), 4)
-        self.assertAlmostEqual(data[0]["edge"][0], 101.62287790513848)
+        assert len(data[0]["corner"]) == 8
+        assert len(data[0]["edge"]) == 4
+        assert data[0]["edge"][0] == approx(101.62287790513848)
 
     def test_nnn_distance_summary(self):
-        """Test getting the nnn distance summary"""
+        """Test getting the nnn distance summary."""
         sa = SiteAnalyzer(self.tin_dioxide)
         data = sa.get_nnn_distance_summary(0)
 
-        self.assertEqual(len(data[0]["corner"]), 8)
-        self.assertEqual(len(data[0]["edge"]), 2)
-        self.assertAlmostEqual(data[0]["edge"][0], 3.24322132)
+        assert len(data[0]["corner"]) == 8
+        assert len(data[0]["edge"]) == 2
+        assert data[0]["edge"][0] == approx(3.24322132)
 
     def test_get_all_site_summaries(self):
         """Test getting all the site summaries."""
         sa = SiteAnalyzer(self.tin_dioxide)
         data = sa.get_all_site_summaries()
-        self.assertEqual(len(data.keys()), 2)
-        self.assertEqual(data[0]["element"], "Sn4+")
-        self.assertEqual(data[0]["geometry"]["type"], "octahedral")
-        self.assertAlmostEqual(data[0]["geometry"]["likeness"], 0.9349776258427136)
-        self.assertEqual(len(data[0]["nn"]), 6)
-        self.assertEqual(len(data[0]["nnn"]["corner"]), 8)
-        self.assertEqual(len(data[0]["nnn"]["edge"]), 2)
-        self.assertEqual(data[0]["poly_formula"], "O6")
-        self.assertEqual(data[0]["sym_labels"], (1,))
+        assert len(data.keys()) == 2
+        assert data[0]["element"] == "Sn4+"
+        assert data[0]["geometry"]["type"] == "octahedral"
+        assert data[0]["geometry"]["likeness"] == approx(0.9349776258427136)
+        assert len(data[0]["nn"]) == 6
+        assert len(data[0]["nnn"]["corner"]) == 8
+        assert len(data[0]["nnn"]["edge"]) == 2
+        assert data[0]["poly_formula"] == "O6"
+        assert data[0]["sym_labels"] == (1,)
 
     def test_get_all_bond_distance_summaries(self):
         sa = SiteAnalyzer(self.tin_dioxide)
         data = sa.get_all_bond_distance_summaries()
-        self.assertEqual(len(data[0][2]), 6)
-        self.assertEqual(len(data[2][0]), 3)
-        self.assertAlmostEqual(data[0][2][0], 2.0922101061490546)
+        assert len(data[0][2]) == 6
+        assert len(data[2][0]) == 3
+        assert data[0][2][0] == approx(2.0922101061490546)
 
     def test_get_all_connectivity_angle_summaries(self):
         sa = SiteAnalyzer(self.tin_dioxide)
         data = sa.get_all_connectivity_angle_summaries()
-        self.assertEqual(len(data[0][0]["corner"]), 8)
-        self.assertEqual(len(data[0][0]["edge"]), 4)
-        self.assertAlmostEqual(data[0][0]["edge"][0], 101.62287790513848)
+        assert len(data[0][0]["corner"]) == 8
+        assert len(data[0][0]["edge"]) == 4
+        assert data[0][0]["edge"][0] == approx(101.62287790513848)
 
     def test_get_all_nnn_distance_summaries(self):
         sa = SiteAnalyzer(self.tin_dioxide)
         data = sa.get_all_nnn_distance_summaries()
-        self.assertEqual(len(data[0][0]["corner"]), 8)
-        self.assertEqual(len(data[0][0]["edge"]), 2)
-        self.assertAlmostEqual(data[0][0]["edge"][0], 3.24322132)
+        assert len(data[0][0]["corner"]) == 8
+        assert len(data[0][0]["edge"]) == 2
+        assert data[0][0]["edge"][0] == approx(3.24322132)
 
     def test_get_inequivalent_site_indices(self):
         sa = SiteAnalyzer(self.ba_n, use_symmetry_equivalent_sites=False)
         inequiv_indices = sa.get_inequivalent_site_indices(list(range(6)))
-        self.assertEqual(inequiv_indices, [0, 0, 0, 0, 4, 4])
+        assert inequiv_indices == [0, 0, 0, 0, 4, 4]
 
         # test using symmetry to determine inequivalent sites.
         sa = SiteAnalyzer(self.ba_n, use_symmetry_equivalent_sites=True)
         inequiv_indices = sa.get_inequivalent_site_indices(list(range(6)))
-        self.assertEqual(inequiv_indices, [0, 0, 0, 0, 4, 4])
+        assert inequiv_indices == [0, 0, 0, 0, 4, 4]
 
         # test symprec option
         sa = SiteAnalyzer(
             self.ba_n, use_symmetry_equivalent_sites=True, symprec=0.000001
         )
         inequiv_indices = sa.get_inequivalent_site_indices(list(range(6)))
-        self.assertEqual(inequiv_indices, [0, 1, 1, 0, 4, 4])
+        assert inequiv_indices == [0, 1, 1, 0, 4, 4]
 
     def test_geometries_match(self):
         """Test geometry matching function."""
         sa = SiteAnalyzer(self.tin_dioxide, use_symmetry_equivalent_sites=False)
         geom_a = sa.get_site_geometry(0)
         geom_b = sa.get_site_geometry(1)
         geom_c = sa.get_site_geometry(4)
 
-        self.assertTrue(geometries_match(geom_a, geom_b))
-        self.assertFalse(geometries_match(geom_a, geom_c))
+        assert geometries_match(geom_a, geom_b)
+        assert not geometries_match(geom_a, geom_c)
 
     def test_nn_summaries_match(self):
         """Test nearest neighbour summary matching function."""
         sa = SiteAnalyzer(self.ba_n, use_symmetry_equivalent_sites=True)
         nn_a = sa.get_nearest_neighbors(0)
         nn_b = sa.get_nearest_neighbors(1)
         nn_c = sa.get_nearest_neighbors(4)
 
-        self.assertTrue(nn_summaries_match(nn_a, nn_b))
-        self.assertFalse(nn_summaries_match(nn_a, nn_c))
+        assert nn_summaries_match(nn_a, nn_b)
+        assert not nn_summaries_match(nn_a, nn_c)
 
         # test bond dist tol works
-        self.assertFalse(nn_summaries_match(nn_a, nn_b, bond_dist_tol=1e-10))
+        assert not nn_summaries_match(nn_a, nn_b, bond_dist_tol=1e-10)
 
         # test not matching bond dists
-        self.assertTrue(
-            nn_summaries_match(nn_a, nn_b, bond_dist_tol=1e-10, match_bond_dists=False)
+        assert nn_summaries_match(
+            nn_a, nn_b, bond_dist_tol=1e-10, match_bond_dists=False
         )
 
     def test_nnn_summaries_match(self):
         """Test nearest neighbour summary matching function."""
         sa = SiteAnalyzer(self.ba_n, use_symmetry_equivalent_sites=True)
         nnn_a = sa.get_next_nearest_neighbors(0)
         nnn_b = sa.get_next_nearest_neighbors(3)
         nnn_c = sa.get_next_nearest_neighbors(4)
 
-        self.assertTrue(nnn_summaries_match(nnn_a, nnn_b))
-        self.assertFalse(nnn_summaries_match(nnn_a, nnn_c))
+        assert nnn_summaries_match(nnn_a, nnn_b)
+        assert not nnn_summaries_match(nnn_a, nnn_c)
 
         # test not matching bond angles
-        self.assertTrue(
-            nnn_summaries_match(
-                nnn_a, nnn_b, bond_angle_tol=1e-10, match_bond_angles=False
-            )
+        assert nnn_summaries_match(
+            nnn_a, nnn_b, bond_angle_tol=1e-10, match_bond_angles=False
         )
```

### Comparing `robocrys-0.2.7/robocrys/describe/adapter.py` & `robocrys-0.2.8/robocrys/describe/adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""
-This module implements a class to resolve the symbolic references in condensed
+"""This module implements a class to resolve the symbolic references in condensed
 structure data.
 """
+from __future__ import annotations
 
 from collections import defaultdict, namedtuple
-from typing import Any, Dict, List, Union
+from typing import Any
 
 import numpy as np
 from pymatgen.core.periodic_table import get_el_sp
 
 from robocrys.adapter import BaseAdapter
 
 ComponentDetails = namedtuple(
@@ -64,27 +64,26 @@
 
     Args:
         condensed_structure: The condensed structure data, formatted as produced
             by :meth:`robocrys.condense.StructureCondenser.condense_structure`.
     """
 
     def __init__(
-        self, condensed_structure: Dict[str, Any], use_iupac_ordering: bool = True
+        self, condensed_structure: dict[str, Any], use_iupac_ordering: bool = True
     ):
         super().__init__(condensed_structure)
 
         self.use_iupac_ordering = use_iupac_ordering
         self.sym_labels = {
-            site_index: self.get_sym_label(site_index)
-            for site_index in self.sites.keys()
+            site_index: self.get_sym_label(site_index) for site_index in self.sites
         }
 
     def get_nearest_neighbor_details(
         self, site_index: int, group: bool = False
-    ) -> List[NeighborSiteDetails]:
+    ) -> list[NeighborSiteDetails]:
         """Gets a summary of all the nearest neighbors to a site.
 
         Args:
             site_index: An inequivalent site index.
             group: Whether to group all nearest neighbor sites
                 with the same element together.
 
@@ -123,15 +122,15 @@
                 )
             )
 
         return sorted(nn_details, key=self._site_order)
 
     def get_next_nearest_neighbor_details(
         self, site_index: int, group: bool = False
-    ) -> List[NextNeighborSiteDetails]:
+    ) -> list[NextNeighborSiteDetails]:
         """Gets a summary of all the next nearest neighbors to a site.
 
         We only get the summaries for next nearest neighbor sites that have a
         geometry type listed in :attr:`robocrys.util.connected_geometries` and
         have a ``poly_formula``.
 
         Args:
@@ -204,15 +203,15 @@
                     count=sum([nn_site["count"] for nn_site in nnn_group]),
                     sym_label=self.get_sym_label(sites),
                 )
             )
 
         return sorted(nnn_details, key=self._site_order)
 
-    def get_component_details(self) -> List[ComponentDetails]:
+    def get_component_details(self) -> list[ComponentDetails]:
         """Gets a summary of all components.
 
         Returns:
             A :obj:`list` of ``ComponentDetails`` objects, each with the
             attributes:
 
             - ``count`` (``int``): The number of these components in the
@@ -237,15 +236,15 @@
                     nsites=len(self.components[index]["sites"]),
                     index=index,
                 )
             )
 
         return sorted(component_details, key=_component_order)
 
-    def get_component_groups(self) -> List[ComponentGroup]:
+    def get_component_groups(self) -> list[ComponentGroup]:
         """Gets a summary of all components groups.
 
         Returns:
             The components, grouped together by formula, dimensionality and
             molecule name. The data will be returned as a :obj:`list` of
             ``ComponentGroup`` objects, each with the attributes:
 
@@ -280,15 +279,15 @@
                     components=sorted(group, key=_component_order),
                     nsites=group[0].nsites,
                 )
             )
 
         return sorted(component_group_details, key=_component_order)
 
-    def get_component_site_groups(self, component_index: int) -> List[SiteGroup]:
+    def get_component_site_groups(self, component_index: int) -> list[SiteGroup]:
         """Gets a summary of the sites in a component.
 
         Returns:
             The sites, grouped together by element. The data will be returned
             as a :obj:`list` of ``SiteGroup`` objects, each with the attributes:
 
             - ``count`` (``int``): The total number of sites in this group.
@@ -309,63 +308,61 @@
                     element=element,
                     sites=group,
                 )
             )
 
         return sorted(site_groups, key=self._site_order)
 
-    def get_sym_label(self, site_indices: Union[int, List[int]]) -> str:
+    def get_sym_label(self, site_indices: int | list[int]) -> str:
         """Convert site indices into a formatted symmetry label.
 
         Args:
             site_indices:  THe site indices.
 
         Returns:
             The formatted symmetry label. E.g., if the set of symmetry labels
             for the sites looks like ``(1, 2)``, the symmetry label will be
             ``(1,2)``.
         """
-        if isinstance(site_indices, int) or isinstance(site_indices, np.int32):
+        if isinstance(site_indices, (int, np.int32)):
             # If only one to_site is provided turn it into a list
             site_indices = [site_indices]
 
         all_labels = sorted(
             [
                 label
                 for site_index in site_indices
                 for label in self.sites[site_index]["sym_labels"]
             ]
         )
         return "({})".format(",".join(map(str, sorted(all_labels))))
 
     def _site_order(
-        self, s: Union[SiteGroup, NeighborSiteDetails, NextNeighborSiteDetails]
+        self, s: SiteGroup | NeighborSiteDetails | NextNeighborSiteDetails
     ):
         """Utility function to help sort NeighborSiteDetails and SiteGroups."""
         specie = get_el_sp(s.element)
         x = specie.iupac_ordering if self.use_iupac_ordering else specie.X
 
         if isinstance(s, NeighborSiteDetails):
             return [x, s.count, s.sym_label, s.sites]
-        elif isinstance(s, NextNeighborSiteDetails):
+        if isinstance(s, NextNeighborSiteDetails):
             return [
                 s.connectivity,
                 s.geometry,
                 s.count,
                 x,
                 s.poly_formula,
                 s.sym_label,
                 s.sites,
             ]
-        else:
-            return [x, s.count, s.sites]
+        return [x, s.count, s.sites]
 
 
-def _component_order(c: Union[ComponentDetails, ComponentGroup]):
+def _component_order(c: ComponentDetails | ComponentGroup):
     """Utility function to help sort ComponentDetails and ComponentGroups."""
     mn = c.molecule_name if c.molecule_name else "z"
 
     if isinstance(c, ComponentDetails):
         ori = c.orientation if c.orientation else (0, 0, 0)
         return [mn, c.dimensionality, c.formula, ori, c.count]
-    else:
-        return [mn, c.dimensionality, c.formula, c.count]
+    return [mn, c.dimensionality, c.formula, c.count]
```

### Comparing `robocrys-0.2.7/robocrys/describe/describer.py` & `robocrys-0.2.8/robocrys/describe/describer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""
-This module provides a class for generating descriptions of condensed structure
+"""This module provides a class for generating descriptions of condensed structure
 data.
 
-TODO:
+Todo:
     * Indicate when molecules have been simplified in the mineral description.
     * Handle distortion in connected polyhedra description.
 """
+from __future__ import annotations
 
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any
 
 import inflect
 from pymatgen.util.string import htmlify, latexify, latexify_spacegroup, unicodeify
 
 from robocrys.describe.adapter import DescriptionAdapter
 from robocrys.util import (
     dimensionality_to_shape,
@@ -98,16 +98,16 @@
             self.angstrom = "Å"
             self.degree = "°"
 
         self._da: DescriptionAdapter = None
         self._seen_bonds: set = None
 
     def describe(
-        self, condensed_structure: Dict[str, Any]
-    ) -> Union[str, Dict[str, str]]:
+        self, condensed_structure: dict[str, Any]
+    ) -> str | dict[str, str]:
         """Convert a condensed structure into a text description.
 
         Args:
             condensed_structure: The condensed structure data, formatted as
                 produced by :meth:`StructureCondenser.condense_structure`.
 
         Returns:
@@ -134,16 +134,15 @@
 
         if not self.return_parts:
             return " ".join(
                 description[part]
                 for part in ["mineral", "component_makeup", "components"]
                 if part in description and description[part] != ""
             )
-        else:
-            return description
+        return description
 
     def get_mineral_description(self) -> str:
         """Gets the mineral name and space group description.
 
         If the structure is a perfect match for a known prototype (e.g.
         the distance parameter is -1, the mineral name is the prototype name.
         If a structure is not a perfect match but similar to a known mineral,
@@ -196,15 +195,15 @@
         ):
             desc = ""
 
         else:
             if self._da.dimensionality == 3:
                 desc = "The structure consists of "
             else:
-                desc = "The structure is {}-dimensional and consists of " "".format(
+                desc = "The structure is {}-dimensional and consists of ".format(
                     en.number_to_words(self._da.dimensionality)
                 )
 
             component_makeup_summaries = []
             nframeworks = len(
                 [
                     c
@@ -218,18 +217,15 @@
                     s_count = "a"
                 else:
                     s_count = en.number_to_words(component_group.count)
 
                 dimensionality = component_group.dimensionality
 
                 if component_group.molecule_name:
-                    if component_group.nsites == 1:
-                        shape = "atom"
-                    else:
-                        shape = "molecule"
+                    shape = "atom" if component_group.nsites == 1 else "molecule"
                     shape = en.plural(shape, s_count)
                     formula = component_group.molecule_name
                 else:
                     shape = en.plural(dimensionality_to_shape[dimensionality], s_count)
                     formula = component_group.formula
 
                 if self.fmt == "latex":
@@ -273,51 +269,47 @@
         """
         if len(self._da.components) == 1:
             return self.get_component_description(
                 self._da.get_component_groups()[0].components[0].index,
                 single_component=True,
             )
 
-        else:
-            component_groups = self._da.get_component_groups()
+        component_groups = self._da.get_component_groups()
+
+        component_descriptions = []
+        for group in component_groups:
+            for component in group.components:
+                if group.molecule_name:
+                    # don't describe known molecules
+                    continue
+
+                formula = group.formula
+                group_count = group.count
+                component_count = component.count
+                shape = dimensionality_to_shape[group.dimensionality]
+
+                if self.fmt == "latex":
+                    formula = latexify(formula)
+                elif self.fmt == "unicode":
+                    formula = unicodeify(formula)
+                elif self.fmt == "html":
+                    formula = htmlify(formula)
 
-            component_descriptions = []
-            for group in component_groups:
-                for component in group.components:
-
-                    if group.molecule_name:
-                        # don't describe known molecules
-                        continue
-
-                    formula = group.formula
-                    group_count = group.count
-                    component_count = component.count
-                    shape = dimensionality_to_shape[group.dimensionality]
-
-                    if self.fmt == "latex":
-                        formula = latexify(formula)
-                    elif self.fmt == "unicode":
-                        formula = unicodeify(formula)
-                    elif self.fmt == "html":
-                        formula = htmlify(formula)
-
-                    if group_count == component_count:
-                        s_filler = "the" if group_count == 1 else "each"
-                    else:
-                        s_filler = "{} of the".format(
-                            en.number_to_words(component_count)
-                        )
-                        shape = en.plural(shape)
+                if group_count == component_count:
+                    s_filler = "the" if group_count == 1 else "each"
+                else:
+                    s_filler = f"{en.number_to_words(component_count)} of the"
+                    shape = en.plural(shape)
 
-                    desc = f"In {s_filler} {formula} {shape}, "
-                    desc += self.get_component_description(component.index)
+                desc = f"In {s_filler} {formula} {shape}, "
+                desc += self.get_component_description(component.index)
 
-                    component_descriptions.append(desc)
+                component_descriptions.append(desc)
 
-            return " ".join(component_descriptions)
+        return " ".join(component_descriptions)
 
     def get_component_description(
         self, component_index: int, single_component: bool = False
     ) -> str:
         """Gets the descriptions of all sites in a component.
 
         Args:
@@ -327,31 +319,27 @@
 
         Returns:
             The description for all sites in the components.
         """
         desc = []
         first_group = True
         for site_group in self._da.get_component_site_groups(component_index):
-
             if len(site_group.sites) == 1:
                 desc.append(self.get_site_description(site_group.sites[0]))
 
             else:
                 element = get_formatted_el(
                     site_group.element,
                     "",
                     use_oxi_state=self.describe_oxidation_state,
                     use_sym_label=False,
                     fmt=self.fmt,
                 )
 
-                if first_group and not single_component:
-                    s_there = "there"
-                else:
-                    s_there = "There"
+                s_there = "there" if first_group and not single_component else "There"
 
                 s_count = en.number_to_words(len(site_group.sites))
 
                 desc.append(f"{s_there} are {s_count} inequivalent {element} sites.")
 
                 for i, site in enumerate(site_group.sites):
                     s_ordinal = en.number_to_words(en.ordinal(i + 1))
@@ -587,15 +575,15 @@
             bond_descriptions.append(
                 self.get_bond_length_description(site_index, nn_site.sites)
             )
 
         # filter empty bond length description strings
         return " ".join(filter(lambda x: x, bond_descriptions))
 
-    def get_bond_length_description(self, from_site: int, to_sites: List[int]) -> str:
+    def get_bond_length_description(self, from_site: int, to_sites: list[int]) -> str:
         """Gets a description of the bond lengths between two sets of sites.
 
         Args:
             from_site: An inequivalent site index.
             to_sites: A :obj:`list` of site indices. The site indices should
                 all be for the same element.
 
@@ -623,53 +611,51 @@
             use_sym_label=self.describe_symmetry_labels,
         )
 
         dists = self._da.get_distance_details(from_site, to_sites)
 
         # if only one bond length
         if len(dists) == 1:
-            return "The {}–{} bond length is {}.".format(
+            return "The {}-{} bond length is {}.".format(
                 from_element, to_element, self._distance_to_string(dists[0])
             )
 
         discrete_bond_lengths = self._rounded_bond_lengths(dists)
 
         # if multiple bond lengths but they are all the same
         if len(set(discrete_bond_lengths)) == 1:
             s_intro = "Both" if len(discrete_bond_lengths) == 2 else "All"
-            return "{} {}–{} bond lengths are {}.".format(
+            return "{} {}-{} bond lengths are {}.".format(
                 s_intro, from_element, to_element, self._distance_to_string(dists[0])
             )
 
         # if two sets of bond lengths
         if len(set(discrete_bond_lengths)) == 2:
             small = min(discrete_bond_lengths)
             s_small_count = en.number_to_words(discrete_bond_lengths.count(small))
             big = max(discrete_bond_lengths)
             s_big_count = en.number_to_words(discrete_bond_lengths.count(big))
 
             s_length = en.plural("length", s_big_count)
 
             return (
-                "There {} {} shorter ({}) and {} " "longer ({}) {}–{} bond {}."
+                "There {} {} shorter ({}) and {} longer ({}) {}-{} bond {}."
             ).format(
                 en.plural_verb("is", s_small_count),
                 s_small_count,
                 self._distance_to_string(small),
                 s_big_count,
                 self._distance_to_string(big),
                 from_element,
                 to_element,
                 s_length,
             )
 
         # otherwise just detail the spread of bond lengths
-        return (
-            "There are a spread of {}–{} bond distances ranging from " "{}."
-        ).format(
+        return ("There are a spread of {}-{} bond distances ranging from {}.").format(
             from_element,
             to_element,
             self._distance_range_to_string(
                 min(discrete_bond_lengths), max(discrete_bond_lengths)
             ),
         )
 
@@ -706,25 +692,24 @@
             return ""
 
         # if only one bond length
         if len(tilts) == 1:
             if tilts[0] == 0:
                 return "The corner-sharing octahedra are not tilted"
 
-            else:
-                return "The corner-sharing octahedral tilt angles " "are {}".format(
-                    self._angle_to_string(tilts[0])
-                )
+            return "The corner-sharing octahedral tilt angles are {}".format(
+                self._angle_to_string(tilts[0])
+            )
 
         # otherwise just detail the spread of bond lengths
         return "The corner-sharing octahedral tilt angles range from {}".format(
             self._angle_range_to_string(min(tilts), max(tilts))
         )
 
-    def _filter_seen_bonds(self, from_site: int, to_sites: List[int]) -> List[int]:
+    def _filter_seen_bonds(self, from_site: int, to_sites: list[int]) -> list[int]:
         """Filter the list of to_sites to only include unseen bonds.
 
         Args:
             from_site: An inequivalent site index.
             to_sites: A :obj:`list` of site indices. The site indices should
                 all be for the same element.
 
@@ -741,58 +726,58 @@
         not_seen_to_sites = []
         for from_site, to_site in not_seen:
             not_seen_to_sites.append(to_site)
             self._seen_bonds.add(frozenset((from_site, to_site)))
 
         return not_seen_to_sites
 
-    def _rounded_bond_lengths(self, data: List[float]) -> Tuple[float]:
+    def _rounded_bond_lengths(self, data: list[float]) -> tuple[float]:
         """Function to round bond lengths to a number of decimal places."""
         return tuple(
             float("{:.{}f}".format(x, self.bond_length_decimal_places)) for x in data
         )
 
     def _distance_to_string(self, distance: float) -> str:
         """Utility function to round a distance and add an Angstrom symbol."""
         return "{:.{}f} {}".format(
             distance, self.bond_length_decimal_places, self.angstrom
         )
 
     def _distance_range_to_string(self, dist_a: float, dist_b: float) -> str:
         """Utility function to format a range of distances."""
-        return "{:.{}f}–{:.{}f} {}".format(
+        return "{:.{}f}-{:.{}f} {}".format(
             dist_a,
             self.bond_length_decimal_places,
             dist_b,
             self.bond_length_decimal_places,
             self.angstrom,
         )
 
-    def _rounded_angles(self, data: List[float]) -> Tuple[float]:
+    def _rounded_angles(self, data: list[float]) -> tuple[float]:
         """Function to round angles to a number of decimal places."""
         return tuple(
             float("{:.{}f}".format(x, self.angle_decimal_places)) for x in data
         )
 
     def _angle_to_string(self, angle: float) -> str:
         """Utility function to round a distance and add an Angstrom symbol."""
         return "{:.{}f}{}".format(angle, self.angle_decimal_places, self.degree)
 
     def _angle_range_to_string(self, angle_a: float, angle_b: float) -> str:
         """Utility function to format a range of distances."""
-        return "{:.{}f}–{:.{}f}{}".format(
+        return "{:.{}f}-{:.{}f}{}".format(
             angle_a,
             self.angle_decimal_places,
             angle_b,
             self.angle_decimal_places,
             self.degree,
         )
 
 
-def get_mineral_name(mineral_dict: Dict[str, Any]) -> Union[str, None]:
+def get_mineral_name(mineral_dict: dict[str, Any]) -> str | None:
     """Get the mineral name from a mineral dictionary.
 
     Args:
         mineral_dict: The mineral dictionary from the condensed description.
 
     Returns:
         If ``mineral_dict["type"]`` is set, the mineral name will be returned as
@@ -804,9 +789,8 @@
         elif mineral_dict["distance"] >= 0:
             suffix = "-like"
         else:
             suffix = ""
 
         return "{}{}".format(mineral_dict["type"], suffix)
 
-    else:
-        return None
+    return None
```

### Comparing `robocrys-0.2.7/robocrys/featurize/adapter.py` & `robocrys-0.2.8/robocrys/featurize/adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-"""
-This module implements a class to resolve the symbolic references in condensed
+"""This module implements a class to resolve the symbolic references in condensed
 structure data.
 """
+from __future__ import annotations
+
 import collections
 from statistics import mean
-from typing import Any, Dict, List, Optional, Set, Union
+from typing import Any
 
 from robocrys.adapter import BaseAdapter
 
 
 class FeaturizerAdapter(BaseAdapter):
     """Class to facilitate featurizing condensed structure data.
 
     Args:
         condensed_structure: The condensed structure data, formatted as produced
             by :meth:`robocrys.condense.StructureCondenser.condense_structure`.
     """
 
-    def __init__(self, condensed_structure: Dict[str, Any], distorted_tol: float = 0.6):
+    def __init__(self, condensed_structure: dict[str, Any], distorted_tol: float = 0.6):
         super().__init__(condensed_structure)
         self._all_sites = [
             site
             for component_index in self.component_makeup
             for site in self.components[component_index]["sites"]
         ]
         self._distorted_tol = distorted_tol
 
     @property
-    def component_dimensionalities(self) -> List[int]:
+    def component_dimensionalities(self) -> list[int]:
         """The dimensionalities of all components."""
         return sorted(c["dimensionality"] for c in self.components.values())
 
     @property
     def contains_named_molecule(self) -> bool:
         """Whether the structure contains any named molecules."""
         return any(c["molecule_name"] for c in self.components.values())
@@ -52,58 +53,50 @@
         return self.component_dimensionalities.count(3) > 1
 
     @property
     def contains_corner_sharing_polyhedra(self) -> bool:
         """Whether the structure contains corner-sharing polyhedra."""
         # criteria: original site poly, nnn site poly and sites corner-sharing
         return any(
-            [
-                site
-                for site in self.sites.values()
-                if site["poly_formula"]
-                and "corner" in site["nnn"]
-                and any(
-                    self.sites[nnn_site]["poly_formula"]
-                    for nnn_site in site["nnn"]["corner"]
-                )
-            ]
+            site
+            for site in self.sites.values()
+            if site["poly_formula"]
+            and "corner" in site["nnn"]
+            and any(
+                self.sites[nnn_site]["poly_formula"]
+                for nnn_site in site["nnn"]["corner"]
+            )
         )
 
     @property
     def contains_edge_sharing_polyhedra(self) -> bool:
         """Whether the structure contains edge-sharing polyhedra."""
         # criteria: original site poly, nnn site poly and sites edge-sharing
         return any(
-            [
-                site
-                for site in self.sites.values()
-                if site["poly_formula"]
-                and "edge" in site["nnn"]
-                and any(
-                    self.sites[nnn_site]["poly_formula"]
-                    for nnn_site in site["nnn"]["edge"]
-                )
-            ]
+            site
+            for site in self.sites.values()
+            if site["poly_formula"]
+            and "edge" in site["nnn"]
+            and any(
+                self.sites[nnn_site]["poly_formula"] for nnn_site in site["nnn"]["edge"]
+            )
         )
 
     @property
     def contains_face_sharing_polyhedra(self) -> bool:
         """Whether the structure contains face-sharing polyhedra."""
         # criteria: original site poly, nnn site poly and sites face-sharing
         return any(
-            [
-                site
-                for site in self.sites.values()
-                if site["poly_formula"]
-                and "face" in site["nnn"]
-                and any(
-                    self.sites[nnn_site]["poly_formula"]
-                    for nnn_site in site["nnn"]["face"]
-                )
-            ]
+            site
+            for site in self.sites.values()
+            if site["poly_formula"]
+            and "face" in site["nnn"]
+            and any(
+                self.sites[nnn_site]["poly_formula"] for nnn_site in site["nnn"]["face"]
+            )
         )
 
     @property
     def frac_sites_polyhedra(self) -> float:
         """The percentage of sites that are connected polyhedra."""
         return sum(
             bool(self.sites[site]["poly_formula"]) for site in self._all_sites
@@ -133,16 +126,15 @@
                     for nnn_site in nnn_sites
                     for angle in self.angles[site][nnn_site]["corner"]
                 ]
             )
 
         if angles:
             return mean(angles)
-        else:
-            return None
+        return None
 
     @property
     def average_coordination_number(self):
         """The average coordination number across all sites."""
         return mean([len(self.sites[site]["nn"]) for site in self._all_sites])
 
     @property
@@ -151,31 +143,29 @@
         cns = [
             len(self.sites[site]["nn"])
             for site in self._all_sites
             if "+" in self.sites[site]["element"]
         ]
         if cns:
             return mean(cns)
-        else:
-            # structure doesn't have oxidation states
-            return self.average_coordination_number
+        # structure doesn't have oxidation states
+        return self.average_coordination_number
 
     @property
     def average_anion_coordination_number(self):
         """The average coordination number across anion sites."""
         cns = [
             len(self.sites[site]["nn"])
             for site in self._all_sites
             if "-" in self.sites[site]["element"]
         ]
         if cns:
             return mean(cns)
-        else:
-            # structure doesn't have oxidation states
-            return self.average_coordination_number
+        # structure doesn't have oxidation states
+        return self.average_coordination_number
 
     def contains_molecule(self, molecule_name: str) -> bool:
         """Whether the structure contains a specific molecule name.
 
         Args:
             molecule_name: A molecule name.
 
@@ -183,85 +173,87 @@
             Whether the structure contains the molecule.
         """
         return any(
             c["molecule_name"] == molecule_name for c in self.components.values()
         )
 
     def is_dimensionality(
-        self, dimensionalities: Union[int, List[int], Set[int]]
+        self, dimensionalities: int | list[int] | set[int]
     ) -> bool:
         """Whether the structure only contains the specified dimensionalities.
 
         Args:
             dimensionalities: One or more dimensionalities.
 
         Returns:
             Whether the structure only contains the specified dimensionalities.
 
         """
+        try:
+            iterable = collections.Iterable
+        except:
+            iterable = collections.abc.Iterable
+
         if isinstance(dimensionalities, set):
             set_dimensionalities = dimensionalities
-        elif isinstance(dimensionalities, collections.Iterable):
+        elif isinstance(dimensionalities, iterable):
             set_dimensionalities = set(dimensionalities)
         else:
             set_dimensionalities = {dimensionalities}
         return set(self.component_dimensionalities) == set_dimensionalities
 
     def contains_geometry_type(
-        self, geometry: str, distorted: Optional[bool] = None
+        self, geometry: str, distorted: bool | None = None
     ) -> bool:
         """Whether the structure contains a specific site geometry.
 
         Args:
             geometry: The site geometry.
             distorted: Whether the geometry is distorted or not. If set to
                 ``None``, then the matching does not take into account the
                 geometry likeness.
 
         Returns:
             Whether the structure contains a specific geometry.
         """
         if distorted is None:
             return any(s["geometry"]["type"] == geometry for s in self.sites.values())
-        elif distorted:
+        if distorted:
             return any(
                 s["geometry"]["type"] == geometry
                 and s["geometry"]["likeness"] < self._distorted_tol
                 for s in self.sites.values()
             )
-        else:
-            return any(
-                s["geometry"]["type"] == geometry
-                and s["geometry"]["likeness"] > self._distorted_tol
-                for s in self.sites.values()
-            )
+        return any(
+            s["geometry"]["type"] == geometry
+            and s["geometry"]["likeness"] > self._distorted_tol
+            for s in self.sites.values()
+        )
 
     def contains_connected_geometry(self, connectivity: str, geometry: str) -> bool:
         """Whether the structure contains the specified connected geometry.
 
         Args:
             connectivity: The connectivity (corner, edge, face)
             geometry: The geometry.
 
         Returns:
             Whether the structure contains the specified connected geometry.
         """
         return any(
-            [
-                site
-                for site in self.sites.values()
-                if site["poly_formula"]
-                and site["geometry"]["type"] == geometry
-                and connectivity in site["nnn"]
-                and any(
-                    self.sites[nnn_site]["poly_formula"]
-                    for nnn_site in site["nnn"][connectivity]
-                    if self.sites[nnn_site]["geometry"]["type"] == geometry
-                )
-            ]
+            site
+            for site in self.sites.values()
+            if site["poly_formula"]
+            and site["geometry"]["type"] == geometry
+            and connectivity in site["nnn"]
+            and any(
+                self.sites[nnn_site]["poly_formula"]
+                for nnn_site in site["nnn"][connectivity]
+                if self.sites[nnn_site]["geometry"]["type"] == geometry
+            )
         )
 
     def frac_site_geometry(self, geometry: str) -> float:
         """The fraction of sites with a specific geometry.
 
         Args:
             geometry: The geometry.
```

### Comparing `robocrys-0.2.7/robocrys/featurize/featurizer.py` & `robocrys-0.2.8/robocrys/featurize/featurizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-"""
-This module contains a class to obtain robocrystallographer ML features.
-"""
+"""This module contains a class to obtain robocrystallographer ML features."""
+from __future__ import annotations
 
 from itertools import product
-from typing import List, Optional, Union
 
 from matminer.featurizers.base import BaseFeaturizer
 from numpy import mean
 from pymatgen.analysis.local_env import cn_opt_params
 from pymatgen.core.structure import Structure
 
 from robocrys import StructureCondenser
@@ -41,21 +39,21 @@
         condenser_kwargs: Keyword arguments that will be passed to
             :obj:`robocrys.condense.StructureCondenser`.
         distorted_tol: The value under which the site geometry will be
             classified as distorted.
     """
 
     def __init__(
-        self, condenser_kwargs: Optional[dict] = None, distorted_tol: float = 0.6
+        self, condenser_kwargs: dict | None = None, distorted_tol: float = 0.6
     ):
         condenser_kwargs = condenser_kwargs if condenser_kwargs else {}
         self._sc = StructureCondenser(**condenser_kwargs)
         self._distorted_tol = distorted_tol
 
-    def featurize(self, s: Structure) -> List[Union[float, bool, str]]:
+    def featurize(self, s: Structure) -> list[float | bool | str]:
         """Featurizes a structure using robocrystallographer.
 
         Args:
             s: A structure.
 
         Returns:
             The robocrystallographer features.
```

### Comparing `robocrys-0.2.7/robocrys/tests/__init__.py` & `robocrys-0.2.8/robocrys/tests/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import unittest
 
 from monty.json import MontyDecoder
 from monty.serialization import loadfn
 
 from robocrys.util import load_condensed_structure_json
```

### Comparing `robocrys-0.2.7/robocrys/tests/adapter.py` & `robocrys-0.2.8/robocrys/tests/adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from __future__ import annotations
+
+from pytest import approx
+
 from robocrys.adapter import BaseAdapter
 from robocrys.tests import RobocrysTest
 
 
 class TestDescriptionAdapter(RobocrysTest):
     """Class to test the base adapter functionality."""
 
@@ -9,46 +13,46 @@
         tin_dioxide = self.get_condensed_structure("SnO2")
         self.tin_dioxide_ba = BaseAdapter(tin_dioxide)
 
         mapi = self.get_condensed_structure("mapi")
         self.mapi_ba = BaseAdapter(mapi)
 
     def test_attributes(self):
-        self.assertEqual(self.mapi_ba.mineral["type"], "Orthorhombic Perovskite")
-        self.assertEqual(self.mapi_ba.mineral["distance"], -1)
-        self.assertEqual(self.mapi_ba.formula, "CH3NH3PbI3")
-        self.assertEqual(self.mapi_ba.spg_symbol, "Pnma")
-        self.assertEqual(self.mapi_ba.crystal_system, "orthorhombic")
-        self.assertEqual(self.mapi_ba.dimensionality, 3)
-        self.assertTrue(self.mapi_ba.sites)
-        self.assertTrue(self.mapi_ba.distances)
-        self.assertTrue(self.mapi_ba.angles)
-        self.assertTrue(self.mapi_ba.components)
-        self.assertTrue(self.mapi_ba.component_makeup)
-        self.assertEqual(self.mapi_ba.elements[0], "H+")
+        assert self.mapi_ba.mineral["type"] == "Orthorhombic Perovskite"
+        assert self.mapi_ba.mineral["distance"] == -1
+        assert self.mapi_ba.formula == "CH3NH3PbI3"
+        assert self.mapi_ba.spg_symbol == "Pnma"
+        assert self.mapi_ba.crystal_system == "orthorhombic"
+        assert self.mapi_ba.dimensionality == 3
+        assert self.mapi_ba.sites
+        assert self.mapi_ba.distances
+        assert self.mapi_ba.angles
+        assert self.mapi_ba.components
+        assert self.mapi_ba.component_makeup
+        assert self.mapi_ba.elements[0] == "H+"
 
     def test_get_distance_details(self):
         # test get distance using int works
         distances = self.tin_dioxide_ba.get_distance_details(0, 2)
-        self.assertTrue(len(distances), 3)
-        self.assertAlmostEqual(distances[0], 2.0922101061490546)
+        assert len(distances), 3
+        assert distances[0] == approx(2.0922101061490546)
 
         # test get distance using list works
         distances = self.tin_dioxide_ba.get_distance_details(0, [2])
-        self.assertTrue(len(distances), 3)
-        self.assertAlmostEqual(distances[0], 2.0922101061490546)
+        assert len(distances), 3
+        assert distances[0] == approx(2.0922101061490546)
 
         # test getting multiple distances
         distances = self.mapi_ba.get_distance_details(44, [0, 8])
-        self.assertTrue(len(distances), 4)
-        self.assertAlmostEqual(distances[0], 1.0386222568611572)
+        assert len(distances), 4
+        assert distances[0] == approx(1.0386222568611572)
 
     def test_get_angle_details(self):
         # test get angles using int works
         distances = self.tin_dioxide_ba.get_angle_details(0, 0, "corner")
-        self.assertTrue(len(distances), 8)
-        self.assertAlmostEqual(distances[0], 129.18849530149342)
+        assert len(distances), 8
+        assert distances[0] == approx(129.18849530149342)
 
         # test get angles using list works
         distances = self.tin_dioxide_ba.get_angle_details(0, [0], "corner")
-        self.assertTrue(len(distances), 8)
-        self.assertAlmostEqual(distances[0], 129.18849530149342)
+        assert len(distances), 8
+        assert distances[0] == approx(129.18849530149342)
```

### Comparing `robocrys-0.2.7/robocrys/tests/test_util.py` & `robocrys-0.2.8/robocrys/tests/test_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import unittest
 
 from pymatgen.core.periodic_table import get_el_sp
 
 from robocrys.util import (
     get_el,
@@ -17,109 +19,109 @@
 
 class TestDescriptionMethods(unittest.TestCase):
     """Class to test utility functions."""
 
     def test_common_formulas(self):
         from robocrys.util import common_formulas
 
-        self.assertEqual(common_formulas["H6CN"], "CH3NH3")
+        assert common_formulas["H6CN"] == "CH3NH3"
 
     def test_connected_geometries(self):
         from robocrys.util import connected_geometries
 
-        self.assertTrue("octahedral" in connected_geometries)
+        assert "octahedral" in connected_geometries
 
     def test_geometry_to_polyhedra(self):
         from robocrys.util import geometry_to_polyhedra
 
-        self.assertEqual(geometry_to_polyhedra["octahedral"], "octahedra")
+        assert geometry_to_polyhedra["octahedral"] == "octahedra"
 
     def test_polyhedra_plurals(self):
         from robocrys.util import polyhedra_plurals
 
-        self.assertEqual(polyhedra_plurals["pentagonal pyramid"], "pentagonal pyramids")
+        assert polyhedra_plurals["pentagonal pyramid"] == "pentagonal pyramids"
 
     def test_dimensionality_to_shape(self):
         from robocrys.util import dimensionality_to_shape
 
-        self.assertEqual(dimensionality_to_shape[3], "framework")
+        assert dimensionality_to_shape[3] == "framework"
 
     def test_superscript_number(self):
-        self.assertEqual(superscript_number("+23"), "⁺²³")
+        assert superscript_number("+23") == "⁺²³"
 
     def test_get_al(self):
-        """Test getting element names"""
+        """Test getting element names."""
         species = get_el_sp("Sn2+")
-        self.assertEqual(get_el(species), "Sn")
+        assert get_el(species) == "Sn"
 
         element = get_el_sp("Sn")
-        self.assertEqual(get_el(element), "Sn")
+        assert get_el(element) == "Sn"
 
-        self.assertEqual(get_el(50), "Sn")
+        assert get_el(50) == "Sn"
 
     def test_get_formatted_el(self):
         """Test getting formatted element strings."""
         species = get_el_sp("Sn2+")
         form_el = get_formatted_el(species, "")
-        self.assertEqual(form_el, "Sn2+")
+        assert form_el == "Sn2+"
 
         element = get_el_sp("Sn")
         form_el = get_formatted_el(element, "")
-        self.assertEqual(form_el, "Sn")
+        assert form_el == "Sn"
 
         form_el = get_formatted_el(get_el(50), "")
-        self.assertEqual(form_el, "Sn")
+        assert form_el == "Sn"
 
         form_el = get_formatted_el(
             "Sn2+", "(1,2)", use_oxi_state=True, use_sym_label=True, fmt="raw"
         )
-        self.assertEqual(form_el, "Sn(1,2)2+")
+        assert form_el == "Sn(1,2)2+"
 
         form_el = get_formatted_el(
             "Sn2+", "(1,2)", use_oxi_state=False, use_sym_label=True, fmt="raw"
         )
-        self.assertEqual(form_el, "Sn(1,2)")
+        assert form_el == "Sn(1,2)"
 
         form_el = get_formatted_el(
             "Sn2+", "(1,2)", use_oxi_state=True, use_sym_label=False, fmt="raw"
         )
-        self.assertEqual(form_el, "Sn2+")
+        assert form_el == "Sn2+"
 
         form_el = get_formatted_el(
             "Sn2+", "(1,2)", use_oxi_state=False, use_sym_label=False, fmt="raw"
         )
-        self.assertEqual(form_el, "Sn")
+        assert form_el == "Sn"
 
         form_el = get_formatted_el(
             "Sn2+", "(1,2)", use_oxi_state=True, use_sym_label=True, fmt="latex"
         )
-        self.assertEqual(form_el, "Sn(1,2)^{2+}")
+        assert form_el == "Sn(1,2)^{2+}"
 
         form_el = get_formatted_el(
             "Sn2+", "(1,2)", use_oxi_state=True, use_sym_label=True, fmt="html"
         )
-        self.assertEqual(form_el, "Sn(1,2)<sup>2+</sup>")
+        assert form_el == "Sn(1,2)<sup>2+</sup>"
 
         form_el = get_formatted_el(
             "Sn2+", "(1,2)", use_oxi_state=True, use_sym_label=True, fmt="unicode"
         )
-        self.assertEqual(form_el, "Sn(1,2)²⁺")
+        assert form_el == "Sn(1,2)²⁺"
 
     def test_unicodeify_spacegroup(self):
         spg_symbol = unicodeify_spacegroup("P-42_1m")
-        self.assertEqual(spg_symbol, "P̅42₁m")
+        assert spg_symbol == "P̅42₁m"
 
     def test_htmlify_spacegroup(self):
         spg_symbol = htmlify_spacegroup("P-42_1m")
-        self.assertEqual(spg_symbol, "P̅42<sub>1</sub>m")
+        assert spg_symbol == "P̅42<sub>1</sub>m"
 
     def test_load_condense_structure_json(self):
         condensed_structure = load_condensed_structure_json(
             os.path.join(test_dir, "condensed_structures", "SnO2.json.gz")
         )
 
         # check that the site keys are correctly converted from str to int
         site_keys = list(condensed_structure["sites"].keys())
-        self.assertIsInstance(site_keys[0], int)
+        assert isinstance(site_keys[0], int)
 
         component_keys = list(condensed_structure["components"].keys())
-        self.assertIsInstance(component_keys[0], int)
+        assert isinstance(component_keys[0], int)
```

### Comparing `robocrys-0.2.7/robocrys/util.py` & `robocrys-0.2.8/robocrys/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,83 +1,84 @@
-"""
-Miscellaneous utility functions and common data.
+"""Miscellaneous utility functions and common data.
 
 Attributes:
     common_formulas: A set of common formulas. The keys to the data are strings
         from :obj:`pymatgen.core.composition.Composition.reduced_formula`.
     connected_geometries: A list of geometries that are considered
         "connectable" polyhedra. E.g. Their face-sharing, edge-sharing, etc
         properties are of interest.
     geometry_to_polyhedra: A mapping from geometry type (e.g. octahedral) to the
         plural polyhedra name (e.g. octahedra).
     dimensionality_to_shape: A mapping from dimensionality to the component
         shape.
 """
+from __future__ import annotations
+
 import re
 from collections import defaultdict
-from typing import Any, Dict, List, Union
+from typing import Any
 
 from monty.json import MontyDecoder
 from monty.serialization import loadfn
 from pkg_resources import resource_filename
 from pymatgen.core.periodic_table import Element, Species, get_el_sp
 from pymatgen.util.string import latexify_spacegroup
 
-common_formulas: Dict[str, str] = loadfn(
+common_formulas: dict[str, str] = loadfn(
     resource_filename("robocrys.condense", "formula_db.json.gz")
 )
 
-connected_geometries: List[str] = [
+connected_geometries: list[str] = [
     "tetrahedral",
     "octahedral",
     "trigonal pyramidal",
     "square pyramidal",
     "trigonal bipyramidal",
     "pentagonal pyramidal",
     "hexagonal pyramidal",
     "pentagonal bipyramidal",
     "hexagonal bipyramidal",
     "cuboctahedral",
 ]
 
-geometry_to_polyhedra: Dict[str, str] = {
+geometry_to_polyhedra: dict[str, str] = {
     "octahedral": "octahedra",
     "tetrahedral": "tetrahedra",
     "trigonal pyramidal": "trigonal pyramid",
     "square pyramidal": "square pyramid",
     "trigonal bipyramidal": "trigonal bipyramid",
     "pentagonal pyramidal": "pentagonal pyramid",
     "hexagonal pyramidal": "hexagonal pyramid",
     "pentagonal bipyramidal": "pentagonal bipyramid",
     "hexagonal bipyramidal": "hexagonal bipyramid",
     "cuboctahedral": "cuboctahedra",
 }
 
-polyhedra_plurals: Dict[str, str] = {
+polyhedra_plurals: dict[str, str] = {
     "octahedra": "octahedra",
     "tetrahedra": "tetrahedra",
     "trigonal pyramid": "trigonal pyramids",
     "square pyramid": "square pyramids",
     "trigonal bipyramid": "trigonal bipyramids",
     "pentagonal pyramid": "pentagonal pyramids",
     "hexagonal pyramid": "hexagonal pyramids",
     "pentagonal bipyramid": "pentagonal bipyramids",
     "hexagonal bipyramid": "hexagonal bipyramids",
     "cuboctahedra": "cuboctahedra",
 }
 
-dimensionality_to_shape: Dict[int, str] = {
+dimensionality_to_shape: dict[int, str] = {
     3: "framework",
     2: "sheet",
     1: "ribbon",
     0: "cluster",
 }
 
 
-def get_el(obj: Union[Element, Species, str, int]) -> str:
+def get_el(obj: Element | Species | str | int) -> str:
     """Utility method to get an element str from a symbol, Element, or Specie.
 
     Args:
         obj: An arbitrary object. Supported objects are Element/Species objects,
             integers (representing atomic numbers), or strings (element
             symbols or species strings).
 
@@ -85,20 +86,19 @@
         The element as a string.
     """
     if isinstance(obj, str):
         obj = get_el_sp(obj)
 
     if isinstance(obj, Element):
         return obj.name
-    elif isinstance(obj, Species):
+    if isinstance(obj, Species):
         return obj.element.name
-    elif isinstance(obj, int):
+    if isinstance(obj, int):
         return Element.from_Z(obj).name
-    else:
-        raise ValueError(f"Unsupported element type: {type(obj)}.")
+    raise ValueError(f"Unsupported element type: {type(obj)}.")
 
 
 def get_formatted_el(
     element: str,
     sym_label: str,
     use_oxi_state: bool = True,
     use_sym_label: bool = True,
@@ -174,15 +174,14 @@
 
     Args:
         string: A string containing the numbers 0-9 or +/- characters.
 
     Returns:
         The superscript string.
     """
-
     if "." in string:
         # no unicode period exists
         return string
 
     subscript_unicode_map = {
         0: "⁰",
         1: "¹",
@@ -252,42 +251,43 @@
         spacegroup_symbol: A spacegroup symbol.
 
     Returns:
         The html formatted spacegroup symbol.
     """
     overline = "\u0305"  # u"\u0304" (macron) is also an option
     symbol = re.sub(r"_(\d+)", r"<sub>\1</sub>", spacegroup_symbol)
-    symbol = re.sub(r"-(\d)", fr"{overline}\1", symbol)
+    symbol = re.sub(r"-(\d)", rf"{overline}\1", symbol)
     return symbol
 
 
-def defaultdict_to_dict(dictionary: defaultdict) -> Dict:
+def defaultdict_to_dict(dictionary: defaultdict) -> dict:
     """Recursively convert nested :obj:`defaultdict` to :obj:`dict`.
 
     Args:
         dictionary: A defaultdict.
 
     Returns:
         The defaultdict as a :obj:`dict`.
     """
     if isinstance(dictionary, defaultdict):
-        dictionary = {k: defaultdict_to_dict(v) for k, v in dictionary.items()}
+        return {k: defaultdict_to_dict(v) for k, v in dictionary.items()}
     return dictionary
 
 
-def load_condensed_structure_json(filename: str) -> Dict[str, Any]:
+def load_condensed_structure_json(filename: str) -> dict[str, Any]:
     """Load condensed structure data from a file.
 
     Args:
         filename: The filename.
 
     Returns:
         The condensed structure data.
     """
 
-    # Json does not support using integeras a dictionary keys, therefore
+    # JSON does not support using integers a dictionary keys, therefore
     # manually convert dictionary keys from str to int if possible.
     def json_keys_to_int(x):
         if isinstance(x, dict):
             return {int(k) if k.isdigit() else k: v for k, v in x.items()}
+        return None
 
     return loadfn(filename, cls=MontyDecoder, object_hook=json_keys_to_int)
```

### Comparing `robocrys-0.2.7/robocrys.egg-info/SOURCES.txt` & `robocrys-0.2.8/robocrys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.7/setup.py` & `robocrys-0.2.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """"
 robocrystallographer: Automatic generation of crystal structure descriptions.
 """
+from __future__ import annotations
 
 from os.path import join as path_join
 
 from setuptools import find_packages, setup
 
-with open("README.md", "r") as file:
+with open("README.md") as file:
     long_description = file.read()
 
 version = open("robocrys/_version.py").readlines()[-1].split()[-1].strip("\"'")
 
 setup(
     name="robocrys",
     version=version,
@@ -51,37 +52,37 @@
         "monty",
         "pubchempy",
         "pybtex",
         "ruamel.yaml",
     ],
     extras_require={
         "docs": [
-            "sphinx==4.0.2",
-            "sphinx-argparse==0.2.5",
-            "sphinx_rtd_theme==0.5.2",
-            "sphinx-autodoc-typehints==1.12.0",
-            "m2r2==0.2.8",
+            "sphinx==5.3.0",
+            "sphinx-argparse==0.4.0",
+            "sphinx_rtd_theme==1.2.0",
+            "sphinx-autodoc-typehints==1.23.0",
+            "m2r2==0.3.2",
         ],
         "dev": ["tqdm", "pybel", "pebble", "maggma"],
-        "tests": ["pytest==6.2.4", "pytest-cov==2.12.1"],
+        "tests": ["pytest==7.3.1", "pytest-cov==4.0.0"],
         "lint": [
-            "coverage==5.5",
+            "coverage==7.2.5",
             "codacy-coverage==1.3.11",
-            "pycodestyle==2.7.0",
-            "mypy==0.910",
+            "pycodestyle==2.9.1",
+            "mypy==1.2.0",
             "pydocstyle==6.1.1",
-            "flake8==3.9.2",
-            "pylint==2.8.3",
-            "black==21.6b0",
+            "flake8==6.0.0",
+            "pylint==2.17.3",
+            "black==23.3.0",
         ],
     },
     package_data={
         "robocrys": [
             path_join("condense", "mineral_db.json.gz"),
             path_join("condense", "molecule_db.json.gz"),
             path_join("condense", "formula_db.json.gz"),
         ]
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     data_files=["LICENSE", "CONTRIBUTING.rst"],
     entry_points={"console_scripts": ["robocrys = robocrys.cli:main"]},
 )
```

