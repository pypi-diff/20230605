# Comparing `tmp/dysweep-0.0.6.tar.gz` & `tmp/dysweep-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.0.6.tar", last modified: Fri Jun  2 22:59:03 2023, max compression
+gzip compressed data, was "dysweep-0.0.7.tar", last modified: Mon Jun  5 19:42:42 2023, max compression
```

## Comparing `dysweep-0.0.6.tar` & `dysweep-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:59:03.373344 dysweep-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 22:56:20.000000 dysweep-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-02 22:59:03.373344 dysweep-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-02 22:56:20.000000 dysweep-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:59:03.369344 dysweep-0.0.6/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 22:56:20.000000 dysweep-0.0.6/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-06-02 22:56:20.000000 dysweep-0.0.6/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21659 2023-06-02 22:56:20.000000 dysweep-0.0.6/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-02 22:56:20.000000 dysweep-0.0.6/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:59:03.373344 dysweep-0.0.6/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-02 22:59:03.000000 dysweep-0.0.6/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-02 22:59:03.000000 dysweep-0.0.6/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:59:03.000000 dysweep-0.0.6/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 22:59:03.000000 dysweep-0.0.6/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 22:59:03.373344 dysweep-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-02 22:56:20.000000 dysweep-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:42:42.111350 dysweep-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 19:40:29.000000 dysweep-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-05 19:42:42.111350 dysweep-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 19:40:29.000000 dysweep-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:42:42.111350 dysweep-0.0.7/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 19:40:29.000000 dysweep-0.0.7/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-06-05 19:40:29.000000 dysweep-0.0.7/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21659 2023-06-05 19:40:29.000000 dysweep-0.0.7/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-05 19:40:29.000000 dysweep-0.0.7/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:42:42.111350 dysweep-0.0.7/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-05 19:42:42.000000 dysweep-0.0.7/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-05 19:42:42.000000 dysweep-0.0.7/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:42:42.000000 dysweep-0.0.7/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 19:42:42.000000 dysweep-0.0.7/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 19:42:42.111350 dysweep-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-05 19:40:29.000000 dysweep-0.0.7/setup.py
```

### Comparing `dysweep-0.0.6/LICENSE` & `dysweep-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.6/PKG-INFO` & `dysweep-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.6
+Version: 0.0.7
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.6/dysweep/parallel.py` & `dysweep-0.0.7/dysweep/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,14 +114,16 @@
                     new_dir_name = f"{mx+1}{SPLIT}{resume_id}"
                     shutil.copytree(checkpoint_dir / dir_name,
                                     checkpoint_dir / new_dir_name)
                     shutil.rmtree(checkpoint_dir / dir_name)
 
                     # create a new checkpoint directory for the inner function
                     new_checkpoint_dir = checkpoint_dir / new_dir_name
+                    
+                    experiment_id = resume_id
                 else:
                     # if the run_id doesn't exist, then create a new run
                     # and create the subdirectory
                     if conf.use_lightning_logger:
                         from lightning.pytorch.loggers import WandbLogger
                         logger = WandbLogger(
                             project=conf.project,
@@ -164,39 +166,52 @@
                 sig = inspect.signature(function)
                 # get the parameters of the function
                 params = sig.parameters
                 # check that the function has two parameters
                 if len(params) != 3 or list(params.keys())[0] != "config" or list(params.keys())[1] != "logger" or list(params.keys())[2] != "checkpoint_dir":
                     raise ValueError(
                         "the run function should have the exact following parameters in order: (config, logger, checkpoint_dir)")
-
-                ret = function(sweep_config, logger, new_checkpoint_dir)
+                try:
+                    ret = function(sweep_config, logger, new_checkpoint_dir)
+                except Exception as e:
+                    # write exception into an err-log.txt file in the checkpoint_dir
+                    with open(new_checkpoint_dir / "err-log.txt", "w") as f:
+                        f.write(traceback.format_exc())
+                    raise e
             else:
                 # check the function signature matches
                 # the one we expect.
                 # in which there are two arguments with the first one
                 # named config and the second one named checkpoint_dir
 
                 # get the signature of the function
                 sig = inspect.signature(function)
                 # get the parameters of the function
                 params = sig.parameters
                 # check that the function has two parameters
                 if len(params) != 2 or list(params.keys())[0] != "config" or list(params.keys())[1] != "checkpoint_dir":
                     raise ValueError(
                         "the run function should have the exact following parameters in order: (config, checkpoint_dir)")
-                ret = function(sweep_config, new_checkpoint_dir)
+                try:
+                    ret = function(sweep_config, new_checkpoint_dir)
+                except Exception as e:
+                    # write exception into an err-log.txt file in the checkpoint_dir
+                    with open(new_checkpoint_dir / "err-log.txt", "w") as f:
+                        f.write(traceback.format_exc())
+                    raise e
 
             # remove the entire new_checkpoint_dir if the function has finished
             # running.
             shutil.copyfile(new_checkpoint_dir / "sweep_config.json",
                             checkpoint_dir / f"{experiment_id}-config.json")
             shutil.rmtree(new_checkpoint_dir)
 
             return ret
+        
+        
         if conf.resume:
             for _ in range(conf.count):
                 if check_non_empty(checkpoint_dir):
                     modified_function()
                 else:
                     break
         else:
```

### Comparing `dysweep-0.0.6/dysweep/utils.py` & `dysweep-0.0.7/dysweep/utils.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.6/dysweep/wandbX.py` & `dysweep-0.0.7/dysweep/wandbX.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.6/dysweep.egg-info/PKG-INFO` & `dysweep-0.0.7/dysweep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.6
+Version: 0.0.7
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.6/setup.py` & `dysweep-0.0.7/setup.py`

 * *Files identical despite different names*

