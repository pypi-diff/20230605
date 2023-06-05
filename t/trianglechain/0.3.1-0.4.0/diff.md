# Comparing `tmp/trianglechain-0.3.1.tar.gz` & `tmp/trianglechain-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trianglechain-0.3.1.tar", last modified: Thu May 11 08:30:40 2023, max compression
+gzip compressed data, was "trianglechain-0.4.0.tar", last modified: Mon Jun  5 12:30:46 2023, max compression
```

## Comparing `trianglechain-0.3.1.tar` & `trianglechain-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.306219 trianglechain-0.3.1/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-05-04 11:29:54.000000 trianglechain-0.3.1/AUTHORS.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-05-04 11:29:54.000000 trianglechain-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1302 2023-05-11 08:30:03.000000 trianglechain-0.3.1/HISTORY.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-05-04 11:29:54.000000 trianglechain-0.3.1/LICENSE
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-05-04 11:29:54.000000 trianglechain-0.3.1/MANIFEST.in
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-05-11 08:30:40.306289 trianglechain-0.3.1/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-05-04 11:29:54.000000 trianglechain-0.3.1/README.md
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-05-04 11:29:54.000000 trianglechain-0.3.1/pyproject.toml
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-05-11 08:30:40.306632 trianglechain-0.3.1/setup.cfg
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.301468 trianglechain-0.3.1/src/
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.304486 trianglechain-0.3.1/src/trianglechain/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/BaseChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/LineChain.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    27750 2023-05-11 08:01:21.000000 trianglechain-0.3.1/src/trianglechain/TriangleChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-05-11 08:29:44.000000 trianglechain-0.3.1/src/trianglechain/__init__.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    10416 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/density_estimation.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16438 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/make_subplots.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/params.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/utils_pj_hpd.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    18937 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/utils_plots.py
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.305330 trianglechain-0.3.1/src/trianglechain.egg-info/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/SOURCES.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/dependency_links.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:24:36.000000 trianglechain-0.3.1/src/trianglechain.egg-info/not-zip-safe
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/requires.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/top_level.txt
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.306046 trianglechain-0.3.1/tests/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_linechain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_params.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_trianglechain.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.771258 trianglechain-0.4.0/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-05-04 11:29:54.000000 trianglechain-0.4.0/AUTHORS.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-05-04 11:29:54.000000 trianglechain-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-06-05 12:29:15.000000 trianglechain-0.4.0/HISTORY.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-05-04 11:29:54.000000 trianglechain-0.4.0/LICENSE
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-05-04 11:29:54.000000 trianglechain-0.4.0/MANIFEST.in
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-05 12:30:46.771324 trianglechain-0.4.0/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-05-04 11:29:54.000000 trianglechain-0.4.0/README.md
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-05-04 11:29:54.000000 trianglechain-0.4.0/pyproject.toml
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-06-05 12:30:46.771685 trianglechain-0.4.0/setup.cfg
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.765245 trianglechain-0.4.0/src/
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.769211 trianglechain-0.4.0/src/trianglechain/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/BaseChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/LineChain.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    28003 2023-06-05 12:25:46.000000 trianglechain-0.4.0/src/trianglechain/TriangleChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-06-05 12:29:22.000000 trianglechain-0.4.0/src/trianglechain/__init__.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9932 2023-06-05 12:25:46.000000 trianglechain-0.4.0/src/trianglechain/density_estimation.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16850 2023-06-05 12:25:46.000000 trianglechain-0.4.0/src/trianglechain/make_subplots.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/params.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-05-04 11:29:54.000000 trianglechain-0.4.0/src/trianglechain/utils_pj_hpd.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    19680 2023-06-05 12:25:46.000000 trianglechain-0.4.0/src/trianglechain/utils_plots.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.770357 trianglechain-0.4.0/src/trianglechain.egg-info/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:24:36.000000 trianglechain-0.4.0/src/trianglechain.egg-info/not-zip-safe
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/requires.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-06-05 12:30:46.000000 trianglechain-0.4.0/src/trianglechain.egg-info/top_level.txt
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-05 12:30:46.771136 trianglechain-0.4.0/tests/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_linechain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_params.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-05-04 11:29:54.000000 trianglechain-0.4.0/tests/test_trianglechain.py
```

### Comparing `trianglechain-0.3.1/CONTRIBUTING.rst` & `trianglechain-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/HISTORY.rst` & `trianglechain-0.4.0/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 .. :changelog:
 
 History
 -------
 
+0.4.0 (2023-06-05)
+++++++++++++++++++
+
+* FEATURE: n_sigma_for_one_sided_tail free parameter to manually set the threshold when to use a 2-sided or 1-sided interval
+* FIX: correct normalization when using samples with prob
+* FIX: avoid upper limits with +- 0.0 and lower limits with -- 0.0
+
 0.3.1 (2023-05-11)
 ++++++++++++++++++
 
 * FIX: showing labels in most upper left corner when using only the upper triangle
-* improved documenation
+* improved documentation
 
 0.3.0 (2023-04-26)
 ++++++++++++++++++
 
 * FEATURE: LineChain class to handle line chains
 * FEATURE: params_from to select params from one specific input
 * FEATURE: add_derived_params to add derived params to the input array
 * FEATURE: new possible input type: pandas DataFrame
 * FEATURE: colors are varied automatically according the matplotlib color cycle
 * FEATURE: when computing bestfits and uncertainties, it automatically detects if to show bestfit +/- uncertainty or a lower/upper limit.
 * FIX: ylimits in 1D plots
 * FIX: tick values when choosing many ticks
-* improved documenation
+* improved documentation
 * dependency cleanup
 
 0.2.1 (2023-03-20)
 ++++++++++++++++++
 
 * FIX: bug in 1D histograms when using prob
```

### Comparing `trianglechain-0.3.1/LICENSE` & `trianglechain-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/PKG-INFO` & `trianglechain-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.3.1
+Version: 0.4.0
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.3.1/README.md` & `trianglechain-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/pyproject.toml` & `trianglechain-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/setup.cfg` & `trianglechain-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/src/trianglechain/BaseChain.py` & `trianglechain-0.4.0/src/trianglechain/BaseChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/src/trianglechain/LineChain.py` & `trianglechain-0.4.0/src/trianglechain/LineChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/src/trianglechain/TriangleChain.py` & `trianglechain-0.4.0/src/trianglechain/TriangleChain.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
     grid=False,
     labels=None,
     plot_histograms_1D=True,
     show_values=False,
     bestfit_method="mode",
     levels_method="hdi",
     credible_interval=0.68,
+    n_sigma_for_one_sided_tail=3,
     lnprobs=None,
     scatter_vline_1D=False,
     label=None,
     density_estimation_method="smoothing",
     n_ticks=3,
     tick_length=3,
     alpha1D=1,
@@ -244,14 +245,17 @@
         method that should be used for the bestfit value
         options: "mode", "median", "mean", default: "mode"
     :param levels_method: string
         method that should be used for the levels
         options: "hdi", "credible_interval", default: "hdi"
     :param credible_interval: float
         credible interval for the levels, default: 0.68
+    :param n_sigma_for_one_sided_tail: how many sigma should be used to decide if one
+        tailed credible interval should be used
+        defaults to 3
     :param lnprobs: None or array
         log probabilities attached to the samples for the level estimation,
         default: None
     :param scatter_vline_1D: bool
         if a vertical line should be plotted at the scatter points in the 1D histograms,
         default: False
     :param label: string
@@ -434,14 +438,15 @@
                     label=label,
                     hist_kwargs=hist_kwargs,
                     fill=fill,
                     lnprobs=lnprobs,
                     levels_method=levels_method,
                     bestfit_method=bestfit_method,
                     credible_interval=credible_interval,
+                    sigma_one_tail=n_sigma_for_one_sided_tail,
                     label_fontsize=label_fontsize,
                 )
 
     if scatter_vline_1D:
         for i in range(n_dim):
             if columns[i] != "EMPTY":
                 axc = get_current_ax(ax, tri, i, i)
```

### Comparing `trianglechain-0.3.1/src/trianglechain/bestfit.py` & `trianglechain-0.4.0/src/trianglechain/bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/src/trianglechain/density_estimation.py` & `trianglechain-0.4.0/src/trianglechain/density_estimation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Tomasz Kacprzak, Silvan Fischbacher
 
 
 import numpy as np
 import scipy
-import warnings
 from trianglechain.utils_plots import (
     safe_normalise,
     normalise,
     pixel_coords,
     get_smoothing_sigma,
 )
 
@@ -115,25 +114,21 @@
     Create a histogram of the data
 
     :param data: data to create histogram from
     :param prob: weights for the data
     :param binedges: bin edges for the histogram
     :return: histogram
     """
-
     if prob is None:
         prob1D, _ = np.histogram(data, bins=binedges)
 
     else:
         assert prob.shape[0] == data.shape[0]
 
-        hist_counts, _ = np.histogram(data, bins=binedges)
-        hist_prob, _ = np.histogram(data, bins=binedges, weights=prob)
-        prob1D = hist_prob / hist_counts.astype(float)
-        prob1D[hist_counts == 0] = 0
+        prob1D, _ = np.histogram(data, bins=binedges, weights=prob)
 
     prob1D = safe_normalise(prob1D)
     prob1D = np.ma.array(prob1D, mask=prob1D == 0)
     return prob1D
 
 
 def get_density_grid_2D(
@@ -259,25 +254,17 @@
     if prob is None:
         prob2d = np.histogram2d(*data_panel, bins=(bins_x, bins_y))[0].T.astype(
             np.float32
         )
 
     else:
         assert prob.shape[0] == data_panel[0].shape[0]
-
-        hist2d_counts = np.histogram2d(*data_panel, bins=(bins_x, bins_y))[0].T.astype(
-            np.float32
-        )
-        hist2d_prob = np.histogram2d(*data_panel, weights=prob, bins=(bins_x, bins_y))[
+        prob2d = np.histogram2d(*data_panel, weights=prob, bins=(bins_x, bins_y))[
             0
         ].T.astype(np.float32)
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            prob2d = hist2d_prob / hist2d_counts.astype(float)
-        prob2d[hist2d_counts == 0] = 0
 
     if np.sum(prob2d) > 0:
         prob2d = prob2d / np.sum(prob2d)
 
     return prob2d
```

### Comparing `trianglechain-0.3.1/src/trianglechain/limits.py` & `trianglechain-0.4.0/src/trianglechain/limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/src/trianglechain/make_subplots.py` & `trianglechain-0.4.0/src/trianglechain/make_subplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     color_hist="k",
     alpha1D=1,
     fill=False,
     lnprobs=None,
     levels_method="hdi",
     bestfit_method="mean",
     credible_interval=0.68,
+    sigma_one_tail=3,
     label_fontsize=12,
 ):
     """
     Plot 1D histogram and density estimation.
 
     :param axc: matplotlib axis
         axis of the plot
@@ -92,14 +93,17 @@
         logprobabilites used for the bestfit and uncertainty finding
     :param levels_method: {"hdi", "percentile", "PJ_HPD"}
         method how to compute the uncertainty
     :param bestfit_method: {"mode", "mean", "median", "best_sample"}
         method how to compute the bestfit
     :param credible_interval: float in [0, 1]
         credible interval of the uncertainty bar
+    :param sigma_one_tail: how many sigma should be used to decide if one tailed
+        credible interval should be used
+        defaults to 3
     :param label_fontsize: int or float
         fontsize of the label of the parameters
     """
 
     try:
         d = data[column]
     except Exception:
@@ -151,27 +155,29 @@
             column,
             data,
             lnprobs,
             label=param_label,
             levels_method=levels_method,
             bestfit_method=bestfit_method,
             credible_interval=credible_interval,
+            sigma_one_tail=sigma_one_tail,
             label_fontsize=label_fontsize,
         )
 
 
 def add_values(
     axc,
     column,
     data,
     lnprobs,
     label,
     levels_method="hdi",
     bestfit_method="mean",
     credible_interval=0.68,
+    sigma_one_tail=3,
     label_fontsize=12,
 ):
     """
     Add values of bestfit and uncertainty to the plot.
 
     :param axc: matplotlib axis
         axis of the plot
@@ -185,28 +191,32 @@
         label of the plot
     :param levels_method: {"hdi", "percentile", "PJ_HPD"}
         method how to compute the uncertainty, default is hdi
     :param bestfit_method: {"mode", "mean", "median", "best_sample"}
         method how to compute the bestfit, default is mean
     :param credible_interval: float in [0, 1]
         credible interval of the uncertainty bar, default is 0.68
+    :param sigma_one_tail: how many sigma should be used to decide if one tailed
+        credible interval should be used
+        defaults to 3
     :param label_fontsize: int or float
         fontsize of the label of the parameters, default is 12
     """
     two_tail, str_bf, up, low = get_values(
         column,
         data,
         lnprobs,
         levels_method=levels_method,
         bestfit_method=bestfit_method,
         credible_interval=credible_interval,
+        sigma_one_tail=sigma_one_tail,
     )
     if two_tail:
         axc.set_title(
-            r"{} $= {}^{{+{} }}_{{-{} }}$".format(label, str_bf, up, low),
+            r"{} $= {}^{{{} }}_{{{} }}$".format(label, str_bf, up, low),
             fontsize=label_fontsize,
         )
     else:
         side = str_bf
         limit = up
         if side[0] == "l":
             axc.set_title(
```

### Comparing `trianglechain-0.3.1/src/trianglechain/params.py` & `trianglechain-0.4.0/src/trianglechain/params.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/src/trianglechain/utils_pj_hpd.py` & `trianglechain-0.4.0/src/trianglechain/utils_pj_hpd.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/src/trianglechain/utils_plots.py` & `trianglechain-0.4.0/src/trianglechain/utils_plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -291,40 +291,58 @@
 def get_values(
     column,
     data,
     lnprobs,
     levels_method="hdi",
     bestfit_method="mean",
     credible_interval=0.68,
+    sigma_one_tail=3,
 ):
     """
     Get the values for the best fit and the uncertainty.
 
     :param column: The column.
     :param data: The data.
     :param lnprobs: The log probabilities.
     :param levels_method: The method to compute the uncertainty.
     :param bestfit_method: The method to compute the best fit.
     :param credible_interval: The credible interval.
+    :param sigma_one_tail: how many sigma should be used to decide if one tailed
+        credible interval should be used
+        defaults to 3
     :return: The best fit and the uncertainty.
     """
     lim, two_tail, side = limits.get_levels(
         data[column],
         lnprobs,
         levels_method,
         credible_interval,
+        sigma_one_tail=sigma_one_tail,
     )
     if two_tail:
         lower, upper = lim
         bf = bestfit.get_bestfit(data[column], lnprobs, bestfit_method)
         uncertainty = (upper - lower) / 2
         rounding_digit, frmt = get_rounding_digit(uncertainty)
         str_bf = f"{frmt}".format(np.around(bf, rounding_digit))
-        low = f"{frmt}".format(np.around(bf - lower, rounding_digit))
-        up = f"{frmt}".format(np.around(upper - bf, rounding_digit))
+
+        if np.around(bf - lower, rounding_digit) < 0:
+            # special case where the bestfit is not in the interval
+            low = f"{frmt}".format(np.around(bf - lower, rounding_digit))
+        else:
+            # take abs for the special case -0.
+            low = f"-{frmt}".format(abs(np.around(bf - lower, rounding_digit)))
+
+        if np.around(upper - bf, rounding_digit) < 0:
+            # special case where the bestfit is not in the interval
+            up = f"{frmt}".format(np.around(upper - bf, rounding_digit))
+        else:
+            # take abs for the special case -0.
+            up = f"+{frmt}".format(abs(np.around(upper - bf, rounding_digit)))
+
         return two_tail, str_bf, up, low
     else:
         uncertainty_estimate = np.std(data[column])
         rounding_digit, frmt = get_rounding_digit(uncertainty_estimate)
         return two_tail, side, f"{frmt}".format(np.around(lim, rounding_digit)), None
```

### Comparing `trianglechain-0.3.1/src/trianglechain.egg-info/PKG-INFO` & `trianglechain-0.4.0/src/trianglechain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.3.1
+Version: 0.4.0
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.3.1/src/trianglechain.egg-info/SOURCES.txt` & `trianglechain-0.4.0/src/trianglechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/tests/test_bestfit.py` & `trianglechain-0.4.0/tests/test_bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/tests/test_limits.py` & `trianglechain-0.4.0/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/tests/test_linechain.py` & `trianglechain-0.4.0/tests/test_linechain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/tests/test_params.py` & `trianglechain-0.4.0/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.1/tests/test_trianglechain.py` & `trianglechain-0.4.0/tests/test_trianglechain.py`

 * *Files identical despite different names*

