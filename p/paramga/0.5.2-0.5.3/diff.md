# Comparing `tmp/paramga-0.5.2.tar.gz` & `tmp/paramga-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paramga-0.5.2.tar", last modified: Mon Mar 20 12:25:11 2023, max compression
+gzip compressed data, was "paramga-0.5.3.tar", last modified: Mon Jun  5 09:54:16 2023, max compression
```

## Comparing `paramga-0.5.2.tar` & `paramga-0.5.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-03-20 12:25:11.635673 paramga-0.5.2/
--rw-rw-r--   0 sam       (1000) sam       (1000)      614 2023-03-20 12:25:11.635673 paramga-0.5.2/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      220 2021-02-15 20:07:22.000000 paramga-0.5.2/README.md
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-03-20 12:25:11.635673 paramga-0.5.2/paramga/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2021-02-09 08:53:28.000000 paramga-0.5.2/paramga/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      679 2023-01-13 16:20:27.000000 paramga-0.5.2/paramga/crossover.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1331 2023-02-03 11:09:39.000000 paramga-0.5.2/paramga/demo.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      130 2021-02-09 08:52:45.000000 paramga-0.5.2/paramga/encoding.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      144 2021-02-10 21:09:14.000000 paramga-0.5.2/paramga/generator.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      791 2023-02-03 13:00:03.000000 paramga-0.5.2/paramga/iteration_state.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-03-20 12:25:11.635673 paramga-0.5.2/paramga/loss_functions/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-02-03 11:00:16.000000 paramga-0.5.2/paramga/loss_functions/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3434 2023-02-03 16:21:55.000000 paramga-0.5.2/paramga/loss_functions/rmse.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      234 2023-02-03 16:26:08.000000 paramga-0.5.2/paramga/loss_functions/rmse_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2770 2023-02-07 14:16:36.000000 paramga-0.5.2/paramga/loss_functions/rsquared.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     5253 2023-02-03 16:25:54.000000 paramga-0.5.2/paramga/loss_functions/rsquared_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6970 2023-02-03 16:25:48.000000 paramga-0.5.2/paramga/loss_functions/testing_utils.py
--rw-rw-r--   0 sam       (1000) sam       (1000)       20 2021-02-09 08:52:13.000000 paramga-0.5.2/paramga/main.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      975 2023-01-13 16:21:06.000000 paramga-0.5.2/paramga/mutation.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2988 2023-01-13 16:20:27.000000 paramga-0.5.2/paramga/plot.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-03-20 12:25:11.635673 paramga-0.5.2/paramga/post_processing/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-02-03 15:08:49.000000 paramga-0.5.2/paramga/post_processing/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1681 2023-03-20 12:20:38.000000 paramga-0.5.2/paramga/post_processing/normalize_outputs.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3577 2023-02-03 16:19:52.000000 paramga-0.5.2/paramga/post_processing/scaling_functions.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      254 2021-02-28 20:32:57.000000 paramga-0.5.2/paramga/random_helpers.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    22372 2023-02-03 16:39:48.000000 paramga-0.5.2/paramga/run.py
--rw-rw-r--   0 sam       (1000) sam       (1000)       17 2023-01-13 16:20:27.000000 paramga-0.5.2/paramga/types.py
--rw-rw-r--   0 sam       (1000) sam       (1000)       41 2023-03-20 12:25:03.000000 paramga-0.5.2/paramga/version.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-03-20 12:25:11.635673 paramga-0.5.2/paramga.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)      614 2023-03-20 12:25:11.000000 paramga-0.5.2/paramga.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      888 2023-03-20 12:25:11.000000 paramga-0.5.2/paramga.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-03-20 12:25:11.000000 paramga-0.5.2/paramga.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-03-20 12:25:11.000000 paramga-0.5.2/paramga.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       14 2023-03-20 12:25:11.000000 paramga-0.5.2/paramga.egg-info/top_level.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)      515 2023-03-20 12:25:11.635673 paramga-0.5.2/setup.cfg
--rw-rw-r--   0 sam       (1000) sam       (1000)     1011 2023-03-20 12:25:03.000000 paramga-0.5.2/setup.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-03-20 12:25:11.635673 paramga-0.5.2/tests/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-01-13 16:20:27.000000 paramga-0.5.2/tests/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      322 2023-02-03 10:51:46.000000 paramga-0.5.2/tests/data_sampling_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1039 2023-01-13 16:20:27.000000 paramga-0.5.2/tests/mutation_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1898 2023-01-13 16:20:27.000000 paramga-0.5.2/tests/objects_test.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    17745 2023-02-03 12:03:03.000000 paramga-0.5.2/tests/run_test.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      614 2023-06-05 09:54:16.228814 paramga-0.5.3/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      220 2021-02-15 20:07:22.000000 paramga-0.5.3/README.md
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.224814 paramga-0.5.3/paramga/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2021-02-09 08:53:28.000000 paramga-0.5.3/paramga/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      679 2023-01-13 16:20:27.000000 paramga-0.5.3/paramga/crossover.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1331 2023-02-03 11:09:39.000000 paramga-0.5.3/paramga/demo.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      130 2021-02-09 08:52:45.000000 paramga-0.5.3/paramga/encoding.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      144 2021-02-10 21:09:14.000000 paramga-0.5.3/paramga/generator.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      791 2023-02-03 13:00:03.000000 paramga-0.5.3/paramga/iteration_state.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/paramga/loss_functions/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-02-03 11:00:16.000000 paramga-0.5.3/paramga/loss_functions/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3434 2023-02-03 16:21:55.000000 paramga-0.5.3/paramga/loss_functions/rmse.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      234 2023-02-03 16:26:08.000000 paramga-0.5.3/paramga/loss_functions/rmse_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2770 2023-02-07 14:16:36.000000 paramga-0.5.3/paramga/loss_functions/rsquared.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     5253 2023-02-03 16:25:54.000000 paramga-0.5.3/paramga/loss_functions/rsquared_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6970 2023-02-03 16:25:48.000000 paramga-0.5.3/paramga/loss_functions/testing_utils.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2021-02-09 08:52:13.000000 paramga-0.5.3/paramga/main.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      975 2023-01-13 16:21:06.000000 paramga-0.5.3/paramga/mutation.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2988 2023-01-13 16:20:27.000000 paramga-0.5.3/paramga/plot.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/paramga/post_processing/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-02-03 15:08:49.000000 paramga-0.5.3/paramga/post_processing/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1681 2023-03-20 12:20:38.000000 paramga-0.5.3/paramga/post_processing/normalize_outputs.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3577 2023-02-03 16:19:52.000000 paramga-0.5.3/paramga/post_processing/scaling_functions.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      254 2021-02-28 20:32:57.000000 paramga-0.5.3/paramga/random_helpers.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    22607 2023-06-05 09:53:29.000000 paramga-0.5.3/paramga/run.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)       17 2023-01-13 16:20:27.000000 paramga-0.5.3/paramga/types.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)       41 2023-06-05 09:54:09.000000 paramga-0.5.3/paramga/version.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/paramga.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      614 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      888 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       14 2023-06-05 09:54:16.000000 paramga-0.5.3/paramga.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)      515 2023-06-05 09:54:16.228814 paramga-0.5.3/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1011 2023-06-05 09:54:09.000000 paramga-0.5.3/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-05 09:54:16.228814 paramga-0.5.3/tests/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-01-13 16:20:27.000000 paramga-0.5.3/tests/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      322 2023-02-03 10:51:46.000000 paramga-0.5.3/tests/data_sampling_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1039 2023-01-13 16:20:27.000000 paramga-0.5.3/tests/mutation_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1898 2023-01-13 16:20:27.000000 paramga-0.5.3/tests/objects_test.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    17745 2023-02-03 12:03:03.000000 paramga-0.5.3/tests/run_test.py
```

### Comparing `paramga-0.5.2/PKG-INFO` & `paramga-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramga
-Version: 0.5.2
+Version: 0.5.3
 Summary: Parameter Regression GA tool
 Author: SBland
 Author-email: sblandcouk@gmail.com
 Keywords: genetic algorithm,optimization,scientific modelling
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paramga-0.5.2/paramga/crossover.py` & `paramga-0.5.3/paramga/crossover.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/demo.py` & `paramga-0.5.3/paramga/demo.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/iteration_state.py` & `paramga-0.5.3/paramga/iteration_state.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/loss_functions/rmse.py` & `paramga-0.5.3/paramga/loss_functions/rmse.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/loss_functions/rsquared.py` & `paramga-0.5.3/paramga/loss_functions/rsquared.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/loss_functions/rsquared_test.py` & `paramga-0.5.3/paramga/loss_functions/rsquared_test.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/loss_functions/testing_utils.py` & `paramga-0.5.3/paramga/loss_functions/testing_utils.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/mutation.py` & `paramga-0.5.3/paramga/mutation.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/plot.py` & `paramga-0.5.3/paramga/plot.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/post_processing/normalize_outputs.py` & `paramga-0.5.3/paramga/post_processing/normalize_outputs.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/post_processing/scaling_functions.py` & `paramga-0.5.3/paramga/post_processing/scaling_functions.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/paramga/run.py` & `paramga-0.5.3/paramga/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,16 @@
         self.tolerance = tolerance
         self.max_iterations = max_iterations
         self.verbose = verbose
         self.parallel = parallel
         self.timeout = timeout
         self.seed = seed
         self.stats = RunStats(None)
+        self.failed = False
+        self.error = None
 
         self.history = []
         self._store_iterations = False
 
         self.logger = Logger(1 if verbose else 0)
 
         self.reset_state()
@@ -562,15 +564,21 @@
         self._store_iterations = v
         return self
 
     def run(self):
         start_time = datetime.now()
         while self.iteration_state.iterations < self.max_iterations \
                 and (self.tolerance is None or self.iteration_state.lowest_loss > self.tolerance):
-            next(self)
+            try:
+                next(self)
+            except Exception as e:
+                self.failed = True
+                self.error = e
+                self.logger.error(e)
+                break
         end_time = datetime.now()
         self.stats = RunStats(end_time - start_time)
         return self
 
     def bootstrap_run(self):
         raise NotImplementedError("Bootstrap runs not implemented")
         # dataset_number = #column with dataset names#.size
```

### Comparing `paramga-0.5.2/paramga.egg-info/PKG-INFO` & `paramga-0.5.3/paramga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramga
-Version: 0.5.2
+Version: 0.5.3
 Summary: Parameter Regression GA tool
 Author: SBland
 Author-email: sblandcouk@gmail.com
 Keywords: genetic algorithm,optimization,scientific modelling
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paramga-0.5.2/paramga.egg-info/SOURCES.txt` & `paramga-0.5.3/paramga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/setup.cfg` & `paramga-0.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/setup.py` & `paramga-0.5.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setuptools.setup(
     name="paramga",
-    version="0.5.2",
+    version="0.5.3",
     author="SBland",
     author_email="sblandcouk@gmail.com",
     description="Parameter Regression GA tool",
     long_description=long_description,
     python_requires='>=3.6',
     setup_requires=[
         'pytest-cov',
```

### Comparing `paramga-0.5.2/tests/mutation_test.py` & `paramga-0.5.3/tests/mutation_test.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/tests/objects_test.py` & `paramga-0.5.3/tests/objects_test.py`

 * *Files identical despite different names*

### Comparing `paramga-0.5.2/tests/run_test.py` & `paramga-0.5.3/tests/run_test.py`

 * *Files identical despite different names*

