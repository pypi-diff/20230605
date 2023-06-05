# Comparing `tmp/aepsych-0.3.0.tar.gz` & `tmp/aepsych-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepsych-0.3.0.tar", last modified: Wed Dec  7 17:55:04 2022, max compression
+gzip compressed data, was "aepsych-0.4.0.tar", last modified: Mon Jun  5 20:25:35 2023, max compression
```

## Comparing `aepsych-0.3.0.tar` & `aepsych-0.4.0.tar`

### file list

```diff
@@ -1,120 +1,170 @@
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:04.583767 aepsych-0.3.0/
--rw-r--r--   0 craigsanders   (501) staff       (20)    19407 2022-12-07 17:18:11.000000 aepsych-0.3.0/LICENSE
--rw-r--r--   0 craigsanders   (501) staff       (20)     4565 2022-12-07 17:55:04.580793 aepsych-0.3.0/PKG-INFO
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.343762 aepsych-0.3.0/aepsych/
--rw-r--r--   0 craigsanders   (501) staff       (20)      983 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/__init__.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.594834 aepsych-0.3.0/aepsych/acquisition/
--rw-r--r--   0 craigsanders   (501) staff       (20)     1365 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/acquisition/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3043 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/acquisition/bvn.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    12367 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/acquisition/lookahead.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     7137 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/acquisition/lookahead_utils.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3176 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/acquisition/lse.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3444 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/acquisition/mc_posterior_variance.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6079 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/acquisition/monotonic_rejection.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4989 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/acquisition/mutual_information.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4157 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/acquisition/objective.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2433 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/acquisition/rejection_sampler.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.654658 aepsych-0.3.0/aepsych/benchmark/
--rw-r--r--   0 craigsanders   (501) staff       (20)      868 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/benchmark/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    11291 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/benchmark/benchmark.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    10521 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/benchmark/pathos_benchmark.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    10010 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/benchmark/problem.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6920 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/benchmark/test_functions.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    12524 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/config.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.694135 aepsych-0.3.0/aepsych/database/
--rw-r--r--   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/database/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    11554 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/database/db.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    17629 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/database/tables.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.727884 aepsych-0.3.0/aepsych/factory/
--rw-r--r--   0 craigsanders   (501) staff       (20)      608 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/factory/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    10120 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/factory/factory.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.854507 aepsych-0.3.0/aepsych/generators/
--rw-r--r--   0 craigsanders   (501) staff       (20)     1139 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/generators/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3075 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/generators/base.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1352 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/generators/epsilon_greedy_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2871 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/generators/manual_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     7978 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/generators/monotonic_rejection_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4432 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/generators/monotonic_thompson_sampler_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6943 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/generators/optimize_acqf_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      732 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/generators/pairwise_optimize_acqf_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      689 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/generators/pairwise_sobol_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2176 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/generators/random_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2934 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/generators/sobol_generator.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.885349 aepsych-0.3.0/aepsych/kernels/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/kernels/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1801 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/kernels/rbf_partial_grad.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.925343 aepsych-0.3.0/aepsych/likelihoods/
--rw-r--r--   0 craigsanders   (501) staff       (20)      473 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/likelihoods/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1053 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/likelihoods/bernoulli.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2246 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/likelihoods/ordinal.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.941084 aepsych-0.3.0/aepsych/means/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/means/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1109 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/means/constant_partial_grad.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:04.055232 aepsych-0.3.0/aepsych/models/
--rw-r--r--   0 craigsanders   (501) staff       (20)      783 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/models/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    14677 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/models/base.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4684 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/models/derivative_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    12041 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/models/gp_classification.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6886 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/models/gp_regression.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    10235 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/models/monotonic_projection_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    13471 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/models/monotonic_rejection_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2246 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/models/ordinal_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6827 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/models/pairwise_probit.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3201 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/models/utils.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    16703 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/plotting.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:04.094497 aepsych-0.3.0/aepsych/server/
--rw-r--r--   0 craigsanders   (501) staff       (20)      282 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/server/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    40054 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/server/server.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     5823 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/server/sockets.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    18541 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/strategy.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     5042 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/utils.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1235 2022-12-07 17:18:11.000000 aepsych-0.3.0/aepsych/utils_logging.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      241 2022-12-07 17:48:47.000000 aepsych-0.3.0/aepsych/version.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:03.428337 aepsych-0.3.0/aepsych.egg-info/
--rw-r--r--   0 craigsanders   (501) staff       (20)     4565 2022-12-07 17:55:02.000000 aepsych-0.3.0/aepsych.egg-info/PKG-INFO
--rw-r--r--   0 craigsanders   (501) staff       (20)     3200 2022-12-07 17:55:03.000000 aepsych-0.3.0/aepsych.egg-info/SOURCES.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)        1 2022-12-07 17:55:02.000000 aepsych-0.3.0/aepsych.egg-info/dependency_links.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)       62 2022-12-07 17:55:02.000000 aepsych-0.3.0/aepsych.egg-info/entry_points.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)      169 2022-12-07 17:55:03.000000 aepsych-0.3.0/aepsych.egg-info/requires.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)       14 2022-12-07 17:55:03.000000 aepsych-0.3.0/aepsych.egg-info/top_level.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)      178 2022-12-07 17:18:11.000000 aepsych-0.3.0/pyproject.toml
--rw-r--r--   0 craigsanders   (501) staff       (20)       38 2022-12-07 17:55:04.586324 aepsych-0.3.0/setup.cfg
--rw-r--r--   0 craigsanders   (501) staff       (20)     1526 2022-12-07 17:48:47.000000 aepsych-0.3.0/setup.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:04.282625 aepsych-0.3.0/tests/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/__init__.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:04.381964 aepsych-0.3.0/tests/acquisition/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/acquisition/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1019 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/acquisition/test_lse.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4924 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/acquisition/test_mi.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1822 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/acquisition/test_monotonic.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1322 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/acquisition/test_objective.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1353 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/acquisition/test_rejection_sampler.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6480 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/common.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:04.475917 aepsych-0.3.0/tests/generators/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/generators/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1868 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/generators/test_epsilon_greedy_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1933 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/generators/test_manual_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2720 2022-12-07 17:48:47.000000 aepsych-0.3.0/tests/generators/test_optimize_acqf_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1966 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/generators/test_random_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2645 2022-12-07 17:48:47.000000 aepsych-0.3.0/tests/generators/test_sobol_generator.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:55:04.554418 aepsych-0.3.0/tests/models/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/models/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2304 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/models/test_derivative_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    26061 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/models/test_gp_classification.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2877 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/models/test_gp_regression.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3014 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/models/test_monotonic_projection_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4945 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/models/test_monotonic_rejection_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    25668 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/models/test_pairwise_probit.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2995 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/models/test_utils.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2297 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/test_ThriftSocketWrapper.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      999 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/test_bench_testfuns.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    11024 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/test_benchmark.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    29365 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/test_config.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    20470 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/test_db.py
--rwxr-xr-x   0 craigsanders   (501) staff       (20)     7450 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/test_integration.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      767 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/test_likelihoods.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4051 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/test_lookahead.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    11726 2022-12-07 17:18:11.000000 aepsych-0.3.0/tests/test_mean_covar_factories.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    26794 2022-12-07 17:48:47.000000 aepsych-0.3.0/tests/test_server.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    10564 2022-12-07 17:48:47.000000 aepsych-0.3.0/tests/test_strategy.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1654 2022-12-07 17:48:47.000000 aepsych-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.832495 aepsych-0.4.0/
+-rw-r--r--   0 craigsanders   (501) staff       (20)    19407 2023-06-05 20:10:09.000000 aepsych-0.4.0/LICENSE
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4565 2023-06-05 20:25:35.831996 aepsych-0.4.0/PKG-INFO
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.664880 aepsych-0.4.0/aepsych/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      983 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/__init__.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.795551 aepsych-0.4.0/aepsych/acquisition/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1390 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      835 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/acquisition.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3043 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/bvn.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    13677 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/lookahead.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     7137 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/lookahead_utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3593 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/lse.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3775 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/mc_posterior_variance.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     6079 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/monotonic_rejection.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5332 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/mutual_information.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.814952 aepsych-0.4.0/aepsych/acquisition/objective/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      735 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/objective/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4307 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/objective/objective.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4702 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/objective/semi_p.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2433 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/rejection_sampler.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.886128 aepsych-0.4.0/aepsych/benchmark/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      868 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11291 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/benchmark.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    10521 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/pathos_benchmark.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    10010 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/problem.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     6920 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/test_functions.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    13010 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/config.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.898430 aepsych-0.4.0/aepsych/database/
+-rw-r--r--   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/database/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11554 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/database/db.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    17629 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/database/tables.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.908941 aepsych-0.4.0/aepsych/factory/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      608 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/factory/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11147 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/factory/factory.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.039654 aepsych-0.4.0/aepsych/generators/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1524 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4076 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/base.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.084667 aepsych-0.4.0/aepsych/generators/completion_criterion/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      749 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      885 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/min_asks.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1454 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/min_total_outcome_occurrences.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      757 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/min_total_tells.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      930 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/run_indefinitely.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1422 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/epsilon_greedy_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2871 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/manual_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     7978 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/monotonic_rejection_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4441 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/monotonic_thompson_sampler_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      736 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/multi_outcome_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    10425 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/optimize_acqf_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      732 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/pairwise_optimize_acqf_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      689 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/pairwise_sobol_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2797 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/random_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2576 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/semi_p.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3696 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/sobol_generator.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.098513 aepsych-0.4.0/aepsych/kernels/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/kernels/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1801 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/kernels/rbf_partial_grad.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.145436 aepsych-0.4.0/aepsych/likelihoods/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      552 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/likelihoods/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1053 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/likelihoods/bernoulli.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2465 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/likelihoods/ordinal.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4332 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/likelihoods/semi_p.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.154163 aepsych-0.4.0/aepsych/means/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/means/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1109 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/means/constant_partial_grad.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.294751 aepsych-0.4.0/aepsych/models/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1462 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    21304 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/base.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4684 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/derivative_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      675 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/exact_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    12946 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/gp_classification.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     6554 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/gp_regression.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    10235 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/monotonic_projection_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    13669 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/monotonic_rejection_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5847 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/multitask_regression.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2338 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/ordinal_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     7071 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/pairwise_probit.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    24658 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/models/semi_p.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2403 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/models/surrogate.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5322 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/models/utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5775 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/models/variational_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    16703 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/plotting.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.344816 aepsych-0.4.0/aepsych/server/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      282 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/__init__.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.439321 aepsych-0.4.0/aepsych/server/message_handlers/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1032 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1612 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_ask.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      748 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_can_model.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      758 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_exit.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      337 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_finish_strategy.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1125 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_get_config.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2056 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_info.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      760 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_params.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2518 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_query.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      682 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_resume.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4635 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_setup.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4951 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_tell.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5639 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/replay.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    16416 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/server.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5823 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/sockets.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2218 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    24592 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/strategy.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     9148 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1235 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/utils_logging.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      241 2023-06-05 20:24:32.000000 aepsych-0.4.0/aepsych/version.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.687806 aepsych-0.4.0/aepsych.egg-info/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4565 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/PKG-INFO
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5151 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/SOURCES.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)        1 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/dependency_links.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)      107 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/entry_points.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)      177 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/requires.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)       14 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/top_level.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)      178 2023-06-05 20:10:10.000000 aepsych-0.4.0/pyproject.toml
+-rw-r--r--   0 craigsanders   (501) staff       (20)       38 2023-06-05 20:25:35.832606 aepsych-0.4.0/setup.cfg
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1587 2023-06-05 20:14:09.000000 aepsych-0.4.0/setup.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.552017 aepsych-0.4.0/tests/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/__init__.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.592255 aepsych-0.4.0/tests/acquisition/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1019 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_lse.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4924 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_mi.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1822 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_monotonic.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1322 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_objective.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1353 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_rejection_sampler.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     6480 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/common.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.643681 aepsych-0.4.0/tests/generators/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3973 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_completion_criteria.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1868 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_epsilon_greedy_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1933 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_manual_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4248 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_optimize_acqf_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2794 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_random_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3492 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_sobol_generator.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.743207 aepsych-0.4.0/tests/models/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2304 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_derivative_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    26030 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_gp_classification.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3066 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_gp_regression.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1666 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_model_query.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3014 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_monotonic_projection_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4945 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_monotonic_rejection_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1627 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_multitask_regression.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    25878 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_pairwise_probit.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    17592 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_semi_p.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3096 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4458 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_variational_gp.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.751008 aepsych-0.4.0/tests/server/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/__init__.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.830998 aepsych-0.4.0/tests/server/message_handlers/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1535 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_can_model.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      774 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_handle_exit.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1471 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_handle_finish_strategy.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1766 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_handle_get_config.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2220 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_query_handlers.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1168 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_tell_handlers.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    13121 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/test_server.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2013 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_ThriftSocketWrapper.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     8589 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_ax_integration.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      999 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_bench_testfuns.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11024 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_benchmark.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    31034 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_config.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    20470 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_db.py
+-rwxr-xr-x   0 craigsanders   (501) staff       (20)     8765 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_integration.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      986 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_likelihoods.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4051 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_lookahead.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    12311 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_mean_covar_factories.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3017 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_multioutcome.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11224 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_strategy.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5975 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_utils.py
```

### Comparing `aepsych-0.3.0/LICENSE` & `aepsych-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/PKG-INFO` & `aepsych-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepsych
-Version: 0.3.0
+Version: 0.4.0
 Summary: Adaptive experimetation for psychophysics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AEPsych
```

### Comparing `aepsych-0.3.0/aepsych/__init__.py` & `aepsych-0.4.0/aepsych/__init__.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/acquisition/__init__.py` & `aepsych-0.4.0/aepsych/acquisition/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     MonotonicBernoulliMCMutualInformation,
 )
 from .objective import (
     FloorGumbelObjective,
     FloorLogitObjective,
     FloorProbitObjective,
     ProbitObjective,
+    semi_p,
 )
 
-
 lse_acqfs = [
     MonotonicMCLSE,
     GlobalMI,
     GlobalSUR,
     ApproxGlobalSUR,
     EAVC,
     LocalMI,
@@ -47,10 +47,11 @@
     "FloorGumbelObjective",
     "GlobalMI",
     "GlobalSUR",
     "ApproxGlobalSUR",
     "EAVC",
     "LocalMI",
     "LocalSUR",
+    "semi_p",
 ]
 
 Config.register_module(sys.modules[__name__])
```

### Comparing `aepsych-0.3.0/aepsych/acquisition/bvn.py` & `aepsych-0.4.0/aepsych/acquisition/bvn.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/acquisition/lookahead.py` & `aepsych-0.4.0/aepsych/acquisition/lookahead.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python3
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import cast, Optional, Tuple
+from typing import Optional, Tuple, cast
 
 import numpy as np
 import torch
 from aepsych.utils import make_scaled_sobol
 from botorch.acquisition import AcquisitionFunction
+from botorch.acquisition.input_constructors import acqf_input_constructor
 from botorch.acquisition.objective import PosteriorTransform
 from botorch.models.gpytorch import GPyTorchModel
 from botorch.utils.transforms import t_batch_mode_transform
 from scipy.stats import norm
 from torch import Tensor
 
 from .lookahead_utils import (
@@ -122,14 +123,85 @@
         elif lookahead_type == "posterior":
             self.lookahead_fn = lookahead_p_at_xstar
             self.gamma = None
         else:
             raise RuntimeError(f"Got unknown lookahead type {lookahead_type}!")
 
 
+## Local look-ahead acquisitions
+class LocalLookaheadAcquisitionFunction(LookaheadAcquisitionFunction):
+    def __init__(
+        self,
+        model: GPyTorchModel,
+        lookahead_type: str = "levelset",
+        target: Optional[float] = None,
+        posterior_transform: Optional[PosteriorTransform] = None,
+    ) -> None:
+        """
+        A localized look-ahead acquisition function.
+
+        Args:
+            model: The gpytorch model.
+            target: Threshold value to target in p-space.
+        """
+
+        super().__init__(model=model, target=target, lookahead_type=lookahead_type)
+        self.posterior_transform = posterior_transform
+
+    @t_batch_mode_transform(expected_q=1)
+    def forward(self, X: Tensor) -> Tensor:
+        """
+        Evaluate acquisition function at X.
+
+        Args:
+            X: (b x 1 x d) point at which to evalaute acquisition function.
+
+        Returns: (b) tensor of acquisition values.
+        """
+
+        Px, P1, P0, py1 = self.lookahead_fn(
+            model=self.model,
+            Xstar=X,
+            Xq=X,
+            gamma=self.gamma,
+            posterior_transform=self.posterior_transform,
+        )  # Return shape here has m=1.
+        return self._compute_acqf(Px, P1, P0, py1)
+
+    def _compute_acqf(self, Px: Tensor, P1: Tensor, P0: Tensor, py1: Tensor) -> Tensor:
+        raise NotImplementedError
+
+
+class LocalMI(LocalLookaheadAcquisitionFunction):
+    def _compute_acqf(self, Px: Tensor, P1: Tensor, P0: Tensor, py1: Tensor) -> Tensor:
+        return MI_fn(Px, P1, P0, py1)
+
+
+class LocalSUR(LocalLookaheadAcquisitionFunction):
+    def _compute_acqf(self, Px: Tensor, P1: Tensor, P0: Tensor, py1: Tensor) -> Tensor:
+        return SUR_fn(Px, P1, P0, py1)
+
+
+@acqf_input_constructor(LocalMI, LocalSUR)
+def construct_inputs_local_lookahead(
+    model: GPyTorchModel,
+    training_data,
+    lookahead_type="levelset",
+    target: Optional[float] = None,
+    posterior_transform: Optional[PosteriorTransform] = None,
+    **kwargs,
+):
+    return {
+        "model": model,
+        "lookahead_type": lookahead_type,
+        "target": target,
+        "posterior_transform": posterior_transform,
+    }
+
+
 ## Global look-ahead acquisitions
 class GlobalLookaheadAcquisitionFunction(LookaheadAcquisitionFunction):
     def __init__(
         self,
         model: GPyTorchModel,
         lookahead_type: str = "levelset",
         target: Optional[float] = None,
@@ -240,68 +312,14 @@
 
 
 class EAVC(GlobalLookaheadAcquisitionFunction):
     def _compute_acqf(self, Px: Tensor, P1: Tensor, P0: Tensor, py1: Tensor) -> Tensor:
         return EAVC_fn(Px, P1, P0, py1)
 
 
-## Local look-ahead acquisitions
-class LocalLookaheadAcquisitionFunction(LookaheadAcquisitionFunction):
-    def __init__(
-        self,
-        model: GPyTorchModel,
-        lookahead_type: str = "levelset",
-        target: Optional[float] = None,
-        posterior_transform: Optional[PosteriorTransform] = None,
-    ) -> None:
-        """
-        A localized look-ahead acquisition function.
-
-        Args:
-            model: The gpytorch model.
-            target: Threshold value to target in p-space.
-        """
-
-        super().__init__(model=model, target=target, lookahead_type=lookahead_type)
-        self.posterior_transform = posterior_transform
-
-    @t_batch_mode_transform(expected_q=1)
-    def forward(self, X: Tensor) -> Tensor:
-        """
-        Evaluate acquisition function at X.
-
-        Args:
-            X: (b x 1 x d) point at which to evalaute acquisition function.
-
-        Returns: (b) tensor of acquisition values.
-        """
-
-        Px, P1, P0, py1 = self.lookahead_fn(
-            model=self.model,
-            Xstar=X,
-            Xq=X,
-            gamma=self.gamma,
-            posterior_transform=self.posterior_transform,
-        )  # Return shape here has m=1.
-        return self._compute_acqf(Px, P1, P0, py1)
-
-    def _compute_acqf(self, Px: Tensor, P1: Tensor, P0: Tensor, py1: Tensor) -> Tensor:
-        raise NotImplementedError
-
-
-class LocalMI(LocalLookaheadAcquisitionFunction):
-    def _compute_acqf(self, Px: Tensor, P1: Tensor, P0: Tensor, py1: Tensor) -> Tensor:
-        return MI_fn(Px, P1, P0, py1)
-
-
-class LocalSUR(LocalLookaheadAcquisitionFunction):
-    def _compute_acqf(self, Px: Tensor, P1: Tensor, P0: Tensor, py1: Tensor) -> Tensor:
-        return SUR_fn(Px, P1, P0, py1)
-
-
 class MOCU(GlobalLookaheadAcquisitionFunction):
     """
     MOCU acquisition function given in expr. 4 of:
 
         Zhao, Guang, et al. "Uncertainty-aware active learning for optimal Bayesian classifier."
         International Conference on Learning Representations (ICLR) 2021.
     """
@@ -353,7 +371,32 @@
         current_score = self.scorefun(Px)
         lookahead_pq1_score = self.scorefun(P1)
         lookahead_pq0_score = self.scorefun(P0)
         lookahead_expected_score = lookahead_pq1_score * py1 + lookahead_pq0_score * (
             1 - py1
         )
         return (lookahead_expected_score - current_score).mean(-1)
+
+
+@acqf_input_constructor(GlobalMI, GlobalSUR, ApproxGlobalSUR, EAVC, MOCU, SMOCU, BEMPS)
+def construct_inputs_global_lookahead(
+    model: GPyTorchModel,
+    training_data,
+    lookahead_type="levelset",
+    target: Optional[float] = None,
+    posterior_transform: Optional[PosteriorTransform] = None,
+    query_set_size: Optional[int] = 256,
+    Xq: Optional[Tensor] = None,
+    **kwargs,
+):
+    lb = [bounds[0] for bounds in kwargs["bounds"]]
+    ub = [bounds[1] for bounds in kwargs["bounds"]]
+    Xq = Xq if Xq is not None else make_scaled_sobol(lb, ub, query_set_size)
+
+    return {
+        "model": model,
+        "lookahead_type": lookahead_type,
+        "target": target,
+        "posterior_transform": posterior_transform,
+        "query_set_size": query_set_size,
+        "Xq": Xq,
+    }
```

### Comparing `aepsych-0.3.0/aepsych/acquisition/lookahead_utils.py` & `aepsych-0.4.0/aepsych/acquisition/lookahead_utils.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/acquisition/lse.py` & `aepsych-0.4.0/aepsych/acquisition/lse.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Optional, Union
 
 import torch
 from aepsych.acquisition.objective import ProbitObjective
+from botorch.acquisition.input_constructors import acqf_input_constructor
 from botorch.acquisition.monte_carlo import (
     MCAcquisitionFunction,
     MCAcquisitionObjective,
     MCSampler,
 )
 from botorch.models.model import Model
 from botorch.sampling.normal import SobolQMCNormalSampler
@@ -80,7 +81,27 @@
         Returns:
             torch.Tensor: Value of the acquisition functiona at these points.
         """
 
         post = self.model.posterior(X)
         samples = self.sampler(post)  # num_samples x batch_shape x q x d_out
         return self.acquisition(self.objective(samples, X)).squeeze(-1)
+
+
+@acqf_input_constructor(MCLevelSetEstimation)
+def construct_inputs_lse(
+    model,
+    training_data,
+    objective=None,
+    target=0.75,
+    beta=3.84,
+    sampler=None,
+    **kwargs,
+):
+
+    return {
+        "model": model,
+        "objective": objective,
+        "target": target,
+        "beta": beta,
+        "sampler": sampler,
+    }
```

### Comparing `aepsych-0.3.0/aepsych/acquisition/mc_posterior_variance.py` & `aepsych-0.4.0/aepsych/acquisition/mc_posterior_variance.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # LICENSE file in the root directory of this source tree.
 
 from typing import Optional
 
 import torch
 from aepsych.acquisition.monotonic_rejection import MonotonicMCAcquisition
 from aepsych.acquisition.objective import ProbitObjective
+from botorch.acquisition.input_constructors import acqf_input_constructor
 from botorch.acquisition.monte_carlo import MCAcquisitionFunction
 from botorch.acquisition.objective import MCAcquisitionObjective
 from botorch.models.model import Model
 from botorch.sampling.base import MCSampler
 from botorch.sampling.normal import SobolQMCNormalSampler
 from botorch.utils.transforms import t_batch_mode_transform
 from torch import Tensor
@@ -82,10 +83,25 @@
         # RejectionSampler drops the final dim so we reaugment it
         # here for compatibility with non-Monotonic MCAcquisition
         if len(obj_samples.shape) == 2:
             obj_samples = obj_samples[..., None]
         return balv_acq(obj_samples)
 
 
+@acqf_input_constructor(MCPosteriorVariance)
+def construct_inputs(
+    model,
+    training_data,
+    objective=None,
+    sampler=None,
+    **kwargs,
+):
+    return {
+        "model": model,
+        "objective": objective,
+        "sampler": sampler,
+    }
+
+
 class MonotonicMCPosteriorVariance(MonotonicMCAcquisition):
     def acquisition(self, obj_samples: torch.Tensor) -> torch.Tensor:
         return balv_acq(obj_samples)
```

### Comparing `aepsych-0.3.0/aepsych/acquisition/monotonic_rejection.py` & `aepsych-0.4.0/aepsych/acquisition/monotonic_rejection.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/acquisition/mutual_information.py` & `aepsych-0.4.0/aepsych/acquisition/mutual_information.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from __future__ import annotations
 
 from typing import Optional
 
 import torch
 from aepsych.acquisition.monotonic_rejection import MonotonicMCAcquisition
+from botorch.acquisition.input_constructors import acqf_input_constructor
 from botorch.acquisition.monte_carlo import MCAcquisitionFunction
 from botorch.acquisition.objective import MCAcquisitionObjective
 from botorch.models.model import Model
 from botorch.sampling.base import MCSampler
 from botorch.sampling.normal import SobolQMCNormalSampler
 from botorch.utils.transforms import t_batch_mode_transform
 from torch import Tensor
@@ -108,14 +109,29 @@
         # RejectionSampler drops the final dim so we reaugment it
         # here for compatibility with non-Monotonic MCAcquisition
         if len(obj_samples.shape) == 2:
             obj_samples = obj_samples[..., None]
         return bald_acq(obj_samples)
 
 
+@acqf_input_constructor(BernoulliMCMutualInformation)
+def construct_inputs_mi(
+    model,
+    training_data,
+    objective=None,
+    sampler=None,
+    **kwargs,
+):
+    return {
+        "model": model,
+        "objective": objective,
+        "sampler": sampler,
+    }
+
+
 class MonotonicBernoulliMCMutualInformation(MonotonicMCAcquisition):
     def acquisition(self, obj_samples: torch.Tensor) -> torch.Tensor:
         """Evaluate the acquisition function value based on samples.
 
         Args:
             obj_samples (torch.Tensor): Samples from the model, transformed through the objective.
```

### Comparing `aepsych-0.3.0/aepsych/acquisition/objective.py` & `aepsych-0.4.0/aepsych/acquisition/objective/objective.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 
 import torch
 from botorch.acquisition.objective import MCAcquisitionObjective
 from torch import Tensor
 from torch.distributions.normal import Normal
 
 
-class ProbitObjective(MCAcquisitionObjective):
+class AEPsychObjective(MCAcquisitionObjective):
+    def inverse(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
+        raise NotImplementedError
+
+
+class ProbitObjective(AEPsychObjective):
     """Probit objective
 
     Transforms the input through the normal CDF (probit).
     """
 
     def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
         """Evaluates the objective (normal CDF).
@@ -44,15 +49,15 @@
 
         Returns:
             Tensor: [description]
         """
         return Normal(loc=0, scale=1).icdf(samples.squeeze(-1))
 
 
-class FloorLinkObjective(MCAcquisitionObjective):
+class FloorLinkObjective(AEPsychObjective):
     """
     Wrapper for objectives to add a floor, when
     the probability is known not to go below it.
     """
 
     def __init__(self, floor=0.5):
         self.floor = floor
```

### Comparing `aepsych-0.3.0/aepsych/acquisition/rejection_sampler.py` & `aepsych-0.4.0/aepsych/acquisition/rejection_sampler.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/benchmark/__init__.py` & `aepsych-0.4.0/aepsych/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/benchmark/benchmark.py` & `aepsych-0.4.0/aepsych/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/benchmark/pathos_benchmark.py` & `aepsych-0.4.0/aepsych/benchmark/pathos_benchmark.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/benchmark/problem.py` & `aepsych-0.4.0/aepsych/benchmark/problem.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/benchmark/test_functions.py` & `aepsych-0.4.0/aepsych/benchmark/test_functions.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/config.py` & `aepsych-0.4.0/aepsych/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
-
+import abc
 import ast
 import configparser
 import json
 import warnings
 from types import ModuleType
 from typing import Any, ClassVar, Dict, List, Mapping, Optional, Sequence, TypeVar
 
@@ -115,20 +115,20 @@
             for setting in self[section]:
                 if deduplicate and section != "common" and setting in self["common"]:
                     continue
                 _dict[section][setting] = self[section][setting]
         return _dict
 
     # Turn the metadata section into JSON.
-    def jsonifyMetadata(self):
+    def jsonifyMetadata(self) -> str:
         configdict = self.to_dict()
         return json.dumps(configdict["metadata"])
 
     # Turn the entire config into JSON format.
-    def jsonifyAll(self):
+    def jsonifyAll(self) -> str:
         configdict = self.to_dict()
         return json.dumps(configdict)
 
     def update(
         self,
         config_dict: Mapping[str, str] = None,
         config_fnames: Sequence[str] = None,
@@ -353,10 +353,23 @@
         ):
             return "0.0"
 
         else:
             raise RuntimeError("Unrecognized config format!")
 
 
+class ConfigurableMixin(abc.ABC):
+    @abc.abstractclassmethod
+    def get_config_options(cls, config: Config, name: str) -> Dict[str, Any]:  # noqa
+        raise NotImplementedError(
+            f"get_config_options hasn't been defined for {cls.__name__}!"
+        )
+
+    @classmethod
+    def from_config(cls, config: Config, name: Optional[str] = None):
+        return cls(**cls.get_config_options(config, name))
+
+
+Config.register_module(gpytorch.likelihoods)
 Config.register_module(gpytorch.kernels)
 Config.register_module(botorch.acquisition)
 Config.registered_names["None"] = None
```

### Comparing `aepsych-0.3.0/aepsych/database/db.py` & `aepsych-0.4.0/aepsych/database/db.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/database/tables.py` & `aepsych-0.4.0/aepsych/database/tables.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/factory/__init__.py` & `aepsych-0.4.0/aepsych/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/factory/factory.py` & `aepsych-0.4.0/aepsych/factory/factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 from configparser import NoOptionError
-from typing import Tuple
+from typing import Optional, Tuple
 
 import gpytorch
 import torch
 from aepsych.config import Config
 from aepsych.kernels.rbf_partial_grad import RBFKernelPartialObsGrad
 from aepsych.means.constant_partial_grad import ConstantMeanPartialObsGrad
+from aepsych.utils import get_dim
 from scipy.stats import norm
 
 """AEPsych factory functions.
 These functions generate a gpytorch Mean and Kernel objects from
 aepsych.config.Config configurations, including setting lengthscale
 priors and so on. They are primarily used for programmatically
 constructing modular AEPsych models from configs.
@@ -31,53 +32,78 @@
 # with a preference for small values to prevent oversmoothing. The idea
 # is taken from https://betanalpha.github.io/assets/case_studies/gaussian_processes.html#323_Informative_Prior_Model
 __default_invgamma_concentration = 4.6
 __default_invgamma_rate = 1.0
 
 
 def default_mean_covar_factory(
-    config: Config,
+    config: Optional[Config] = None, dim: Optional[int] = None
 ) -> Tuple[gpytorch.means.ConstantMean, gpytorch.kernels.ScaleKernel]:
     """Default factory for generic GP models
 
     Args:
-        config (Config): Object containing bounds (and potentially other
+        config (Config, optional): Object containing bounds (and potentially other
             config details).
+        dim (int, optional): Dimensionality of the parameter space. Must be provided
+            if config is None.
 
     Returns:
         Tuple[gpytorch.means.Mean, gpytorch.kernels.Kernel]: Instantiated
             ConstantMean and ScaleKernel with priors based on bounds.
     """
 
-    lb = config.gettensor("default_mean_covar_factory", "lb")
-    ub = config.gettensor("default_mean_covar_factory", "ub")
-    fixed_mean = config.getboolean(
-        "default_mean_covar_factory", "fixed_mean", fallback=False
-    )
-    lengthscale_prior = config.get(
-        "default_mean_covar_factory", "lengthscale_prior", fallback="gamma"
-    )
-    outputscale_prior = config.get(
-        "default_mean_covar_factory", "outputscale_prior", fallback="box"
-    )
-    kernel = config.getobj(
-        "default_mean_covar_factory", "kernel", fallback=gpytorch.kernels.RBFKernel
-    )
+    assert (config is not None) or (
+        dim is not None
+    ), "Either config or dim must be provided!"
+
+    fixed_mean = False
+    lengthscale_prior = "gamma"
+    outputscale_prior = "box"
+    kernel = gpytorch.kernels.RBFKernel
 
-    assert lb.shape[0] == ub.shape[0], "bounds shape mismatch!"
-    dim = lb.shape[0]
     mean = gpytorch.means.ConstantMean()
 
-    if fixed_mean:
-        try:
-            target = config.getfloat("default_mean_covar_factory", "target")
-            mean.constant.requires_grad_(False)
-            mean.constant.copy_(torch.tensor(norm.ppf(target)))
-        except NoOptionError:
-            raise RuntimeError("Config got fixed_mean=True but no target included!")
+    if config is not None:
+        fixed_mean = config.getboolean(
+            "default_mean_covar_factory", "fixed_mean", fallback=fixed_mean
+        )
+        lengthscale_prior = config.get(
+            "default_mean_covar_factory",
+            "lengthscale_prior",
+            fallback=lengthscale_prior,
+        )
+        outputscale_prior = config.get(
+            "default_mean_covar_factory",
+            "outputscale_prior",
+            fallback=outputscale_prior,
+        )
+        kernel = config.getobj("default_mean_covar_factory", "kernel", fallback=kernel)
+
+        if fixed_mean:
+            try:
+                target = config.getfloat("default_mean_covar_factory", "target")
+                mean.constant.requires_grad_(False)
+                mean.constant.copy_(torch.tensor(norm.ppf(target)))
+            except NoOptionError:
+                raise RuntimeError("Config got fixed_mean=True but no target included!")
+
+        if config.getboolean("common", "use_ax", fallback=False):
+            config_dim = get_dim(config)
+
+        else:
+            lb = config.gettensor("default_mean_covar_factory", "lb")
+            ub = config.gettensor("default_mean_covar_factory", "ub")
+            assert lb.shape[0] == ub.shape[0], "bounds shape mismatch!"
+            config_dim = lb.shape[0]
+
+        if dim is not None:
+            assert dim == config_dim, "Provided config does not match provided dim!"
+
+        else:
+            dim = config_dim
 
     if lengthscale_prior == "invgamma":
 
         ls_prior = gpytorch.priors.GammaPrior(
             concentration=__default_invgamma_concentration,
             rate=__default_invgamma_rate,
             transform=lambda x: 1 / x,
@@ -180,18 +206,23 @@
         config (Config): Config object containing (at least) bounds and optionally
             LSE target.
 
     Returns:
         Tuple[gpytorch.means.ConstantMean, gpytorch.kernels.AdditiveKernel]: Instantiated
             constant mean object and additive kernel object.
     """
-    lb = config.gettensor("song_mean_covar_factory", "lb")
-    ub = config.gettensor("song_mean_covar_factory", "ub")
-    assert lb.shape[0] == ub.shape[0], "bounds shape mismatch!"
-    dim = lb.shape[0]
+
+    if config.getboolean("common", "use_ax", fallback=False):
+        dim = get_dim(config)
+
+    else:
+        lb = config.gettensor("song_mean_covar_factory", "lb")
+        ub = config.gettensor("song_mean_covar_factory", "ub")
+        assert lb.shape[0] == ub.shape[0], "bounds shape mismatch!"
+        dim = lb.shape[0]
 
     mean = gpytorch.means.ConstantMean()
 
     try:
         target = config.getfloat("song_mean_covar_factory", "target")
     except NoOptionError:
         target = 0.75
```

### Comparing `aepsych-0.3.0/aepsych/generators/__init__.py` & `aepsych-0.4.0/aepsych/generators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,26 +8,34 @@
 import sys
 
 from ..config import Config
 from .epsilon_greedy_generator import EpsilonGreedyGenerator
 from .manual_generator import ManualGenerator
 from .monotonic_rejection_generator import MonotonicRejectionGenerator
 from .monotonic_thompson_sampler_generator import MonotonicThompsonSamplerGenerator
-from .optimize_acqf_generator import OptimizeAcqfGenerator
+from .multi_outcome_generator import MultiOutcomeOptimizationGenerator
+from .optimize_acqf_generator import AxOptimizeAcqfGenerator, OptimizeAcqfGenerator
 from .pairwise_optimize_acqf_generator import PairwiseOptimizeAcqfGenerator
 from .pairwise_sobol_generator import PairwiseSobolGenerator
 from .random_generator import RandomGenerator
-from .sobol_generator import SobolGenerator
+from .random_generator import AxRandomGenerator, RandomGenerator
+from .semi_p import IntensityAwareSemiPGenerator
+from .sobol_generator import AxSobolGenerator, SobolGenerator
 
 __all__ = [
     "OptimizeAcqfGenerator",
     "MonotonicRejectionGenerator",
     "MonotonicThompsonSamplerGenerator",
     "RandomGenerator",
     "SobolGenerator",
     "EpsilonGreedyGenerator",
     "ManualGenerator",
     "PairwiseOptimizeAcqfGenerator",
     "PairwiseSobolGenerator",
+    "AxOptimizeAcqfGenerator",
+    "AxSobolGenerator",
+    "IntensityAwareSemiPGenerator",
+    "MultiOutcomeOptimizationGenerator",
+    "AxRandomGenerator",
 ]
 
 Config.register_module(sys.modules[__name__])
```

### Comparing `aepsych-0.3.0/aepsych/generators/epsilon_greedy_generator.py` & `aepsych-0.4.0/aepsych/generators/epsilon_greedy_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import numpy as np
+import torch
 from aepsych.config import Config
 
 from ..models.base import ModelProtocol
 from .base import AEPsychGenerator
 from .optimize_acqf_generator import OptimizeAcqfGenerator
 
 
@@ -28,10 +29,11 @@
         epsilon = config.getfloat(classname, "epsilon", fallback=0.1)
         return cls(subgenerator=subgen, epsilon=epsilon)
 
     def gen(self, num_points: int, model: ModelProtocol):
         if num_points > 1:
             raise NotImplementedError("Epsilon-greedy batched gen is not implemented!")
         if np.random.uniform() < self.epsilon:
-            return np.random.uniform(low=model.lb, high=model.ub)
+            sample = np.random.uniform(low=model.lb, high=model.ub)
+            return torch.tensor(sample).reshape(1, -1)
         else:
             return self.subgenerator.gen(num_points, model)
```

### Comparing `aepsych-0.3.0/aepsych/generators/manual_generator.py` & `aepsych-0.4.0/aepsych/generators/manual_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/generators/monotonic_rejection_generator.py` & `aepsych-0.4.0/aepsych/generators/monotonic_rejection_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/generators/monotonic_thompson_sampler_generator.py` & `aepsych-0.4.0/aepsych/generators/monotonic_thompson_sampler_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.objective = objective()
         self.explore_features = explore_features
 
     def gen(
         self,
         num_points: int,  # Current implementation only generates 1 point at a time
         model: MonotonicRejectionGP,
-    ) -> np.ndarray:
+    ) -> torch.Tensor:
         """Query next point(s) to run by optimizing the acquisition function.
         Args:
             num_points (int, optional): Number of points to query.
             model (AEPsychMixin): Fitted model of the data.
         Returns:
             np.ndarray: Next set of point(s) to evaluate, [num_points x dim].
         """
@@ -82,15 +82,15 @@
             num_samples=self.n_samples,
             num_rejection_samples=self.n_rejection_samples,
         )
 
         # Find the point closest to target
         dist = torch.abs(self.objective(f_samp) - self.target_value)
         best_indx = torch.argmin(dist, dim=1)
-        return X[best_indx].numpy()
+        return torch.Tensor(X[best_indx])
 
     @classmethod
     def from_config(cls, config: Config):
         classname = cls.__name__
         n_samples = config.getint(classname, "num_samples", fallback=1)
         n_rejection_samples = config.getint(
             classname, "num_rejection_samples", fallback=500
@@ -102,9 +102,9 @@
 
         return cls(
             n_samples=n_samples,
             n_rejection_samples=n_rejection_samples,
             num_ts_points=num_ts_points,
             target_value=target,
             objective=objective,
-            explore_features=explore_features, # type: ignore
+            explore_features=explore_features,  # type: ignore
         )
```

### Comparing `aepsych-0.3.0/aepsych/generators/optimize_acqf_generator.py` & `aepsych-0.4.0/aepsych/generators/optimize_acqf_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 #!/usr/bin/env python3
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
+from __future__ import annotations
+
 import time
-from typing import Any, Dict, Optional
+from inspect import signature
+from typing import Any, cast, Dict, Optional
 
 import numpy as np
 import torch
-from aepsych.config import Config
-from aepsych.generators.base import AEPsychGenerator
+from aepsych.acquisition.acquisition import AEPsychAcquisition
+from aepsych.config import Config, ConfigurableMixin
+from aepsych.generators.base import AEPsychGenerationStep, AEPsychGenerator
 from aepsych.models.base import ModelProtocol
+from aepsych.models.surrogate import AEPsychSurrogate
 from aepsych.utils_logging import getLogger
+from ax.modelbridge import Models
+from ax.modelbridge.registry import Cont_X_trans
 from botorch.acquisition import AcquisitionFunction
 from botorch.acquisition.preference import AnalyticExpectedUtilityOfBestOption
 from botorch.optim import optimize_acqf
 from botorch.utils import draw_sobol_samples
 
 logger = getLogger()
 
@@ -60,15 +67,15 @@
         if self.acqf in self.baseline_requiring_acqfs:
             return self.acqf(
                 model=model, X_baseline=model.train_inputs[0], **self.acqf_kwargs
             )
         else:
             return self.acqf(model=model, **self.acqf_kwargs)
 
-    def gen(self, num_points: int, model: ModelProtocol, **gen_options) -> np.ndarray:
+    def gen(self, num_points: int, model: ModelProtocol, **gen_options) -> torch.Tensor:
         """Query next point(s) to run by optimizing the acquisition function.
         Args:
             num_points (int, optional): Number of points to query.
             model (ModelProtocol): Fitted model of the data.
         Returns:
             np.ndarray: Next set of point(s) to evaluate, [num_points x dim].
         """
@@ -81,15 +88,17 @@
             # output of super() is (q, dim) but the contract is (num_points, dim, 2)
             # so we need to split q into q and pairs and then move the pair dim to the end
             return qbatch_points.reshape(num_points, 2, -1).swapaxes(-1, -2)
 
         else:
             return self._gen(num_points=num_points, model=model, **gen_options)
 
-    def _gen(self, num_points: int, model: ModelProtocol, **gen_options) -> np.ndarray:
+    def _gen(
+        self, num_points: int, model: ModelProtocol, **gen_options
+    ) -> torch.Tensor:
         # eval should be inherited from superclass
         model.eval()  # type: ignore
         train_x = model.train_inputs[0]
         acqf = self._instantiate_acquisition_fn(model)
 
         logger.info("Starting gen...")
         starttime = time.time()
@@ -162,7 +171,93 @@
             acqf=acqf,
             acqf_kwargs=extra_acqf_args,
             restarts=restarts,
             samps=samps,
             max_gen_time=max_gen_time,
             stimuli_per_trial=stimuli_per_trial,
         )
+
+    @classmethod
+    def get_config_options(cls, config: Config, name: str):
+        return AxOptimizeAcqfGenerator.get_config_options(config, name)
+
+
+class AxOptimizeAcqfGenerator(AEPsychGenerationStep, ConfigurableMixin):
+    @classmethod
+    def get_config_options(cls, config: Config, name: str) -> Dict:
+        classname = "OptimizeAcqfGenerator"
+
+        model_class = config.getobj(name, "model", fallback=None)
+        model_options = model_class.get_config_options(config)
+
+        acqf_cls = config.getobj(name, "acqf", fallback=None)
+        if acqf_cls is None:
+            acqf_cls = config.getobj(classname, "acqf")
+
+        acqf_options = cls._get_acqf_options(acqf_cls, config)
+        gen_options = cls._get_gen_options(config)
+
+        max_fit_time = model_options["max_fit_time"]
+
+        model_kwargs = {
+            "surrogate": AEPsychSurrogate(
+                botorch_model_class=model_class,
+                mll_class=model_class.get_mll_class(),
+                model_options=model_options,
+                max_fit_time=max_fit_time,
+            ),
+            "acquisition_class": AEPsychAcquisition,
+            "botorch_acqf_class": acqf_cls,
+            "acquisition_options": acqf_options,
+            # The Y transforms are removed because they are incompatible with our thresholding-finding acqfs
+            # The target value doesn't get transformed, so it searches for the target in the wrong space.
+            "transforms": Cont_X_trans,  # TODO: Make LSE acqfs compatible with Y transforms
+        }
+
+        opts = {
+            "model": Models.BOTORCH_MODULAR,
+            "model_kwargs": model_kwargs,
+            "model_gen_kwargs": gen_options,
+        }
+
+        opts.update(super().get_config_options(config, name))
+
+        return opts
+
+    @classmethod
+    def _get_acqf_options(cls, acqf: AcquisitionFunction, config: Config):
+        class MissingValue:
+            pass
+
+        if acqf is not None:
+            acqf_name = acqf.__name__
+
+            acqf_args_expected = signature(acqf).parameters.keys()
+            acqf_args = {
+                k: config.getobj(
+                    acqf_name,
+                    k,
+                    fallback_type=float,
+                    fallback=MissingValue(),
+                    warn=False,
+                )
+                for k in acqf_args_expected
+            }
+            acqf_args = {
+                k: v for k, v in acqf_args.items() if not isinstance(v, MissingValue)
+            }
+            for k, v in acqf_args.items():
+                if hasattr(v, "from_config"):  # configure if needed
+                    acqf_args[k] = cast(Any, v).from_config(config)
+                elif isinstance(v, type):  # instaniate a class if needed
+                    acqf_args[k] = v()
+        else:
+            acqf_args = {}
+
+        return acqf_args
+
+    @classmethod
+    def _get_gen_options(cls, config: Config):
+        classname = "OptimizeAcqfGenerator"
+        restarts = config.getint(classname, "restarts", fallback=10)
+        samps = config.getint(classname, "samps", fallback=1000)
+        return {"restarts": restarts, "samps": samps}
```

### Comparing `aepsych-0.3.0/aepsych/generators/pairwise_optimize_acqf_generator.py` & `aepsych-0.4.0/aepsych/generators/pairwise_optimize_acqf_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/generators/pairwise_sobol_generator.py` & `aepsych-0.4.0/aepsych/generators/pairwise_sobol_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/generators/random_generator.py` & `aepsych-0.4.0/aepsych/generators/random_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python3
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Optional, Union
+from typing import Dict, Optional, Union
 
 import numpy as np
 import torch
 from aepsych.config import Config
-from aepsych.generators.base import AEPsychGenerator
+from aepsych.generators.base import AEPsychGenerationStep, AEPsychGenerator
 from aepsych.models.base import AEPsychMixin
 from aepsych.utils import _process_bounds
+from ax.modelbridge import Models
 
 
 class RandomGenerator(AEPsychGenerator):
     """Generator that generates points randomly without an acquisition function."""
 
     _requires_model = False
 
@@ -36,26 +37,44 @@
         self.lb, self.ub, self.dim = _process_bounds(lb, ub, dim)
         self.bounds_ = torch.stack([self.lb, self.ub])
 
     def gen(
         self,
         num_points: int = 1,
         model: Optional[AEPsychMixin] = None,  # included for API compatibility.
-    ) -> np.ndarray:
+    ) -> torch.Tensor:
         """Query next point(s) to run by randomly sampling the parameter space.
         Args:
             num_points (int, optional): Number of points to query. Currently, only 1 point can be queried at a time.
         Returns:
             np.ndarray: Next set of point(s) to evaluate, [num_points x dim].
         """
         X = self.bounds_[0] + torch.rand((num_points, self.bounds_.shape[1])) * (
             self.bounds_[1] - self.bounds_[0]
         )
-        return X.numpy()
+        return X
 
     @classmethod
     def from_config(cls, config: Config):
         classname = cls.__name__
         lb = config.gettensor(classname, "lb")
         ub = config.gettensor(classname, "ub")
         dim = config.getint(classname, "dim", fallback=None)
         return cls(lb=lb, ub=ub, dim=dim)
+
+
+class AxRandomGenerator(AEPsychGenerationStep):
+    classname = "RandomGenerator"
+    model = Models.UNIFORM
+
+    @classmethod
+    def get_config_options(cls, config: Config, name: str) -> Dict:
+        seed = config.getint(cls.classname, "seed", fallback=None)
+        deduplicate = config.getboolean(cls.classname, "deduplicate", fallback=True)
+        opts = {
+            "model": cls.model,
+            "model_kwargs": {"seed": seed, "deduplicate": deduplicate},
+        }
+
+        opts.update(super().get_config_options(config, name))
+
+        return opts
```

### Comparing `aepsych-0.3.0/aepsych/generators/sobol_generator.py` & `aepsych-0.4.0/aepsych/generators/sobol_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
+from __future__ import annotations
 
-from typing import Optional, Union
+from typing import Dict, Optional, Union
 
 import numpy as np
 import torch
 from aepsych.config import Config
-from aepsych.generators.base import AEPsychGenerator
+from aepsych.generators.base import AEPsychGenerationStep, AEPsychGenerator
 from aepsych.models.base import AEPsychMixin
 from aepsych.utils import _process_bounds
+from ax.modelbridge import Models
 from torch.quasirandom import SobolEngine
 
 
 class SobolGenerator(AEPsychGenerator):
     """Generator that generates points from the Sobol Sequence."""
 
     _requires_model = False
@@ -78,7 +80,27 @@
         dim = config.getint(classname, "dim", fallback=None)
         seed = config.getint(classname, "seed", fallback=None)
         stimuli_per_trial = config.getint(classname, "stimuli_per_trial")
 
         return cls(
             lb=lb, ub=ub, dim=dim, seed=seed, stimuli_per_trial=stimuli_per_trial
         )
+
+    @classmethod
+    def get_config_options(cls, config: Config, name: str):
+        return AxSobolGenerator.get_config_options(config, name)
+
+
+class AxSobolGenerator(AEPsychGenerationStep):
+    @classmethod
+    def get_config_options(cls, config: Config, name: str) -> Dict:
+        classname = "SobolGenerator"
+        seed = config.getint(classname, "seed", fallback=None)
+        scramble = config.getboolean(classname, "scramble", fallback=True)
+
+        opts = {
+            "model": Models.SOBOL,
+            "model_kwargs": {"seed": seed, "scramble": scramble},
+        }
+        opts.update(super().get_config_options(config, name))
+
+        return opts
```

### Comparing `aepsych-0.3.0/aepsych/kernels/rbf_partial_grad.py` & `aepsych-0.4.0/aepsych/kernels/rbf_partial_grad.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/likelihoods/bernoulli.py` & `aepsych-0.4.0/aepsych/likelihoods/bernoulli.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/likelihoods/ordinal.py` & `aepsych-0.4.0/aepsych/likelihoods/ordinal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+#!/usr/bin/env python3
+# Copyright (c) Facebook, Inc. and its affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
 from typing import Callable, Optional
 
 import gpytorch
 import torch
 from gpytorch.likelihoods import Likelihood
 from torch.distributions import Categorical, Normal
```

### Comparing `aepsych-0.3.0/aepsych/means/constant_partial_grad.py` & `aepsych-0.4.0/aepsych/means/constant_partial_grad.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/models/base.py` & `aepsych-0.4.0/aepsych/models/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 from __future__ import annotations
 
+import abc
+
 import time
 from typing import Any, Dict, List, Mapping, Optional, Protocol, Tuple, Union
 
 import gpytorch
 import numpy as np
 import torch
-from aepsych.utils import dim_grid, get_jnd_multid, make_scaled_sobol
+
+from aepsych.config import Config, ConfigurableMixin
+from aepsych.factory.factory import default_mean_covar_factory
+from aepsych.models.utils import get_extremum
+from aepsych.utils import dim_grid, get_jnd_multid, make_scaled_sobol, promote_0d
 from aepsych.utils_logging import getLogger
-from botorch.acquisition import PosteriorMean
 from botorch.fit import fit_gpytorch_mll, fit_gpytorch_mll_scipy
 from botorch.models.gpytorch import GPyTorchModel
-from botorch.optim import optimize_acqf
 from botorch.posteriors import GPyTorchPosterior
 from gpytorch.likelihoods import Likelihood
 from gpytorch.mlls import MarginalLogLikelihood
 from scipy.optimize import minimize
 from scipy.stats import norm
 
 logger = getLogger()
@@ -108,70 +112,43 @@
     extremum_solver = "Nelder-Mead"
     outcome_types: List[str] = []
 
     @property
     def bounds(self):
         return torch.stack((self.lb, self.ub))
 
-    def _get_extremum(
-        self: ModelProtocol,
-        extremum_type: str,
-        locked_dims: Optional[Mapping[int, List[float]]] = None,
-        n_samples: int = 1000,
-    ) -> Tuple[float, np.ndarray]:
-        """Return the extremum (min or max) of the modeled function
-        Args:
-            extremum_type (str): type of extremum (currently 'min' or 'max'
-            n_samples (int, optional): number of coarse grid points to sample for optimization estimate.
-        Returns:
-            Tuple[float, np.ndarray]: Tuple containing the min and its location (argmin).
-        """
-        locked_dims = locked_dims or {}
-
-        acqf = PosteriorMean(model=self, maximize=(extremum_type == "max"))
-        bounds = torch.stack((self.lb, self.ub))
-        best_point, best_val = optimize_acqf(
-            acq_function=acqf,
-            bounds=bounds,
-            q=1,
-            num_restarts=10,
-            raw_samples=n_samples,
-            fixed_features=locked_dims,
-        )
-
-        # PosteriorMean flips the sign on minimize, we flip it back
-        if extremum_type == "min":
-            best_val = -best_val
-        return best_val, best_point.squeeze(0)
-
     def get_max(
         self: ModelProtocol,
         locked_dims: Optional[Mapping[int, List[float]]] = None,
+        n_samples: int = 1000,
     ) -> Tuple[float, np.ndarray]:
         """Return the maximum of the modeled function, subject to constraints
         Returns:
             Tuple[float, np.ndarray]: Tuple containing the max and its location (argmax).
             locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
                 inverse is along a slice of the full surface.
+            n_samples int: number of coarse grid points to sample for optimization estimate.
         """
         locked_dims = locked_dims or {}
-        return self._get_extremum("max", locked_dims)
+        return get_extremum(self, "max", self.bounds, locked_dims, n_samples)
 
     def get_min(
         self: ModelProtocol,
         locked_dims: Optional[Mapping[int, List[float]]] = None,
+        n_samples: int = 1000,
     ) -> Tuple[float, np.ndarray]:
         """Return the minimum of the modeled function, subject to constraints
         Returns:
             Tuple[float, np.ndarray]: Tuple containing the min and its location (argmin).
             locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
                 inverse is along a slice of the full surface.
+            n_samples int: number of coarse grid points to sample for optimization estimate.
         """
         locked_dims = locked_dims or {}
-        return self._get_extremum("min", locked_dims)
+        return get_extremum(self, "min", self.bounds, locked_dims, n_samples)
 
     def inv_query(
         self: ModelProtocol,
         y: float,
         locked_dims: Optional[Mapping[int, List[float]]] = None,
         probability_space: bool = False,
         n_samples: int = 1000,
@@ -391,18 +368,218 @@
             starttime = time.time()
             _ = mll(self(train_x), train_y)
             single_eval_time = time.time() - starttime
             n_eval = int(max_fit_time / single_eval_time)
             optimizer_kwargs["options"] = {"maxfun": n_eval}
             logger.info(f"fit maxfun is {n_eval}")
 
-        logger.info("Starting fit...")
         starttime = time.time()
         res = fit_gpytorch_mll(
             mll, optimizer=optimizer, optimizer_kwargs=optimizer_kwargs, **kwargs
         )
-        logger.info(f"Fit done, time={time.time()-starttime}")
         return res
 
     def p_below_threshold(self, x, f_thresh) -> np.ndarray:
         f, var = self.predict(x)
         return norm.cdf((f_thresh - f.detach().numpy()) / var.sqrt().detach().numpy())
+
+
+class AEPsychModel(ConfigurableMixin, abc.ABC):
+    extremum_solver = "Nelder-Mead"
+    outcome_type: Optional[str] = None
+
+    def predict(
+        self: GPyTorchModel, x: Union[torch.Tensor, np.ndarray]
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """Query the model for posterior mean and variance.
+
+        Args:
+            x (Union[torch.Tensor, np.ndarray]): Points at which to predict from the model.
+
+        Returns:
+            Tuple[torch.Tensor, torch.Tensor]: Posterior mean and variance at queried points.
+        """
+        with torch.no_grad():
+            post = self.posterior(x)
+        fmean = post.mean.squeeze()
+        fvar = post.variance.squeeze()
+        return promote_0d(fmean), promote_0d(fvar)
+
+    def predict_probability(self: GPyTorchModel, x: Union[torch.Tensor, np.ndarray]):
+        raise NotImplementedError
+
+    def sample(
+        self: GPyTorchModel, x: Union[torch.Tensor, np.ndarray], n: int
+    ) -> torch.Tensor:
+        """Sample the model posterior at the given points.
+
+        Args:
+            x (Union[torch.Tensor, np.ndarray]): Points at which to sample from the model.
+            n (int): Number of samples to take at each point.
+
+        Returns:
+            torch.Tensor: Posterior samples at queried points. Shape is n x len(x) x number of outcomes.
+        """
+        return self.posterior(x).sample(torch.Size([n]))
+
+    @classmethod
+    def get_config_options(cls, config: Config, name: Optional[str] = None) -> Dict:
+        if name is None:
+            name = cls.__name__
+
+        mean_covar_factory = config.getobj(
+            name, "mean_covar_factory", fallback=default_mean_covar_factory
+        )
+        mean, covar = mean_covar_factory(config)
+
+        likelihood_cls = config.getobj(name, "likelihood", fallback=None)
+        if likelihood_cls is not None:
+            if hasattr(likelihood_cls, "from_config"):
+                likelihood = likelihood_cls.from_config(config)
+            else:
+                likelihood = likelihood_cls()
+        else:
+            likelihood = None  # fall back to __init__ default
+
+        max_fit_time = config.getfloat(name, "max_fit_time", fallback=None)
+
+        options = {
+            "likelihood": likelihood,
+            "covar_module": covar,
+            "mean_module": mean,
+            "max_fit_time": max_fit_time,
+        }
+
+        return options
+
+    @classmethod
+    def construct_inputs(cls, training_data, **kwargs):
+        train_X = training_data.X()
+        train_Y = training_data.Y()
+
+        likelihood = kwargs.get("likelihood")
+        covar_module = kwargs.get("covar_module")
+        mean_module = kwargs.get("mean_module")
+
+        inputs = {
+            "train_X": train_X,
+            "train_Y": train_Y,
+            "likelihood": likelihood,
+            "covar_module": covar_module,
+            "mean_module": mean_module,
+        }
+
+        return inputs
+
+    def get_max(
+        self,
+        bounds: torch.Tensor,
+        locked_dims: Optional[Mapping[int, List[float]]] = None,
+        n_samples: int = 1000,
+    ) -> Tuple[float, np.ndarray]:
+        """Return the maximum of the modeled function, subject to constraints
+        Args:
+            bounds (torch.Tensor): The lower and upper bounds in the parameter space to search for the maximum,
+                formatted as a 2xn tensor, where d is the number of parameters.
+            locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
+                    inverse is along a slice of the full surface.
+            n_samples int: number of coarse grid points to sample for optimization estimate.
+        Returns:
+            Tuple[torch.Tensor, torch.Tensor]: Tuple containing the max and its location (argmax).
+        """
+        locked_dims = locked_dims or {}
+        return get_extremum(self, "max", bounds, locked_dims, n_samples)
+
+    def get_min(
+        self,
+        bounds: torch.Tensor,
+        locked_dims: Optional[Mapping[int, List[float]]] = None,
+        n_samples: int = 1000,
+    ) -> Tuple[float, np.ndarray]:
+        """Return the minimum of the modeled function, subject to constraints
+        Args:
+            bounds (torch.Tensor): The lower and upper bounds in the parameter space to search for the minimum,
+                formatted as a 2xn tensor, where d is the number of parameters.
+            locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
+                inverse is along a slice of the full surface.
+        Returns:
+            Tuple[torch.Tensor, torch.Tensor]: Tuple containing the min and its location (argmin).
+        """
+        locked_dims = locked_dims or {}
+        return get_extremum(self, "min", bounds, locked_dims, n_samples)
+
+    def inv_query(
+        self,
+        y: float,
+        bounds: torch.Tensor,
+        locked_dims: Optional[Mapping[int, List[float]]] = None,
+        probability_space: bool = False,
+        n_samples: int = 1000,
+    ) -> Tuple[float, torch.Tensor]:
+        """Query the model inverse.
+        Return nearest x such that f(x) = queried y, and also return the
+            value of f at that point.
+        Args:
+            y (float): Points at which to find the inverse.
+            locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
+                inverse is along a slice of the full surface.
+            probability_space (bool): Is y (and therefore the
+                returned nearest_y) in probability space instead of latent
+                function space? Defaults to False.
+        Returns:
+            Tuple[float, np.ndarray]: Tuple containing the value of f
+                nearest to queried y and the x position of this value.
+        """
+        if probability_space:
+            assert (
+                self.outcome_type == "binary" or self.outcome_type is None
+            ), f"Cannot get probability space for outcome_type '{self.outcome_type}'"
+            pred_function = self.predict_probability
+
+        else:
+            pred_function = self.predict
+
+        locked_dims = locked_dims or {}
+
+        def model_distance(x, pt, probability_space):
+            return np.abs(pred_function(torch.tensor([x]))[0].detach().numpy() - pt)
+
+        # Look for point with value closest to y, subject the dict of locked dims
+
+        query_lb = bounds[0]
+        query_ub = bounds[-1]
+
+        for locked_dim in locked_dims.keys():
+            dim_values = locked_dims[locked_dim]
+            if len(dim_values) == 1:
+                query_lb[locked_dim] = dim_values[0]
+                query_ub[locked_dim] = dim_values[0]
+            else:
+                query_lb[locked_dim] = dim_values[0]
+                query_ub[locked_dim] = dim_values[1]
+
+        d = make_scaled_sobol(query_lb, query_ub, n_samples, seed=0)
+
+        opt_bounds = zip(query_lb.numpy(), query_ub.numpy())
+
+        fmean, _ = pred_function(d)
+
+        f = torch.abs(fmean - y)
+        estimate = d[torch.where(f == torch.min(f))[0][0]].numpy()
+        a = minimize(
+            model_distance,
+            estimate,
+            args=(y, probability_space),
+            method=self.extremum_solver,
+            bounds=opt_bounds,
+        )
+        val = pred_function(torch.tensor([a.x]))[0].item()
+        return val, torch.Tensor(a.x)
+
+    @abc.abstractmethod
+    def get_mll_class(self):
+        raise NotImplementedError
+
+    def fit(self):
+        mll_class = self.get_mll_class()
+        mll = mll_class(self.likelihood, self)
+        fit_gpytorch_mll(mll)
```

### Comparing `aepsych-0.3.0/aepsych/models/derivative_gp.py` & `aepsych-0.4.0/aepsych/models/derivative_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/models/gp_classification.py` & `aepsych-0.4.0/aepsych/models/gp_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import torch
 from aepsych.config import Config
 from aepsych.factory.factory import default_mean_covar_factory
 from aepsych.models.base import AEPsychMixin
 from aepsych.models.utils import select_inducing_points
 from aepsych.utils import _process_bounds, promote_0d
 from aepsych.utils_logging import getLogger
-from gpytorch.likelihoods import BernoulliLikelihood, Likelihood
+from gpytorch.likelihoods import BernoulliLikelihood, BetaLikelihood, Likelihood
 from gpytorch.models import ApproximateGP
 from gpytorch.variational import CholeskyVariationalDistribution, VariationalStrategy
 from scipy.special import owens_t
 from scipy.stats import norm
 from torch.distributions import Normal
 
 logger = getLogger()
@@ -100,23 +100,15 @@
             inducing_points,
             variational_distribution,
             learn_inducing_locations=False,
         )
         super().__init__(variational_strategy)
 
         if mean_module is None or covar_module is None:
-            config = Config(
-                config_dict={
-                    "default_mean_covar_factory": {
-                        "lb": str(self.lb.tolist()),
-                        "ub": str(self.ub.tolist()),
-                    }
-                }
-            )  # type: ignore
-            default_mean, default_covar = default_mean_covar_factory(config)
+            default_mean, default_covar = default_mean_covar_factory(dim=self.dim)
 
         self.mean_module = mean_module or default_mean
         self.covar_module = covar_module or default_covar
         self.likelihood = likelihood
 
         self._fresh_state_dict = deepcopy(self.state_dict())
         self._fresh_likelihood_dict = deepcopy(self.likelihood.state_dict())
@@ -185,15 +177,15 @@
         state_dict.update(vsd_hack)
         self.load_state_dict(state_dict)
         self.likelihood.load_state_dict(self._fresh_likelihood_dict)
 
     def _reset_variational_strategy(self):
         inducing_points = select_inducing_points(
             inducing_size=self.inducing_size,
-            model=self,
+            covar_module=self.covar_module,
             X=self.train_inputs[0],
             bounds=self.bounds,
             method=self.inducing_point_method,
         )
         variational_distribution = CholeskyVariationalDistribution(
             inducing_points.size(0), batch_shape=torch.Size([self._batch_size])
         )
@@ -263,16 +255,16 @@
                 response probability instead of latent function value. Defaults to False.
 
         Returns:
             Tuple[np.ndarray, np.ndarray]: Posterior mean and variance at queries points.
         """
         with torch.no_grad():
             post = self.posterior(x)
-        fmean = post.mean.squeeze()
-        fvar = post.variance.squeeze()
+            fmean = post.mean.squeeze()
+            fvar = post.variance.squeeze()
         if probability_space:
             if isinstance(self.likelihood, BernoulliLikelihood):
                 # Probability-space mean and variance for Bernoulli-probit models is
                 # available in closed form, Proposition 1 in Letham et al. 2022 (AISTATS).
                 a_star = fmean / torch.sqrt(1 + fvar)
                 pmean = Normal(0, 1).cdf(a_star)
                 t_term = torch.tensor(
@@ -289,12 +281,47 @@
                     psamps = norm.cdf(fsamps)
                 pmean, pvar = psamps.mean(0), psamps.var(0)
                 return promote_0d(pmean), promote_0d(pvar)
 
         else:
             return promote_0d(fmean), promote_0d(fvar)
 
+    def predict_probability(
+        self, x: Union[torch.Tensor, np.ndarray]
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        return self.predict(x, probability_space=True)
+
     def update(self, train_x: torch.Tensor, train_y: torch.Tensor, **kwargs):
         """Perform a warm-start update of the model from previous fit."""
         return self.fit(
             train_x, train_y, warmstart_hyperparams=True, warmstart_induc=True, **kwargs
         )
+
+
+class GPBetaRegressionModel(GPClassificationModel):
+    outcome_type = "percentage"
+
+    def __init__(
+        self,
+        lb: Union[np.ndarray, torch.Tensor],
+        ub: Union[np.ndarray, torch.Tensor],
+        dim: Optional[int] = None,
+        mean_module: Optional[gpytorch.means.Mean] = None,
+        covar_module: Optional[gpytorch.kernels.Kernel] = None,
+        likelihood: Optional[Likelihood] = None,
+        inducing_size: int = 100,
+        max_fit_time: Optional[float] = None,
+        inducing_point_method: str = "auto",
+    ):
+        if likelihood is None:
+            likelihood = BetaLikelihood()
+        super().__init__(
+            lb=lb,
+            ub=ub,
+            dim=dim,
+            mean_module=mean_module,
+            covar_module=covar_module,
+            likelihood=likelihood,
+            inducing_size=inducing_size,
+            max_fit_time=max_fit_time,
+            inducing_point_method=inducing_point_method,
+        )
```

### Comparing `aepsych-0.3.0/aepsych/models/gp_regression.py` & `aepsych-0.4.0/aepsych/models/gp_regression.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import Optional, Tuple, Union
+from typing import Dict, Optional, Tuple, Union
 
 import gpytorch
 import numpy as np
 import torch
 from aepsych.config import Config
 from aepsych.factory.factory import default_mean_covar_factory
 from aepsych.models.base import AEPsychMixin
@@ -36,15 +36,14 @@
         lb: Union[np.ndarray, torch.Tensor],
         ub: Union[np.ndarray, torch.Tensor],
         dim: Optional[int] = None,
         mean_module: Optional[gpytorch.means.Mean] = None,
         covar_module: Optional[gpytorch.kernels.Kernel] = None,
         likelihood: Optional[Likelihood] = None,
         max_fit_time: Optional[float] = None,
-        num_outputs: Optional[int] = None,
     ):
         """Initialize the GP regression model
 
         Args:
             lb (Union[numpy.ndarray, torch.Tensor]): Lower bounds of the parameters.
             ub (Union[numpy.ndarray, torch.Tensor]): Upper bounds of the parameters.
             dim (int, optional): The number of dimensions in the parameter space. If None, it is inferred from the size
@@ -56,55 +55,30 @@
                 Gaussian likelihood.
             max_fit_time (float, optional): The maximum amount of time, in seconds, to spend fitting the model. If None,
                 there is no limit to the fitting time.
         """
         if likelihood is None:
             likelihood = GaussianLikelihood()
 
-        if num_outputs is not None:
-            self._num_outputs = num_outputs
-            self._batch_size = num_outputs
-
         super().__init__(None, None, likelihood)
 
         self.lb, self.ub, self.dim = _process_bounds(lb, ub, dim)
         self.max_fit_time = max_fit_time
 
         if mean_module is None or covar_module is None:
-            config = Config(
-                config_dict={
-                    "default_mean_covar_factory": {
-                        "lb": str(self.lb.tolist()),
-                        "ub": str(self.ub.tolist()),
-                        "num_outputs": num_outputs,
-                    }
-                }
-            )  # type: ignore
-            default_mean, default_covar = default_mean_covar_factory(config)
+            default_mean, default_covar = default_mean_covar_factory(dim=self.dim)
 
         self.mean_module = mean_module or default_mean
         self.covar_module = covar_module or default_covar
 
         self._fresh_state_dict = deepcopy(self.state_dict())
         self._fresh_likelihood_dict = deepcopy(self.likelihood.state_dict())
 
     @classmethod
-    def from_config(cls, config: Config) -> GPRegressionModel:
-        """Alternate constructor for GP regression model.
-
-        This is used when we recursively build a full sampling strategy
-        from a configuration. TODO: document how this works in some tutorial.
-
-        Args:
-            config (Config): A configuration containing keys/values matching this class
-
-        Returns:
-            GPRegressionModel: Configured class instance.
-        """
-
+    def construct_inputs(cls, config: Config) -> Dict:
         classname = cls.__name__
 
         lb = config.gettensor(classname, "lb")
         ub = config.gettensor(classname, "ub")
         dim = config.getint(classname, "dim", fallback=None)
 
         mean_covar_factory = config.getobj(
@@ -120,24 +94,41 @@
                 likelihood = likelihood_cls.from_config(config)
             else:
                 likelihood = likelihood_cls()
         else:
             likelihood = None  # fall back to __init__ default
 
         max_fit_time = config.getfloat(classname, "max_fit_time", fallback=None)
+        return {
+            "lb": lb,
+            "ub": ub,
+            "dim": dim,
+            "mean_module": mean,
+            "covar_module": covar,
+            "likelihood": likelihood,
+            "max_fit_time": max_fit_time,
+        }
 
-        return cls(
-            lb=lb,
-            ub=ub,
-            dim=dim,
-            mean_module=mean,
-            covar_module=covar,
-            likelihood=likelihood,
-            max_fit_time=max_fit_time,
-        )
+    @classmethod
+    def from_config(cls, config: Config) -> GPRegressionModel:
+        """Alternate constructor for GP regression model.
+
+        This is used when we recursively build a full sampling strategy
+        from a configuration. TODO: document how this works in some tutorial.
+
+        Args:
+            config (Config): A configuration containing keys/values matching this class
+
+        Returns:
+            GPRegressionModel: Configured class instance.
+        """
+
+        args = cls.construct_inputs(config)
+
+        return cls(**args)
 
     def fit(self, train_x: torch.Tensor, train_y: torch.Tensor, **kwargs) -> None:
         """Fit underlying model.
 
         Args:
             train_x (torch.Tensor): Inputs.
             train_y (torch.LongTensor): Responses.
```

### Comparing `aepsych-0.3.0/aepsych/models/monotonic_projection_gp.py` & `aepsych-0.4.0/aepsych/models/monotonic_projection_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/models/monotonic_rejection_gp.py` & `aepsych-0.4.0/aepsych/models/monotonic_rejection_gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             train_x (Tensor): Training x points
             train_y (Tensor): Training y points. Should be (n x 1).
         """
         self.set_train_data(train_x, train_y)
 
         self.inducing_points = select_inducing_points(
             inducing_size=self.inducing_size,
-            model=self,
+            covar_module=self.covar_module,
             X=self.train_inputs[0],
             bounds=self.bounds,
             method=self.inducing_point_method,
         )
         self._set_model(train_x, train_y)
 
     def _set_model(
@@ -275,14 +275,19 @@
             return (
                 torch.Tensor(promote_0d(norm.cdf(mean))),
                 torch.Tensor(promote_0d(norm.cdf(variance))),
             )
 
         return mean, variance
 
+    def predict_probability(
+        self, x: Union[torch.Tensor, np.ndarray]
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        return self.predict(x, probability_space=True)
+
     def _augment_with_deriv_index(self, x: Tensor, indx):
         return torch.cat(
             (x, indx * torch.ones(x.shape[0], 1)),
             dim=1,
         )
 
     def _get_deriv_constraint_points(self):
```

### Comparing `aepsych-0.3.0/aepsych/models/ordinal_gp.py` & `aepsych-0.4.0/aepsych/models/ordinal_gp.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
     outcome_type = "ordinal"
 
     def __init__(self, likelihood=None, *args, **kwargs):
         covar_module = kwargs.pop("covar_module", None)
         dim = kwargs.get("dim")
         if covar_module is None:
-
             ls_prior = gpytorch.priors.GammaPrior(concentration=1.5, rate=3.0)
             ls_prior_mode = (ls_prior.concentration - 1) / ls_prior.rate
             ls_constraint = gpytorch.constraints.Positive(
                 transform=None, initial_value=ls_prior_mode
             )
 
             # no outputscale due to shift identifiability in d.
@@ -42,22 +41,25 @@
             covar_module=covar_module,
             likelihood=likelihood,
             **kwargs,
         )
 
     def predict_probs(self, xgrid):
         fmean, fvar = self.predict(xgrid)
+        return self.calculate_probs(fmean, fvar)
+
+    def calculate_probs(self, fmean, fvar):
         fsd = torch.sqrt(1 + fvar)
         probs = torch.zeros(*fmean.size(), self.likelihood.n_levels)
 
         probs[..., 0] = self.likelihood.link(
             (self.likelihood.cutpoints[0] - fmean) / fsd
         )
 
         for i in range(1, self.likelihood.n_levels - 1):
             probs[..., i] = self.likelihood.link(
                 (self.likelihood.cutpoints[i] - fmean) / fsd
             ) - self.likelihood.link((self.likelihood.cutpoints[i - 1] - fmean) / fsd)
         probs[..., -1] = 1 - self.likelihood.link(
             (self.likelihood.cutpoints[-1] - fmean) / fsd
         )
-        return probs
+        return probs
```

### Comparing `aepsych-0.3.0/aepsych/models/pairwise_probit.py` & `aepsych-0.4.0/aepsych/models/pairwise_probit.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,14 +138,21 @@
             return (
                 promote_0d(norm.cdf(fmean)),
                 promote_0d(norm.cdf(fvar)),
             )
         else:
             return fmean, fvar
 
+    def predict_probability(
+        self, x, probability_space=False, num_samples=1000, rereference="x_min"
+    ):
+        return self.predict(
+            x, probability_space=True, num_samples=num_samples, rereference=rereference
+        )
+
     def sample(self, x, num_samples, rereference="x_min"):
         if len(x.shape) < 2:
             x = x.reshape(-1, 1)
         if rereference is None:
             return self.posterior(x).rsample(torch.Size([num_samples]))
 
         if rereference == "x_min":
```

### Comparing `aepsych-0.3.0/aepsych/plotting.py` & `aepsych-0.4.0/aepsych/plotting.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/server/sockets.py` & `aepsych-0.4.0/aepsych/server/sockets.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych/strategy.py` & `aepsych-0.4.0/aepsych/server/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,486 +1,496 @@
 #!/usr/bin/env python3
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
-import time
+import argparse
+import io
+import logging
+import os
+import sys
+import threading
+import traceback
 import warnings
-from typing import List, Optional, Sequence, Tuple, Type, Union
 
+from typing import Optional
+
+import aepsych.database.db as db
+
+import aepsych.utils_logging as utils_logging
+import dill
 import numpy as np
+import pandas as pd
 import torch
 
-from aepsych.config import Config
-from aepsych.generators.base import AEPsychGenerator
-from aepsych.generators.sobol_generator import SobolGenerator
-from aepsych.models.base import ModelProtocol
-from aepsych.utils import _process_bounds, make_scaled_sobol
-from aepsych.utils_logging import getLogger
-from botorch.exceptions.errors import ModelFittingError
-
-logger = getLogger()
-
-
-def ensure_model_is_fresh(f):
-    def wrapper(self, *args, **kwargs):
-        if self.can_fit and not self._model_is_fresh:
-            starttime = time.time()
-            if self._count % self.refit_every == 0 or self.refit_every == 1:
-                logger.info("Starting fitting (no warm start)...")
-                # don't warm start
-                self.fit()
-            else:
-                logger.info("Starting fitting (warm start)...")
-                # warm start
-                self.update()
-            logger.info(f"Fitting done, took {time.time()-starttime}")
-        self._model_is_fresh = True
-        return f(self, *args, **kwargs)
-
-    return wrapper
+from aepsych.server.message_handlers import MESSAGE_MAP
+from aepsych.server.message_handlers.handle_ask import ask
+from aepsych.server.message_handlers.handle_setup import configure
+from aepsych.server.replay import (
+    get_dataframe_from_replay,
+    get_strat_from_replay,
+    get_strats_from_replay,
+    replay,
+)
+
+from aepsych.server.sockets import BAD_REQUEST, createSocket, DummySocket
+
+logger = utils_logging.getLogger(logging.INFO)
+DEFAULT_DESC = "default description"
+DEFAULT_NAME = "default name"
+
+
+def get_next_filename(folder, fname, ext):
+    """Generates appropriate filename for logging purposes."""
+    n = sum(1 for f in os.listdir(folder) if os.path.isfile(os.path.join(folder, f)))
+    return f"{folder}/{fname}_{n+1}.{ext}"
+
+
+class AEPsychServer(object):
+    def __init__(self, socket=None, database_path=None, thrift=False):
+        """Server for doing black box optimization using gaussian processes.
+        Keyword Arguments:
+            socket -- socket object that implements `send` and `receive` for json
+            messages (default: DummySocket()).
+            TODO actually make an abstract interface to subclass from here
+        """
+        if socket is None:
+            self.socket = DummySocket()
+        else:
+            self.socket = socket
+        self.db = None
+        self.is_performing_replay = False
+        self.exit_server_loop = False
+        self._db_master_record = None
+        self._db_raw_record = None
+        self.db = db.Database(database_path)
+        self.skip_computations = False
+        self.strat_names = None
+
+        if self.db.is_update_required():
+            self.db.perform_updates()
+
+        self._strats = []
+        self._parnames = []
+        self._configs = []
+        self.strat_id = -1
+        self._pregen_asks = []
+        self.enable_pregen = False
+
+        self.debug = False
+        self.is_using_thrift = thrift
+        self.receive_thread = threading.Thread(
+            target=self._receive_send, args=(self.exit_server_loop,), daemon=True
+        )
 
+        self.queue = []
 
-class Strategy(object):
-    """Object that combines models and generators to generate points to sample."""
+    def cleanup(self):
+        """Close the socket and terminate connection to the server.
 
-    _n_eval_points: int = 1000
+        Returns:
+            None
+        """
+        self.socket.close()
 
-    def __init__(
-        self,
-        generator: AEPsychGenerator,
-        lb: Union[np.ndarray, torch.Tensor],
-        ub: Union[np.ndarray, torch.Tensor],
-        stimuli_per_trial: int,
-        outcome_types: Sequence[Type[str]],
-        dim: Optional[int] = None,
-        min_total_tells: int = 0,
-        min_asks: int = 0,
-        model: Optional[ModelProtocol] = None,
-        refit_every: int = 1,
-        min_total_outcome_occurrences: int = 1,
-        max_asks: Optional[int] = None,
-        keep_most_recent: Optional[int] = None,
-        min_post_range: Optional[float] = None,
-        name: str = "",
-        run_indefinitely: bool = False,
-    ):
-        """Initialize the strategy object.
+    def _receive_send(self, is_exiting: bool) -> None:
+        """Receive messages from the client.
 
         Args:
-            generator (AEPsychGenerator): The generator object that determines how points are sampled.
-            lb (Union[numpy.ndarray, torch.Tensor]): Lower bounds of the parameters.
-            ub (Union[numpy.ndarray, torch.Tensor]): Upper bounds of the parameters.
-            dim (int, optional): The number of dimensions in the parameter space. If None, it is inferred from the size
-                of lb and ub.
-            min_total_tells (int): The minimum number of total observations needed to complete this strategy.
-            min_asks (int): The minimum number of points that should be generated from this strategy.
-            model (ModelProtocol, optional): The AEPsych model of the data.
-            refit_every (int): How often to refit the model from scratch.
-            min_total_outcome_occurrences (int): The minimum number of total observations needed for each outcome before the strategy will finish.
-                Defaults to 1 (i.e., for binary outcomes, there must be at least one "yes" trial and one "no" trial).
-            max_asks (int, optional): The maximum number of trials to generate using this strategy.
-                If None, there is no upper bound (default).
-            keep_most_recent (int, optional): Experimental. The number of most recent data points that the model will be fitted on.
-                This may be useful for discarding noisy data from trials early in the experiment that are not as informative
-                as data collected from later trials. When None, the model is fitted on all data.
-            min_post_range (float, optional): Experimental. The required difference between the posterior's minimum and maximum value in
-                probablity space before the strategy will finish. Ignored if None (default).
-            name (str): The name of the strategy. Defaults to the empty string.
-            run_indefinitely (bool): If true, the strategy will run indefinitely until finish() is explicitly called. Other stopping criteria will
-                be ignored. Defaults to False.
+            is_exiting (bool): True to terminate reception of new messages from the client, False otherwise.
+
+        Returns:
+            None
         """
-        self.is_finished = False
+        while True:
+            request = self.socket.receive(is_exiting)
+            if request != BAD_REQUEST:
+                self.queue.append(request)
+            if self.exit_server_loop:
+                break
+        logger.info("Terminated input thread")
 
-        if run_indefinitely:
-            warnings.warn(
-                f"Strategy {name} will run indefinitely until finish() is explicitly called. Other stopping criteria will be ignored."
-            )
+    def _handle_queue(self) -> None:
+        """Handles the queue of messages received by the server.
 
-        elif min_total_tells > 0 and min_asks > 0:
-            warnings.warn(
-                "Specifying both min_total_tells and min_asks > 0 may lead to unintended behavior."
-            )
+        Returns:
+            None
+        """
+        if self.queue:
+            request = self.queue.pop(0)
+            try:
+                result = self.handle_request(request)
+            except Exception as e:
+                error_message = f"Request '{request}' raised error '{e}'!"
+                result = f"server_error, {error_message}"
+                logger.error(f"{error_message}! Full traceback follows:")
+                logger.error(traceback.format_exc())
+            self.socket.send(result)
+        else:
+            if self.can_pregen_ask and (len(self._pregen_asks) == 0):
+                self._pregen_asks.append(ask(self))
 
-        if model is not None:
-            assert (
-                len(outcome_types) == model._num_outputs
-            ), f"Strategy has {len(outcome_types)} outcomes, but model {type(model).__name__} supports {model._num_outputs}!"
-            assert (
-                stimuli_per_trial == model.stimuli_per_trial
-            ), f"Strategy has {stimuli_per_trial} stimuli_per_trial, but model {type(model).__name__} supports {model.stimuli_per_trial}!"
-
-            if isinstance(model.outcome_type, str):
-                assert (
-                    len(outcome_types) == 1 and outcome_types[0] == model.outcome_type
-                ), f"Strategy outcome types is {outcome_types} but model outcome type is {model.outcome_type}!"
-            else:
-                assert set(outcome_types) == set(
-                    model.outcome_type
-                ), f"Strategy outcome types is {outcome_types} but model outcome type is {model.outcome_type}!"
-
-        self.run_indefinitely = run_indefinitely
-        self.lb, self.ub, self.dim = _process_bounds(lb, ub, dim)
-        self.min_total_outcome_occurrences = min_total_outcome_occurrences
-        self.max_asks = max_asks
-        self.keep_most_recent = keep_most_recent
-
-        self.min_post_range = min_post_range
-        if self.min_post_range is not None:
-            assert model is not None, "min_post_range must be None if model is None!"
-            self.eval_grid = make_scaled_sobol(
-                lb=self.lb, ub=self.ub, size=self._n_eval_points
-            )
+    def serve(self) -> None:
+        """Run the server. Note that all configuration outside of socket type and port
+        happens via messages from the client. The server simply forwards messages from
+        the client to its `setup`, `ask` and `tell` methods, and responds with either
+        acknowledgment or other response as needed. To understand the server API, see
+        the docs on the methods in this class.
+
+        Returns:
+            None
 
-        self.x = None
-        self.y = None
-        self.n = 0
-        self.min_asks = min_asks
-        self._count = 0
-        self.min_total_tells = min_total_tells
-        self.stimuli_per_trial = stimuli_per_trial
-        self.outcome_types = outcome_types
-
-        if self.stimuli_per_trial == 1:
-            self.event_shape: Tuple[int, ...] = (self.dim,)
-
-        if self.stimuli_per_trial == 2:
-            self.event_shape = (self.dim, self.stimuli_per_trial)
-
-        self.model = model
-        self.refit_every = refit_every
-        self._model_is_fresh = False
-        self.generator = generator
-        self.has_model = self.model is not None
-        if self.generator._requires_model:
-            assert self.model is not None, f"{self.generator} requires a model!"
+        Raises:
+            RuntimeError: if a request from a client has no request type
+            RuntimeError: if a request from a client has no known request type
+            TODO make things a little more robust to bad messages from client; this
+             requires resetting the req/rep queue status.
 
-        if self.min_asks == self.min_total_tells == 0:
+        """
+        logger.info("Server up, waiting for connections!")
+        logger.info("Ctrl-C to quit!")
+        # yeah we're not sanitizing input at all
+
+        # Start the method to accept a client connection
+
+        if self.is_using_thrift is True:
+            self.queue.append(self.socket.receive())
+            self._handle_queue()
+        else:
+            self.socket.accept_client()
+            self.receive_thread.start()
+            while True:
+                self._handle_queue()
+                if self.exit_server_loop:
+                    break
+            # Close the socket and terminate with code 0
+            self.cleanup()
+            sys.exit(0)
+
+    def _unpack_strat_buffer(self, strat_buffer):
+        if isinstance(strat_buffer, io.BytesIO):
+            strat = torch.load(strat_buffer, pickle_module=dill)
+            strat_buffer.seek(0)
+        elif isinstance(strat_buffer, bytes):
             warnings.warn(
-                "strategy.min_asks == strategy.min_total_tells == 0. This strategy will not generate any points!",
-                UserWarning,
+                "Strat buffer is not in bytes format!"
+                + " This is a deprecated format, loading using dill.loads.",
+                DeprecationWarning,
             )
+            strat = dill.loads(strat_buffer)
+        else:
+            raise RuntimeError("Trying to load strat in unknown format!")
+        return strat
 
-        self.name = name
+    def generate_experiment_table(
+        self,
+        experiment_id: str,
+        table_name: str = "experiment_table",
+        return_df: bool = False,
+    ) -> Optional[pd.DataFrame]:
+        """Generate a table of a given experiment with all the raw data.
 
-    def normalize_inputs(self, x, y):
-        """converts inputs into normalized format for this strategy
+        This table is generated from the database, and is added to the
+        experiment's database.
 
         Args:
-            x (np.ndarray): training inputs
-            y (np.ndarray): training outputs
+            experiment_id (str): The experiment ID to generate the table for.
+            table_name (str): The name of the table. Defaults to
+                "experiment_table".
+            return_df (bool): If True, also return the dataframe.
 
         Returns:
-            x (np.ndarray): training inputs, normalized
-            y (np.ndarray): training outputs, normalized
-            n (int): number of observations
+            pd.DataFrame: The dataframe of the experiment table, if
+                return_df is True.
         """
-        assert (
-            x.shape == self.event_shape or x.shape[1:] == self.event_shape
-        ), f"x shape should be {self.event_shape} or batch x {self.event_shape}, instead got {x.shape}"
-
-        if x.shape == self.event_shape:
-            x = x[None, :]
-
-        if self.x is None:
-            x = np.r_[x]
-        else:
-            x = np.r_[self.x, x]
+        param_space = self.db.get_param_for(experiment_id, 1)
+        outcome_space = self.db.get_outcome_for(experiment_id, 1)
 
-        if self.y is None:
-            y = np.r_[y]
-        else:
-            y = np.r_[self.y, y]
+        columns = []
+        columns.append("iteration_id")
+        for param in param_space:
+            columns.append(param.param_name)
+        for outcome in outcome_space:
+            columns.append(outcome.outcome_name)
+
+        columns.append("timestamp")
+
+        # Create dataframe
+        df = pd.DataFrame(columns=columns)
+
+        # Fill dataframe
+        for raw in self.db.get_raw_for(experiment_id):
+            row = {}
+            row["iteration_id"] = raw.unique_id
+            for param in raw.children_param:
+                row[param.param_name] = param.param_value
+            for outcome in raw.children_outcome:
+                row[outcome.outcome_name] = outcome.outcome_value
+            row["timestamp"] = raw.timestamp
+            # concat to dataframe
+            df = pd.concat([df, pd.DataFrame([row])], ignore_index=True)
 
-        n = y.shape[0]
+        # Make iteration_id the index
+        df.set_index("iteration_id", inplace=True)
 
-        return torch.Tensor(x), torch.Tensor(y), n
+        # Save to .db file
+        df.to_sql(table_name, self.db.get_engine(), if_exists="replace")
 
-    # TODO: allow user to pass in generator options
-    @ensure_model_is_fresh
-    def gen(self, num_points: int = 1):
-        """Query next point(s) to run by optimizing the acquisition function.
+        if return_df:
+            return df
+        else:
+            return None
 
-        Args:
-            num_points (int, optional): Number of points to query. Defaults to 1.
-            Other arguments are forwared to underlying model.
+    ### Properties that are set on a per-strat basis
+    @property
+    def strat(self):
+        if self.strat_id == -1:
+            return None
+        else:
+            return self._strats[self.strat_id]
 
-        Returns:
-            np.ndarray: Next set of point(s) to evaluate, [num_points x dim].
-        """
-        self._count = self._count + num_points
-        return self.generator.gen(num_points, self.model)
+    @strat.setter
+    def strat(self, s):
+        self._strats.append(s)
 
-    @ensure_model_is_fresh
-    def get_max(self, constraints=None):
-        constraints = constraints or {}
-        return self.model.get_max(constraints)
-
-    @ensure_model_is_fresh
-    def get_min(self, constraints=None):
-        constraints = constraints or {}
-        return self.model.get_min(constraints)
-
-    @ensure_model_is_fresh
-    def inv_query(self, y, constraints=None, probability_space=False):
-        constraints = constraints or {}
-        return self.model.inv_query(y, constraints, probability_space)
-
-    @ensure_model_is_fresh
-    def predict(self, x, probability_space=False):
-        return self.model.predict(x=x, probability_space=probability_space)
-
-    @ensure_model_is_fresh
-    def get_jnd(self, *args, **kwargs):
-        return self.model.get_jnd(*args, **kwargs)
-
-    @ensure_model_is_fresh
-    def sample(self, x, num_samples=None):
-        return self.model.sample(x, num_samples=num_samples)
+    @property
+    def config(self):
+        if self.strat_id == -1:
+            return None
+        else:
+            return self._configs[self.strat_id]
 
-    def finish(self):
-        self.is_finished = True
+    @config.setter
+    def config(self, s):
+        self._configs.append(s)
 
     @property
-    def finished(self):
-        if self.is_finished:
-            return True
-
-        if self.run_indefinitely:
-            return False
-
-        if hasattr(self.generator, "finished"):  # defer to generator if possible
-            return self.generator.finished
-
-        if self.y is None:  # always need some data before switching strats
-            return False
-
-        if self.max_asks is not None and self._count >= self.max_asks:
-            return True
-
-        if "binary" in self.outcome_types:
-            n_yes_trials = (self.y == 1).sum()
-            n_no_trials = (self.y == 0).sum()
-            sufficient_outcomes = (
-                n_yes_trials >= self.min_total_outcome_occurrences
-                and n_no_trials >= self.min_total_outcome_occurrences
-            )
+    def parnames(self):
+        if self.strat_id == -1:
+            return []
         else:
-            sufficient_outcomes = True
+            return self._parnames[self.strat_id]
 
-        if self.min_post_range is not None:
-            fmean, _ = self.model.predict(self.eval_grid, probability_space=True)
-            meets_post_range = (fmean.max() - fmean.min()) >= self.min_post_range
-        else:
-            meets_post_range = True
-        finished = (
-            self._count >= self.min_asks
-            and self.n >= self.min_total_tells
-            and sufficient_outcomes
-            and meets_post_range
-        )
-        return finished
+    @parnames.setter
+    def parnames(self, s):
+        self._parnames.append(s)
 
     @property
-    def can_fit(self):
-        return self.has_model and self.x is not None and self.y is not None
+    def n_strats(self):
+        return len(self._strats)
 
     @property
-    def n_trials(self):
-        warnings.warn(
-            "'n_trials' is deprecated and will be removed in a future release. Specify 'min_asks' instead.",
-            DeprecationWarning,
-        )
-        return self.min_asks
+    def can_pregen_ask(self):
+        return self.strat is not None and self.enable_pregen
 
-    def add_data(self, x, y):
-        self.x, self.y, self.n = self.normalize_inputs(x, y)
-        self._model_is_fresh = False
-
-    def fit(self):
-        if self.can_fit:
-            if self.keep_most_recent is not None:
-                try:
-                    self.model.fit(
-                        self.x[-self.keep_most_recent :],
-                        self.y[-self.keep_most_recent :],
-                    )
-                except (ModelFittingError):
-                    logger.warning(
-                        "Failed to fit model! Predictions may not be accurate!"
-                    )
-            else:
-                try:
-                    self.model.fit(self.x, self.y)
-                except (ModelFittingError):
-                    logger.warning(
-                        "Failed to fit model! Predictions may not be accurate!"
-                    )
-        else:
-            warnings.warn("Cannot fit: no model has been initialized!", RuntimeWarning)
-
-    def update(self):
-        if self.can_fit:
-            if self.keep_most_recent is not None:
-                try:
-                    self.model.update(
-                        self.x[-self.keep_most_recent :],
-                        self.y[-self.keep_most_recent :],
-                    )
-                except (ModelFittingError):
-                    logger.warning(
-                        "Failed to fit model! Predictions may not be accurate!"
-                    )
+    def _tensor_to_config(self, next_x):
+        config = {}
+        for name, val in zip(self.parnames, next_x):
+            if val.dim() == 0:
+                config[name] = [float(val)]
             else:
-                try:
-                    self.model.update(self.x, self.y)
-                except (ModelFittingError):
-                    logger.warning(
-                        "Failed to fit model! Predictions may not be accurate!"
-                    )
-        else:
-            warnings.warn("Cannot fit: no model has been initialized!", RuntimeWarning)
-
-    @classmethod
-    def from_config(cls, config: Config, name: str):
-        lb = config.gettensor(name, "lb")
-        ub = config.gettensor(name, "ub")
-        dim = config.getint(name, "dim", fallback=None)
-
-        stimuli_per_trial = config.getint(name, "stimuli_per_trial", fallback=1)
-        outcome_types = config.getlist(name, "outcome_types", element_type=str)
-
-        gen_cls = config.getobj(name, "generator", fallback=SobolGenerator)
-        generator = gen_cls.from_config(config)
-
-        model_cls = config.getobj(name, "model", fallback=None)
-        if model_cls is not None:
-            model = model_cls.from_config(config)
-        else:
-            model = None
-
-        acqf_cls = config.getobj(name, "acqf", fallback=None)
-        if acqf_cls is not None and hasattr(generator, "acqf"):
-            if generator.acqf is None:
-                generator.acqf = acqf_cls
-                generator.acqf_kwargs = generator._get_acqf_options(acqf_cls, config)
-
-        min_asks = config.getint(name, "min_asks", fallback=0)
-        min_total_tells = config.getint(name, "min_total_tells", fallback=0)
-
-        refit_every = config.getint(name, "refit_every", fallback=1)
-
-        if model is not None and not generator._requires_model:
-            if refit_every < min_asks:
-                warnings.warn(
-                    f"Strategy '{name}' has refit_every < min_asks even though its generator does not require a model. Consider making refit_every = min_asks to speed up point generation.",
-                    UserWarning,
-                )
-        keep_most_recent = config.getint(name, "keep_most_recent", fallback=None)
-
-        min_total_outcome_occurrences = config.getint(
-            name,
-            "min_total_outcome_occurrences",
-            fallback=1 if "binary" in outcome_types else 0,
-        )
-        min_post_range = config.getfloat(name, "min_post_range", fallback=None)
-        keep_most_recent = config.getint(name, "keep_most_recent", fallback=None)
-
-        n_trials = config.getint(name, "n_trials", fallback=None)
-        if n_trials is not None:
-            warnings.warn(
-                "'n_trials' is deprecated and will be removed in a future release. Specify 'min_asks' instead.",
-                DeprecationWarning,
-            )
-            min_asks = n_trials
-
-        return cls(
-            lb=lb,
-            ub=ub,
-            stimuli_per_trial=stimuli_per_trial,
-            outcome_types=outcome_types,
-            dim=dim,
-            model=model,
-            generator=generator,
-            min_asks=min_asks,
-            refit_every=refit_every,
-            min_total_outcome_occurrences=min_total_outcome_occurrences,
-            min_post_range=min_post_range,
-            keep_most_recent=keep_most_recent,
-            min_total_tells=min_total_tells,
-            name=name,
-        )
-
+                config[name] = np.array(val)
+        return config
 
-class SequentialStrategy(object):
-    """Runs a sequence of strategies defined by its config
+    def _config_to_tensor(self, config):
+        unpacked = [config[name] for name in self.parnames]
 
-    All getter methods defer to the current strat
+        # handle config elements being either scalars or length-1 lists
+        if isinstance(unpacked[0], list):
+            x = torch.tensor(np.stack(unpacked, axis=0)).squeeze(-1)
+        else:
+            x = torch.tensor(np.stack(unpacked))
+        return x
 
-    Args:
-        strat_list (list[Strategy]): TODO make this nicely typed / doc'd
-    """
-
-    def __init__(self, strat_list: List[Strategy]):
-        self.strat_list = strat_list
-        self._strat_idx = 0
-        self._suggest_count = 0
+    def __getstate__(self):
+        # nuke the socket since it's not pickleble
+        state = self.__dict__.copy()
+        del state["socket"]
+        del state["db"]
+        return state
+
+    def write_strats(self, termination_type):
+        if self._db_master_record is not None and self.strat is not None:
+            logger.info(f"Dumping strats to DB due to {termination_type}.")
+            for strat in self._strats:
+                buffer = io.BytesIO()
+                torch.save(strat, buffer, pickle_module=dill)
+                buffer.seek(0)
+                self.db.record_strat(master_table=self._db_master_record, strat=buffer)
+
+    def generate_debug_info(self, exception_type, dumptype):
+        fname = get_next_filename(".", dumptype, "pkl")
+        logger.exception(f"Got {exception_type}, exiting! Server dump in {fname}")
+        dill.dump(self, open(fname, "wb"))
+
+    def handle_request(self, request):
+        if "type" not in request.keys():
+            raise RuntimeError(f"Request {request} contains no request type!")
+        else:
+            type = request["type"]
+            if type in MESSAGE_MAP.keys():
+                logger.info(f"Received msg [{type}]")
+                ret_val = MESSAGE_MAP[type](self, request)
+                return ret_val
 
-    @property
-    def _strat(self):
-        return self.strat_list[self._strat_idx]
+            else:
+                exception_message = (
+                    f"unknown type: {type}. Allowed types [{MESSAGE_MAP.keys()}]"
+                )
 
-    def __getattr__(self, name: str):
-        # return current strategy's attr if it's not a container attr
-        if "strat_list" not in vars(self):
-            raise AttributeError("Have no strategies in container, what happened?")
-        return getattr(self._strat, name)
+                raise RuntimeError(exception_message)
 
-    def _make_next_strat(self):
-        if (self._strat_idx + 1) >= len(self.strat_list):
-            warnings.warn(
-                "Ran out of generators, staying on final generator!", RuntimeWarning
-            )
-            return
+    def replay(self, uuid_to_replay, skip_computations=False):
+        return replay(self, uuid_to_replay, skip_computations)
 
-        # populate new model with final data from last model
-        assert (
-            self.x is not None and self.y is not None
-        ), "Cannot initialize next strategy; no data has been given!"
-        self.strat_list[self._strat_idx + 1].add_data(self.x, self.y)
-
-        self._suggest_count = 0
-        self._strat_idx = self._strat_idx + 1
-
-    def gen(self, num_points: int = 1, **kwargs):
-        if self._strat.finished:
-            self._make_next_strat()
-        self._suggest_count = self._suggest_count + num_points
-        return self._strat.gen(num_points=num_points, **kwargs)
+    def get_strats_from_replay(self, uuid_of_replay=None, force_replay=False):
+        return get_strats_from_replay(self, uuid_of_replay, force_replay)
 
-    def finish(self):
-        self._strat.finish()
-
-    @property
-    def finished(self):
-        return self._strat_idx == (len(self.strat_list) - 1) and self._strat.finished
+    def get_strat_from_replay(self, uuid_of_replay=None, strat_id=-1):
+        return get_strat_from_replay(self, uuid_of_replay, strat_id)
+
+    def get_dataframe_from_replay(self, uuid_of_replay=None, force_replay=False):
+        return get_dataframe_from_replay(self, uuid_of_replay, force_replay)
+
+
+#! THIS IS WHAT START THE SERVER
+def startServerAndRun(
+    server_class, socket=None, database_path=None, config_path=None, uuid_of_replay=None
+):
+    server = server_class(socket=socket, database_path=database_path)
+    try:
+        if config_path is not None:
+            with open(config_path) as f:
+                config_str = f.read()
+            configure(server, config_str=config_str)
+
+        if socket is not None:
+            if uuid_of_replay is not None:
+                server.replay(uuid_of_replay, skip_computations=True)
+                server._db_master_record = server.db.get_master_record(uuid_of_replay)
+            server.serve()
+        else:
+            if config_path is not None:
+                logger.info(
+                    "You have passed in a config path but this is a replay. If there's a config in the database it will be used instead of the passed in config path."
+                )
+            server.replay(uuid_of_replay)
+    except KeyboardInterrupt:
+        exception_type = "CTRL+C"
+        dump_type = "dump"
+        server.write_strats(exception_type)
+        server.generate_debug_info(exception_type, dump_type)
+    except RuntimeError as e:
+        exception_type = "RuntimeError"
+        dump_type = "crashdump"
+        server.write_strats(exception_type)
+        server.generate_debug_info(exception_type, dump_type)
+        raise RuntimeError(e)
+
+
+def parse_argument():
+    parser = argparse.ArgumentParser(description="AEPsych Server!")
+    parser.add_argument(
+        "--port", metavar="N", type=int, default=5555, help="port to serve on"
+    )
+    parser.add_argument(
+        "--socket_type",
+        choices=["zmq", "pysocket"],
+        default="pysocket",
+        help="method to serve over",
+    )
+    parser.add_argument(
+        "--ip",
+        metavar="M",
+        type=str,
+        default="0.0.0.0",
+        help="ip to bind",
+    )
+
+    parser.add_argument(
+        "-s",
+        "--stratconfig",
+        help="Location of ini config file for strat",
+        type=str,
+    )
+
+    parser.add_argument(
+        "--logs",
+        type=str,
+        help="The logs path to use if not the default (./logs).",
+        default="logs",
+    )
+
+    parser.add_argument(
+        "-d",
+        "--db",
+        type=str,
+        help="The database to use if not the default (./databases/default.db).",
+        default=None,
+    )
+    parser.add_argument(
+        "-r", "--replay", type=str, help="UUID of the experiment to replay."
+    )
+
+    parser.add_argument(
+        "-m", "--resume", action="store_true", help="Resume server after replay."
+    )
+
+    args = parser.parse_args()
+    return args
+
+
+def start_server(server_class, args):
+    logger.info("Starting the AEPsychServer")
+    try:
+        if "db" in args and args.db is not None:
+            database_path = args.db
+            if "replay" in args and args.replay is not None:
+                logger.info(f"Attempting to replay {args.replay}")
+                if args.resume is True:
+                    sock = createSocket(socket_type=args.socket_type, port=args.port)
+                    logger.info(f"Will resume {args.replay}")
+                else:
+                    sock = None
+                startServerAndRun(
+                    server_class,
+                    socket=sock,
+                    database_path=database_path,
+                    uuid_of_replay=args.replay,
+                    config_path=args.stratconfig,
+                )
+            else:
+                logger.info(f"Setting the database path {database_path}")
+                sock = createSocket(socket_type=args.socket_type, port=args.port)
+                startServerAndRun(
+                    server_class,
+                    database_path=database_path,
+                    socket=sock,
+                    config_path=args.stratconfig,
+                )
+        else:
+            sock = createSocket(socket_type=args.socket_type, port=args.port)
+            startServerAndRun(server_class, socket=sock, config_path=args.stratconfig)
 
-    def add_data(self, x, y):
-        self._strat.add_data(x, y)
+    except (KeyboardInterrupt, SystemExit):
+        logger.exception("Got Ctrl+C, exiting!")
+        sys.exit()
+    except RuntimeError as e:
+        fname = get_next_filename(".", "dump", "pkl")
+        logger.exception(f"CRASHING!! dump in {fname}")
+        raise RuntimeError(e)
+
+
+def main(server_class=AEPsychServer):
+    args = parse_argument()
+    if args.logs:
+        # overide logger path
+        log_path = args.logs
+        logger = utils_logging.getLogger(logging.DEBUG, log_path)
+    logger.info(f"Saving logs to path: {log_path}")
+    start_server(server_class, args)
 
-    @classmethod
-    def from_config(cls, config: Config):
-        strat_names = config.getlist("common", "strategy_names", element_type=str)
-
-        # ensure strat_names are unique
-        assert len(strat_names) == len(
-            set(strat_names)
-        ), f"Strategy names {strat_names} are not all unique!"
-
-        strats = []
-        for name in strat_names:
-            strat = Strategy.from_config(config, str(name))
-            strats.append(strat)
 
-        return cls(strat_list=strats)
+if __name__ == "__main__":
+    main(AEPsychServer)
```

### Comparing `aepsych-0.3.0/aepsych/utils_logging.py` & `aepsych-0.4.0/aepsych/utils_logging.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/aepsych.egg-info/PKG-INFO` & `aepsych-0.4.0/aepsych.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepsych
-Version: 0.3.0
+Version: 0.4.0
 Summary: Adaptive experimetation for psychophysics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AEPsych
```

### Comparing `aepsych-0.3.0/tests/acquisition/test_lse.py` & `aepsych-0.4.0/tests/acquisition/test_lse.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/acquisition/test_mi.py` & `aepsych-0.4.0/tests/acquisition/test_mi.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/acquisition/test_monotonic.py` & `aepsych-0.4.0/tests/acquisition/test_monotonic.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/acquisition/test_objective.py` & `aepsych-0.4.0/tests/acquisition/test_objective.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/acquisition/test_rejection_sampler.py` & `aepsych-0.4.0/tests/acquisition/test_rejection_sampler.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/common.py` & `aepsych-0.4.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/generators/test_epsilon_greedy_generator.py` & `aepsych-0.4.0/tests/generators/test_epsilon_greedy_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/generators/test_manual_generator.py` & `aepsych-0.4.0/tests/generators/test_manual_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/generators/test_random_generator.py` & `aepsych-0.4.0/tests/generators/test_random_generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 # LICENSE file in the root directory of this source tree.
 
 import unittest
 
 import numpy as np
 import numpy.testing as npt
 from aepsych.config import Config
-from aepsych.generators import RandomGenerator
+from aepsych.generators import AxRandomGenerator, RandomGenerator
+from ax.modelbridge import Models
 
 
 class TestRandomGenerator(unittest.TestCase):
     def test_randomgen_single(self):
         # test that RandomGenerator doesn't mess with shapes
         n = 100
         rand = np.zeros((n, 3))
@@ -35,27 +36,52 @@
         # test that RandomGenerator doesn't mess with shapes
         n = 100
         mod = RandomGenerator(lb=[1, 2, 3], ub=[2, 3, 4], dim=3)
 
         rand = mod.gen(n)
 
         # check that bounds are right
-        self.assertTrue(np.all(rand[:, 0] > 1))
-        self.assertTrue(np.all(rand[:, 1] > 2))
-        self.assertTrue(np.all(rand[:, 2] > 3))
-        self.assertTrue(np.all(rand[:, 0] < 2))
-        self.assertTrue(np.all(rand[:, 1] < 3))
-        self.assertTrue(np.all(rand[:, 2] < 4))
+        self.assertTrue((rand[:, 0] > 1).all())
+        self.assertTrue((rand[:, 1] > 2).all())
+        self.assertTrue((rand[:, 2] > 3).all())
+        self.assertTrue((rand[:, 0] < 2).all())
+        self.assertTrue((rand[:, 1] < 3).all())
+        self.assertTrue((rand[:, 2] < 4).all())
 
     def test_randomgen_config(self):
         lb = [-1, 0]
         ub = [1, 2]
         config_str = f"""
         [common]
         lb = {lb}
         ub = {ub}
         """
         config = Config(config_str=config_str)
         gen = RandomGenerator.from_config(config)
         npt.assert_equal(gen.lb.numpy(), np.array(lb))
         npt.assert_equal(gen.ub.numpy(), np.array(ub))
         self.assertEqual(gen.dim, len(lb))
+
+    def test_axrandom_config(self):
+        config_str = """
+                [common]
+                parnames = [par1, par2]
+                lb = [-1, 0]
+                ub = [1, 2]
+                outcome_types = [continuous]
+                strategy_names = [init]
+
+                [init]
+                generator = RandomGenerator
+                [RandomGenerator]
+                seed=231
+                deduplicate=True
+                """
+        config = Config(config_str=config_str)
+        gen = AxRandomGenerator.from_config(config, name="init")
+        self.assertEqual(gen.model, Models.UNIFORM)
+        self.assertEqual(gen.model_kwargs["seed"], 231)
+        self.assertTrue(gen.model_kwargs["deduplicate"])
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `aepsych-0.3.0/tests/generators/test_sobol_generator.py` & `aepsych-0.4.0/tests/generators/test_sobol_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 import unittest
 
 import numpy as np
 import numpy.testing as npt
 import torch
 from aepsych.config import Config
-from aepsych.generators import SobolGenerator
+from aepsych.generators import AxSobolGenerator, SobolGenerator
 from aepsych.utils import make_scaled_sobol
+from ax.modelbridge import Models
 
 
 class TestSobolGenerator(unittest.TestCase):
     def test_batchsobol(self):
         mod = SobolGenerator(lb=[1, 2, 3], ub=[2, 3, 4], dim=3, seed=12345)
         acq1 = mod.gen(num_points=2)
         self.assertEqual(acq1.shape, (2, 3))
@@ -71,7 +72,34 @@
                 generator = SobolGenerator(
                     lb=np.arange(dim).tolist(),
                     ub=(1 + np.arange(dim)).tolist(),
                     stimuli_per_trial=2,
                 )
                 shape_out = (nsamp, dim, 2)
                 self.assertEqual(generator.gen(nsamp).shape, shape_out)
+
+    def test_axsobol_config(self):
+        config_str = """
+                [common]
+                parnames = [par1]
+                lb = [0]
+                ub = [1]
+                stimuli_per_trial = 1
+                outcome_types = [continuous]
+                strategy_names = [init]
+
+                [init]
+                generator = SobolGenerator
+
+                [SobolGenerator]
+                seed=12345
+                scramble=False
+                """
+        config = Config(config_str=config_str)
+        gen = AxSobolGenerator.from_config(config, name="init")
+        self.assertEqual(gen.model, Models.SOBOL)
+        self.assertEqual(gen.model_kwargs["seed"], 12345)
+        self.assertFalse(gen.model_kwargs["scramble"])
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `aepsych-0.3.0/tests/models/test_derivative_gp.py` & `aepsych-0.4.0/tests/models/test_derivative_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/models/test_gp_classification.py` & `aepsych-0.4.0/tests/models/test_gp_classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import torch
 
 # run on single threads to keep us from deadlocking weirdly in CI
 if "CI" in os.environ or "SANDCASTLE" in os.environ:
     torch.set_num_threads(1)
 
+from functools import partial
 from unittest.mock import MagicMock
 
 import numpy as np
 import numpy.testing as npt
 from aepsych.acquisition import MCLevelSetEstimation
 from aepsych.config import Config
 from aepsych.generators import OptimizeAcqfGenerator, SobolGenerator
@@ -27,15 +28,14 @@
 from botorch.optim.fit import fit_gpytorch_mll_torch
 from botorch.optim.stopping import ExpMAStoppingCriterion
 from botorch.posteriors import GPyTorchPosterior
 from gpytorch.distributions import MultivariateNormal
 from scipy.stats import bernoulli, norm, pearsonr
 from sklearn.datasets import make_classification
 from torch.distributions import Normal
-from functools import partial
 from torch.optim import Adam
 
 from ..common import cdf_new_novel_det, f_1d, f_2d
 
 
 class GPClassificationSmoketest(unittest.TestCase):
     """
@@ -64,28 +64,28 @@
         model = GPClassificationModel(
             torch.Tensor([-3]), torch.Tensor([3]), inducing_size=10
         )
 
         model.fit(X[:50], y[:50])
 
         # pspace
-        pm, _ = model.predict(X[:50], probability_space=True)
+        pm, _ = model.predict_probability(X[:50])
         pred = (pm > 0.5).numpy()
         npt.assert_allclose(pred, y[:50])
 
         # fspace
         pm, _ = model.predict(X[:50], probability_space=False)
         pred = (pm > 0).numpy()
         npt.assert_allclose(pred, y[:50])
 
         # smoke test update
         model.update(X, y)
 
         # pspace
-        pm, _ = model.predict(X, probability_space=True)
+        pm, _ = model.predict_probability(X)
         pred = (pm > 0.5).numpy()
         npt.assert_allclose(pred, y)
 
         # fspace
         pm, _ = model.predict(X, probability_space=False)
         pred = (pm > 0).numpy()
         npt.assert_allclose(pred, y)
@@ -99,37 +99,40 @@
             torch.Tensor([-3]), torch.Tensor([3]), inducing_size=10
         )
 
         model.fit(
             X[:50],
             y[:50],
             optimizer=fit_gpytorch_mll_torch,
-            optimizer_kwargs={"stopping_criterion":ExpMAStoppingCriterion(maxiter=30),'optimizer':partial(Adam, lr=0.05)}
+            optimizer_kwargs={
+                "stopping_criterion": ExpMAStoppingCriterion(maxiter=30),
+                "optimizer": partial(Adam, lr=0.05),
+            },
         )
 
         # pspace
-        pm, _ = model.predict(X[:50], probability_space=True)
+        pm, _ = model.predict_probability(X[:50])
         pred = (pm > 0.5).numpy()
         npt.assert_allclose(pred, y[:50])
 
         # fspace
         pm, _ = model.predict(X[:50], probability_space=False)
         pred = (pm > 0).numpy()
         npt.assert_allclose(pred, y[:50])
 
         # smoke test update
         model.update(
             X,
             y,
             optimizer=fit_gpytorch_mll_torch,
-            optimizer_kwargs={"stopping_criterion":ExpMAStoppingCriterion(maxiter=30)}
+            optimizer_kwargs={"stopping_criterion": ExpMAStoppingCriterion(maxiter=30)},
         )
 
         # pspace
-        pm, _ = model.predict(X, probability_space=True)
+        pm, _ = model.predict_probability(X)
         pred = (pm > 0.5).numpy()
         npt.assert_allclose(pred, y)
 
         # fspace
         pm, _ = model.predict(X, probability_space=False)
         pred = (pm > 0).numpy()
         npt.assert_allclose(pred, y)
@@ -154,28 +157,28 @@
         ub = [3000, 0.003]
 
         model = GPClassificationModel(lb=lb, ub=ub, inducing_size=20)
 
         model.fit(X[:50], y[:50])
 
         # pspace
-        pm, _ = model.predict(X[:50], probability_space=True)
+        pm, _ = model.predict_probability(X[:50])
         pred = (pm > 0.5).numpy()
         npt.assert_allclose(pred, y[:50])
 
         # fspace
         pm, _ = model.predict(X[:50], probability_space=False)
         pred = (pm > 0).numpy()
         npt.assert_allclose(pred, y[:50])
 
         # smoke test update
         model.update(X, y)
 
         # pspace
-        pm, _ = model.predict(X, probability_space=True)
+        pm, _ = model.predict_probability(X)
         pred = (pm > 0.5).numpy()
         npt.assert_allclose(pred, y)
 
         # fspace
         pm, _ = model.predict(X, probability_space=False)
         pred = (pm > 0).numpy()
         npt.assert_allclose(pred, y)
@@ -243,15 +246,15 @@
         """
         X, y = self.X, self.y
         model = GPClassificationModel(
             torch.Tensor([-3]), torch.Tensor([3]), inducing_size=10
         )
         model.fit(X, y)
 
-        pmean_analytic, pvar_analytic = model.predict(X, probability_space=True)
+        pmean_analytic, pvar_analytic = model.predict_probability(X)
 
         fsamps = model.sample(X, 150000)
         psamps = norm.cdf(fsamps)
         pmean_samp = psamps.mean(0)
         pvar_samp = psamps.var(0)
         # TODO these tolerances are a bit loose, verify this is right.
         self.assertTrue(np.allclose(pmean_analytic, pmean_samp, atol=0.001))
```

### Comparing `aepsych-0.3.0/tests/models/test_gp_regression.py` & `aepsych-0.4.0/tests/models/test_gp_regression.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 import numpy as np
 import numpy.testing as npt
 import torch
 from aepsych.server import AEPsychServer
 from gpytorch.likelihoods import GaussianLikelihood
 
+from aepsych.server.message_handlers.handle_ask import ask
+from aepsych.server.message_handlers.handle_tell import tell
+from aepsych.server.message_handlers.handle_setup import configure
+
 # run on single threads to keep us from deadlocking weirdly in CI
 if "CI" in os.environ or "SANDCASTLE" in os.environ:
     torch.set_num_threads(1)
 
 
 class GPRegressionTest(unittest.TestCase):
     def f(self, x):
@@ -54,20 +58,20 @@
             acqf = qNoisyExpectedImprovement
 
             [GPRegressionModel]
             likelihood = GaussianLikelihood
             max_fit_time = 1
         """
         self.server = AEPsychServer(database_path=dbname)
-        self.server.configure(config_str=config)
+        configure(self.server, config_str=config)
 
         while not self.server.strat.finished:
-            trial_params = self.server.ask()
+            trial_params = ask(self.server)
             outcome = self.simulate_response(trial_params)
-            self.server.tell(outcome, trial_params)
+            tell(self.server, outcome, trial_params)
 
     def tearDown(self):
         self.server.db.delete_db()
 
     def test_extremum(self):
         tol = 0.2  # don't need to be super precise because it's small data
         fmax, argmax = self.server.strat.get_max()
```

### Comparing `aepsych-0.3.0/tests/models/test_monotonic_projection_gp.py` & `aepsych-0.4.0/tests/models/test_monotonic_projection_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/models/test_monotonic_rejection_gp.py` & `aepsych-0.4.0/tests/models/test_monotonic_rejection_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/models/test_pairwise_probit.py` & `aepsych-0.4.0/tests/models/test_pairwise_probit.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 import numpy.testing as npt
 import torch
 from aepsych import server, utils_logging
 from aepsych.acquisition.objective import ProbitObjective
 from aepsych.config import Config
 from aepsych.generators import OptimizeAcqfGenerator, SobolGenerator
 from aepsych.models import PairwiseProbitModel
+from aepsych.server.message_handlers.handle_ask import ask
+from aepsych.server.message_handlers.handle_setup import configure
+from aepsych.server.message_handlers.handle_tell import tell
 from aepsych.strategy import SequentialStrategy, Strategy
 from botorch.acquisition import qUpperConfidenceBound
 from botorch.acquisition.active_learning import PairwiseMCPosteriorVariance
 from scipy.stats import bernoulli, norm, pearsonr
 
 from ..common import f_1d, f_2d, f_pairwise, new_novel_det
 
@@ -292,15 +295,14 @@
                 strat.model.predict(test_x[..., 0])[0]
                 - strat.model.predict(test_x[..., 1])[0]
             )
 
         self.assertTrue(pearsonr(fdiff_test_reref, ftrue_test)[0] >= 0.9)
 
     def test_2d_pairwise_probit(self):
-
         seed = 1
         torch.manual_seed(seed)
         np.random.seed(seed)
         n_init = 20
         n_opt = 1
         lb = np.r_[-1, -1]
         ub = np.r_[1, 1]
@@ -342,15 +344,14 @@
 
         zhat, _ = strat.predict(torch.Tensor(xy))
 
         # true min is at 0,0
         self.assertTrue(np.all(np.abs(xy[np.argmax(zhat.detach().numpy())]) < 0.2))
 
     def test_2d_pairwise_probit_pure_exploration(self):
-
         seed = 1
         torch.manual_seed(seed)
         np.random.seed(seed)
         n_init = 20
         n_opt = 1
         lb = np.r_[-1, -1]
         ub = np.r_[1, 1]
@@ -458,15 +459,14 @@
         self.s.cleanup()
 
         # cleanup the db
         if self.s.db is not None:
             self.s.db.delete_db()
 
     def test_1d_pairwise_server(self):
-
         seed = 123
         torch.manual_seed(seed)
         np.random.seed(seed)
         n_init = 50
         n_opt = 2
         config_str = f"""
             [common]
@@ -495,22 +495,23 @@
 
             [OptimizeAcqfGenerator]
             restarts = 10
             samps = 1000
             """
 
         server = self.s
-        server.configure(
+        configure(
+            server,
             config_str=config_str,
         )
 
         for _i in range(n_init + n_opt):
-            next_config = server.ask()
+            next_config = ask(server)
             next_y = bernoulli.rvs(f_pairwise(f_1d, next_config["x"], noise_scale=0.1))
-            server.tell(config=next_config, outcome=next_y)
+            tell(server, config=next_config, outcome=next_y)
 
         x = torch.linspace(-4, 4, 100)
         zhat, _ = server.strat.predict(x)
         self.assertTrue(np.abs(x[np.argmax(zhat.detach().numpy())]) < 0.5)
 
     def test_2d_pairwise_server(self):
         seed = 1
@@ -545,32 +546,32 @@
 
             [OptimizeAcqfGenerator]
             restarts = 10
             samps = 1000
             """
 
         server = self.s
-        server.configure(
+        configure(
+            server,
             config_str=config_str,
         )
         for _i in range(n_init + n_opt):
-            next_config = server.ask()
+            next_config = ask(server)
             next_pair = np.c_[next_config["x"], next_config["y"]].T
             next_y = bernoulli.rvs(f_pairwise(f_2d, next_pair, noise_scale=0.1))
-            server.tell(config=next_config, outcome=next_y)
+            tell(server, config=next_config, outcome=next_y)
 
         xy = np.mgrid[-1:1:30j, -1:1:30j].reshape(2, -1).T
 
         zhat, _ = server.strat.predict(torch.Tensor(xy))
 
         # true min is at 0,0
         self.assertTrue(np.all(np.abs(xy[np.argmax(zhat.detach().numpy())]) < 0.2))
 
     def test_serialization_1d(self):
-
         seed = 1
         torch.manual_seed(seed)
         np.random.seed(seed)
         n_init = 3
         n_opt = 1
         config_str = f"""
             [common]
@@ -599,20 +600,20 @@
 
             [OptimizeAcqfGenerator]
             restarts = 10
             samps = 1000
             """
 
         server = self.s
-        server.configure(config_str=config_str)
+        configure(server, config_str=config_str)
 
         for _i in range(n_init + n_opt):
-            next_config = server.ask()
+            next_config = ask(server)
             next_y = bernoulli.rvs(f_pairwise(f_1d, next_config["x"]))
-            server.tell(config=next_config, outcome=next_y)
+            tell(server, config=next_config, outcome=next_y)
 
         import dill
 
         # just make sure it works
         try:
             s = dill.dumps(server)
             server2 = dill.loads(s)
@@ -623,15 +624,14 @@
                 self.assertTrue(torch.equal(strat1.x, strat2.x))
                 self.assertTrue(torch.equal(strat1.y, strat2.y))
 
         except Exception:
             self.fail()
 
     def test_serialization_2d(self):
-
         seed = 1
         torch.manual_seed(seed)
         np.random.seed(seed)
         n_init = 3
         n_opt = 1
 
         config_str = f"""
@@ -662,21 +662,21 @@
             [PairwiseOptimizeAcqfGenerator]
             restarts = 10
             samps = 1000
             """
 
         server = self.s
 
-        server.configure(config_str=config_str)
+        configure(server, config_str=config_str)
 
         for _i in range(n_init + n_opt):
-            next_config = server.ask()
+            next_config = ask(server)
             next_pair = np.c_[next_config["x"], next_config["y"]].T
             next_y = bernoulli.rvs(f_pairwise(f_2d, next_pair))
-            server.tell(config=next_config, outcome=next_y)
+            tell(server, config=next_config, outcome=next_y)
 
         import dill
 
         # just make sure it works
         try:
             s = dill.dumps(server)
             server2 = dill.loads(s)
@@ -717,17 +717,17 @@
 
             [OptimizeAcqfGenerator]
             restarts = 10
             samps = 1000
             """
         server = self.s
 
-        server.configure(config_str=config_str)
+        configure(server, config_str=config_str)
 
-        conf = server.ask()
+        conf = ask(server)
 
         self.assertTrue(server._config_to_tensor(conf).shape == (1, 2))
 
         config_str = """
             [common]
             lb = [-1, -1]
             ub = [1, 1]
@@ -753,17 +753,17 @@
             objective = ProbitObjective
 
             [OptimizeAcqfGenerator]
             restarts = 10
             samps = 1000
             """
 
-        server.configure(config_str=config_str)
+        configure(server, config_str=config_str)
 
-        conf = server.ask()
+        conf = ask(server)
 
         self.assertTrue(server._config_to_tensor(conf).shape == (2, 2))
 
         config_str = """
             [common]
             lb = [-1, -1, -1]
             ub = [1, 1, 1]
@@ -789,16 +789,16 @@
             objective = ProbitObjective
 
             [OptimizeAcqfGenerator]
             restarts = 10
             samps = 1000
             """
 
-        server.configure(config_str=config_str)
+        configure(server, config_str=config_str)
 
-        conf = server.ask()
+        conf = ask(server)
 
         self.assertTrue(server._config_to_tensor(conf).shape == (3, 2))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aepsych-0.3.0/tests/models/test_utils.py` & `aepsych-0.4.0/tests/models/test_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import unittest
 
 import numpy as np
 import torch
+from sklearn.datasets import make_classification
+
 from aepsych.models import GPClassificationModel
 from aepsych.models.utils import select_inducing_points
-from sklearn.datasets import make_classification
 
 
 class UtilsTestCase(unittest.TestCase):
     def test_select_inducing_points(self):
         """Verify that when we have n_induc > data size, we use data as inducing,
         and otherwise we correctly select inducing points."""
         X, y = make_classification(
@@ -35,68 +36,68 @@
         model.set_train_data(X[:10, ...], y[:10])
 
         # (inducing point selection sorts the inputs so we sort X to verify)
         self.assertTrue(
             np.allclose(
                 select_inducing_points(
                     inducing_size=inducing_size,
-                    model=model,
+                    covar_module=model.covar_module,
                     X=model.train_inputs[0],
                     bounds=model.bounds,
                     method="auto",
                 ),
                 X[:10].sort(0).values,
             )
         )
 
         model.set_train_data(X, y)
 
         self.assertTrue(
             len(
                 select_inducing_points(
                     inducing_size=inducing_size,
-                    model=model,
+                    covar_module=model.covar_module,
                     X=model.train_inputs[0],
                     bounds=model.bounds,
                     method="auto",
                 )
             )
             <= 20
         )
 
         self.assertTrue(
             len(
                 select_inducing_points(
                     inducing_size=inducing_size,
-                    model=model,
+                    covar_module=model.covar_module,
                     X=model.train_inputs[0],
                     bounds=model.bounds,
                     method="pivoted_chol",
                 )
             )
             <= 20
         )
 
         self.assertEqual(
             len(
                 select_inducing_points(
                     inducing_size=inducing_size,
-                    model=model,
+                    covar_module=model.covar_module,
                     X=model.train_inputs[0],
                     bounds=model.bounds,
                     method="kmeans++",
                 )
             ),
             20,
         )
 
         with self.assertRaises(AssertionError):
             select_inducing_points(
                 inducing_size=inducing_size,
-                model=model,
+                covar_module=model.covar_module,
                 X=model.train_inputs[0],
                 bounds=model.bounds,
                 method="12345",
             )
 
 
 if __name__ == "__main__":
```

### Comparing `aepsych-0.3.0/tests/test_ThriftSocketWrapper.py` & `aepsych-0.4.0/tests/test_ThriftSocketWrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,25 +32,18 @@
         # cleanup the db
         if self.s.db is not None:
             self.s.db.delete_db()
 
     def test_serve(self):
         request = {"version": 0}
         self.s.socket.receive = MagicMock(return_value=request)
-        self.s.versioned_handler = MagicMock()
-        self.s.unversioned_handler = MagicMock()
+        self.s.handle_request = MagicMock()
+        self.s.handle_request = MagicMock()
         self.s.serve()
-        self.s.versioned_handler.assert_called_once_with(request)
-
-        request = {}
-        self.s.socket.receive = MagicMock(return_value=request)
-        self.s.versioned_handler = MagicMock()
-        self.s.unversioned_handler = MagicMock()
-        self.s.serve()
-        self.s.unversioned_handler.assert_called_once_with(request)
+        self.s.handle_request.assert_called_once_with(request)
 
     def test_receive(self):
         request = {"version": 0}
         self.s.socket.msg_queue.put(request, block=True)
         res = self.s.socket.receive()
         self.assertEqual(res, request)
```

### Comparing `aepsych-0.3.0/tests/test_bench_testfuns.py` & `aepsych-0.4.0/tests/test_bench_testfuns.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/test_benchmark.py` & `aepsych-0.4.0/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/test_config.py` & `aepsych-0.4.0/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,34 +7,38 @@
 
 import json
 import os
 import unittest
 import uuid
 
 import torch
-from aepsych.acquisition import MCLevelSetEstimation
+from aepsych.acquisition import EAVC, MCLevelSetEstimation
 from aepsych.acquisition.monotonic_rejection import MonotonicMCLSE
-from aepsych.acquisition.objective import ProbitObjective
+from aepsych.acquisition.objective import FloorGumbelObjective, ProbitObjective
 from aepsych.config import Config
 from aepsych.generators import (
     MonotonicRejectionGenerator,
     OptimizeAcqfGenerator,
     SobolGenerator,
 )
+from aepsych.likelihoods import BernoulliObjectiveLikelihood
 from aepsych.models import (
     GPClassificationModel,
+    HadamardSemiPModel,
     MonotonicRejectionGP,
     PairwiseProbitModel,
 )
 from aepsych.server import AEPsychServer
 from aepsych.strategy import SequentialStrategy, Strategy
 from aepsych.version import __version__
 from botorch.acquisition import qNoisyExpectedImprovement
 from botorch.acquisition.active_learning import PairwiseMCPosteriorVariance
 
+from aepsych.server.message_handlers.handle_setup import configure
+
 
 class ConfigTestCase(unittest.TestCase):
     def test_single_probit_config(self):
         config_str = """
         [common]
         lb = [0, 0]
         ub = [1, 1]
@@ -141,39 +145,30 @@
 
         self.assertTrue(isinstance(strat.strat_list[0].generator, SobolGenerator))
         self.assertTrue(strat.strat_list[0].model is None)
 
         self.assertTrue(
             isinstance(strat.strat_list[1].generator, OptimizeAcqfGenerator)
         )
-        self.assertTrue(strat.strat_list[1].generator.acqf is MCLevelSetEstimation)
+        self.assertTrue(strat.strat_list[1].generator.acqf is EAVC)
         self.assertTrue(
-            set(strat.strat_list[1].generator.acqf_kwargs.keys())
-            == {"beta", "target", "objective"}
+            set(strat.strat_list[1].generator.acqf_kwargs.keys()) == {"target"}
         )
         self.assertTrue(strat.strat_list[1].generator.acqf_kwargs["target"] == 0.75)
-        self.assertTrue(strat.strat_list[1].generator.acqf_kwargs["beta"] == 3.84)
-        self.assertTrue(
-            isinstance(
-                strat.strat_list[1].generator.acqf_kwargs["objective"],
-                ProbitObjective,
-            )
-        )
         self.assertTrue(strat.strat_list[1].generator.samps == 1000)
         self.assertTrue(strat.strat_list[0].min_asks == 10)
         self.assertTrue(strat.strat_list[0].stimuli_per_trial == 1)
         self.assertTrue(strat.strat_list[0].outcome_types == ["binary"])
         self.assertTrue(strat.strat_list[1].min_asks == 20)
         self.assertTrue(torch.all(strat.strat_list[0].lb == strat.strat_list[1].lb))
         self.assertTrue(torch.all(strat.strat_list[1].model.lb == torch.Tensor([0, 0])))
         self.assertTrue(torch.all(strat.strat_list[0].ub == strat.strat_list[1].ub))
         self.assertTrue(torch.all(strat.strat_list[1].model.ub == torch.Tensor([1, 1])))
 
     def test_nonmonotonic_optimization_config_file(self):
-
         config_file = "../configs/nonmonotonic_optimization_example.ini"
         config_file = os.path.join(os.path.dirname(__file__), config_file)
 
         config = Config()
         config.update(config_fnames=[config_file])
         strat = SequentialStrategy.from_config(config)
 
@@ -489,15 +484,15 @@
     def test_pairwise_al_config_file(self):
         # random datebase path name without dashes
         database_path = "./{}.db".format(str(uuid.uuid4().hex))
         server = AEPsychServer(database_path=database_path)
 
         config_file = "../configs/pairwise_al_example.ini"
         config_file = os.path.join(os.path.dirname(__file__), config_file)
-        server.configure(config_fnames=[config_file])
+        configure(server, config_fnames=[config_file])
         strat = server.strat
 
         self.assertTrue(isinstance(strat.strat_list[0].generator, SobolGenerator))
         self.assertTrue(strat.strat_list[0].model is None)
 
         self.assertTrue(
             isinstance(strat.strat_list[1].generator, OptimizeAcqfGenerator)
@@ -534,15 +529,15 @@
         # random datebase path name without dashes
         database_path = "./{}.db".format(str(uuid.uuid4().hex))
         server = AEPsychServer(database_path=database_path)
 
         config_file = "../configs/pairwise_opt_example.ini"
         config_file = os.path.join(os.path.dirname(__file__), config_file)
 
-        server.configure(config_fnames=[config_file])
+        configure(server, config_fnames=[config_file])
         strat = server.strat
 
         self.assertTrue(isinstance(strat.strat_list[0].generator, SobolGenerator))
         self.assertTrue(strat.strat_list[0].model is None)
 
         self.assertTrue(isinstance(strat.strat_list[1].model, PairwiseProbitModel))
         self.assertTrue(strat.strat_list[1].generator.acqf is qNoisyExpectedImprovement)
@@ -807,10 +802,65 @@
         # this should work
         SequentialStrategy.from_config(good_config)
 
         # this should fail
         with self.assertRaises(AssertionError):
             SequentialStrategy.from_config(bad_config)
 
+    def test_semip_config(self):
+        config_str = """
+            [common]
+            lb = [0, 0]
+            ub = [1, 1]
+            stimuli_per_trial = 1
+            outcome_types = [binary]
+            parnames = [par1, par2]
+            strategy_names = [init_strat, opt_strat]
+            acqf = MCLevelSetEstimation
+            model = HadamardSemiPModel
+
+            [init_strat]
+            min_asks = 10
+            generator = SobolGenerator
+            refit_every = 10
+
+            [opt_strat]
+            min_asks = 20
+            generator = OptimizeAcqfGenerator
+
+            [HadamardSemiPModel]
+            stim_dim = 1
+            inducing_size = 10
+            inducing_point_method = sobol
+            likelihood = BernoulliObjectiveLikelihood
+
+            [BernoulliObjectiveLikelihood]
+            objective = FloorGumbelObjective
+
+            [FloorGumbelObjective]
+            floor = 0.123
+
+            [OptimizeAcqfGenerator]
+            restarts = 10
+            samps = 1000
+            """
+
+        config = Config()
+        config.update(config_str=config_str)
+
+        strat = SequentialStrategy.from_config(config)
+        opt_strat = strat.strat_list[1]
+        model = opt_strat.model
+
+        self.assertTrue(isinstance(model, HadamardSemiPModel))
+        self.assertTrue(torch.all(model.lb == torch.Tensor([0, 0])))
+        self.assertTrue(torch.all(model.ub == torch.Tensor([1, 1])))
+        self.assertTrue(model.dim == 2)
+        self.assertTrue(model.inducing_size == 10)
+        self.assertTrue(model.stim_dim == 1)
+        self.assertTrue(model.inducing_point_method == "sobol")
+        self.assertTrue(isinstance(model.likelihood, BernoulliObjectiveLikelihood))
+        self.assertTrue(isinstance(model.likelihood.objective, FloorGumbelObjective))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aepsych-0.3.0/tests/test_db.py` & `aepsych-0.4.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/test_integration.py` & `aepsych-0.4.0/tests/test_integration.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,14 +42,86 @@
         [[0], [0]],
         [[-0.1], [0]],
         [[0], [0]],
         [[0], [0]],
     ],
 }
 
+multistim_config = """
+# Configuration for multi-stimulus experiment integration test
+
+[common]
+lb = [0, 0]
+ub = [1, 1]
+parnames = [x1, x2]
+stimuli_per_trial = 2
+outcome_types = [binary]
+strategy_names = [init_strat, opt_strat]
+
+[init_strat]
+min_asks = 3
+generator = SobolGenerator
+min_total_outcome_occurrences = 0
+
+[opt_strat]
+min_asks = 4
+generator = OptimizeAcqfGenerator
+acqf = qNoisyExpectedImprovement
+model = PairwiseProbitModel
+min_total_outcome_occurrences = 0
+
+[SobolGenerator]
+n_points = 2
+
+[PairwiseMCPosteriorVariance]
+objective = ProbitObjective
+
+[PairwiseProbitModel]
+inducing_size = 100
+mean_covar_factory = default_mean_covar_factory
+
+[OptimizeAcqfGenerator]
+restarts = 10
+samps = 1000
+
+[qNoisyExpectedImprovement]
+objective = ProbitObjective
+"""
+
+singlestim_config = """
+[common]
+lb = [0, 0]
+ub = [1, 1]
+parnames = [x1, x2]
+stimuli_per_trial = 1
+outcome_types = [binary]
+strategy_names = [init_strat, opt_strat]
+
+[init_strat]
+min_asks = 3
+generator = SobolGenerator
+min_total_outcome_occurrences = 0
+
+[opt_strat]
+min_asks = 4
+generator = OptimizeAcqfGenerator
+acqf = MCPosteriorVariance
+model = GPClassificationModel
+min_total_outcome_occurrences = 0
+
+[GPClassificationModel]
+inducing_size = 10
+mean_covar_factory = default_mean_covar_factory
+
+[SobolGenerator]
+n_points = 2
+"""
+
+test_configs = {"singleStimuli": singlestim_config, "multiStimuli": multistim_config}
+
 all_tests = list(product(params, outcomes))
 
 
 class IntegrationTestCase(unittest.TestCase):
     def setUp(self):
         # setup logger
         server.logger = utils_logging.getLogger(logging.DEBUG, "logs")
@@ -181,27 +253,26 @@
 
     @parameterized.expand(all_tests)
     def test_experiment(self, param_type, outcome_type):
         x1 = params[param_type]["x1"]
         x2 = params[param_type]["x2"]
         outcome = outcomes[outcome_type]
 
-        with open(f"tests/configs/{param_type}" + ".ini", "r") as f:
-            dummy_config = f.read()
+        dummy_config = test_configs[param_type]
 
         self.setup_request["message"]["config_str"] = dummy_config
 
-        self.s.versioned_handler(self.setup_request)
+        self.s.handle_request(self.setup_request)
 
         i = 0
         while not self.s.strat.finished:
-            self.s.unversioned_handler(self.ask_request)
+            self.s.handle_request(self.ask_request)
             self.get_tell(x1[i], x2[i], outcome[i])
             i = i + 1
-            self.s.unversioned_handler(self.tell_request)
+            self.s.handle_request(self.tell_request)
 
         # Experiment id
         exp_id = self.s.db.get_master_records()[0].experiment_id
 
         # Create table with experiment data
         self.s.generate_experiment_table(exp_id, return_df=True)
```

### Comparing `aepsych-0.3.0/tests/test_likelihoods.py` & `aepsych-0.4.0/tests/test_likelihoods.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+#!/usr/bin/env python3
+# Copyright (c) Facebook, Inc. and its affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
 import unittest
 
 import torch
 from aepsych.likelihoods import OrdinalLikelihood
 from gpytorch.test.base_likelihood_test_case import BaseLikelihoodTestCase
 
 emtpy_batch_shape = torch.Size([])
```

### Comparing `aepsych-0.3.0/tests/test_lookahead.py` & `aepsych-0.4.0/tests/test_lookahead.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.3.0/tests/test_mean_covar_factories.py` & `aepsych-0.4.0/tests/test_mean_covar_factories.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,15 @@
 )
 from aepsych.kernels.rbf_partial_grad import RBFKernelPartialObsGrad
 from aepsych.means.constant_partial_grad import ConstantMeanPartialObsGrad
 from scipy.stats import norm
 
 
 class TestFactories(unittest.TestCase):
-    def test_default_factory_1d(self):
-
-        conf = {"default_mean_covar_factory": {"lb": [0], "ub": [1]}}
-        config = Config(config_dict=conf)
-        meanfun, covarfun = default_mean_covar_factory(config)
+    def _test_mean_covar(self, meanfun, covarfun):
         self.assertTrue(covarfun.base_kernel.ard_num_dims == 1)
         self.assertTrue(meanfun.constant.requires_grad)
         self.assertTrue(isinstance(meanfun, gpytorch.means.ConstantMean))
         self.assertTrue(isinstance(covarfun, gpytorch.kernels.ScaleKernel))
         self.assertTrue(
             isinstance(
                 covarfun.base_kernel._priors["lengthscale_prior"][0],
@@ -40,14 +36,25 @@
             isinstance(
                 covarfun._priors["outputscale_prior"][0],
                 gpytorch.priors.SmoothedBoxPrior,
             )
         )
         self.assertTrue(isinstance(covarfun.base_kernel, gpytorch.kernels.RBFKernel))
 
+    def test_default_factory_1d_config(self):
+        config = Config(
+            config_dict={"default_mean_covar_factory": {"lb": [0], "ub": [1]}}
+        )
+        meanfun, covarfun = default_mean_covar_factory(config=config)
+        self._test_mean_covar(meanfun, covarfun)
+
+    def test_default_factory_1d_dim(self):
+        meanfun, covarfun = default_mean_covar_factory(dim=1)
+        self._test_mean_covar(meanfun, covarfun)
+
     def test_default_factory_args_1d(self):
 
         conf = {
             "default_mean_covar_factory": {
                 "lb": [0],
                 "ub": [1],
                 "fixed_mean": True,
@@ -106,14 +113,23 @@
             {"default_mean_covar_factory": {"lb": [0], "ub": [1], "fixed_mean": True}},
         ]
         for conf in bad_confs:
             with self.assertRaises(RuntimeError):
                 config = Config(conf)
                 _, __ = default_mean_covar_factory(config)
 
+        with self.assertRaises(AssertionError):
+            default_mean_covar_factory()
+
+        config = Config(
+            config_dict={"default_mean_covar_factory": {"lb": [0], "ub": [1]}}
+        )
+        with self.assertRaises(AssertionError):
+            default_mean_covar_factory(config=config, dim=2)
+
     def test_default_factory_2d(self):
         conf = {"default_mean_covar_factory": {"lb": [-2, 3], "ub": [1, 10]}}
         config = Config(config_dict=conf)
         meanfun, covarfun = default_mean_covar_factory(config)
         self.assertTrue(covarfun.base_kernel.ard_num_dims == 2)
         self.assertTrue(isinstance(meanfun, gpytorch.means.ConstantMean))
         self.assertTrue(isinstance(covarfun, gpytorch.kernels.ScaleKernel))
```

### Comparing `aepsych-0.3.0/tests/test_strategy.py` & `aepsych-0.4.0/tests/test_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 
 import unittest
 from unittest.mock import MagicMock
 
 import numpy as np
 import torch
 from aepsych.acquisition.monotonic_rejection import MonotonicMCLSE
+from aepsych.config import Config
 from aepsych.generators import MonotonicRejectionGenerator, SobolGenerator
 from aepsych.models.gp_classification import GPClassificationModel
 from aepsych.models.monotonic_rejection_gp import MonotonicRejectionGP
-from aepsych.strategy import SequentialStrategy, Strategy
+from aepsych.strategy import AEPsychStrategy, SequentialStrategy, Strategy
 
 
 class TestSequenceGenerators(unittest.TestCase):
     def setUp(self):
         seed = 1
         torch.manual_seed(seed)
         np.random.seed(seed)
@@ -330,9 +331,33 @@
                 generator=SobolGenerator(lb=[-1], ub=[1], stimuli_per_trial=2),
                 outcome_types=["binary", "extra"],
             )
         except AssertionError:
             self.fail("Strategy raised unexpected AssertionError on __init__!")
 
 
+class GenerationStrategyTestCase(unittest.TestCase):
+    def test_finish(self):
+        config_str = """
+        [common]
+        use_ax = True
+        stimuli_per_trial = 1
+        outcome_types = [binary]
+        parnames = [x]
+        lb = [0]
+        ub = [1]
+        strategy_names = [test_strat]
+
+        [test_strat]
+        generator = SobolGenerator
+        run_indefinitely = True
+        """
+        config = Config(config_str=config_str)
+        strat = AEPsychStrategy.from_config(config)
+
+        self.assertFalse(strat.finished)
+        strat.finish()
+        self.assertTrue(strat.finished)
+
+
 if __name__ == "__main__":
     unittest.main()
```

