# Comparing `tmp/tabular_ml-0.0.1.tar.gz` & `tmp/tabular_ml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabular_ml-0.0.1.tar", last modified: Sun Jun  4 05:51:00 2023, max compression
+gzip compressed data, was "tabular_ml-0.0.2.tar", last modified: Mon Jun  5 19:33:23 2023, max compression
```

## Comparing `tabular_ml-0.0.1.tar` & `tabular_ml-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:51:00.267893 tabular_ml-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-04 05:51:00.267893 tabular_ml-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:51:00.263893 tabular_ml-0.0.1/images/
--rw-r--r--   0 runner    (1001) docker     (123)   144245 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/images/readme_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/pypi_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 05:51:00.267893 tabular_ml-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:51:00.263893 tabular_ml-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:51:00.263893 tabular_ml-0.0.1/src/tabular_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:51:00.263893 tabular_ml-0.0.1/src/tabular_ml/ml_models/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/ml_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/ml_models/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/ml_models/lgbm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/ml_models/linear_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/ml_models/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-04 05:50:42.000000 tabular_ml-0.0.1/src/tabular_ml/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:51:00.263893 tabular_ml-0.0.1/src/tabular_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-04 05:51:00.000000 tabular_ml-0.0.1/src/tabular_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-04 05:51:00.000000 tabular_ml-0.0.1/src/tabular_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 05:51:00.000000 tabular_ml-0.0.1/src/tabular_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 05:51:00.000000 tabular_ml-0.0.1/src/tabular_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 05:51:00.000000 tabular_ml-0.0.1/src/tabular_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:23.363161 tabular_ml-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-05 19:33:23.363161 tabular_ml-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:23.355161 tabular_ml-0.0.2/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   144245 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/images/readme_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/pypi_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 19:33:23.363161 tabular_ml-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:23.355161 tabular_ml-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:23.359161 tabular_ml-0.0.2/src/tabular_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:23.359161 tabular_ml-0.0.2/src/tabular_ml/ml_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/ml_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/ml_models/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/ml_models/lgbm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/ml_models/linear_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/ml_models/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-05 19:33:10.000000 tabular_ml-0.0.2/src/tabular_ml/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:23.359161 tabular_ml-0.0.2/src/tabular_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-05 19:33:23.000000 tabular_ml-0.0.2/src/tabular_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-05 19:33:23.000000 tabular_ml-0.0.2/src/tabular_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:33:23.000000 tabular_ml-0.0.2/src/tabular_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 19:33:23.000000 tabular_ml-0.0.2/src/tabular_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 19:33:23.000000 tabular_ml-0.0.2/src/tabular_ml.egg-info/top_level.txt
```

### Comparing `tabular_ml-0.0.1/PKG-INFO` & `tabular_ml-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabular_ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: This library wraps popular tabular regression/classification model enabling rapid evaluation and optimization.
 Author-email: Xavier Nogueira <xavier.rojas.nogueira@gmail.com>
 Keywords: machine-learning,pipeline,factory,tabular,regression,classification
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tabular_ml-0.0.1/images/readme_image.png` & `tabular_ml-0.0.2/images/readme_image.png`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/pypi_readme.md` & `tabular_ml-0.0.2/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/pyproject.toml` & `tabular_ml-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/src/tabular_ml/base.py` & `tabular_ml-0.0.2/src/tabular_ml/base.py`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/src/tabular_ml/factory.py` & `tabular_ml-0.0.2/src/tabular_ml/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,19 +37,39 @@
             )
         if model.model_type not in get_args(ModelTypes):
             raise TypeError(
                 f'Please provide a valid model type! '
                 f'Expected one of {ModelTypes}, got {model.model_type}',
             )
         for func in MLModel.__abstractmethods__:
-            assert hasattr(model, func)
+            if not hasattr(model, func):
+                raise TypeError(
+                    f'Please provide a valid model implementation! '
+                    f'Model is missing {func} method.',
+                )
 
         cls.__registered_models[model.model_type][model.__name__] = model
 
     @classmethod
+    def unregister_model(
+        cls,
+        model_name: str,
+    ) -> None:
+        """Un-registers a model."""
+        if model_name in cls.__registered_models['regression'].keys():
+            del cls.__registered_models['regression'][model_name]
+        elif model_name in cls.__registered_models['classification'].keys():
+            del cls.__registered_models['classification'][model_name]
+        else:
+            raise KeyError(
+                f'{model_name} is not a registered model name! '
+                f'Use ModelFactory.get_all_models() to see registered models.',
+            )
+
+    @classmethod
     def get_all_models(cls) -> Dict[str, List[str]]:
         """Returns all registered models sorted by types."""
         return {
             'regression': list(cls.__registered_models['regression'].keys()),
             'classification': list(cls.__registered_models['classification'].keys()),
         }
```

### Comparing `tabular_ml-0.0.1/src/tabular_ml/functions.py` & `tabular_ml-0.0.2/src/tabular_ml/functions.py`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/src/tabular_ml/ml_models/catboost_model.py` & `tabular_ml-0.0.2/src/tabular_ml/ml_models/catboost_model.py`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/src/tabular_ml/ml_models/lgbm_model.py` & `tabular_ml-0.0.2/src/tabular_ml/ml_models/lgbm_model.py`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/src/tabular_ml/ml_models/linear_models.py` & `tabular_ml-0.0.2/src/tabular_ml/ml_models/linear_models.py`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/src/tabular_ml/ml_models/xgboost_model.py` & `tabular_ml-0.0.2/src/tabular_ml/ml_models/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/src/tabular_ml/utilities.py` & `tabular_ml-0.0.2/src/tabular_ml/utilities.py`

 * *Files identical despite different names*

### Comparing `tabular_ml-0.0.1/src/tabular_ml.egg-info/PKG-INFO` & `tabular_ml-0.0.2/src/tabular_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabular-ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: This library wraps popular tabular regression/classification model enabling rapid evaluation and optimization.
 Author-email: Xavier Nogueira <xavier.rojas.nogueira@gmail.com>
 Keywords: machine-learning,pipeline,factory,tabular,regression,classification
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tabular_ml-0.0.1/src/tabular_ml.egg-info/SOURCES.txt` & `tabular_ml-0.0.2/src/tabular_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

