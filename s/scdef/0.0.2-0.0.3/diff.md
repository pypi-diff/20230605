# Comparing `tmp/scdef-0.0.2.tar.gz` & `tmp/scdef-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdef-0.0.2.tar", max compression
+gzip compressed data, was "scdef-0.0.3.tar", max compression
```

## Comparing `scdef-0.0.2.tar` & `scdef-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      983 2023-06-04 23:53:18.027853 scdef-0.0.2/README.md
--rw-r--r--   0        0        0      641 2023-06-05 00:08:18.411482 scdef-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       68 2023-06-04 22:36:21.759434 scdef-0.0.2/scdef/__init__.py
--rw-r--r--   0        0        0    10950 2023-06-04 23:23:33.986978 scdef-0.0.2/scdef/bscdef.py
--rw-r--r--   0        0        0     7953 2023-06-04 23:24:28.116267 scdef-0.0.2/scdef/iscdef.py
--rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.2/scdef/main.py
--rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.2/scdef/models/integrated.py
--rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.2/scdef/models/joint.py
--rw-r--r--   0        0        0       21 2023-06-04 23:23:30.271994 scdef-0.0.2/scdef/models/single.py
--rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.2/scdef/models/spatial.py
--rw-r--r--   0        0        0    50501 2023-06-05 00:03:59.456164 scdef-0.0.2/scdef/scdef.py
--rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.2/scdef/util.py
--rw-r--r--   0        0        0     2053 1970-01-01 00:00:00.000000 scdef-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      983 2023-06-04 23:53:18.027853 scdef-0.0.3/README.md
+-rw-r--r--   0        0        0      641 2023-06-05 00:51:08.825806 scdef-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-06-04 22:36:21.759434 scdef-0.0.3/scdef/__init__.py
+-rw-r--r--   0        0        0    10950 2023-06-04 23:23:33.986978 scdef-0.0.3/scdef/bscdef.py
+-rw-r--r--   0        0        0     7953 2023-06-04 23:24:28.116267 scdef-0.0.3/scdef/iscdef.py
+-rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.3/scdef/main.py
+-rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.3/scdef/models/integrated.py
+-rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.3/scdef/models/joint.py
+-rw-r--r--   0        0        0       21 2023-06-04 23:23:30.271994 scdef-0.0.3/scdef/models/single.py
+-rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.3/scdef/models/spatial.py
+-rw-r--r--   0        0        0    50604 2023-06-05 00:50:35.777620 scdef-0.0.3/scdef/scdef.py
+-rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.3/scdef/util.py
+-rw-r--r--   0        0        0     2053 1970-01-01 00:00:00.000000 scdef-0.0.3/PKG-INFO
```

### Comparing `scdef-0.0.2/README.md` & `scdef-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `scdef-0.0.2/pyproject.toml` & `scdef-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scdef"
-version = "0.0.2"
+version = "0.0.3"
 description = "Extract hierarchical signatures of cell state from single-cell data."
 license = "MIT"
 authors = ["pedrofale <pedro.miguel.ferreira.pf@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/cbg-ethz/scdef"
 
 [tool.poetry.dependencies]
```

### Comparing `scdef-0.0.2/scdef/bscdef.py` & `scdef-0.0.3/scdef/bscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.2/scdef/iscdef.py` & `scdef-0.0.3/scdef/iscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.2/scdef/main.py` & `scdef-0.0.3/scdef/main.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.2/scdef/models/integrated.py` & `scdef-0.0.3/scdef/models/integrated.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.2/scdef/models/joint.py` & `scdef-0.0.3/scdef/models/joint.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.2/scdef/models/spatial.py` & `scdef-0.0.3/scdef/models/spatial.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.2/scdef/scdef.py` & `scdef-0.0.3/scdef/scdef.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import logging
 
 import scipy
 import numpy as np
 import pandas as pd
 from anndata import AnnData
+import scanpy as sc
 
 from scdef.util import *
 
 
 class scDEF(object):
     def __init__(
         self,
@@ -73,14 +74,16 @@
         elif isinstance(layer_diagonals, float) or isinstance(layer_diagonals, int):
             layer_diagonals = [float(layer_diagonals)] * self.n_layers
         elif len(layer_diagonals) != self.n_layers:
             raise ValueError("layer_diagonals list must be of size scDEF.n_layers")
 
         if layer_cpal is None:
             layer_cpal = ["Set1"] * self.n_layers
+            if self.n_layers <= 3:
+                layer_cpal = [f"Set{i}" for i in range(1, self.n_layers+1)]
         elif isinstance(layer_cpal, str):
             layer_cpal = [layer_cpal] * self.n_layers
         elif len(layer_cpal) != self.n_layers:
             raise ValueError("layer_cpal list must be of size scDEF.n_layers")
 
         self.layer_shapes = layer_shapes
         self.layer_diagonals = layer_diagonals
@@ -174,15 +177,15 @@
         )
         out += (
             "\n\t"
             + "Layer factor rate parameters: "
             + ", ".join([str(rate) for rate in self.factor_rates])
         )
         out += (
-            "\n\t" + "Lowe layer factor relevance prior concentration: " + str(self.brd)
+            "\n\t" + "BRD prior parameter: " + str(self.brd)
         )
         out += "\n\t" + "Number of batches: " + str(self.n_batches)
         out += "\n" + "Contains " + self.adata.__str__()
         return out
 
     def load_adata(self, adata, layer=None, batch_key="batch"):
         if not isinstance(adata, AnnData):
```

### Comparing `scdef-0.0.2/scdef/util.py` & `scdef-0.0.3/scdef/util.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.2/PKG-INFO` & `scdef-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdef
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extract hierarchical signatures of cell state from single-cell data.
 Home-page: https://github.com/cbg-ethz/scdef
 License: MIT
 Author: pedrofale
 Author-email: pedro.miguel.ferreira.pf@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

