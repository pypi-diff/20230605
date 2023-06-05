# Comparing `tmp/scdef-0.0.5.tar.gz` & `tmp/scdef-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdef-0.0.5.tar", max compression
+gzip compressed data, was "scdef-0.0.6.tar", max compression
```

## Comparing `scdef-0.0.5.tar` & `scdef-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      983 2023-06-04 23:53:18.027853 scdef-0.0.5/README.md
--rw-r--r--   0        0        0      660 2023-06-05 02:00:48.891212 scdef-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      141 2023-06-05 01:25:33.034355 scdef-0.0.5/scdef/__init__.py
--rw-r--r--   0        0        0    13737 2023-06-05 01:13:30.448424 scdef-0.0.5/scdef/bscdef.py
--rw-r--r--   0        0        0    10025 2023-06-05 01:13:30.354772 scdef-0.0.5/scdef/iscdef.py
--rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.5/scdef/main.py
--rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.5/scdef/models/integrated.py
--rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.5/scdef/models/joint.py
--rw-r--r--   0        0        0        0 2023-06-05 01:42:20.961736 scdef-0.0.5/scdef/models/single.py
--rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.5/scdef/models/spatial.py
--rw-r--r--   0        0        0    50582 2023-06-05 01:35:39.438519 scdef-0.0.5/scdef/scdef.py
--rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.5/scdef/util.py
--rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 scdef-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      961 2023-06-05 12:00:48.737739 scdef-0.0.6/README.md
+-rw-r--r--   0        0        0      660 2023-06-05 17:13:49.185037 scdef-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-06-05 01:25:33.034355 scdef-0.0.6/scdef/__init__.py
+-rw-r--r--   0        0        0    13737 2023-06-05 01:13:30.448424 scdef-0.0.6/scdef/bscdef.py
+-rw-r--r--   0        0        0    10025 2023-06-05 01:13:30.354772 scdef-0.0.6/scdef/iscdef.py
+-rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.6/scdef/main.py
+-rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.6/scdef/models/integrated.py
+-rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.6/scdef/models/joint.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:42:20.961736 scdef-0.0.6/scdef/models/single.py
+-rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.6/scdef/models/spatial.py
+-rw-r--r--   0        0        0    50586 2023-06-05 17:05:58.304170 scdef-0.0.6/scdef/scdef.py
+-rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.6/scdef/util.py
+-rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 scdef-0.0.6/PKG-INFO
```

### Comparing `scdef-0.0.5/README.md` & `scdef-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <div align="left">
   <img src="https://github.com/cbg-ethz/scDEF/raw/main/figures/scdef.png", width="300px">
 </div>
 <p></p>
 
 [![pypi](https://img.shields.io/pypi/v/scdef.svg?style=flat)](https://pypi.python.org/pypi/scdef)
-[![build](https://github.com/cbg-ethz/scDEF/actions/workflows/main.yaml/badge.svg)](https://github.com/cbg-ethz/scDEF/actions/workflows/main.yaml) 
+[![build](https://github.com/cbg-ethz/scDEF/actions/workflows/main.yaml/badge.svg)](https://github.com/cbg-ethz/scDEF/actions/workflows/main.yaml)
 
 Deep exponential families for single-cell data. scDEF learns *de novo* gene signatures from scRNA-seq data at multiple levels of resolution.
 
 ## Installation
 ```
 pip install scdef
 ```
 
 Please be sure to install a version of [JAX](https://jax.readthedocs.io/) that is compatible with your GPU (if applicable).
 
 ## Getting started
-scDEF takes as input an [AnnData](https://anndata.readthedocs.io/) object containing filtered, but not normalized, UMI counts. The [notebooks](https://github.com/cbg-ethz/scDEF/notebooks/) directory contains IPython notebooks with examples showcasing the analyses enabled by scDEF.
+scDEF takes as input an [AnnData](https://anndata.readthedocs.io/) object containing UMI counts. The [notebooks](https://github.com/cbg-ethz/scDEF/tree/main/notebooks) directory contains IPython notebooks with examples showcasing the analyses enabled by scDEF.
```

### Comparing `scdef-0.0.5/pyproject.toml` & `scdef-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scdef"
-version = "0.0.5"
+version = "0.0.6"
 description = "Extract hierarchical signatures of cell state from single-cell data."
 license = "MIT"
 authors = ["pedrofale <pedro.miguel.ferreira.pf@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/cbg-ethz/scdef"
 
 [tool.poetry.dependencies]
```

### Comparing `scdef-0.0.5/scdef/bscdef.py` & `scdef-0.0.6/scdef/bscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.5/scdef/iscdef.py` & `scdef-0.0.6/scdef/iscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.5/scdef/main.py` & `scdef-0.0.6/scdef/main.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.5/scdef/models/integrated.py` & `scdef-0.0.6/scdef/models/integrated.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.5/scdef/models/joint.py` & `scdef-0.0.6/scdef/models/joint.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.5/scdef/models/spatial.py` & `scdef-0.0.6/scdef/models/spatial.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.5/scdef/scdef.py` & `scdef-0.0.6/scdef/scdef.py`

 * *Files 0% similar despite different names*

```diff
@@ -912,24 +912,24 @@
             raise IndexError("top_genes list must be of size scDEF.n_layers")
 
         if filled is None:
             style = None
         elif filled == "factor":
             style = "filled"
         else:
-            if filled not in scd.adata.obs:
+            if filled not in self.adata.obs:
                 raise ValueError("filled must be factor or any `obs` in self.adata")
             else:
                 style = "filled"
 
         if style is None:
             if wedged is None:
                 style = None
             else:
-                if wedged not in scd.adata.obs:
+                if wedged not in self.adata.obs:
                     raise ValueError("wedged must be any `obs` in self.adata")
                 else:
                     style = "wedged"
         else:
             if wedged is not None:
                 self.logger.info("Filled style takes precedence over wedged")
 
@@ -996,15 +996,15 @@
                         cells = np.where(
                             self.adata.obs[f"{layer_name}factor"] == str(factor_idx)
                         )[0]
                         if len(cells) > 0:
                             # cells in this factor that belong to each obs
                             prevs = [
                                 np.count_nonzero(self.adata.obs[filled][cells] == b)
-                                for b in scd.adata.obs[filled].unique()
+                                for b in self.adata.obs[filled].unique()
                             ]
                             obs_idx = np.argmax(prevs)  # obs attachment
                             alpha = prevs[obs_idx] / np.sum(
                                 prevs
                             )  # confidence on obs_idx attachment -- should I account for the number of cells in each batch in total?
                             alpha = matplotlib.colors.rgb2hex(
                                 (0, 0, 0, alpha), keep_alpha=True
@@ -1017,15 +1017,15 @@
                     cells = np.where(
                         self.adata.obs[f"{layer_name}factor"] == str(factor_idx)
                     )[0]
                     if len(cells) > 0:
                         # cells in this factor that belong to each obs
                         prevs = [
                             np.count_nonzero(self.adata.obs[wedged][cells] == b)
-                            for b in scd.adata.obs[wedged].unique()
+                            for b in self.adata.obs[wedged].unique()
                         ]
                         fracs = prevs / np.sum(prevs)
                         # make color string for pie chart
                         fillcolor = ":".join(
                             [
                                 f"{self.adata.uns[f'{wedged}_colors'][obs_idx]};{frac}"
                                 for obs_idx, frac in enumerate(fracs)
```

### Comparing `scdef-0.0.5/scdef/util.py` & `scdef-0.0.6/scdef/util.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.5/PKG-INFO` & `scdef-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdef
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extract hierarchical signatures of cell state from single-cell data.
 Home-page: https://github.com/cbg-ethz/scdef
 License: MIT
 Author: pedrofale
 Author-email: pedro.miguel.ferreira.pf@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -29,21 +29,21 @@
 
 <div align="left">
   <img src="https://github.com/cbg-ethz/scDEF/raw/main/figures/scdef.png", width="300px">
 </div>
 <p></p>
 
 [![pypi](https://img.shields.io/pypi/v/scdef.svg?style=flat)](https://pypi.python.org/pypi/scdef)
-[![build](https://github.com/cbg-ethz/scDEF/actions/workflows/main.yaml/badge.svg)](https://github.com/cbg-ethz/scDEF/actions/workflows/main.yaml) 
+[![build](https://github.com/cbg-ethz/scDEF/actions/workflows/main.yaml/badge.svg)](https://github.com/cbg-ethz/scDEF/actions/workflows/main.yaml)
 
 Deep exponential families for single-cell data. scDEF learns *de novo* gene signatures from scRNA-seq data at multiple levels of resolution.
 
 ## Installation
 ```
 pip install scdef
 ```
 
 Please be sure to install a version of [JAX](https://jax.readthedocs.io/) that is compatible with your GPU (if applicable).
 
 ## Getting started
-scDEF takes as input an [AnnData](https://anndata.readthedocs.io/) object containing filtered, but not normalized, UMI counts. The [notebooks](https://github.com/cbg-ethz/scDEF/notebooks/) directory contains IPython notebooks with examples showcasing the analyses enabled by scDEF.
+scDEF takes as input an [AnnData](https://anndata.readthedocs.io/) object containing UMI counts. The [notebooks](https://github.com/cbg-ethz/scDEF/tree/main/notebooks) directory contains IPython notebooks with examples showcasing the analyses enabled by scDEF.
```

