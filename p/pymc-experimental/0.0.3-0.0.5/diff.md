# Comparing `tmp/pymc-experimental-0.0.3.tar.gz` & `tmp/pymc-experimental-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-experimental-0.0.3.tar", last modified: Mon May 29 09:55:34 2023, max compression
+gzip compressed data, was "pymc-experimental-0.0.5.tar", last modified: Mon Jun  5 16:04:57 2023, max compression
```

## Comparing `pymc-experimental-0.0.3.tar` & `pymc-experimental-0.0.5.tar`

### file list

```diff
@@ -1,69 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.548601 pymc-experimental-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-29 09:55:34.548601 pymc-experimental-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.528601 pymc-experimental-0.0.3/pymc_experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.536601 pymc-experimental-0.0.3/pymc_experimental/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/histogram_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.536601 pymc-experimental-0.0.3/pymc_experimental/distributions/multivariate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/multivariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/multivariate/r2d2m2cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.536601 pymc-experimental-0.0.3/pymc_experimental/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/gp/latent_approx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.540601 pymc-experimental-0.0.3/pymc_experimental/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/inference/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/inference/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20459 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.540601 pymc-experimental-0.0.3/pymc_experimental/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.544601 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_histogram_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_prior_from_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.544601 pymc-experimental-0.0.3/pymc_experimental/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/utils/test_model_fgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.548601 pymc-experimental-0.0.3/pymc_experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/model_fgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/pytensorf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.532600 pymc-experimental-0.0.3/pymc_experimental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-29 09:55:34.548601 pymc-experimental-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.155985 pymc-experimental-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-05 16:04:57.155985 pymc-experimental-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.139985 pymc-experimental-0.0.5/pymc_experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.143985 pymc-experimental-0.0.5/pymc_experimental/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/histogram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.143985 pymc-experimental-0.0.5/pymc_experimental/distributions/multivariate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/multivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/multivariate/r2d2m2cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.143985 pymc-experimental-0.0.5/pymc_experimental/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/gp/latent_approx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.143985 pymc-experimental-0.0.5/pymc_experimental/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/inference/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/inference/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24222 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.147985 pymc-experimental-0.0.5/pymc_experimental/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/model_transform/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/model_transform/conditioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.147985 pymc-experimental-0.0.5/pymc_experimental/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.151985 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_multivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.151985 pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/test_conditioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_histogram_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_prior_from_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.151985 pymc-experimental-0.0.5/pymc_experimental/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/utils/test_model_fgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.155985 pymc-experimental-0.0.5/pymc_experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/model_fgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/pytensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.139985 pymc-experimental-0.0.5/pymc_experimental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-05 16:04:57.155985 pymc-experimental-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/setup.py
```

### Comparing `pymc-experimental-0.0.3/CODE_OF_CONDUCT.md` & `pymc-experimental-0.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/LICENSE` & `pymc-experimental-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/PKG-INFO` & `pymc-experimental-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.3
+Version: 0.0.5
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,56 +1,57 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.3 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.5 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Operating System :: OS Independent Requires-Python: >=3.8
-Description-Content-Type: text/markdown Provides-Extra: dask_histogram
-Provides-Extra: histogram Provides-Extra: complete Provides-Extra: dev License-
-File: LICENSE # Welcome to `pymc-experimental` [Contribute_with_Gitpod]
-[Codecov Badge] As PyMC continues to mature and expand its functionality to
-accommodate more domains of application, we increasingly see cutting-edge
-methodologies, highly specialized statistical distributions, and complex models
-appear. While this adds to the functionality and relevance of the project, it
-can also introduce instability and impose a burden on testing and quality
-control. To reduce the burden on the main `pymc` repository, this `pymc-
-experimental` repository can become the aggregator and testing ground for new
-additions to PyMC. This may include unusual probability distributions, advanced
-model fitting algorithms, innovative yet not fully tested methods or any code
-that may be inappropriate to include in the `pymc` repository, but may want to
-be made available to users. The `pymc-experimental` repository can be
-understood as the first step in the PyMC development pipeline, where all novel
-code is introduced until it is obvious that it belongs in the main repository.
-We hope that this organization improves the stability and streamlines the
-testing overhead of the `pymc` repository, while allowing users and developers
-to test and evaluate cutting-edge methods and not yet fully mature features.
-`pymc-experimental` would be designed to mirror the namespaces in `pymc` to
-make usage and migration as easy as possible. For example, a `ParabolicFractal`
-distribution could be used analogously to those in `pymc`: ```python import
-pymc as pm import pymc_experimental as pmx with pm.Model(): alpha =
-pmx.ParabolicFractal('alpha', b=1, c=1) ... ``` ## Questions ### What belongs
-in `pymc-experimental`? - newly-implemented statistical methods, for example
-step methods or model construction helpers - distributions that are tricky to
-sample from or test - infrequently-used fitting methods or distributions - any
-code that requires additional optimization before it can be used in practice
-### What does not belong in `pymc-experimental`? - Case studies -
-Implementations that cannot be applied generically, for example because they
-are tied to variables from a toy example ### Should there be more than one add-
-on repository? Since there is a lot of code that we may not want in the main
-repository, does it make sense to have more than one additional repository? For
-example, `pymc-experimental` may just include methods that are not fully
-developed, tested and trusted, while code that is known to work well and has
-adequate test coverage, but is still too specialized to become part of `pymc`
-could reside in a `pymc-extras` (or similar) repository. ### Unanswered
-questions & ToDos This project is still young and many things have not been
-answered or implemented. Please get involved! * What are guidelines for
-organizing submodules? * Proposal: No default imports of WIP/unstable
-submodules. By importing manually we can avoid breaking the package if a
-submodule breaks, for example because of an updated dependency.
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Operating System :: OS
+Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dask_histogram Provides-Extra: histogram Provides-Extra:
+complete Provides-Extra: dev License-File: LICENSE # Welcome to `pymc-
+experimental` [Contribute_with_Gitpod] [Codecov Badge] As PyMC continues to
+mature and expand its functionality to accommodate more domains of application,
+we increasingly see cutting-edge methodologies, highly specialized statistical
+distributions, and complex models appear. While this adds to the functionality
+and relevance of the project, it can also introduce instability and impose a
+burden on testing and quality control. To reduce the burden on the main `pymc`
+repository, this `pymc-experimental` repository can become the aggregator and
+testing ground for new additions to PyMC. This may include unusual probability
+distributions, advanced model fitting algorithms, innovative yet not fully
+tested methods or any code that may be inappropriate to include in the `pymc`
+repository, but may want to be made available to users. The `pymc-experimental`
+repository can be understood as the first step in the PyMC development
+pipeline, where all novel code is introduced until it is obvious that it
+belongs in the main repository. We hope that this organization improves the
+stability and streamlines the testing overhead of the `pymc` repository, while
+allowing users and developers to test and evaluate cutting-edge methods and not
+yet fully mature features. `pymc-experimental` would be designed to mirror the
+namespaces in `pymc` to make usage and migration as easy as possible. For
+example, a `ParabolicFractal` distribution could be used analogously to those
+in `pymc`: ```python import pymc as pm import pymc_experimental as pmx with
+pm.Model(): alpha = pmx.ParabolicFractal('alpha', b=1, c=1) ... ``` ##
+Questions ### What belongs in `pymc-experimental`? - newly-implemented
+statistical methods, for example step methods or model construction helpers -
+distributions that are tricky to sample from or test - infrequently-used
+fitting methods or distributions - any code that requires additional
+optimization before it can be used in practice ### What does not belong in
+`pymc-experimental`? - Case studies - Implementations that cannot be applied
+generically, for example because they are tied to variables from a toy example
+### Should there be more than one add-on repository? Since there is a lot of
+code that we may not want in the main repository, does it make sense to have
+more than one additional repository? For example, `pymc-experimental` may just
+include methods that are not fully developed, tested and trusted, while code
+that is known to work well and has adequate test coverage, but is still too
+specialized to become part of `pymc` could reside in a `pymc-extras` (or
+similar) repository. ### Unanswered questions & ToDos This project is still
+young and many things have not been answered or implemented. Please get
+involved! * What are guidelines for organizing submodules? * Proposal: No
+default imports of WIP/unstable submodules. By importing manually we can avoid
+breaking the package if a submodule breaks, for example because of an updated
+dependency.
```

### Comparing `pymc-experimental-0.0.3/README.md` & `pymc-experimental-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/__init__.py` & `pymc-experimental-0.0.5/pymc_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/distributions/__init__.py` & `pymc-experimental-0.0.5/pymc_experimental/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/distributions/continuous.py` & `pymc-experimental-0.0.5/pymc_experimental/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/distributions/discrete.py` & `pymc-experimental-0.0.5/pymc_experimental/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/distributions/histogram_utils.py` & `pymc-experimental-0.0.5/pymc_experimental/distributions/histogram_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/distributions/multivariate/r2d2m2cp.py` & `pymc-experimental-0.0.5/pymc_experimental/distributions/multivariate/r2d2m2cp.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/distributions/timeseries.py` & `pymc-experimental-0.0.5/pymc_experimental/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/gp/__init__.py` & `pymc-experimental-0.0.5/pymc_experimental/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/gp/latent_approx.py` & `pymc-experimental-0.0.5/pymc_experimental/gp/latent_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/inference/__init__.py` & `pymc-experimental-0.0.5/pymc_experimental/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/inference/fit.py` & `pymc-experimental-0.0.5/pymc_experimental/inference/fit.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/inference/pathfinder.py` & `pymc-experimental-0.0.5/pymc_experimental/inference/pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/linearmodel.py` & `pymc-experimental-0.0.5/pymc_experimental/linearmodel.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/marginal_model.py` & `pymc-experimental-0.0.5/pymc_experimental/marginal_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -391,52 +391,46 @@
     raise NotImplementedError(f"Cannot compute domain for op {op}")
 
 
 @_logprob.register(FiniteDiscreteMarginalRV)
 def finite_discrete_marginal_rv_logp(op, values, *inputs, **kwargs):
     # Clone the inner RV graph of the Marginalized RV
     marginalized_rvs_node = op.make_node(*inputs)
-    marginalized_rv, *dependent_rvs = clone_replace(
+    inner_rvs = clone_replace(
         op.inner_outputs,
         replace={u: v for u, v in zip(op.inner_inputs, marginalized_rvs_node.inputs)},
     )
+    marginalized_rv = inner_rvs[0]
 
     # Obtain the joint_logp graph of the inner RV graph
-    # Some inputs are not root inputs (such as transformed projections of value variables)
-    # Or cannot be used as inputs to an OpFromGraph (shared variables and constants)
-    inputs = list(inputvars(inputs))
-    rvs_to_values = {}
-    dummy_marginalized_value = marginalized_rv.clone()
-    rvs_to_values[marginalized_rv] = dummy_marginalized_value
-    rvs_to_values.update(zip(dependent_rvs, values))
-    logps_dict = factorized_joint_logprob(rv_values=rvs_to_values, **kwargs)
+    inner_rvs_to_values = {rv: rv.clone() for rv in inner_rvs}
+    logps_dict = factorized_joint_logprob(rv_values=inner_rvs_to_values, **kwargs)
 
     # Reduce logp dimensions corresponding to broadcasted variables
-    values_axis_bcast = []
-    for value in values:
-        vbcast = value.type.broadcastable
-        mbcast = dummy_marginalized_value.type.broadcastable
+    joint_logp = logps_dict[inner_rvs_to_values[marginalized_rv]]
+    for inner_rv, inner_value in inner_rvs_to_values.items():
+        if inner_rv is marginalized_rv:
+            continue
+        vbcast = inner_value.type.broadcastable
+        mbcast = marginalized_rv.type.broadcastable
         mbcast = (True,) * (len(vbcast) - len(mbcast)) + mbcast
-        values_axis_bcast.append([i for i, (m, v) in enumerate(zip(mbcast, vbcast)) if m != v])
-    joint_logp = logps_dict[dummy_marginalized_value]
-    for value, values_axis_bcast in zip(values, values_axis_bcast):
-        joint_logp += logps_dict[value].sum(values_axis_bcast, keepdims=True)
+        values_axis_bcast = [i for i, (m, v) in enumerate(zip(mbcast, vbcast)) if m != v]
+        joint_logp += logps_dict[inner_value].sum(values_axis_bcast, keepdims=True)
 
     # Wrap the joint_logp graph in an OpFromGrah, so that we can evaluate it at different
     # values of the marginalized RV
-    # OpFromGraph does not accept constant inputs
-    non_const_values = [
-        value
-        for value in rvs_to_values.values()
-        if not isinstance(value, (Constant, SharedVariable))
-    ]
-    joint_logp_op = OpFromGraph([*non_const_values, *inputs], [joint_logp], inline=True)
+    # Some inputs are not root inputs (such as transformed projections of value variables)
+    # Or cannot be used as inputs to an OpFromGraph (shared variables and constants)
+    inputs = list(inputvars(inputs))
+    joint_logp_op = OpFromGraph(
+        list(inner_rvs_to_values.values()) + inputs, [joint_logp], inline=True
+    )
 
     # Compute the joint_logp for all possible n values of the marginalized RV. We assume
-    # each original dimension is independent so that it sufficies to evaluate the graph
+    # each original dimension is independent so that it suffices to evaluate the graph
     # n times, once with each possible value of the marginalized RV replicated across
     # batched dimensions of the marginalized RV
 
     # PyMC does not allow RVs in the logp graph, even if we are just using the shape
     marginalized_rv_shape = constant_fold(tuple(marginalized_rv.shape))
     marginalized_rv_domain = get_domain_of_finite_discrete_rv(marginalized_rv)
     marginalized_rv_domain_tensor = pt.swapaxes(
@@ -445,35 +439,31 @@
             marginalized_rv_domain,
             dtype=marginalized_rv.dtype,
         ),
         axis1=0,
         axis2=-1,
     )
 
-    # OpFromGraph does not accept constant inputs
-    non_const_values = [
-        value for value in values if not isinstance(value, (Constant, SharedVariable))
-    ]
     # Arbitrary cutoff to switch to Scan implementation to keep graph size under control
     if len(marginalized_rv_domain) <= 10:
         joint_logps = [
-            joint_logp_op(marginalized_rv_domain_tensor[i], *non_const_values, *inputs)
+            joint_logp_op(marginalized_rv_domain_tensor[i], *values, *inputs)
             for i in range(len(marginalized_rv_domain))
         ]
     else:
-        # Make sure this is rewrite is registered
+        # Make sure this rewrite is registered
         from pymc.pytensorf import local_remove_check_parameter
 
         def logp_fn(marginalized_rv_const, *non_sequences):
             return joint_logp_op(marginalized_rv_const, *non_sequences)
 
         joint_logps, _ = scan_map(
             fn=logp_fn,
             sequences=marginalized_rv_domain_tensor,
-            non_sequences=[*non_const_values, *inputs],
+            non_sequences=[*values, *inputs],
             mode=Mode().including("local_remove_check_parameter"),
         )
 
     joint_logps = pt.logsumexp(joint_logps, axis=0)
 
     # We have to add dummy logps for the remaining value variables, otherwise PyMC will raise
     return joint_logps, *(pt.constant(0),) * (len(values) - 1)
```

### Comparing `pymc-experimental-0.0.3/pymc_experimental/model_builder.py` & `pymc-experimental-0.0.5/pymc_experimental/model_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -464,25 +464,27 @@
         self.idata.add_groups(fit_data=combined_data.to_xarray())  # type: ignore
         return self.idata  # type: ignore
 
     def predict(
         self,
         X_pred: Union[np.ndarray, pd.DataFrame, pd.Series],
         extend_idata: bool = True,
+        **kwargs,
     ) -> np.ndarray:
         """
         Uses model to predict on unseen data and return point prediction of all the samples. The point prediction
         for each input row is the expected output value, computed as the mean of MCMC samples.
 
         Parameters
         ---------
         X_pred : array-like if sklearn is available, otherwise array, shape (n_pred, n_features)
             The input data used for prediction.
         extend_idata : Boolean determining whether the predictions should be added to inference data object.
             Defaults to True.
+        **kwargs: Additional arguments to pass to pymc.sample_posterior_predictive
 
         Returns
         -------
         y_pred : ndarray, shape (n_pred,)
             Predicted output corresponding to input X_pred.
 
         Examples
@@ -491,15 +493,15 @@
         >>> idata = model.fit(data)
         >>> x_pred = []
         >>> prediction_data = pd.DataFrame({'input':x_pred})
         >>> pred_mean = model.predict(prediction_data)
         """
 
         posterior_predictive_samples = self.sample_posterior_predictive(
-            X_pred, extend_idata, combined=False
+            X_pred, extend_idata, combined=False, **kwargs
         )
 
         if self.output_var not in posterior_predictive_samples:
             raise KeyError(
                 f"Output variable {self.output_var} not found in posterior predictive samples."
             )
 
@@ -510,14 +512,15 @@
 
     def sample_prior_predictive(
         self,
         X_pred,
         samples: Optional[int] = None,
         extend_idata: bool = False,
         combined: bool = True,
+        **kwargs,
     ):
         """
         Sample from the model's prior predictive distribution.
 
         Parameters
         ---------
         X_pred : array, shape (n_pred, n_features)
@@ -525,14 +528,15 @@
         samples : int
             Number of samples from the prior parameter distributions to generate.
             If not set, uses sampler_config['draws'] if that is available, otherwise defaults to 500.
         extend_idata : Boolean determining whether the predictions should be added to inference data object.
             Defaults to False.
         combined: Combine chain and draw dims into sample. Won't work if a dim named sample already exists.
             Defaults to True.
+        **kwargs: Additional arguments to pass to pymc.sample_prior_predictive
 
         Returns
         -------
         prior_predictive_samples : DataArray, shape (n_pred, samples)
             Prior predictive samples for each input X_pred
         """
         if samples is None:
@@ -540,48 +544,49 @@
 
         if self.model is None:
             self.build_model()
 
         self._data_setter(X_pred)
         if self.model is not None:
             with self.model:  # sample with new input data
-                prior_pred: az.InferenceData = pm.sample_prior_predictive(samples)
+                prior_pred: az.InferenceData = pm.sample_prior_predictive(samples, **kwargs)
                 self.set_idata_attrs(prior_pred)
                 if extend_idata:
                     if self.idata is not None:
                         self.idata.extend(prior_pred)
                     else:
                         self.idata = prior_pred
 
         prior_predictive_samples = az.extract(prior_pred, "prior_predictive", combined=combined)
 
         return prior_predictive_samples
 
-    def sample_posterior_predictive(self, X_pred, extend_idata, combined):
+    def sample_posterior_predictive(self, X_pred, extend_idata, combined, **kwargs):
         """
         Sample from the model's posterior predictive distribution.
 
         Parameters
         ---------
         X_pred : array, shape (n_pred, n_features)
             The input data used for prediction using prior distribution..
         extend_idata : Boolean determining whether the predictions should be added to inference data object.
             Defaults to False.
         combined: Combine chain and draw dims into sample. Won't work if a dim named sample already exists.
             Defaults to True.
+        **kwargs: Additional arguments to pass to pymc.sample_posterior_predictive
 
         Returns
         -------
         posterior_predictive_samples : DataArray, shape (n_pred, samples)
             Posterior predictive samples for each input X_pred
         """
         self._data_setter(X_pred)
 
         with self.model:  # sample with new input data
-            post_pred = pm.sample_posterior_predictive(self.idata)
+            post_pred = pm.sample_posterior_predictive(self.idata, **kwargs)
             if extend_idata:
                 self.idata.extend(post_pred)
 
         posterior_predictive_samples = az.extract(
             post_pred, "posterior_predictive", combined=combined
         )
 
@@ -617,45 +622,48 @@
         """
 
     def predict_proba(
         self,
         X_pred: Union[np.ndarray, pd.DataFrame, pd.Series],
         extend_idata: bool = True,
         combined: bool = False,
+        **kwargs,
     ) -> xr.DataArray:
         """Alias for `predict_posterior`, for consistency with scikit-learn probabilistic estimators."""
-        return self.predict_posterior(X_pred, extend_idata, combined)
+        return self.predict_posterior(X_pred, extend_idata, combined, **kwargs)
 
     def predict_posterior(
         self,
         X_pred: Union[np.ndarray, pd.DataFrame, pd.Series],
         extend_idata: bool = True,
         combined: bool = True,
+        **kwargs,
     ) -> xr.DataArray:
         """
         Generate posterior predictive samples on unseen data.
 
         Parameters
         ---------
         X_pred : array-like if sklearn is available, otherwise array, shape (n_pred, n_features)
             The input data used for prediction.
         extend_idata : Boolean determining whether the predictions should be added to inference data object.
             Defaults to True.
         combined: Combine chain and draw dims into sample. Won't work if a dim named sample already exists.
             Defaults to True.
+        **kwargs: Additional arguments to pass to pymc.sample_posterior_predictive
 
         Returns
         -------
         y_pred : DataArray, shape (n_pred, chains * draws) if combined is True, otherwise (chains, draws, n_pred)
             Posterior predictive samples for each input X_pred
         """
 
         X_pred = self._validate_data(X_pred)
         posterior_predictive_samples = self.sample_posterior_predictive(
-            X_pred, extend_idata, combined
+            X_pred, extend_idata, combined, **kwargs
         )
 
         if self.output_var not in posterior_predictive_samples:
             raise KeyError(
                 f"Output variable {self.output_var} not found in posterior predictive samples."
             )
```

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/__init__.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/distributions/__init__.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_continuous.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_discrete.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_discrete_markov_chain.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_discrete_markov_chain.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_multivariate.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/test_histogram_approximation.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/test_histogram_approximation.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/test_linearmodel.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/test_linearmodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,19 +78,18 @@
     model = fitted_linear_model_instance
     temp = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False)
     model.save(temp.name)
     model2 = LinearModel.load(temp.name)
     assert model.idata.groups() == model2.idata.groups()
 
     x_pred = np.random.uniform(low=0, high=1, size=(100, 1))
-    pred1 = model.predict(x_pred)
-    pred2 = model2.predict(x_pred)
-    # Predictions should have similar statistical characteristics
-    assert pred1.mean() == pytest.approx(pred2.mean(), 1e-3)
-    assert pred1.var() == pytest.approx(pred2.var(), 1e-2)
+    pred1 = model.predict(x_pred, random_seed=423)
+    pred2 = model2.predict(x_pred, random_seed=423)
+    # Predictions should be identical
+    np.testing.assert_array_equal(pred1, pred2)
     temp.close()
 
 
 def test_predict(fitted_linear_model_instance):
     model = fitted_linear_model_instance
     x_pred = np.random.uniform(low=0, high=1, size=(100, 1))
     pred = model.predict(x_pred)
```

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/test_marginal_model.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/test_marginal_model.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/test_model_builder.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/test_model_builder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/test_pathfinder.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/test_pivoted_cholesky.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/test_prior_from_trace.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/test_prior_from_trace.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/test_splines.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/tests/utils/test_model_fgraph.py` & `pymc-experimental-0.0.5/pymc_experimental/tests/utils/test_model_fgraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,36 +72,49 @@
     ip = m_new.initial_point()
     np.testing.assert_equal(
         m_new.compile_logp()(ip),
         m_old.compile_logp()(ip),
     )
 
 
-def test_data():
+@pytest.mark.parametrize("inline_views", (False, True))
+def test_data(inline_views):
     """Test shared RNGs, MutableData, ConstantData and Dim lengths are handled correctly.
 
     Everything should be preserved across new and old models, except for shared RNGs
     """
     with pm.Model(coords_mutable={"test_dim": range(3)}) as m_old:
         x = pm.MutableData("x", [0.0, 1.0, 2.0], dims=("test_dim",))
         y = pm.MutableData("y", [10.0, 11.0, 12.0], dims=("test_dim",))
-        b0 = pm.ConstantData("b0", 0.0)
+        b0 = pm.ConstantData("b0", np.zeros(3))
         b1 = pm.Normal("b1")
         mu = pm.Deterministic("mu", b0 + b1 * x, dims=("test_dim",))
         obs = pm.Normal("obs", mu, sigma=1e-5, observed=y, dims=("test_dim",))
 
-    m_fgraph, memo = fgraph_from_model(m_old)
+    m_fgraph, memo = fgraph_from_model(m_old, inlined_views=inline_views)
     assert isinstance(memo[x].owner.op, ModelNamed)
     assert isinstance(memo[y].owner.op, ModelNamed)
     assert isinstance(memo[b0].owner.op, ModelNamed)
+    mu_inp = memo[mu].owner.inputs[0]
+    obs = memo[obs]
+    if not inline_views:
+        # Add(b0, Mul(FreeRV(b1), x) not Add(Named(b0), Mul(FreeRV(b1), Named(x))
+        assert mu_inp.owner.inputs[0] is memo[b0].owner.inputs[0]
+        assert mu_inp.owner.inputs[1].owner.inputs[1] is memo[x].owner.inputs[0]
+        # ObservedRV(obs, y, *dims) not ObservedRV(obs, Named(y), *dims)
+        assert obs.owner.inputs[1] is memo[y].owner.inputs[0]
+    else:
+        assert mu_inp.owner.inputs[0] is memo[b0]
+        assert mu_inp.owner.inputs[1].owner.inputs[1] is memo[x]
+        assert obs.owner.inputs[1] is memo[y]
 
     m_new = model_from_fgraph(m_fgraph)
 
     # ConstantData is preserved
-    assert m_new["b0"].data == m_old["b0"].data
+    assert np.all(m_new["b0"].data == m_old["b0"].data)
 
     # Shared non-rng shared variables are preserved
     assert m_new["x"].container is x.container
     assert m_new["y"].container is y.container
     assert m_new.rvs_to_values[m_new["obs"]] is m_new["y"]
 
     # Shared rng shared variables are not preserved
@@ -110,15 +123,16 @@
     with m_old:
         pm.set_data({"x": [100.0, 200.0]}, coords={"test_dim": range(2)})
 
     assert m_new.dim_lengths["test_dim"].eval() == 2
     np.testing.assert_array_almost_equal(pm.draw(m_new["x"]), [100.0, 200.0])
 
 
-def test_deterministics():
+@pytest.mark.parametrize("inline_views", (False, True))
+def test_deterministics(inline_views):
     """Test handling of deterministics.
 
     We don't want Deterministics in the middle of the FunctionGraph, as they would make rewrites cumbersome
     However we want them in the middle of Model.basic_RVs, so they display nicely in graphviz
 
     There is one edge case that has to be considered, when a Deterministic is just a copy of a RV.
     In that case we don't bother to reintroduce it in between other Model.basic_RVs
@@ -136,30 +150,35 @@
         y__ = pm.Deterministic("y__", y_)
         z = pm.Normal("z", y__)
 
     # Deterministic mu is in the graph of x to y but not sigma
     assert m["y"].owner.inputs[3] is m["mu"]
     assert m["y"].owner.inputs[4] is not m["sigma"]
 
-    fg, _ = fgraph_from_model(m)
+    fg, _ = fgraph_from_model(m, inlined_views=inline_views)
 
     # Check that no Deterministics are in graph of x to y and y to z
     x, y, z, det_mu, det_sigma, det_y_, det_y__ = fg.outputs
     # [Det(mu), Det(sigma)]
     mu = det_mu.owner.inputs[0]
     sigma = det_sigma.owner.inputs[0]
-    # [FreeRV(y(mu, sigma))] not [FreeRV(y(Det(mu), Det(sigma)))]
-    assert y.owner.inputs[0].owner.inputs[3] is mu
     assert y.owner.inputs[0].owner.inputs[4] is sigma
-    # [FreeRV(z(y))] not [FreeRV(z(Det(Det(y))))]
-    assert z.owner.inputs[0].owner.inputs[3] is y
-    # [Det(y), Det(y)], not [Det(y), Det(Det(y))]
-    assert det_y_.owner.inputs[0] is y
-    assert det_y__.owner.inputs[0] is y
     assert det_y_ is not det_y__
+    assert det_y_.owner.inputs[0] is y
+    if not inline_views:
+        # FreeRV(y(mu, sigma)) not FreeRV(y(Det(mu), Det(sigma)))
+        assert y.owner.inputs[0].owner.inputs[3] is mu
+        # FreeRV(z(y)) not FreeRV(z(Det(Det(y))))
+        assert z.owner.inputs[0].owner.inputs[3] is y
+        # Det(y), not Det(Det(y))
+        assert det_y__.owner.inputs[0] is y
+    else:
+        assert y.owner.inputs[0].owner.inputs[3] is det_mu
+        assert z.owner.inputs[0].owner.inputs[3] is det_y__
+        assert det_y__.owner.inputs[0] is det_y_
 
     # Both mu and sigma deterministics are now in the graph of x to y
     m = model_from_fgraph(fg)
     assert m["y"].owner.inputs[3] is m["mu"]
     assert m["y"].owner.inputs[4] is m["sigma"]
     # But not y_* in y to z, since there was no real Op in between
     assert m["z"].owner.inputs[3] is m["y"]
```

### Comparing `pymc-experimental-0.0.3/pymc_experimental/utils/__init__.py` & `pymc-experimental-0.0.5/pymc_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/utils/linear_cg.py` & `pymc-experimental-0.0.5/pymc_experimental/utils/linear_cg.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/utils/model_fgraph.py` & `pymc-experimental-0.0.5/pymc_experimental/utils/model_fgraph.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,38 +86,49 @@
 model_observed_rv = ModelObservedRV()
 model_potential = ModelPotential()
 model_deterministic = ModelDeterministic()
 model_named = ModelNamed()
 
 
 def toposort_replace(
-    fgraph: FunctionGraph, replacements: Sequence[Tuple[Variable, Variable]]
+    fgraph: FunctionGraph, replacements: Sequence[Tuple[Variable, Variable]], reverse: bool = False
 ) -> None:
     """Replace multiple variables in topological order."""
     toposort = fgraph.toposort()
     sorted_replacements = sorted(
-        replacements, key=lambda pair: toposort.index(pair[0].owner) if pair[0].owner else -1
+        replacements,
+        key=lambda pair: toposort.index(pair[0].owner) if pair[0].owner else -1,
+        reverse=reverse,
     )
-    fgraph.replace_all(tuple(sorted_replacements), import_missing=True)
+    fgraph.replace_all(sorted_replacements, import_missing=True)
 
 
 @node_rewriter([Elemwise])
 def local_remove_identity(fgraph, node):
     if isinstance(node.op.scalar_op, Identity):
         return [node.inputs[0]]
 
 
 remove_identity_rewrite = out2in(local_remove_identity)
 
 
-def fgraph_from_model(model: Model) -> Tuple[FunctionGraph, Dict[Variable, Variable]]:
+def fgraph_from_model(
+    model: Model, inlined_views=False
+) -> Tuple[FunctionGraph, Dict[Variable, Variable]]:
     """Convert Model to FunctionGraph.
 
     See: model_from_fgraph
 
+    Parameters
+    ----------
+    model: PyMC model
+    inlined_views: bool, default False
+        Whether "view" variables (Deterministics and Data) should be inlined among RVs in the fgraph,
+        or show up as separate branches.
+
     Returns
     -------
     fgraph: FunctionGraph
         FunctionGraph that includes a copy of model variables, wrapped in dummy `ModelVar` Ops.
         It should be possible to reconstruct a valid PyMC model using `model_from_fgraph`.
 
     memo: Dict
@@ -134,27 +145,44 @@
 
     # Collect PyTensor variables
     rvs_to_values = model.rvs_to_values
     rvs = list(rvs_to_values.keys())
     free_rvs = model.free_RVs
     observed_rvs = model.observed_RVs
     potentials = model.potentials
+    named_vars = model.named_vars.values()
     # We copy Deterministics (Identity Op) so that they don't show in between "main" variables
     # We later remove these Identity Ops when we have a Deterministic ModelVar Op as a separator
     old_deterministics = model.deterministics
-    deterministics = [det.copy(det.name) for det in old_deterministics]
-    # Other variables that are in model.named_vars but are not any of the categories above
+    deterministics = [det if inlined_views else det.copy(det.name) for det in old_deterministics]
+    # Value variables (we also have to decide whether to inline named ones)
+    old_value_vars = list(rvs_to_values.values())
+    unnamed_value_vars = [val for val in old_value_vars if val not in named_vars]
+    named_value_vars = [
+        val if inlined_views else val.copy(val.name) for val in old_value_vars if val in named_vars
+    ]
+    value_vars = old_value_vars.copy()
+    if inlined_views:
+        # In this case we want to use the named_value_vars as the value_vars in RVs
+        for named_val in named_value_vars:
+            idx = value_vars.index(named_val)
+            value_vars[idx] = named_val
+    # Other variables that are in named_vars but are not any of the categories above
     # E.g., MutableData, ConstantData, _dim_lengths
     # We use the same trick as deterministics!
-    accounted_for = free_rvs + observed_rvs + potentials + old_deterministics
-    old_other_named_vars = [var for var in model.named_vars.values() if var not in accounted_for]
-    other_named_vars = [var.copy(var.name) for var in old_other_named_vars]
-    value_vars = [val for val in rvs_to_values.values() if val not in old_other_named_vars]
+    accounted_for = set(free_rvs + observed_rvs + potentials + old_deterministics + old_value_vars)
+    other_named_vars = [
+        var if inlined_views else var.copy(var.name)
+        for var in named_vars
+        if var not in accounted_for
+    ]
 
-    model_vars = rvs + potentials + deterministics + other_named_vars + value_vars
+    model_vars = (
+        rvs + potentials + deterministics + other_named_vars + named_value_vars + unnamed_value_vars
+    )
 
     memo = {}
 
     # Replace RNG nodes so that seeding does not interfere with old model
     for rng in find_rng_nodes(model_vars):
         new_rng = rng.clone()
         new_rng.set_value(rng.get_value(borrow=False))
@@ -172,21 +200,21 @@
     fgraph._dim_lengths = model._dim_lengths.copy()
 
     rvs_to_transforms = model.rvs_to_transforms
     named_vars_to_dims = model.named_vars_to_dims
 
     # Introduce dummy `ModelVar` Ops
     free_rvs_to_transforms = {memo[k]: tr for k, tr in rvs_to_transforms.items()}
-    free_rvs_to_values = {memo[k]: memo[v] for k, v in rvs_to_values.items() if k in free_rvs}
+    free_rvs_to_values = {memo[k]: memo[v] for k, v in zip(rvs, value_vars) if k in free_rvs}
     observed_rvs_to_values = {
-        memo[k]: memo[v] for k, v in rvs_to_values.items() if k in observed_rvs
+        memo[k]: memo[v] for k, v in zip(rvs, value_vars) if k in observed_rvs
     }
     potentials = [memo[k] for k in potentials]
     deterministics = [memo[k] for k in deterministics]
-    other_named_vars = [memo[k] for k in other_named_vars]
+    named_vars = [memo[k] for k in other_named_vars + named_value_vars]
 
     vars = fgraph.outputs
     new_vars = []
     for var in vars:
         dims = named_vars_to_dims.get(var.name, ())
         if var in free_rvs_to_values:
             new_var = model_free_rv(
@@ -194,77 +222,83 @@
             )
         elif var in observed_rvs_to_values:
             new_var = model_observed_rv(var, observed_rvs_to_values[var], *dims)
         elif var in potentials:
             new_var = model_potential(var, *dims)
         elif var in deterministics:
             new_var = model_deterministic(var, *dims)
-        elif var in other_named_vars:
+        elif var in named_vars:
             new_var = model_named(var, *dims)
         else:
-            # Value variables
+            # Unnamed value variables
             new_var = var
         new_vars.append(new_var)
 
     replacements = tuple(zip(vars, new_vars))
-    toposort_replace(fgraph, replacements)
+    toposort_replace(fgraph, replacements, reverse=True)
 
     # Reference model vars in memo
     inverse_memo = {v: k for k, v in memo.items()}
     for var, model_var in replacements:
-        if isinstance(
-            model_var.owner is not None and model_var.owner.op, (ModelDeterministic, ModelNamed)
+        if not inlined_views and (
+            model_var.owner and isinstance(model_var.owner.op, (ModelDeterministic, ModelNamed))
         ):
             # Ignore extra identity that will be removed at the end
             var = var.owner.inputs[0]
         original_var = inverse_memo[var]
         memo[original_var] = model_var
 
-    # Remove value variable as outputs, now that they are graph inputs
-    first_value_idx = len(fgraph.outputs) - len(value_vars)
-    for _ in value_vars:
-        fgraph.remove_output(first_value_idx)
+    # Remove the last outputs corresponding to unnamed value variables, now that they are graph inputs
+    first_idx_to_remove = len(fgraph.outputs) - len(unnamed_value_vars)
+    for _ in unnamed_value_vars:
+        fgraph.remove_output(first_idx_to_remove)
 
     # Now that we have Deterministic dummy Ops, we remove the noisy `Identity`s from the graph
     remove_identity_rewrite.apply(fgraph)
 
     return fgraph, memo
 
 
 def model_from_fgraph(fgraph: FunctionGraph) -> Model:
     """Convert FunctionGraph to PyMC model.
 
     This requires nodes to be properly tagged with `ModelVar` dummy Ops.
 
     See: fgraph_from_model
     """
+
+    def first_non_model_var(var):
+        if var.owner and isinstance(var.owner.op, ModelVar):
+            new_var = var.owner.inputs[0]
+            return first_non_model_var(new_var)
+        else:
+            return var
+
     model = Model()
     if model.parent is not None:
         raise RuntimeError("model_to_fgraph cannot be called inside a PyMC model context")
     model._coords = getattr(fgraph, "_coords", {})
     model._dim_lengths = getattr(fgraph, "_dim_lengths", {})
 
     # Replace dummy `ModelVar` Ops by the underlying variables,
-    # Except for Deterministics which could reintroduce the old graphs
     fgraph = fgraph.clone()
     model_dummy_vars = [
         model_node.outputs[0]
         for model_node in fgraph.toposort()
         if isinstance(model_node.op, ModelVar)
     ]
     model_dummy_vars_to_vars = {
-        dummy_var: dummy_var.owner.inputs[0]
+        # Deterministics could refer to other model variables directly,
+        # We make sure to replace them by the first non-model variable
+        dummy_var: first_non_model_var(dummy_var.owner.inputs[0])
         for dummy_var in model_dummy_vars
-        # Don't include Deterministics!
-        if not isinstance(dummy_var.owner.op, ModelDeterministic)
     }
     toposort_replace(fgraph, tuple(model_dummy_vars_to_vars.items()))
 
     # Populate new PyMC model mappings
-    non_det_model_vars = set(model_dummy_vars_to_vars.values())
     for model_var in model_dummy_vars:
         if isinstance(model_var.owner.op, ModelFreeRV):
             var, value, *dims = model_var.owner.inputs
             transform = model_var.owner.op.transform
             model.free_RVs.append(var)
             # PyMC does not allow setting transform when we pass a value_var. Why?
             model.create_value_var(var, transform=None, value_var=value)
@@ -275,44 +309,42 @@
             model.observed_RVs.append(var)
             model.create_value_var(var, transform=None, value_var=value)
         elif isinstance(model_var.owner.op, ModelPotential):
             var, *dims = model_var.owner.inputs
             model.potentials.append(var)
         elif isinstance(model_var.owner.op, ModelDeterministic):
             var, *dims = model_var.owner.inputs
-            # Register the original var (not the copy) as the Deterministic
-            # So it shows in the expected place in graphviz.
-            # unless it's another model var, in which case we need a copy!
-            if var in non_det_model_vars:
+            # If a Deterministic is a direct view on an RV, copy it
+            if var in model.basic_RVs:
                 var = var.copy()
             model.deterministics.append(var)
         elif isinstance(model_var.owner.op, ModelNamed):
             var, *dims = model_var.owner.inputs
         else:
             raise TypeError(f"Unexpected ModelVar type {type(model_var)}")
 
         var.name = model_var.name
         dims = [dim.data for dim in dims] if dims else None
         model.add_named_variable(var, dims=dims)
 
     return model
 
 
-def clone_model(model: Model) -> Tuple[Model]:
+def clone_model(model: Model) -> Model:
     """Clone a PyMC model.
 
     Recreates a PyMC model with clones of the original variables.
     Shared variables will point to the same container but be otherwise different objects.
     Constants are not cloned.
 
 
     Examples
     --------
 
-        .. code-block:: python
+    .. code-block:: python
 
         import pymc as pm
         from pymc_experimental.utils import clone_model
 
         with pm.Model() as m:
             p = pm.Beta("p", 1, 1)
             x = pm.Bernoulli("x", p=p, shape=(3,))
@@ -322,7 +354,18 @@
             clone_x = clone_m["x"]
 
             # z will be part of clone_m but not m
             z = pm.Deterministic("z", clone_x + 1)
 
     """
     return model_from_fgraph(fgraph_from_model(model)[0])
+
+
+def extract_dims(var) -> Tuple:
+    dims = ()
+    node = var.owner
+    if node and isinstance(node.op, ModelVar):
+        if isinstance(node.op, ModelValuedVar):
+            dims = node.inputs[2:]
+        else:
+            dims = node.inputs[1:]
+    return dims
```

### Comparing `pymc-experimental-0.0.3/pymc_experimental/utils/pivoted_cholesky.py` & `pymc-experimental-0.0.5/pymc_experimental/utils/pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/utils/prior.py` & `pymc-experimental-0.0.5/pymc_experimental/utils/prior.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental/utils/spline.py` & `pymc-experimental-0.0.5/pymc_experimental/utils/spline.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.3/pymc_experimental.egg-info/PKG-INFO` & `pymc-experimental-0.0.5/pymc_experimental.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.3
+Version: 0.0.5
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,56 +1,57 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.3 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.5 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Operating System :: OS Independent Requires-Python: >=3.8
-Description-Content-Type: text/markdown Provides-Extra: dask_histogram
-Provides-Extra: histogram Provides-Extra: complete Provides-Extra: dev License-
-File: LICENSE # Welcome to `pymc-experimental` [Contribute_with_Gitpod]
-[Codecov Badge] As PyMC continues to mature and expand its functionality to
-accommodate more domains of application, we increasingly see cutting-edge
-methodologies, highly specialized statistical distributions, and complex models
-appear. While this adds to the functionality and relevance of the project, it
-can also introduce instability and impose a burden on testing and quality
-control. To reduce the burden on the main `pymc` repository, this `pymc-
-experimental` repository can become the aggregator and testing ground for new
-additions to PyMC. This may include unusual probability distributions, advanced
-model fitting algorithms, innovative yet not fully tested methods or any code
-that may be inappropriate to include in the `pymc` repository, but may want to
-be made available to users. The `pymc-experimental` repository can be
-understood as the first step in the PyMC development pipeline, where all novel
-code is introduced until it is obvious that it belongs in the main repository.
-We hope that this organization improves the stability and streamlines the
-testing overhead of the `pymc` repository, while allowing users and developers
-to test and evaluate cutting-edge methods and not yet fully mature features.
-`pymc-experimental` would be designed to mirror the namespaces in `pymc` to
-make usage and migration as easy as possible. For example, a `ParabolicFractal`
-distribution could be used analogously to those in `pymc`: ```python import
-pymc as pm import pymc_experimental as pmx with pm.Model(): alpha =
-pmx.ParabolicFractal('alpha', b=1, c=1) ... ``` ## Questions ### What belongs
-in `pymc-experimental`? - newly-implemented statistical methods, for example
-step methods or model construction helpers - distributions that are tricky to
-sample from or test - infrequently-used fitting methods or distributions - any
-code that requires additional optimization before it can be used in practice
-### What does not belong in `pymc-experimental`? - Case studies -
-Implementations that cannot be applied generically, for example because they
-are tied to variables from a toy example ### Should there be more than one add-
-on repository? Since there is a lot of code that we may not want in the main
-repository, does it make sense to have more than one additional repository? For
-example, `pymc-experimental` may just include methods that are not fully
-developed, tested and trusted, while code that is known to work well and has
-adequate test coverage, but is still too specialized to become part of `pymc`
-could reside in a `pymc-extras` (or similar) repository. ### Unanswered
-questions & ToDos This project is still young and many things have not been
-answered or implemented. Please get involved! * What are guidelines for
-organizing submodules? * Proposal: No default imports of WIP/unstable
-submodules. By importing manually we can avoid breaking the package if a
-submodule breaks, for example because of an updated dependency.
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Operating System :: OS
+Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dask_histogram Provides-Extra: histogram Provides-Extra:
+complete Provides-Extra: dev License-File: LICENSE # Welcome to `pymc-
+experimental` [Contribute_with_Gitpod] [Codecov Badge] As PyMC continues to
+mature and expand its functionality to accommodate more domains of application,
+we increasingly see cutting-edge methodologies, highly specialized statistical
+distributions, and complex models appear. While this adds to the functionality
+and relevance of the project, it can also introduce instability and impose a
+burden on testing and quality control. To reduce the burden on the main `pymc`
+repository, this `pymc-experimental` repository can become the aggregator and
+testing ground for new additions to PyMC. This may include unusual probability
+distributions, advanced model fitting algorithms, innovative yet not fully
+tested methods or any code that may be inappropriate to include in the `pymc`
+repository, but may want to be made available to users. The `pymc-experimental`
+repository can be understood as the first step in the PyMC development
+pipeline, where all novel code is introduced until it is obvious that it
+belongs in the main repository. We hope that this organization improves the
+stability and streamlines the testing overhead of the `pymc` repository, while
+allowing users and developers to test and evaluate cutting-edge methods and not
+yet fully mature features. `pymc-experimental` would be designed to mirror the
+namespaces in `pymc` to make usage and migration as easy as possible. For
+example, a `ParabolicFractal` distribution could be used analogously to those
+in `pymc`: ```python import pymc as pm import pymc_experimental as pmx with
+pm.Model(): alpha = pmx.ParabolicFractal('alpha', b=1, c=1) ... ``` ##
+Questions ### What belongs in `pymc-experimental`? - newly-implemented
+statistical methods, for example step methods or model construction helpers -
+distributions that are tricky to sample from or test - infrequently-used
+fitting methods or distributions - any code that requires additional
+optimization before it can be used in practice ### What does not belong in
+`pymc-experimental`? - Case studies - Implementations that cannot be applied
+generically, for example because they are tied to variables from a toy example
+### Should there be more than one add-on repository? Since there is a lot of
+code that we may not want in the main repository, does it make sense to have
+more than one additional repository? For example, `pymc-experimental` may just
+include methods that are not fully developed, tested and trusted, while code
+that is known to work well and has adequate test coverage, but is still too
+specialized to become part of `pymc` could reside in a `pymc-extras` (or
+similar) repository. ### Unanswered questions & ToDos This project is still
+young and many things have not been answered or implemented. Please get
+involved! * What are guidelines for organizing submodules? * Proposal: No
+default imports of WIP/unstable submodules. By importing manually we can avoid
+breaking the package if a submodule breaks, for example because of an updated
+dependency.
```

### Comparing `pymc-experimental-0.0.3/pymc_experimental.egg-info/SOURCES.txt` & `pymc-experimental-0.0.5/pymc_experimental.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -28,28 +28,34 @@
 pymc_experimental/distributions/multivariate/__init__.py
 pymc_experimental/distributions/multivariate/r2d2m2cp.py
 pymc_experimental/gp/__init__.py
 pymc_experimental/gp/latent_approx.py
 pymc_experimental/inference/__init__.py
 pymc_experimental/inference/fit.py
 pymc_experimental/inference/pathfinder.py
+pymc_experimental/model_transform/__init__.py
+pymc_experimental/model_transform/basic.py
+pymc_experimental/model_transform/conditioning.py
 pymc_experimental/tests/__init__.py
 pymc_experimental/tests/test_histogram_approximation.py
 pymc_experimental/tests/test_linearmodel.py
 pymc_experimental/tests/test_marginal_model.py
 pymc_experimental/tests/test_model_builder.py
 pymc_experimental/tests/test_pathfinder.py
 pymc_experimental/tests/test_pivoted_cholesky.py
 pymc_experimental/tests/test_prior_from_trace.py
 pymc_experimental/tests/test_splines.py
 pymc_experimental/tests/distributions/__init__.py
 pymc_experimental/tests/distributions/test_continuous.py
 pymc_experimental/tests/distributions/test_discrete.py
 pymc_experimental/tests/distributions/test_discrete_markov_chain.py
 pymc_experimental/tests/distributions/test_multivariate.py
+pymc_experimental/tests/model_transform/__init__.py
+pymc_experimental/tests/model_transform/test_basic.py
+pymc_experimental/tests/model_transform/test_conditioning.py
 pymc_experimental/tests/utils/__init__.py
 pymc_experimental/tests/utils/test_model_fgraph.py
 pymc_experimental/utils/__init__.py
 pymc_experimental/utils/linear_cg.py
 pymc_experimental/utils/model_fgraph.py
 pymc_experimental/utils/pivoted_cholesky.py
 pymc_experimental/utils/prior.py
```

### Comparing `pymc-experimental-0.0.3/setup.py` & `pymc-experimental-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Operating System :: OS Independent",
 ]
```

