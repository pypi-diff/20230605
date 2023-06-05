# Comparing `tmp/data-science-helper-utility-0.0.94.tar.gz` & `tmp/data-science-helper-utility-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-science-helper-utility-0.0.94.tar", last modified: Wed Sep 21 20:53:15 2022, max compression
+gzip compressed data, was "data-science-helper-utility-0.0.99.tar", last modified: Wed Sep 21 21:02:52 2022, max compression
```

## Comparing `data-science-helper-utility-0.0.94.tar` & `data-science-helper-utility-0.0.99.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-09-21 20:53:15.667509 data-science-helper-utility-0.0.94/
--rw-rw-rw-   0        0        0      765 2022-09-21 20:53:15.663516 data-science-helper-utility-0.0.94/PKG-INFO
--rw-rw-rw-   0        0        0       18 2022-09-21 20:53:01.000000 data-science-helper-utility-0.0.94/README.md
-drwxrwxrwx   0        0        0        0 2022-09-21 20:53:15.585362 data-science-helper-utility-0.0.94/data_science_helper/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.94/data_science_helper/__init__.py
--rw-rw-rw-   0        0        0     1107 2022-09-21 17:33:05.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_cache.py
--rw-rw-rw-   0        0        0    33154 2022-09-21 20:06:39.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_classification_model.py
--rw-rw-rw-   0        0        0     1443 2022-09-21 17:32:48.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_clean.py
--rw-rw-rw-   0        0        0    13132 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_clustering.py
--rw-rw-rw-   0        0        0     5475 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_dataframe.py
--rw-rw-rw-   0        0        0     1498 2022-09-21 17:32:52.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_feature_selection.py
--rw-rw-rw-   0        0        0     3916 2022-09-13 19:46:04.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_functions.py
--rw-rw-rw-   0        0        0     1392 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_general.py
--rw-rw-rw-   0        0        0     2546 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_output.py
--rw-rw-rw-   0        0        0     5984 2022-09-21 20:06:39.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_plot.py
--rw-rw-rw-   0        0        0    11271 2022-09-21 17:32:56.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_text_mining.py
--rw-rw-rw-   0        0        0     9877 2022-09-21 17:32:55.000000 data-science-helper-utility-0.0.94/data_science_helper/helper_transformers.py
-drwxrwxrwx   0        0        0        0 2022-09-21 20:53:15.615515 data-science-helper-utility-0.0.94/data_science_helper/model/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.94/data_science_helper/model/__init__.py
--rw-rw-rw-   0        0        0     4834 2022-09-21 17:33:03.000000 data-science-helper-utility-0.0.94/data_science_helper/model/custom_bagging__lgb_model.py
--rw-rw-rw-   0        0        0    13061 2022-09-21 17:33:30.000000 data-science-helper-utility-0.0.94/data_science_helper/model/general.py
--rw-rw-rw-   0        0        0    10851 2022-09-21 17:33:33.000000 data-science-helper-utility-0.0.94/data_science_helper/model/lgb_model.py
--rw-rw-rw-   0        0        0     3943 2022-09-21 17:33:47.000000 data-science-helper-utility-0.0.94/data_science_helper/model/neg_bagging_fraction__lgb_model.py
--rw-rw-rw-   0        0        0    24727 2022-09-21 17:33:49.000000 data-science-helper-utility-0.0.94/data_science_helper/model/optuna.py
--rw-rw-rw-   0        0        0     2225 2022-09-21 17:33:51.000000 data-science-helper-utility-0.0.94/data_science_helper/model/scale_pos_weight__lgb_model.py
-drwxrwxrwx   0        0        0        0 2022-09-21 20:53:15.647518 data-science-helper-utility-0.0.94/data_science_helper_utility.egg-info/
--rw-rw-rw-   0        0        0      765 2022-09-21 20:53:15.000000 data-science-helper-utility-0.0.94/data_science_helper_utility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1229 2022-09-21 20:53:15.000000 data-science-helper-utility-0.0.94/data_science_helper_utility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-21 20:53:15.000000 data-science-helper-utility-0.0.94/data_science_helper_utility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      242 2022-09-21 20:53:15.000000 data-science-helper-utility-0.0.94/data_science_helper_utility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-09-21 20:53:15.000000 data-science-helper-utility-0.0.94/data_science_helper_utility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-21 20:53:15.667509 data-science-helper-utility-0.0.94/setup.cfg
--rw-rw-rw-   0        0        0     4562 2022-09-21 20:53:06.000000 data-science-helper-utility-0.0.94/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-21 20:53:15.659510 data-science-helper-utility-0.0.94/test/
--rw-rw-rw-   0        0        0     2474 2022-09-21 17:33:14.000000 data-science-helper-utility-0.0.94/test/test_classification.py
--rw-rw-rw-   0        0        0     4461 2022-09-21 20:06:39.000000 data-science-helper-utility-0.0.94/test/test_classification_2.py
--rw-rw-rw-   0        0        0      832 2022-09-21 17:33:25.000000 data-science-helper-utility-0.0.94/test/test_import.py
--rw-rw-rw-   0        0        0     4016 2022-09-21 17:33:28.000000 data-science-helper-utility-0.0.94/test/test_optuna.py
--rw-rw-rw-   0        0        0     4619 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.94/test/test_roc.py
+drwxrwxrwx   0        0        0        0 2022-09-21 21:02:52.471952 data-science-helper-utility-0.0.99/
+-rw-rw-rw-   0        0        0      736 2022-09-21 21:02:52.467939 data-science-helper-utility-0.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2022-09-21 21:02:42.000000 data-science-helper-utility-0.0.99/README.md
+drwxrwxrwx   0        0        0        0 2022-09-21 21:02:52.391698 data-science-helper-utility-0.0.99/data_science_helper/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.99/data_science_helper/__init__.py
+-rw-rw-rw-   0        0        0     1107 2022-09-21 17:33:05.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_cache.py
+-rw-rw-rw-   0        0        0    33154 2022-09-21 20:06:39.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_classification_model.py
+-rw-rw-rw-   0        0        0     1443 2022-09-21 17:32:48.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_clean.py
+-rw-rw-rw-   0        0        0    13132 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_clustering.py
+-rw-rw-rw-   0        0        0     5475 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_dataframe.py
+-rw-rw-rw-   0        0        0     1498 2022-09-21 17:32:52.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_feature_selection.py
+-rw-rw-rw-   0        0        0     3916 2022-09-13 19:46:04.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_functions.py
+-rw-rw-rw-   0        0        0     1392 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_general.py
+-rw-rw-rw-   0        0        0     2546 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_output.py
+-rw-rw-rw-   0        0        0     5984 2022-09-21 20:06:39.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_plot.py
+-rw-rw-rw-   0        0        0    11271 2022-09-21 17:32:56.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_text_mining.py
+-rw-rw-rw-   0        0        0     9877 2022-09-21 17:32:55.000000 data-science-helper-utility-0.0.99/data_science_helper/helper_transformers.py
+drwxrwxrwx   0        0        0        0 2022-09-21 21:02:52.411695 data-science-helper-utility-0.0.99/data_science_helper/model/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.99/data_science_helper/model/__init__.py
+-rw-rw-rw-   0        0        0     4834 2022-09-21 17:33:03.000000 data-science-helper-utility-0.0.99/data_science_helper/model/custom_bagging__lgb_model.py
+-rw-rw-rw-   0        0        0    13061 2022-09-21 17:33:30.000000 data-science-helper-utility-0.0.99/data_science_helper/model/general.py
+-rw-rw-rw-   0        0        0    10851 2022-09-21 17:33:33.000000 data-science-helper-utility-0.0.99/data_science_helper/model/lgb_model.py
+-rw-rw-rw-   0        0        0     3943 2022-09-21 17:33:47.000000 data-science-helper-utility-0.0.99/data_science_helper/model/neg_bagging_fraction__lgb_model.py
+-rw-rw-rw-   0        0        0    24727 2022-09-21 17:33:49.000000 data-science-helper-utility-0.0.99/data_science_helper/model/optuna.py
+-rw-rw-rw-   0        0        0     2225 2022-09-21 17:33:51.000000 data-science-helper-utility-0.0.99/data_science_helper/model/scale_pos_weight__lgb_model.py
+drwxrwxrwx   0        0        0        0 2022-09-21 21:02:52.447953 data-science-helper-utility-0.0.99/data_science_helper_utility.egg-info/
+-rw-rw-rw-   0        0        0      736 2022-09-21 21:02:52.000000 data-science-helper-utility-0.0.99/data_science_helper_utility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1229 2022-09-21 21:02:52.000000 data-science-helper-utility-0.0.99/data_science_helper_utility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-21 21:02:52.000000 data-science-helper-utility-0.0.99/data_science_helper_utility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      242 2022-09-21 21:02:52.000000 data-science-helper-utility-0.0.99/data_science_helper_utility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2022-09-21 21:02:52.000000 data-science-helper-utility-0.0.99/data_science_helper_utility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-09-21 21:02:52.471952 data-science-helper-utility-0.0.99/setup.cfg
+-rw-rw-rw-   0        0        0     4562 2022-09-21 21:02:44.000000 data-science-helper-utility-0.0.99/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-21 21:02:52.463945 data-science-helper-utility-0.0.99/test/
+-rw-rw-rw-   0        0        0     2474 2022-09-21 17:33:14.000000 data-science-helper-utility-0.0.99/test/test_classification.py
+-rw-rw-rw-   0        0        0     4461 2022-09-21 20:06:39.000000 data-science-helper-utility-0.0.99/test/test_classification_2.py
+-rw-rw-rw-   0        0        0      832 2022-09-21 17:33:25.000000 data-science-helper-utility-0.0.99/test/test_import.py
+-rw-rw-rw-   0        0        0     4016 2022-09-21 17:33:28.000000 data-science-helper-utility-0.0.99/test/test_optuna.py
+-rw-rw-rw-   0        0        0     4619 2022-09-09 17:44:10.000000 data-science-helper-utility-0.0.99/test/test_roc.py
```

### Comparing `data-science-helper-utility-0.0.94/PKG-INFO` & `data-science-helper-utility-0.0.99/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 Metadata-Version: 1.1
 Name: data-science-helper-utility
-Version: 0.0.94
+Version: 0.0.99
 Summary: data-science-helper de proyectos de analitica avanzada
 Home-page: UNKNOWN
 Author: Analitica Avanzada
 Author-email: analitica.avanzada.talento@gmail.com
 License: NOTFOUND
 Download-URL: https://URL_PAQUETE/data-science-helper-utility/-/archive/master/data-science-helper-utility-master.tar
 Description: 
-        
-        
-        
-        
-        
-        
+        # data-science-helper
         
         
         
 Keywords: data-science-helper-utility,ds-helper,paquete,package
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_cache.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_cache.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_classification_model.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_classification_model.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_clean.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_clean.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_clustering.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_clustering.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_dataframe.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_dataframe.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_feature_selection.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_feature_selection.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_functions.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_functions.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_general.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_general.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_output.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_output.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_plot.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_plot.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_text_mining.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_text_mining.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/helper_transformers.py` & `data-science-helper-utility-0.0.99/data_science_helper/helper_transformers.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/model/custom_bagging__lgb_model.py` & `data-science-helper-utility-0.0.99/data_science_helper/model/custom_bagging__lgb_model.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/model/general.py` & `data-science-helper-utility-0.0.99/data_science_helper/model/general.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/model/lgb_model.py` & `data-science-helper-utility-0.0.99/data_science_helper/model/lgb_model.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/model/neg_bagging_fraction__lgb_model.py` & `data-science-helper-utility-0.0.99/data_science_helper/model/neg_bagging_fraction__lgb_model.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/model/optuna.py` & `data-science-helper-utility-0.0.99/data_science_helper/model/optuna.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper/model/scale_pos_weight__lgb_model.py` & `data-science-helper-utility-0.0.99/data_science_helper/model/scale_pos_weight__lgb_model.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/data_science_helper_utility.egg-info/PKG-INFO` & `data-science-helper-utility-0.0.99/data_science_helper_utility.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 Metadata-Version: 1.1
 Name: data-science-helper-utility
-Version: 0.0.94
+Version: 0.0.99
 Summary: data-science-helper de proyectos de analitica avanzada
 Home-page: UNKNOWN
 Author: Analitica Avanzada
 Author-email: analitica.avanzada.talento@gmail.com
 License: NOTFOUND
 Download-URL: https://URL_PAQUETE/data-science-helper-utility/-/archive/master/data-science-helper-utility-master.tar
 Description: 
-        
-        
-        
-        
-        
-        
+        # data-science-helper
         
         
         
 Keywords: data-science-helper-utility,ds-helper,paquete,package
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `data-science-helper-utility-0.0.94/data_science_helper_utility.egg-info/SOURCES.txt` & `data-science-helper-utility-0.0.99/data_science_helper_utility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/setup.py` & `data-science-helper-utility-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import json
 from os import path
 from setuptools import setup, find_packages
 from sys import version_info
 
 
-VERSION = "0.0.94"
+VERSION = "0.0.99"
 CURR_PATH = "{}{}".format(path.abspath(path.dirname(__file__)), '/')
 
 
 
 def path_format(file_path=None, file_name=None, is_abspath=False,
                 ignore_raises=False):
     """
```

### Comparing `data-science-helper-utility-0.0.94/test/test_classification.py` & `data-science-helper-utility-0.0.99/test/test_classification.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/test/test_classification_2.py` & `data-science-helper-utility-0.0.99/test/test_classification_2.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/test/test_import.py` & `data-science-helper-utility-0.0.99/test/test_import.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/test/test_optuna.py` & `data-science-helper-utility-0.0.99/test/test_optuna.py`

 * *Files identical despite different names*

### Comparing `data-science-helper-utility-0.0.94/test/test_roc.py` & `data-science-helper-utility-0.0.99/test/test_roc.py`

 * *Files identical despite different names*

