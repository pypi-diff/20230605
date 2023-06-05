# Comparing `tmp/flamapy-sat-1.0.1.dev0.tar.gz` & `tmp/flamapy-sat-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-sat-1.0.1.dev0.tar", last modified: Sat Aug 13 16:59:32 2022, max compression
+gzip compressed data, was "flamapy-sat-1.1.3.tar", last modified: Mon Jun  5 14:02:52 2023, max compression
```

## Comparing `flamapy-sat-1.0.1.dev0.tar` & `flamapy-sat-1.1.3.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:32.322892 flamapy-sat-1.0.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-08-13 16:59:32.322892 flamapy-sat-1.0.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:32.318892 flamapy-sat-1.0.1.dev0/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:32.318892 flamapy-sat-1.0.1.dev0/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:32.318892 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:32.318892 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/models/pysat_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8825 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:32.318892 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:32.318892 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5759 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
--rw-r--r--   0 runner    (1001) docker     (121)     7277 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:32.322892 flamapy-sat-1.0.1.dev0/flamapy_sat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-08-13 16:59:32.000000 flamapy-sat-1.0.1.dev0/flamapy_sat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-08-13 16:59:32.000000 flamapy-sat-1.0.1.dev0/flamapy_sat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-13 16:59:32.000000 flamapy-sat-1.0.1.dev0/flamapy_sat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-08-13 16:59:32.000000 flamapy-sat-1.0.1.dev0/flamapy_sat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-13 16:59:32.000000 flamapy-sat-1.0.1.dev0/flamapy_sat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-13 16:59:32.322892 flamapy-sat-1.0.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-08-13 16:59:23.000000 flamapy-sat-1.0.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.731328 flamapy-sat-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:02:52.731328 flamapy-sat-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/pysat_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.727328 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:02:52.731328 flamapy-sat-1.1.3/flamapy_sat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:02:52.000000 flamapy-sat-1.1.3/flamapy_sat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:02:52.731328 flamapy-sat-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 14:02:35.000000 flamapy-sat-1.1.3/setup.py
```

### Comparing `flamapy-sat-1.0.1.dev0/PKG-INFO` & `flamapy-sat-1.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-sat
-Version: 1.0.1.dev0
+Version: 1.1.3
 Summary: flamapy-sat is a plugin to flamapy module
 Home-page: https://github.com/flamapy/pysat_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/models/pysat_model.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/pysat_model.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 from enum import Enum, auto
+from flamapy.core.exceptions import FlamaException
 
 
 class CNFLogicConnective(Enum):
     """The propositional logic connectives a formula in CNF can contain."""
     NOT = auto()
     AND = auto()
     OR = auto()
@@ -75,26 +76,26 @@
         cnf_formula = self.get_textual_cnf_formula(syntax)
         with open(filepath, 'w+', encoding='utf-8') as file:
             file.write(cnf_formula)
 
     def get_textual_cnf_notation(self) -> TextCNFNotation:
         """Return the notation used for the CNF formula."""
         if self._cnf_formula is None:
-            raise Exception("CNF Model not initialized. Use a `from_` method first.")
+            raise FlamaException("CNF Model not initialized. Use a `from_` method first.")
         assert self._cnf_notation is not None
         return self._cnf_notation
 
     def get_textual_cnf_formula(self,
                                 syntax: Optional[TextCNFNotation] = None) -> str:
         """Return the CNF formula in the specified notation syntax.
 
         Default syntax is TextCNFNotation.JAVA_SHORT: (A) & (!B | C) && ...
         """
         if self._cnf_formula is None:
-            raise Exception("CNF Model not initialized. Use a `from_` method first.")
+            raise FlamaException("CNF Model not initialized. Use a `from_` method first.")
         assert self._cnf_notation is not None
 
         cnf_formula = self._cnf_formula
         cnf_notation = self._cnf_notation
 
         if syntax is not None and syntax == cnf_notation:
             return cnf_formula
@@ -134,15 +135,15 @@
             new_symbol = '(' + syntax.value[CNFLogicConnective.NOT]
             cnf_formula = cnf_formula.replace(symbol_pattern, new_symbol)
         return cnf_formula
 
     def get_variables(self) -> list[str]:
         """Return the list of variables' names in the CNF formula."""
         if self._cnf_formula is None:
-            raise Exception("CNF Model not initialized. Use a `from_` method first.")
+            raise FlamaException("CNF Model not initialized. Use a `from_` method first.")
         return self._variables
 
 
 def identify_notation(cnf_formula: str) -> TextCNFNotation:
     """Return the notation used by the given CNF formula.
 
     Default TextCNFNotation.JAVA.
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/__init__.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_commonality.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_core_features.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from typing import Any
+from typing import Any, cast
 
-from pysat.solvers import Glucose3
+from pysat.solvers import Solver
 
 from flamapy.core.operations import CoreFeatures
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
 
 
 class Glucose3CoreFeatures(CoreFeatures):
 
     def __init__(self) -> None:
         self.core_features: list[list[Any]] = []
+        self.solver = Solver(name='glucose3')
 
     def get_core_features(self) -> list[list[Any]]:
         return self.core_features
 
     def get_result(self) -> list[list[Any]]:
         return self.get_core_features()
 
-    def execute(self, model: PySATModel) -> 'Glucose3CoreFeatures':
-        glucose = Glucose3()
+    def execute(self, model: VariabilityModel) -> 'Glucose3CoreFeatures':
+        model=cast(PySATModel, model)
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
-            glucose.add_clause(clause)  # añadimos la constraint
+            self.solver.add_clause(clause)  # añadimos la constraint
 
         core_features = []
-        if glucose.solve():
+        if self.solver.solve():
             for variable in model.variables.items():
-                if not glucose.solve(assumptions=[-variable[1]]):
+                if not self.solver.solve(assumptions=[-variable[1]]):
                     core_features.append(variable[0])
 
         self.core_features = core_features
-        glucose.delete()
+        self.solver.delete()
         return self
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_dead_features.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from typing import Any
+from typing import Any,cast
 
-from pysat.solvers import Glucose3
+from pysat.solvers import Solver
 
 from flamapy.core.operations import DeadFeatures
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
+from flamapy.core.models import VariabilityModel
 
 
 class Glucose3DeadFeatures(DeadFeatures):
 
     def __init__(self) -> None:
         self.dead_features: list[list[Any]] = []
+        self.solver = Solver(name='glucose3')
 
     def get_dead_features(self) -> list[list[Any]]:
         return self.dead_features
 
     def get_result(self) -> list[list[Any]]:
         return self.get_dead_features()
 
-    def execute(self, model: PySATModel) -> 'Glucose3DeadFeatures':
-        glucose = Glucose3()
+    def execute(self, model: VariabilityModel) -> 'Glucose3DeadFeatures':
+        model=cast(PySATModel, model)
 
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
-            glucose.add_clause(clause)  # añadimos la constraint
+            self.solver.add_clause(clause)  # añadimos la constraint
 
         dead_features = []
         for variable in model.variables.items():
-            if not glucose.solve(assumptions=[variable[1]]):
+            if not self.solver.solve(assumptions=[variable[1]]):
                 dead_features.append(variable[0])
         self.dead_features = dead_features
-        glucose.delete()
+        self.solver.delete()
         return self
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_error_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,41 @@
-#from pysat.solvers import Glucose3
+from typing import cast
 
 from flamapy.core.operations import ErrorDetection
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
 from flamapy.metamodels.pysat_metamodel.operations.glucose3_dead_features import (
     Glucose3DeadFeatures
 )
 from flamapy.metamodels.pysat_metamodel.operations.glucose3_false_optional_features import (
     Glucose3FalseOptionalFeatures
 )
 from flamapy.metamodels.pysat_metamodel.operations.glucose3_valid import Glucose3Valid
 from flamapy.metamodels.fm_metamodel.models.feature_model import FeatureModel
+from flamapy.core.models import VariabilityModel
+from flamapy.core.exceptions import FLAMAException
 
 
 class Glucose3ErrorDetection(ErrorDetection):
 
-    def __init__(self, feature_model: FeatureModel) -> None:
-        self.feature_model = feature_model
+    def __init__(self) -> None:
+        self.feature_model = None
         self.errors_messages: list[str] = []
 
     def get_errors_messages(self) -> list[str]:
         return self.get_result()
 
     def get_result(self) -> list[str]:
         return self.errors_messages
 
-    def execute(self, model: PySATModel) -> 'Glucose3ErrorDetection':
+    def execute(self, model: VariabilityModel) -> 'Glucose3ErrorDetection':
+        if self.feature_model is None:
+            raise FLAMAException('The feature model is not setted')
+        
+        model=cast(PySATModel, model)
+
         # Valid feature model check
         valid = Glucose3Valid().execute(model).get_result()
         if not valid:
             self.errors_messages.append('The model is not valid (it is void), \
                                         so it has not any product.')
 
         # Dead features detection
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_false_optional_features.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,50 @@
-from typing import Any
+from typing import Any,cast
 
-from pysat.solvers import Glucose3
+from pysat.solvers import Solver
 
 from flamapy.core.operations import FalseOptionalFeatures
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
 from flamapy.metamodels.fm_metamodel.models.feature_model import FeatureModel
-
+from flamapy.core.models import VariabilityModel
+from flamapy.core.exceptions import FLAMAException
 
 class Glucose3FalseOptionalFeatures(FalseOptionalFeatures):
 
-    def __init__(self, feature_model: FeatureModel) -> None:
+    def __init__(self) -> None:
         self.result: list[Any] = []
-        self.feature_model = feature_model
+        self.feature_model = None
+        self.solver = Solver(name='glucose3')
+
+    def execute(self, model: VariabilityModel) -> 'Glucose3FalseOptionalFeatures':
+        if self.feature_model is None:
+            raise FLAMAException('The feature model is not setted')
+        
+        model=cast(PySATModel, model)
 
-    def execute(self, model: PySATModel) -> 'Glucose3FalseOptionalFeatures':
-        self.result = get_false_optional_features(model, self.feature_model)
+        self.result = self._get_false_optional_features(model, self.feature_model)
         return self
 
     def get_false_optional_features(self) -> list[list[Any]]:
         return self.get_result()
 
     def get_result(self) -> list[Any]:
         return self.result
 
-
-def get_false_optional_features(sat_model: PySATModel, feature_model: FeatureModel) -> list[Any]:
-    real_optional_features = [f for f in feature_model.get_features() 
-                              if not f.is_root() and not f.is_mandatory()]
-
-    result = []
-    solver = Glucose3()
-    for clause in sat_model.get_all_clauses():
-        solver.add_clause(clause)
-
-    for feature in real_optional_features:
-        variable = sat_model.variables.get(feature.name)
-        parent_variable = sat_model.variables.get(feature.get_parent().name)
-        assert variable is not None
-        satisfiable = solver.solve(assumptions=[parent_variable, -variable])
-        if not satisfiable:
-            result.append(feature.name)
-    solver.delete()
-    return result
+    def _get_false_optional_features(self, sat_model: PySATModel, 
+                                     feature_model: FeatureModel) -> list[Any]:
+        real_optional_features = [f for f in feature_model.get_features() 
+                                  if not f.is_root() and not f.is_mandatory()]
+
+        result = []
+        for clause in sat_model.get_all_clauses():
+            self.solver.add_clause(clause)
+
+        for feature in real_optional_features:
+            variable = sat_model.variables.get(feature.name)
+            parent_variable = sat_model.variables.get(feature.get_parent().name)
+            assert variable is not None
+            satisfiable = self.solver.solve(assumptions=[parent_variable, -variable])
+            if not satisfiable:
+                result.append(feature.name)
+        self.solver.delete()
+        return result
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-from typing import Any
+from typing import Any, cast
 
-from pysat.solvers import Glucose3
+from pysat.solvers import Solver
 
 from flamapy.metamodels.configuration_metamodel.models.configuration import Configuration
 from flamapy.core.operations import Filter
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
+from flamapy.core.models import VariabilityModel
 
 
 class Glucose3Filter(Filter):
 
     def __init__(self) -> None:
         self.filter_products: list[list[Any]] = []
         self.configuration = Configuration({})
+        self.solver = Solver(name='glucose3')
 
     def get_filter_products(self) -> list[list[Any]]:
         return self.filter_products
 
     def get_result(self) -> list[list[Any]]:
         return self.get_filter_products()
 
     def set_configuration(self, configuration: Configuration) -> None:
         self.configuration = configuration
 
-    def execute(self, model: PySATModel) -> 'Glucose3Filter':
-        glucose = Glucose3()
+    def execute(self, model: VariabilityModel) -> 'Glucose3Filter':
+        model=cast(PySATModel, model)
+
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
-            glucose.add_clause(clause)  # añadimos la constraint
+            self.solver.add_clause(clause)  # añadimos la constraint
 
         assumptions = [
             model.variables.get(feat[0].name) if feat[1]
             else -model.variables.get(feat[0].name)
             for feat in self.configuration.elements.items()
         ]
 
-        for solution in glucose.enum_models(assumptions=assumptions):
+        for solution in self.solver.enum_models(assumptions=assumptions):
             product = []
             for variable in solution:
                 if variable > 0:
                     product.append(model.features.get(variable))
             self.filter_products.append(product)
-        glucose.delete()
+        self.solver.delete()
         return self
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from pysat.solvers import Glucose3
+from typing import cast
+
+from pysat.solvers import Solver
 
 from flamapy.core.operations import ProductsNumber
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
+from flamapy.core.models import VariabilityModel
 
 
 class Glucose3ProductsNumber(ProductsNumber):
 
     def __init__(self) -> None:
         self.products_number = 0
+        self.solver = Solver(name='glucose3')
 
     def get_products_number(self) -> int:
         return self.products_number
 
     def get_result(self) -> int:
         return self.get_products_number()
 
-    def execute(self, model: PySATModel) -> 'Glucose3ProductsNumber':
-        glucose = Glucose3()
+    def execute(self, model: VariabilityModel) -> 'Glucose3ProductsNumber':
+        model=cast(PySATModel, model)
+
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
-            glucose.add_clause(clause)  # añadimos la constraint
+            self.solver.add_clause(clause)  # añadimos la constraint
 
-        for _ in glucose.enum_models():
+        for _ in self.solver.enum_models():
             self.products_number += 1
-        glucose.delete()
+        self.solver.delete()
         return self
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-from pysat.solvers import Glucose3
+from typing import cast
+
+from pysat.solvers import Solver
 
 from flamapy.core.operations import Valid
 
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
+from flamapy.core.models import VariabilityModel
 
 
 class Glucose3Valid(Valid):
 
     def __init__(self) -> None:
         self.result = False
+        self.solver = Solver(name='glucose3')
 
     def is_valid(self) -> bool:
         return self.result
 
     def get_result(self) -> bool:
         return self.is_valid()
 
-    def execute(self, model: PySATModel) -> 'Glucose3Valid':
-        glucose = Glucose3()
+    def execute(self, model: VariabilityModel) -> 'Glucose3Valid':
+        model=cast(PySATModel, model)
+
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
-            glucose.add_clause(clause)  # añadimos la constraint
-        self.result = glucose.solve()
-        glucose.delete()
-        return self
+            self.solver.add_clause(clause)  # añadimos la constraint
+        self.result = self.solver.solve()
+        self.solver.delete()
+        return self
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,53 @@
-from pysat.solvers import Glucose3
+from typing import cast
 
-from flamapy.core.operations import ValidConfiguration
-from flamapy.metamodels.configuration_metamodel.models.configuration import Configuration
+from pysat.solvers import Solver
 
+from flamapy.core.operations import ValidProduct
+from flamapy.metamodels.configuration_metamodel.models.configuration import Configuration
 
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
+from flamapy.core.models import VariabilityModel
 
 
-class Glucose3ValidConfiguration(ValidConfiguration):
+class Glucose3ValidProduct(ValidProduct):
 
     def __init__(self) -> None:
         self.result = False
         self.configuration = Configuration({})
+        self.solver = Solver(name='glucose3')
 
     def is_valid(self) -> bool:
         return self.result
 
     def get_result(self) -> bool:
         return self.is_valid()
 
     def set_configuration(self, configuration: Configuration) -> None:
         self.configuration = configuration
 
-    def execute(self, model: PySATModel) -> 'Glucose3ValidConfiguration':
-        glucose = Glucose3()
+    def execute(self, model: VariabilityModel) -> 'Glucose3ValidProduct':
+        model=cast(PySATModel, model)
 
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
-            glucose.add_clause(clause)  # añadimos la constraint
+            self.solver.add_clause(clause)  # añadimos la constraint
 
         assumptions = []
-        for feat in self.configuration.elements.items():
-            if feat[1]:
-                assumptions.append(model.variables[feat[0].name])
-            elif not feat[1]:
-                assumptions.append(-model.variables[feat[0].name])
 
-        self.result = glucose.solve(assumptions=assumptions)
-        glucose.delete()
+        config: list[str] = []
+        if self.configuration is not None:
+            config = [feat.name for feat in self.configuration.elements]
+
+        for feat in config:
+            if feat not in model.variables.keys():
+                self.result = False
+                return self
+
+        for feat in model.features.values():
+            if feat in config:
+                assumptions.append(model.variables[feat])
+            else:
+                assumptions.append(-model.variables[feat])
+
+        self.result = self.solver.solve(assumptions=assumptions)
+        self.solver.delete()
         return self
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.0.1.dev0/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py` & `flamapy-sat-1.1.3/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.0.1.dev0/flamapy_sat.egg-info/PKG-INFO` & `flamapy-sat-1.1.3/flamapy_sat.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-sat
-Version: 1.0.1.dev0
+Version: 1.1.3
 Summary: flamapy-sat is a plugin to flamapy module
 Home-page: https://github.com/flamapy/pysat_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-sat-1.0.1.dev0/flamapy_sat.egg-info/SOURCES.txt` & `flamapy-sat-1.1.3/flamapy_sat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,13 +14,15 @@
 flamapy/metamodels/pysat_metamodel/operations/glucose3_products.py
 flamapy/metamodels/pysat_metamodel/operations/glucose3_products_number.py
 flamapy/metamodels/pysat_metamodel/operations/glucose3_valid.py
 flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_configuration.py
 flamapy/metamodels/pysat_metamodel/operations/glucose3_valid_product.py
 flamapy/metamodels/pysat_metamodel/transformations/__init__.py
 flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
+flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py
+flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py
 flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
 flamapy_sat.egg-info/PKG-INFO
 flamapy_sat.egg-info/SOURCES.txt
 flamapy_sat.egg-info/dependency_links.txt
 flamapy_sat.egg-info/requires.txt
 flamapy_sat.egg-info/top_level.txt
```

### Comparing `flamapy-sat-1.0.1.dev0/setup.py` & `flamapy-sat-1.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-sat",
-    version="1.0.1.dev0",
+    version="1.1.3",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="flamapy-sat is a plugin to flamapy module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/pysat_metamodel",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
     install_requires=[
-        'flamapy~=1.0.1.dev0',
-        'flamapy-fm~=1.0.1.dev0',
+        'flamapy~=1.1.3',
+        'flamapy-fm~=1.1.3',
         'python-sat>=0.1.7.dev6'
     ],
     extras_require={
         'dev': [
             'pytest',
             'pytest-mock',
             'prospector',
             'mypy',
             'coverage',
         ]
     },
     dependency_links=[
-        'flamapy~=1.0.1.dev0'
+        'flamapy~=1.1.3'
     ]
 )
```

