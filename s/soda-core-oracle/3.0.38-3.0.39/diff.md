# Comparing `tmp/soda-core-oracle-3.0.38.tar.gz` & `tmp/soda-core-oracle-3.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-oracle-3.0.38.tar", last modified: Fri May 19 03:35:09 2023, max compression
+gzip compressed data, was "soda-core-oracle-3.0.39.tar", last modified: Mon Jun  5 18:04:44 2023, max compression
```

## Comparing `soda-core-oracle-3.0.38.tar` & `soda-core-oracle-3.0.39.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 03:35:09.093995 soda-core-oracle-3.0.38/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-19 03:35:09.093995 soda-core-oracle-3.0.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-19 03:35:09.093995 soda-core-oracle-3.0.38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-19 03:34:25.000000 soda-core-oracle-3.0.38/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 03:35:09.093995 soda-core-oracle-3.0.38/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 03:35:09.093995 soda-core-oracle-3.0.38/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     9209 2023-05-19 03:34:25.000000 soda-core-oracle-3.0.38/soda/data_sources/oracle_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 03:35:09.093995 soda-core-oracle-3.0.38/soda_core_oracle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-19 03:35:09.000000 soda-core-oracle-3.0.38/soda_core_oracle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-19 03:35:09.000000 soda-core-oracle-3.0.38/soda_core_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 03:35:09.000000 soda-core-oracle-3.0.38/soda_core_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-19 03:35:09.000000 soda-core-oracle-3.0.38/soda_core_oracle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-19 03:35:09.000000 soda-core-oracle-3.0.38/soda_core_oracle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:04:44.267605 soda-core-oracle-3.0.39/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-05 18:04:44.267605 soda-core-oracle-3.0.39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-05 18:04:44.267605 soda-core-oracle-3.0.39/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-05 18:04:04.000000 soda-core-oracle-3.0.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:04:44.263605 soda-core-oracle-3.0.39/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:04:44.263605 soda-core-oracle-3.0.39/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     9209 2023-06-05 18:04:04.000000 soda-core-oracle-3.0.39/soda/data_sources/oracle_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 18:04:44.267605 soda-core-oracle-3.0.39/soda_core_oracle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-05 18:04:44.000000 soda-core-oracle-3.0.39/soda_core_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-05 18:04:44.000000 soda-core-oracle-3.0.39/soda_core_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 18:04:44.000000 soda-core-oracle-3.0.39/soda_core_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-05 18:04:44.000000 soda-core-oracle-3.0.39/soda_core_oracle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-05 18:04:44.000000 soda-core-oracle-3.0.39/soda_core_oracle.egg-info/top_level.txt
```

### Comparing `soda-core-oracle-3.0.38/setup.py` & `soda-core-oracle-3.0.39/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-oracle"
-package_version = "3.0.38"
+package_version = "3.0.39"
 # TODO Add proper description
 description = "Soda Core Oracle Package"
 
 requires = [f"soda-core=={package_version}", "oracledb==1.1.1"]
 # TODO Fix the params
 setup(
     name=package_name,
```

### Comparing `soda-core-oracle-3.0.38/soda/data_sources/oracle_data_source.py` & `soda-core-oracle-3.0.39/soda/data_sources/oracle_data_source.py`

 * *Files identical despite different names*

