# Comparing `tmp/paramga-0.5.3.tar.gz` & `tmp/paramga-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paramga-0.5.3.tar", last modified: Mon Jun  5 09:54:16 2023, max compression
+gzip compressed data, was "paramga-0.5.4.tar", last modified: Mon Jun  5 10:26:04 2023, max compression
```

## Comparing `paramga-0.5.3.tar` & `paramga-0.5.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/
--rw-rw-r--   0 sam       (1000) sam       (1000)      614 2023-06-05 09:54:16.228814 paramga-0.5.3/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      220 2021-02-15 20:07:22.000000 paramga-0.5.3/README.md
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.224814 paramga-0.5.3/paramga/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2021-02-09 08:53:28.000000 paramga-0.5.3/paramga/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      679 2023-01-13 16:20:27.000000 paramga-0.5.3/paramga/crossover.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1331 2023-02-03 11:09:39.000000 paramga-0.5.3/paramga/demo.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      130 2021-02-09 08:52:45.000000 paramga-0.5.3/paramga/encoding.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      144 2021-02-10 21:09:14.000000 paramga-0.5.3/paramga/generator.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      791 2023-02-03 13:00:03.000000 paramga-0.5.3/paramga/iteration_state.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/paramga/loss_functions/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-02-03 11:00:16.000000 paramga-0.5.3/paramga/loss_functions/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3434 2023-02-03 16:21:55.000000 paramga-0.5.3/paramga/loss_functions/rmse.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      234 2023-02-03 16:26:08.000000 paramga-0.5.3/paramga/loss_functions/rmse_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2770 2023-02-07 14:16:36.000000 paramga-0.5.3/paramga/loss_functions/rsquared.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     5253 2023-02-03 16:25:54.000000 paramga-0.5.3/paramga/loss_functions/rsquared_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6970 2023-02-03 16:25:48.000000 paramga-0.5.3/paramga/loss_functions/testing_utils.py
--rw-rw-r--   0 sam       (1000) sam       (1000)       20 2021-02-09 08:52:13.000000 paramga-0.5.3/paramga/main.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      975 2023-01-13 16:21:06.000000 paramga-0.5.3/paramga/mutation.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2988 2023-01-13 16:20:27.000000 paramga-0.5.3/paramga/plot.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/paramga/post_processing/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-02-03 15:08:49.000000 paramga-0.5.3/paramga/post_processing/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1681 2023-03-20 12:20:38.000000 paramga-0.5.3/paramga/post_processing/normalize_outputs.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3577 2023-02-03 16:19:52.000000 paramga-0.5.3/paramga/post_processing/scaling_functions.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      254 2021-02-28 20:32:57.000000 paramga-0.5.3/paramga/random_helpers.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    22607 2023-06-05 09:53:29.000000 paramga-0.5.3/paramga/run.py
--rw-rw-r--   0 sam       (1000) sam       (1000)       17 2023-01-13 16:20:27.000000 paramga-0.5.3/paramga/types.py
--rw-rw-r--   0 sam       (1000) sam       (1000)       41 2023-06-05 09:54:09.000000 paramga-0.5.3/paramga/version.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/paramga.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)      614 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      888 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       14 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/top_level.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)      515 2023-06-05 09:54:16.228814 paramga-0.5.3/setup.cfg
--rw-rw-r--   0 sam       (1000) sam       (1000)     1011 2023-06-05 09:54:09.000000 paramga-0.5.3/setup.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/tests/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-01-13 16:20:27.000000 paramga-0.5.3/tests/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      322 2023-02-03 10:51:46.000000 paramga-0.5.3/tests/data_sampling_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1039 2023-01-13 16:20:27.000000 paramga-0.5.3/tests/mutation_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1898 2023-01-13 16:20:27.000000 paramga-0.5.3/tests/objects_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    17745 2023-02-03 12:03:03.000000 paramga-0.5.3/tests/run_test.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 10:26:04.363322 paramga-0.5.4/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      614 2023-06-05 10:26:04.363322 paramga-0.5.4/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      220 2021-02-15 20:07:22.000000 paramga-0.5.4/README.md
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 10:26:04.359322 paramga-0.5.4/paramga/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2021-02-09 08:53:28.000000 paramga-0.5.4/paramga/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      679 2023-01-13 16:20:27.000000 paramga-0.5.4/paramga/crossover.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1331 2023-02-03 11:09:39.000000 paramga-0.5.4/paramga/demo.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      130 2021-02-09 08:52:45.000000 paramga-0.5.4/paramga/encoding.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      144 2021-02-10 21:09:14.000000 paramga-0.5.4/paramga/generator.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      791 2023-02-03 13:00:03.000000 paramga-0.5.4/paramga/iteration_state.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 10:26:04.363322 paramga-0.5.4/paramga/loss_functions/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-02-03 11:00:16.000000 paramga-0.5.4/paramga/loss_functions/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3434 2023-02-03 16:21:55.000000 paramga-0.5.4/paramga/loss_functions/rmse.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      234 2023-02-03 16:26:08.000000 paramga-0.5.4/paramga/loss_functions/rmse_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2770 2023-02-07 14:16:36.000000 paramga-0.5.4/paramga/loss_functions/rsquared.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     5253 2023-02-03 16:25:54.000000 paramga-0.5.4/paramga/loss_functions/rsquared_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6970 2023-02-03 16:25:48.000000 paramga-0.5.4/paramga/loss_functions/testing_utils.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2021-02-09 08:52:13.000000 paramga-0.5.4/paramga/main.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      975 2023-01-13 16:21:06.000000 paramga-0.5.4/paramga/mutation.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2988 2023-01-13 16:20:27.000000 paramga-0.5.4/paramga/plot.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 10:26:04.363322 paramga-0.5.4/paramga/post_processing/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-02-03 15:08:49.000000 paramga-0.5.4/paramga/post_processing/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1681 2023-03-20 12:20:38.000000 paramga-0.5.4/paramga/post_processing/normalize_outputs.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3577 2023-02-03 16:19:52.000000 paramga-0.5.4/paramga/post_processing/scaling_functions.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      254 2021-02-28 20:32:57.000000 paramga-0.5.4/paramga/random_helpers.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    22607 2023-06-05 10:25:57.000000 paramga-0.5.4/paramga/run.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)       17 2023-01-13 16:20:27.000000 paramga-0.5.4/paramga/types.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)       41 2023-06-05 10:25:57.000000 paramga-0.5.4/paramga/version.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 10:26:04.363322 paramga-0.5.4/paramga.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      614 2023-06-05 10:26:04.000000 paramga-0.5.4/paramga.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      888 2023-06-05 10:26:04.000000 paramga-0.5.4/paramga.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-06-05 10:26:04.000000 paramga-0.5.4/paramga.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-06-05 10:26:04.000000 paramga-0.5.4/paramga.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       14 2023-06-05 10:26:04.000000 paramga-0.5.4/paramga.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)      515 2023-06-05 10:26:04.363322 paramga-0.5.4/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1011 2023-06-05 10:25:57.000000 paramga-0.5.4/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 10:26:04.363322 paramga-0.5.4/tests/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-01-13 16:20:27.000000 paramga-0.5.4/tests/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      322 2023-02-03 10:51:46.000000 paramga-0.5.4/tests/data_sampling_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1039 2023-01-13 16:20:27.000000 paramga-0.5.4/tests/mutation_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1898 2023-01-13 16:20:27.000000 paramga-0.5.4/tests/objects_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    17745 2023-02-03 12:03:03.000000 paramga-0.5.4/tests/run_test.py
```

### Comparing `paramga-0.5.3/PKG-INFO` & `paramga-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramga
-Version: 0.5.3
+Version: 0.5.4
 Summary: Parameter Regression GA tool
 Author: SBland
 Author-email: sblandcouk@gmail.com
 Keywords: genetic algorithm,optimization,scientific modelling
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paramga-0.5.3/paramga/crossover.py` & `paramga-0.5.4/paramga/crossover.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/demo.py` & `paramga-0.5.4/paramga/demo.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/iteration_state.py` & `paramga-0.5.4/paramga/iteration_state.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/loss_functions/rmse.py` & `paramga-0.5.4/paramga/loss_functions/rmse.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/loss_functions/rsquared.py` & `paramga-0.5.4/paramga/loss_functions/rsquared.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/loss_functions/rsquared_test.py` & `paramga-0.5.4/paramga/loss_functions/rsquared_test.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/loss_functions/testing_utils.py` & `paramga-0.5.4/paramga/loss_functions/testing_utils.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/mutation.py` & `paramga-0.5.4/paramga/mutation.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/plot.py` & `paramga-0.5.4/paramga/plot.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/post_processing/normalize_outputs.py` & `paramga-0.5.4/paramga/post_processing/normalize_outputs.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/post_processing/scaling_functions.py` & `paramga-0.5.4/paramga/post_processing/scaling_functions.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga/run.py` & `paramga-0.5.4/paramga/run.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/paramga.egg-info/PKG-INFO` & `paramga-0.5.4/paramga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramga
-Version: 0.5.3
+Version: 0.5.4
 Summary: Parameter Regression GA tool
 Author: SBland
 Author-email: sblandcouk@gmail.com
 Keywords: genetic algorithm,optimization,scientific modelling
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paramga-0.5.3/paramga.egg-info/SOURCES.txt` & `paramga-0.5.4/paramga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/setup.cfg` & `paramga-0.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/setup.py` & `paramga-0.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setuptools.setup(
     name="paramga",
-    version="0.5.3",
+    version="0.5.4",
     author="SBland",
     author_email="sblandcouk@gmail.com",
     description="Parameter Regression GA tool",
     long_description=long_description,
     python_requires='>=3.6',
     setup_requires=[
         'pytest-cov',
```

### Comparing `paramga-0.5.3/tests/mutation_test.py` & `paramga-0.5.4/tests/mutation_test.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/tests/objects_test.py` & `paramga-0.5.4/tests/objects_test.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.3/tests/run_test.py` & `paramga-0.5.4/tests/run_test.py`

 * *Files identical despite different names*

