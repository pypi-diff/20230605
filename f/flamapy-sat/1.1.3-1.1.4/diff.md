# Comparing `tmp/flamapy-sat-1.1.3.tar.gz` & `tmp/flamapy-sat-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-sat-1.1.3.tar", last modified: Mon Jun  5 14:02:52 2023, max compression
+gzip compressed data, was "flamapy-sat-1.1.4.tar", last modified: Mon Jun  5 14:04:36 2023, max compression
```

## Comparing `flamapy-sat-1.1.3.tar` & `flamapy-sat-1.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.731328 flamapy-sat-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:02:52.731328 flamapy-sat-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/pysat_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.731328 flamapy-sat-1.1.3/flamapy_sat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:02:52.731328 flamapy-sat-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.140648 flamapy-sat-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:04:36.140648 flamapy-sat-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/pysat_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:04:36.136648 flamapy-sat-1.1.4/flamapy_sat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:04:36.000000 flamapy-sat-1.1.4/flamapy_sat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:04:36.140648 flamapy-sat-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 14:04:23.000000 flamapy-sat-1.1.4/setup.py
```

### Comparing `flamapy-sat-1.1.3/PKG-INFO` & `flamapy-sat-1.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-sat
-Version: 1.1.3
+Version: 1.1.4
 Summary: flamapy-sat is a plugin to flamapy module
 Home-page: https://github.com/flamapy/pysat_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/pysat_model.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/pysat_model.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/__init__.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, cast
 
 from pysat.solvers import Solver
 
 from flamapy.core.operations import CoreFeatures
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
+from flamapy.core.models import VariabilityModel
 
 
 class Glucose3CoreFeatures(CoreFeatures):
 
     def __init__(self) -> None:
         self.core_features: list[list[Any]] = []
         self.solver = Solver(name='glucose3')
```

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py` & `flamapy-sat-1.1.4/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/flamapy_sat.egg-info/PKG-INFO` & `flamapy-sat-1.1.4/flamapy_sat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-sat
-Version: 1.1.3
+Version: 1.1.4
 Summary: flamapy-sat is a plugin to flamapy module
 Home-page: https://github.com/flamapy/pysat_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-sat-1.1.3/flamapy_sat.egg-info/SOURCES.txt` & `flamapy-sat-1.1.4/flamapy_sat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.1.3/setup.py` & `flamapy-sat-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-sat",
-    version="1.1.3",
+    version="1.1.4",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="flamapy-sat is a plugin to flamapy module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/pysat_metamodel",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
```

