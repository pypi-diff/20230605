# Comparing `tmp/scdef-0.0.1.tar.gz` & `tmp/scdef-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdef-0.0.1.tar", max compression
+gzip compressed data, was "scdef-0.0.2.tar", max compression
```

## Comparing `scdef-0.0.1.tar` & `scdef-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0      429 2022-10-17 12:52:20.724622 scdef-0.0.1/README.md
--rw-r--r--   0        0        0      641 2023-06-04 23:01:06.486540 scdef-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-06-04 22:36:21.759434 scdef-0.0.1/scdef/__init__.py
--rw-r--r--   0        0        0    10950 2023-06-04 22:41:15.840361 scdef-0.0.1/scdef/bscdef.py
--rw-r--r--   0        0        0     7953 2023-06-04 22:37:30.112390 scdef-0.0.1/scdef/iscdef.py
--rw-r--r--   0        0        0     2993 2023-06-04 21:59:58.686871 scdef-0.0.1/scdef/main.py
--rw-r--r--   0        0        0       29 2022-10-14 22:08:14.017012 scdef-0.0.1/scdef/models/__init__.py
--rw-r--r--   0        0        0     6928 2022-07-13 07:23:03.532435 scdef-0.0.1/scdef/models/integrated.py
--rw-r--r--   0        0        0     6892 2022-07-13 07:23:59.804540 scdef-0.0.1/scdef/models/joint.py
--rw-r--r--   0        0        0       21 2022-07-13 07:17:40.291393 scdef-0.0.1/scdef/models/single.py
--rw-r--r--   0        0        0    17568 2022-08-25 17:11:00.366742 scdef-0.0.1/scdef/models/spatial.py
--rw-r--r--   0        0        0    43343 2023-06-04 22:35:49.786104 scdef-0.0.1/scdef/scdef.py
--rw-r--r--   0        0        0     3108 2023-04-18 07:59:07.253000 scdef-0.0.1/scdef/util.py
--rw-r--r--   0        0        0     1461 2023-06-04 23:03:27.239137 scdef-0.0.1/setup.py
--rw-r--r--   0        0        0     1448 2023-06-04 23:03:27.239472 scdef-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      983 2023-06-04 23:53:18.027853 scdef-0.0.2/README.md
+-rw-r--r--   0        0        0      641 2023-06-05 00:08:18.411482 scdef-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-06-04 22:36:21.759434 scdef-0.0.2/scdef/__init__.py
+-rw-r--r--   0        0        0    10950 2023-06-04 23:23:33.986978 scdef-0.0.2/scdef/bscdef.py
+-rw-r--r--   0        0        0     7953 2023-06-04 23:24:28.116267 scdef-0.0.2/scdef/iscdef.py
+-rw-r--r--   0        0        0     3113 2023-06-04 23:18:51.711931 scdef-0.0.2/scdef/main.py
+-rw-r--r--   0        0        0     7584 2023-06-04 23:23:31.968859 scdef-0.0.2/scdef/models/integrated.py
+-rw-r--r--   0        0        0     7548 2023-06-04 23:23:29.433437 scdef-0.0.2/scdef/models/joint.py
+-rw-r--r--   0        0        0       21 2023-06-04 23:23:30.271994 scdef-0.0.2/scdef/models/single.py
+-rw-r--r--   0        0        0    20159 2023-06-04 23:23:30.962929 scdef-0.0.2/scdef/models/spatial.py
+-rw-r--r--   0        0        0    50501 2023-06-05 00:03:59.456164 scdef-0.0.2/scdef/scdef.py
+-rw-r--r--   0        0        0     3328 2023-06-04 23:18:52.167043 scdef-0.0.2/scdef/util.py
+-rw-r--r--   0        0        0     2053 1970-01-01 00:00:00.000000 scdef-0.0.2/PKG-INFO
```

### Comparing `scdef-0.0.1/pyproject.toml` & `scdef-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scdef"
-version = "0.0.1"
+version = "0.0.2"
 description = "Extract hierarchical signatures of cell state from single-cell data."
 license = "MIT"
 authors = ["pedrofale <pedro.miguel.ferreira.pf@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/cbg-ethz/scdef"
 
 [tool.poetry.dependencies]
@@ -18,12 +18,12 @@
 click = "^8.0.1"
 tqdm = "^4.64.0"
 gseapy = "^1.0.4"
 graphviz = "^0.14.2"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
-black = "^22.3.0"
+black = "^23.3.0"
 pytest = "^6.2.4"
 
 [tool.poetry.scripts]
 scdef = "scdef:main"
```

### Comparing `scdef-0.0.1/scdef/bscdef.py` & `scdef-0.0.2/scdef/bscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.1/scdef/iscdef.py` & `scdef-0.0.2/scdef/iscdef.py`

 * *Files identical despite different names*

### Comparing `scdef-0.0.1/scdef/main.py` & `scdef-0.0.2/scdef/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,25 @@
 import pandas as pd
 
 import logging
 import click
 import os
 from pathlib import Path
 
-@click.command(help="Extract hierarchical signatures of cell state from single-cell data.")
-@click.argument("--input-data",type=click.Path(exists=True, dir_okay=False))
-@click.option("-l", "--level-sizes", default=[10, 3], help="List of sizes for different levels, starting from the lowest level.")
+
+@click.command(
+    help="Extract hierarchical signatures of cell state from single-cell data."
+)
+@click.argument("--input-data", type=click.Path(exists=True, dir_okay=False))
+@click.option(
+    "-l",
+    "--level-sizes",
+    default=[10, 3],
+    help="List of sizes for different levels, starting from the lowest level.",
+)
 @click.option(
     "-e",
     "--epochs",
     default=1000,
     help="Number of epochs to run.",
 )
 @click.option(
@@ -55,51 +63,68 @@
     "--verbose",
     is_flag=True,
     help="Report inference diagnostics.",
 )
 @click.option(
     "-o",
     "--output-path",
-    default='./',
+    default="./",
     help="Output directory.",
 )
 def main(
-    input_file, level_sizes, epochs, minibatch_size, step_size, mc_samples, max_genes, batch_key, verbose, output_path
+    input_file,
+    level_sizes,
+    epochs,
+    minibatch_size,
+    step_size,
+    mc_samples,
+    max_genes,
+    batch_key,
+    verbose,
+    output_path,
 ):
     logging.basicConfig(level=logging.INFO)
 
     adata = sc.read_h5ad(input_file)
 
     # Do some basic pre-processing
     adata.var_names_make_unique()
     sc.pp.filter_cells(adata, min_genes=200)
     sc.pp.filter_genes(adata, min_cells=3)
-    adata.var['mt'] = adata.var_names.str.startswith('MT-')  # annotate the group of mitochondrial genes as 'mt'
-    sc.pp.calculate_qc_metrics(adata, qc_vars=['mt'], percent_top=None, log1p=False, inplace=True)
+    adata.var["mt"] = adata.var_names.str.startswith(
+        "MT-"
+    )  # annotate the group of mitochondrial genes as 'mt'
+    sc.pp.calculate_qc_metrics(
+        adata, qc_vars=["mt"], percent_top=None, log1p=False, inplace=True
+    )
     adata = adata[adata.obs.n_genes_by_counts < 2500, :]
     adata = adata[adata.obs.pct_counts_mt < 5, :]
     adata.raw = adata
     raw_adata = adata.raw
     raw_adata = raw_adata.to_adata()
     raw_adata.X = raw_adata.X.toarray()
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
-    sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5, n_top_genes=max_genes)
+    sc.pp.highly_variable_genes(
+        adata, min_mean=0.0125, max_mean=3, min_disp=0.5, n_top_genes=max_genes
+    )
     raw_adata = raw_adata[:, adata.var.highly_variable]
 
     # Run scDEF
     scdef = scDEF(raw_adata, layer_sizes=level_sizes)
-    elbos = scdef.optimize(n_epochs=epochs, batch_size=minibatch_size, lr=step_size, num_samples=mc_samples)
+    elbos = scdef.optimize(
+        n_epochs=epochs, batch_size=minibatch_size, lr=step_size, num_samples=mc_samples
+    )
 
     summary = scdef.get_summary(top_genes=5)
 
     # Save object, annotated AnnData and graph
     Path(output_path).mkdir(parents=True, exist_ok=True)
-    pickle.dump(scdef, os.path.join(output_path, 'scdef.pkl'))
-    scdef.adata.write(os.path.join(output_path), 'scdef_adata.h5ad')
+    pickle.dump(scdef, os.path.join(output_path, "scdef.pkl"))
+    scdef.adata.write(os.path.join(output_path), "scdef_adata.h5ad")
     scd.graph.render(directory=output_path)
 
     logging.info(f"Saved results to {output_path}.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `scdef-0.0.1/scdef/models/integrated.py` & `scdef-0.0.2/scdef/models/integrated.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,130 +1,171 @@
 class Integrated(scDEF):
     """
     Different cells, overlapping genes between two modalities.
     """
+
     def elbo(self, rng, indices, var_params):
         # Single-sample Monte Carlo estimate of the variational lower bound.
         batch_indices_onehot = self.batch_indices_onehot[indices]
 
         min_loc = jnp.log(1e-10)
         cell_scale_params = jnp.clip(var_params[0], a_min=min_loc)
         gene_scale_params = jnp.clip(var_params[1], a_min=min_loc)
-#         unconst_gene_scales = jnp.clip(var_params[1], a_min=min_loc)
+        #         unconst_gene_scales = jnp.clip(var_params[1], a_min=min_loc)
         hfactor_scale_params = jnp.clip(var_params[2], a_min=min_loc)
         factor_scale_params = jnp.clip(var_params[3], a_min=min_loc)
         hz_params = jnp.clip(var_params[4], a_min=min_loc)
         hW_params = jnp.clip(var_params[5], a_min=min_loc)
-#         unconst_hW = jnp.clip(var_params[5], a_min=min_loc)
+        #         unconst_hW = jnp.clip(var_params[5], a_min=min_loc)
         z_params = jnp.clip(var_params[6], a_min=min_loc)
         W_params = jnp.clip(var_params[7], a_min=min_loc)
-#         unconst_W = jnp.clip(var_params[7], a_min=min_loc)
+        #         unconst_W = jnp.clip(var_params[7], a_min=min_loc)
         W_noise_params = jnp.clip(var_params[8], a_min=min_loc)
         z_noise_params = jnp.clip(var_params[9], a_min=min_loc)
 
         min_concentration = 1e-10
         min_scale = 1e-10
-        cell_scale_concentration = jnp.maximum(jnn.softplus(cell_scale_params[0][indices]), min_concentration)
-        cell_scale_rate = 1./jnp.maximum(jnn.softplus(cell_scale_params[1][indices]), min_scale)
-
-        z_concentration = jnp.maximum(jnn.softplus(z_params[0][indices]), min_concentration)
-        z_rate = 1./jnp.maximum(jnn.softplus(z_params[1][indices]), min_scale)
-
-        hz_concentration = jnp.maximum(jnn.softplus(hz_params[0][indices]), min_concentration)
-        hz_rate = 1./jnp.maximum(jnn.softplus(hz_params[1][indices]), min_scale)
-
-        gene_scale_concentration = jnp.maximum(jnn.softplus(gene_scale_params[0]), min_concentration)
-        gene_scale_rate = 1./jnp.maximum(jnn.softplus(gene_scale_params[1]), min_scale)
-
-        hfactor_scale_concentration = jnp.maximum(jnn.softplus(hfactor_scale_params[0]), min_concentration)
-        hfactor_scale_rate = 1./jnp.maximum(jnn.softplus(hfactor_scale_params[1]), min_scale)
-
-        factor_scale_concentration = jnp.maximum(jnn.softplus(factor_scale_params[0]), min_concentration)
-        factor_scale_rate = 1./jnp.maximum(jnn.softplus(factor_scale_params[1]), min_scale)
+        cell_scale_concentration = jnp.maximum(
+            jnn.softplus(cell_scale_params[0][indices]), min_concentration
+        )
+        cell_scale_rate = 1.0 / jnp.maximum(
+            jnn.softplus(cell_scale_params[1][indices]), min_scale
+        )
+
+        z_concentration = jnp.maximum(
+            jnn.softplus(z_params[0][indices]), min_concentration
+        )
+        z_rate = 1.0 / jnp.maximum(jnn.softplus(z_params[1][indices]), min_scale)
+
+        hz_concentration = jnp.maximum(
+            jnn.softplus(hz_params[0][indices]), min_concentration
+        )
+        hz_rate = 1.0 / jnp.maximum(jnn.softplus(hz_params[1][indices]), min_scale)
+
+        gene_scale_concentration = jnp.maximum(
+            jnn.softplus(gene_scale_params[0]), min_concentration
+        )
+        gene_scale_rate = 1.0 / jnp.maximum(
+            jnn.softplus(gene_scale_params[1]), min_scale
+        )
+
+        hfactor_scale_concentration = jnp.maximum(
+            jnn.softplus(hfactor_scale_params[0]), min_concentration
+        )
+        hfactor_scale_rate = 1.0 / jnp.maximum(
+            jnn.softplus(hfactor_scale_params[1]), min_scale
+        )
+
+        factor_scale_concentration = jnp.maximum(
+            jnn.softplus(factor_scale_params[0]), min_concentration
+        )
+        factor_scale_rate = 1.0 / jnp.maximum(
+            jnn.softplus(factor_scale_params[1]), min_scale
+        )
 
         W_concentration = jnp.maximum(jnn.softplus(W_params[0]), min_concentration)
-        W_rate = 1./jnp.maximum(jnn.softplus(W_params[1]), min_scale)
+        W_rate = 1.0 / jnp.maximum(jnn.softplus(W_params[1]), min_scale)
 
         hW_concentration = jnp.maximum(jnn.softplus(hW_params[0]), min_concentration)
-        hW_rate = 1./jnp.maximum(jnn.softplus(hW_params[1]), min_scale)
+        hW_rate = 1.0 / jnp.maximum(jnn.softplus(hW_params[1]), min_scale)
 
-        z_noise_concentration = jnp.maximum(jnn.softplus(z_noise_params[0][indices]), min_concentration)
-        z_noise_rate = 1./jnp.maximum(jnn.softplus(z_noise_params[1][indices]), min_scale)
-
-        W_noise_concentration = jnp.maximum(jnn.softplus(W_noise_params[0]), min_concentration)
-        W_noise_rate = 1./jnp.maximum(jnn.softplus(W_noise_params[1]), min_scale)
+        z_noise_concentration = jnp.maximum(
+            jnn.softplus(z_noise_params[0][indices]), min_concentration
+        )
+        z_noise_rate = 1.0 / jnp.maximum(
+            jnn.softplus(z_noise_params[1][indices]), min_scale
+        )
+
+        W_noise_concentration = jnp.maximum(
+            jnn.softplus(W_noise_params[0]), min_concentration
+        )
+        W_noise_rate = 1.0 / jnp.maximum(jnn.softplus(W_noise_params[1]), min_scale)
 
         # Sample from variational distribution
         cell_scales = gamma_sample(rng, cell_scale_concentration, cell_scale_rate)
-#         cell_scales = jnp.exp(log_cell_scales)
+        #         cell_scales = jnp.exp(log_cell_scales)
         gene_scales = gamma_sample(rng, gene_scale_concentration, gene_scale_rate)
-#         gene_scales = jnp.exp(log_gene_scales)
-#         gene_scales = jnn.softplus(unconst_gene_scales)
+        #         gene_scales = jnp.exp(log_gene_scales)
+        #         gene_scales = jnn.softplus(unconst_gene_scales)
 
-#         log_hfactor_scales = gaussian_sample(rng, hfactor_scale_params[0], hfactor_scale_params[1])
-#         hfactor_scales = jnp.exp(log_hfactor_scales)
-        hfactor_scales = gamma_sample(rng, hfactor_scale_concentration, hfactor_scale_rate)
+        #         log_hfactor_scales = gaussian_sample(rng, hfactor_scale_params[0], hfactor_scale_params[1])
+        #         hfactor_scales = jnp.exp(log_hfactor_scales)
+        hfactor_scales = gamma_sample(
+            rng, hfactor_scale_concentration, hfactor_scale_rate
+        )
         factor_scales = gamma_sample(rng, factor_scale_concentration, factor_scale_rate)
-#         factor_scales = jnp.exp(log_factor_scales)
+        #         factor_scales = jnp.exp(log_factor_scales)
 
         hz = gamma_sample(rng, hz_concentration, hz_rate)
-#         hz = jnp.exp(log_hz)
+        #         hz = jnp.exp(log_hz)
         hW = gamma_sample(rng, hW_concentration, hW_rate)
-#         hW = jnp.exp(log_hW)
-#         hW = jnn.softplus(unconst_hW)
+        #         hW = jnp.exp(log_hW)
+        #         hW = jnn.softplus(unconst_hW)
         mean_top = jnp.matmul(hz, hW)
 
         z = gamma_sample(rng, z_concentration, z_rate)
-#         z = jnp.exp(log_z)
-#         log_z_noise = gaussian_sample(rng, z_noise_params[0][indices], z_noise_params[1][indices])
-#         z_noise = jnp.exp(log_z_noise)
-#         z_noise = gamma_sample(rng, z_noise_concentration, z_noise_rate)
+        #         z = jnp.exp(log_z)
+        #         log_z_noise = gaussian_sample(rng, z_noise_params[0][indices], z_noise_params[1][indices])
+        #         z_noise = jnp.exp(log_z_noise)
+        #         z_noise = gamma_sample(rng, z_noise_concentration, z_noise_rate)
         W = gamma_sample(rng, W_concentration, W_rate)
-#         W = jnp.exp(log_W)
-#         W = jnn.softplus(unconst_W)
-#         W_noise = jnn.softplus(unconst_W_noise)
-#         W_noise = gamma_sample(rng, W_noise_concentration, W_noise_rate)
+        #         W = jnp.exp(log_W)
+        #         W = jnn.softplus(unconst_W)
+        #         W_noise = jnn.softplus(unconst_W_noise)
+        #         W_noise = gamma_sample(rng, W_noise_concentration, W_noise_rate)
         mean_bottom_bio = jnp.matmul(z, W)
-#         mean_bottom_batch = jnp.matmul(batch_indices_onehot * z_noise, W_noise) # jnn.softplus(jnp.matmul(batch_indices_onehot, unconst_W_noise))
-        mean_bottom = mean_bottom_bio #+ mean_bottom_batch
+        #         mean_bottom_batch = jnp.matmul(batch_indices_onehot * z_noise, W_noise) # jnn.softplus(jnp.matmul(batch_indices_onehot, unconst_W_noise))
+        mean_bottom = mean_bottom_bio  # + mean_bottom_batch
 
         # Compute log likelihood
         ll = jnp.sum(vmap(poisson.logpmf)(self.X[indices], mean_bottom))
 
         # Compute KL divergence
-        kl = 0.
+        kl = 0.0
         gene_size = jnp.sum(self.X, axis=0)
-        kl += gamma_logpdf(gene_scales, 1., jnp.mean(gene_size)/jnp.var(gene_size)) -\
-                gamma_logpdf(gene_scales, gene_scale_concentration, gene_scale_rate)
-
-        kl += gamma_logpdf(hfactor_scales, 1e-3, 1e-3) -\
-                gamma_logpdf(hfactor_scales, hfactor_scale_concentration, hfactor_scale_rate)
-
-        kl += gamma_logpdf(factor_scales, 1e-3, 1e-3) -\
-                gamma_logpdf(factor_scales, factor_scale_concentration, factor_scale_rate)
-#         normalized_factor_scales = factor_scales / jnp.sum(factor_scales)
-
-        kl += gamma_logpdf(hW, .3, 1. * hfactor_scales.reshape(-1,1)) -\
-                gamma_logpdf(hW, hW_concentration, hW_rate)
-
-        kl += gamma_logpdf(W, .3, 1 * gene_scales.reshape(1,-1) * factor_scales.reshape(-1,1)) -\
-                gamma_logpdf(W, W_concentration, W_rate)
-
-#         kl += gamma_logpdf(W_noise, 10, 10. * gene_scales.reshape(1,-1)) -\
-#                 gamma_logpdf(W_noise, W_noise_concentration, W_noise_rate)
-
-        kl *= indices.shape[0] / self.X.shape[0] # scale by minibatch size
-
-        kl += gamma_logpdf(cell_scales, 1., 1.*self.batch_lib_ratio[indices]) -\
-                gamma_logpdf(cell_scales, cell_scale_concentration, cell_scale_rate)
-
-        kl += gamma_logpdf(hz, 1.,  1. / hfactor_scales.reshape(1,-1)) -\
-                gamma_logpdf(hz, hz_concentration, hz_rate)
+        kl += gamma_logpdf(
+            gene_scales, 1.0, jnp.mean(gene_size) / jnp.var(gene_size)
+        ) - gamma_logpdf(gene_scales, gene_scale_concentration, gene_scale_rate)
+
+        kl += gamma_logpdf(hfactor_scales, 1e-3, 1e-3) - gamma_logpdf(
+            hfactor_scales, hfactor_scale_concentration, hfactor_scale_rate
+        )
+
+        kl += gamma_logpdf(factor_scales, 1e-3, 1e-3) - gamma_logpdf(
+            factor_scales, factor_scale_concentration, factor_scale_rate
+        )
+        #         normalized_factor_scales = factor_scales / jnp.sum(factor_scales)
+
+        kl += gamma_logpdf(hW, 0.3, 1.0 * hfactor_scales.reshape(-1, 1)) - gamma_logpdf(
+            hW, hW_concentration, hW_rate
+        )
+
+        kl += gamma_logpdf(
+            W, 0.3, 1 * gene_scales.reshape(1, -1) * factor_scales.reshape(-1, 1)
+        ) - gamma_logpdf(W, W_concentration, W_rate)
+
+        #         kl += gamma_logpdf(W_noise, 10, 10. * gene_scales.reshape(1,-1)) -\
+        #                 gamma_logpdf(W_noise, W_noise_concentration, W_noise_rate)
+
+        kl *= indices.shape[0] / self.X.shape[0]  # scale by minibatch size
+
+        kl += gamma_logpdf(
+            cell_scales, 1.0, 1.0 * self.batch_lib_ratio[indices]
+        ) - gamma_logpdf(cell_scales, cell_scale_concentration, cell_scale_rate)
+
+        kl += gamma_logpdf(hz, 1.0, 1.0 / hfactor_scales.reshape(1, -1)) - gamma_logpdf(
+            hz, hz_concentration, hz_rate
+        )
 
         # Tieing the scales avoids the factors with low scales in W learn z's that correlate with cell scales
-        kl += gamma_logpdf(z, self.shape, cell_scales.reshape(-1,1) * self.shape / (factor_scales.reshape(1,-1) * mean_top) ) -\
-                gamma_logpdf(z, z_concentration, z_rate)
+        kl += gamma_logpdf(
+            z,
+            self.shape,
+            cell_scales.reshape(-1, 1)
+            * self.shape
+            / (factor_scales.reshape(1, -1) * mean_top),
+        ) - gamma_logpdf(z, z_concentration, z_rate)
 
-#         kl += gamma_logpdf(z_noise, 10., 10. * cell_scales.reshape(-1,1)) -\
-#                 gamma_logpdf(z_noise, z_noise_concentration, z_noise_rate)
+        #         kl += gamma_logpdf(z_noise, 10., 10. * cell_scales.reshape(-1,1)) -\
+        #                 gamma_logpdf(z_noise, z_noise_concentration, z_noise_rate)
 
         return ll + kl
```

### Comparing `scdef-0.0.1/scdef/models/joint.py` & `scdef-0.0.2/scdef/models/joint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,130 +1,171 @@
 class Joint(scDEF):
     """
     Same cells, two modalities.
     """
+
     def elbo(self, rng, indices, var_params):
         # Single-sample Monte Carlo estimate of the variational lower bound.
         batch_indices_onehot = self.batch_indices_onehot[indices]
 
         min_loc = jnp.log(1e-10)
         cell_scale_params = jnp.clip(var_params[0], a_min=min_loc)
         gene_scale_params = jnp.clip(var_params[1], a_min=min_loc)
-#         unconst_gene_scales = jnp.clip(var_params[1], a_min=min_loc)
+        #         unconst_gene_scales = jnp.clip(var_params[1], a_min=min_loc)
         hfactor_scale_params = jnp.clip(var_params[2], a_min=min_loc)
         factor_scale_params = jnp.clip(var_params[3], a_min=min_loc)
         hz_params = jnp.clip(var_params[4], a_min=min_loc)
         hW_params = jnp.clip(var_params[5], a_min=min_loc)
-#         unconst_hW = jnp.clip(var_params[5], a_min=min_loc)
+        #         unconst_hW = jnp.clip(var_params[5], a_min=min_loc)
         z_params = jnp.clip(var_params[6], a_min=min_loc)
         W_params = jnp.clip(var_params[7], a_min=min_loc)
-#         unconst_W = jnp.clip(var_params[7], a_min=min_loc)
+        #         unconst_W = jnp.clip(var_params[7], a_min=min_loc)
         W_noise_params = jnp.clip(var_params[8], a_min=min_loc)
         z_noise_params = jnp.clip(var_params[9], a_min=min_loc)
 
         min_concentration = 1e-10
         min_scale = 1e-10
-        cell_scale_concentration = jnp.maximum(jnn.softplus(cell_scale_params[0][indices]), min_concentration)
-        cell_scale_rate = 1./jnp.maximum(jnn.softplus(cell_scale_params[1][indices]), min_scale)
-
-        z_concentration = jnp.maximum(jnn.softplus(z_params[0][indices]), min_concentration)
-        z_rate = 1./jnp.maximum(jnn.softplus(z_params[1][indices]), min_scale)
-
-        hz_concentration = jnp.maximum(jnn.softplus(hz_params[0][indices]), min_concentration)
-        hz_rate = 1./jnp.maximum(jnn.softplus(hz_params[1][indices]), min_scale)
-
-        gene_scale_concentration = jnp.maximum(jnn.softplus(gene_scale_params[0]), min_concentration)
-        gene_scale_rate = 1./jnp.maximum(jnn.softplus(gene_scale_params[1]), min_scale)
-
-        hfactor_scale_concentration = jnp.maximum(jnn.softplus(hfactor_scale_params[0]), min_concentration)
-        hfactor_scale_rate = 1./jnp.maximum(jnn.softplus(hfactor_scale_params[1]), min_scale)
-
-        factor_scale_concentration = jnp.maximum(jnn.softplus(factor_scale_params[0]), min_concentration)
-        factor_scale_rate = 1./jnp.maximum(jnn.softplus(factor_scale_params[1]), min_scale)
+        cell_scale_concentration = jnp.maximum(
+            jnn.softplus(cell_scale_params[0][indices]), min_concentration
+        )
+        cell_scale_rate = 1.0 / jnp.maximum(
+            jnn.softplus(cell_scale_params[1][indices]), min_scale
+        )
+
+        z_concentration = jnp.maximum(
+            jnn.softplus(z_params[0][indices]), min_concentration
+        )
+        z_rate = 1.0 / jnp.maximum(jnn.softplus(z_params[1][indices]), min_scale)
+
+        hz_concentration = jnp.maximum(
+            jnn.softplus(hz_params[0][indices]), min_concentration
+        )
+        hz_rate = 1.0 / jnp.maximum(jnn.softplus(hz_params[1][indices]), min_scale)
+
+        gene_scale_concentration = jnp.maximum(
+            jnn.softplus(gene_scale_params[0]), min_concentration
+        )
+        gene_scale_rate = 1.0 / jnp.maximum(
+            jnn.softplus(gene_scale_params[1]), min_scale
+        )
+
+        hfactor_scale_concentration = jnp.maximum(
+            jnn.softplus(hfactor_scale_params[0]), min_concentration
+        )
+        hfactor_scale_rate = 1.0 / jnp.maximum(
+            jnn.softplus(hfactor_scale_params[1]), min_scale
+        )
+
+        factor_scale_concentration = jnp.maximum(
+            jnn.softplus(factor_scale_params[0]), min_concentration
+        )
+        factor_scale_rate = 1.0 / jnp.maximum(
+            jnn.softplus(factor_scale_params[1]), min_scale
+        )
 
         W_concentration = jnp.maximum(jnn.softplus(W_params[0]), min_concentration)
-        W_rate = 1./jnp.maximum(jnn.softplus(W_params[1]), min_scale)
+        W_rate = 1.0 / jnp.maximum(jnn.softplus(W_params[1]), min_scale)
 
         hW_concentration = jnp.maximum(jnn.softplus(hW_params[0]), min_concentration)
-        hW_rate = 1./jnp.maximum(jnn.softplus(hW_params[1]), min_scale)
+        hW_rate = 1.0 / jnp.maximum(jnn.softplus(hW_params[1]), min_scale)
 
-        z_noise_concentration = jnp.maximum(jnn.softplus(z_noise_params[0][indices]), min_concentration)
-        z_noise_rate = 1./jnp.maximum(jnn.softplus(z_noise_params[1][indices]), min_scale)
-
-        W_noise_concentration = jnp.maximum(jnn.softplus(W_noise_params[0]), min_concentration)
-        W_noise_rate = 1./jnp.maximum(jnn.softplus(W_noise_params[1]), min_scale)
+        z_noise_concentration = jnp.maximum(
+            jnn.softplus(z_noise_params[0][indices]), min_concentration
+        )
+        z_noise_rate = 1.0 / jnp.maximum(
+            jnn.softplus(z_noise_params[1][indices]), min_scale
+        )
+
+        W_noise_concentration = jnp.maximum(
+            jnn.softplus(W_noise_params[0]), min_concentration
+        )
+        W_noise_rate = 1.0 / jnp.maximum(jnn.softplus(W_noise_params[1]), min_scale)
 
         # Sample from variational distribution
         cell_scales = gamma_sample(rng, cell_scale_concentration, cell_scale_rate)
-#         cell_scales = jnp.exp(log_cell_scales)
+        #         cell_scales = jnp.exp(log_cell_scales)
         gene_scales = gamma_sample(rng, gene_scale_concentration, gene_scale_rate)
-#         gene_scales = jnp.exp(log_gene_scales)
-#         gene_scales = jnn.softplus(unconst_gene_scales)
+        #         gene_scales = jnp.exp(log_gene_scales)
+        #         gene_scales = jnn.softplus(unconst_gene_scales)
 
-#         log_hfactor_scales = gaussian_sample(rng, hfactor_scale_params[0], hfactor_scale_params[1])
-#         hfactor_scales = jnp.exp(log_hfactor_scales)
-        hfactor_scales = gamma_sample(rng, hfactor_scale_concentration, hfactor_scale_rate)
+        #         log_hfactor_scales = gaussian_sample(rng, hfactor_scale_params[0], hfactor_scale_params[1])
+        #         hfactor_scales = jnp.exp(log_hfactor_scales)
+        hfactor_scales = gamma_sample(
+            rng, hfactor_scale_concentration, hfactor_scale_rate
+        )
         factor_scales = gamma_sample(rng, factor_scale_concentration, factor_scale_rate)
-#         factor_scales = jnp.exp(log_factor_scales)
+        #         factor_scales = jnp.exp(log_factor_scales)
 
         hz = gamma_sample(rng, hz_concentration, hz_rate)
-#         hz = jnp.exp(log_hz)
+        #         hz = jnp.exp(log_hz)
         hW = gamma_sample(rng, hW_concentration, hW_rate)
-#         hW = jnp.exp(log_hW)
-#         hW = jnn.softplus(unconst_hW)
+        #         hW = jnp.exp(log_hW)
+        #         hW = jnn.softplus(unconst_hW)
         mean_top = jnp.matmul(hz, hW)
 
         z = gamma_sample(rng, z_concentration, z_rate)
-#         z = jnp.exp(log_z)
-#         log_z_noise = gaussian_sample(rng, z_noise_params[0][indices], z_noise_params[1][indices])
-#         z_noise = jnp.exp(log_z_noise)
-#         z_noise = gamma_sample(rng, z_noise_concentration, z_noise_rate)
+        #         z = jnp.exp(log_z)
+        #         log_z_noise = gaussian_sample(rng, z_noise_params[0][indices], z_noise_params[1][indices])
+        #         z_noise = jnp.exp(log_z_noise)
+        #         z_noise = gamma_sample(rng, z_noise_concentration, z_noise_rate)
         W = gamma_sample(rng, W_concentration, W_rate)
-#         W = jnp.exp(log_W)
-#         W = jnn.softplus(unconst_W)
-#         W_noise = jnn.softplus(unconst_W_noise)
-#         W_noise = gamma_sample(rng, W_noise_concentration, W_noise_rate)
+        #         W = jnp.exp(log_W)
+        #         W = jnn.softplus(unconst_W)
+        #         W_noise = jnn.softplus(unconst_W_noise)
+        #         W_noise = gamma_sample(rng, W_noise_concentration, W_noise_rate)
         mean_bottom_bio = jnp.matmul(z, W)
-#         mean_bottom_batch = jnp.matmul(batch_indices_onehot * z_noise, W_noise) # jnn.softplus(jnp.matmul(batch_indices_onehot, unconst_W_noise))
-        mean_bottom = mean_bottom_bio #+ mean_bottom_batch
+        #         mean_bottom_batch = jnp.matmul(batch_indices_onehot * z_noise, W_noise) # jnn.softplus(jnp.matmul(batch_indices_onehot, unconst_W_noise))
+        mean_bottom = mean_bottom_bio  # + mean_bottom_batch
 
         # Compute log likelihood
         ll = jnp.sum(vmap(poisson.logpmf)(self.X[indices], mean_bottom))
 
         # Compute KL divergence
-        kl = 0.
+        kl = 0.0
         gene_size = jnp.sum(self.X, axis=0)
-        kl += gamma_logpdf(gene_scales, 1., jnp.mean(gene_size)/jnp.var(gene_size)) -\
-                gamma_logpdf(gene_scales, gene_scale_concentration, gene_scale_rate)
-
-        kl += gamma_logpdf(hfactor_scales, 1e-3, 1e-3) -\
-                gamma_logpdf(hfactor_scales, hfactor_scale_concentration, hfactor_scale_rate)
-
-        kl += gamma_logpdf(factor_scales, 1e-3, 1e-3) -\
-                gamma_logpdf(factor_scales, factor_scale_concentration, factor_scale_rate)
-#         normalized_factor_scales = factor_scales / jnp.sum(factor_scales)
-
-        kl += gamma_logpdf(hW, .3, 1. * hfactor_scales.reshape(-1,1)) -\
-                gamma_logpdf(hW, hW_concentration, hW_rate)
-
-        kl += gamma_logpdf(W, .3, 1 * gene_scales.reshape(1,-1) * factor_scales.reshape(-1,1)) -\
-                gamma_logpdf(W, W_concentration, W_rate)
-
-#         kl += gamma_logpdf(W_noise, 10, 10. * gene_scales.reshape(1,-1)) -\
-#                 gamma_logpdf(W_noise, W_noise_concentration, W_noise_rate)
-
-        kl *= indices.shape[0] / self.X.shape[0] # scale by minibatch size
-
-        kl += gamma_logpdf(cell_scales, 1., 1.*self.batch_lib_ratio[indices]) -\
-                gamma_logpdf(cell_scales, cell_scale_concentration, cell_scale_rate)
-
-        kl += gamma_logpdf(hz, 1.,  1. / hfactor_scales.reshape(1,-1)) -\
-                gamma_logpdf(hz, hz_concentration, hz_rate)
+        kl += gamma_logpdf(
+            gene_scales, 1.0, jnp.mean(gene_size) / jnp.var(gene_size)
+        ) - gamma_logpdf(gene_scales, gene_scale_concentration, gene_scale_rate)
+
+        kl += gamma_logpdf(hfactor_scales, 1e-3, 1e-3) - gamma_logpdf(
+            hfactor_scales, hfactor_scale_concentration, hfactor_scale_rate
+        )
+
+        kl += gamma_logpdf(factor_scales, 1e-3, 1e-3) - gamma_logpdf(
+            factor_scales, factor_scale_concentration, factor_scale_rate
+        )
+        #         normalized_factor_scales = factor_scales / jnp.sum(factor_scales)
+
+        kl += gamma_logpdf(hW, 0.3, 1.0 * hfactor_scales.reshape(-1, 1)) - gamma_logpdf(
+            hW, hW_concentration, hW_rate
+        )
+
+        kl += gamma_logpdf(
+            W, 0.3, 1 * gene_scales.reshape(1, -1) * factor_scales.reshape(-1, 1)
+        ) - gamma_logpdf(W, W_concentration, W_rate)
+
+        #         kl += gamma_logpdf(W_noise, 10, 10. * gene_scales.reshape(1,-1)) -\
+        #                 gamma_logpdf(W_noise, W_noise_concentration, W_noise_rate)
+
+        kl *= indices.shape[0] / self.X.shape[0]  # scale by minibatch size
+
+        kl += gamma_logpdf(
+            cell_scales, 1.0, 1.0 * self.batch_lib_ratio[indices]
+        ) - gamma_logpdf(cell_scales, cell_scale_concentration, cell_scale_rate)
+
+        kl += gamma_logpdf(hz, 1.0, 1.0 / hfactor_scales.reshape(1, -1)) - gamma_logpdf(
+            hz, hz_concentration, hz_rate
+        )
 
         # Tieing the scales avoids the factors with low scales in W learn z's that correlate with cell scales
-        kl += gamma_logpdf(z, self.shape, cell_scales.reshape(-1,1) * self.shape / (factor_scales.reshape(1,-1) * mean_top) ) -\
-                gamma_logpdf(z, z_concentration, z_rate)
+        kl += gamma_logpdf(
+            z,
+            self.shape,
+            cell_scales.reshape(-1, 1)
+            * self.shape
+            / (factor_scales.reshape(1, -1) * mean_top),
+        ) - gamma_logpdf(z, z_concentration, z_rate)
 
-#         kl += gamma_logpdf(z_noise, 10., 10. * cell_scales.reshape(-1,1)) -\
-#                 gamma_logpdf(z_noise, z_noise_concentration, z_noise_rate)
+        #         kl += gamma_logpdf(z_noise, 10., 10. * cell_scales.reshape(-1,1)) -\
+        #                 gamma_logpdf(z_noise, z_noise_concentration, z_noise_rate)
 
         return ll + kl
```

### Comparing `scdef-0.0.1/scdef/models/spatial.py` & `scdef-0.0.2/scdef/models/spatial.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,420 +10,508 @@
 from os import path
 from math import ceil
 from tensorflow import linalg as tfl
 from sklearn.decomposition import TruncatedSVD
 from sklearn.linear_model import LinearRegression
 from sklearn.neighbors import KNeighborsRegressor
 
-from spatial_factorization import likelihoods,misc,nnfu
+from spatial_factorization import likelihoods, misc, nnfu
+
 tfd = tfp.distributions
 tfb = tfp.bijectors
 tv = tfp.util.TransformedVariable
 tfk = tfp.math.psd_kernels
 
 dtp = "float32"
 rng = np.random.default_rng()
 
-class SpatialDEF(object):
-  def __init__(self, J, L, Z, lik="poi", psd_kernel=tfk.MaternThreeHalves,
-               nugget=1e-5, length_scale=0.1, disp="default",
-               nonneg=False, isotropic=True, feature_means=None, **kwargs):
-    """
-    Non-negative process factorization
-    Parameters
-    ----------
-    J : integer scalar
-        Number of features in the multivariate outcome.
-    L : integer scalar
-        Number of desired latent Gaussian processes.
-    T : integer scalar
-        Number of desired non-spatial latent factors
-    Z : 2D numpy array
-        Coordinates of inducing point locations in input space.
-        First dimension: 'M' is number of inducing points.
-        Second dimension: 'D' is dimensionality of input to GP.
-        More inducing points= slower but more accurate inference.
-    lik: likelihood (Poisson or Gaussian)
-    disp: overdispersion parameter initialization.
-    --for Gaussian likelihood, the scale (stdev) parameter
-    --for negative binomial likelihood, the parameter phi such that
-      var=mean+phi*mean^2, i.e. phi->0 corresponds to Poisson, phi=1 to geometric
-    --for Poisson likelihood, this parameter is ignored and set to None
-    psd_kernel : an object of class PositiveSemidefiniteKernel, must accept a
-        length_scale parameter.
-    feature_means : if input data is centered (for lik='gau', nonneg=False)
-    """
-    super().__init__(**kwargs)
-    # self.is_spatial=True
-    self.lik = lik
-    self.isotropic=isotropic
-    M,D = Z.shape
-    self.Z = tf.Variable(Z, trainable=False, dtype=dtp, name="inducing_points")
-    self.nonneg = tf.Variable(nonneg, trainable=False, name="is_non_negative")
-    #variational parameters
-    with tf.name_scope("variational"):
-      self.delta = tf.Variable(rng.normal(size=(L,M)), dtype=dtp, name="mean") #LxM
-      _Omega_tril = self._init_Omega_tril(L,M,nugget=nugget)
-      # _Omega_tril = .01*tf.eye(M,batch_shape=[L],dtype=dtp)
-      self.Omega_tril=tv(_Omega_tril, tfb.FillScaleTriL(), dtype=dtp, name="covar_tril") #LxMxM
-    #GP hyperparameters
-    with tf.name_scope("gp_mean"):
-      if self.nonneg:
-        prior_mu, prior_sigma = misc.lnormal_approx_dirichlet(max(L,1.1))
-        self.beta0 = tf.Variable(prior_mu*tf.ones((L,1)), dtype=dtp,
-                                 name="intercepts")
-      else:
-        self.beta0 = tf.Variable(tf.zeros((L,1)), dtype=dtp, name="intercepts") #L
-      self.beta = tf.Variable(tf.zeros((L,D)), dtype=dtp, name="slopes") #LxD
-    with tf.name_scope("gp_kernel"):
-      self.nugget = tf.Variable(nugget, dtype=dtp, trainable=False, name="nugget")
-      self.amplitude = tv(np.tile(1.0,[L]), tfb.Softplus(), dtype=dtp, name="amplitude")
-      self._ls0 = length_scale #store for .reset() method
-      if self.isotropic:
-        self.length_scale = tv(np.tile(self._ls0,[L]), tfb.Softplus(),
-                               dtype=dtp, name="length_scale")
-      else:
-        self.scale_diag = tv(np.tile(np.sqrt(self._ls0),[L,D]),
-                             tfb.Softplus(), dtype=dtp, name="scale_diag")
-    #Loadings weights
-    if self.nonneg:
-      self.W = tf.Variable(rng.exponential(size=(J,L)), dtype=dtp,
-                           constraint=misc.make_nonneg, name="loadings") #JxL
-    else:
-      self.W = tf.Variable(rng.normal(size=(J,L)), dtype=dtp, name="loadings") #JxL
-    self.psd_kernel = psd_kernel #this is a class, not yet an object
-    #likelihood parameters, set defaults
-    self._disp0 = disp
-    self._init_misc()
-    self.Kuu_chol = tf.Variable(self.eval_Kuu_chol(self.get_kernel()), dtype=dtp, trainable=False)
-    if self.lik=="gau" and not self.nonneg:
-      self.feature_means = feature_means
-    else:
-      self.feature_means = None
-
-  @staticmethod
-  def _init_Omega_tril(L, M, nugget=None):
-    """
-    convenience function for initializing the batch of lower triangular
-    cholesky factors of the variational covariance matrices.
-    L: number of latent dimensions (factors)
-    M: number of inducing points
-    """
-    #note most of these operations are in float64 by default
-    #the 0.01 below is to make the elbo more numerically stable at initialization
-    Omega_sqt = 0.01*rng.normal(size=(L,M,M)) #LxMxM
-    Omega = [Omega_sqt[l,:,:]@ Omega_sqt[l,:,:].T for l in range(L)] #list len L, elements MxM
-    # Omega += nugget*np.eye(M)
-    res = np.stack([np.linalg.cholesky(Omega[l]) for l in range(L)], axis=0)
-    return res.astype(dtp)
-
-  def _init_misc(self):
-    """
-    misc initialization shared between __init__ and reset
-    """
-    J = self.W.shape[0]
-    self.disp = likelihoods.init_lik(self.lik, J, disp=self._disp0, dtp=dtp)
-    #stuff to facilitate caching
-    self.trvars_kernel = tuple(i for i in self.trainable_variables if i.name[:10]=="gp_kernel/")
-    self.trvars_nonkernel = tuple(i for i in self.trainable_variables if i.name[:10]!="gp_kernel/")
-    if self.isotropic:
-      self.kernel = self.psd_kernel(amplitude=self.amplitude, length_scale=self.length_scale)
-    else:
-      self.kernel = tfk.FeatureScaled(self.psd_kernel(amplitude=self.amplitude), self.scale_diag)
-
-  def get_dims(self):
-    return self.W.shape[1]
-
-  def get_loadings(self):
-    return self.W.numpy()
-
-  def set_loadings(self,Wnew):
-    self.W.assign(Wnew,read_value=False)
 
-  def init_loadings(self,Y,X=None,sz=1,**kwargs):
-    """
-    Use either PCA or NMF to initialize the loadings matrix from data Y
-    """
-    if self.nonneg:
-      init_nsf_with_nmf(self,Y,X=X,sz=sz,**kwargs)
-    else: #real-valued factors
-      if self.lik in ("poi","nb"):
-        pass #use GLM-PCA?
-      elif self.lik=="gau":
+class SpatialDEF(object):
+    def __init__(
+        self,
+        J,
+        L,
+        Z,
+        lik="poi",
+        psd_kernel=tfk.MaternThreeHalves,
+        nugget=1e-5,
+        length_scale=0.1,
+        disp="default",
+        nonneg=False,
+        isotropic=True,
+        feature_means=None,
+        **kwargs
+    ):
+        """
+        Non-negative process factorization
+        Parameters
+        ----------
+        J : integer scalar
+            Number of features in the multivariate outcome.
+        L : integer scalar
+            Number of desired latent Gaussian processes.
+        T : integer scalar
+            Number of desired non-spatial latent factors
+        Z : 2D numpy array
+            Coordinates of inducing point locations in input space.
+            First dimension: 'M' is number of inducing points.
+            Second dimension: 'D' is dimensionality of input to GP.
+            More inducing points= slower but more accurate inference.
+        lik: likelihood (Poisson or Gaussian)
+        disp: overdispersion parameter initialization.
+        --for Gaussian likelihood, the scale (stdev) parameter
+        --for negative binomial likelihood, the parameter phi such that
+          var=mean+phi*mean^2, i.e. phi->0 corresponds to Poisson, phi=1 to geometric
+        --for Poisson likelihood, this parameter is ignored and set to None
+        psd_kernel : an object of class PositiveSemidefiniteKernel, must accept a
+            length_scale parameter.
+        feature_means : if input data is centered (for lik='gau', nonneg=False)
+        """
+        super().__init__(**kwargs)
+        # self.is_spatial=True
+        self.lik = lik
+        self.isotropic = isotropic
+        M, D = Z.shape
+        self.Z = tf.Variable(Z, trainable=False, dtype=dtp, name="inducing_points")
+        self.nonneg = tf.Variable(nonneg, trainable=False, name="is_non_negative")
+        # variational parameters
+        with tf.name_scope("variational"):
+            self.delta = tf.Variable(
+                rng.normal(size=(L, M)), dtype=dtp, name="mean"
+            )  # LxM
+            _Omega_tril = self._init_Omega_tril(L, M, nugget=nugget)
+            # _Omega_tril = .01*tf.eye(M,batch_shape=[L],dtype=dtp)
+            self.Omega_tril = tv(
+                _Omega_tril, tfb.FillScaleTriL(), dtype=dtp, name="covar_tril"
+            )  # LxMxM
+        # GP hyperparameters
+        with tf.name_scope("gp_mean"):
+            if self.nonneg:
+                prior_mu, prior_sigma = misc.lnormal_approx_dirichlet(max(L, 1.1))
+                self.beta0 = tf.Variable(
+                    prior_mu * tf.ones((L, 1)), dtype=dtp, name="intercepts"
+                )
+            else:
+                self.beta0 = tf.Variable(
+                    tf.zeros((L, 1)), dtype=dtp, name="intercepts"
+                )  # L
+            self.beta = tf.Variable(tf.zeros((L, D)), dtype=dtp, name="slopes")  # LxD
+        with tf.name_scope("gp_kernel"):
+            self.nugget = tf.Variable(nugget, dtype=dtp, trainable=False, name="nugget")
+            self.amplitude = tv(
+                np.tile(1.0, [L]), tfb.Softplus(), dtype=dtp, name="amplitude"
+            )
+            self._ls0 = length_scale  # store for .reset() method
+            if self.isotropic:
+                self.length_scale = tv(
+                    np.tile(self._ls0, [L]),
+                    tfb.Softplus(),
+                    dtype=dtp,
+                    name="length_scale",
+                )
+            else:
+                self.scale_diag = tv(
+                    np.tile(np.sqrt(self._ls0), [L, D]),
+                    tfb.Softplus(),
+                    dtype=dtp,
+                    name="scale_diag",
+                )
+        # Loadings weights
+        if self.nonneg:
+            self.W = tf.Variable(
+                rng.exponential(size=(J, L)),
+                dtype=dtp,
+                constraint=misc.make_nonneg,
+                name="loadings",
+            )  # JxL
+        else:
+            self.W = tf.Variable(
+                rng.normal(size=(J, L)), dtype=dtp, name="loadings"
+            )  # JxL
+        self.psd_kernel = psd_kernel  # this is a class, not yet an object
+        # likelihood parameters, set defaults
+        self._disp0 = disp
+        self._init_misc()
+        self.Kuu_chol = tf.Variable(
+            self.eval_Kuu_chol(self.get_kernel()), dtype=dtp, trainable=False
+        )
+        if self.lik == "gau" and not self.nonneg:
+            self.feature_means = feature_means
+        else:
+            self.feature_means = None
+
+    @staticmethod
+    def _init_Omega_tril(L, M, nugget=None):
+        """
+        convenience function for initializing the batch of lower triangular
+        cholesky factors of the variational covariance matrices.
+        L: number of latent dimensions (factors)
+        M: number of inducing points
+        """
+        # note most of these operations are in float64 by default
+        # the 0.01 below is to make the elbo more numerically stable at initialization
+        Omega_sqt = 0.01 * rng.normal(size=(L, M, M))  # LxMxM
+        Omega = [
+            Omega_sqt[l, :, :] @ Omega_sqt[l, :, :].T for l in range(L)
+        ]  # list len L, elements MxM
+        # Omega += nugget*np.eye(M)
+        res = np.stack([np.linalg.cholesky(Omega[l]) for l in range(L)], axis=0)
+        return res.astype(dtp)
+
+    def _init_misc(self):
+        """
+        misc initialization shared between __init__ and reset
+        """
+        J = self.W.shape[0]
+        self.disp = likelihoods.init_lik(self.lik, J, disp=self._disp0, dtp=dtp)
+        # stuff to facilitate caching
+        self.trvars_kernel = tuple(
+            i for i in self.trainable_variables if i.name[:10] == "gp_kernel/"
+        )
+        self.trvars_nonkernel = tuple(
+            i for i in self.trainable_variables if i.name[:10] != "gp_kernel/"
+        )
+        if self.isotropic:
+            self.kernel = self.psd_kernel(
+                amplitude=self.amplitude, length_scale=self.length_scale
+            )
+        else:
+            self.kernel = tfk.FeatureScaled(
+                self.psd_kernel(amplitude=self.amplitude), self.scale_diag
+            )
+
+    def get_dims(self):
+        return self.W.shape[1]
+
+    def get_loadings(self):
+        return self.W.numpy()
+
+    def set_loadings(self, Wnew):
+        self.W.assign(Wnew, read_value=False)
+
+    def init_loadings(self, Y, X=None, sz=1, **kwargs):
+        """
+        Use either PCA or NMF to initialize the loadings matrix from data Y
+        """
+        if self.nonneg:
+            init_nsf_with_nmf(self, Y, X=X, sz=sz, **kwargs)
+        else:  # real-valued factors
+            if self.lik in ("poi", "nb"):
+                pass  # use GLM-PCA?
+            elif self.lik == "gau":
+                L = self.W.shape[1]
+                fit = TruncatedSVD(L).fit(Y)
+                self.set_loadings(fit.components_.T)
+            else:
+                raise likelihoods.InvalidLikelihoodError
+
+    def generate_pickle_path(self, sz, base=None):
+        """
+        sz : str
+          Indicate what type of size factors are used (eg 'none' or 'scanpy').
+        base : str, optional
+          Parent directory for saving pickle files. The default is cwd.
+        """
+        pars = {
+            "L": self.W.shape[1],
+            "lik": self.lik,
+            "sz": sz,
+            "model": "NSF" if self.nonneg else "RSF",
+            "kernel": self.psd_kernel.__name__,
+            "M": self.Z.shape[0],
+        }
+        pth = misc.params2key(pars)
+        if base:
+            pth = path.join(base, pth)
+        return pth
+
+    def get_kernel(self):
+        return self.kernel
+
+    def eval_Kuu_chol(self, kernel=None):
+        if kernel is None:
+            kernel = self.get_kernel()
+        M, D = self.Z.shape
+        Kuu = kernel.matrix(self.Z, self.Z) + self.nugget * tf.eye(M)
+        # Kuu_chol is LxMxM and lower triangular in last two dims
+        return tfl.cholesky(Kuu)
+
+    def get_Kuu_chol(self, kernel=None, from_cache=False):
+        if not from_cache:
+            Kuu_chol = self.eval_Kuu_chol(kernel=kernel)
+            self.Kuu_chol.assign(Kuu_chol)  # update cache
+            return Kuu_chol
+        else:  # use cached variable, gradients cannot propagate to kernel hps
+            return self.Kuu_chol
+
+    def get_mu_z(self):
+        return self.beta0 + tfl.matmul(self.beta, self.Z, transpose_b=True)  # LxM
+
+    def sample_latent_GP_funcs(
+        self, X, S=1, kernel=None, mu_z=None, Kuu_chol=None, chol=True
+    ):
+        """
+        Draw random samples of the latent variational GP function values "F"
+        based on spatial coordinates X.
+        The sampling comes from the variational approximation to the posterior.
+        This function is needed to compute the expected log-likelihood term of the
+        ELBO.
+        X is a numpy array with shape NxD
+        N=number of observations
+        D=number of spatial dimensions
+        The first dimension can be observations from a minibatch.
+        S is the number of random samples to draw from latent GPs
+        logscale: if False the function vals are exponentiated before returning
+        i.e. they are positive valued random functions.
+        If logscale=True (default), the functions are real-valued
+        """
+        if kernel is None:
+            kernel = self.get_kernel()
+        if mu_z is None:
+            mu_z = self.get_mu_z()
+        if Kuu_chol is None:
+            Kuu_chol = self.get_Kuu_chol(kernel=kernel, from_cache=(not chol))
+        N = X.shape[0]
         L = self.W.shape[1]
-        fit = TruncatedSVD(L).fit(Y)
-        self.set_loadings(fit.components_.T)
-      else:
-        raise likelihoods.InvalidLikelihoodError
-
-  def generate_pickle_path(self,sz,base=None):
-    """
-    sz : str
-      Indicate what type of size factors are used (eg 'none' or 'scanpy').
-    base : str, optional
-      Parent directory for saving pickle files. The default is cwd.
-    """
-    pars = {"L":self.W.shape[1], "lik":self.lik, "sz":sz,
-            "model":"NSF" if self.nonneg else "RSF",
-            "kernel":self.psd_kernel.__name__,
-            "M":self.Z.shape[0]
-            }
-    pth = misc.params2key(pars)
-    if base: pth = path.join(base,pth)
-    return pth
-
-  def get_kernel(self):
-    return self.kernel
-
-  def eval_Kuu_chol(self, kernel=None):
-    if kernel is None:
-      kernel = self.get_kernel()
-    M,D = self.Z.shape
-    Kuu = kernel.matrix(self.Z, self.Z) + self.nugget*tf.eye(M)
-    #Kuu_chol is LxMxM and lower triangular in last two dims
-    return tfl.cholesky(Kuu)
-
-  def get_Kuu_chol(self, kernel=None, from_cache=False):
-    if not from_cache:
-      Kuu_chol = self.eval_Kuu_chol(kernel=kernel)
-      self.Kuu_chol.assign(Kuu_chol) #update cache
-      return Kuu_chol
-    else: #use cached variable, gradients cannot propagate to kernel hps
-      return self.Kuu_chol
-
-  def get_mu_z(self):
-    return self.beta0+tfl.matmul(self.beta, self.Z, transpose_b=True) #LxM
-
-  def sample_latent_GP_funcs(self, X, S=1, kernel=None, mu_z=None, Kuu_chol=None, chol=True):
-    """
-    Draw random samples of the latent variational GP function values "F"
-    based on spatial coordinates X.
-    The sampling comes from the variational approximation to the posterior.
-    This function is needed to compute the expected log-likelihood term of the
-    ELBO.
-    X is a numpy array with shape NxD
-    N=number of observations
-    D=number of spatial dimensions
-    The first dimension can be observations from a minibatch.
-    S is the number of random samples to draw from latent GPs
-    logscale: if False the function vals are exponentiated before returning
-    i.e. they are positive valued random functions.
-    If logscale=True (default), the functions are real-valued
-    """
-    if kernel is None:
-      kernel = self.get_kernel()
-    if mu_z is None:
-      mu_z = self.get_mu_z()
-    if Kuu_chol is None:
-      Kuu_chol = self.get_Kuu_chol(kernel=kernel, from_cache=(not chol))
-    N = X.shape[0]
-    L = self.W.shape[1]
-    mu_x = self.beta0+tfl.matmul(self.beta, X, transpose_b=True) #LxN
-    Kuf = kernel.matrix(self.Z, X) #LxMxN
-    Kff_diag = kernel.apply(X, X, example_ndims=1)+self.nugget #LxN
-    alpha_x = tfl.cholesky_solve(Kuu_chol, Kuf) #LxMxN
-    mu_tilde = mu_x + tfl.matvec(alpha_x, self.delta-mu_z, transpose_a=True) #LxN
-    #compute the alpha(x_i)'(K_uu-Omega)alpha(x_i) term
-    a_t_Kchol = tfl.matmul(alpha_x, Kuu_chol, transpose_a=True) #LxNxM
-    aKa = tf.reduce_sum(tf.square(a_t_Kchol), axis=2) #LxN
-    a_t_Omega_tril = tfl.matmul(alpha_x, self.Omega_tril, transpose_a=True) #LxNxM
-    aOmega_a = tf.reduce_sum(tf.square(a_t_Omega_tril), axis=2) #LxN
-    Sigma_tilde = Kff_diag - aKa + aOmega_a #LxN
-    eps = tf.random.normal((S,L,N)) #note this is not the same random generator as self.rng!
-    return mu_tilde + tf.math.sqrt(Sigma_tilde)*eps #"F", dims: SxLxN
-
-  def sample_predictive_mean(self, X, sz=1, S=1, kernel=None, mu_z=None, Kuu_chol=None, chol=True):
-    """
-    See sample_latent_variational_GP_funcs for X,S definitions
-    sz is a tensor of shape (N,1) of size factors.
-    Typically sz would be the rowSums or rowMeans of the outcome matrix Y.
-    """
-    F = self.sample_latent_GP_funcs(X, S=S, kernel=kernel, mu_z=mu_z,
-                                    Kuu_chol=Kuu_chol, chol=chol) #SxLxN
-    if self.nonneg:
-      Lam = tfl.matrix_transpose(tfl.matmul(self.W, tf.exp(F))) #SxNxJ
-      if self.lik=="gau":
-        return Lam
-      else:
-        return sz*Lam
-    else:
-      Lam = tfl.matrix_transpose(tfl.matmul(self.W, F))
-      if self.lik=="gau": #identity link
-        return Lam
-      else: #log link (poi, nb)
-        return tf.exp(tf.math.log(sz)+Lam)
-
-  def eval_kl_term(self, mu_z, Kuu_chol):
-    """
-    KL divergence from the prior distribution to the variational distribution.
-    This is one component of the ELBO:
-    ELBO=expected log-likelihood - sum(kl_terms)
-    qpars: a tuple containing (mu_z,Kuu_chol)
-    qpars can be obtained by calling self.get_variational_params()
-    mu_z is the GP mean function at all inducing points (dimension: LxM)
-    Kuu_chol is the cholesky lower triangular of the kernel matrix of all inducing points.
-    Its dimension is LxMxM
-    where L = number of latent dimensions and M = number of inducing points.
-    """
-    qu = tfd.MultivariateNormalTriL(loc=self.delta, scale_tril=self.Omega_tril)
-    pu = tfd.MultivariateNormalTriL(loc=mu_z, scale_tril=Kuu_chol)
-    return qu.kl_divergence(pu) #L-vector
-
-  # @tf.function
-  def elbo_avg(self, X, Y, sz=1, S=1, Ntot=None, chol=True):
-    """
-    Parameters
-    ----------
-    X : numpy array of spatial coordinates (NxD)
-        **OR** a tuple of spatial coordinates, multivariate outcomes,
-        and size factors (convenient for minibatches from tensor slices)
-    Y : numpy array of multivariate outcomes (NxJ)
-        If Y is None then X must be a tuple of length three
-    sz : size factors, optional
-        vector of length N, typically the rowSums or rowMeans of Y.
-        If X is a tuple then this is ignored as sz is expected in the third
-        element of the X tuple.
-    S : integer, optional
-        Number of random GP function evaluations to use. The default is 1.
-        Larger S=more accurate approximation to true ELBO but slower
-    Ntot : total number of observations in full dataset
-        This is needed when X,Y,sz are a minibatch from the full data
-        If Ntot is None, we assume X,Y,sz provided are the full data NOT a minibatch.
-    Returns
-    -------
-    The numeric evidence lower bound value, divided by Ntot.
-    """
-    batch_size, J = Y.shape
-    if Ntot is None: Ntot = batch_size #no minibatch, all observations provided
-    ker = self.get_kernel()
-    mu_z = self.get_mu_z()
-    Kuu_chol = self.get_Kuu_chol(kernel=ker,from_cache=(not chol))
-    #kl_terms is not affected by minibatching so use reduce_sum
-    kl_term = tf.reduce_sum(self.eval_kl_term(mu_z, Kuu_chol))
-    # Sample z1
-    z1 = self.sample_predictive_mean(X, sz=sz, S=S, kernel=ker, mu_z=mu_z, Kuu_chol=Kuu_chol)
-    # Compute p(z0|z1) using sampled z1 and z0
-    mean_top = jnp.exp(z1).dot(W1)
-    # Sample z0
-    z0 = gamma_sample(var_shape_z0, var_rate_z0)
-    prior_z0 = gamma_logpdf(z0, alpha, alpha / mean_top)
-    # And entropy of z0
-    ent_z0 = -gamma_logpdf(z0, var_shape_z0, var_rate_z0)
-    kl_term = kl_term + prior_z0 + ent_z0
-    # Compute p(y|z0)
-    mean_bottom = z0.dot(W0)
-    eloglik = poisson_logpdf()
-    eloglik = likelihoods.lik_to_distr(self.lik, Mu, self.disp).log_prob(Y)
-    return J*tf.reduce_mean(eloglik) - kl_term/Ntot
-
-  def train_step(self, D, optimizer, optimizer_k, S=1, Ntot=None, chol=True):
-    """
-    Executes one training step and returns the loss.
-    D is training data: a tensorflow dataset (from slices) of (X,Y,sz)
-    This function computes the loss and gradients, and uses the latter to
-    update the model's parameters.
-    """
-    with tf.GradientTape(persistent=True) as tape:
-      loss = -self.elbo_avg(D["X"], D["Y"], sz=D["sz"], S=S, Ntot=Ntot, chol=chol)
-    try:
-      gradients = tape.gradient(loss, self.trvars_nonkernel)
-      if chol:
-        gradients_k = tape.gradient(loss, self.trvars_kernel)
-        optimizer_k.apply_gradients(zip(gradients_k, self.trvars_kernel))
-      optimizer.apply_gradients(zip(gradients, self.trvars_nonkernel))
-    finally:
-      del tape
-    return loss
-
-  def validation_step(self, D, S=1, chol=False):
-    """
-    Compute the validation loss on held-out data D
-    D is a tensorflow dataset (from slices) of (X,Y,sz)
-    """
-    return -self.elbo_avg(D["X"], D["Y"], sz=D["sz"], S=S, chol=chol)
-
-  def predict(self, Dtr, Dval=None, S=10):
-    """
-    Here Dtr,Dval should be raw counts (not normalized or log-transformed)
-    returns the predicted training data mean and validation data mean
-    on the original count scale
-    """
-    Mu_tr = misc.t2np(self.sample_predictive_mean(Dtr["X"], sz=Dtr["sz"], S=S))
-    if self.lik=="gau":
-      sz_tr = Dtr["Y"].sum(axis=1)
-      #note self.feature_means is None if self.nonneg=True
-      misc.reverse_normalization(Mu_tr, feature_means=self.feature_means,
-                            transform=np.expm1, sz=sz_tr, inplace=True)
-    if Dval:
-      Mu_val = misc.t2np(self.sample_predictive_mean(Dval["X"], sz=Dval["sz"], S=S))
-      if self.lik=="gau":
-        sz_val = Dval["Y"].sum(axis=1)
-        misc.reverse_normalization(Mu_val, feature_means=self.feature_means,
-                              transform=np.expm1, sz=sz_val, inplace=True)
-    else:
-      Mu_val = None
-    return Mu_tr,Mu_val
-
-def smooth_spatial_factors(F,Z,X=None):
-  """
-  F: real-valued factors (ie on the log scale for NSF)
-  Z: inducing point locations
-  X: spatial coordinates
-  """
-  M = Z.shape[0]
-  if X is None: #no spatial coordinates, just use the mean
-    beta0 = F.mean(axis=0)
-    U = np.tile(beta0,[M,1])
-    beta = None
-  else: #spatial coordinates
-    lr = LinearRegression().fit(X,F)
-    beta0 = lr.intercept_
-    beta = lr.coef_
-    nn = max(2, ceil(X.shape[0]/M))
-    knn = KNeighborsRegressor(n_neighbors=nn).fit(X,F)
-    U = knn.predict(Z)
-  return U,beta0,beta
-
-def init_nsf_with_nmf(fit, Y, X=None, sz=1, pseudocount=1e-2, factors=None,
-                      loadings=None, shrinkage=0.2):
-  L = fit.W.shape[1]
-  # M = fit.Z.shape[0] #number of inducing points
-  kw = likelihoods.choose_nmf_pars(fit.lik)
-  F,W = nnfu.regularized_nmf(Y, L, sz=sz, pseudocount=pseudocount,
-                             factors=factors, loadings=loadings,
-                             shrinkage=shrinkage, **kw)
-  # eF = factors
-  # W = loadings
-  # if eF is None or W is None:
-  #   kw = likelihoods.choose_nmf_pars(fit.lik)
-  #   nmf = NMF(L,**kw)
-  #   eF = nmf.fit_transform(Y)#/sz
-  #   W = nmf.components_.T
-  # W = postprocess.shrink_loadings(W, shrinkage=shrinkage)
-  # wsum = W.sum(axis=0)
-  # eF = postprocess.shrink_factors(eF*wsum, shrinkage=shrinkage)
-  # F = np.log(pseudocount+eF)-np.log(sz)
-  # beta0 = fit.beta0.numpy().flatten()
-  # wt_to_W = F.mean(axis=0)- beta0
-  # F-= wt_to_W
-  # W*= np.exp(wt_to_W-np.log(wsum))
-  # W,wsum = normalize_cols(W)
-  # eF *= wsum
-  # eFm2 = eF.mean()/2
-  # eF/=eFm2
-  # W*=eFm2
-  # F = np.log(pseudocount+eF)
-  fit.set_loadings(W)
-  U,beta0,beta = smooth_spatial_factors(F,fit.Z.numpy(),X=X)
-  # if X is None: #no spatial coordinates, just use the mean
-  #   beta0 = F.mean(axis=0)
-  #   U = np.tile(beta0,[M,1])
-  # else: #spatial coordinates
-  #   lr = LinearRegression().fit(X,F)
-  #   beta0 = lr.intercept_
-  #   fit.beta.assign(lr.coef_,read_value=False)
-  #   nn = max(2, ceil(X.shape[0]/M))
-  #   knn = KNeighborsRegressor(n_neighbors=nn).fit(X,F)
-  #   U = knn.predict(fit.Z.numpy())
-  fit.beta0.assign(beta0[:,None],read_value=False)
-  fit.delta.assign(U.T,read_value=False)
-  if beta is not None: fit.beta.assign(beta,read_value=False)
+        mu_x = self.beta0 + tfl.matmul(self.beta, X, transpose_b=True)  # LxN
+        Kuf = kernel.matrix(self.Z, X)  # LxMxN
+        Kff_diag = kernel.apply(X, X, example_ndims=1) + self.nugget  # LxN
+        alpha_x = tfl.cholesky_solve(Kuu_chol, Kuf)  # LxMxN
+        mu_tilde = mu_x + tfl.matvec(
+            alpha_x, self.delta - mu_z, transpose_a=True
+        )  # LxN
+        # compute the alpha(x_i)'(K_uu-Omega)alpha(x_i) term
+        a_t_Kchol = tfl.matmul(alpha_x, Kuu_chol, transpose_a=True)  # LxNxM
+        aKa = tf.reduce_sum(tf.square(a_t_Kchol), axis=2)  # LxN
+        a_t_Omega_tril = tfl.matmul(alpha_x, self.Omega_tril, transpose_a=True)  # LxNxM
+        aOmega_a = tf.reduce_sum(tf.square(a_t_Omega_tril), axis=2)  # LxN
+        Sigma_tilde = Kff_diag - aKa + aOmega_a  # LxN
+        eps = tf.random.normal(
+            (S, L, N)
+        )  # note this is not the same random generator as self.rng!
+        return mu_tilde + tf.math.sqrt(Sigma_tilde) * eps  # "F", dims: SxLxN
+
+    def sample_predictive_mean(
+        self, X, sz=1, S=1, kernel=None, mu_z=None, Kuu_chol=None, chol=True
+    ):
+        """
+        See sample_latent_variational_GP_funcs for X,S definitions
+        sz is a tensor of shape (N,1) of size factors.
+        Typically sz would be the rowSums or rowMeans of the outcome matrix Y.
+        """
+        F = self.sample_latent_GP_funcs(
+            X, S=S, kernel=kernel, mu_z=mu_z, Kuu_chol=Kuu_chol, chol=chol
+        )  # SxLxN
+        if self.nonneg:
+            Lam = tfl.matrix_transpose(tfl.matmul(self.W, tf.exp(F)))  # SxNxJ
+            if self.lik == "gau":
+                return Lam
+            else:
+                return sz * Lam
+        else:
+            Lam = tfl.matrix_transpose(tfl.matmul(self.W, F))
+            if self.lik == "gau":  # identity link
+                return Lam
+            else:  # log link (poi, nb)
+                return tf.exp(tf.math.log(sz) + Lam)
+
+    def eval_kl_term(self, mu_z, Kuu_chol):
+        """
+        KL divergence from the prior distribution to the variational distribution.
+        This is one component of the ELBO:
+        ELBO=expected log-likelihood - sum(kl_terms)
+        qpars: a tuple containing (mu_z,Kuu_chol)
+        qpars can be obtained by calling self.get_variational_params()
+        mu_z is the GP mean function at all inducing points (dimension: LxM)
+        Kuu_chol is the cholesky lower triangular of the kernel matrix of all inducing points.
+        Its dimension is LxMxM
+        where L = number of latent dimensions and M = number of inducing points.
+        """
+        qu = tfd.MultivariateNormalTriL(loc=self.delta, scale_tril=self.Omega_tril)
+        pu = tfd.MultivariateNormalTriL(loc=mu_z, scale_tril=Kuu_chol)
+        return qu.kl_divergence(pu)  # L-vector
+
+    # @tf.function
+    def elbo_avg(self, X, Y, sz=1, S=1, Ntot=None, chol=True):
+        """
+        Parameters
+        ----------
+        X : numpy array of spatial coordinates (NxD)
+            **OR** a tuple of spatial coordinates, multivariate outcomes,
+            and size factors (convenient for minibatches from tensor slices)
+        Y : numpy array of multivariate outcomes (NxJ)
+            If Y is None then X must be a tuple of length three
+        sz : size factors, optional
+            vector of length N, typically the rowSums or rowMeans of Y.
+            If X is a tuple then this is ignored as sz is expected in the third
+            element of the X tuple.
+        S : integer, optional
+            Number of random GP function evaluations to use. The default is 1.
+            Larger S=more accurate approximation to true ELBO but slower
+        Ntot : total number of observations in full dataset
+            This is needed when X,Y,sz are a minibatch from the full data
+            If Ntot is None, we assume X,Y,sz provided are the full data NOT a minibatch.
+        Returns
+        -------
+        The numeric evidence lower bound value, divided by Ntot.
+        """
+        batch_size, J = Y.shape
+        if Ntot is None:
+            Ntot = batch_size  # no minibatch, all observations provided
+        ker = self.get_kernel()
+        mu_z = self.get_mu_z()
+        Kuu_chol = self.get_Kuu_chol(kernel=ker, from_cache=(not chol))
+        # kl_terms is not affected by minibatching so use reduce_sum
+        kl_term = tf.reduce_sum(self.eval_kl_term(mu_z, Kuu_chol))
+        # Sample z1
+        z1 = self.sample_predictive_mean(
+            X, sz=sz, S=S, kernel=ker, mu_z=mu_z, Kuu_chol=Kuu_chol
+        )
+        # Compute p(z0|z1) using sampled z1 and z0
+        mean_top = jnp.exp(z1).dot(W1)
+        # Sample z0
+        z0 = gamma_sample(var_shape_z0, var_rate_z0)
+        prior_z0 = gamma_logpdf(z0, alpha, alpha / mean_top)
+        # And entropy of z0
+        ent_z0 = -gamma_logpdf(z0, var_shape_z0, var_rate_z0)
+        kl_term = kl_term + prior_z0 + ent_z0
+        # Compute p(y|z0)
+        mean_bottom = z0.dot(W0)
+        eloglik = poisson_logpdf()
+        eloglik = likelihoods.lik_to_distr(self.lik, Mu, self.disp).log_prob(Y)
+        return J * tf.reduce_mean(eloglik) - kl_term / Ntot
+
+    def train_step(self, D, optimizer, optimizer_k, S=1, Ntot=None, chol=True):
+        """
+        Executes one training step and returns the loss.
+        D is training data: a tensorflow dataset (from slices) of (X,Y,sz)
+        This function computes the loss and gradients, and uses the latter to
+        update the model's parameters.
+        """
+        with tf.GradientTape(persistent=True) as tape:
+            loss = -self.elbo_avg(D["X"], D["Y"], sz=D["sz"], S=S, Ntot=Ntot, chol=chol)
+        try:
+            gradients = tape.gradient(loss, self.trvars_nonkernel)
+            if chol:
+                gradients_k = tape.gradient(loss, self.trvars_kernel)
+                optimizer_k.apply_gradients(zip(gradients_k, self.trvars_kernel))
+            optimizer.apply_gradients(zip(gradients, self.trvars_nonkernel))
+        finally:
+            del tape
+        return loss
+
+    def validation_step(self, D, S=1, chol=False):
+        """
+        Compute the validation loss on held-out data D
+        D is a tensorflow dataset (from slices) of (X,Y,sz)
+        """
+        return -self.elbo_avg(D["X"], D["Y"], sz=D["sz"], S=S, chol=chol)
+
+    def predict(self, Dtr, Dval=None, S=10):
+        """
+        Here Dtr,Dval should be raw counts (not normalized or log-transformed)
+        returns the predicted training data mean and validation data mean
+        on the original count scale
+        """
+        Mu_tr = misc.t2np(self.sample_predictive_mean(Dtr["X"], sz=Dtr["sz"], S=S))
+        if self.lik == "gau":
+            sz_tr = Dtr["Y"].sum(axis=1)
+            # note self.feature_means is None if self.nonneg=True
+            misc.reverse_normalization(
+                Mu_tr,
+                feature_means=self.feature_means,
+                transform=np.expm1,
+                sz=sz_tr,
+                inplace=True,
+            )
+        if Dval:
+            Mu_val = misc.t2np(
+                self.sample_predictive_mean(Dval["X"], sz=Dval["sz"], S=S)
+            )
+            if self.lik == "gau":
+                sz_val = Dval["Y"].sum(axis=1)
+                misc.reverse_normalization(
+                    Mu_val,
+                    feature_means=self.feature_means,
+                    transform=np.expm1,
+                    sz=sz_val,
+                    inplace=True,
+                )
+        else:
+            Mu_val = None
+        return Mu_tr, Mu_val
+
+
+def smooth_spatial_factors(F, Z, X=None):
+    """
+    F: real-valued factors (ie on the log scale for NSF)
+    Z: inducing point locations
+    X: spatial coordinates
+    """
+    M = Z.shape[0]
+    if X is None:  # no spatial coordinates, just use the mean
+        beta0 = F.mean(axis=0)
+        U = np.tile(beta0, [M, 1])
+        beta = None
+    else:  # spatial coordinates
+        lr = LinearRegression().fit(X, F)
+        beta0 = lr.intercept_
+        beta = lr.coef_
+        nn = max(2, ceil(X.shape[0] / M))
+        knn = KNeighborsRegressor(n_neighbors=nn).fit(X, F)
+        U = knn.predict(Z)
+    return U, beta0, beta
+
+
+def init_nsf_with_nmf(
+    fit, Y, X=None, sz=1, pseudocount=1e-2, factors=None, loadings=None, shrinkage=0.2
+):
+    L = fit.W.shape[1]
+    # M = fit.Z.shape[0] #number of inducing points
+    kw = likelihoods.choose_nmf_pars(fit.lik)
+    F, W = nnfu.regularized_nmf(
+        Y,
+        L,
+        sz=sz,
+        pseudocount=pseudocount,
+        factors=factors,
+        loadings=loadings,
+        shrinkage=shrinkage,
+        **kw
+    )
+    # eF = factors
+    # W = loadings
+    # if eF is None or W is None:
+    #   kw = likelihoods.choose_nmf_pars(fit.lik)
+    #   nmf = NMF(L,**kw)
+    #   eF = nmf.fit_transform(Y)#/sz
+    #   W = nmf.components_.T
+    # W = postprocess.shrink_loadings(W, shrinkage=shrinkage)
+    # wsum = W.sum(axis=0)
+    # eF = postprocess.shrink_factors(eF*wsum, shrinkage=shrinkage)
+    # F = np.log(pseudocount+eF)-np.log(sz)
+    # beta0 = fit.beta0.numpy().flatten()
+    # wt_to_W = F.mean(axis=0)- beta0
+    # F-= wt_to_W
+    # W*= np.exp(wt_to_W-np.log(wsum))
+    # W,wsum = normalize_cols(W)
+    # eF *= wsum
+    # eFm2 = eF.mean()/2
+    # eF/=eFm2
+    # W*=eFm2
+    # F = np.log(pseudocount+eF)
+    fit.set_loadings(W)
+    U, beta0, beta = smooth_spatial_factors(F, fit.Z.numpy(), X=X)
+    # if X is None: #no spatial coordinates, just use the mean
+    #   beta0 = F.mean(axis=0)
+    #   U = np.tile(beta0,[M,1])
+    # else: #spatial coordinates
+    #   lr = LinearRegression().fit(X,F)
+    #   beta0 = lr.intercept_
+    #   fit.beta.assign(lr.coef_,read_value=False)
+    #   nn = max(2, ceil(X.shape[0]/M))
+    #   knn = KNeighborsRegressor(n_neighbors=nn).fit(X,F)
+    #   U = knn.predict(fit.Z.numpy())
+    fit.beta0.assign(beta0[:, None], read_value=False)
+    fit.delta.assign(U.T, read_value=False)
+    if beta is not None:
+        fit.beta.assign(beta, read_value=False)
```

### Comparing `scdef-0.0.1/scdef/scdef.py` & `scdef-0.0.2/scdef/scdef.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,97 +19,126 @@
 import scipy
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 
 from scdef.util import *
 
-class scDEF(object):
-    def __init__(self, adata, layer_sizes=[60, 30, 15], batch_key='batch', seed=42, logginglevel=logging.INFO,
-                 layer_shapes=None, brd=1e3, factor_shapes=None, factor_rates=None, layer_diagonals=None,
-                 batch_cpal='Dark2', layer_cpal=None):
 
+class scDEF(object):
+    def __init__(
+        self,
+        adata,
+        counts_layer=None,
+        layer_sizes=[60, 30, 15],
+        batch_key="batch",
+        seed=42,
+        logginglevel=logging.INFO,
+        layer_shapes=None,
+        brd=1e3,
+        factor_shapes=None,
+        factor_rates=None,
+        layer_diagonals=None,
+        batch_cpal="Dark2",
+        layer_cpal=None,
+    ):
         self.layer_sizes = [int(x) for x in layer_sizes]
         self.n_layers = len(self.layer_sizes)
 
         if self.n_layers < 2:
-            raise ValueError('scDEF requires at least 2 layers')
+            raise ValueError("scDEF requires at least 2 layers")
 
         if layer_shapes is None:
-            layer_shapes = [1.] * self.n_layers
+            layer_shapes = [1.0] * self.n_layers
         elif isinstance(layer_shapes, float) or isinstance(layer_shapes, int):
             layer_shapes = [float(layer_shapes)] * self.n_layers
         elif len(layer_shapes) != self.n_layers:
-            raise ValueError('layer_shapes list must be of size scDEF.n_layers')
+            raise ValueError("layer_shapes list must be of size scDEF.n_layers")
 
         if factor_shapes is None:
-            factor_shapes = [1.] + [.1] * (self.n_layers-1)
+            factor_shapes = [1.0] + [0.1] * (self.n_layers - 1)
         elif isinstance(factor_shapes, float) or isinstance(factor_shapes, int):
             factor_shapes = [float(factor_shapes)] * self.n_layers
         elif len(factor_shapes) != self.n_layers:
-            raise ValueError('factor_shapes list must be of size scDEF.n_layers')
+            raise ValueError("factor_shapes list must be of size scDEF.n_layers")
 
         if factor_rates is None:
-            factor_rates = [.1] + [1.] * (self.n_layers-1)
+            factor_rates = [0.1] + [1.0] * (self.n_layers - 1)
         elif isinstance(factor_rates, float) or isinstance(factor_rates, int):
             factor_rates = [float(factor_rates)] * self.n_layers
         elif len(factor_rates) != self.n_layers:
-            raise ValueError('factor_rates list must be of size scDEF.n_layers')
+            raise ValueError("factor_rates list must be of size scDEF.n_layers")
 
         if layer_diagonals is None:
-            layer_diagonals = [1.] * self.n_layers
+            layer_diagonals = [1.0] * self.n_layers
         elif isinstance(layer_diagonals, float) or isinstance(layer_diagonals, int):
             layer_diagonals = [float(layer_diagonals)] * self.n_layers
         elif len(layer_diagonals) != self.n_layers:
-            raise ValueError('layer_diagonals list must be of size scDEF.n_layers')
+            raise ValueError("layer_diagonals list must be of size scDEF.n_layers")
 
         if layer_cpal is None:
             layer_cpal = ["Set1"] * self.n_layers
         elif isinstance(layer_cpal, str):
             layer_cpal = [layer_cpal] * self.n_layers
         elif len(layer_cpal) != self.n_layers:
-            raise ValueError('layer_cpal list must be of size scDEF.n_layers')
+            raise ValueError("layer_cpal list must be of size scDEF.n_layers")
 
         self.layer_shapes = layer_shapes
         self.layer_diagonals = layer_diagonals
 
         self.factor_lists = [np.arange(size) for size in self.layer_sizes]
 
         self.factor_shapes = factor_shapes
         self.factor_rates = factor_rates
 
         self.brd = brd
 
-        self.logger = logging.getLogger('scDEF')
+        self.logger = logging.getLogger("scDEF")
         self.logger.setLevel(logginglevel)
 
         self.n_batches = 1
-        self.batches = ['']
+        self.batches = [""]
 
         self.seed = seed
-        self.layer_names = ['h' * i for i in range(self.n_layers)]
+        self.layer_names = ["h" * i for i in range(self.n_layers)]
         self.layer_cpal = layer_cpal
         self.batch_cpal = batch_cpal
-        self.layer_colorpalettes = [sns.color_palette(layer_cpal[idx], n_colors=size) for idx, size in enumerate(layer_sizes)]
+        self.layer_colorpalettes = [
+            sns.color_palette(layer_cpal[idx], n_colors=size)
+            for idx, size in enumerate(layer_sizes)
+        ]
 
-        self.load_adata(adata, batch_key=batch_key)
+        self.load_adata(adata, layer=counts_layer, batch_key=batch_key)
         self.batch_key = batch_key
         self.n_cells, self.n_genes = adata.shape
 
         self.w_priors = []
         for idx in range(self.n_layers):
             prior_shapes = self.factor_shapes[idx]
             prior_rates = self.factor_rates[idx]
 
             if idx > 0:
-                prior_shapes = np.ones((self.layer_sizes[idx], self.layer_sizes[idx-1])) * self.factor_shapes[idx] * 1./self.layer_diagonals[idx]
-                prior_rates = np.ones((self.layer_sizes[idx], self.layer_sizes[idx-1])) * self.factor_rates[idx] * self.layer_diagonals[idx]
+                prior_shapes = (
+                    np.ones((self.layer_sizes[idx], self.layer_sizes[idx - 1]))
+                    * self.factor_shapes[idx]
+                    * 1.0
+                    / self.layer_diagonals[idx]
+                )
+                prior_rates = (
+                    np.ones((self.layer_sizes[idx], self.layer_sizes[idx - 1]))
+                    * self.factor_rates[idx]
+                    * self.layer_diagonals[idx]
+                )
                 for l in range(self.layer_sizes[idx]):
-                    prior_shapes[l,l] = self.factor_shapes[idx] * self.layer_diagonals[idx]
-                    prior_rates[l,l] = self.factor_rates[idx] * self.layer_diagonals[idx]
+                    prior_shapes[l, l] = (
+                        self.factor_shapes[idx] * self.layer_diagonals[idx]
+                    )
+                    prior_rates[l, l] = (
+                        self.factor_rates[idx] * self.layer_diagonals[idx]
+                    )
                 prior_shapes = jnp.clip(jnp.array(prior_shapes), 1e-12, 1e12)
                 prior_rates = jnp.clip(jnp.array(prior_rates), 1e-12, 1e12)
 
             self.w_priors.append([prior_shapes, prior_rates])
 
         self.init_var_params()
         self.set_posterior_means()
@@ -119,25 +148,47 @@
         self.get_params = None
         self.opt_update = None
         self.elbos = []
         self.step_sizes = []
 
     def __repr__(self):
         out = f"scDEF object with {self.n_layers} layers"
-        out += "\n\t" + "Layer names: " + ", ".join([f'{name}factor' for name in self.layer_names])
-        out += "\n\t" + "Layer sizes: " + ", ".join([str(len(factors)) for factors in self.factor_lists])
-        out += "\n\t" + "Layer shape parameters: " + ", ".join([str(shape) for shape in self.layer_shapes])
-        out += "\n\t" + "Layer factor shape parameters: " + ", ".join([str(shape) for shape in self.factor_shapes])
-        out += "\n\t" + "Layer factor rate parameters: " + ", ".join([str(rate) for rate in self.factor_rates])
-        out += "\n\t" + "Lowe layer factor relevance prior concentration: " + str(self.brd)
+        out += (
+            "\n\t"
+            + "Layer names: "
+            + ", ".join([f"{name}factor" for name in self.layer_names])
+        )
+        out += (
+            "\n\t"
+            + "Layer sizes: "
+            + ", ".join([str(len(factors)) for factors in self.factor_lists])
+        )
+        out += (
+            "\n\t"
+            + "Layer shape parameters: "
+            + ", ".join([str(shape) for shape in self.layer_shapes])
+        )
+        out += (
+            "\n\t"
+            + "Layer factor shape parameters: "
+            + ", ".join([str(shape) for shape in self.factor_shapes])
+        )
+        out += (
+            "\n\t"
+            + "Layer factor rate parameters: "
+            + ", ".join([str(rate) for rate in self.factor_rates])
+        )
+        out += (
+            "\n\t" + "Lowe layer factor relevance prior concentration: " + str(self.brd)
+        )
         out += "\n\t" + "Number of batches: " + str(self.n_batches)
         out += "\n" + "Contains " + self.adata.__str__()
         return out
 
-    def load_adata(self, adata, layer=None, batch_key='batch'):
+    def load_adata(self, adata, layer=None, batch_key="batch"):
         if not isinstance(adata, AnnData):
             raise TypeError("adata must be an instance of AnnData.")
         self.adata = adata.copy()
         self.adata.raw = self.adata
         X = self.adata.raw.X
         if layer is not None:
             X = self.adata.layers[layer]
@@ -145,295 +196,483 @@
         if isinstance(X, scipy.sparse.csr_matrix):
             self.X = np.array(self.adata.raw.X.toarray())
         else:
             self.X = np.array(X)
 
         self.batch_indices_onehot = np.ones((self.adata.shape[0], 1))
         self.batch_lib_sizes = np.sum(self.X, axis=1)
-        self.batch_lib_ratio = np.ones((self.X.shape[0],1)) * np.mean(self.batch_lib_sizes)/np.var(self.batch_lib_sizes)
+        self.batch_lib_ratio = (
+            np.ones((self.X.shape[0], 1))
+            * np.mean(self.batch_lib_sizes)
+            / np.var(self.batch_lib_sizes)
+        )
         gene_size = np.sum(self.X, axis=0)
-        self.gene_ratio = np.mean(gene_size)/np.var(gene_size)
+        self.gene_ratio = np.mean(gene_size) / np.var(gene_size)
         if batch_key in self.adata.obs.columns:
             batches = np.unique(self.adata.obs[batch_key].values)
             self.batches = batches
             self.n_batches = len(batches)
-            self.logger.info(f"Found {self.n_batches} values for `{batch_key}` in data: {batches}")
-            if f'{batch_key}_colors' in self.adata.uns:
-                self.batch_colors = self.adata.uns[f'{batch_key}_colors']
-            else:
-                batch_colorpalette = sns.color_palette(self.batch_cpal, n_colors=self.n_batches)
-                self.batch_colors = [matplotlib.colors.to_hex(batch_colorpalette[idx]) for idx in range(self.n_batches)]
-                self.adata.uns[f'{batch_key}_colors'] = self.batch_colors
+            self.logger.info(
+                f"Found {self.n_batches} values for `{batch_key}` in data: {batches}"
+            )
+            if f"{batch_key}_colors" in self.adata.uns:
+                self.batch_colors = self.adata.uns[f"{batch_key}_colors"]
+            else:
+                batch_colorpalette = sns.color_palette(
+                    self.batch_cpal, n_colors=self.n_batches
+                )
+                self.batch_colors = [
+                    matplotlib.colors.to_hex(batch_colorpalette[idx])
+                    for idx in range(self.n_batches)
+                ]
+                self.adata.uns[f"{batch_key}_colors"] = self.batch_colors
             self.batch_indices_onehot = np.zeros((self.adata.shape[0], self.n_batches))
             if self.n_batches > 1:
                 self.gene_ratio = np.ones((self.n_batches, self.adata.shape[1]))
                 for i, b in enumerate(batches):
                     cells = np.where(self.adata.obs[batch_key] == b)[0]
                     self.batch_indices_onehot[cells, i] = 1
                     self.batch_lib_sizes[cells] = np.sum(self.X, axis=1)[cells]
-                    self.batch_lib_ratio[cells] = np.mean(self.batch_lib_sizes[cells])/np.var(self.batch_lib_sizes[cells])
+                    self.batch_lib_ratio[cells] = np.mean(
+                        self.batch_lib_sizes[cells]
+                    ) / np.var(self.batch_lib_sizes[cells])
                     batch_gene_size = np.sum(self.X[cells], axis=0)
-                    self.gene_ratio[i] = np.mean(batch_gene_size)/np.var(batch_gene_size)
+                    self.gene_ratio[i] = np.mean(batch_gene_size) / np.var(
+                        batch_gene_size
+                    )
         self.batch_indices_onehot = jnp.array(self.batch_indices_onehot)
         self.batch_lib_sizes = jnp.array(self.batch_lib_sizes)
         self.batch_lib_ratio = jnp.array(self.batch_lib_ratio)
         self.gene_ratio = jnp.array(self.gene_ratio)
 
         self.X = jnp.array(self.X)
 
     def init_var_params(self, minval=0.5, maxval=1.5):
         rngs = random.split(random.PRNGKey(self.seed), 4 + 2 * 3 * self.n_layers)
 
         self.var_params = [
-            jnp.array((jnp.log(random.uniform(rngs[0], minval=0.5, maxval=1.5,shape=[self.n_cells,1]) * 10 ), # cell_scales
-                       jnp.log(random.uniform(rngs[1], minval=0.5, maxval=1.5, shape=[self.n_cells,1])) * jnp.clip(10 * self.batch_lib_ratio, 1e-6, 1e2))),
-            jnp.array((jnp.log(random.uniform(rngs[2], minval=0.5, maxval=1.5,shape=[self.n_batches,self.n_genes]) * 10), # gene_scales
-                       jnp.log(random.uniform(rngs[3], minval=0.5, maxval=1.5 ,shape=[self.n_batches,self.n_genes]) * jnp.clip(10 * self.gene_ratio, 1e-6, 1e2)))),
+            jnp.array(
+                (
+                    jnp.log(
+                        random.uniform(
+                            rngs[0], minval=0.5, maxval=1.5, shape=[self.n_cells, 1]
+                        )
+                        * 10
+                    ),  # cell_scales
+                    jnp.log(
+                        random.uniform(
+                            rngs[1], minval=0.5, maxval=1.5, shape=[self.n_cells, 1]
+                        )
+                    )
+                    * jnp.clip(10 * self.batch_lib_ratio, 1e-6, 1e2),
+                )
+            ),
+            jnp.array(
+                (
+                    jnp.log(
+                        random.uniform(
+                            rngs[2],
+                            minval=0.5,
+                            maxval=1.5,
+                            shape=[self.n_batches, self.n_genes],
+                        )
+                        * 10
+                    ),  # gene_scales
+                    jnp.log(
+                        random.uniform(
+                            rngs[3],
+                            minval=0.5,
+                            maxval=1.5,
+                            shape=[self.n_batches, self.n_genes],
+                        )
+                        * jnp.clip(10 * self.gene_ratio, 1e-6, 1e2)
+                    ),
+                )
+            ),
         ]
 
         fscale_shapes = []
         fscale_rates = []
         z_shapes = []
         z_rates = []
         rng_cnt = 0
-        for layer_idx in range(self.n_layers): # we go from layer 0 (bottom) to layer L (top)
+        for layer_idx in range(
+            self.n_layers
+        ):  # we go from layer 0 (bottom) to layer L (top)
             # Init scales
             if layer_idx == 0:
-                fscale_shape = jnp.log(random.uniform(rngs[rng_cnt], minval=minval, maxval=maxval, shape=[self.layer_sizes[layer_idx],1]) )
+                fscale_shape = jnp.log(
+                    random.uniform(
+                        rngs[rng_cnt],
+                        minval=minval,
+                        maxval=maxval,
+                        shape=[self.layer_sizes[layer_idx], 1],
+                    )
+                )
             else:
-                fscale_shape = jnp.log(random.uniform(rngs[rng_cnt], minval=minval, maxval=maxval, shape=[self.layer_sizes[layer_idx],1]))
+                fscale_shape = jnp.log(
+                    random.uniform(
+                        rngs[rng_cnt],
+                        minval=minval,
+                        maxval=maxval,
+                        shape=[self.layer_sizes[layer_idx], 1],
+                    )
+                )
             fscale_shapes.append(fscale_shape)
             rng_cnt += 1
             if layer_idx == 0:
-                fscale_rate = jnp.log(random.uniform(rngs[rng_cnt], minval=minval, maxval=maxval, shape=[self.layer_sizes[layer_idx],1]) )
+                fscale_rate = jnp.log(
+                    random.uniform(
+                        rngs[rng_cnt],
+                        minval=minval,
+                        maxval=maxval,
+                        shape=[self.layer_sizes[layer_idx], 1],
+                    )
+                )
             else:
-                fscale_rate = jnp.log(random.uniform(rngs[rng_cnt], minval=minval, maxval=maxval, shape=[self.layer_sizes[layer_idx],1]))
+                fscale_rate = jnp.log(
+                    random.uniform(
+                        rngs[rng_cnt],
+                        minval=minval,
+                        maxval=maxval,
+                        shape=[self.layer_sizes[layer_idx], 1],
+                    )
+                )
             fscale_rates.append(fscale_rate)
             rng_cnt += 1
 
             # Init z
-            z_shape = jnp.log(random.uniform(rngs[rng_cnt], minval=minval, maxval=maxval, shape=[self.n_cells,self.layer_sizes[layer_idx]]) )
+            z_shape = jnp.log(
+                random.uniform(
+                    rngs[rng_cnt],
+                    minval=minval,
+                    maxval=maxval,
+                    shape=[self.n_cells, self.layer_sizes[layer_idx]],
+                )
+            )
             z_shapes.append(z_shape)
             rng_cnt += 1
-            z_rate = jnp.log(random.uniform(rngs[rng_cnt], minval=minval, maxval=maxval, shape=[self.n_cells,self.layer_sizes[layer_idx]]) )
+            z_rate = jnp.log(
+                random.uniform(
+                    rngs[rng_cnt],
+                    minval=minval,
+                    maxval=maxval,
+                    shape=[self.n_cells, self.layer_sizes[layer_idx]],
+                )
+            )
             z_rates.append(z_rate)
             rng_cnt += 1
 
-        self.var_params.append(jnp.array((jnp.vstack(fscale_shapes), jnp.vstack(fscale_rates))))
+        self.var_params.append(
+            jnp.array((jnp.vstack(fscale_shapes), jnp.vstack(fscale_rates)))
+        )
         self.var_params.append(jnp.array((jnp.hstack(z_shapes), jnp.hstack(z_rates))))
 
-        for layer_idx in range(self.n_layers): # the w don't have a shared axis across all, so we can't vectorize
+        for layer_idx in range(
+            self.n_layers
+        ):  # the w don't have a shared axis across all, so we can't vectorize
             # Init w
             in_layer = self.layer_sizes[layer_idx]
             if layer_idx == 0:
                 out_layer = self.n_genes
             else:
-                out_layer = self.layer_sizes[layer_idx-1]
-            w_shape = jnp.log(random.uniform(rngs[rng_cnt], minval=minval, maxval=maxval, shape=[in_layer, out_layer]) * jnp.clip(self.w_priors[layer_idx][0], 1e-2, 1e2) )
+                out_layer = self.layer_sizes[layer_idx - 1]
+            w_shape = jnp.log(
+                random.uniform(
+                    rngs[rng_cnt],
+                    minval=minval,
+                    maxval=maxval,
+                    shape=[in_layer, out_layer],
+                )
+                * jnp.clip(self.w_priors[layer_idx][0], 1e-2, 1e2)
+            )
             rng_cnt += 1
-            w_rate = jnp.log(random.uniform(rngs[rng_cnt], minval=minval, maxval=maxval, shape=[in_layer, out_layer]) * jnp.clip(self.w_priors[layer_idx][1], 1e-2, 1e2) )
+            w_rate = jnp.log(
+                random.uniform(
+                    rngs[rng_cnt],
+                    minval=minval,
+                    maxval=maxval,
+                    shape=[in_layer, out_layer],
+                )
+                * jnp.clip(self.w_priors[layer_idx][1], 1e-2, 1e2)
+            )
             rng_cnt += 1
 
-            self.var_params.append(
-                jnp.array((w_shape, w_rate))
-            )
+            self.var_params.append(jnp.array((w_shape, w_rate)))
 
-    def elbo(self, rng, indices, var_params, annealing_parameter, min_shape=1e-5, min_rate=1e-3, max_rate=1e3):
+    def elbo(
+        self,
+        rng,
+        indices,
+        var_params,
+        annealing_parameter,
+        min_shape=1e-5,
+        min_rate=1e-3,
+        max_rate=1e3,
+    ):
         # Single-sample Monte Carlo estimate of the variational lower bound.
         batch_indices_onehot = self.batch_indices_onehot[indices]
 
         cell_budget_params = var_params[0]
         gene_budget_params = var_params[1]
         fscale_params = var_params[2]
         z_params = var_params[3]
 
-        cell_budget_shape = jnp.maximum(jnp.exp(cell_budget_params[0][indices]), min_shape)
-        cell_budget_rate = jnp.minimum(jnp.maximum(jnp.exp(cell_budget_params[1][indices]), min_rate), max_rate)
+        cell_budget_shape = jnp.maximum(
+            jnp.exp(cell_budget_params[0][indices]), min_shape
+        )
+        cell_budget_rate = jnp.minimum(
+            jnp.maximum(jnp.exp(cell_budget_params[1][indices]), min_rate), max_rate
+        )
 
         gene_budget_shape = jnp.maximum(jnp.exp(gene_budget_params[0]), min_shape)
-        gene_budget_rate = jnp.minimum(jnp.maximum(jnp.exp(gene_budget_params[1]), min_rate), max_rate)
+        gene_budget_rate = jnp.minimum(
+            jnp.maximum(jnp.exp(gene_budget_params[1]), min_rate), max_rate
+        )
 
         fscale_shapes = jnp.maximum(jnp.exp(fscale_params[0]), min_shape)
-        fscale_rates = jnp.minimum(jnp.maximum(jnp.exp(fscale_params[1]), min_rate), max_rate)
+        fscale_rates = jnp.minimum(
+            jnp.maximum(jnp.exp(fscale_params[1]), min_rate), max_rate
+        )
 
         z_shapes = jnp.maximum(jnp.exp(z_params[0][indices]), min_shape)
-        z_rates = jnp.minimum(jnp.maximum(jnp.exp(z_params[1][indices]), min_rate), max_rate)
+        z_rates = jnp.minimum(
+            jnp.maximum(jnp.exp(z_params[1][indices]), min_rate), max_rate
+        )
 
         # Sample from variational distribution
         cell_budget_sample = gamma_sample(rng, cell_budget_shape, cell_budget_rate)
         gene_budget_sample = gamma_sample(rng, gene_budget_shape, gene_budget_rate)
-        fscale_samples = gamma_sample(rng, fscale_shapes, fscale_rates) # vectorized
-        z_samples = gamma_sample(rng, z_shapes, z_rates) # vectorized
+        fscale_samples = gamma_sample(rng, fscale_shapes, fscale_rates)  # vectorized
+        z_samples = gamma_sample(rng, z_shapes, z_rates)  # vectorized
         # w will be sampled in a loop below because it cannot be vectorized
 
         # Compute ELBO
-        global_pl = gamma_logpdf(gene_budget_sample, 1., self.gene_ratio)
-        global_en = -gamma_logpdf(gene_budget_sample, gene_budget_shape, gene_budget_rate)
-        local_pl = gamma_logpdf(cell_budget_sample, 1., self.batch_lib_ratio[indices])
-        local_en = -gamma_logpdf(cell_budget_sample, cell_budget_shape, cell_budget_rate)
+        global_pl = gamma_logpdf(gene_budget_sample, 1.0, self.gene_ratio)
+        global_en = -gamma_logpdf(
+            gene_budget_sample, gene_budget_shape, gene_budget_rate
+        )
+        local_pl = gamma_logpdf(cell_budget_sample, 1.0, self.batch_lib_ratio[indices])
+        local_en = -gamma_logpdf(
+            cell_budget_sample, cell_budget_shape, cell_budget_rate
+        )
 
         # Top layer
-        idx = self.n_layers-1
+        idx = self.n_layers - 1
         start = np.sum(self.layer_sizes[:idx])
         end = start + self.layer_sizes[idx]
         # scale
         _fscale_sample = fscale_samples[start:end]
         _fscale_shape = fscale_shapes[start:end]
         _fscale_rate = fscale_rates[start:end]
         global_pl += gamma_logpdf(_fscale_sample, 1e0, 1e0)
         global_en += -gamma_logpdf(_fscale_sample, _fscale_shape, _fscale_rate)
         # w
-        _w_shape = jnp.maximum(jnp.exp(var_params[4+idx][0]), min_shape)
-        _w_rate = jnp.minimum(jnp.maximum(jnp.exp(var_params[4+idx][1]), min_rate), max_rate)
+        _w_shape = jnp.maximum(jnp.exp(var_params[4 + idx][0]), min_shape)
+        _w_rate = jnp.minimum(
+            jnp.maximum(jnp.exp(var_params[4 + idx][1]), min_rate), max_rate
+        )
         _w_sample = gamma_sample(rng, _w_shape, _w_rate)
-        global_pl += gamma_logpdf(_w_sample, self.w_priors[idx][0], self.w_priors[idx][1] / _fscale_sample)
+        global_pl += gamma_logpdf(
+            _w_sample, self.w_priors[idx][0], self.w_priors[idx][1] / _fscale_sample
+        )
         global_en += -gamma_logpdf(_w_sample, _w_shape, _w_rate)
         # z
         _z_sample = z_samples[:, start:end]
         _z_shape = z_shapes[:, start:end]
         _z_rate = z_rates[:, start:end]
-        local_pl += gamma_logpdf(_z_sample, self.layer_shapes[idx], self.layer_shapes[idx])
+        local_pl += gamma_logpdf(
+            _z_sample, self.layer_shapes[idx], self.layer_shapes[idx]
+        )
         local_en += -gamma_logpdf(_z_sample, _z_shape, _z_rate)
 
         fscale_mean = _w_sample.T.dot(_fscale_sample)
-        z_mean = jnp.einsum('nk,kp->np', _z_sample, _w_sample)
+        z_mean = jnp.einsum("nk,kp->np", _z_sample, _w_sample)
 
-        for idx in list(np.arange(0, self.n_layers-1)[::-1]):
+        for idx in list(np.arange(0, self.n_layers - 1)[::-1]):
             start = np.sum(self.layer_sizes[:idx]).astype(int)
             end = start + self.layer_sizes[idx]
             # scale
             _fscale_sample = fscale_samples[start:end]
             _fscale_shape = fscale_shapes[start:end]
             _fscale_rate = fscale_rates[start:end]
             if idx == 0:
                 global_pl += gamma_logpdf(_fscale_sample, self.brd, self.brd)
             else:
                 global_pl += gamma_logpdf(_fscale_sample, 1e0, 1e0)
             global_en += -gamma_logpdf(_fscale_sample, _fscale_shape, _fscale_rate)
             # w
-            _w_shape = jnp.maximum(jnp.exp(var_params[4+idx][0]), min_shape)
-            _w_rate = jnp.minimum(jnp.maximum(jnp.exp(var_params[4+idx][1]), min_rate), max_rate)
+            _w_shape = jnp.maximum(jnp.exp(var_params[4 + idx][0]), min_shape)
+            _w_rate = jnp.minimum(
+                jnp.maximum(jnp.exp(var_params[4 + idx][1]), min_rate), max_rate
+            )
             _w_sample = gamma_sample(rng, _w_shape, _w_rate)
             if idx == 0:
-                global_pl += gamma_logpdf(_w_sample, self.w_priors[idx][0] / _fscale_sample  , self.w_priors[idx][1] / _fscale_sample)
+                global_pl += gamma_logpdf(
+                    _w_sample,
+                    self.w_priors[idx][0] / _fscale_sample,
+                    self.w_priors[idx][1] / _fscale_sample,
+                )
             else:
-                global_pl += gamma_logpdf(_w_sample, self.w_priors[idx][0], self.w_priors[idx][1] / _fscale_sample)
+                global_pl += gamma_logpdf(
+                    _w_sample,
+                    self.w_priors[idx][0],
+                    self.w_priors[idx][1] / _fscale_sample,
+                )
             global_en += -gamma_logpdf(_w_sample, _w_shape, _w_rate)
             # z
             _z_sample = z_samples[:, start:end]
             _z_shape = z_shapes[:, start:end]
             _z_rate = z_rates[:, start:end]
-            local_pl += gamma_logpdf(_z_sample, self.layer_shapes[idx] ,  self.layer_shapes[idx] / z_mean)
+            local_pl += gamma_logpdf(
+                _z_sample, self.layer_shapes[idx], self.layer_shapes[idx] / z_mean
+            )
             local_en += -gamma_logpdf(_z_sample, _z_shape, _z_rate)
 
             fscale_mean = _w_sample.T.dot(_fscale_sample)
-            z_mean = jnp.einsum('nk,kp->np', _z_sample, _w_sample)
+            z_mean = jnp.einsum("nk,kp->np", _z_sample, _w_sample)
 
         # Compute log likelihood
-        mean_bottom = jnp.einsum('nk,kg->ng', _z_sample / cell_budget_sample, _w_sample) / (batch_indices_onehot.dot(gene_budget_sample) )
+        mean_bottom = jnp.einsum(
+            "nk,kg->ng", _z_sample / cell_budget_sample, _w_sample
+        ) / (batch_indices_onehot.dot(gene_budget_sample))
         ll = jnp.sum(vmap(poisson.logpmf)(self.X[indices], mean_bottom))
 
         # Anneal the entropy
         global_en *= annealing_parameter
         local_en *= annealing_parameter
 
-        return ll + (local_pl + local_en + (indices.shape[0] / self.X.shape[0]) * (global_pl + global_en) )
+        return ll + (
+            local_pl
+            + local_en
+            + (indices.shape[0] / self.X.shape[0]) * (global_pl + global_en)
+        )
 
     def batch_elbo(self, rng, indices, var_params, num_samples, annealing_parameter):
         # Average over a batch of random samples.
         rngs = random.split(rng, num_samples)
         vectorized_elbo = vmap(self.elbo, in_axes=(0, None, None, None))
         return jnp.mean(vectorized_elbo(rngs, indices, var_params, annealing_parameter))
 
-    def _optimize(self, update_func, opt_state, n_epochs=500, batch_size=1, step_size=0.1, annealing_parameter=1., seed=None):
+    def _optimize(
+        self,
+        update_func,
+        opt_state,
+        n_epochs=500,
+        batch_size=1,
+        step_size=0.1,
+        annealing_parameter=1.0,
+        seed=None,
+    ):
         if seed is None:
             seed = self.seed
 
         num_complete_batches, leftover = divmod(self.n_cells, batch_size)
         num_batches = num_complete_batches + bool(leftover)
-        self.logger.info(f"Each epoch contains {num_batches} batches of size {batch_size}")
+        self.logger.info(
+            f"Each epoch contains {num_batches} batches of size {batch_size}"
+        )
+
         def data_stream():
             rng = np.random.RandomState(0)
             while True:
                 perm = rng.permutation(self.n_cells)
                 for i in range(num_batches):
-                    batch_idx = perm[i * batch_size:(i + 1) * batch_size]
+                    batch_idx = perm[i * batch_size : (i + 1) * batch_size]
                     yield jnp.array(batch_idx)
+
         batches = data_stream()
 
         losses = []
 
-
         annealing_parameter = jnp.array(annealing_parameter)
         rng = random.PRNGKey(seed)
         t = 0
         pbar = tqdm(range(n_epochs))
         for epoch in pbar:
             epoch_losses = []
             start_time = time.time()
             for it in range(num_batches):
                 rng, rng_input = random.split(rng)
-                loss, opt_state = update_func(next(batches), t, rng_input, opt_state, annealing_parameter)
+                loss, opt_state = update_func(
+                    next(batches), t, rng_input, opt_state, annealing_parameter
+                )
                 epoch_losses.append(loss)
                 t += 1
             losses.append(np.mean(epoch_losses))
             epoch_time = time.time() - start_time
-            pbar.set_postfix({'Loss': losses[-1]})
+            pbar.set_postfix({"Loss": losses[-1]})
 
         return losses, opt_state
 
-    def learn(self, n_epoch=1000, lr=0.2, annealing=1., num_samples=5, batch_size=None):
-
+    def learn(
+        self, n_epoch=1000, lr=0.2, annealing=1.0, num_samples=5, batch_size=None
+    ):
         n_steps = 1
 
         if isinstance(n_epoch, list):
             n_steps = len(n_epoch)
             n_epoch_schedule = n_epoch
         else:
             n_epoch_schedule = [n_epoch]
 
         if isinstance(lr, list):
             lr_schedule = lr
             if len(lr_schedule) != n_steps:
-                raise ValueError('lr_schedule list must be of same length as n_epoch_schedule')
+                raise ValueError(
+                    "lr_schedule list must be of same length as n_epoch_schedule"
+                )
         else:
-            lr_schedule = [lr*0.5**step for step in range(n_steps)]
+            lr_schedule = [lr * 0.5**step for step in range(n_steps)]
 
         if isinstance(annealing, list):
             annealing_schedule = annealing
             if len(annealing_schedule) != n_steps:
-                raise ValueError('annealing_schedule list must be of same length as n_epoch_schedule')
+                raise ValueError(
+                    "annealing_schedule list must be of same length as n_epoch_schedule"
+                )
         else:
             annealing_schedule = [annealing] * n_steps
 
         if batch_size is None:
             batch_size = self.n_cells
 
         # Set up jitted functions
         init_params = self.var_params
 
         def objective(indices, var_params, key, annealing_parameter):
-            return -self.batch_elbo(key, indices, var_params, num_samples, annealing_parameter) # minimize -ELBO
+            return -self.batch_elbo(
+                key, indices, var_params, num_samples, annealing_parameter
+            )  # minimize -ELBO
 
         loss_grad = jit(value_and_grad(objective, argnums=1))
 
         for i in range(len(lr_schedule)):
             step_size = lr_schedule[i]
             anneal_param = annealing_schedule[i]
-            self.logger.info(f"Initializing optimizer with learning rate {step_size} and annealing parameter {anneal_param}")
+            self.logger.info(
+                f"Initializing optimizer with learning rate {step_size} and annealing parameter {anneal_param}"
+            )
             opt_init, opt_update, get_params = optimizers.adam(step_size=step_size)
+
             def update(indices, i, key, opt_state, annealing_parameter):
                 params = get_params(opt_state)
                 value, gradient = loss_grad(indices, params, key, annealing_parameter)
                 return value, opt_update(i, gradient, opt_state)
+
             opt_state = opt_init(self.var_params)
 
-            losses, opt_state = self._optimize(update, opt_state, n_epochs=n_epoch_schedule[i],
-                                          step_size=lr_schedule[i], batch_size=batch_size,
-                                              annealing_parameter=anneal_param)
+            losses, opt_state = self._optimize(
+                update,
+                opt_state,
+                n_epochs=n_epoch_schedule[i],
+                step_size=lr_schedule[i],
+                batch_size=batch_size,
+                annealing_parameter=anneal_param,
+            )
             params = get_params(opt_state)
             self.var_params = params
             self.elbos.append(losses)
             self.step_sizes.append(lr_schedule[i])
 
         self.set_posterior_means()
         self.filter_factors()
@@ -442,109 +681,160 @@
         cell_budget_params = self.var_params[0]
         gene_budget_params = self.var_params[1]
         fscale_params = self.var_params[2]
         z_params = self.var_params[3]
         w_params = self.var_params[4]
 
         self.pmeans = {
-            'cell_scale': np.array(np.exp(cell_budget_params[0]) / np.exp(cell_budget_params[1])),
-            'gene_scale': np.array(np.exp(gene_budget_params[0]) / np.exp(gene_budget_params[1])),
+            "cell_scale": np.array(
+                np.exp(cell_budget_params[0]) / np.exp(cell_budget_params[1])
+            ),
+            "gene_scale": np.array(
+                np.exp(gene_budget_params[0]) / np.exp(gene_budget_params[1])
+            ),
         }
 
         for idx in range(self.n_layers):
             start = sum(self.layer_sizes[:idx])
             end = start + self.layer_sizes[idx]
-            self.pmeans[f'{self.layer_names[idx]}fscale'] = np.array(np.exp(fscale_params[0][start:end])/np.exp(fscale_params[1][start:end]))
-            self.pmeans[f'{self.layer_names[idx]}z'] = np.array(np.exp(z_params[0][:,start:end])/np.exp(z_params[1][:,start:end]))
-            _w_shape = self.var_params[4+idx][0]
-            _w_rate = self.var_params[4+idx][1]
-            self.pmeans[f'{self.layer_names[idx]}W'] = np.array(np.exp(_w_shape) / np.exp(_w_rate))
+            self.pmeans[f"{self.layer_names[idx]}fscale"] = np.array(
+                np.exp(fscale_params[0][start:end])
+                / np.exp(fscale_params[1][start:end])
+            )
+            self.pmeans[f"{self.layer_names[idx]}z"] = np.array(
+                np.exp(z_params[0][:, start:end]) / np.exp(z_params[1][:, start:end])
+            )
+            _w_shape = self.var_params[4 + idx][0]
+            _w_rate = self.var_params[4 + idx][1]
+            self.pmeans[f"{self.layer_names[idx]}W"] = np.array(
+                np.exp(_w_shape) / np.exp(_w_rate)
+            )
 
-    def filter_factors(self, ard=.5):
+    def filter_factors(self, ard=0.5):
         if isinstance(ard, float):
             ard = [ard] * self.n_layers
         elif len(ard) != self.n_layers:
-            raise IndexError('ard list must be of size scDEF.n_layers')
+            raise IndexError("ard list must be of size scDEF.n_layers")
         self.factor_lists = []
         for i, layer_name in enumerate(self.layer_names):
-            thres = np.quantile(self.pmeans[f'{layer_name}fscale'], q=ard[i])
-            self.factor_lists.append(np.where(self.pmeans[f'{layer_name}fscale'] >= thres)[0])
+            thres = np.quantile(self.pmeans[f"{layer_name}fscale"], q=ard[i])
+            self.factor_lists.append(
+                np.where(self.pmeans[f"{layer_name}fscale"] >= thres)[0]
+            )
         self.annotate_adata()
         self.make_graph()
 
     def annotate_adata(self):
-        self.adata.obs['cell_scale'] = 1/self.pmeans['cell_scale']
+        self.adata.obs["cell_scale"] = 1 / self.pmeans["cell_scale"]
         if self.n_batches == 1:
-            self.adata.var['gene_scale'] = 1/self.pmeans['gene_scale'][0]
+            self.adata.var["gene_scale"] = 1 / self.pmeans["gene_scale"][0]
             self.logger.info("Updated adata.var: `gene_scale`")
         else:
             for batch_idx in range(self.n_batches):
-                name = f'gene_scale_{batch_idx}'
-                self.adata.var[name] = 1/self.pmeans['gene_scale'][batch_idx]
+                name = f"gene_scale_{batch_idx}"
+                self.adata.var[name] = 1 / self.pmeans["gene_scale"][batch_idx]
                 self.logger.info(f"Updated adata.var: `{name}` for batch {batch_idx}.")
 
         for idx in range(self.n_layers):
             layer_name = self.layer_names[idx]
-            self.adata.obsm[f'X_{layer_name}factors'] = self.pmeans[f'{layer_name}z'][:,self.factor_lists[idx]]
-            self.adata.obs[f'{layer_name}factor'] = np.argmax(self.adata.obsm[f'X_{layer_name}factors'], axis=1).astype(str)
-            self.adata.uns[f'{layer_name}factor_colors'] = [matplotlib.colors.to_hex(self.layer_colorpalettes[idx][i]) for i in range(len(self.factor_lists[idx]))]
-            df = pd.DataFrame(self.adata.obsm[f'X_{layer_name}factors'], index=self.adata.obs.index, columns=[f'{layer_name}z_{i}' for i in range(len(self.factor_lists[idx]))])
-            if f'{layer_name}z_0' not in self.adata.obs.columns:
+            self.adata.obsm[f"X_{layer_name}factors"] = self.pmeans[f"{layer_name}z"][
+                :, self.factor_lists[idx]
+            ]
+            self.adata.obs[f"{layer_name}factor"] = np.argmax(
+                self.adata.obsm[f"X_{layer_name}factors"], axis=1
+            ).astype(str)
+            self.adata.uns[f"{layer_name}factor_colors"] = [
+                matplotlib.colors.to_hex(self.layer_colorpalettes[idx][i])
+                for i in range(len(self.factor_lists[idx]))
+            ]
+            df = pd.DataFrame(
+                self.adata.obsm[f"X_{layer_name}factors"],
+                index=self.adata.obs.index,
+                columns=[
+                    f"{layer_name}z_{i}" for i in range(len(self.factor_lists[idx]))
+                ],
+            )
+            if f"{layer_name}z_0" not in self.adata.obs.columns:
                 self.adata.obs = pd.concat([self.adata.obs, df], axis=1)
             else:
-                self.adata.obs = self.adata.obs.drop(columns=[col for col in self.adata.obs.columns if f'{layer_name}z_' in col])
+                self.adata.obs = self.adata.obs.drop(
+                    columns=[
+                        col
+                        for col in self.adata.obs.columns
+                        if f"{layer_name}z_" in col
+                    ]
+                )
                 self.adata.obs[df.columns] = df
 
-            self.logger.info(f"Updated adata.obs with layer {idx}: `{layer_name}factor` and `{layer_name}z_<factor_idx>` for all factors in layer {idx}")
-            self.logger.info(f"Updated adata.obsm with layer {idx}: `X_{layer_name}factors`")
+            self.logger.info(
+                f"Updated adata.obs with layer {idx}: `{layer_name}factor` and `{layer_name}z_<factor_idx>` for all factors in layer {idx}"
+            )
+            self.logger.info(
+                f"Updated adata.obsm with layer {idx}: `X_{layer_name}factors`"
+            )
 
     def get_annotations(self, marker_reference, gene_rankings=None):
         if gene_rankings is None:
             gene_rankings = self.get_rankings(layer_idx=0)
 
         annotations = []
         keys = list(marker_reference.keys())
         for rank in gene_rankings:
             # Get annotation in marker_reference that contains the highest score
             # score is length of intersection over length of union
-            scores = np.array([len(set(rank).intersection(set(marker_reference[a])))/len(set(rank).union(set(marker_reference[a]))) for a in keys])
+            scores = np.array(
+                [
+                    len(set(rank).intersection(set(marker_reference[a])))
+                    / len(set(rank).union(set(marker_reference[a])))
+                    for a in keys
+                ]
+            )
             sorted_ann_idx = np.argsort(scores)[::-1]
             sorted_scores = scores[sorted_ann_idx]
 
             # Get only annotations for which score is not zero
             sorted_ann_idx = sorted_ann_idx[np.where(sorted_scores > 0)[0]]
 
             ann = np.array(keys)[sorted_ann_idx]
-            ann = np.array([f'{a} ({sorted_scores[i]:.4f})' for i, a in enumerate(ann)]).tolist()
+            ann = np.array(
+                [f"{a} ({sorted_scores[i]:.4f})" for i, a in enumerate(ann)]
+            ).tolist()
             annotations.append(ann)
         return annotations
 
-    def get_rankings(self, layer_idx=0, q=.1, genes=True, return_scores=False):
+    def get_rankings(self, layer_idx=0, q=0.1, genes=True, return_scores=False):
         term_names = np.array(self.adata.var_names)
-        term_scores = self.pmeans['W'][self.factor_lists[0]]
+        term_scores = self.pmeans["W"][self.factor_lists[0]]
         n_factors = len(self.factor_lists[layer_idx])
 
         if layer_idx > 0:
             if genes:
-                term_scores = self.pmeans[f'{self.layer_names[layer_idx]}W'][self.factor_lists[layer_idx]][:,self.factor_lists[layer_idx-1]]
-                for layer in range(layer_idx-1, 0, -1):
-                    lower_mat = self.pmeans[f'{self.layer_names[layer]}W'][self.factor_lists[layer]][:,self.factor_lists[layer-1]]
+                term_scores = self.pmeans[f"{self.layer_names[layer_idx]}W"][
+                    self.factor_lists[layer_idx]
+                ][:, self.factor_lists[layer_idx - 1]]
+                for layer in range(layer_idx - 1, 0, -1):
+                    lower_mat = self.pmeans[f"{self.layer_names[layer]}W"][
+                        self.factor_lists[layer]
+                    ][:, self.factor_lists[layer - 1]]
                     term_scores = term_scores.dot(lower_mat)
-                term_scores = term_scores.dot(self.pmeans[f'{self.layer_names[0]}W'][self.factor_lists[0]])
+                term_scores = term_scores.dot(
+                    self.pmeans[f"{self.layer_names[0]}W"][self.factor_lists[0]]
+                )
             else:
-                n_factors_below = len(self.factor_lists[layer_idx-1])
+                n_factors_below = len(self.factor_lists[layer_idx - 1])
                 term_names = np.arange(n_factors_below).astype(str)
-                term_scores = self.pmeans[f'{self.layer_names[layer_idx]}W'][self.factor_lists[layer_idx]][:,self.factor_lists[layer_idx-1]]
-
+                term_scores = self.pmeans[f"{self.layer_names[layer_idx]}W"][
+                    self.factor_lists[layer_idx]
+                ][:, self.factor_lists[layer_idx - 1]]
 
         top_terms = []
         top_scores = []
         for k in range(n_factors):
             top_terms_idx = (term_scores[k, :]).argsort()[::-1]
-            sorted_term_scores_k = term_scores[k,:][top_terms_idx]
+            sorted_term_scores_k = term_scores[k, :][top_terms_idx]
             thres = np.quantile(sorted_term_scores_k, q=q)
             top_terms_idx = top_terms_idx[np.where(sorted_term_scores_k > thres)[0]]
             top_terms_list = term_names[top_terms_idx].tolist()
             top_scores_list = sorted_term_scores_k.tolist()
             top_terms.append(top_terms_list)
             top_scores.append(top_scores_list)
 
@@ -558,197 +848,272 @@
         genes, scores = self.get_rankings(return_scores=True)
 
         summary = f"Found {n_factors_eff} factors grouped in the following way:\n"
 
         # Group the factors
         assignments = []
         for i, factor in enumerate(tokeep):
-            assignments.append(np.argmax(self.pmeans[f'{self.layer_names[1]}W'][:,factor]))
+            assignments.append(
+                np.argmax(self.pmeans[f"{self.layer_names[1]}W"][:, factor])
+            )
         assignments = np.array(assignments)
         factor_order = np.argsort(np.array(assignments))
 
         for group in np.unique(assignments):
             factors = tokeep[np.where(assignments == group)[0]]
             if len(factors) > 0:
                 summary += f"Group {group}:\n"
             for i, factor in enumerate(factors):
                 summary += f"    Factor {i}: "
-                summary += ", ".join([f"{genes[factor][j]} ({scores[factor][j]:.3f})" for j in range(top_genes)])
+                summary += ", ".join(
+                    [
+                        f"{genes[factor][j]} ({scores[factor][j]:.3f})"
+                        for j in range(top_genes)
+                    ]
+                )
                 summary += "\n"
             summary += "\n"
 
         self.logger.info(summary)
 
         return summary
 
-    def get_enrichments(self, libs=['KEGG_2019_Human'], gene_rankings=None):
+    def get_enrichments(self, libs=["KEGG_2019_Human"], gene_rankings=None):
         if gene_rankings is None:
             gene_rankings = self.get_rankings(layer_idx=0)
 
         for rank in tqdm(gene_rankings):
-            enr = gp.enrichr(gene_list=rank,
-                         gene_sets=libs,
-                         organism='Human',
-                         outdir='test/enrichr',
-                         cutoff=0.05
-                        )
+            enr = gp.enrichr(
+                gene_list=rank,
+                gene_sets=libs,
+                organism="Human",
+                outdir="test/enrichr",
+                cutoff=0.05,
+            )
             enrichments.append(enr)
         return enrichments
 
-    def make_graph(self, show_signatures=True, enrichments=None, top_genes=None, show_batch_counts=False, filled=None, wedged=None, color_edges=True, **fontsize_kwargs):
+    def make_graph(
+        self,
+        show_signatures=True,
+        enrichments=None,
+        top_genes=None,
+        show_batch_counts=False,
+        filled=None,
+        wedged=None,
+        color_edges=True,
+        **fontsize_kwargs,
+    ):
         if top_genes is None:
             top_genes = [10] * self.n_layers
         elif isinstance(top_genes, float):
             top_genes = [top_genes] * self.n_layers
         elif len(top_genes) != self.n_layers:
-            raise IndexError('top_genes list must be of size scDEF.n_layers')
+            raise IndexError("top_genes list must be of size scDEF.n_layers")
 
         if filled is None:
             style = None
-        elif filled == 'factor':
-            style = 'filled'
+        elif filled == "factor":
+            style = "filled"
         else:
             if filled not in scd.adata.obs:
-                raise ValueError('filled must be factor or any `obs` in self.adata')
+                raise ValueError("filled must be factor or any `obs` in self.adata")
             else:
-                style = 'filled'
+                style = "filled"
 
         if style is None:
             if wedged is None:
                 style = None
             else:
                 if wedged not in scd.adata.obs:
-                    raise ValueError('wedged must be any `obs` in self.adata')
+                    raise ValueError("wedged must be any `obs` in self.adata")
                 else:
-                    style = 'wedged'
+                    style = "wedged"
         else:
             if wedged is not None:
                 self.logger.info("Filled style takes precedence over wedged")
 
-
         layer_factor_orders = []
-        for layer_idx in np.arange(0, self.n_layers)[::-1]: # Go top down
+        for layer_idx in np.arange(0, self.n_layers)[::-1]:  # Go top down
             factors = self.factor_lists[layer_idx]
             n_factors = len(factors)
-            if layer_idx < self.n_layers-1:
+            if layer_idx < self.n_layers - 1:
                 # Assign factors to upper factors to set the plotting order
-                mat = self.pmeans[f'{self.layer_names[layer_idx+1]}W'][self.factor_lists[layer_idx+1]][:, self.factor_lists[layer_idx]]
-                normalized_factor_weights = mat/np.sum(mat, axis=1).reshape(-1,1)
+                mat = self.pmeans[f"{self.layer_names[layer_idx+1]}W"][
+                    self.factor_lists[layer_idx + 1]
+                ][:, self.factor_lists[layer_idx]]
+                normalized_factor_weights = mat / np.sum(mat, axis=1).reshape(-1, 1)
                 assignments = []
                 for factor_idx in range(n_factors):
-                    assignments.append(np.argmax(normalized_factor_weights[:,factor_idx]))
+                    assignments.append(
+                        np.argmax(normalized_factor_weights[:, factor_idx])
+                    )
                 assignments = np.array(assignments)
 
                 factor_order = []
                 for upper_factor_idx in layer_factor_orders[-1]:
-                    factor_order.append(np.where(assignments==upper_factor_idx)[0])
+                    factor_order.append(np.where(assignments == upper_factor_idx)[0])
                 factor_order = np.concatenate(factor_order).astype(int)
                 layer_factor_orders.append(factor_order)
             else:
                 layer_factor_orders.append(np.arange(n_factors))
         layer_factor_orders = layer_factor_orders[::-1]
 
         def map_scores_to_fontsizes(scores, max_fontsize=11, min_fontsize=5):
             scores = scores - np.min(scores)
             scores = scores / np.max(scores)
-            fontsizes = min_fontsize + scores * (max_fontsize-min_fontsize)
+            fontsizes = min_fontsize + scores * (max_fontsize - min_fontsize)
             return fontsizes
 
         g = Graph()
-        ordering = 'out'
+        ordering = "out"
 
         for layer_idx in range(self.n_layers):
             layer_name = self.layer_names[layer_idx]
             factors = self.factor_lists[layer_idx]
             n_factors = len(factors)
             layer_colors = self.layer_colorpalettes[layer_idx][:n_factors]
 
             if show_signatures:
-                gene_rankings, gene_scores = self.get_rankings(layer_idx=layer_idx, genes=True, return_scores=True)
+                gene_rankings, gene_scores = self.get_rankings(
+                    layer_idx=layer_idx, genes=True, return_scores=True
+                )
 
             factor_order = layer_factor_orders[layer_idx]
             for factor_idx in factor_order:
                 factor_idx = int(factor_idx)
-                alpha = 'FF'
+                alpha = "FF"
                 color = None
                 if color_edges:
                     color = matplotlib.colors.to_hex(layer_colors[factor_idx])
-                fillcolor = '#FFFFFF'
-                if style == 'filled':
-                    if filled == 'factor':
+                fillcolor = "#FFFFFF"
+                if style == "filled":
+                    if filled == "factor":
                         fillcolor = matplotlib.colors.to_hex(layer_colors[factor_idx])
                     elif filled is not None:
                         # cells attached to this factor
                         original_factor_index = self.factor_lists[layer_idx][factor_idx]
-                        cells = np.where(self.adata.obs[f'{layer_name}factor'] == str(factor_idx))[0]
+                        cells = np.where(
+                            self.adata.obs[f"{layer_name}factor"] == str(factor_idx)
+                        )[0]
                         if len(cells) > 0:
                             # cells in this factor that belong to each obs
-                            prevs = [np.count_nonzero(self.adata.obs[filled][cells]==b) for b in scd.adata.obs[filled].unique()]
-                            obs_idx = np.argmax(prevs) # obs attachment
-                            alpha = prevs[obs_idx] / np.sum(prevs) # confidence on obs_idx attachment -- should I account for the number of cells in each batch in total?
-                            alpha = matplotlib.colors.rgb2hex((0,0,0,alpha),keep_alpha=True)[-2:].upper()
-                            fillcolor = self.adata.uns[f'{filled}_colors'][obs_idx]
+                            prevs = [
+                                np.count_nonzero(self.adata.obs[filled][cells] == b)
+                                for b in scd.adata.obs[filled].unique()
+                            ]
+                            obs_idx = np.argmax(prevs)  # obs attachment
+                            alpha = prevs[obs_idx] / np.sum(
+                                prevs
+                            )  # confidence on obs_idx attachment -- should I account for the number of cells in each batch in total?
+                            alpha = matplotlib.colors.rgb2hex(
+                                (0, 0, 0, alpha), keep_alpha=True
+                            )[-2:].upper()
+                            fillcolor = self.adata.uns[f"{filled}_colors"][obs_idx]
                     fillcolor = fillcolor + alpha
-                elif style == 'wedged':
+                elif style == "wedged":
                     # cells attached to this factor
                     original_factor_index = self.factor_lists[layer_idx][factor_idx]
-                    cells = np.where(self.adata.obs[f'{layer_name}factor'] == str(factor_idx))[0]
+                    cells = np.where(
+                        self.adata.obs[f"{layer_name}factor"] == str(factor_idx)
+                    )[0]
                     if len(cells) > 0:
                         # cells in this factor that belong to each obs
-                        prevs = [np.count_nonzero(self.adata.obs[wedged][cells]==b) for b in scd.adata.obs[wedged].unique()]
+                        prevs = [
+                            np.count_nonzero(self.adata.obs[wedged][cells] == b)
+                            for b in scd.adata.obs[wedged].unique()
+                        ]
                         fracs = prevs / np.sum(prevs)
                         # make color string for pie chart
-                        fillcolor = ":".join([f"{self.adata.uns[f'{wedged}_colors'][obs_idx]};{frac}" for obs_idx, frac in enumerate(fracs)])
+                        fillcolor = ":".join(
+                            [
+                                f"{self.adata.uns[f'{wedged}_colors'][obs_idx]};{frac}"
+                                for obs_idx, frac in enumerate(fracs)
+                            ]
+                        )
 
-                label = f'{int(factor_idx)}'
+                label = f"{int(factor_idx)}"
 
                 if enrichments is not None:
-                    label += '<br/><br/>' + "<br/>".join([enrichments[factor_idx].results['Term'].values[i] + f" ({enrichments[factor_idx].results['Adjusted P-value'][i]:.3f})" for i in range(top_genes[layer_idx])])
+                    label += "<br/><br/>" + "<br/>".join(
+                        [
+                            enrichments[factor_idx].results["Term"].values[i]
+                            + f" ({enrichments[factor_idx].results['Adjusted P-value'][i]:.3f})"
+                            for i in range(top_genes[layer_idx])
+                        ]
+                    )
                 elif show_signatures:
-                    factor_gene_rankings = gene_rankings[factor_idx][:top_genes[layer_idx]]
-                    factor_gene_scores = gene_scores[factor_idx][:top_genes[layer_idx]]
-                    fontsizes = map_scores_to_fontsizes(gene_scores[factor_idx], **fontsize_kwargs)[:top_genes[layer_idx]]
+                    factor_gene_rankings = gene_rankings[factor_idx][
+                        : top_genes[layer_idx]
+                    ]
+                    factor_gene_scores = gene_scores[factor_idx][: top_genes[layer_idx]]
+                    fontsizes = map_scores_to_fontsizes(
+                        gene_scores[factor_idx], **fontsize_kwargs
+                    )[: top_genes[layer_idx]]
                     gene_labels = []
                     for j, gene in enumerate(factor_gene_rankings):
-                        gene_labels.append(f'<FONT POINT-SIZE="{fontsizes[j]}">{gene}</FONT>')
-                    label += '<br/><br/>' + "<br/>".join(gene_labels)
+                        gene_labels.append(
+                            f'<FONT POINT-SIZE="{fontsizes[j]}">{gene}</FONT>'
+                        )
+                    label += "<br/><br/>" + "<br/>".join(gene_labels)
 
-                label = '<' + label + '>'
-                g.node(f'{layer_name}f' + str(factor_idx), label=label,
-                        fillcolor=fillcolor, color=color, ordering=ordering, style=style, )
+                label = "<" + label + ">"
+                g.node(
+                    f"{layer_name}f" + str(factor_idx),
+                    label=label,
+                    fillcolor=fillcolor,
+                    color=color,
+                    ordering=ordering,
+                    style=style,
+                )
 
                 if layer_idx > 0:
-                    mat = self.pmeans[f'{self.layer_names[layer_idx]}W'][self.factor_lists[layer_idx]][:,self.factor_lists[layer_idx-1]]
-                    normalized_factor_weights = mat/np.sum(mat, axis=1).reshape(-1,1)
-                    for lower_factor_idx in layer_factor_orders[layer_idx-1]:
-                        g.edge(f'{layer_name}f' + str(factor_idx), f'{self.layer_names[layer_idx-1]}f' + str(lower_factor_idx),
-                               penwidth=str(4*normalized_factor_weights[factor_idx,lower_factor_idx]), color=color)
+                    mat = self.pmeans[f"{self.layer_names[layer_idx]}W"][
+                        self.factor_lists[layer_idx]
+                    ][:, self.factor_lists[layer_idx - 1]]
+                    normalized_factor_weights = mat / np.sum(mat, axis=1).reshape(-1, 1)
+                    for lower_factor_idx in layer_factor_orders[layer_idx - 1]:
+                        g.edge(
+                            f"{layer_name}f" + str(factor_idx),
+                            f"{self.layer_names[layer_idx-1]}f" + str(lower_factor_idx),
+                            penwidth=str(
+                                4
+                                * normalized_factor_weights[
+                                    factor_idx, lower_factor_idx
+                                ]
+                            ),
+                            color=color,
+                        )
 
         self.graph = g
 
         self.logger.info(f"Updated scDEF graph")
 
-    def plot_ard(self, layer_idx=None, ard=0.5, show_yticks=False, scale='linear', **kwargs):
+    def plot_ard(
+        self, layer_idx=None, ard=0.5, show_yticks=False, scale="linear", **kwargs
+    ):
         def _plot_ard(layer_idx, ard):
-            scales = self.pmeans[f'{self.layer_names[layer_idx]}fscale'].ravel()
+            scales = self.pmeans[f"{self.layer_names[layer_idx]}fscale"].ravel()
             layer_size = self.layer_sizes[layer_idx]
             thres = np.quantile(scales, q=ard)
-            plt.axhline(thres, color='red', ls='--')
+            plt.axhline(thres, color="red", ls="--")
             above = np.where(scales >= thres)[0]
             below = np.where(scales < thres)[0]
             plt.bar(np.arange(layer_size)[above], scales[above])
-            plt.bar(np.arange(layer_size)[below], scales[below], alpha=0.6, color='gray')
+            plt.bar(
+                np.arange(layer_size)[below], scales[below], alpha=0.6, color="gray"
+            )
             if len(scales) > 15:
                 plt.xticks(np.arange(0, layer_size, 2))
             else:
                 plt.xticks(np.arange(layer_size))
             if not show_yticks:
                 plt.yticks([])
-            plt.title(f'Layer {layer_idx}')
-            plt.xlabel('Factor')
+            plt.title(f"Layer {layer_idx}")
+            plt.xlabel("Factor")
             plt.yscale(scale)
 
         if layer_idx is None:
             layer_idx = range(self.n_layers)
         elif isinstance(layer_idx, int):
             layer_idx = [layer_idx]
 
@@ -757,134 +1122,182 @@
             for i, layer in enumerate(layer_idx):
                 plt.sca(axes[i])
                 _plot_ard(layer, ard)
             plt.sca(axes[0])
         else:
             _plot_ard(layer_idx[0], ard)
 
-        plt.ylabel('Sparsity')
+        plt.ylabel("Sparsity")
 
         plt.show()
 
-    def plot_obs_factor_dotplot(self, obs_key, layer_idx, figsize=(8,2), s_min=10, s_max=500, titlesize=12, labelsize=12, legend_fontsize=12, legend_titlesize=12, cmap='viridis', logged=False):
+    def plot_obs_factor_dotplot(
+        self,
+        obs_key,
+        layer_idx,
+        figsize=(8, 2),
+        s_min=10,
+        s_max=500,
+        titlesize=12,
+        labelsize=12,
+        legend_fontsize=12,
+        legend_titlesize=12,
+        cmap="viridis",
+        logged=False,
+    ):
         # For each obs, compute the average cell score on each factor among the cells that attach to that obs, use as color
         # And compute the fraction of cells in the obs that attach to each factor, use as circle size
         layer_name = self.layer_names[layer_idx]
 
         obs = self.adata.obs[obs_key].unique()
         n_obs = len(obs)
         n_factors = len(self.factor_lists[layer_idx])
 
         df_rows = []
         c = np.zeros((n_obs, n_factors))
         s = np.zeros((n_obs, n_factors))
         for i, obs_val in enumerate(obs):
-            cells_from_obs = self.adata.obs.index[np.where(self.adata.obs[obs_key] == obs_val)[0]]
+            cells_from_obs = self.adata.obs.index[
+                np.where(self.adata.obs[obs_key] == obs_val)[0]
+            ]
             n_cells_obs = len(cells_from_obs)
             for factor in range(n_factors):
-                factor_name = f'{layer_name}z_{factor}'
-                cells_attached = self.adata.obs.index[np.where(self.adata.obs.loc[cells_from_obs][f'{layer_name}factor'] == str(factor))[0]]
+                factor_name = f"{layer_name}z_{factor}"
+                cells_attached = self.adata.obs.index[
+                    np.where(
+                        self.adata.obs.loc[cells_from_obs][f"{layer_name}factor"]
+                        == str(factor)
+                    )[0]
+                ]
                 if len(cells_attached) == 0:
-                    average_weight = 0#np.nan
-                    fraction_attached = 0#np.nan
+                    average_weight = 0  # np.nan
+                    fraction_attached = 0  # np.nan
                 else:
-                    average_weight = np.mean(self.adata.obs.loc[cells_from_obs][factor_name])
+                    average_weight = np.mean(
+                        self.adata.obs.loc[cells_from_obs][factor_name]
+                    )
                     fraction_attached = len(cells_attached) / n_cells_obs
-                c[i,factor] = average_weight
-                s[i,factor] = fraction_attached
+                c[i, factor] = average_weight
+                s[i, factor] = fraction_attached
 
         ylabels = obs
         xlabels = [str(i) for i in range(n_factors)]
 
         x, y = np.meshgrid(np.arange(len(xlabels)), np.arange(len(ylabels)))
 
-        fig, axes = plt.subplots(1,3, figsize=figsize, width_ratios=[5, 1, 1])
+        fig, axes = plt.subplots(1, 3, figsize=figsize, width_ratios=[5, 1, 1])
         plt.sca(axes[0])
         ax = plt.gca()
         s = s / np.max(s)
         s *= s_max
         s += s_max / s_min
         if logged:
             c = np.log(c)
-        plt.scatter(x,y,  c=c, s=s, cmap=cmap)
+        plt.scatter(x, y, c=c, s=s, cmap=cmap)
 
-        ax.set(xticks=np.arange(n_factors), yticks=np.arange(n_obs),
-               xticklabels=xlabels, yticklabels=ylabels)
-        ax.tick_params(axis='both', which='major', labelsize=labelsize)
-        ax.set_xticks(np.arange(n_factors+1)-0.5, minor=True)
-        ax.set_yticks(np.arange(n_obs+1)-0.5, minor=True)
-        ax.grid(which='minor')
+        ax.set(
+            xticks=np.arange(n_factors),
+            yticks=np.arange(n_obs),
+            xticklabels=xlabels,
+            yticklabels=ylabels,
+        )
+        ax.tick_params(axis="both", which="major", labelsize=labelsize)
+        ax.set_xticks(np.arange(n_factors + 1) - 0.5, minor=True)
+        ax.set_yticks(np.arange(n_obs + 1) - 0.5, minor=True)
+        ax.grid(which="minor")
 
         plt.ylabel(obs_key, fontsize=labelsize)
-        plt.xlabel('Factor', fontsize=labelsize)
-        plt.title(f'Layer {layer_idx}\n', fontsize=titlesize)
+        plt.xlabel("Factor", fontsize=labelsize)
+        plt.title(f"Layer {layer_idx}\n", fontsize=titlesize)
 
         # Make legend
-        map_f_to_s = {'0': 5, '25': 7, '50': 9, '75': 11, '100': 13}
+        map_f_to_s = {"0": 5, "25": 7, "50": 9, "75": 11, "100": 13}
         plt.sca(axes[1])
         ax = plt.gca()
-        ax.spines['top'].set_visible(False)
-        ax.spines['right'].set_visible(False)
-        ax.spines['bottom'].set_visible(False)
-        ax.spines['left'].set_visible(False)
+        ax.spines["top"].set_visible(False)
+        ax.spines["right"].set_visible(False)
+        ax.spines["bottom"].set_visible(False)
+        ax.spines["left"].set_visible(False)
 
         ax.get_xaxis().set_ticks([])
         ax.get_yaxis().set_ticks([])
-        circles = [Line2D([], [], color="white", marker='o', markersize=map_f_to_s[f], markerfacecolor="gray") for f in map_f_to_s.keys()]
-        lg = plt.legend(circles[::-1], list(map_f_to_s.keys())[::-1], numpoints=1, loc=2,
-                    frameon=False, fontsize=legend_fontsize)
+        circles = [
+            Line2D(
+                [],
+                [],
+                color="white",
+                marker="o",
+                markersize=map_f_to_s[f],
+                markerfacecolor="gray",
+            )
+            for f in map_f_to_s.keys()
+        ]
+        lg = plt.legend(
+            circles[::-1],
+            list(map_f_to_s.keys())[::-1],
+            numpoints=1,
+            loc=2,
+            frameon=False,
+            fontsize=legend_fontsize,
+        )
         plt.title("Fraction of \ncells in group (%)", fontsize=legend_titlesize)
 
         plt.sca(axes[2])
         ax = plt.gca()
-        ax.spines['top'].set_visible(False)
-        ax.spines['right'].set_visible(False)
-        ax.spines['bottom'].set_visible(False)
-        ax.spines['left'].set_visible(False)
+        ax.spines["top"].set_visible(False)
+        ax.spines["right"].set_visible(False)
+        ax.spines["bottom"].set_visible(False)
+        ax.spines["left"].set_visible(False)
 
         ax.get_xaxis().set_ticks([])
         ax.get_yaxis().set_ticks([])
-        cb = plt.colorbar(ax = axes[0], cmap=cmap)
-        cb.ax.set_title('Average\ncell score', fontsize=legend_titlesize)
+        cb = plt.colorbar(ax=axes[0], cmap=cmap)
+        cb.ax.set_title("Average\ncell score", fontsize=legend_titlesize)
         cb.ax.tick_params(labelsize=legend_fontsize)
-        plt.grid('off')
+        plt.grid("off")
         plt.show()
 
-    def plot_multilevel_paga(self, neighbors_rep="X_factors", figsize=(16,4), reuse_pos=True, **paga_kwargs):
+    def plot_multilevel_paga(
+        self, neighbors_rep="X_factors", figsize=(16, 4), reuse_pos=True, **paga_kwargs
+    ):
         "Plot PAGA graphs at all scDEF levels"
 
         fig, axes = plt.subplots(1, self.n_layers, figsize=figsize)
         sc.pp.neighbors(self.adata, use_rep=neighbors_rep)
         pos = None
-        for i, layer_idx in enumerate(range(self.n_layers-1, -1, -1)):
+        for i, layer_idx in enumerate(range(self.n_layers - 1, -1, -1)):
             ax = axes[i]
-            new_layer_name = f'{self.layer_names[layer_idx]}factor'
+            new_layer_name = f"{self.layer_names[layer_idx]}factor"
 
             self.logger.info(f"Computing PAGA graph of layer {layer_idx}")
 
             # Use previous PAGA as initial positions for new PAGA
-            if layer_idx != self.n_layers-1 and reuse_pos:
-                self.logger.info(f"Re-using PAGA positions from layer {layer_idx+1} to init {layer_idx}")
-                matches = sc._utils.identify_groups(self.adata.obs[new_layer_name], self.adata.obs[old_layer_name])
+            if layer_idx != self.n_layers - 1 and reuse_pos:
+                self.logger.info(
+                    f"Re-using PAGA positions from layer {layer_idx+1} to init {layer_idx}"
+                )
+                matches = sc._utils.identify_groups(
+                    self.adata.obs[new_layer_name], self.adata.obs[old_layer_name]
+                )
                 pos = []
                 np.random.seed(0)
                 for i, c in enumerate(self.adata.obs[new_layer_name].cat.categories):
-                    pos_coarse = self.adata.uns['paga']['pos'] # previous PAGA
+                    pos_coarse = self.adata.uns["paga"]["pos"]  # previous PAGA
                     coarse_categories = self.adata.obs[old_layer_name].cat.categories
                     idx = coarse_categories.get_loc(matches[c][0])
                     pos_i = pos_coarse[idx] + np.random.random(2)
                     pos.append(pos_i)
                 pos = np.array(pos)
 
             sc.tl.paga(self.adata, groups=new_layer_name)
             sc.pl.paga(
                 self.adata,
                 init_pos=pos,
-                layout='fa',
+                layout="fa",
                 ax=ax,
-                title=f'Layer {layer_idx} PAGA',
+                title=f"Layer {layer_idx} PAGA",
                 show=False,
                 **paga_kwargs,
             )
 
             old_layer_name = new_layer_name
         plt.show()
```

### Comparing `scdef-0.0.1/scdef/util.py` & `scdef-0.0.2/scdef/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,112 @@
 import numpy as np
 import jax.numpy as jnp
 from jax import vmap, random
 from jax.scipy.stats import norm, gamma, poisson
 
+
 def gaussian_sample(rng, mean, log_scale):
     scale = jnp.exp(log_scale)
     return mean + scale * random.normal(rng, mean.shape)
 
+
 def gaussian_logpdf(x, mean, log_scale):
     scale = jnp.exp(log_scale)
-    return jnp.sum(vmap(norm.logpdf)(x, mean * jnp.ones(x.shape), scale * jnp.ones(x.shape)))
+    return jnp.sum(
+        vmap(norm.logpdf)(x, mean * jnp.ones(x.shape), scale * jnp.ones(x.shape))
+    )
+
 
 def gamma_sample(rng, shape, rate):
-    scale = 1./rate
+    scale = 1.0 / rate
     return jnp.clip(scale * random.gamma(rng, shape), a_min=1e-15, a_max=1e15)
 
+
 def gamma_logpdf(x, shape, rate):
-    scale = 1./rate
-    return jnp.sum(vmap(gamma.logpdf)(x, shape * jnp.ones(x.shape), scale=scale * jnp.ones(x.shape)))
+    scale = 1.0 / rate
+    return jnp.sum(
+        vmap(gamma.logpdf)(
+            x, shape * jnp.ones(x.shape), scale=scale * jnp.ones(x.shape)
+        )
+    )
+
 
 def get_mean_cellscore_per_group(cell_scores, cell_groups):
     unique_cluster_ids = np.unique(cell_groups)
     mean_cluster_scores = []
     for c in unique_cluster_ids:
         cell_idx = np.where(cell_groups == c)[0]
         mean_cluster_scores.append(np.mean(cell_scores[cell_idx], axis=0))
     mean_cluster_scores = np.array(mean_cluster_scores)
     return mean_cluster_scores
 
+
 def mod_score(factors_by_groups_matrix):
-    total_factor_relative_weight = np.sum(factors_by_groups_matrix,axis=1)
-    total_factor_relative_weight = total_factor_relative_weight / np.sum(total_factor_relative_weight)
+    total_factor_relative_weight = np.sum(factors_by_groups_matrix, axis=1)
+    total_factor_relative_weight = total_factor_relative_weight / np.sum(
+        total_factor_relative_weight
+    )
 
     # Per factor
-    n1 = factors_by_groups_matrix/np.sum(factors_by_groups_matrix, axis=1)[:,np.newaxis]
+    n1 = (
+        factors_by_groups_matrix
+        / np.sum(factors_by_groups_matrix, axis=1)[:, np.newaxis]
+    )
     n1 = np.sum(np.max(n1, axis=1) * total_factor_relative_weight)
 
     # Per group
-    n2 = factors_by_groups_matrix/np.sum(factors_by_groups_matrix, axis=0)[np.newaxis,:]
+    n2 = (
+        factors_by_groups_matrix
+        / np.sum(factors_by_groups_matrix, axis=0)[np.newaxis, :]
+    )
     n2 = np.mean(np.max(n2, axis=0))
 
-    return np.mean([n1,n2])
+    return np.mean([n1, n2])
+
 
 def entropy_score(factors_by_groups_matrix):
-    total_factor_relative_weight = np.sum(factors_by_groups_matrix,axis=1)
-    total_factor_relative_weight = total_factor_relative_weight / np.sum(total_factor_relative_weight)
+    total_factor_relative_weight = np.sum(factors_by_groups_matrix, axis=1)
+    total_factor_relative_weight = total_factor_relative_weight / np.sum(
+        total_factor_relative_weight
+    )
 
     # Per factor
-    n1 = factors_by_groups_matrix/np.sum(factors_by_groups_matrix, axis=1)[:,np.newaxis]
-    n1 = np.sum(-np.sum(n1*np.log(n1), axis=1) * total_factor_relative_weight)
+    n1 = (
+        factors_by_groups_matrix
+        / np.sum(factors_by_groups_matrix, axis=1)[:, np.newaxis]
+    )
+    n1 = np.sum(-np.sum(n1 * np.log(n1), axis=1) * total_factor_relative_weight)
 
     # Per group
-    n2 = factors_by_groups_matrix/np.sum(factors_by_groups_matrix, axis=0)[np.newaxis,:]
-    n2 = np.mean(-np.sum(n2*np.log(n2), axis=0))
+    n2 = (
+        factors_by_groups_matrix
+        / np.sum(factors_by_groups_matrix, axis=0)[np.newaxis, :]
+    )
+    n2 = np.mean(-np.sum(n2 * np.log(n2), axis=0))
+
+    return np.mean([n1, n2])
 
-    return np.mean([n1,n2])
 
 def compute_geneset_coherence(genes, counts_adata):
     # As in Spectra: https://github.com/dpeerlab/spectra/blob/ff0e5c456127a33938b1ea560432f228dc26a08b/spectra/initialization.py
-    mat = np.array(counts_adata[:,genes].X)
+    mat = np.array(counts_adata[:, genes].X)
     n_genes = len(genes)
     score = 0
     for i in range(1, n_genes):
         for j in range(i):
             dw1 = mat[:, i] > 0
             dw2 = mat[:, j] > 0
             dw1w2 = (dw1 & dw2).astype(float).sum()
             dw1 = dw1.astype(float).sum()
             dw2 = dw2.astype(float).sum()
-            score += np.log((dw1w2 + 1)/(dw2))
+            score += np.log((dw1w2 + 1) / (dw2))
+
+    denom = n_genes * (n_genes - 1) / 2
 
-    denom = n_genes*(n_genes-1)/2
+    return score / denom
 
-    return score/denom
 
 def coherence_score(marker_gene_sets, heldout_counts_adata):
     chs = []
     for marker_genes in marker_gene_sets:
         chs.append(compute_geneset_coherence(marker_genes, heldout_counts_adata))
     return np.mean(chs)
```

