# Comparing `tmp/scdef-0.0.4.tar.gz` & `tmp/scdef-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdef-0.0.4.tar", max compression
+gzip compressed data, was "scdef-0.0.5.tar", max compression
```

## Comparing `scdef-0.0.4.tar` & `scdef-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      983 2023-06-04 23:53:18.027853 scdef-0.0.4/README.md
--rw-r--r--   0        0        0      641 2023-06-05 01:10:04.407475 scdef-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      141 2023-06-05 01:09:01.157479 scdef-0.0.4/scdef/__init__.py
--rw-r--r--   0        0        0    10950 2023-06-04 23:23:33.986978 scdef-0.0.4/scdef/bscdef.py
--rw-r--r--   0        0        0     7953 2023-06-04 23:24:28.116267 scdef-0.0.4/scdef/iscdef.py
--rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.4/scdef/main.py
--rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.4/scdef/models/integrated.py
--rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.4/scdef/models/joint.py
--rw-r--r--   0        0        0       21 2023-06-04 23:23:30.271994 scdef-0.0.4/scdef/models/single.py
--rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.4/scdef/models/spatial.py
--rw-r--r--   0        0        0    50604 2023-06-05 00:50:35.777620 scdef-0.0.4/scdef/scdef.py
--rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.4/scdef/util.py
--rw-r--r--   0        0        0     2053 1970-01-01 00:00:00.000000 scdef-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      983 2023-06-04 23:53:18.027853 scdef-0.0.5/README.md
+-rw-r--r--   0        0        0      660 2023-06-05 02:00:48.891212 scdef-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-06-05 01:25:33.034355 scdef-0.0.5/scdef/__init__.py
+-rw-r--r--   0        0        0    13737 2023-06-05 01:13:30.448424 scdef-0.0.5/scdef/bscdef.py
+-rw-r--r--   0        0        0    10025 2023-06-05 01:13:30.354772 scdef-0.0.5/scdef/iscdef.py
+-rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.5/scdef/main.py
+-rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.5/scdef/models/integrated.py
+-rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.5/scdef/models/joint.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:42:20.961736 scdef-0.0.5/scdef/models/single.py
+-rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.5/scdef/models/spatial.py
+-rw-r--r--   0        0        0    50582 2023-06-05 01:35:39.438519 scdef-0.0.5/scdef/scdef.py
+-rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.5/scdef/util.py
+-rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 scdef-0.0.5/PKG-INFO
```

### Comparing `scdef-0.0.4/README.md` & `scdef-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `scdef-0.0.4/pyproject.toml` & `scdef-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scdef"
-version = "0.0.4"
+version = "0.0.5"
 description = "Extract hierarchical signatures of cell state from single-cell data."
 license = "MIT"
 authors = ["pedrofale <pedro.miguel.ferreira.pf@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/cbg-ethz/scdef"
 
 [tool.poetry.dependencies]
@@ -15,14 +15,15 @@
 jaxlib = "^0.3.20"
 scanpy = "^1.9.3"
 anndata = "^0.9.1"
 click = "^8.0.1"
 tqdm = "^4.64.0"
 gseapy = "^1.0.4"
 graphviz = "^0.14.2"
+igraph = "^0.10.4"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
 black = "^23.3.0"
 pytest = "^6.2.4"
 
 [tool.poetry.scripts]
```

### Comparing `scdef-0.0.4/scdef/iscdef.py` & `scdef-0.0.5/scdef/iscdef.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,71 +22,160 @@
 
 import scipy
 import numpy as np
 from anndata import AnnData
 
 
 class iscDEF(scDEF):
-    def __init__(self, adata, markers_matrix, n_factors_per_hfactor=2, gs_big_scale=2., cn_big_scale=1., gene_set_strength=1000, **kwargs):
+    def __init__(
+        self,
+        adata,
+        markers_matrix,
+        n_factors_per_hfactor=2,
+        gs_big_scale=2.0,
+        cn_big_scale=1.0,
+        gene_set_strength=1000,
+        **kwargs
+    ):
         """
         markers_matrix is a dataframe where the indices are gene symbols, columns are cell groups,
         and each entry is either 0 or 1
         """
         n_hfactors = markers_matrix.shape[1]
-        n_factors = n_factors_per_hfactor*markers_matrix.shape[1]
+        n_factors = n_factors_per_hfactor * markers_matrix.shape[1]
         self.connectivity_matrix = np.ones((n_hfactors, n_factors))
         self.gene_sets = np.ones((n_factors, adata.X.shape[1]))
 
-        super(iscDEF, self).__init__(adata, n_hfactors=n_hfactors, n_factors=n_factors, **kwargs)
+        super(iscDEF, self).__init__(
+            adata, n_hfactors=n_hfactors, n_factors=n_factors, **kwargs
+        )
 
         self.markers_matrix = markers_matrix
         self.n_factors_per_hfactor = n_factors_per_hfactor
         self.gs_big_scale = gs_big_scale
         self.cn_big_scale = cn_big_scale
         self.gene_set_strength = gene_set_strength
 
         # Build hW and W priors
-        gs_small_scale = 1/self.gs_big_scale
+        gs_small_scale = 1 / self.gs_big_scale
         cn_small_scale = 0.1
-        self.connectivity_matrix = cn_small_scale * np.ones((self.n_hfactors, self.n_factors))
+        self.connectivity_matrix = cn_small_scale * np.ones(
+            (self.n_hfactors, self.n_factors)
+        )
         self.gene_sets = np.ones((self.n_factors, self.n_genes))
         self.marker_gene_locs = []
         for i, cellgroup in enumerate(self.markers_matrix.columns):
-            self.connectivity_matrix[i,i*self.n_factors_per_hfactor:(i+1)*self.n_factors_per_hfactor] = self.cn_big_scale
+            self.connectivity_matrix[
+                i, i * self.n_factors_per_hfactor : (i + 1) * self.n_factors_per_hfactor
+            ] = self.cn_big_scale
             for gene in self.markers_matrix.index:
                 loc = np.where(self.adata.var.index == gene)[0]
                 self.marker_gene_locs.append(loc)
                 if self.markers_matrix[cellgroup].loc[gene] == 1:
-                    self.gene_sets[i*self.n_factors_per_hfactor:(i+1)*self.n_factors_per_hfactor,loc] = self.gs_big_scale
+                    self.gene_sets[
+                        i
+                        * self.n_factors_per_hfactor : (i + 1)
+                        * self.n_factors_per_hfactor,
+                        loc,
+                    ] = self.gs_big_scale
                 else:
-                    self.gene_sets[i*self.n_factors_per_hfactor:(i+1)*self.n_factors_per_hfactor,loc] = gs_small_scale
+                    self.gene_sets[
+                        i
+                        * self.n_factors_per_hfactor : (i + 1)
+                        * self.n_factors_per_hfactor,
+                        loc,
+                    ] = gs_small_scale
 
         self.init_var_params()
 
     def init_var_params(self):
         self.var_params = [
-            jnp.array((np.log(np.random.uniform(0.5, 1.5,size=[self.n_cells,1])),
-                       np.log(np.random.uniform(0.5 , 1.5,size=[self.n_cells,1])))),
-            jnp.array((np.log(np.random.uniform(0.5, 1.5,size=[1,self.n_genes])),
-                       np.log(np.random.uniform(0.5 , 1.5,size=[1,self.n_genes])))),
-            jnp.array((np.log(np.random.uniform(0.5, 1.5, size=[self.n_hfactors,1])),
-                       np.log(np.random.uniform(0.5, 1.5, size=[self.n_hfactors,1])))), # hfactor_scales
-            jnp.array((np.log(np.random.uniform(0.5, 1.5, size=[self.n_factors,1])),
-                       np.log(np.random.uniform(0.5, 1.5, size=[self.n_factors,1])))), # factor_scales
-            jnp.array((np.log(np.random.uniform(0.5 * self.shape, 1.5* self.shape,size=[self.n_cells,self.n_hfactors])), # hz
-                       np.log(np.random.uniform(0.5 * self.shape, 1.5* self.shape,size=[self.n_cells,self.n_hfactors])))),
-            jnp.array((np.log(np.random.uniform(0.5 * self.connectivity_matrix, 1.5 * self.connectivity_matrix)), # hW
-                       np.log(np.random.uniform(0.5, 1.5,size=[self.n_hfactors,self.n_factors])))),
-            jnp.array((np.log(np.random.uniform(0.5 * self.shape, 1.5* self.shape,size=[self.n_cells,self.n_factors])), # z
-                       np.log(np.random.uniform(0.5, 1.5,size=[self.n_cells,self.n_factors])))),
-            jnp.array((np.log(np.random.uniform(0.5 * self.gene_sets, 1.5 * self.gene_sets)), # W
-                       np.log(np.random.uniform(0.5, 1.5,size=[self.n_factors,self.n_genes])))),
+            jnp.array(
+                (
+                    np.log(np.random.uniform(0.5, 1.5, size=[self.n_cells, 1])),
+                    np.log(np.random.uniform(0.5, 1.5, size=[self.n_cells, 1])),
+                )
+            ),
+            jnp.array(
+                (
+                    np.log(np.random.uniform(0.5, 1.5, size=[1, self.n_genes])),
+                    np.log(np.random.uniform(0.5, 1.5, size=[1, self.n_genes])),
+                )
+            ),
+            jnp.array(
+                (
+                    np.log(np.random.uniform(0.5, 1.5, size=[self.n_hfactors, 1])),
+                    np.log(np.random.uniform(0.5, 1.5, size=[self.n_hfactors, 1])),
+                )
+            ),  # hfactor_scales
+            jnp.array(
+                (
+                    np.log(np.random.uniform(0.5, 1.5, size=[self.n_factors, 1])),
+                    np.log(np.random.uniform(0.5, 1.5, size=[self.n_factors, 1])),
+                )
+            ),  # factor_scales
+            jnp.array(
+                (
+                    np.log(
+                        np.random.uniform(
+                            0.5 * self.shape,
+                            1.5 * self.shape,
+                            size=[self.n_cells, self.n_hfactors],
+                        )
+                    ),  # hz
+                    np.log(
+                        np.random.uniform(
+                            0.5 * self.shape,
+                            1.5 * self.shape,
+                            size=[self.n_cells, self.n_hfactors],
+                        )
+                    ),
+                )
+            ),
+            jnp.array(
+                (
+                    np.log(
+                        np.random.uniform(
+                            0.5 * self.connectivity_matrix,
+                            1.5 * self.connectivity_matrix,
+                        )
+                    ),  # hW
+                    np.log(
+                        np.random.uniform(
+                            0.5, 1.5, size=[self.n_hfactors, self.n_factors]
+                        )
+                    ),
+                )
+            ),
+            jnp.array(
+                (
+                    np.log(
+                        np.random.uniform(
+                            0.5 * self.shape,
+                            1.5 * self.shape,
+                            size=[self.n_cells, self.n_factors],
+                        )
+                    ),  # z
+                    np.log(
+                        np.random.uniform(0.5, 1.5, size=[self.n_cells, self.n_factors])
+                    ),
+                )
+            ),
+            jnp.array(
+                (
+                    np.log(
+                        np.random.uniform(0.5 * self.gene_sets, 1.5 * self.gene_sets)
+                    ),  # W
+                    np.log(
+                        np.random.uniform(0.5, 1.5, size=[self.n_factors, self.n_genes])
+                    ),
+                )
+            ),
         ]
 
-
     def elbo(self, rng, indices, var_params):
         # Single-sample Monte Carlo estimate of the variational lower bound.
         batch_indices_onehot = self.batch_indices_onehot[indices]
 
         min_loc = jnp.log(1e-10)
         cell_budget_params = jnp.clip(var_params[0], a_min=min_loc)
         gene_budget_params = jnp.clip(var_params[1], a_min=min_loc)
@@ -95,28 +184,46 @@
         z_params = jnp.clip(var_params[6], a_min=min_loc)
         W_params = jnp.clip(var_params[7], a_min=min_loc)
 
         min_concentration = 1e-10
         min_scale = 1e-10
         min_rate = 1e-10
         max_rate = 1e10
-        cell_budget_concentration = jnp.maximum(jnp.exp(cell_budget_params[0][indices]), min_concentration)
-        cell_budget_rate = jnp.minimum(jnp.maximum(jnp.exp(cell_budget_params[1][indices]), min_rate), max_rate)
+        cell_budget_concentration = jnp.maximum(
+            jnp.exp(cell_budget_params[0][indices]), min_concentration
+        )
+        cell_budget_rate = jnp.minimum(
+            jnp.maximum(jnp.exp(cell_budget_params[1][indices]), min_rate), max_rate
+        )
 
         z_concentration = jnp.maximum(jnp.exp(z_params[0][indices]), min_concentration)
-        z_rate = jnp.minimum(jnp.maximum(jnp.exp(z_params[1][indices]), min_rate), max_rate)
-
-        hz_concentration = jnp.maximum(jnp.exp(hz_params[0][indices]), min_concentration)
-        hz_rate = jnp.minimum(jnp.maximum(jnp.exp(hz_params[1][indices]), min_rate), max_rate)
-
-        gene_budget_concentration = jnp.maximum(jnp.exp(gene_budget_params[0]), min_concentration)
-        gene_budget_rate = jnp.minimum(jnp.maximum(jnp.exp(gene_budget_params[1]), min_rate), max_rate)
-
-        factor_scale_concentration = jnp.maximum(jnp.exp(factor_scale_params[0]), min_concentration)
-        factor_scale_rate = jnp.minimum(jnp.maximum(jnp.exp(factor_scale_params[1]), min_rate), max_rate)
+        z_rate = jnp.minimum(
+            jnp.maximum(jnp.exp(z_params[1][indices]), min_rate), max_rate
+        )
+
+        hz_concentration = jnp.maximum(
+            jnp.exp(hz_params[0][indices]), min_concentration
+        )
+        hz_rate = jnp.minimum(
+            jnp.maximum(jnp.exp(hz_params[1][indices]), min_rate), max_rate
+        )
+
+        gene_budget_concentration = jnp.maximum(
+            jnp.exp(gene_budget_params[0]), min_concentration
+        )
+        gene_budget_rate = jnp.minimum(
+            jnp.maximum(jnp.exp(gene_budget_params[1]), min_rate), max_rate
+        )
+
+        factor_scale_concentration = jnp.maximum(
+            jnp.exp(factor_scale_params[0]), min_concentration
+        )
+        factor_scale_rate = jnp.minimum(
+            jnp.maximum(jnp.exp(factor_scale_params[1]), min_rate), max_rate
+        )
 
         W_concentration = jnp.maximum(jnp.exp(W_params[0]), min_concentration)
         W_rate = jnp.minimum(jnp.maximum(jnp.exp(W_params[1]), min_rate), max_rate)
 
         hW_concentration = jnp.maximum(jnp.exp(hW_params[0]), min_concentration)
         hW_rate = jnp.minimum(jnp.maximum(jnp.exp(hW_params[1]), min_rate), max_rate)
 
@@ -125,37 +232,45 @@
         gene_budgets = gamma_sample(rng, gene_budget_concentration, gene_budget_rate)
 
         hz = gamma_sample(rng, hz_concentration, hz_rate)
         hW = gamma_sample(rng, hW_concentration, hW_rate)
         mean_top = jnp.matmul(hz, hW)
         z = gamma_sample(rng, z_concentration, z_rate)
         W = gamma_sample(rng, W_concentration, W_rate)
-        mean_bottom_bio = jnp.matmul(z, W )
+        mean_bottom_bio = jnp.matmul(z, W)
         mean_bottom = mean_bottom_bio
 
         # Compute log likelihood
         ll = jnp.sum(vmap(poisson.logpmf)(self.X[indices], mean_bottom))
 
         # Compute KL divergence
-        kl = 0.
-        kl += gamma_logpdf(gene_budgets, 1., self.gene_ratio) -\
-                gamma_logpdf(gene_budgets, gene_budget_concentration, gene_budget_rate)
-
-        kl += gamma_logpdf(hW, self.connectivity_matrix, 1.) -\
-                gamma_logpdf(hW, hW_concentration, hW_rate)
-
-        kl += gamma_logpdf(W, self.gene_set_strength*self.gene_sets, self.gene_set_strength*gene_budgets) -\
-                gamma_logpdf(W, W_concentration, W_rate)
-
-        kl *= indices.shape[0] / self.X.shape[0] # scale by minibatch size
-
-        kl += gamma_logpdf(cell_budgets, 1., 1.*self.batch_lib_ratio[indices]) -\
-                gamma_logpdf(cell_budgets, cell_budget_concentration, cell_budget_rate)
-
-        kl += gamma_logpdf(hz, self.shape,  self.shape) -\
-                gamma_logpdf(hz, hz_concentration, hz_rate)
+        kl = 0.0
+        kl += gamma_logpdf(gene_budgets, 1.0, self.gene_ratio) - gamma_logpdf(
+            gene_budgets, gene_budget_concentration, gene_budget_rate
+        )
+
+        kl += gamma_logpdf(hW, self.connectivity_matrix, 1.0) - gamma_logpdf(
+            hW, hW_concentration, hW_rate
+        )
+
+        kl += gamma_logpdf(
+            W,
+            self.gene_set_strength * self.gene_sets,
+            self.gene_set_strength * gene_budgets,
+        ) - gamma_logpdf(W, W_concentration, W_rate)
+
+        kl *= indices.shape[0] / self.X.shape[0]  # scale by minibatch size
+
+        kl += gamma_logpdf(
+            cell_budgets, 1.0, 1.0 * self.batch_lib_ratio[indices]
+        ) - gamma_logpdf(cell_budgets, cell_budget_concentration, cell_budget_rate)
+
+        kl += gamma_logpdf(hz, self.shape, self.shape) - gamma_logpdf(
+            hz, hz_concentration, hz_rate
+        )
 
         # Tieing the scales avoids the factors with low scales in W learn z's that correlate with cell scales
-        kl += gamma_logpdf(z, self.shape, cell_budgets * self.shape / mean_top  ) -\
-                gamma_logpdf(z, z_concentration, z_rate)
+        kl += gamma_logpdf(
+            z, self.shape, cell_budgets * self.shape / mean_top
+        ) - gamma_logpdf(z, z_concentration, z_rate)
 
         return ll + kl
```

### Comparing `scdef-0.0.4/scdef/main.py` & `scdef-0.0.5/scdef/main.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.4/scdef/models/integrated.py` & `scdef-0.0.5/scdef/models/integrated.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.4/scdef/models/joint.py` & `scdef-0.0.5/scdef/models/joint.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.4/scdef/models/spatial.py` & `scdef-0.0.5/scdef/models/spatial.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.4/scdef/scdef.py` & `scdef-0.0.5/scdef/scdef.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             layer_diagonals = [float(layer_diagonals)] * self.n_layers
         elif len(layer_diagonals) != self.n_layers:
             raise ValueError("layer_diagonals list must be of size scDEF.n_layers")
 
         if layer_cpal is None:
             layer_cpal = ["Set1"] * self.n_layers
             if self.n_layers <= 3:
-                layer_cpal = [f"Set{i}" for i in range(1, self.n_layers+1)]
+                layer_cpal = [f"Set{i}" for i in range(1, self.n_layers + 1)]
         elif isinstance(layer_cpal, str):
             layer_cpal = [layer_cpal] * self.n_layers
         elif len(layer_cpal) != self.n_layers:
             raise ValueError("layer_cpal list must be of size scDEF.n_layers")
 
         self.layer_shapes = layer_shapes
         self.layer_diagonals = layer_diagonals
@@ -176,17 +176,15 @@
             + ", ".join([str(shape) for shape in self.factor_shapes])
         )
         out += (
             "\n\t"
             + "Layer factor rate parameters: "
             + ", ".join([str(rate) for rate in self.factor_rates])
         )
-        out += (
-            "\n\t" + "BRD prior parameter: " + str(self.brd)
-        )
+        out += "\n\t" + "BRD prior parameter: " + str(self.brd)
         out += "\n\t" + "Number of batches: " + str(self.n_batches)
         out += "\n" + "Contains " + self.adata.__str__()
         return out
 
     def load_adata(self, adata, layer=None, batch_key="batch"):
         if not isinstance(adata, AnnData):
             raise TypeError("adata must be an instance of AnnData.")
```

### Comparing `scdef-0.0.4/scdef/util.py` & `scdef-0.0.5/scdef/util.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.4/PKG-INFO` & `scdef-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdef
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extract hierarchical signatures of cell state from single-cell data.
 Home-page: https://github.com/cbg-ethz/scdef
 License: MIT
 Author: pedrofale
 Author-email: pedro.miguel.ferreira.pf@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anndata (>=0.9.1,<0.10.0)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: graphviz (>=0.14.2,<0.15.0)
 Requires-Dist: gseapy (>=1.0.4,<2.0.0)
+Requires-Dist: igraph (>=0.10.4,<0.11.0)
 Requires-Dist: jax (>=0.3.20,<0.4.0)
 Requires-Dist: jaxlib (>=0.3.20,<0.4.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: scanpy (>=1.9.3,<2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Project-URL: Repository, https://github.com/cbg-ethz/scdef
```

