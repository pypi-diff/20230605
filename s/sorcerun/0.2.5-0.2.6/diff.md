# Comparing `tmp/sorcerun-0.2.5.tar.gz` & `tmp/sorcerun-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.2.5.tar", last modified: Tue May 30 19:01:41 2023, max compression
+gzip compressed data, was "sorcerun-0.2.6.tar", last modified: Mon Jun  5 07:34:02 2023, max compression
```

## Comparing `sorcerun-0.2.5.tar` & `sorcerun-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:41.480824 sorcerun-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 19:01:30.000000 sorcerun-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-30 19:01:41.480824 sorcerun-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-30 19:01:30.000000 sorcerun-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:01:41.480824 sorcerun-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 19:01:30.000000 sorcerun-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:41.480824 sorcerun-0.2.5/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:41.480824 sorcerun-0.2.5/sorcerun_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:02.833937 sorcerun-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-05 07:33:51.000000 sorcerun-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 07:34:02.833937 sorcerun-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-05 07:33:51.000000 sorcerun-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:34:02.833937 sorcerun-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-05 07:33:51.000000 sorcerun-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:02.829937 sorcerun-0.2.6/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 07:34:02.000000 sorcerun-0.2.6/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:02.833937 sorcerun-0.2.6/sorcerun_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-05 07:33:51.000000 sorcerun-0.2.6/sorcerun_package/sacred_utils.py
```

### Comparing `sorcerun-0.2.5/LICENSE` & `sorcerun-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.5/PKG-INFO` & `sorcerun-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.5
+Version: 0.2.6
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.5/README.md` & `sorcerun-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.5/setup.py` & `sorcerun-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.2.5",
+    version="0.2.6",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred==0.8.4",
         "pymongo",
         "pyyaml",
```

### Comparing `sorcerun-0.2.5/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.2.6/sorcerun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.5
+Version: 0.2.6
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.5/sorcerun_package/auth_mongodb_option.py` & `sorcerun-0.2.6/sorcerun_package/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.5/sorcerun_package/cli.py` & `sorcerun-0.2.6/sorcerun_package/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,16 +48,28 @@
 
     param_grid = ParameterGrid([config])
     total_num_params = len(param_grid)
     print(f"Parameter grid contains {total_num_params} combinations")
 
     # Run the Sacred experiment with the provided adapter function and config
     for i, param in enumerate(param_grid):
-        print(f"Run {i+1}/{total_num_params} with config:\n{param}")
+        print(
+            "-" * 5
+            + "GRID RUN INFO: "
+            + f"Starting run {i+1}/{total_num_params}"
+            + "-" * 5
+        )
+        print(f"Config:\n{param}")
         run_sacred_experiment(adapter_func, param, auth_path)
+        print(
+            "-" * 5
+            + "GRID RUN INFO: "
+            + f"Completed run {i+1}/{total_num_params}"
+            + "-" * 5
+        )
 
 
 @sorcerun.group()
 def mongo():
     pass
```

### Comparing `sorcerun-0.2.5/sorcerun_package/mongodb_utils.py` & `sorcerun-0.2.6/sorcerun_package/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.5/sorcerun_package/sacred_utils.py` & `sorcerun-0.2.6/sorcerun_package/sacred_utils.py`

 * *Files identical despite different names*

