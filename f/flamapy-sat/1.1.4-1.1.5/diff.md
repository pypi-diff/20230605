# Comparing `tmp/flamapy-sat-1.1.4.tar.gz` & `tmp/flamapy-sat-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-sat-1.1.4.tar", last modified: Mon Jun  5 14:04:36 2023, max compression
+gzip compressed data, was "flamapy-sat-1.1.5.tar", last modified: Mon Jun  5 14:13:37 2023, max compression
```

## Comparing `flamapy-sat-1.1.4.tar` & `flamapy-sat-1.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.140648 flamapy-sat-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:04:36.140648 flamapy-sat-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/pysat_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy_sat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:04:36.140648 flamapy-sat-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:13:37.910485 flamapy-sat-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:13:37.910485 flamapy-sat-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:13:37.902485 flamapy-sat-1.1.5/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:13:37.902485 flamapy-sat-1.1.5/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:13:37.902485 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:13:37.902485 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/models/pysat_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:13:37.910485 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:13:37.910485 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:13:37.910485 flamapy-sat-1.1.5/flamapy_sat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:13:37.000000 flamapy-sat-1.1.5/flamapy_sat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-05 14:13:37.000000 flamapy-sat-1.1.5/flamapy_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 14:13:37.000000 flamapy-sat-1.1.5/flamapy_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 14:13:37.000000 flamapy-sat-1.1.5/flamapy_sat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:13:37.000000 flamapy-sat-1.1.5/flamapy_sat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:13:37.910485 flamapy-sat-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 14:13:22.000000 flamapy-sat-1.1.5/setup.py
```

### Comparing `flamapy-sat-1.1.4/PKG-INFO` & `flamapy-sat-1.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-sat
-Version: 1.1.4
+Version: 1.1.5
 Summary: flamapy-sat is a plugin to flamapy module
 Home-page: https://github.com/flamapy/pysat_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/pysat_model.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/models/pysat_model.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/__init__.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 from flamapy.metamodels.pysat_metamodel.operations.glucose3_false_optional_features import (
     Glucose3FalseOptionalFeatures
 )
 from flamapy.metamodels.pysat_metamodel.operations.glucose3_valid import Glucose3Valid
 from flamapy.metamodels.fm_metamodel.models.feature_model import FeatureModel
 from flamapy.core.models import VariabilityModel
-from flamapy.core.exceptions import FLAMAException
+from flamapy.core.exceptions import FlamaException
 
 
 class Glucose3ErrorDetection(ErrorDetection):
 
     def __init__(self) -> None:
         self.feature_model = None
         self.errors_messages: list[str] = []
@@ -24,15 +24,15 @@
         return self.get_result()
 
     def get_result(self) -> list[str]:
         return self.errors_messages
 
     def execute(self, model: VariabilityModel) -> 'Glucose3ErrorDetection':
         if self.feature_model is None:
-            raise FLAMAException('The feature model is not setted')
+            raise FlamaException('The feature model is not setted')
         
         model=cast(PySATModel, model)
 
         # Valid feature model check
         valid = Glucose3Valid().execute(model).get_result()
         if not valid:
             self.errors_messages.append('The model is not valid (it is void), \
```

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from pysat.solvers import Solver
 
 from flamapy.core.operations import FalseOptionalFeatures
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
 from flamapy.metamodels.fm_metamodel.models.feature_model import FeatureModel
 from flamapy.core.models import VariabilityModel
-from flamapy.core.exceptions import FLAMAException
+from flamapy.core.exceptions import FlamaException
 
 class Glucose3FalseOptionalFeatures(FalseOptionalFeatures):
 
     def __init__(self) -> None:
         self.result: list[Any] = []
         self.feature_model = None
         self.solver = Solver(name='glucose3')
 
     def execute(self, model: VariabilityModel) -> 'Glucose3FalseOptionalFeatures':
         if self.feature_model is None:
-            raise FLAMAException('The feature model is not setted')
+            raise FlamaException('The feature model is not setted')
         
         model=cast(PySATModel, model)
 
         self.result = self._get_false_optional_features(model, self.feature_model)
         return self
 
     def get_false_optional_features(self) -> list[list[Any]]:
```

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py` & `flamapy-sat-1.1.5/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/flamapy_sat.egg-info/PKG-INFO` & `flamapy-sat-1.1.5/flamapy_sat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-sat
-Version: 1.1.4
+Version: 1.1.5
 Summary: flamapy-sat is a plugin to flamapy module
 Home-page: https://github.com/flamapy/pysat_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-sat-1.1.4/flamapy_sat.egg-info/SOURCES.txt` & `flamapy-sat-1.1.5/flamapy_sat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.4/setup.py` & `flamapy-sat-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-sat",
-    version="1.1.4",
+    version="1.1.5",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="flamapy-sat is a plugin to flamapy module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/pysat_metamodel",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
```

