# Comparing `tmp/mlproj_manager-0.0.5.tar.gz` & `tmp/mlproj_manager-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlproj_manager-0.0.5.tar", last modified: Wed Mar  1 03:26:29 2023, max compression
+gzip compressed data, was "mlproj_manager-0.0.6.tar", last modified: Mon Jun  5 20:15:35 2023, max compression
```

## Comparing `mlproj_manager-0.0.5.tar` & `mlproj_manager-0.0.6.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.219398 mlproj_manager-0.0.5/
--rw-r--r--   0 rlai       (501) staff       (20)     1068 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/LICENSE
--rw-r--r--   0 rlai       (501) staff       (20)     2254 2023-03-01 03:26:29.219580 mlproj_manager-0.0.5/PKG-INFO
--rw-r--r--   0 rlai       (501) staff       (20)     1764 2023-02-08 21:02:01.000000 mlproj_manager-0.0.5/README.md
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.183527 mlproj_manager-0.0.5/mlproj_manager/
--rw-r--r--   0 rlai       (501) staff       (20)       62 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)      301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/definitions.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.191983 mlproj_manager-0.0.5/mlproj_manager/experiments/
--rw-r--r--   0 rlai       (501) staff       (20)      102 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/experiments/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1605 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/experiments/abstract_experiment.py
--rw-r--r--   0 rlai       (501) staff       (20)     3184 2023-02-09 17:13:35.000000 mlproj_manager-0.0.5/mlproj_manager/experiments/experiment_runner.py
--rw-r--r--   0 rlai       (501) staff       (20)     2724 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/experiments/register_experiment.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.194564 mlproj_manager-0.0.5/mlproj_manager/file_management/
--rw-r--r--   0 rlai       (501) staff       (20)      760 2023-02-17 21:24:26.000000 mlproj_manager-0.0.5/mlproj_manager/file_management/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     5286 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/file_management/experiment_management.py
--rw-r--r--   0 rlai       (501) staff       (20)    13624 2023-03-01 03:25:29.000000 mlproj_manager-0.0.5/mlproj_manager/file_management/file_and_directory_management.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.195171 mlproj_manager-0.0.5/mlproj_manager/function_approximators/
--rw-r--r--   0 rlai       (501) staff       (20)       30 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/function_approximators/__init__.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.197184 mlproj_manager-0.0.5/mlproj_manager/function_approximators/neural_networks/
--rw-r--r--   0 rlai       (501) staff       (20)       43 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/function_approximators/neural_networks/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     9821 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/function_approximators/neural_networks/convolutional_network.py
--rw-r--r--   0 rlai       (501) staff       (20)     8467 2023-02-22 15:34:35.000000 mlproj_manager-0.0.5/mlproj_manager/main.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.200607 mlproj_manager-0.0.5/mlproj_manager/plots_and_summaries/
--rw-r--r--   0 rlai       (501) staff       (20)        0 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/plots_and_summaries/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)    12903 2023-02-21 20:11:42.000000 mlproj_manager-0.0.5/mlproj_manager/plots_and_summaries/plot_results.py
--rw-r--r--   0 rlai       (501) staff       (20)     3960 2023-02-21 19:55:11.000000 mlproj_manager-0.0.5/mlproj_manager/plots_and_summaries/plotting_functions.py
--rw-r--r--   0 rlai       (501) staff       (20)      659 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/plots_and_summaries/summaries.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.201428 mlproj_manager-0.0.5/mlproj_manager/problems/
--rw-r--r--   0 rlai       (501) staff       (20)       35 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/problems/__init__.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.204170 mlproj_manager-0.0.5/mlproj_manager/problems/reinforcement_learning/
--rw-r--r--   0 rlai       (501) staff       (20)       89 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/problems/reinforcement_learning/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1574 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py
--rw-r--r--   0 rlai       (501) staff       (20)     6238 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/problems/reinforcement_learning/mountain_car.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.206185 mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/
--rw-r--r--   0 rlai       (501) staff       (20)      243 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/abstract_dataset.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.207545 mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/cifar/
--rw-r--r--   0 rlai       (501) staff       (20)     9890 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.208416 mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/mnist/
--rw-r--r--   0 rlai       (501) staff       (20)     7610 2023-02-09 19:08:17.000000 mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.209251 mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/target_generating_network/
--rw-r--r--   0 rlai       (501) staff       (20)     4336 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.211572 mlproj_manager-0.0.5/mlproj_manager/util/
--rw-r--r--   0 rlai       (501) staff       (20)      145 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/util/__init__.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.214286 mlproj_manager-0.0.5/mlproj_manager/util/data_preprocessing_and_transformations/
--rw-r--r--   0 rlai       (501) staff       (20)      163 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/util/data_preprocessing_and_transformations/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     7164 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py
--rw-r--r--   0 rlai       (501) staff       (20)     3928 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py
--rw-r--r--   0 rlai       (501) staff       (20)     1750 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/util/experiments_util.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.218485 mlproj_manager-0.0.5/mlproj_manager/util/neural_networks/
--rw-r--r--   0 rlai       (501) staff       (20)      420 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/util/neural_networks/__init__.py
--rw-r--r--   0 rlai       (501) staff       (20)     1692 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/util/neural_networks/network_architecture.py
--rw-r--r--   0 rlai       (501) staff       (20)      287 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/util/neural_networks/other_torch_utilities.py
--rw-r--r--   0 rlai       (501) staff       (20)     6328 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py
-drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-03-01 03:26:29.186726 mlproj_manager-0.0.5/mlproj_manager.egg-info/
--rw-r--r--   0 rlai       (501) staff       (20)     2254 2023-03-01 03:26:29.000000 mlproj_manager-0.0.5/mlproj_manager.egg-info/PKG-INFO
--rw-r--r--   0 rlai       (501) staff       (20)     2220 2023-03-01 03:26:29.000000 mlproj_manager-0.0.5/mlproj_manager.egg-info/SOURCES.txt
--rw-r--r--   0 rlai       (501) staff       (20)        1 2023-03-01 03:26:29.000000 mlproj_manager-0.0.5/mlproj_manager.egg-info/dependency_links.txt
--rw-r--r--   0 rlai       (501) staff       (20)       69 2023-03-01 03:26:29.000000 mlproj_manager-0.0.5/mlproj_manager.egg-info/requires.txt
--rw-r--r--   0 rlai       (501) staff       (20)       15 2023-03-01 03:26:29.000000 mlproj_manager-0.0.5/mlproj_manager.egg-info/top_level.txt
--rw-r--r--   0 rlai       (501) staff       (20)       87 2023-02-07 20:44:06.000000 mlproj_manager-0.0.5/pyproject.toml
--rw-r--r--   0 rlai       (501) staff       (20)      657 2023-03-01 03:26:29.220343 mlproj_manager-0.0.5/setup.cfg
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.106946 mlproj_manager-0.0.6/
+-rw-r--r--   0 rlai       (501) staff       (20)     1068 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/LICENSE
+-rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-05 20:15:35.107138 mlproj_manager-0.0.6/PKG-INFO
+-rw-r--r--   0 rlai       (501) staff       (20)     1777 2023-06-05 20:14:53.000000 mlproj_manager-0.0.6/README.md
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.061129 mlproj_manager-0.0.6/mlproj_manager/
+-rw-r--r--   0 rlai       (501) staff       (20)       62 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)      301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/definitions.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.069338 mlproj_manager-0.0.6/mlproj_manager/experiments/
+-rw-r--r--   0 rlai       (501) staff       (20)      102 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/experiments/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1605 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/experiments/abstract_experiment.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3184 2023-02-09 17:13:35.000000 mlproj_manager-0.0.6/mlproj_manager/experiments/experiment_runner.py
+-rw-r--r--   0 rlai       (501) staff       (20)     2724 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/experiments/register_experiment.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.072206 mlproj_manager-0.0.6/mlproj_manager/file_management/
+-rw-r--r--   0 rlai       (501) staff       (20)      760 2023-02-17 21:24:26.000000 mlproj_manager-0.0.6/mlproj_manager/file_management/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     5286 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/file_management/experiment_management.py
+-rw-r--r--   0 rlai       (501) staff       (20)    13624 2023-03-01 03:25:29.000000 mlproj_manager-0.0.6/mlproj_manager/file_management/file_and_directory_management.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.075178 mlproj_manager-0.0.6/mlproj_manager/function_approximators/
+-rw-r--r--   0 rlai       (501) staff       (20)       30 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/function_approximators/__init__.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.079877 mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/
+-rw-r--r--   0 rlai       (501) staff       (20)       92 2023-06-05 19:50:34.000000 mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     9821 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/convolutional_network.py
+-rw-r--r--   0 rlai       (501) staff       (20)     6295 2023-06-05 20:07:54.000000 mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/general_deep_network.py
+-rw-r--r--   0 rlai       (501) staff       (20)     8422 2023-03-01 03:30:11.000000 mlproj_manager-0.0.6/mlproj_manager/main.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.088051 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/
+-rw-r--r--   0 rlai       (501) staff       (20)        0 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)    12903 2023-02-21 20:11:42.000000 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/plot_results.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3960 2023-02-21 19:55:11.000000 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/plotting_functions.py
+-rw-r--r--   0 rlai       (501) staff       (20)      659 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/summaries.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.089134 mlproj_manager-0.0.6/mlproj_manager/problems/
+-rw-r--r--   0 rlai       (501) staff       (20)       35 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/__init__.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.091976 mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/
+-rw-r--r--   0 rlai       (501) staff       (20)       89 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1574 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py
+-rw-r--r--   0 rlai       (501) staff       (20)     6238 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/mountain_car.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.093601 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/
+-rw-r--r--   0 rlai       (501) staff       (20)      243 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1301 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/abstract_dataset.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.094643 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/cifar/
+-rw-r--r--   0 rlai       (501) staff       (20)     9890 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.095456 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/mnist/
+-rw-r--r--   0 rlai       (501) staff       (20)     7610 2023-02-09 19:08:17.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.096426 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/target_generating_network/
+-rw-r--r--   0 rlai       (501) staff       (20)     4336 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.099774 mlproj_manager-0.0.6/mlproj_manager/util/
+-rw-r--r--   0 rlai       (501) staff       (20)      145 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/__init__.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.102788 mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/
+-rw-r--r--   0 rlai       (501) staff       (20)      163 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     7164 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py
+-rw-r--r--   0 rlai       (501) staff       (20)     3928 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1750 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/experiments_util.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.106237 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/
+-rw-r--r--   0 rlai       (501) staff       (20)      449 2023-06-05 20:01:39.000000 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/__init__.py
+-rw-r--r--   0 rlai       (501) staff       (20)     1986 2023-06-05 20:07:28.000000 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/network_architecture.py
+-rw-r--r--   0 rlai       (501) staff       (20)      287 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/other_torch_utilities.py
+-rw-r--r--   0 rlai       (501) staff       (20)     6328 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py
+drwxr-xr-x   0 rlai       (501) staff       (20)        0 2023-06-05 20:15:35.065001 mlproj_manager-0.0.6/mlproj_manager.egg-info/
+-rw-r--r--   0 rlai       (501) staff       (20)     2266 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/PKG-INFO
+-rw-r--r--   0 rlai       (501) staff       (20)     2298 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 rlai       (501) staff       (20)        1 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 rlai       (501) staff       (20)       69 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/requires.txt
+-rw-r--r--   0 rlai       (501) staff       (20)       15 2023-06-05 20:15:35.000000 mlproj_manager-0.0.6/mlproj_manager.egg-info/top_level.txt
+-rw-r--r--   0 rlai       (501) staff       (20)       87 2023-02-07 20:44:06.000000 mlproj_manager-0.0.6/pyproject.toml
+-rw-r--r--   0 rlai       (501) staff       (20)      657 2023-06-05 20:15:35.108015 mlproj_manager-0.0.6/setup.cfg
```

### Comparing `mlproj_manager-0.0.5/LICENSE` & `mlproj_manager-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/PKG-INFO` & `mlproj_manager-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlproj_manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package with utilities for managing and running machine learning projects
 Home-page: https://github.com/JFernando4/Research_Project_Manager
 Author: J. Fernando Hernandez-Garcia
 Author-email: jfhernan@ualberta.ca
 Keywords: ml,rl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 `python3 -m pip install mlproj_manager`
 
 ## Usage 
 Here is a quick list of steps to create and run a new experiment:
 
 1. Write a python script with a class that is a child of the `Experiment` abstract class in 
 `./mlproj_manager/experiments/abstract_experiment.py`. See `./examples/non_stationary_cifar_example` for an example. 
-2. Register the experiment using the command `python -m mlproj_manager.register_experiment` with the arguments
+2. Register the experiment using the command `python -m mlproj_manager.experiments.register_experiment` with the arguments
 `--experiment-name` followed by a named of your choosing, `--experiment-path` followed by the path to the script
 created in step 1, and `--experiment-class-name` followed by the name of the class defined in the script created in 
 step 1.
 3. Create a `config.json` file for your experiment that contains all the relevant details for running the experiment.
 See `./examples/non_stationary_cifar_example/config_files/backprop.json` for an example.
 4. Finally, run the experiment using the command `python -m mlproj_manager.main` with the arguments `--experiment-name` 
 followed by the experiment name used in step 2, `--experiment-config-path` followed by the path to the config file
```

### Comparing `mlproj_manager-0.0.5/README.md` & `mlproj_manager-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 `python3 -m pip install mlproj_manager`
 
 ## Usage 
 Here is a quick list of steps to create and run a new experiment:
 
 1. Write a python script with a class that is a child of the `Experiment` abstract class in 
 `./mlproj_manager/experiments/abstract_experiment.py`. See `./examples/non_stationary_cifar_example` for an example. 
-2. Register the experiment using the command `python -m mlproj_manager.register_experiment` with the arguments
+2. Register the experiment using the command `python -m mlproj_manager.experiments.register_experiment` with the arguments
 `--experiment-name` followed by a named of your choosing, `--experiment-path` followed by the path to the script
 created in step 1, and `--experiment-class-name` followed by the name of the class defined in the script created in 
 step 1.
 3. Create a `config.json` file for your experiment that contains all the relevant details for running the experiment.
 See `./examples/non_stationary_cifar_example/config_files/backprop.json` for an example.
 4. Finally, run the experiment using the command `python -m mlproj_manager.main` with the arguments `--experiment-name` 
 followed by the experiment name used in step 2, `--experiment-config-path` followed by the path to the config file
 created in step 3, `--use-slurm` (optional) to indicate whether to schedule the experiment using slurm, and
 `--slurm-config-path` (required only if using slurm) followed by the path to a similar file as the one created for step
-3 but with parameters relevant to the slurm scheduler. 
+3 but with parameters relevant to the slurm scheduler.
```

### Comparing `mlproj_manager-0.0.5/mlproj_manager/experiments/abstract_experiment.py` & `mlproj_manager-0.0.6/mlproj_manager/experiments/abstract_experiment.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/experiments/experiment_runner.py` & `mlproj_manager-0.0.6/mlproj_manager/experiments/experiment_runner.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/experiments/register_experiment.py` & `mlproj_manager-0.0.6/mlproj_manager/experiments/register_experiment.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/file_management/__init__.py` & `mlproj_manager-0.0.6/mlproj_manager/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/file_management/experiment_management.py` & `mlproj_manager-0.0.6/mlproj_manager/file_management/experiment_management.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/file_management/file_and_directory_management.py` & `mlproj_manager-0.0.6/mlproj_manager/file_management/file_and_directory_management.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/function_approximators/neural_networks/convolutional_network.py` & `mlproj_manager-0.0.6/mlproj_manager/function_approximators/neural_networks/convolutional_network.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/main.py` & `mlproj_manager-0.0.6/mlproj_manager/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 
     num_processed = 0           # number of processed runs
     current_job = 0             # current job number
     current_exp_batch = []      # list of experiments to be run in batch
 
     while num_processed != len(missing_indices):    # continue until all missing indices have been scheduled
         temp_job_num = num_processed + len(current_exp_batch)
-        print(missing_indices[temp_job_num])
         temp_dict = {**experiment["dict"], "index": int(missing_indices[temp_job_num]),
                      "plot_results": False, "verbose": verbose, "debug": False}
         current_exp_batch.append(temp_dict)
 
         # when batch size matches max_runs_per_job or when this is the last missing index, then schedule job
         if len(current_exp_batch) == slurm_config["max_runs_per_job"] or temp_job_num + 1 == len(missing_indices):
             # write slurm file
```

### Comparing `mlproj_manager-0.0.5/mlproj_manager/plots_and_summaries/plot_results.py` & `mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/plot_results.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/plots_and_summaries/plotting_functions.py` & `mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/plots_and_summaries/summaries.py` & `mlproj_manager-0.0.6/mlproj_manager/plots_and_summaries/summaries.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py` & `mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/problems/reinforcement_learning/mountain_car.py` & `mlproj_manager-0.0.6/mlproj_manager/problems/reinforcement_learning/mountain_car.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/abstract_dataset.py` & `mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/abstract_dataset.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py` & `mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/cifar/cifar_data_loader.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py` & `mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/mnist/mnist_data_loader.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py` & `mlproj_manager-0.0.6/mlproj_manager/problems/supervised_learning/target_generating_network/taget_generating_network.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py` & `mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/image_transformations.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py` & `mlproj_manager-0.0.6/mlproj_manager/util/data_preprocessing_and_transformations/normalization_and_preprocessing.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/util/experiments_util.py` & `mlproj_manager-0.0.6/mlproj_manager/util/experiments_util.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager/util/neural_networks/network_architecture.py` & `mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/network_architecture.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,7 +40,18 @@
         return tanh
     elif name == "sigmoid":
         return sigmoid
     elif name is None:
         return lambda x: x
     else:
         raise ValueError("{0} is not a valid activation!")
+
+
+def get_activation_module(name: str):
+    if name == "relu":
+        return torch.nn.ReLU()
+    elif name == "tanh":
+        return torch.nn.Tanh()
+    elif name == "sigmoid":
+        return torch.nn.Sigmoid()
+    else:
+        raise ValueError("{0} is not a valid activation!".format(name))
```

### Comparing `mlproj_manager-0.0.5/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py` & `mlproj_manager-0.0.6/mlproj_manager/util/neural_networks/weights_initialization_and_manipulation.py`

 * *Files identical despite different names*

### Comparing `mlproj_manager-0.0.5/mlproj_manager.egg-info/PKG-INFO` & `mlproj_manager-0.0.6/mlproj_manager.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlproj-manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package with utilities for managing and running machine learning projects
 Home-page: https://github.com/JFernando4/Research_Project_Manager
 Author: J. Fernando Hernandez-Garcia
 Author-email: jfhernan@ualberta.ca
 Keywords: ml,rl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 `python3 -m pip install mlproj_manager`
 
 ## Usage 
 Here is a quick list of steps to create and run a new experiment:
 
 1. Write a python script with a class that is a child of the `Experiment` abstract class in 
 `./mlproj_manager/experiments/abstract_experiment.py`. See `./examples/non_stationary_cifar_example` for an example. 
-2. Register the experiment using the command `python -m mlproj_manager.register_experiment` with the arguments
+2. Register the experiment using the command `python -m mlproj_manager.experiments.register_experiment` with the arguments
 `--experiment-name` followed by a named of your choosing, `--experiment-path` followed by the path to the script
 created in step 1, and `--experiment-class-name` followed by the name of the class defined in the script created in 
 step 1.
 3. Create a `config.json` file for your experiment that contains all the relevant details for running the experiment.
 See `./examples/non_stationary_cifar_example/config_files/backprop.json` for an example.
 4. Finally, run the experiment using the command `python -m mlproj_manager.main` with the arguments `--experiment-name` 
 followed by the experiment name used in step 2, `--experiment-config-path` followed by the path to the config file
```

### Comparing `mlproj_manager-0.0.5/mlproj_manager.egg-info/SOURCES.txt` & `mlproj_manager-0.0.6/mlproj_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 mlproj_manager/experiments/register_experiment.py
 mlproj_manager/file_management/__init__.py
 mlproj_manager/file_management/experiment_management.py
 mlproj_manager/file_management/file_and_directory_management.py
 mlproj_manager/function_approximators/__init__.py
 mlproj_manager/function_approximators/neural_networks/__init__.py
 mlproj_manager/function_approximators/neural_networks/convolutional_network.py
+mlproj_manager/function_approximators/neural_networks/general_deep_network.py
 mlproj_manager/plots_and_summaries/__init__.py
 mlproj_manager/plots_and_summaries/plot_results.py
 mlproj_manager/plots_and_summaries/plotting_functions.py
 mlproj_manager/plots_and_summaries/summaries.py
 mlproj_manager/problems/__init__.py
 mlproj_manager/problems/reinforcement_learning/__init__.py
 mlproj_manager/problems/reinforcement_learning/abstract_rl_environment.py
```

### Comparing `mlproj_manager-0.0.5/setup.cfg` & `mlproj_manager-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlproj_manager
-version = 0.0.5
+version = 0.0.6
 author = J. Fernando Hernandez-Garcia
 author_email = jfhernan@ualberta.ca
 description = A package with utilities for managing and running machine learning projects
 long_description = file: README.md
 url = https://github.com/JFernando4/Research_Project_Manager
 license_files = LICENSE
 keywords = ml, rl
```

