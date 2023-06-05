# Comparing `tmp/databaseRestoreIntegrity-1.0.1.tar.gz` & `tmp/databaseRestoreIntegrity-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databaseRestoreIntegrity-1.0.1.tar", last modified: Mon Jun  5 04:59:12 2023, max compression
+gzip compressed data, was "databaseRestoreIntegrity-1.0.2.tar", last modified: Mon Jun  5 05:50:20 2023, max compression
```

## Comparing `databaseRestoreIntegrity-1.0.1.tar` & `databaseRestoreIntegrity-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 04:59:12.740197 databaseRestoreIntegrity-1.0.1/
--rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 02:34:52.000000 databaseRestoreIntegrity-1.0.1/LICENSE.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:13:57.000000 databaseRestoreIntegrity-1.0.1/MANIFEST.in
--rw-r--r--   0 mhasan     (502) staff       (20)     2378 2023-06-05 04:59:12.740327 databaseRestoreIntegrity-1.0.1/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)      686 2023-06-05 04:48:32.000000 databaseRestoreIntegrity-1.0.1/README.md
--rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 03:25:16.000000 databaseRestoreIntegrity-1.0.1/pyproject.toml
--rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-05 04:59:12.742256 databaseRestoreIntegrity-1.0.1/setup.cfg
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 04:59:12.719318 databaseRestoreIntegrity-1.0.1/src/
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 04:59:12.735393 databaseRestoreIntegrity-1.0.1/src/databaseRestoreIntegrity/
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:23:11.000000 databaseRestoreIntegrity-1.0.1/src/databaseRestoreIntegrity/__init__.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2527 2023-06-05 04:08:18.000000 databaseRestoreIntegrity-1.0.1/src/databaseRestoreIntegrity/mysql.py
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 04:59:12.739332 databaseRestoreIntegrity-1.0.1/src/databaseRestoreIntegrity.egg-info/
--rw-r--r--   0 mhasan     (502) staff       (20)     2378 2023-06-05 04:59:12.000000 databaseRestoreIntegrity-1.0.1/src/databaseRestoreIntegrity.egg-info/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)      345 2023-06-05 04:59:12.000000 databaseRestoreIntegrity-1.0.1/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-05 04:59:12.000000 databaseRestoreIntegrity-1.0.1/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
--rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-05 04:59:12.000000 databaseRestoreIntegrity-1.0.1/src/databaseRestoreIntegrity.egg-info/top_level.txt
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 05:50:20.896263 databaseRestoreIntegrity-1.0.2/
+-rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 02:34:52.000000 databaseRestoreIntegrity-1.0.2/LICENSE.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:13:57.000000 databaseRestoreIntegrity-1.0.2/MANIFEST.in
+-rw-r--r--   0 mhasan     (502) staff       (20)     3613 2023-06-05 05:50:20.896346 databaseRestoreIntegrity-1.0.2/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)     1921 2023-06-05 05:47:06.000000 databaseRestoreIntegrity-1.0.2/README.md
+-rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 03:25:16.000000 databaseRestoreIntegrity-1.0.2/pyproject.toml
+-rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-05 05:50:20.900637 databaseRestoreIntegrity-1.0.2/setup.cfg
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 05:50:20.888604 databaseRestoreIntegrity-1.0.2/src/
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 05:50:20.891781 databaseRestoreIntegrity-1.0.2/src/databaseRestoreIntegrity/
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:23:11.000000 databaseRestoreIntegrity-1.0.2/src/databaseRestoreIntegrity/__init__.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2527 2023-06-05 04:08:18.000000 databaseRestoreIntegrity-1.0.2/src/databaseRestoreIntegrity/mysql.py
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 05:50:20.895584 databaseRestoreIntegrity-1.0.2/src/databaseRestoreIntegrity.egg-info/
+-rw-r--r--   0 mhasan     (502) staff       (20)     3613 2023-06-05 05:50:20.000000 databaseRestoreIntegrity-1.0.2/src/databaseRestoreIntegrity.egg-info/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)      345 2023-06-05 05:50:20.000000 databaseRestoreIntegrity-1.0.2/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-05 05:50:20.000000 databaseRestoreIntegrity-1.0.2/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-05 05:50:20.000000 databaseRestoreIntegrity-1.0.2/src/databaseRestoreIntegrity.egg-info/top_level.txt
```

### Comparing `databaseRestoreIntegrity-1.0.1/LICENSE.txt` & `databaseRestoreIntegrity-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.1/setup.cfg` & `databaseRestoreIntegrity-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = databaseRestoreIntegrity
-version = 1.0.1
+version = 1.0.2
 author = Maihraj Hasan
 author_email = maihrajhasan@gmail.com
 description = A package to check mysql restore integrity check
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `databaseRestoreIntegrity-1.0.1/src/databaseRestoreIntegrity/mysql.py` & `databaseRestoreIntegrity-1.0.2/src/databaseRestoreIntegrity/mysql.py`

 * *Files identical despite different names*

