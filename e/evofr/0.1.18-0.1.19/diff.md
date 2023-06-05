# Comparing `tmp/evofr-0.1.18.tar.gz` & `tmp/evofr-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evofr-0.1.18.tar", max compression
+gzip compressed data, was "evofr-0.1.19.tar", max compression
```

## Comparing `evofr-0.1.18.tar` & `evofr-0.1.19.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    34523 2023-01-10 22:30:08.129997 evofr-0.1.18/LICENSE.txt
--rw-r--r--   0        0        0      888 2023-01-25 21:51:20.520616 evofr-0.1.18/evofr/__init__.py
--rw-r--r--   0        0        0      296 2022-06-23 22:50:02.937378 evofr-0.1.18/evofr/data/__init__.py
--rw-r--r--   0        0        0     1020 2022-09-14 16:20:57.633521 evofr-0.1.18/evofr/data/case_counts.py
--rw-r--r--   0        0        0     4419 2022-10-03 18:11:22.276420 evofr-0.1.18/evofr/data/case_frequencies.py
--rw-r--r--   0        0        0     5110 2022-10-03 18:22:14.382080 evofr-0.1.18/evofr/data/data_helpers.py
--rw-r--r--   0        0        0      471 2022-08-27 00:43:53.017698 evofr-0.1.18/evofr/data/data_spec.py
--rw-r--r--   0        0        0     1410 2022-08-27 00:43:53.018135 evofr-0.1.18/evofr/data/hier_cases.py
--rw-r--r--   0        0        0     2291 2022-10-03 18:10:38.950987 evofr-0.1.18/evofr/data/hier_frequencies.py
--rw-r--r--   0        0        0     3097 2023-02-01 20:10:34.869507 evofr-0.1.18/evofr/data/variant_frequencies.py
--rw-r--r--   0        0        0     1194 2023-01-06 07:10:08.312029 evofr-0.1.18/evofr/infer/BJBackendsScrap.py
--rw-r--r--   0        0        0     8451 2023-01-25 21:51:20.521303 evofr-0.1.18/evofr/infer/InferBlackJax.py
--rw-r--r--   0        0        0     2149 2022-09-15 21:51:48.846733 evofr-0.1.18/evofr/infer/InferMCMC.py
--rw-r--r--   0        0        0     3278 2023-01-25 21:51:20.522220 evofr-0.1.18/evofr/infer/InferSVI.py
--rw-r--r--   0        0        0     2478 2022-08-27 00:43:53.040621 evofr-0.1.18/evofr/infer/MCMC_handler.py
--rw-r--r--   0        0        0     2995 2022-08-27 00:43:53.019730 evofr-0.1.18/evofr/infer/SVI_handler.py
--rw-r--r--   0        0        0     1652 2023-01-25 21:51:20.522616 evofr-0.1.18/evofr/infer/SamplePrior.py
--rw-r--r--   0        0        0      302 2023-01-25 21:51:20.523080 evofr-0.1.18/evofr/infer/__init__.py
--rw-r--r--   0        0        0       78 2023-01-25 21:51:20.523543 evofr-0.1.18/evofr/infer/backends.py
--rw-r--r--   0        0        0      289 2022-12-21 20:12:56.042653 evofr-0.1.18/evofr/models/__init__.py
--rw-r--r--   0        0        0     4269 2023-02-01 20:10:34.870453 evofr-0.1.18/evofr/models/mlr_hierarchical.py
--rw-r--r--   0        0        0     9727 2023-02-01 20:10:34.871076 evofr-0.1.18/evofr/models/mlr_innovation.py
--rw-r--r--   0        0        0    11893 2022-11-08 19:03:50.750502 evofr-0.1.18/evofr/models/mlr_nowcast.py
--rw-r--r--   0        0        0     2886 2022-09-30 21:23:27.866766 evofr-0.1.18/evofr/models/mlr_spline.py
--rw-r--r--   0        0        0      700 2022-08-27 20:30:22.404715 evofr-0.1.18/evofr/models/model_spec.py
--rw-r--r--   0        0        0     4553 2023-04-05 18:05:00.919362 evofr-0.1.18/evofr/models/multinomial_logistic_regression.py
--rw-r--r--   0        0        0     5778 2023-01-25 21:51:20.524940 evofr-0.1.18/evofr/models/mutational_fitness_mlr.py
--rw-r--r--   0        0        0     3333 2022-09-26 17:53:00.939634 evofr-0.1.18/evofr/models/piantham_model.py
--rw-r--r--   0        0        0     2243 2022-08-27 01:00:23.614755 evofr-0.1.18/evofr/models/renewal_model/LAS.py
--rw-r--r--   0        0        0      257 2022-11-08 19:05:19.255557 evofr-0.1.18/evofr/models/renewal_model/__init__.py
--rw-r--r--   0        0        0      149 2022-07-13 00:53:30.188448 evofr-0.1.18/evofr/models/renewal_model/basis_functions/__init__.py
--rw-r--r--   0        0        0      198 2022-07-08 20:37:47.686469 evofr-0.1.18/evofr/models/renewal_model/basis_functions/basis_fns.py
--rw-r--r--   0        0        0     3391 2022-07-14 20:27:07.660069 evofr-0.1.18/evofr/models/renewal_model/basis_functions/hilbert_space_gaussian_process.py
--rw-r--r--   0        0        0     4778 2022-09-30 21:38:46.300190 evofr-0.1.18/evofr/models/renewal_model/basis_functions/splines.py
--rw-r--r--   0        0        0     6540 2023-04-06 23:46:59.942673 evofr-0.1.18/evofr/models/renewal_model/model_factories.py
--rw-r--r--   0        0        0     2405 2023-01-10 22:30:08.131767 evofr-0.1.18/evofr/models/renewal_model/model_functions.py
--rw-r--r--   0        0        0     1366 2023-01-10 22:30:08.132058 evofr-0.1.18/evofr/models/renewal_model/model_helpers.py
--rw-r--r--   0        0        0    11999 2023-04-05 18:05:00.920309 evofr-0.1.18/evofr/models/renewal_model/model_options.py
--rw-r--r--   0        0        0     1655 2023-02-01 21:09:24.709123 evofr-0.1.18/evofr/models/renewal_model/renewal_model.py
--rw-r--r--   0        0        0     4392 2022-09-10 15:55:23.454857 evofr-0.1.18/evofr/models/renewal_model/renewal_regression.py
--rw-r--r--   0        0        0     4933 2023-02-01 21:09:24.709494 evofr-0.1.18/evofr/models/renewal_model/renewal_single_variant.py
--rw-r--r--   0        0        0      831 2022-07-08 20:51:40.490887 evofr-0.1.18/evofr/models/renewal_model/spline_incidence.py
--rw-r--r--   0        0        0       62 2023-01-12 23:49:44.920731 evofr-0.1.18/evofr/plotting/__init__.py
--rw-r--r--   0        0        0    11903 2023-01-12 23:49:44.921903 evofr-0.1.18/evofr/plotting/plot_functions.py
--rw-r--r--   0        0        0    11557 2023-01-25 21:51:20.525631 evofr-0.1.18/evofr/plotting/plotting_classes.py
--rw-r--r--   0        0        0       97 2022-12-22 03:54:22.139076 evofr-0.1.18/evofr/posterior/__init__.py
--rw-r--r--   0        0        0     2996 2022-12-22 03:54:22.139787 evofr-0.1.18/evofr/posterior/posterior_handler.py
--rw-r--r--   0        0        0    14113 2023-04-06 23:46:59.943078 evofr-0.1.18/evofr/posterior/posterior_helpers.py
--rw-r--r--   0        0        0      512 2023-04-06 23:47:12.046165 evofr-0.1.18/pyproject.toml
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 evofr-0.1.18/setup.py
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 evofr-0.1.18/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-01-10 22:30:08.129997 evofr-0.1.19/LICENSE.txt
+-rw-r--r--   0        0        0      888 2023-01-25 21:51:20.520616 evofr-0.1.19/evofr/__init__.py
+-rw-r--r--   0        0        0      296 2022-06-23 22:50:02.937378 evofr-0.1.19/evofr/data/__init__.py
+-rw-r--r--   0        0        0     1020 2022-09-14 16:20:57.633521 evofr-0.1.19/evofr/data/case_counts.py
+-rw-r--r--   0        0        0     4419 2022-10-03 18:11:22.276420 evofr-0.1.19/evofr/data/case_frequencies.py
+-rw-r--r--   0        0        0     5110 2022-10-03 18:22:14.382080 evofr-0.1.19/evofr/data/data_helpers.py
+-rw-r--r--   0        0        0      471 2022-08-27 00:43:53.017698 evofr-0.1.19/evofr/data/data_spec.py
+-rw-r--r--   0        0        0     1410 2022-08-27 00:43:53.018135 evofr-0.1.19/evofr/data/hier_cases.py
+-rw-r--r--   0        0        0     2291 2022-10-03 18:10:38.950987 evofr-0.1.19/evofr/data/hier_frequencies.py
+-rw-r--r--   0        0        0     3097 2023-02-01 20:10:34.869507 evofr-0.1.19/evofr/data/variant_frequencies.py
+-rw-r--r--   0        0        0     1194 2023-01-06 07:10:08.312029 evofr-0.1.19/evofr/infer/BJBackendsScrap.py
+-rw-r--r--   0        0        0     8451 2023-01-25 21:51:20.521303 evofr-0.1.19/evofr/infer/InferBlackJax.py
+-rw-r--r--   0        0        0     2149 2022-09-15 21:51:48.846733 evofr-0.1.19/evofr/infer/InferMCMC.py
+-rw-r--r--   0        0        0     3278 2023-01-25 21:51:20.522220 evofr-0.1.19/evofr/infer/InferSVI.py
+-rw-r--r--   0        0        0     2478 2022-08-27 00:43:53.040621 evofr-0.1.19/evofr/infer/MCMC_handler.py
+-rw-r--r--   0        0        0     2995 2022-08-27 00:43:53.019730 evofr-0.1.19/evofr/infer/SVI_handler.py
+-rw-r--r--   0        0        0     1652 2023-01-25 21:51:20.522616 evofr-0.1.19/evofr/infer/SamplePrior.py
+-rw-r--r--   0        0        0      302 2023-01-25 21:51:20.523080 evofr-0.1.19/evofr/infer/__init__.py
+-rw-r--r--   0        0        0       78 2023-01-25 21:51:20.523543 evofr-0.1.19/evofr/infer/backends.py
+-rw-r--r--   0        0        0      289 2022-12-21 20:12:56.042653 evofr-0.1.19/evofr/models/__init__.py
+-rw-r--r--   0        0        0     5083 2023-06-05 20:35:41.520530 evofr-0.1.19/evofr/models/mlr_hierarchical.py
+-rw-r--r--   0        0        0     9727 2023-02-01 20:10:34.871076 evofr-0.1.19/evofr/models/mlr_innovation.py
+-rw-r--r--   0        0        0    11893 2022-11-08 19:03:50.750502 evofr-0.1.19/evofr/models/mlr_nowcast.py
+-rw-r--r--   0        0        0     2886 2022-09-30 21:23:27.866766 evofr-0.1.19/evofr/models/mlr_spline.py
+-rw-r--r--   0        0        0      700 2022-08-27 20:30:22.404715 evofr-0.1.19/evofr/models/model_spec.py
+-rw-r--r--   0        0        0     4553 2023-04-05 18:05:00.919362 evofr-0.1.19/evofr/models/multinomial_logistic_regression.py
+-rw-r--r--   0        0        0     5778 2023-04-20 23:41:11.598062 evofr-0.1.19/evofr/models/mutational_fitness_mlr.py
+-rw-r--r--   0        0        0     3333 2022-09-26 17:53:00.939634 evofr-0.1.19/evofr/models/piantham_model.py
+-rw-r--r--   0        0        0     2243 2022-08-27 01:00:23.614755 evofr-0.1.19/evofr/models/renewal_model/LAS.py
+-rw-r--r--   0        0        0      257 2022-11-08 19:05:19.255557 evofr-0.1.19/evofr/models/renewal_model/__init__.py
+-rw-r--r--   0        0        0      149 2022-07-13 00:53:30.188448 evofr-0.1.19/evofr/models/renewal_model/basis_functions/__init__.py
+-rw-r--r--   0        0        0      198 2022-07-08 20:37:47.686469 evofr-0.1.19/evofr/models/renewal_model/basis_functions/basis_fns.py
+-rw-r--r--   0        0        0     3391 2022-07-14 20:27:07.660069 evofr-0.1.19/evofr/models/renewal_model/basis_functions/hilbert_space_gaussian_process.py
+-rw-r--r--   0        0        0     4778 2022-09-30 21:38:46.300190 evofr-0.1.19/evofr/models/renewal_model/basis_functions/splines.py
+-rw-r--r--   0        0        0     6540 2023-04-06 23:46:59.942673 evofr-0.1.19/evofr/models/renewal_model/model_factories.py
+-rw-r--r--   0        0        0     2405 2023-01-10 22:30:08.131767 evofr-0.1.19/evofr/models/renewal_model/model_functions.py
+-rw-r--r--   0        0        0     1366 2023-01-10 22:30:08.132058 evofr-0.1.19/evofr/models/renewal_model/model_helpers.py
+-rw-r--r--   0        0        0    11983 2023-06-05 20:37:51.670043 evofr-0.1.19/evofr/models/renewal_model/model_options.py
+-rw-r--r--   0        0        0     1655 2023-05-25 17:19:40.179597 evofr-0.1.19/evofr/models/renewal_model/renewal_model.py
+-rw-r--r--   0        0        0     4392 2022-09-10 15:55:23.454857 evofr-0.1.19/evofr/models/renewal_model/renewal_regression.py
+-rw-r--r--   0        0        0     4898 2023-06-05 20:32:08.169834 evofr-0.1.19/evofr/models/renewal_model/renewal_single_variant.py
+-rw-r--r--   0        0        0      831 2022-07-08 20:51:40.490887 evofr-0.1.19/evofr/models/renewal_model/spline_incidence.py
+-rw-r--r--   0        0        0       62 2023-01-12 23:49:44.920731 evofr-0.1.19/evofr/plotting/__init__.py
+-rw-r--r--   0        0        0    11903 2023-01-12 23:49:44.921903 evofr-0.1.19/evofr/plotting/plot_functions.py
+-rw-r--r--   0        0        0    11557 2023-01-25 21:51:20.525631 evofr-0.1.19/evofr/plotting/plotting_classes.py
+-rw-r--r--   0        0        0       97 2022-12-22 03:54:22.139076 evofr-0.1.19/evofr/posterior/__init__.py
+-rw-r--r--   0        0        0     2996 2022-12-22 03:54:22.139787 evofr-0.1.19/evofr/posterior/posterior_handler.py
+-rw-r--r--   0        0        0    14113 2023-04-06 23:46:59.943078 evofr-0.1.19/evofr/posterior/posterior_helpers.py
+-rw-r--r--   0        0        0      512 2023-06-05 20:39:48.949092 evofr-0.1.19/pyproject.toml
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 evofr-0.1.19/setup.py
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 evofr-0.1.19/PKG-INFO
```

### Comparing `evofr-0.1.18/LICENSE.txt` & `evofr-0.1.19/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/__init__.py` & `evofr-0.1.19/evofr/__init__.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/data/case_counts.py` & `evofr-0.1.19/evofr/data/case_counts.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/data/case_frequencies.py` & `evofr-0.1.19/evofr/data/case_frequencies.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/data/data_helpers.py` & `evofr-0.1.19/evofr/data/data_helpers.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/data/hier_cases.py` & `evofr-0.1.19/evofr/data/hier_cases.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/data/hier_frequencies.py` & `evofr-0.1.19/evofr/data/hier_frequencies.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/data/variant_frequencies.py` & `evofr-0.1.19/evofr/data/variant_frequencies.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/infer/BJBackendsScrap.py` & `evofr-0.1.19/evofr/infer/BJBackendsScrap.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/infer/InferBlackJax.py` & `evofr-0.1.19/evofr/infer/InferBlackJax.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/infer/InferMCMC.py` & `evofr-0.1.19/evofr/infer/InferMCMC.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/infer/InferSVI.py` & `evofr-0.1.19/evofr/infer/InferSVI.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/infer/MCMC_handler.py` & `evofr-0.1.19/evofr/infer/MCMC_handler.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/infer/SVI_handler.py` & `evofr-0.1.19/evofr/infer/SVI_handler.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/infer/SamplePrior.py` & `evofr-0.1.19/evofr/infer/SamplePrior.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/mlr_hierarchical.py` & `evofr-0.1.19/evofr/models/mlr_hierarchical.py`

 * *Files 17% similar despite different names*

```diff
@@ -84,17 +84,15 @@
     numpyro.deterministic("freq", softmax(logits, axis=1))
 
     # Compute growth advantage from model
     if tau is not None:
         numpyro.deterministic(
             "ga", jnp.exp(beta[-1, :-1, :] * tau)
         )  # Last row corresponds to linear predictor / growth advantage
-        numpyro.deterministic(
-            "ga_loc", jnp.exp(beta_loc[-1, :, 0] * tau)
-        )
+        numpyro.deterministic("ga_loc", jnp.exp(beta_loc[-1, :, 0] * tau))
 
 
 class HierMLR(ModelSpec):
     def __init__(self, tau: float, pool_scale: Optional[float] = None) -> None:
         """Construct ModelSpec for Hierarchial multinomial logistic regression.
 
         Parameters
@@ -131,7 +129,31 @@
         X_flat = MultinomialLogisticRegression.make_ols_feature(start, stop)
         return np.stack([X_flat] * n_groups, axis=-1)
 
     def augment_data(self, data: dict) -> None:
         T, G = data["N"].shape
         data["tau"] = self.tau
         data["X"] = self.make_ols_feature(0, T, G)
+
+    @staticmethod
+    def forecast_frequencies(samples, forecast_L):
+        """
+        Use posterior beta to forecast posterior frequencies.
+        """
+
+        # Making feature matrix for forecasting
+        last_T = samples["freq"].shape[1]
+        n_groups = samples["freq"].shape[-1]
+
+        X = HierMLR.make_ols_feature(
+            start=last_T, stop=last_T + forecast_L, n_groups=n_groups
+        )
+
+        # (T, F, G) times (F, V, G) -> (T, V, G)
+        dot_by_group = vmap(jnp.dot, in_axes=(-1, -1), out_axes=-1)
+        dbg_by_sample = vmap(dot_by_group, in_axes=(None, 0), out_axes=0)
+
+        # Creating frequencies from posterior beta
+        beta = jnp.array(samples["beta"])
+        logits = dbg_by_sample(X, beta)
+        samples["freq_forecast"] = softmax(logits, axis=-2)  # (S, T, V, G)
+        return samples
```

### Comparing `evofr-0.1.18/evofr/models/mlr_innovation.py` & `evofr-0.1.19/evofr/models/mlr_innovation.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/mlr_nowcast.py` & `evofr-0.1.19/evofr/models/mlr_nowcast.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/mlr_spline.py` & `evofr-0.1.19/evofr/models/mlr_spline.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/model_spec.py` & `evofr-0.1.19/evofr/models/model_spec.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/multinomial_logistic_regression.py` & `evofr-0.1.19/evofr/models/multinomial_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/mutational_fitness_mlr.py` & `evofr-0.1.19/evofr/models/mutational_fitness_mlr.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/piantham_model.py` & `evofr-0.1.19/evofr/models/piantham_model.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/renewal_model/LAS.py` & `evofr-0.1.19/evofr/models/renewal_model/LAS.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/renewal_model/basis_functions/hilbert_space_gaussian_process.py` & `evofr-0.1.19/evofr/models/renewal_model/basis_functions/hilbert_space_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/renewal_model/basis_functions/splines.py` & `evofr-0.1.19/evofr/models/renewal_model/basis_functions/splines.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/renewal_model/model_factories.py` & `evofr-0.1.19/evofr/models/renewal_model/model_factories.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/renewal_model/model_functions.py` & `evofr-0.1.19/evofr/models/renewal_model/model_functions.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/renewal_model/model_helpers.py` & `evofr-0.1.19/evofr/models/renewal_model/model_helpers.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/renewal_model/model_options.py` & `evofr-0.1.19/evofr/models/renewal_model/model_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         return R
 
 
 class GARW:
     def __init__(
         self, gam_prior=0.5, gam_delta_prior=0.5, prior_family="Cauchy"
     ):
-        """Construct FixedGrowthAdvantage model.
+        """Construct GARW model.
         Parameters
         ----------
         gam_prior:
             hyper_prior for scale of Rt increment.
         gam_delta_prior:
             hyper_prior for scale of growth advantage increment.
         prior_family:
```

### Comparing `evofr-0.1.18/evofr/models/renewal_model/renewal_model.py` & `evofr-0.1.19/evofr/models/renewal_model/renewal_model.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/renewal_model/renewal_regression.py` & `evofr-0.1.19/evofr/models/renewal_model/renewal_regression.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/models/renewal_model/renewal_single_variant.py` & `evofr-0.1.19/evofr/models/renewal_model/renewal_single_variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import jax.numpy as jnp
 import numpy as np
 
 from evofr.models.model_spec import ModelSpec
 from evofr.models.renewal_model.model_helpers import to_survivor_function
 from .basis_functions import BasisFunction, Spline
 
-from .LAS import LaplaceRandomWalk
 from .model_functions import forward_simulate_I_and_prev, reporting_to_vec
 from .model_options import NegBinomCases
 
 import numpyro
 import numpyro.distributions as dist
 
 
@@ -30,16 +29,16 @@
     if CaseLik is None:
         CaseLik = NegBinomCases()
 
     T, k = X.shape
     obs_range = jnp.arange(seed_L, seed_L + T, 1)
 
     # Effective Reproduction number likelihood
-    gam = numpyro.sample("gam", dist.HalfNormal(1.0))
-    beta_0 = numpyro.sample("beta_0", dist.Normal(0.0, 1.0))
+    gam = numpyro.sample("gam", dist.HalfNormal(0.5))
+    beta_0 = numpyro.sample("beta_0", dist.Normal(0.0, 0.5))
     with numpyro.plate("N_steps_base", k - 1):
         beta_rw_step = numpyro.sample("beta_rw_step", dist.Laplace()) * gam
         beta_rw = numpyro.deterministic("beta_rw", jnp.cumsum(beta_rw_step))
 
     # Combine increments and starting position
     beta_rw = jnp.append(jnp.zeros(1), beta_rw)
     beta = beta_0 + beta_rw
```

### Comparing `evofr-0.1.18/evofr/models/renewal_model/spline_incidence.py` & `evofr-0.1.19/evofr/models/renewal_model/spline_incidence.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/plotting/plot_functions.py` & `evofr-0.1.19/evofr/plotting/plot_functions.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/plotting/plotting_classes.py` & `evofr-0.1.19/evofr/plotting/plotting_classes.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/posterior/posterior_handler.py` & `evofr-0.1.19/evofr/posterior/posterior_handler.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/evofr/posterior/posterior_helpers.py` & `evofr-0.1.19/evofr/posterior/posterior_helpers.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.18/pyproject.toml` & `evofr-0.1.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evofr"
-version = "0.1.18"
+version = "0.1.19"
 description = "Tools for evolutionary forecasting."
 authors = ["marlinfiggins <marlinfiggins@gmail.com>"]
 license = "AGPL-3.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.22.4"
```

### Comparing `evofr-0.1.18/setup.py` & `evofr-0.1.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'jaxlib>=0.3.10,<0.4.0',
  'numpy>=1.22.4,<2.0.0',
  'numpyro>=0.9.2,<0.10.0',
  'pandas>=1.4.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'evofr',
-    'version': '0.1.18',
+    'version': '0.1.19',
     'description': 'Tools for evolutionary forecasting.',
     'long_description': 'None',
     'author': 'marlinfiggins',
     'author_email': 'marlinfiggins@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `evofr-0.1.18/PKG-INFO` & `evofr-0.1.19/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evofr
-Version: 0.1.18
+Version: 0.1.19
 Summary: Tools for evolutionary forecasting.
 License: AGPL-3.0
 Author: marlinfiggins
 Author-email: marlinfiggins@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

