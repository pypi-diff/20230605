# Comparing `tmp/RL_OM-0.1.1.tar.gz` & `tmp/RL_OM-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.1.1.tar", last modified: Sat Jun  3 18:14:17 2023, max compression
+gzip compressed data, was "RL_OM-0.1.2.tar", last modified: Mon Jun  5 07:04:23 2023, max compression
```

## Comparing `RL_OM-0.1.1.tar` & `RL_OM-0.1.2.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.791353 RL_OM-0.1.1/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.1.1/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.1.1/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-03 18:14:17.791202 RL_OM-0.1.1/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.1.1/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.783570 RL_OM-0.1.1/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   131239 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.785835 RL_OM-0.1.1/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.786090 RL_OM-0.1.1/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     5975 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/benchmark_agents/eoq.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.786625 RL_OM-0.1.1/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.787040 RL_OM-0.1.1/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1141 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.787961 RL_OM-0.1.1/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.789135 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.789989 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     5053 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5269 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16656 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     5082 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.790714 RL_OM-0.1.1/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     4407 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    11345 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.791001 RL_OM-0.1.1/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:03.000000 RL_OM-0.1.1/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     7822 2023-06-03 18:14:02.000000 RL_OM-0.1.1/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-03 18:14:17.785680 RL_OM-0.1.1/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.1.1/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-06-03 18:14:17.000000 RL_OM-0.1.1/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      989 2023-06-03 18:13:53.000000 RL_OM-0.1.1/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-06-03 18:14:17.791396 RL_OM-0.1.1/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.1.1/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.099292 RL_OM-0.1.2/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.1.2/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.1.2/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-05 07:04:23.099158 RL_OM-0.1.2/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.1.2/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.093088 RL_OM-0.1.2/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   135627 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.094201 RL_OM-0.1.2/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.094573 RL_OM-0.1.2/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6015 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/benchmark_agents/eoq.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10435 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/benchmark_agents/qr.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.095091 RL_OM-0.1.2/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.095476 RL_OM-0.1.2/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1141 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.096329 RL_OM-0.1.2/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.097197 RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.098067 RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16656 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5082 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.098714 RL_OM-0.1.2/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4407 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    11346 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.098961 RL_OM-0.1.2/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     7822 2023-06-05 07:00:55.000000 RL_OM-0.1.2/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-05 07:04:23.094068 RL_OM-0.1.2/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-05 07:04:23.000000 RL_OM-0.1.2/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     1824 2023-06-05 07:04:23.000000 RL_OM-0.1.2/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-06-05 07:04:23.000000 RL_OM-0.1.2/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2023-06-05 07:04:23.000000 RL_OM-0.1.2/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.1.2/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2023-06-05 07:04:23.000000 RL_OM-0.1.2/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-06-05 07:04:23.000000 RL_OM-0.1.2/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2023-06-05 07:00:51.000000 RL_OM-0.1.2/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-06-05 07:04:23.099334 RL_OM-0.1.2/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.1.2/setup.py
```

### Comparing `RL_OM-0.1.1/LICENSE` & `RL_OM-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/PKG-INFO` & `RL_OM-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.1.1
+Version: 0.1.2
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.1.1/RL_OM/_modidx.py` & `RL_OM-0.1.2/RL_OM/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,42 @@
                                                                                                              'RL_OM/agents/benchmark_agents/eoq.py'),
                                                    'RL_OM.agents.benchmark_agents.eoq.EOQPolicy.draw_action': ( 'agents/benchmark_agents/eoq.html#eoqpolicy.draw_action',
                                                                                                                 'RL_OM/agents/benchmark_agents/eoq.py'),
                                                    'RL_OM.agents.benchmark_agents.eoq.EOQPolicy.reset': ( 'agents/benchmark_agents/eoq.html#eoqpolicy.reset',
                                                                                                           'RL_OM/agents/benchmark_agents/eoq.py'),
                                                    'RL_OM.agents.benchmark_agents.eoq.EOQPolicy.set_q_star': ( 'agents/benchmark_agents/eoq.html#eoqpolicy.set_q_star',
                                                                                                                'RL_OM/agents/benchmark_agents/eoq.py')},
+            'RL_OM.agents.benchmark_agents.qr': { 'RL_OM.agents.benchmark_agents.qr.QRAgent': ( 'agents/benchmark_agents/qr.html#qragent',
+                                                                                                'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRAgent.__init__': ( 'agents/benchmark_agents/qr.html#qragent.__init__',
+                                                                                                         'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRAgent.fit': ( 'agents/benchmark_agents/qr.html#qragent.fit',
+                                                                                                    'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy': ( 'agents/benchmark_agents/qr.html#qrpolicy',
+                                                                                                 'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.__init__': ( 'agents/benchmark_agents/qr.html#qrpolicy.__init__',
+                                                                                                          'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.calculate_incremental_Q': ( 'agents/benchmark_agents/qr.html#qrpolicy.calculate_incremental_q',
+                                                                                                                         'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.calculate_incremental_R': ( 'agents/benchmark_agents/qr.html#qrpolicy.calculate_incremental_r',
+                                                                                                                         'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.calculate_initial_R': ( 'agents/benchmark_agents/qr.html#qrpolicy.calculate_initial_r',
+                                                                                                                     'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.draw_action': ( 'agents/benchmark_agents/qr.html#qrpolicy.draw_action',
+                                                                                                             'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.draw_action_train': ( 'agents/benchmark_agents/qr.html#qrpolicy.draw_action_train',
+                                                                                                                   'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.expected_stockouts': ( 'agents/benchmark_agents/qr.html#qrpolicy.expected_stockouts',
+                                                                                                                    'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.reset': ( 'agents/benchmark_agents/qr.html#qrpolicy.reset',
+                                                                                                       'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.run_simulation': ( 'agents/benchmark_agents/qr.html#qrpolicy.run_simulation',
+                                                                                                                'RL_OM/agents/benchmark_agents/qr.py'),
+                                                  'RL_OM.agents.benchmark_agents.qr.QRPolicy.set_q_r': ( 'agents/benchmark_agents/qr.html#qrpolicy.set_q_r',
+                                                                                                         'RL_OM/agents/benchmark_agents/qr.py')},
             'RL_OM.agents.networks.actors': { 'RL_OM.agents.networks.actors.ActorNetwork': ( 'agents/networks/actors.html#actornetwork',
                                                                                              'RL_OM/agents/networks/actors.py'),
                                               'RL_OM.agents.networks.actors.ActorNetwork.__init__': ( 'agents/networks/actors.html#actornetwork.__init__',
                                                                                                       'RL_OM/agents/networks/actors.py'),
                                               'RL_OM.agents.networks.actors.ActorNetwork.forward': ( 'agents/networks/actors.html#actornetwork.forward',
                                                                                                      'RL_OM/agents/networks/actors.py'),
                                               'RL_OM.agents.networks.actors.ActorNetworkDiscrete': ( 'agents/networks/actors.html#actornetworkdiscrete',
```

### Comparing `RL_OM-0.1.1/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.1.2/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,16 @@
         Returns:
             None
 
         """
 
         self.q_star = np.sqrt((2*self.s*self.d)/self.h)
 
+        print("q_star: ", self.q_star)
+
     def draw_action(self, input):
 
         """
         Generate an action based on the current state.
 
         Returns zero for products which have still sufficient inventory, and the optimal order quantity for products which are running out of stock.
```

### Comparing `RL_OM-0.1.1/RL_OM/agents/networks/actors.py` & `RL_OM-0.1.2/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/networks/base.py` & `RL_OM-0.1.2/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/networks/critics.py` & `RL_OM-0.1.2/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.1.2/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/processors/processors.py` & `RL_OM-0.1.2/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.1.2/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/environments/calculation_functions.py` & `RL_OM-0.1.2/RL_OM/environments/calculation_functions.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/environments/data_generators.py` & `RL_OM-0.1.2/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/environments/feature_converters.py` & `RL_OM-0.1.2/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.1.2/RL_OM/environments/multi_period_inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     def reset(self, state = None):
 
         # TODO: Check in mushroom where state would come from and implement here
         if self.num_observations == self._mdp_info.horizon:
             self.period = 0
         else:
             self.period = np.random.choice(self.num_observations-self._mdp_info.horizon)
-        print("reset with period {}".format(self.period))
+        #print("reset with period {}".format(self.period))
         self.demand_backlog = np.zeros(self.num_products)
         self.inventory = self.start_inventory.copy()
         self.order_pipeline = np.zeros((self.num_products,np.max(self.max_lead_time)))
 
         self.set_observation_state()
 
         return self.observation_state
```

### Comparing `RL_OM-0.1.1/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.1.2/RL_OM/experiment_functions/run_experiment.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.1.1/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.1.2/RL_OM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.1.1
+Version: 0.1.2
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.1.1/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.1.2/RL_OM.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 RL_OM.egg-info/entry_points.txt
 RL_OM.egg-info/not-zip-safe
 RL_OM.egg-info/requires.txt
 RL_OM.egg-info/top_level.txt
 RL_OM/agents/__init__.py
 RL_OM/agents/benchmark_agents/__init__.py
 RL_OM/agents/benchmark_agents/eoq.py
+RL_OM/agents/benchmark_agents/qr.py
 RL_OM/agents/networks/__init__.py
 RL_OM/agents/networks/actors.py
 RL_OM/agents/networks/base.py
 RL_OM/agents/networks/critics.py
 RL_OM/agents/processors/__init__.py
 RL_OM/agents/processors/eoq_preprocessors.py
 RL_OM/agents/processors/processors.py
```

### Comparing `RL_OM-0.1.1/settings.ini` & `RL_OM-0.1.2/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.1.1
+version = 0.1.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.1.1/setup.py` & `RL_OM-0.1.2/setup.py`

 * *Files identical despite different names*

