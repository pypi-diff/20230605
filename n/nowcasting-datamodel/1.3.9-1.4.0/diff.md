# Comparing `tmp/nowcasting_datamodel-1.3.9.tar.gz` & `tmp/nowcasting_datamodel-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.3.9.tar", last modified: Thu May  4 11:42:00 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.4.0.tar", last modified: Mon Jun  5 15:51:27 2023, max compression
```

## Comparing `nowcasting_datamodel-1.3.9.tar` & `nowcasting_datamodel-1.4.0.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.207097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_pv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9578 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.211097 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 11:42:00.000000 nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:42:00.215097 nowcasting_datamodel-1.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-04 11:41:45.000000 nowcasting_datamodel-1.3.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.258225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.258225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.258225 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.3.9/PKG-INFO` & `nowcasting_datamodel-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.3.9
+Version: 1.4.0
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
 
 # nowcasting_datamodel
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 Datamodel for the nowcasting project
 
 
 The data model has been made using `sqlalchemy` with a mirrored model in `pydantic`.
 
 ⚠️ Database tables are currently made automatically,
@@ -124,16 +124,17 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center"><a href="http://lostcoding.com"><img src="https://avatars.githubusercontent.com/u/20285369?v=4?s=100" width="100px;" alt="Brandon Ly"/><br /><sub><b>Brandon Ly</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=branberry" title="Code">💻</a></td>
-      <td align="center"><a href="https://github.com/lucasc896"><img src="https://avatars.githubusercontent.com/u/1273006?v=4?s=100" width="100px;" alt="Chris Lucas"/><br /><sub><b>Chris Lucas</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=lucasc896" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://lostcoding.com"><img src="https://avatars.githubusercontent.com/u/20285369?v=4?s=100" width="100px;" alt="Brandon Ly"/><br /><sub><b>Brandon Ly</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=branberry" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lucasc896"><img src="https://avatars.githubusercontent.com/u/1273006?v=4?s=100" width="100px;" alt="Chris Lucas"/><br /><sub><b>Chris Lucas</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=lucasc896" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dfulu"><img src="https://avatars.githubusercontent.com/u/41546094?v=4?s=100" width="100px;" alt="James Fulton"/><br /><sub><b>James Fulton</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=dfulu" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `nowcasting_datamodel-1.3.9/README.md` & `nowcasting_datamodel-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # nowcasting_datamodel
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 Datamodel for the nowcasting project
 
 
 The data model has been made using `sqlalchemy` with a mirrored model in `pydantic`.
 
 ⚠️ Database tables are currently made automatically,
@@ -113,16 +113,17 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center"><a href="http://lostcoding.com"><img src="https://avatars.githubusercontent.com/u/20285369?v=4?s=100" width="100px;" alt="Brandon Ly"/><br /><sub><b>Brandon Ly</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=branberry" title="Code">💻</a></td>
-      <td align="center"><a href="https://github.com/lucasc896"><img src="https://avatars.githubusercontent.com/u/1273006?v=4?s=100" width="100px;" alt="Chris Lucas"/><br /><sub><b>Chris Lucas</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=lucasc896" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://lostcoding.com"><img src="https://avatars.githubusercontent.com/u/20285369?v=4?s=100" width="100px;" alt="Brandon Ly"/><br /><sub><b>Brandon Ly</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=branberry" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lucasc896"><img src="https://avatars.githubusercontent.com/u/1273006?v=4?s=100" width="100px;" alt="Chris Lucas"/><br /><sub><b>Chris Lucas</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=lucasc896" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dfulu"><img src="https://avatars.githubusercontent.com/u/41546094?v=4?s=100" width="100px;" alt="James Fulton"/><br /><sub><b>James Fulton</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=dfulu" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `nowcasting_datamodel-1.3.9/diagram.png` & `nowcasting_datamodel-1.4.0/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/diagram_pv.png` & `nowcasting_datamodel-1.4.0/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/fake.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,15 @@
         session=session,
         start_datetime_utc=datetime(2023, 1, 1),
         end_datetime_utc=datetime(2023, 1, 8),
     )
     location = get_location(
         gsp_id=0, session=session, installed_capacity_mw=14000, label=national_gb_label
     )
+    model = MLModelSQL(name=model_name, version="0.1.2")
 
     session.add_all([location, datetime_interval, metric])
 
     metric_values = []
     for forecast_horizon in range(0, 60 * 9, 30):
         for minutes in range(0, 60 * 24, 30):
             time_of_day = time(hour=minutes // 60, minute=minutes % 60)
@@ -291,11 +292,12 @@
                 time_of_day=time_of_day,
                 forecast_horizon_minutes=forecast_horizon,
                 number_of_data_points=1,
                 datetime_interval=datetime_interval,
                 metric=metric,
                 location=location,
                 model_name=model_name,
+                model=model,
             )
             metric_values.append(m)
 
     return metric_values
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,12 +16,13 @@
 But there can be multiple forecasts for similar values.
 
 Later on it would be good to add a forecast latest table,
     where the latest forecast can be read.
 The primary keys could be 'gsp_id' and 'target_datetime_utc'.
 """
 
+from .api import *  # noqa F403
 from .forecast import *  # noqa F403
 from .gsp import *  # noqa F403
 from .metric import *  # noqa F403
 from .models import *  # noqa F403
 from .pv import *  # noqa F403
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/gsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,30 +30,30 @@
 
     id = Column(Integer, primary_key=True)
     label = Column(String)
     gsp_id = Column(Integer, index=True, unique=True, nullable=False)
     gsp_name = Column(String, nullable=True)
     gsp_group = Column(String, nullable=True)
     region_name = Column(String, nullable=True)
-    installed_capacity_mw = Column(Integer, nullable=True)
+    installed_capacity_mw = Column(Float, nullable=True)
 
     forecast = relationship("ForecastSQL", back_populates="location")
     gsp_yields = relationship("GSPYieldSQL", back_populates="location")
     metric_value = relationship("MetricValueSQL", back_populates="location")
 
 
 class Location(EnhancedBaseModel):
     """Location that the forecast is for"""
 
     label: str = Field(..., description="")
     gsp_id: Optional[int] = Field(None, description="The Grid Supply Point (GSP) id", index=True)
     gsp_name: Optional[str] = Field(None, description="The GSP name")
     gsp_group: Optional[str] = Field(None, description="The GSP group name")
     region_name: Optional[str] = Field(None, description="The GSP region name")
-    installed_capacity_mw: Optional[int] = Field(
+    installed_capacity_mw: Optional[float] = Field(
         None, description="The installed capacity of the GSP in MW"
     )
 
     rm_mode = True
 
     def to_orm(self) -> LocationSQL:
         """Change model to LocationSQL"""
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/blend.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         # sum the weights
         duplicated = duplicated.groupby(["target_time"]).sum()
 
         # make sure target_time is a columns
         duplicated["target_time"] = duplicated.index
         duplicated.reset_index(inplace=True, drop=True)
 
-        # divide by the sum of the weights
+        # divide by the sum of the weights, # TODO should we be worried about dividing by zero?
         duplicated["expected_power_generation_megawatts"] /= duplicated["weight"]
         duplicated["adjust_mw"] /= duplicated["weight"]
 
         logger.debug(duplicated)
     # join unique and duplicates together
     forecast_values_blended = pd.concat([forecast_values_blended, duplicated], axis=0)
     # sort by target time
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,25 +221,27 @@
 def get_all_gsp_ids_latest_forecast(
     session: Session,
     start_created_utc: Optional[datetime] = None,
     start_target_time: Optional[datetime] = None,
     preload_children: Optional[bool] = False,
     historic: bool = False,
     include_national: bool = True,
+    model_name: Optional[bool] = None,
 ) -> List[ForecastSQL]:
     """
     Read forecasts
 
     :param session: database session
     :param start_created_utc: Filter: forecast creation time should be larger than this datetime
     :param start_target_time:
         Filter: forecast values target time should be larger than this datetime
     :param preload_children: Option to preload children. This is a speed up, if we need them.
     :param historic: Option to load historic values or not
     :param include_national: Option to include national forecast or not
+    :param model_name: Optional to filter on model name
 
     return: List of forecasts objects from database
     """
 
     logger.debug(f"Getting latest forecast for all gsps, {include_national=}")
 
     if include_national:
@@ -250,14 +252,15 @@
     return get_latest_forecast_for_gsps(
         session=session,
         start_created_utc=start_created_utc,
         start_target_time=start_target_time,
         preload_children=preload_children,
         historic=historic,
         gsp_ids=gsp_ids,
+        model_name=model_name,
     )
 
 
 def get_latest_forecast_for_gsps(
     session: Session,
     start_created_utc: Optional[datetime] = None,
     start_target_time: Optional[datetime] = None,
@@ -302,28 +305,34 @@
             query = query.distinct(LocationSQL.gsp_id)
         query = query.filter(LocationSQL.gsp_id.in_(gsp_ids))
         order_by_cols.append(LocationSQL.gsp_id)
 
     # filter on historic
     query = query.filter(ForecastSQL.historic == historic)
 
-    # filter on model name
-    if model_name is not None:
-        query = query.join(MLModelSQL)
-        query = query.filter(MLModelSQL.name == model_name)
-
     # filter on target time
     if start_target_time is not None:
         query = filter_query_on_target_time(
             query=query,
             start_target_time=start_target_time,
             historic=historic,
             end_target_time=end_target_time,
         )
 
+    # filter on model name
+    if model_name is not None:
+        if historic:
+            # if start target time is None, we need to join with forecast value latest
+            if start_target_time is None:
+                query = query.join(ForecastValueLatestSQL)
+            query = query.join(MLModelSQL, ForecastValueLatestSQL.model_id == MLModelSQL.id)
+        else:
+            query = query.join(MLModelSQL)
+        query = query.filter(MLModelSQL.name == model_name)
+
     query = query.join(LocationSQL)
 
     # option to preload values, makes querying quicker
     if preload_children:
         query = query.options(joinedload(ForecastSQL.location))
         query = query.options(joinedload(ForecastSQL.model))
         query = query.options(joinedload(ForecastSQL.input_data_last_updated))
@@ -391,35 +400,42 @@
 
 
 def get_forecast_values(
     session: Session,
     gsp_id: Optional[int] = None,
     gsp_ids: Optional[List[int]] = None,
     start_datetime: Optional[datetime] = None,
+    end_datetime: Optional[datetime] = None,
     forecast_horizon_minutes: Optional[int] = None,
     only_return_latest: Optional[bool] = False,
     model: Optional = ForecastValueSQL,
     model_name: Optional[str] = None,
+    created_utc_limit: Optional[datetime] = None,
 ) -> List[ForecastValueSQL]:
     """
     Get forecast values
 
     :param session: database session
     :param gsp_id: optional to gsp id, to filter query on
         If None is given then all are returned. This should be changed to [gsp_id]
     :param gsp_ids: optional to provide multiple gsp id, to filter query on
         If None is given then all are returned.
     :param start_datetime: optional to filterer target_time by start_datetime
         If None is given then all are returned.
+    :param end_datetime: optional to filterer target_time by end_datetime
+        If None is given then all are returned.
     :param only_return_latest: Optional to only return the latest forecast, not all of them.
         Default is False
     :param forecast_horizon_minutes: Optional filter on forecast horizon. For example
         forecast_horizon_minutes=120, means load the forecast than was made 2 hours before the
         target time. Note this only works for non-historic data.
     :param model: Can be 'ForecastValueSQL' or 'ForecastValueSevenDaysSQL'
+    :param model_name: Optional to filter on model name
+    :param created_utc_limit: Optional to filter on created_utc.
+        We only get forecast that are made before this time
 
     return: List of forecasts values objects from database
 
     """
 
     # start main query
     assert model.__tablename__ in [
@@ -447,14 +463,20 @@
         query = query.filter(model.target_time >= start_datetime)
 
         # also filter on creation time, to speed up things
         created_utc_filter = start_datetime - timedelta(days=1)
         query = query.filter(model.created_utc >= created_utc_filter)
         query = query.filter(ForecastSQL.created_utc >= created_utc_filter)
 
+    if end_datetime is not None:
+        query = query.filter(model.target_time <= end_datetime)
+
+    if created_utc_limit is not None:
+        query = query.filter(model.created_utc <= created_utc_limit)
+
     if forecast_horizon_minutes is not None:
         # this seems to only work for postgres
         query = query.filter(
             model.target_time - model.created_utc
             >= text(f"interval '{forecast_horizon_minutes} minute'")
         )
         query = query.filter(
@@ -527,19 +549,25 @@
         query = query.filter(ForecastValueLatestSQL.created_utc >= created_utc_filter)
 
     # filter on gsp_id
     if gsp_id is not None:
         query = query.filter(ForecastValueLatestSQL.gsp_id == gsp_id)
 
     if model_name is not None:
+        # make sure we only get the latest
+        query = query.distinct(ForecastValueLatestSQL.target_time)
+
+        # filter on model name
         query = query.join(MLModelSQL, ForecastValueLatestSQL.model_id == MLModelSQL.id)
         query = query.filter(MLModelSQL.name == model_name)
 
     # order by target time and created time desc
-    query = query.order_by(ForecastValueLatestSQL.target_time)
+    query = query.order_by(
+        ForecastValueLatestSQL.target_time, ForecastValueLatestSQL.created_utc.desc()
+    )
 
     # get all results
     forecast_values_latest = query.all()
 
     for forecast_value in forecast_values_latest:
         forecast_value.created_utc = forecast_value.created_utc.replace(tzinfo=timezone.utc)
 
@@ -604,15 +632,15 @@
     return created_utc[0]
 
 
 def get_location(
     session: Session,
     gsp_id: int,
     label: Optional[str] = None,
-    installed_capacity_mw: Optional[int] = None,
+    installed_capacity_mw: Optional[float] = None,
 ) -> LocationSQL:
     """
     Get location object from gsp id
 
     :param session: database session
     :param gsp_id: gsp id of the location
     :param label: label of the location
@@ -698,15 +726,15 @@
     if get_national:
         nation = get_location(session=session, gsp_id=0, label=national_gb_label)
         locations = [nation] + locations
 
     return locations
 
 
-def get_model(session: Session, name: str, version: Optional[str]) -> MLModelSQL:
+def get_model(session: Session, name: str, version: Optional[str] = None) -> MLModelSQL:
     """
     Get model object from name and version
 
     :param session: database session
     :param name: name of the model
     :param version: version of the model
 
@@ -715,22 +743,26 @@
     """
 
     # start main query
     query = session.query(MLModelSQL)
 
     # filter on gsp_id
     query = query.filter(MLModelSQL.name == name)
-    query = query.filter(MLModelSQL.version == version)
+    if version is not None:
+        query = query.filter(MLModelSQL.version == version)
+
+    # gets the latest version
+    query = query.order_by(MLModelSQL.version.desc())
 
     # get all results
     models = query.all()
 
     if len(models) == 0:
         logger.debug(
-            f"Model for name {name} and version {version }does not exist so going to add it"
+            f"Model for name {name} and version {version} does not exist so going to add it"
         )
 
         model = MLModelSQL(name=name, version=version)
         session.add(model)
         session.commit()
 
     else:
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Read database functions
 
 1. Get the one metric
 2. get datetime interval
 """
 import logging
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import List, Optional
 
 from sqlalchemy.orm.session import Session
 
-from nowcasting_datamodel.models.metric import DatetimeIntervalSQL, MetricSQL, MetricValueSQL
+from nowcasting_datamodel.models import DatetimeIntervalSQL, MetricSQL, MetricValueSQL, MLModelSQL
 
 logger = logging.getLogger(__name__)
 
 
 def get_metric(session: Session, name: str) -> MetricSQL:
     """
     Get metric object from database
@@ -121,13 +121,23 @@
     query = query.order_by(
         MetricValueSQL.time_of_day,
         MetricValueSQL.forecast_horizon_minutes,
         MetricValueSQL.created_utc.desc(),
     )
 
     if model_name is not None:
-        query = query.filter(MetricValueSQL.model_name == model_name)
+        query = query.join(MLModelSQL)
+        query = query.filter(MLModelSQL.name == model_name)
 
     # get all results
     metric_values = query.all()
 
+    # add timezone, show be the same datetime interval for all
+    datetime_interval = metric_values[0].datetime_interval
+    datetime_interval.start_datetime_utc = datetime_interval.start_datetime_utc.replace(
+        tzinfo=timezone.utc
+    )
+    datetime_interval.end_datetime_utc = datetime_interval.end_datetime_utc.replace(
+        tzinfo=timezone.utc
+    )
+
     return metric_values
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/adjust.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Methods for adding adjust values to the forecast"""
 import logging
 from datetime import datetime, timedelta
-from typing import List
+from typing import List, Union
 
 import pandas as pd
 
-from nowcasting_datamodel.models import ForecastSQL, MetricValue, MetricValueSQL
+from nowcasting_datamodel.models import Forecast, ForecastSQL, MetricValue, MetricValueSQL
 from nowcasting_datamodel.read.read_metric import read_latest_me_national
 
 logger = logging.getLogger()
 
 
 def add_adjust_to_forecasts(forecasts_sql: List[ForecastSQL], session):
     """
@@ -42,24 +42,33 @@
     :param forecast: national forecast
     :param session:
     :return:
     """
 
     # get the target time and model name
     datetime_now = forecast.forecast_values[0].target_time
+    last_datetime = forecast.forecast_values[-1].target_time
     model_name = forecast.model.name
 
+    logger.debug(
+        f"Adding adjuster to national forecast for "
+        f"{datetime_now} and {model_name}, {last_datetime=}"
+    )
+
     # 1. read metric values
     latest_me = read_latest_me_national(session=session, model_name=model_name)
     assert len(latest_me) > 0
+    logger.debug(f"Found {len(latest_me)} latest ME values")
 
     # 2. filter value down to now onwards
+    # get the number of hours to go ahead, we've added 1 to make sure we use the last one as well
+    hours_ahead = get_forecast_horizon_from_forecast(forecast)
     # change to dataframe
     latest_me_df = reduce_metric_values_to_correct_forecast_horizon(
-        latest_me=latest_me, datetime_now=datetime_now
+        latest_me=latest_me, datetime_now=datetime_now, hours_ahead=hours_ahead
     )
     assert len(latest_me_df) > 0
 
     # 3. add values to forecast_values
     for forecast_value in forecast.forecast_values:
         target_time = forecast_value.target_time
         try:
@@ -70,16 +79,33 @@
             # add value to ForecastValueSQL
             forecast_value.adjust_mw = value
 
         except Exception:
             logger.debug(f"Could not find ME value for {target_time} in {latest_me_df}")
 
 
+def get_forecast_horizon_from_forecast(forecast: Union[ForecastSQL, Forecast]):
+    """
+    Get the number of hours ahead from the forecast
+
+    :param forecast:
+    :return:
+    """
+    datetime_now = forecast.forecast_values[0].target_time
+    last_datetime = forecast.forecast_values[-1].target_time
+    hours_ahead = int((last_datetime - datetime_now).seconds / 3600) + 1
+    hours_ahead += (last_datetime - datetime_now).days * 24
+
+    logger.debug(f"Hours ahead is {hours_ahead}, {last_datetime=}, {datetime_now=} ")
+
+    return hours_ahead
+
+
 def reduce_metric_values_to_correct_forecast_horizon(
-    latest_me: List[MetricValueSQL], datetime_now: datetime, hours_ahead=8
+    latest_me: List[MetricValueSQL], datetime_now: datetime, hours_ahead=4
 ) -> pd.DataFrame:
     """
     Change all latest ME results 2D to 1D array
 
     Start:
     # time forecast_horizon value
     # 00.00 0  0.1
@@ -109,14 +135,18 @@
     :return: dataframe containing
         'datetime'
         'time_of_day'
         'forecast_horizon'
         'value'
     """
 
+    logger.debug(
+        f"Reducing metric values to correct forecast horizon {datetime_now=} {hours_ahead=}"
+    )
+
     latest_me_df = pd.DataFrame([MetricValue.from_orm(m).dict() for m in latest_me])
 
     # Let now big a dataframe of datetimes from now onwards. Lets say the time is 04.30, then
     # time forecast_horizon value
     # 04.30 0  0.1
     # 05.00 30 0.2
     # 05.30 60 0.6
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/save.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,28 +17,31 @@
 
 
 def save(
     forecasts: List[ForecastSQL],
     session: Session,
     update_national: Optional[bool] = True,
     update_gsp: Optional[bool] = True,
+    apply_adjuster: Optional[bool] = True,
 ):
     """
     Save forecast to database
 
     1. Add sqlalchemy onjects to database
     2. Saves to 'latest' table aswell
 
     :param forecasts: list of sql forecasts
     :param session: database session
     :param update_national: Optional (default true), to update the national forecast
     :param update_gsp: Optional (default true), to update all the GSP forecasts
+    :param apply_adjuster: Optional (default true), to apply the adjuster
     """
-    logger.debug("Add Adjust to forecasts")
-    add_adjust_to_forecasts(session=session, forecasts_sql=forecasts)
+    if apply_adjuster:
+        logger.debug("Add Adjust to forecasts")
+        add_adjust_to_forecasts(session=session, forecasts_sql=forecasts)
 
     # save objects to database
     logger.debug("Saving models")
     session.add_all(forecasts)
     session.commit()
 
     logger.debug("Updating to latest")
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     # 2. create forecast value latest
     forecast_values = []
     for forecast_value in forecast.forecast_values:
         forecast_value_latest = change_forecast_value_to_latest(
             forecast_value,
             gsp_id=forecast.location.gsp_id,
             forecast_id=forecast_historic.id,
-            model_id=forecast_historic.model_id,
+            model_id=forecast.model_id,
         )
         logger.debug(f"{forecast_historic.model_id=}")
         forecast_values.append(forecast_value_latest.__dict__)
 
     # upsert forecast values
     upsert(session=session, model=ForecastValueLatestSQL, rows=forecast_values)
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.3.9
+Version: 1.4.0
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
 
 # nowcasting_datamodel
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 Datamodel for the nowcasting project
 
 
 The data model has been made using `sqlalchemy` with a mirrored model in `pydantic`.
 
 ⚠️ Database tables are currently made automatically,
@@ -124,16 +124,17 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center"><a href="http://lostcoding.com"><img src="https://avatars.githubusercontent.com/u/20285369?v=4?s=100" width="100px;" alt="Brandon Ly"/><br /><sub><b>Brandon Ly</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=branberry" title="Code">💻</a></td>
-      <td align="center"><a href="https://github.com/lucasc896"><img src="https://avatars.githubusercontent.com/u/1273006?v=4?s=100" width="100px;" alt="Chris Lucas"/><br /><sub><b>Chris Lucas</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=lucasc896" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://lostcoding.com"><img src="https://avatars.githubusercontent.com/u/20285369?v=4?s=100" width="100px;" alt="Brandon Ly"/><br /><sub><b>Brandon Ly</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=branberry" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lucasc896"><img src="https://avatars.githubusercontent.com/u/1273006?v=4?s=100" width="100px;" alt="Chris Lucas"/><br /><sub><b>Chris Lucas</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=lucasc896" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dfulu"><img src="https://avatars.githubusercontent.com/u/41546094?v=4?s=100" width="100px;" alt="James Fulton"/><br /><sub><b>James Fulton</b></sub></a><br /><a href="https://github.com/openclimatefix/nowcasting_datamodel/commits?author=dfulu" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `nowcasting_datamodel-1.3.9/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 nowcasting_datamodel.egg-info/SOURCES.txt
 nowcasting_datamodel.egg-info/dependency_links.txt
 nowcasting_datamodel.egg-info/requires.txt
 nowcasting_datamodel.egg-info/top_level.txt
 nowcasting_datamodel/migrations/__init__.py
 nowcasting_datamodel/migrations/app.py
 nowcasting_datamodel/models/__init__.py
+nowcasting_datamodel/models/api.py
 nowcasting_datamodel/models/base.py
 nowcasting_datamodel/models/convert.py
 nowcasting_datamodel/models/forecast.py
 nowcasting_datamodel/models/gsp.py
 nowcasting_datamodel/models/metric.py
 nowcasting_datamodel/models/models.py
 nowcasting_datamodel/models/pv.py
 nowcasting_datamodel/models/utils.py
 nowcasting_datamodel/read/__init__.py
 nowcasting_datamodel/read/read.py
 nowcasting_datamodel/read/read_gsp.py
 nowcasting_datamodel/read/read_metric.py
 nowcasting_datamodel/read/read_pv.py
+nowcasting_datamodel/read/read_user.py
 nowcasting_datamodel/read/blend/__init__.py
 nowcasting_datamodel/read/blend/blend.py
 nowcasting_datamodel/read/blend/utils.py
 nowcasting_datamodel/read/blend/weights.py
 nowcasting_datamodel/save/__init__.py
 nowcasting_datamodel/save/adjust.py
 nowcasting_datamodel/save/save.py
```

### Comparing `nowcasting_datamodel-1.3.9/setup.py` & `nowcasting_datamodel-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.4.0/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/tests/test_fake.py` & `nowcasting_datamodel-1.4.0/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/tests/test_fake_pv.py` & `nowcasting_datamodel-1.4.0/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/tests/test_national.py` & `nowcasting_datamodel-1.4.0/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.9/tests/test_utils.py` & `nowcasting_datamodel-1.4.0/tests/test_utils.py`

 * *Files identical despite different names*

