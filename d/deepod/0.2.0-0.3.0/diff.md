# Comparing `tmp/deepod-0.2.0.tar.gz` & `tmp/deepod-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepod-0.2.0.tar", last modified: Thu Dec  1 08:13:16 2022, max compression
+gzip compressed data, was "deepod-0.3.0.tar", last modified: Mon Jun  5 06:31:10 2023, max compression
```

## Comparing `deepod-0.2.0.tar` & `deepod-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,70 @@
-drwxr-xr-x   0 think      (501) staff       (20)        0 2022-12-01 08:13:16.712689 deepod-0.2.0/
--rw-r--r--   0 think      (501) staff       (20)     3412 2022-12-01 08:13:16.712571 deepod-0.2.0/PKG-INFO
--rw-r--r--   0 think      (501) staff       (20)     2909 2022-12-01 08:13:00.000000 deepod-0.2.0/README.rst
-drwxr-xr-x   0 think      (501) staff       (20)        0 2022-12-01 08:13:16.707381 deepod-0.2.0/deepod/
--rw-r--r--   0 think      (501) staff       (20)      146 2022-11-12 15:17:47.000000 deepod-0.2.0/deepod/__init__.py
-drwxr-xr-x   0 think      (501) staff       (20)        0 2022-12-01 08:13:16.708373 deepod-0.2.0/deepod/core/
--rw-r--r--   0 think      (501) staff       (20)      614 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/core/__init__.py
--rw-r--r--   0 think      (501) staff       (20)    11309 2022-12-01 02:55:28.000000 deepod-0.2.0/deepod/core/base_model.py
--rw-r--r--   0 think      (501) staff       (20)     4739 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/core/base_networks.py
-drwxr-xr-x   0 think      (501) staff       (20)        0 2022-12-01 08:13:16.708742 deepod-0.2.0/deepod/model_selection/
--rw-r--r--   0 think      (501) staff       (20)       43 2022-11-12 16:07:52.000000 deepod-0.2.0/deepod/model_selection/__init__.py
--rw-r--r--   0 think      (501) staff       (20)     7894 2022-11-12 16:07:52.000000 deepod-0.2.0/deepod/model_selection/fmms.py
--rw-r--r--   0 think      (501) staff       (20)    13562 2022-12-01 02:55:28.000000 deepod-0.2.0/deepod/model_selection/gene_feature.py
-drwxr-xr-x   0 think      (501) staff       (20)        0 2022-12-01 08:13:16.710195 deepod-0.2.0/deepod/models/
--rw-r--r--   0 think      (501) staff       (20)      383 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/models/__init__.py
--rw-r--r--   0 think      (501) staff       (20)     7381 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/models/anogan.py
--rw-r--r--   0 think      (501) staff       (20)     6376 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/models/devnet.py
--rw-r--r--   0 think      (501) staff       (20)     6375 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/models/dsad.py
--rw-r--r--   0 think      (501) staff       (20)     5647 2022-11-19 07:51:53.000000 deepod-0.2.0/deepod/models/dsvdd.py
--rw-r--r--   0 think      (501) staff       (20)     7187 2022-11-20 11:58:26.000000 deepod-0.2.0/deepod/models/goad.py
--rw-r--r--   0 think      (501) staff       (20)    10711 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/models/icl.py
--rw-r--r--   0 think      (501) staff       (20)     6781 2022-11-19 07:51:53.000000 deepod-0.2.0/deepod/models/neutral.py
--rw-r--r--   0 think      (501) staff       (20)     7104 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/models/prenet.py
--rw-r--r--   0 think      (501) staff       (20)     8445 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/models/rca.py
--rw-r--r--   0 think      (501) staff       (20)     5348 2022-11-19 07:51:53.000000 deepod-0.2.0/deepod/models/rdp.py
--rw-r--r--   0 think      (501) staff       (20)     9321 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/models/repen.py
-drwxr-xr-x   0 think      (501) staff       (20)        0 2022-12-01 08:13:16.711723 deepod-0.2.0/deepod/test/
--rw-r--r--   0 think      (501) staff       (20)       23 2022-12-01 02:55:28.000000 deepod-0.2.0/deepod/test/__init__.py
--rw-r--r--   0 think      (501) staff       (20)     6210 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/test/test_devnet.py
--rw-r--r--   0 think      (501) staff       (20)     6146 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/test/test_dsad.py
--rw-r--r--   0 think      (501) staff       (20)     5649 2022-12-01 02:55:28.000000 deepod-0.2.0/deepod/test/test_dsvdd.py
--rw-r--r--   0 think      (501) staff       (20)     5631 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/test/test_goad.py
--rw-r--r--   0 think      (501) staff       (20)     5651 2022-12-01 02:55:28.000000 deepod-0.2.0/deepod/test/test_icl.py
--rw-r--r--   0 think      (501) staff       (20)     5640 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/test/test_neutral.py
--rw-r--r--   0 think      (501) staff       (20)     6249 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/test/test_prenet.py
--rw-r--r--   0 think      (501) staff       (20)     5649 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/test/test_rca.py
--rw-r--r--   0 think      (501) staff       (20)     5645 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/test/test_rdp.py
--rw-r--r--   0 think      (501) staff       (20)     5640 2022-12-01 08:00:53.000000 deepod-0.2.0/deepod/test/test_repen.py
-drwxr-xr-x   0 think      (501) staff       (20)        0 2022-12-01 08:13:16.711933 deepod-0.2.0/deepod/utils/
--rw-r--r--   0 think      (501) staff       (20)        0 2022-12-01 02:55:28.000000 deepod-0.2.0/deepod/utils/__init__.py
--rw-r--r--   0 think      (501) staff       (20)     5091 2022-12-01 02:55:28.000000 deepod-0.2.0/deepod/utils/data.py
--rw-r--r--   0 think      (501) staff       (20)      569 2022-11-09 08:48:54.000000 deepod-0.2.0/deepod/version.py
-drwxr-xr-x   0 think      (501) staff       (20)        0 2022-12-01 08:13:16.708005 deepod-0.2.0/deepod.egg-info/
--rw-r--r--   0 think      (501) staff       (20)     3412 2022-12-01 08:13:16.000000 deepod-0.2.0/deepod.egg-info/PKG-INFO
--rw-r--r--   0 think      (501) staff       (20)     1101 2022-12-01 08:13:16.000000 deepod-0.2.0/deepod.egg-info/SOURCES.txt
--rw-r--r--   0 think      (501) staff       (20)        1 2022-12-01 08:13:16.000000 deepod-0.2.0/deepod.egg-info/dependency_links.txt
--rw-r--r--   0 think      (501) staff       (20)       87 2022-12-01 08:13:16.000000 deepod-0.2.0/deepod.egg-info/requires.txt
--rw-r--r--   0 think      (501) staff       (20)       16 2022-12-01 08:13:16.000000 deepod-0.2.0/deepod.egg-info/top_level.txt
-drwxr-xr-x   0 think      (501) staff       (20)        0 2022-12-01 08:13:16.712394 deepod-0.2.0/examples/
--rw-r--r--   0 think      (501) staff       (20)        0 2022-11-12 15:17:47.000000 deepod-0.2.0/examples/__init__.py
--rw-r--r--   0 think      (501) staff       (20)     4195 2022-11-19 07:51:53.000000 deepod-0.2.0/examples/detection_run_all.py
--rw-r--r--   0 think      (501) staff       (20)     1446 2022-11-12 16:07:52.000000 deepod-0.2.0/examples/model_selection_fmms_example.py
--rw-r--r--   0 think      (501) staff       (20)     8530 2022-12-01 08:00:53.000000 deepod-0.2.0/examples/utils.py
--rw-r--r--   0 think      (501) staff       (20)       38 2022-12-01 08:13:16.712731 deepod-0.2.0/setup.cfg
--rw-r--r--   0 think      (501) staff       (20)     1049 2022-12-01 08:01:12.000000 deepod-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.197908 deepod-0.3.0/
+-rw-rw-rw-   0        0        0     5098 2023-06-05 06:31:10.196911 deepod-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4540 2023-06-05 05:04:29.000000 deepod-0.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.124581 deepod-0.3.0/deepod/
+-rw-rw-rw-   0        0        0      149 2022-11-13 02:46:33.000000 deepod-0.3.0/deepod/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.138544 deepod-0.3.0/deepod/core/
+-rw-rw-rw-   0        0        0      631 2022-12-01 06:37:35.000000 deepod-0.3.0/deepod/core/__init__.py
+-rw-rw-rw-   0        0        0    14018 2023-04-11 12:08:45.000000 deepod-0.3.0/deepod/core/base_model.py
+-rw-rw-rw-   0        0        0    22809 2023-06-05 05:26:14.000000 deepod-0.3.0/deepod/core/base_networks.py
+-rw-rw-rw-   0        0        0    17614 2023-06-05 05:16:46.000000 deepod-0.3.0/deepod/core/base_transformer_network.py
+-rw-rw-rw-   0        0        0    22776 2023-04-05 14:24:42.000000 deepod-0.3.0/deepod/core/base_transformer_network_dev.py
+-rw-rw-rw-   0        0        0      834 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/core/network_utility.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.142534 deepod-0.3.0/deepod/core/transformer/
+-rw-rw-rw-   0        0        0        0 2023-04-11 11:47:40.000000 deepod-0.3.0/deepod/core/transformer/__init__.py
+-rw-rw-rw-   0        0        0     6574 2023-04-11 11:47:40.000000 deepod-0.3.0/deepod/core/transformer/embed.py
+-rw-rw-rw-   0        0        0    13085 2023-04-11 11:47:40.000000 deepod-0.3.0/deepod/core/transformer/selfattention_family.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.145526 deepod-0.3.0/deepod/model_selection/
+-rw-rw-rw-   0        0        0       46 2022-11-13 02:57:43.000000 deepod-0.3.0/deepod/model_selection/__init__.py
+-rw-rw-rw-   0        0        0     8137 2022-11-13 02:57:43.000000 deepod-0.3.0/deepod/model_selection/fmms.py
+-rw-rw-rw-   0        0        0    13968 2022-11-16 06:32:40.000000 deepod-0.3.0/deepod/model_selection/gene_feature.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.166991 deepod-0.3.0/deepod/models/
+-rw-rw-rw-   0        0        0      527 2023-06-05 04:51:55.000000 deepod-0.3.0/deepod/models/__init__.py
+-rw-rw-rw-   0        0        0     4349 2023-06-05 05:27:01.000000 deepod-0.3.0/deepod/models/_local_test_.py
+-rw-rw-rw-   0        0        0     7726 2023-06-05 05:12:12.000000 deepod-0.3.0/deepod/models/devnet.py
+-rw-rw-rw-   0        0        0    13905 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/models/dif.py
+-rw-rw-rw-   0        0        0     8738 2023-04-11 11:47:40.000000 deepod-0.3.0/deepod/models/dsad.py
+-rw-rw-rw-   0        0        0     6845 2023-06-05 05:26:23.000000 deepod-0.3.0/deepod/models/dsvdd.py
+-rw-rw-rw-   0        0        0     7631 2023-06-05 05:30:27.000000 deepod-0.3.0/deepod/models/feawad.py
+-rw-rw-rw-   0        0        0     6798 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/models/goad.py
+-rw-rw-rw-   0        0        0     9856 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/models/icl.py
+-rw-rw-rw-   0        0        0     6399 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/models/neutral.py
+-rw-rw-rw-   0        0        0     8222 2023-04-11 12:32:32.000000 deepod-0.3.0/deepod/models/prenet.py
+-rw-rw-rw-   0        0        0     8114 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/models/rca.py
+-rw-rw-rw-   0        0        0     4906 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/models/rdp.py
+-rw-rw-rw-   0        0        0     9443 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/models/repen.py
+-rw-rw-rw-   0        0        0    13234 2023-03-28 04:07:38.000000 deepod-0.3.0/deepod/models/rosas.py
+-rw-rw-rw-   0        0        0    10063 2023-06-05 05:52:51.000000 deepod-0.3.0/deepod/models/slad.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.187935 deepod-0.3.0/deepod/test/
+-rw-rw-rw-   0        0        0       23 2022-11-16 06:32:40.000000 deepod-0.3.0/deepod/test/__init__.py
+-rw-rw-rw-   0        0        0     7594 2023-06-05 06:27:58.000000 deepod-0.3.0/deepod/test/test_devnet.py
+-rw-rw-rw-   0        0        0     7038 2023-06-05 06:27:55.000000 deepod-0.3.0/deepod/test/test_dif.py
+-rw-rw-rw-   0        0        0     8625 2023-06-05 05:47:12.000000 deepod-0.3.0/deepod/test/test_dsad.py
+-rw-rw-rw-   0        0        0     7452 2023-06-05 05:13:57.000000 deepod-0.3.0/deepod/test/test_dsvdd.py
+-rw-rw-rw-   0        0        0     7497 2023-06-05 06:28:30.000000 deepod-0.3.0/deepod/test/test_feawad.py
+-rw-rw-rw-   0        0        0     5790 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/test/test_goad.py
+-rw-rw-rw-   0        0        0     5798 2022-12-01 06:37:35.000000 deepod-0.3.0/deepod/test/test_icl.py
+-rw-rw-rw-   0        0        0     5787 2022-12-01 06:37:35.000000 deepod-0.3.0/deepod/test/test_neutral.py
+-rw-rw-rw-   0        0        0     7344 2023-06-05 06:29:30.000000 deepod-0.3.0/deepod/test/test_prenet.py
+-rw-rw-rw-   0        0        0     5796 2022-12-01 06:37:35.000000 deepod-0.3.0/deepod/test/test_rca.py
+-rw-rw-rw-   0        0        0     5792 2022-12-01 06:37:35.000000 deepod-0.3.0/deepod/test/test_rdp.py
+-rw-rw-rw-   0        0        0     7034 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/test/test_repen.py
+-rw-rw-rw-   0        0        0     5794 2023-06-05 05:50:09.000000 deepod-0.3.0/deepod/test/test_slad.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.189929 deepod-0.3.0/deepod/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-16 06:32:40.000000 deepod-0.3.0/deepod/utils/__init__.py
+-rw-rw-rw-   0        0        0     5248 2022-11-16 06:32:40.000000 deepod-0.3.0/deepod/utils/data.py
+-rw-rw-rw-   0        0        0     3167 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/utils/utility.py
+-rw-rw-rw-   0        0        0      593 2023-03-31 01:10:21.000000 deepod-0.3.0/deepod/version.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.128570 deepod-0.3.0/deepod.egg-info/
+-rw-rw-rw-   0        0        0     5098 2023-06-05 06:31:10.000000 deepod-0.3.0/deepod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1529 2023-06-05 06:31:10.000000 deepod-0.3.0/deepod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 06:31:10.000000 deepod-0.3.0/deepod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-06-05 06:31:10.000000 deepod-0.3.0/deepod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 06:31:10.000000 deepod-0.3.0/deepod.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 06:31:10.195914 deepod-0.3.0/examples/
+-rw-rw-rw-   0        0        0        0 2022-11-13 02:46:33.000000 deepod-0.3.0/examples/__init__.py
+-rw-rw-rw-   0        0        0     4303 2023-06-05 05:55:06.000000 deepod-0.3.0/examples/detection_run_all.py
+-rw-rw-rw-   0        0        0     1482 2022-11-13 02:57:43.000000 deepod-0.3.0/examples/model_selection_fmms_example.py
+-rw-rw-rw-   0        0        0     8786 2022-12-01 06:37:35.000000 deepod-0.3.0/examples/utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-05 06:31:10.197908 deepod-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2023-06-05 06:21:29.000000 deepod-0.3.0/setup.py
```

### Comparing `deepod-0.2.0/PKG-INFO` & `deepod-0.3.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,114 @@
-Metadata-Version: 2.1
-Name: deepod
-Version: 0.2.0
-Home-page: https://github.com/xuhongzuo/DeepOD
-Author: Hongzuo Xu
-Author-email: hongzuoxu@126.com
-License: MIT License
-Keywords: outlier detection,anomaly detection,deep anomaly detection,deep learning,data mining
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: BSD License
-Description-Content-Type: text/x-rst
-
-Python Deep Outlier/Anomaly Detection (DeepOD)
-==================================================
-
-.. image:: https://github.com/xuhongzuo/DeepOD/actions/workflows/testing_conda.yml/badge.svg
-   :target: https://github.com/xuhongzuo/DeepOD/actions/workflows/testing_conda.yml
-   :alt: testing
-
-.. image:: https://github.com/xuhongzuo/DeepOD/actions/workflows/testing.yml/badge.svg
-   :target: https://github.com/xuhongzuo/DeepOD/actions/workflows/testing.yml
-   :alt: testing2
-   
-.. image:: https://pepy.tech/badge/deepod
-   :target: https://pepy.tech/project/deepod
-   :alt: downloads
-   
-
-**DeepOD** is an open-source python framework for deep learning-based anomaly detection on multivariate data. DeepOD provides unified low-code implementation of different detection models based on PyTorch.
-
-
-DeepOD includes ten popular deep outlier detection / anomaly detection algorithms (in unsupervised/weakly-supervised paradigm) for now. More baseline algorithms will be included later.
-
-
-
-Installation
-~~~~~~~~~~~~~~
-The DeepOD framework can be installed via:
-
-
-.. code-block:: bash
-
-
-    pip install deepod
-
-
-install a developing version
-
-
-.. code-block:: bash
-
-
-    git clone https://github.com/xuhongzuo/DeepOD.git
-    cd DeepOD
-    pip install .
-
-
-Supported Models
-~~~~~~~~~~~~~~~~~
-
-**Detection models:**
-
-.. csv-table:: 
- :header: "Model", "Venue", "Year", "Type", "Title"  
- :widths: 4, 4, 4, 8, 20 
-
- Deep SVDD, ICML, 2018, unsupervised, Deep One-Class Classification  
- REPEN, KDD, 2018, unsupervised, Learning Representations of Ultrahigh-dimensional Data for Random Distance-based Outlier Detection
- RDP, IJCAI, 2020, unsupervised, Unsupervised Representation Learning by Predicting Random Distances  
- RCA, IJCAI, 2021, unsupervised, RCA: A Deep Collaborative Autoencoder Approach for Anomaly Detection
- GOAD, ICLR, 2020, unsupervised, Classification-Based Anomaly Detection for General Data
- NeuTraL, ICML, 2021, unsupervised, Neural Transformation Learning for Deep Anomaly Detection Beyond Images
- ICL, ICLR, 2022, unsupervised, Anomaly Detection for Tabular Data with Internal Contrastive Learning
- DevNet, KDD, 2019, weakly-supervised, Deep Anomaly Detection with Deviation Networks
- PReNet, ArXiv, 2020, weakly-supervised, Deep Weakly-supervised Anomaly Detection
- Deep SAD, ICLR, 2020, weakly-supervised, Deep Semi-Supervised Anomaly Detection
-
-
-Usages
-~~~~~~~~~~~~~~~~~
-
-
-DeepOD can be used in a few lines of code. This API style is the same with sklearn and PyOD.
-
-
-.. code-block:: python
-
-
-    # unsupervised methods
-    from deepod.models.dsvdd import DeepSVDD
-    clf = DeepSVDD()
-    clf.fit(X_train, y=None)
-    scores = clf.decision_function(X_test)
-
-    # weakly-supervised methods
-    from deepod.models.devnet import DevNet
-    clf = DevNet()
-    clf.fit(X_train, y=semi_y) # semi_y uses 1 for known anomalies, and 0 for unlabeled data
-    scores = clf.decision_function(X_test)
-
+Python Deep Outlier/Anomaly Detection (DeepOD)
+==================================================
+
+.. image:: https://github.com/xuhongzuo/DeepOD/actions/workflows/testing_conda.yml/badge.svg
+   :target: https://github.com/xuhongzuo/DeepOD/actions/workflows/testing_conda.yml
+   :alt: testing
+
+.. image:: https://github.com/xuhongzuo/DeepOD/actions/workflows/testing.yml/badge.svg
+   :target: https://github.com/xuhongzuo/DeepOD/actions/workflows/testing.yml
+   :alt: testing2
+
+.. image:: https://coveralls.io/repos/github/xuhongzuo/DeepOD/badge.svg?branch=main
+    :target: https://coveralls.io/github/xuhongzuo/DeepOD?branch=main
+    :alt: coveralls
+
+.. image:: https://static.pepy.tech/personalized-badge/deepod?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+   :target: https://pepy.tech/project/deepod
+   :alt: downloads
+   
+
+**DeepOD** is an open-source python framework for deep learning-based anomaly detection on multivariate/time-series data. DeepOD provides unified implementation of different detection models based on PyTorch.
+
+
+DeepOD includes 13 deep outlier detection / anomaly detection algorithms (in unsupervised/weakly-supervised paradigm) for now. More baseline algorithms will be included later.
+
+
+🔭 *We are working on a new feature -- by simply setting a few parameters, different deep anomaly detection models can not only handle different data types.*   
+
+- We have finished some attempts on partial models like Deep SVDD, DevNet, Deep SAD, PReNet and DIF. These models can use temporal networks like LSTM, GRU, TCN, Conv, Transformer to handle time series data. 
+- *Future work*: we also want to implement several network structure, so as to processing more data types like graphs and images by simply plugging in corresponding network architecture. 
+
+
+Installation
+~~~~~~~~~~~~~~
+The DeepOD framework can be installed via:
+
+
+.. code-block:: bash
+
+
+    pip install deepod
+
+
+install a developing version (strongly recommend)
+
+
+.. code-block:: bash
+
+
+    git clone https://github.com/xuhongzuo/DeepOD.git
+    cd DeepOD
+    pip install .
+
+
+Supported Models
+~~~~~~~~~~~~~~~~~
+
+**Detection models:**
+
+.. csv-table:: 
+ :header: "Model", "Venue", "Year", "Type", "Title"
+ :widths: 4, 4, 4, 8, 20 
+
+ Deep SVDD, ICML, 2018, unsupervised, Deep One-Class Classification  
+ REPEN, KDD, 2018, unsupervised, Learning Representations of Ultrahigh-dimensional Data for Random Distance-based Outlier Detection
+ RDP, IJCAI, 2020, unsupervised, Unsupervised Representation Learning by Predicting Random Distances  
+ RCA, IJCAI, 2021, unsupervised, RCA: A Deep Collaborative Autoencoder Approach for Anomaly Detection
+ GOAD, ICLR, 2020, unsupervised, Classification-Based Anomaly Detection for General Data
+ NeuTraL, ICML, 2021, unsupervised, Neural Transformation Learning for Deep Anomaly Detection Beyond Images
+ ICL, ICLR, 2022, unsupervised, Anomaly Detection for Tabular Data with Internal Contrastive Learning
+ DIF, TKDE, 2023, unsupervised, Deep Isolation Forest for Anomaly Detection
+ SLAD, ICML, 2023, unsupervised, Fascinating Supervisory Signals and Where to Find Them: Deep Anomaly Detection with Scale Learning
+ DevNet, KDD, 2019, weakly-supervised, Deep Anomaly Detection with Deviation Networks
+ PReNet, KDD, 2023, weakly-supervised, Deep Weakly-supervised Anomaly Detection
+ Deep SAD, ICLR, 2020, weakly-supervised, Deep Semi-Supervised Anomaly Detection
+ FeaWAD, TNNLS, 2021, weakly-supervised, Feature Encoding with AutoEncoders for Weakly-supervised Anomaly Detection
+
+
+Usages
+~~~~~~~~~~~~~~~~~
+
+
+DeepOD can be used in a few lines of code. This API style is the same with sklearn and PyOD.
+
+
+.. code-block:: python
+
+
+    # unsupervised methods
+    from deepod.models.dsvdd import DeepSVDD
+    clf = DeepSVDD()
+    clf.fit(X_train, y=None)
+    scores = clf.decision_function(X_test)
+
+    # weakly-supervised methods
+    from deepod.models.devnet import DevNet
+    clf = DevNet()
+    clf.fit(X_train, y=semi_y) # semi_y uses 1 for known anomalies, and 0 for unlabeled data
+    scores = clf.decision_function(X_test)
+
+
+
+Citation
+~~~~~~~~~~~~~~~~~
+If you use this library in your work, please use the BibTex entry below for citation.
+
+.. code-block:: bibtex
+
+   @misc{deepod,
+      author = {{Xu, Hongzuo}},
+      title = {{DeepOD: Python Deep Outlier/Anomaly Detection}},
+      url = {https://github.com/xuhongzuo/DeepOD},
+      version = {0.2},
+   }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepod-0.2.0/deepod/core/__init__.py` & `deepod-0.3.0/deepod/core/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""
-The :mod:`pysad.core` module covers base classes of the `PySAD`.
-"""
-from .base_model import BaseDeepAD
-
-
-__all__ = ["BaseDeepAD"]
-
-# print("""
-# ╭━━━╮          ╭━━━╮ ╭━━━ ╮
-# ╰╮╭╮┃          ┃╭━╮┃ ╰╮╭ ╮┃
-#  ┃┃┃┣━━┳━━┳━━╮ ┃┃ ┃┃  ┃┃ ┃┃
-#  ┃┃┃┃┃━┫┃━┫╭╮┃ ┃┃ ┃┃  ┃┃ ┃┃
-# ╭╯╰╯┃┃━┫┃━┫╰╯┃ ┃╰━╯┃ ╭╯╯ ╰┃
-# ╰━━━┻━━┻━━┫╭━╯ ╰━━━╯ ╰━━━━╯
-#           ┃┃
-#           ╰╯
+"""
+The :mod:`pysad.core` module covers base classes of the `PySAD`.
+"""
+from .base_model import BaseDeepAD
+
+
+__all__ = ["BaseDeepAD"]
+
+# print("""
+# ╭━━━╮          ╭━━━╮ ╭━━━ ╮
+# ╰╮╭╮┃          ┃╭━╮┃ ╰╮╭ ╮┃
+#  ┃┃┃┣━━┳━━┳━━╮ ┃┃ ┃┃  ┃┃ ┃┃
+#  ┃┃┃┃┃━┫┃━┫╭╮┃ ┃┃ ┃┃  ┃┃ ┃┃
+# ╭╯╰╯┃┃━┫┃━┫╰╯┃ ┃╰━╯┃ ╭╯╯ ╰┃
+# ╰━━━┻━━┻━━┫╭━╯ ╰━━━╯ ╰━━━━╯
+#           ┃┃
+#           ╰╯
 # """)
```

### Comparing `deepod-0.2.0/deepod/core/base_model.py` & `deepod-0.3.0/deepod/core/base_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,362 +1,421 @@
-# -*- coding: utf-8 -*-
-"""
-Base class for deep Anomaly detection models
-some functions are adapted from the pyod library
-@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
-"""
-
-import numpy as np
-import torch
-import random
-import time
-from abc import ABCMeta, abstractmethod
-from scipy.stats import binom
-from sklearn.utils import check_array
-from sklearn.utils.validation import check_is_fitted
-
-
-class BaseDeepAD(metaclass=ABCMeta):
-    """
-    Abstract class for deep outlier detection models
-
-    Parameters
-    ----------
-
-    epochs: int, optional (default=100)
-        Number of training epochs
-
-    batch_size: int, optional (default=64)
-        Number of samples in a mini-batch
-
-    lr: float, optional (default=1e-3)
-        Learning rate
-
-    n_ensemble: int or str, optional (default=1)
-        Number of ensemble size
-
-    epoch_steps: int, optional (default=-1)
-        Maximum steps in an epoch
-            - If -1, all the batches will be processed
-
-    prt_steps: int, optional (default=10)
-        Number of epoch intervals per printing
-
-    device: str, optional (default='cuda')
-        torch device,
-
-    contamination : float in (0., 0.5), optional (default=0.1)
-        The amount of contamination of the data set,
-        i.e. the proportion of outliers in the data set. Used when fitting to
-        define the threshold on the decision function.
-
-    verbose: int, optional (default=1)
-        Verbosity mode
-
-    random_state： int, optional (default=42)
-        the seed used by the random
-
-    Attributes
-    ----------
-    decision_scores_ : numpy array of shape (n_samples,)
-        The outlier scores of the training data.
-        The higher, the more abnormal. Outliers tend to have higher
-        scores. This value is available once the detector is fitted.
-
-    threshold_ : float
-        The threshold is based on ``contamination``. It is the
-        ``n_samples * contamination`` most abnormal samples in
-        ``decision_scores_``. The threshold is calculated for generating
-        binary outlier labels.
-
-    labels_ : int, either 0 or 1
-        The binary labels of the training data. 0 stands for inliers
-        and 1 for outliers/anomalies. It is generated by applying
-        ``threshold_`` on ``decision_scores_``.
-
-    """
-    def __init__(self, model_name, epochs=100, batch_size=64, lr=1e-3,
-                 n_ensemble=1,
-                 epoch_steps=-1, prt_steps=10,
-                 device='cuda', contamination=0.1,
-                 verbose=1, random_state=42):
-        self.model_name = model_name
-
-        self.epochs = epochs
-        self.batch_size = batch_size
-        self.lr = lr
-
-        self.device = device
-        self.contamination = contamination
-
-        self.epoch_steps = epoch_steps
-        self.prt_steps = prt_steps
-        self.verbose = verbose
-
-        self.n_features = -1
-        self.n_samples = -1
-        self.criterion = None
-        self.net = None
-
-        self.n_ensemble = n_ensemble
-
-        self.train_loader = None
-        self.test_loader = None
-
-        self.epoch_time = None
-
-        self.train_data = None
-        self.train_label = None
-
-        self.decision_scores_ = None
-        self.labels_ = None
-        self.threshold_ = None
-
-        self.random_state = random_state
-        self.set_seed(random_state)
-        return
-
-    def fit(self, X, y=None):
-        """
-        Fit detector. y is ignored in unsupervised methods.
-
-        Parameters
-        ----------
-        X : numpy array of shape (n_samples, n_features)
-            The input samples.
-
-        y : numpy array of shape (n_samples, )
-            Not used in unsupervised methods, present for API consistency by convention.
-            used in (semi-/weakly-) supervised methods
-
-        Returns
-        -------
-        self : object
-            Fitted estimator.
-        """
-
-        self.train_data = X
-        self.train_label = y
-        self.n_samples, self.n_features = X.shape
-
-        if self.verbose >= 1:
-            print('Start Training...')
-
-        if self.n_ensemble == 'auto':
-            self.n_ensemble = int(np.floor(100 / (np.log(self.n_samples) + self.n_features)) + 1)
-        if self.verbose >= 1:
-            print(f'ensemble size: {self.n_ensemble}')
-
-        for _ in range(self.n_ensemble):
-            self.train_loader, self.net, self.criterion = self.training_prepare(X, y=y)
-            self._training()
-
-        if self.verbose >= 1:
-            print('Start Inference on the training data...')
-
-        self.decision_scores_ = self.decision_function(X)
-        self.labels_ = self._process_decision_scores()
-
-        return self
-
-    def decision_function(self, X):
-        """Predict raw anomaly scores of X using the fitted detector.
-
-        The anomaly score of an input sample is computed based on the fitted
-        detector. For consistency, outliers are assigned with
-        higher anomaly scores.
-
-        Parameters
-        ----------
-        X : numpy array of shape (n_samples, n_features)
-            The input samples. Sparse matrices are accepted only
-            if they are supported by the base estimator.
-
-        Returns
-        -------
-        anomaly_scores : numpy array of shape (n_samples,)
-            The anomaly score of the input samples.
-        """
-        testing_n_samples = X.shape[0]
-        s_final = np.zeros(testing_n_samples)
-        for _ in range(self.n_ensemble):
-            self.test_loader = self.inference_prepare(X)
-            z, scores = self._inference()
-            z, scores = self.decision_function_update(z, scores)
-            s_final += scores
-
-        return s_final
-
-    def predict(self, X, return_confidence=False):
-        """Predict if a particular sample is an outlier or not.
-
-        Parameters
-        ----------
-        X : numpy array of shape (n_samples, n_features)
-            The input samples.
-
-        return_confidence : boolean, optional(default=False)
-            If True, also return the confidence of prediction.
-
-        Returns
-        -------
-        outlier_labels : numpy array of shape (n_samples,)
-            For each observation, tells whether
-            it should be considered as an outlier according to the
-            fitted model. 0 stands for inliers and 1 for outliers.
-        confidence : numpy array of shape (n_samples,).
-            Only if return_confidence is set to True.
-        """
-
-        pred_score = self.decision_function(X)
-        prediction = (pred_score > self.threshold_).astype('int').ravel()
-
-        if return_confidence:
-            confidence = self._predict_confidence(pred_score)
-            return prediction, confidence
-
-        return prediction
-
-    def _predict_confidence(self, test_scores):
-        """Predict the model's confidence in making the same prediction
-        under slightly different training sets.
-        See :cite:`perini2020quantifying`.
-
-        Parameters
-        -------
-        test_scores : numpy array of shape (n_samples,)
-            The anomaly score of the input samples.
-
-        Returns
-        -------
-        confidence : numpy array of shape (n_samples,)
-            For each observation, tells how consistently the model would
-            make the same prediction if the training set was perturbed.
-            Return a probability, ranging in [0,1].
-
-        """
-        n = len(self.decision_scores_)
-
-        count_instances = np.vectorize(lambda x: np.count_nonzero(self.decision_scores_ <= x))
-        n_instances = count_instances(test_scores)
-
-        # Derive the outlier probability using Bayesian approach
-        posterior_prob = np.vectorize(lambda x: (1 + x) / (2 + n))(n_instances)
-
-        # Transform the outlier probability into a confidence value
-        confidence = np.vectorize(
-            lambda p: 1 - binom.cdf(n - int(n*self.contamination), n, p)
-        )(posterior_prob)
-        prediction = (test_scores > self.threshold_).astype('int').ravel()
-        np.place(confidence, prediction==0, 1-confidence[prediction == 0])
-        return confidence
-
-    def _process_decision_scores(self):
-        """Internal function to calculate key attributes:
-
-        - threshold_: used to decide the binary label
-        - labels_: binary labels of training data
-
-        Returns
-        -------
-        self
-        """
-
-        self.threshold_ = np.percentile(self.decision_scores_, 100 * (1 - self.contamination))
-        self.labels_ = (self.decision_scores_ > self.threshold_).astype('int').ravel()
-
-        self._mu = np.mean(self.decision_scores_)
-        self._sigma = np.std(self.decision_scores_)
-
-        return self
-
-
-    def _training(self):
-        optimizer = torch.optim.Adam(self.net.parameters(),
-                                     lr=self.lr,
-                                     weight_decay=1e-5)
-
-        self.net.train()
-        for i in range(self.epochs):
-            t1 = time.time()
-            total_loss = 0
-            cnt = 0
-            for batch_x in self.train_loader:
-                loss = self.training_forward(batch_x, self.net, self.criterion)
-                self.net.zero_grad()
-                loss.backward()
-                optimizer.step()
-
-                total_loss += loss.item()
-                cnt += 1
-
-                # terminate this epoch when reaching assigned maximum steps per epoch
-                if cnt > self.epoch_steps != -1:
-                    break
-
-            t = time.time() - t1
-            if self.verbose >= 1 and (i == 0 or (i+1) % self.prt_steps == 0):
-                print(f'epoch{i+1}, '
-                      f'training loss: {total_loss/cnt:.6f}, '
-                      f'time: {t:.1f}s')
-
-            if i == 0:
-                self.epoch_time = t
-
-            self.epoch_update()
-
-        return
-
-    def _inference(self):
-        self.net.eval()
-        with torch.no_grad():
-            z_lst = []
-            score_lst = []
-            for batch_x in self.test_loader:
-                batch_z, s = self.inference_forward(batch_x, self.net, self.criterion)
-
-                z_lst.append(batch_z)
-                score_lst.append(s)
-
-        z = torch.cat(z_lst).data.cpu().numpy()
-        scores = torch.cat(score_lst).data.cpu().numpy()
-
-        return z, scores
-
-    @abstractmethod
-    def training_forward(self, batch_x, net, criterion):
-        """define forward step in training"""
-        pass
-
-    @abstractmethod
-    def inference_forward(self, batch_x, net, criterion):
-        """define forward step in inference"""
-        pass
-
-    @abstractmethod
-    def training_prepare(self, X, y):
-        """define train_loader, net, and criterion"""
-        pass
-
-    @abstractmethod
-    def inference_prepare(self, X):
-        """define test_loader"""
-        pass
-
-    def epoch_update(self):
-        """for any updating operation after each training epoch"""
-        return
-
-    def decision_function_update(self, z, scores):
-        """for any updating operation after decision function"""
-        return z, scores
-
-
-    @staticmethod
-    def set_seed(seed):
-        torch.manual_seed(seed)
-        torch.cuda.manual_seed(seed)
-        torch.cuda.manual_seed_all(seed)
-        np.random.seed(seed)
-        random.seed(seed)
-        torch.backends.cudnn.benchmark = False
-        torch.backends.cudnn.deterministic = True
+# -*- coding: utf-8 -*-
+"""
+Base class for deep Anomaly detection models
+some functions are adapted from the pyod library
+@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
+"""
+
+import numpy as np
+import torch
+import random
+import time
+from abc import ABCMeta, abstractmethod
+from scipy.stats import binom
+from deepod.utils.utility import get_sub_seqs, get_sub_seqs_label
+from deepod.core.base_networks import sequential_net_name
+from sklearn.utils import check_array
+from sklearn.utils.validation import check_is_fitted
+from tqdm import tqdm
+
+
+class BaseDeepAD(metaclass=ABCMeta):
+    """
+    Abstract class for deep outlier detection models
+
+    Parameters
+    ----------
+
+    data_type: str, optional (default='tabular')
+        Data type, choice = ['tabular', 'ts']
+
+    network: str, optional (default='MLP')
+        network structure for different data structures
+
+    epochs: int, optional (default=100)
+        Number of training epochs
+
+    batch_size: int, optional (default=64)
+        Number of samples in a mini-batch
+
+    lr: float, optional (default=1e-3)
+        Learning rate
+
+    n_ensemble: int or str, optional (default=1)
+        Number of ensemble size
+
+    seq_len: int, optional (default=100)
+        Size of window used to create subsequences from the data
+        deprecated when handling tabular data (network=='MLP')
+
+    stride: int, optional (default=1)
+        number of time points the window will move between two subsequences
+        deprecated when handling tabular data (network=='MLP')
+
+    epoch_steps: int, optional (default=-1)
+        Maximum steps in an epoch
+            - If -1, all the batches will be processed
+
+    prt_steps: int, optional (default=10)
+        Number of epoch intervals per printing
+
+    device: str, optional (default='cuda')
+        torch device,
+
+    contamination : float in (0., 0.5), optional (default=0.1)
+        The amount of contamination of the data set,
+        i.e. the proportion of outliers in the data set. Used when fitting to
+        define the threshold on the decision function.
+
+    verbose: int, optional (default=1)
+        Verbosity mode
+
+    random_state： int, optional (default=42)
+        the seed used by the random
+
+    Attributes
+    ----------
+    decision_scores_ : numpy array of shape (n_samples,)
+        The outlier scores of the training data.
+        The higher, the more abnormal. Outliers tend to have higher
+        scores. This value is available once the detector is fitted.
+
+    threshold_ : float
+        The threshold is based on ``contamination``. It is the
+        ``n_samples * contamination`` most abnormal samples in
+        ``decision_scores_``. The threshold is calculated for generating
+        binary outlier labels.
+
+    labels_ : int, either 0 or 1
+        The binary labels of the training data. 0 stands for inliers
+        and 1 for outliers/anomalies. It is generated by applying
+        ``threshold_`` on ``decision_scores_``.
+
+    """
+    def __init__(self, model_name, data_type='tabular', network='MLP',
+                 epochs=100, batch_size=64, lr=1e-3,
+                 n_ensemble=1, seq_len=100, stride=1,
+                 epoch_steps=-1, prt_steps=10,
+                 device='cuda', contamination=0.1,
+                 verbose=1, random_state=42):
+        self.model_name = model_name
+
+        self.data_type = data_type
+        self.network = network
+
+        if data_type == 'ts':
+            assert self.network in sequential_net_name, \
+                'Assigned network cannot handle time-series data'
+
+        self.seq_len = seq_len
+        self.stride = stride
+
+        self.epochs = epochs
+        self.batch_size = batch_size
+        self.lr = lr
+
+        self.device = device
+        self.contamination = contamination
+
+        self.epoch_steps = epoch_steps
+        self.prt_steps = prt_steps
+        self.verbose = verbose
+
+        self.n_features = -1
+        self.n_samples = -1
+        self.criterion = None
+        self.net = None
+
+        self.n_ensemble = n_ensemble
+
+        self.train_loader = None
+        self.test_loader = None
+
+        self.epoch_time = None
+
+        self.train_data = None
+        self.train_label = None
+
+        self.decision_scores_ = None
+        self.labels_ = None
+        self.threshold_ = None
+
+        self.random_state = random_state
+        self.set_seed(random_state)
+        return
+
+    def fit(self, X, y=None):
+        """
+        Fit detector. y is ignored in unsupervised methods.
+
+        Parameters
+        ----------
+        X : numpy array of shape (n_samples, n_features)
+            The input samples.
+
+        y : numpy array of shape (n_samples, )
+            Not used in unsupervised methods, present for API consistency by convention.
+            used in (semi-/weakly-) supervised methods
+
+        Returns
+        -------
+        self : object
+            Fitted estimator.
+        """
+
+        if self.data_type == 'ts':
+            X_seqs = get_sub_seqs(X, seq_len=self.seq_len, stride=self.stride)
+            y_seqs = get_sub_seqs_label(y, seq_len=self.seq_len, stride=self.stride) if y is not None else None
+            self.train_data = X_seqs
+            self.train_label = y_seqs
+            self.n_samples, self.n_features = X_seqs.shape[0], X_seqs.shape[2]
+        else:
+            self.train_data = X
+            self.train_label = y
+            self.n_samples, self.n_features = X.shape
+
+        if self.verbose >= 1:
+            print('Start Training...')
+
+        if self.n_ensemble == 'auto':
+            self.n_ensemble = int(np.floor(100 / (np.log(self.n_samples) + self.n_features)) + 1)
+        if self.verbose >= 1:
+            print(f'ensemble size: {self.n_ensemble}')
+
+        for _ in range(self.n_ensemble):
+            self.train_loader, self.net, self.criterion = self.training_prepare(self.train_data,
+                                                                                y=self.train_label)
+            self._training()
+
+        if self.verbose >= 1:
+            print('Start Inference on the training data...')
+
+        self.decision_scores_ = self.decision_function(X)
+        self.labels_ = self._process_decision_scores()
+
+        return self
+
+    def decision_function(self, X, return_rep=False):
+        """Predict raw anomaly scores of X using the fitted detector.
+
+        The anomaly score of an input sample is computed based on the fitted
+        detector. For consistency, outliers are assigned with
+        higher anomaly scores.
+
+        Parameters
+        ----------
+        X : numpy array of shape (n_samples, n_features)
+            The input samples. Sparse matrices are accepted only
+            if they are supported by the base estimator.
+
+        return_rep: boolean, optional, default=False
+            whether return representations
+
+        Returns
+        -------
+        anomaly_scores : numpy array of shape (n_samples,)
+            The anomaly score of the input samples.
+        """
+
+        testing_n_samples = X.shape[0]
+
+        if self.data_type == 'ts':
+            X = get_sub_seqs(X, seq_len=self.seq_len, stride=1)
+
+        representations = []
+        s_final = np.zeros(testing_n_samples)
+        for _ in range(self.n_ensemble):
+            self.test_loader = self.inference_prepare(X)
+
+            z, scores = self._inference()
+            z, scores = self.decision_function_update(z, scores)
+
+            if self.data_type == 'ts':
+                padding = np.zeros(self.seq_len-1)
+                scores = np.hstack((padding, scores))
+
+            s_final += scores
+            representations.extend(z)
+        representations = np.array(representations)
+
+        if return_rep:
+            return s_final, representations
+        else:
+            return s_final
+
+    def predict(self, X, return_confidence=False):
+        """Predict if a particular sample is an outlier or not.
+
+        Parameters
+        ----------
+        X : numpy array of shape (n_samples, n_features)
+            The input samples.
+
+        return_confidence : boolean, optional(default=False)
+            If True, also return the confidence of prediction.
+
+        Returns
+        -------
+        outlier_labels : numpy array of shape (n_samples,)
+            For each observation, tells whether
+            it should be considered as an outlier according to the
+            fitted model. 0 stands for inliers and 1 for outliers.
+        confidence : numpy array of shape (n_samples,).
+            Only if return_confidence is set to True.
+        """
+
+        pred_score = self.decision_function(X)
+        prediction = (pred_score > self.threshold_).astype('int').ravel()
+
+        if return_confidence:
+            confidence = self._predict_confidence(pred_score)
+            return prediction, confidence
+
+        return prediction
+
+    def _predict_confidence(self, test_scores):
+        """Predict the model's confidence in making the same prediction
+        under slightly different training sets.
+        See :cite:`perini2020quantifying`.
+
+        Parameters
+        -------
+        test_scores : numpy array of shape (n_samples,)
+            The anomaly score of the input samples.
+
+        Returns
+        -------
+        confidence : numpy array of shape (n_samples,)
+            For each observation, tells how consistently the model would
+            make the same prediction if the training set was perturbed.
+            Return a probability, ranging in [0,1].
+
+        """
+        n = len(self.decision_scores_)
+
+        count_instances = np.vectorize(lambda x: np.count_nonzero(self.decision_scores_ <= x))
+        n_instances = count_instances(test_scores)
+
+        # Derive the outlier probability using Bayesian approach
+        posterior_prob = np.vectorize(lambda x: (1 + x) / (2 + n))(n_instances)
+
+        # Transform the outlier probability into a confidence value
+        confidence = np.vectorize(
+            lambda p: 1 - binom.cdf(n - int(n*self.contamination), n, p)
+        )(posterior_prob)
+        prediction = (test_scores > self.threshold_).astype('int').ravel()
+        np.place(confidence, prediction==0, 1-confidence[prediction == 0])
+        return confidence
+
+    def _process_decision_scores(self):
+        """Internal function to calculate key attributes:
+
+        - threshold_: used to decide the binary label
+        - labels_: binary labels of training data
+
+        Returns
+        -------
+        self
+        """
+
+        self.threshold_ = np.percentile(self.decision_scores_, 100 * (1 - self.contamination))
+        self.labels_ = (self.decision_scores_ > self.threshold_).astype('int').ravel()
+
+        self._mu = np.mean(self.decision_scores_)
+        self._sigma = np.std(self.decision_scores_)
+
+        return self
+
+    def _training(self):
+        optimizer = torch.optim.Adam(self.net.parameters(),
+                                     lr=self.lr,
+                                     weight_decay=1e-5)
+
+        self.net.train()
+        for i in range(self.epochs):
+            t1 = time.time()
+            total_loss = 0
+            cnt = 0
+            for batch_x in self.train_loader:
+                loss = self.training_forward(batch_x, self.net, self.criterion)
+                self.net.zero_grad()
+                loss.backward()
+                optimizer.step()
+
+                total_loss += loss.item()
+                cnt += 1
+
+                # terminate this epoch when reaching assigned maximum steps per epoch
+                if cnt > self.epoch_steps != -1:
+                    break
+
+            t = time.time() - t1
+            if self.verbose >= 1 and (i == 0 or (i+1) % self.prt_steps == 0):
+                print(f'epoch{i+1:3d}, '
+                      f'training loss: {total_loss/cnt:.6f}, '
+                      f'time: {t:.1f}s')
+
+            if i == 0:
+                self.epoch_time = t
+
+            self.epoch_update()
+
+        return
+
+    def _inference(self):
+        self.net.eval()
+        with torch.no_grad():
+            z_lst = []
+            score_lst = []
+
+            if self.verbose >= 2:
+                _iter_ = tqdm(self.test_loader, desc='testing: ')
+            else:
+                _iter_ = self.test_loader
+
+            for batch_x in _iter_:
+                batch_z, s = self.inference_forward(batch_x, self.net, self.criterion)
+                z_lst.append(batch_z)
+                score_lst.append(s)
+
+        z = torch.cat(z_lst).data.cpu().numpy()
+        scores = torch.cat(score_lst).data.cpu().numpy()
+
+        return z, scores
+
+    @abstractmethod
+    def training_forward(self, batch_x, net, criterion):
+        """define forward step in training"""
+        pass
+
+    @abstractmethod
+    def inference_forward(self, batch_x, net, criterion):
+        """define forward step in inference"""
+        pass
+
+    @abstractmethod
+    def training_prepare(self, X, y):
+        """define train_loader, net, and criterion"""
+        pass
+
+    @abstractmethod
+    def inference_prepare(self, X):
+        """define test_loader"""
+        pass
+
+    def epoch_update(self):
+        """for any updating operation after each training epoch"""
+        return
+
+    def decision_function_update(self, z, scores):
+        """for any updating operation after decision function"""
+        return z, scores
+
+    @staticmethod
+    def set_seed(seed):
+        torch.manual_seed(seed)
+        torch.cuda.manual_seed(seed)
+        torch.cuda.manual_seed_all(seed)
+        np.random.seed(seed)
+        random.seed(seed)
+        # torch.backends.cudnn.benchmark = False
+        # torch.backends.cudnn.deterministic = True
```

### Comparing `deepod-0.2.0/deepod/model_selection/fmms.py` & `deepod-0.3.0/deepod/model_selection/fmms.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,243 +1,243 @@
-# -*- coding: utf-8 -*-
-"""
-Factorization Machine-based Unsupervised Model Selection Method
-@Author: Ruyi Zhang & Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
-"""
-
-import torch
-import torch.utils.data as Data
-import numpy as np
-from deepod.model_selection.gene_feature import generate_meta_features
-from sklearn.model_selection import train_test_split
-
-
-class FMMS:
-    def __init__(self, embedding_size=4, batch=4, lr=0.001, epoch=50,
-                 prt_steps=10, verbose=1, random_state=0):
-        """
-        Factorization Machine-based Unsupervised Model Selection Method.
-        FMMS is trained by historical performance on a large suite of data collection
-        and the characteristics of these datasets. Fitted FMMS can be used to
-        recommend more suitable detection model on new datasets according to
-        their characteristics.
-
-        Parameters
-        ----------
-
-        embedding_size: int, optional (default=4)
-            The dimension of the auxiliary vector
-
-        batch: int, optional (default=4)
-            Batch size
-
-        lr: float, optional (default=0.001)
-            Learning rate
-
-        epoch: int, optional (default=50)
-            Training epoch
-
-        verbose: int, optional (default=1)
-            Verbosity mode
-
-        prt_steps: int, optional (default=10)
-            Number of epoch intervals per printing
-
-        random_state: int, optional (default=0)
-            Random statement
-
-        """
-
-        self.embedding_size = embedding_size
-        self.batch = batch
-        self.lr = lr
-        self.epoch = epoch
-        self.random_state = random_state
-
-        self.verbose = verbose
-        self.prt_steps = prt_steps
-
-        self.net = None
-        self.model_size = None
-        self.feature_size = None
-
-        return
-
-    def fit(self, Fmap, Pmap, save_path=None):
-        """
-        Fit model selection model.
-
-        Parameters
-        ----------
-
-        Fmap: np.array (D*F), required
-            The feature Map of the historical dataset.
-
-        Pmap: np.array (M*D), required
-            The performance of the candidate models on the historical dataset.
-
-        save_path: str, optional (default=None)
-            The location where the trained model is stored.
-
-        Returns
-        -------
-        self : object
-            Fitted estimator.
-        """
-        self.feature_size = Fmap.shape[1]
-        self.model_size = Pmap.shape[1]
-
-        f_train, f_valid, p_train, p_valid = train_test_split(Fmap, Pmap, test_size=0.2,
-                                                              random_state=self.random_state)
-        f_valid = torch.from_numpy(f_valid)
-        p_valid = torch.from_numpy(p_valid)
-
-        self.net = FMMSNet(feature_size=self.feature_size, model_size=self.model_size,
-                           embedding_size=self.embedding_size)
-
-        train_dataset = Data.TensorDataset(torch.tensor(f_train), torch.tensor(p_train))
-        loader = Data.DataLoader(
-            dataset=train_dataset,
-            batch_size=self.batch,
-            shuffle=False
-        )
-
-        optimizer = torch.optim.Adam(self.net.parameters(), lr=self.lr, weight_decay=1e-5)
-        loss_valid_set = []
-        np_ctr = 1
-
-        total_loss = 0.
-        cnt = 0
-        for i in range(self.epoch):
-            # early stop
-            if f_valid is not None:
-                if i >= 2 and (loss_valid_set[-2] - loss_valid_set[-1]) / loss_valid_set[-1] <= 0.001:
-                    np_ctr += 1
-                else:
-                    np_ctr = 1
-                if np_ctr > 5:
-                    break
-
-            for step, (batch_x, batch_y) in enumerate(loader):
-                optimizer.zero_grad()
-                output = self.net(batch_x)
-                loss_train = self.cos_loss(output, batch_y)
-
-                # @TODO: seems not used
-                l2_regularization = torch.tensor(0).float()
-                for param in self.net.parameters():
-                    l2_regularization += torch.norm(param, 2)
-
-                loss_train.backward()
-                optimizer.step()
-
-                total_loss += loss_train.item()
-                cnt += 1
-
-            # validation phase
-            valid_output = self.net(f_valid)
-            loss_valid = self.cos_loss(valid_output, p_valid)
-            loss_valid_set.append(loss_valid.item())
-
-            if self.verbose >= 1 and (i == 0 or (i+1) % self.prt_steps == 0):
-                print(f'epoch {i+1:3d}, '
-                      f'training loss: {total_loss / cnt:.6f}, ')
-
-        # save trained models
-        if save_path is not None:
-            torch.save(self.net, save_path)
-
-        return self
-
-    def predict(self, x=None, f=None, topn=5, load_path=None):
-        """
-
-        Parameters
-        ----------
-        x: np.array, optional (default=None)
-            Target dataset
-
-        f: np.array, optional (default=None)
-            Features of the target dataset, x and f should be
-
-        topn: int, optional (default=5)
-            Number of the recommended models
-
-        load_path: str, optional (default=None)
-
-        Returns
-        -------
-
-        """
-        if load_path is not None:
-            self.net = torch.load(load_path)
-            self.feature_size = self.net.feature_size
-            self.model_size = self.net.embedding_size
-
-        if f is None and x is None:
-            raise AttributeError('Either x or f should be fitted.')
-        if f is not None and x is not None:
-            raise Warning('f is deprecated by re-generate features from the target dataset x')
-
-        if x is not None:
-            f = generate_meta_features(x)[0]
-
-        assert f.shape[1] == self.feature_size, \
-            f'The feature size of historical dataset ({f.shape[0]}) ' \
-            f'and target dataset ({self.feature_size}) does not match'
-
-        pred = self.net(torch.tensor(f))
-        pred = pred.detach().numpy()[0]
-        ranking = np.argsort(pred)  # ranking
-
-        recommend = ranking[::-1]
-        # @TODO return the ranking of model names
-        print(f"Predicted Top {topn} better models are {recommend[:topn]}")
-
-        return
-
-    @staticmethod
-    def cos_loss(pred, real):
-        # pred = pred.type(torch.DoubleTensor)
-        # real = torch.tensor(real).double()
-        pred = pred.double()
-        real = real.double()
-
-        mul = pred * real
-        mul = torch.sum(mul, dim=1)
-        length = torch.norm(pred, p=2, dim=1) * torch.norm(real, p=2, dim=1)
-        loss = 1 - mul / length
-        loss = sum(loss) / len(pred)
-        return loss
-
-
-class FMMSNet(torch.nn.Module):
-    def __init__(self, feature_size, model_size, embedding_size):
-        super(FMMSNet, self).__init__()
-        self.feature_size = feature_size  # denote as F, the size of the feature dictionary
-        self.embedding_size = embedding_size  # denote as K, the size of the feature embedding
-        self.model_size = model_size  # denote as M, the size of the model list
-        self.linear = torch.nn.Sequential(torch.nn.Linear(self.feature_size, self.model_size, bias=True))
-        self.weight = torch.nn.Parameter(torch.rand(self.embedding_size, self.feature_size, self.model_size))
-
-    def forward(self, x):
-        # FM part
-        outFM = self.linear(x.clone().detach().float())
-        for i in range(self.embedding_size):
-            v = self.weight[i]
-            xv = torch.mm(x.clone().detach().float(), v)
-            xv2 = torch.pow(xv, 2)
-
-            z = torch.pow(x.clone().detach().float(), 2)
-            P = torch.pow(v, 2)
-            zp = torch.mm(z, P)
-
-            outFM = outFM + (xv2 - zp) / 2
-        out = outFM
-        return out
-
-    def show(self):
-        for parameters in self.parameters():
-            print(parameters)
-
-        for name, parameters in self.named_parameters():
-            print(name, ':', parameters.size())
+# -*- coding: utf-8 -*-
+"""
+Factorization Machine-based Unsupervised Model Selection Method
+@Author: Ruyi Zhang & Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
+"""
+
+import torch
+import torch.utils.data as Data
+import numpy as np
+from deepod.model_selection.gene_feature import generate_meta_features
+from sklearn.model_selection import train_test_split
+
+
+class FMMS:
+    def __init__(self, embedding_size=4, batch=4, lr=0.001, epoch=50,
+                 prt_steps=10, verbose=1, random_state=0):
+        """
+        Factorization Machine-based Unsupervised Model Selection Method.
+        FMMS is trained by historical performance on a large suite of data collection
+        and the characteristics of these datasets. Fitted FMMS can be used to
+        recommend more suitable detection model on new datasets according to
+        their characteristics.
+
+        Parameters
+        ----------
+
+        embedding_size: int, optional (default=4)
+            The dimension of the auxiliary vector
+
+        batch: int, optional (default=4)
+            Batch size
+
+        lr: float, optional (default=0.001)
+            Learning rate
+
+        epoch: int, optional (default=50)
+            Training epoch
+
+        verbose: int, optional (default=1)
+            Verbosity mode
+
+        prt_steps: int, optional (default=10)
+            Number of epoch intervals per printing
+
+        random_state: int, optional (default=0)
+            Random statement
+
+        """
+
+        self.embedding_size = embedding_size
+        self.batch = batch
+        self.lr = lr
+        self.epoch = epoch
+        self.random_state = random_state
+
+        self.verbose = verbose
+        self.prt_steps = prt_steps
+
+        self.net = None
+        self.model_size = None
+        self.feature_size = None
+
+        return
+
+    def fit(self, Fmap, Pmap, save_path=None):
+        """
+        Fit model selection model.
+
+        Parameters
+        ----------
+
+        Fmap: np.array (D*F), required
+            The feature Map of the historical dataset.
+
+        Pmap: np.array (M*D), required
+            The performance of the candidate models on the historical dataset.
+
+        save_path: str, optional (default=None)
+            The location where the trained model is stored.
+
+        Returns
+        -------
+        self : object
+            Fitted estimator.
+        """
+        self.feature_size = Fmap.shape[1]
+        self.model_size = Pmap.shape[1]
+
+        f_train, f_valid, p_train, p_valid = train_test_split(Fmap, Pmap, test_size=0.2,
+                                                              random_state=self.random_state)
+        f_valid = torch.from_numpy(f_valid)
+        p_valid = torch.from_numpy(p_valid)
+
+        self.net = FMMSNet(feature_size=self.feature_size, model_size=self.model_size,
+                           embedding_size=self.embedding_size)
+
+        train_dataset = Data.TensorDataset(torch.tensor(f_train), torch.tensor(p_train))
+        loader = Data.DataLoader(
+            dataset=train_dataset,
+            batch_size=self.batch,
+            shuffle=False
+        )
+
+        optimizer = torch.optim.Adam(self.net.parameters(), lr=self.lr, weight_decay=1e-5)
+        loss_valid_set = []
+        np_ctr = 1
+
+        total_loss = 0.
+        cnt = 0
+        for i in range(self.epoch):
+            # early stop
+            if f_valid is not None:
+                if i >= 2 and (loss_valid_set[-2] - loss_valid_set[-1]) / loss_valid_set[-1] <= 0.001:
+                    np_ctr += 1
+                else:
+                    np_ctr = 1
+                if np_ctr > 5:
+                    break
+
+            for step, (batch_x, batch_y) in enumerate(loader):
+                optimizer.zero_grad()
+                output = self.net(batch_x)
+                loss_train = self.cos_loss(output, batch_y)
+
+                # @TODO: seems not used
+                l2_regularization = torch.tensor(0).float()
+                for param in self.net.parameters():
+                    l2_regularization += torch.norm(param, 2)
+
+                loss_train.backward()
+                optimizer.step()
+
+                total_loss += loss_train.item()
+                cnt += 1
+
+            # validation phase
+            valid_output = self.net(f_valid)
+            loss_valid = self.cos_loss(valid_output, p_valid)
+            loss_valid_set.append(loss_valid.item())
+
+            if self.verbose >= 1 and (i == 0 or (i+1) % self.prt_steps == 0):
+                print(f'epoch {i+1:3d}, '
+                      f'training loss: {total_loss / cnt:.6f}, ')
+
+        # save trained models
+        if save_path is not None:
+            torch.save(self.net, save_path)
+
+        return self
+
+    def predict(self, x=None, f=None, topn=5, load_path=None):
+        """
+
+        Parameters
+        ----------
+        x: np.array, optional (default=None)
+            Target dataset
+
+        f: np.array, optional (default=None)
+            Features of the target dataset, x and f should be
+
+        topn: int, optional (default=5)
+            Number of the recommended models
+
+        load_path: str, optional (default=None)
+
+        Returns
+        -------
+
+        """
+        if load_path is not None:
+            self.net = torch.load(load_path)
+            self.feature_size = self.net.feature_size
+            self.model_size = self.net.embedding_size
+
+        if f is None and x is None:
+            raise AttributeError('Either x or f should be fitted.')
+        if f is not None and x is not None:
+            raise Warning('f is deprecated by re-generate features from the target dataset x')
+
+        if x is not None:
+            f = generate_meta_features(x)[0]
+
+        assert f.shape[1] == self.feature_size, \
+            f'The feature size of historical dataset ({f.shape[0]}) ' \
+            f'and target dataset ({self.feature_size}) does not match'
+
+        pred = self.net(torch.tensor(f))
+        pred = pred.detach().numpy()[0]
+        ranking = np.argsort(pred)  # ranking
+
+        recommend = ranking[::-1]
+        # @TODO return the ranking of model names
+        print(f"Predicted Top {topn} better models are {recommend[:topn]}")
+
+        return
+
+    @staticmethod
+    def cos_loss(pred, real):
+        # pred = pred.type(torch.DoubleTensor)
+        # real = torch.tensor(real).double()
+        pred = pred.double()
+        real = real.double()
+
+        mul = pred * real
+        mul = torch.sum(mul, dim=1)
+        length = torch.norm(pred, p=2, dim=1) * torch.norm(real, p=2, dim=1)
+        loss = 1 - mul / length
+        loss = sum(loss) / len(pred)
+        return loss
+
+
+class FMMSNet(torch.nn.Module):
+    def __init__(self, feature_size, model_size, embedding_size):
+        super(FMMSNet, self).__init__()
+        self.feature_size = feature_size  # denote as F, the size of the feature dictionary
+        self.embedding_size = embedding_size  # denote as K, the size of the feature embedding
+        self.model_size = model_size  # denote as M, the size of the model list
+        self.linear = torch.nn.Sequential(torch.nn.Linear(self.feature_size, self.model_size, bias=True))
+        self.weight = torch.nn.Parameter(torch.rand(self.embedding_size, self.feature_size, self.model_size))
+
+    def forward(self, x):
+        # FM part
+        outFM = self.linear(x.clone().detach().float())
+        for i in range(self.embedding_size):
+            v = self.weight[i]
+            xv = torch.mm(x.clone().detach().float(), v)
+            xv2 = torch.pow(xv, 2)
+
+            z = torch.pow(x.clone().detach().float(), 2)
+            P = torch.pow(v, 2)
+            zp = torch.mm(z, P)
+
+            outFM = outFM + (xv2 - zp) / 2
+        out = outFM
+        return out
+
+    def show(self):
+        for parameters in self.parameters():
+            print(parameters)
+
+        for name, parameters in self.named_parameters():
+            print(name, ':', parameters.size())
```

### Comparing `deepod-0.2.0/deepod/model_selection/gene_feature.py` & `deepod-0.3.0/deepod/model_selection/gene_feature.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,406 +1,406 @@
-# -*- coding: utf-8 -*-
-"""Generate meta-features from an arbitrary dataset.
-"""
-# Author: Yue Zhao <zhaoy@cmu.edu>
-# License: BSD 2 clause
-
-
-import pandas as pd
-import numpy as np
-import itertools
-
-from sklearn.decomposition import PCA as sklearn_PCA
-from scipy.stats import skew, kurtosis
-from scipy.stats import f_oneway
-from scipy.stats import entropy
-
-from scipy.stats import moment
-from scipy.stats import normaltest
-
-# from pyod.models.hbos import HBOS
-# from pyod.models.iforest import IForest
-# from pyod.models.pca import PCA
-# from pyod.models.loda import LODA
-from sklearn.utils import check_array
-
-
-def gini(array):
-    """Calculate the Gini coefficient of a numpy array."""
-    # based on bottom eq:
-    # http://www.statsdirect.com/help/generatedimages/equations/equation154.svg
-    # from:
-    # http://www.statsdirect.com/help/default.htm#nonparametric_methods/gini.htm
-    # All values are treated equally, arrays must be 1d:
-    array = array.flatten()
-    if np.amin(array) < 0:
-        # Values cannot be negative:
-        array -= np.amin(array)
-    # Values cannot be 0:
-    array = np.add(array, 0.0000001, casting="unsafe")
-    # Values must be sorted:
-    array = np.sort(array)
-    # Index per array element:
-    index = np.arange(1, array.shape[0] + 1)
-    # Number of array elements:
-    n = array.shape[0]
-    # Gini coefficient:
-    return ((np.sum((2 * index - n - 1) * array)) / (n * np.sum(array)))
-
-
-def Diff(li1, li2):
-    """Calculate the difference of two list
-
-    Parameters
-    ----------
-    li1
-    li2
-
-    Returns
-    -------
-
-    """
-    return (list(set(li1) - set(li2)))
-
-
-def argmaxn(w, nth):
-    w = np.asarray(w).ravel()
-    t = np.argsort(w)
-    return t[-1 * nth]
-
-
-def flatten_diagonally(x, diags=None):
-    diags = np.array(diags)
-    if x.shape[1] > x.shape[0]:
-        diags += x.shape[1] - x.shape[0]
-    n = max(x.shape)
-    ndiags = 2 * n - 1
-    i, j = np.indices(x.shape)
-    d = np.array([])
-    for ndi in range(ndiags):
-        if diags != None:
-            if not ndi in diags:
-                continue
-        d = np.concatenate((d, x[i == j + (n - 1) - ndi]))
-    return d
-
-
-def list_process(x, r_min=True, r_max=True, r_mean=True, r_std=True,
-                 r_skew=True, r_kurtosis=True):
-    """Return statistics of a list
-
-    Parameters
-    ----------
-    x
-    r_min
-    r_max
-    r_mean
-    r_std
-    r_skew
-    r_kurtosis
-
-    Returns
-    -------
-
-    """
-    x = np.asarray(x).reshape(-1, 1)
-    return_list = []
-
-    if r_min:
-        return_list.append(np.nanmin(x))
-
-    if r_max:
-        return_list.append(np.nanmax(x))
-
-    if r_mean:
-        return_list.append(np.nanmean(x))
-
-    if r_std:
-        return_list.append(np.nanstd(x))
-
-    if r_skew:
-        return_list.append(skew(x, nan_policy='omit')[0])
-
-    if r_kurtosis:
-        return_list.append(kurtosis(x, nan_policy='omit')[0])
-
-    return return_list
-
-
-def list_process_name(var):
-    return [var + '_min', var + '_max', var + '_mean', var + '_std',
-            var + '_skewness', var + '_kurtosis']
-
-
-def generate_meta_features(X):
-    """Get the meta-features of a datasets X
-
-    Parameters
-    ----------
-    X : numpy array of shape (n_samples, n_features)
-        Input array
-
-    Returns
-    -------
-    meta_features : numpy array of shape (1, 200)
-        Meta-feature in dimension of 200
-
-    """
-    # outliers_fraction = np.count_nonzero(y) / len(y)
-    # outliers_percentage = round(outliers_fraction * 100, ndigits=4)
-    X = check_array(X)
-
-    meta_vec = []
-    meta_vec_names = []
-
-    # on the sample level
-    n_samples, n_features = X.shape[0], X.shape[1]
-
-    meta_vec.append(n_samples)
-    meta_vec.append(n_features)
-
-    meta_vec_names.append('n_samples')
-    meta_vec_names.append('n_features')
-
-    sample_mean = np.mean(X)
-    sample_median = np.median(X)
-    sample_var = np.var(X)
-    sample_min = np.min(X)
-    sample_max = np.max(X)
-    sample_std = np.std(X)
-
-    q1, q25, q75, q99 = np.percentile(X, [0.01, 0.25, 0.75, 0.99])
-    iqr = q75 - q25
-
-    normalized_mean = sample_mean / sample_max
-    normalized_median = sample_median / sample_max
-    sample_range = sample_max - sample_min
-    sample_gini = gini(X)
-    med_abs_dev = np.median(np.absolute(X - sample_median))
-    avg_abs_dev = np.mean(np.absolute(X - sample_mean))
-    quant_coeff_disp = (q75 - q25) / (q75 + q25)
-    coeff_var = sample_var / sample_mean
-
-    outliers_15iqr = np.logical_or(
-        X < (q25 - 1.5 * iqr), X > (q75 + 1.5 * iqr))
-    outliers_3iqr = np.logical_or(X < (q25 - 3 * iqr), X > (q75 + 3 * iqr))
-    outliers_1_99 = np.logical_or(X < q1, X > q99)
-    outliers_3std = np.logical_or(X < (sample_mean - 3 * sample_std),
-                                  X > (sample_mean + 3 * sample_std))
-
-    percent_outliers_15iqr = np.sum(outliers_15iqr) / len(X)
-    percent_outliers_3iqr = np.sum(outliers_3iqr) / len(X)
-    percent_outliers_1_99 = np.sum(outliers_1_99) / len(X)
-    percent_outliers_3std = np.sum(outliers_3std) / len(X)
-
-    has_outliers_15iqr = np.any(outliers_15iqr).astype(int)
-    has_outliers_3iqr = np.any(outliers_3iqr).astype(int)
-    has_outliers_1_99 = np.any(outliers_1_99).astype(int)
-    has_outliers_3std = np.any(outliers_3std).astype(int)
-
-    meta_vec.extend(
-        [sample_mean, sample_median, sample_var, sample_min, sample_max,
-         sample_std,
-         q1, q25, q75, q99, iqr, normalized_mean, normalized_median,
-         sample_range, sample_gini,
-         med_abs_dev, avg_abs_dev, quant_coeff_disp, coeff_var,
-         # moment_5, moment_6, moment_7, moment_8, moment_9, moment_10,
-         percent_outliers_15iqr, percent_outliers_3iqr, percent_outliers_1_99,
-         percent_outliers_3std,
-         has_outliers_15iqr, has_outliers_3iqr, has_outliers_1_99,
-         has_outliers_3std])
-
-    meta_vec_names.extend(
-        ['sample_mean', 'sample_median', 'sample_var', 'sample_min',
-         'sample_max', 'sample_std',
-         'q1', 'q25', 'q75', 'q99', 'iqr', 'normalized_mean',
-         'normalized_median', 'sample_range', 'sample_gini',
-         'med_abs_dev', 'avg_abs_dev', 'quant_coeff_disp', 'coeff_var',
-         # moment_5, moment_6, moment_7, moment_8, moment_9, moment_10,
-         'percent_outliers_15iqr', 'percent_outliers_3iqr',
-         'percent_outliers_1_99', 'percent_outliers_3std',
-         'has_outliers_15iqr', 'has_outliers_3iqr', 'has_outliers_1_99',
-         'has_outliers_3std'])
-
-    ###########################################################################
-
-    normality_k2, normality_p = normaltest(X)
-    is_normal_5 = (normality_p < 0.05).astype(int)
-    is_normal_1 = (normality_p < 0.01).astype(int)
-
-    meta_vec.extend(list_process(normality_p))
-    meta_vec.extend(list_process(is_normal_5))
-    meta_vec.extend(list_process(is_normal_1))
-
-    meta_vec_names.extend(list_process_name('normality_p'))
-    meta_vec_names.extend(list_process_name('is_normal_5'))
-    meta_vec_names.extend(list_process_name('is_normal_1'))
-
-    moment_5 = moment(X, moment=5)
-    moment_6 = moment(X, moment=6)
-    moment_7 = moment(X, moment=7)
-    moment_8 = moment(X, moment=8)
-    moment_9 = moment(X, moment=9)
-    moment_10 = moment(X, moment=10)
-    meta_vec.extend(list_process(moment_5))
-    meta_vec.extend(list_process(moment_6))
-    meta_vec.extend(list_process(moment_7))
-    meta_vec.extend(list_process(moment_8))
-    meta_vec.extend(list_process(moment_9))
-    meta_vec.extend(list_process(moment_10))
-    meta_vec_names.extend(list_process_name('moment_5'))
-    meta_vec_names.extend(list_process_name('moment_6'))
-    meta_vec_names.extend(list_process_name('moment_7'))
-    meta_vec_names.extend(list_process_name('moment_8'))
-    meta_vec_names.extend(list_process_name('moment_9'))
-    meta_vec_names.extend(list_process_name('moment_10'))
-
-    # note: this is for each dimension == the number of dimensions
-    skewness_list = skew(X).reshape(-1, 1)
-    skew_values = list_process(skewness_list)
-    meta_vec.extend(skew_values)
-    meta_vec_names.extend(list_process_name('skewness'))
-
-    # note: this is for each dimension == the number of dimensions
-    kurtosis_list = kurtosis(X)
-    kurtosis_values = list_process(kurtosis_list)
-    meta_vec.extend(kurtosis_values)
-    meta_vec_names.extend(list_process_name('kurtosis'))
-
-    correlation = np.nan_to_num(pd.DataFrame(X).corr(), nan=0)
-    correlation_list = flatten_diagonally(correlation)[
-                       0:int((n_features * n_features - n_features) / 2)]
-    correlation_values = list_process(correlation_list)
-    meta_vec.extend(correlation_values)
-    meta_vec_names.extend(list_process_name('correlation'))
-
-    covariance = np.cov(X.T)
-    covariance_list = flatten_diagonally(covariance)[
-                      0:int((n_features * n_features - n_features) / 2)]
-    covariance_values = list_process(covariance_list)
-    meta_vec.extend(covariance_values)
-    meta_vec_names.extend(list_process_name('covariance'))
-
-    # sparsity
-    rep_counts = []
-    for i in range(n_features):
-        rep_counts.append(len(np.unique(X[:, i])))
-    sparsity_list = np.asarray(rep_counts) / (n_samples)
-    sparsity = list_process(sparsity_list)
-    meta_vec.extend(sparsity)
-    meta_vec_names.extend(list_process_name('sparsity'))
-
-    # ANOVA p value
-    p_values_list = []
-    all_perm = list(itertools.combinations(list(range(n_features)), 2))
-    for j in all_perm:
-        p_values_list.append(f_oneway(X[:, j[0]], X[:, j[1]])[1])
-    anova_p_value = list_process(np.asarray(p_values_list))
-    # anova_p_value = np.mean(p_values_list)
-    # anova_p_value_exceed_thresh = np.mean((np.asarray(p_values_list)<0.05).astype(int))
-    meta_vec.extend(anova_p_value)
-    meta_vec_names.extend(list_process_name('anova_p_value'))
-
-    # pca
-    pca_transformer = sklearn_PCA(n_components=3)
-    X_transform = pca_transformer.fit_transform(X)
-
-    # first pc
-    pca_fpc = list_process(X_transform[0, :], r_min=False, r_max=False,
-                           r_mean=False,
-                           r_std=True, r_skew=True, r_kurtosis=True)
-    meta_vec.extend(pca_fpc)
-    meta_vec_names.extend(
-        ['first_pca_std', 'first_pca_skewness', 'first_pca_kurtosis'])
-
-    # entropy
-    entropy_list = []
-    for i in range(n_features):
-        counts = pd.Series(X[:, i]).value_counts()
-        entropy_list.append(entropy(counts) / n_samples)
-    entropy_values = list_process(entropy_list)
-    meta_vec.extend(entropy_values)
-    meta_vec_names.extend(list_process_name('entropy'))
-
-    # ##############################Landmarkers######################################
-    # # HBOS
-    # clf = HBOS(n_bins=10)
-    # clf.fit(X)
-    # HBOS_hists = clf.hist_
-    # HBOS_mean = np.mean(HBOS_hists, axis=0)
-    # HBOS_max = np.max(HBOS_hists, axis=0)
-    # HBOS_min = np.min(HBOS_hists, axis=0)
-    # meta_vec.extend(list_process(HBOS_mean))
-    # meta_vec.extend(list_process(HBOS_max))
-    # meta_vec.extend(list_process(HBOS_min))
-    # meta_vec_names.extend(list_process_name('HBOS_mean'))
-    # meta_vec_names.extend(list_process_name('HBOS_max'))
-    # meta_vec_names.extend(list_process_name('HBOS_min'))
-    #
-    # # IForest
-    # n_estimators = 100
-    # clf = IForest(n_estimators=n_estimators)
-    # clf.fit(X)
-    #
-    # n_leaves = []
-    # n_depth = []
-    # fi_mean = []
-    # fi_max = []
-    #
-    # # doing this for each sub-trees
-    # for i in range(n_estimators):
-    #     n_leaves.append(clf.estimators_[i].get_n_leaves())
-    #     n_depth.append(clf.estimators_[i].get_depth())
-    #     fi_mean.append(clf.estimators_[i].feature_importances_.mean())
-    #     fi_max.append(clf.estimators_[i].feature_importances_.max())
-    #     # print(clf.estimators_[i].tree_)
-    #
-    # meta_vec.extend(list_process(n_leaves))
-    # meta_vec.extend(list_process(n_depth))
-    # meta_vec.extend(list_process(fi_mean))
-    # meta_vec.extend(list_process(fi_max))
-    #
-    # meta_vec_names.extend(list_process_name('IForest_n_leaves'))
-    # meta_vec_names.extend(list_process_name('IForest_n_depth'))
-    # meta_vec_names.extend(list_process_name('IForest_fi_mean'))
-    # meta_vec_names.extend(list_process_name('IForest_fi_max'))
-    #
-    # # PCA
-    # clf = PCA(n_components=3)
-    # clf.fit(X)
-    # meta_vec.extend(clf.explained_variance_ratio_)
-    # meta_vec.extend(clf.singular_values_)
-    # meta_vec_names.extend(
-    #     ['pca_expl_ratio_1', 'pca_expl_ratio_2', 'pca_expl_ratio_3'])
-    # meta_vec_names.extend(['pca_sv_1', 'pca_sv_2', 'pca_sv_3'])
-    #
-    # # LODA
-    # n_bins = 10
-    # n_random_cuts = 100
-    #
-    # n_hists_mean = []
-    # n_hists_max = []
-    #
-    # n_cuts_mean = []
-    # n_cuts_max = []
-    #
-    # clf = LODA(n_bins=n_bins, n_random_cuts=n_random_cuts)
-    # clf.fit(X)
-    #
-    # for i in range(n_bins):
-    #     n_hists_mean.append(clf.histograms_[:, i].mean())
-    #     n_hists_max.append(clf.histograms_[:, i].max())
-    # for i in range(n_random_cuts):
-    #     n_cuts_mean.append(clf.histograms_[i, :].mean())
-    #     n_cuts_max.append(clf.histograms_[i, :].max())
-    #
-    # meta_vec.extend(list_process(n_hists_mean))
-    # meta_vec.extend(list_process(n_hists_max))
-    # meta_vec.extend(list_process(n_cuts_mean))
-    # meta_vec.extend(list_process(n_cuts_max))
-    #
-    # meta_vec_names.extend(list_process_name('LODA_n_hists_mean'))
-    # meta_vec_names.extend(list_process_name('LODA_n_hists_max'))
-    # meta_vec_names.extend(list_process_name('LODA_n_cuts_mean'))
-    # meta_vec_names.extend(list_process_name('LODA_n_cuts_max'))
-
-    return meta_vec, meta_vec_names
+# -*- coding: utf-8 -*-
+"""Generate meta-features from an arbitrary dataset.
+"""
+# Author: Yue Zhao <zhaoy@cmu.edu>
+# License: BSD 2 clause
+
+
+import pandas as pd
+import numpy as np
+import itertools
+
+from sklearn.decomposition import PCA as sklearn_PCA
+from scipy.stats import skew, kurtosis
+from scipy.stats import f_oneway
+from scipy.stats import entropy
+
+from scipy.stats import moment
+from scipy.stats import normaltest
+
+# from pyod.models.hbos import HBOS
+# from pyod.models.iforest import IForest
+# from pyod.models.pca import PCA
+# from pyod.models.loda import LODA
+from sklearn.utils import check_array
+
+
+def gini(array):
+    """Calculate the Gini coefficient of a numpy array."""
+    # based on bottom eq:
+    # http://www.statsdirect.com/help/generatedimages/equations/equation154.svg
+    # from:
+    # http://www.statsdirect.com/help/default.htm#nonparametric_methods/gini.htm
+    # All values are treated equally, arrays must be 1d:
+    array = array.flatten()
+    if np.amin(array) < 0:
+        # Values cannot be negative:
+        array -= np.amin(array)
+    # Values cannot be 0:
+    array = np.add(array, 0.0000001, casting="unsafe")
+    # Values must be sorted:
+    array = np.sort(array)
+    # Index per array element:
+    index = np.arange(1, array.shape[0] + 1)
+    # Number of array elements:
+    n = array.shape[0]
+    # Gini coefficient:
+    return ((np.sum((2 * index - n - 1) * array)) / (n * np.sum(array)))
+
+
+def Diff(li1, li2):
+    """Calculate the difference of two list
+
+    Parameters
+    ----------
+    li1
+    li2
+
+    Returns
+    -------
+
+    """
+    return (list(set(li1) - set(li2)))
+
+
+def argmaxn(w, nth):
+    w = np.asarray(w).ravel()
+    t = np.argsort(w)
+    return t[-1 * nth]
+
+
+def flatten_diagonally(x, diags=None):
+    diags = np.array(diags)
+    if x.shape[1] > x.shape[0]:
+        diags += x.shape[1] - x.shape[0]
+    n = max(x.shape)
+    ndiags = 2 * n - 1
+    i, j = np.indices(x.shape)
+    d = np.array([])
+    for ndi in range(ndiags):
+        if diags != None:
+            if not ndi in diags:
+                continue
+        d = np.concatenate((d, x[i == j + (n - 1) - ndi]))
+    return d
+
+
+def list_process(x, r_min=True, r_max=True, r_mean=True, r_std=True,
+                 r_skew=True, r_kurtosis=True):
+    """Return statistics of a list
+
+    Parameters
+    ----------
+    x
+    r_min
+    r_max
+    r_mean
+    r_std
+    r_skew
+    r_kurtosis
+
+    Returns
+    -------
+
+    """
+    x = np.asarray(x).reshape(-1, 1)
+    return_list = []
+
+    if r_min:
+        return_list.append(np.nanmin(x))
+
+    if r_max:
+        return_list.append(np.nanmax(x))
+
+    if r_mean:
+        return_list.append(np.nanmean(x))
+
+    if r_std:
+        return_list.append(np.nanstd(x))
+
+    if r_skew:
+        return_list.append(skew(x, nan_policy='omit')[0])
+
+    if r_kurtosis:
+        return_list.append(kurtosis(x, nan_policy='omit')[0])
+
+    return return_list
+
+
+def list_process_name(var):
+    return [var + '_min', var + '_max', var + '_mean', var + '_std',
+            var + '_skewness', var + '_kurtosis']
+
+
+def generate_meta_features(X):
+    """Get the meta-features of a datasets X
+
+    Parameters
+    ----------
+    X : numpy array of shape (n_samples, n_features)
+        Input array
+
+    Returns
+    -------
+    meta_features : numpy array of shape (1, 200)
+        Meta-feature in dimension of 200
+
+    """
+    # outliers_fraction = np.count_nonzero(y) / len(y)
+    # outliers_percentage = round(outliers_fraction * 100, ndigits=4)
+    X = check_array(X)
+
+    meta_vec = []
+    meta_vec_names = []
+
+    # on the sample level
+    n_samples, n_features = X.shape[0], X.shape[1]
+
+    meta_vec.append(n_samples)
+    meta_vec.append(n_features)
+
+    meta_vec_names.append('n_samples')
+    meta_vec_names.append('n_features')
+
+    sample_mean = np.mean(X)
+    sample_median = np.median(X)
+    sample_var = np.var(X)
+    sample_min = np.min(X)
+    sample_max = np.max(X)
+    sample_std = np.std(X)
+
+    q1, q25, q75, q99 = np.percentile(X, [0.01, 0.25, 0.75, 0.99])
+    iqr = q75 - q25
+
+    normalized_mean = sample_mean / sample_max
+    normalized_median = sample_median / sample_max
+    sample_range = sample_max - sample_min
+    sample_gini = gini(X)
+    med_abs_dev = np.median(np.absolute(X - sample_median))
+    avg_abs_dev = np.mean(np.absolute(X - sample_mean))
+    quant_coeff_disp = (q75 - q25) / (q75 + q25)
+    coeff_var = sample_var / sample_mean
+
+    outliers_15iqr = np.logical_or(
+        X < (q25 - 1.5 * iqr), X > (q75 + 1.5 * iqr))
+    outliers_3iqr = np.logical_or(X < (q25 - 3 * iqr), X > (q75 + 3 * iqr))
+    outliers_1_99 = np.logical_or(X < q1, X > q99)
+    outliers_3std = np.logical_or(X < (sample_mean - 3 * sample_std),
+                                  X > (sample_mean + 3 * sample_std))
+
+    percent_outliers_15iqr = np.sum(outliers_15iqr) / len(X)
+    percent_outliers_3iqr = np.sum(outliers_3iqr) / len(X)
+    percent_outliers_1_99 = np.sum(outliers_1_99) / len(X)
+    percent_outliers_3std = np.sum(outliers_3std) / len(X)
+
+    has_outliers_15iqr = np.any(outliers_15iqr).astype(int)
+    has_outliers_3iqr = np.any(outliers_3iqr).astype(int)
+    has_outliers_1_99 = np.any(outliers_1_99).astype(int)
+    has_outliers_3std = np.any(outliers_3std).astype(int)
+
+    meta_vec.extend(
+        [sample_mean, sample_median, sample_var, sample_min, sample_max,
+         sample_std,
+         q1, q25, q75, q99, iqr, normalized_mean, normalized_median,
+         sample_range, sample_gini,
+         med_abs_dev, avg_abs_dev, quant_coeff_disp, coeff_var,
+         # moment_5, moment_6, moment_7, moment_8, moment_9, moment_10,
+         percent_outliers_15iqr, percent_outliers_3iqr, percent_outliers_1_99,
+         percent_outliers_3std,
+         has_outliers_15iqr, has_outliers_3iqr, has_outliers_1_99,
+         has_outliers_3std])
+
+    meta_vec_names.extend(
+        ['sample_mean', 'sample_median', 'sample_var', 'sample_min',
+         'sample_max', 'sample_std',
+         'q1', 'q25', 'q75', 'q99', 'iqr', 'normalized_mean',
+         'normalized_median', 'sample_range', 'sample_gini',
+         'med_abs_dev', 'avg_abs_dev', 'quant_coeff_disp', 'coeff_var',
+         # moment_5, moment_6, moment_7, moment_8, moment_9, moment_10,
+         'percent_outliers_15iqr', 'percent_outliers_3iqr',
+         'percent_outliers_1_99', 'percent_outliers_3std',
+         'has_outliers_15iqr', 'has_outliers_3iqr', 'has_outliers_1_99',
+         'has_outliers_3std'])
+
+    ###########################################################################
+
+    normality_k2, normality_p = normaltest(X)
+    is_normal_5 = (normality_p < 0.05).astype(int)
+    is_normal_1 = (normality_p < 0.01).astype(int)
+
+    meta_vec.extend(list_process(normality_p))
+    meta_vec.extend(list_process(is_normal_5))
+    meta_vec.extend(list_process(is_normal_1))
+
+    meta_vec_names.extend(list_process_name('normality_p'))
+    meta_vec_names.extend(list_process_name('is_normal_5'))
+    meta_vec_names.extend(list_process_name('is_normal_1'))
+
+    moment_5 = moment(X, moment=5)
+    moment_6 = moment(X, moment=6)
+    moment_7 = moment(X, moment=7)
+    moment_8 = moment(X, moment=8)
+    moment_9 = moment(X, moment=9)
+    moment_10 = moment(X, moment=10)
+    meta_vec.extend(list_process(moment_5))
+    meta_vec.extend(list_process(moment_6))
+    meta_vec.extend(list_process(moment_7))
+    meta_vec.extend(list_process(moment_8))
+    meta_vec.extend(list_process(moment_9))
+    meta_vec.extend(list_process(moment_10))
+    meta_vec_names.extend(list_process_name('moment_5'))
+    meta_vec_names.extend(list_process_name('moment_6'))
+    meta_vec_names.extend(list_process_name('moment_7'))
+    meta_vec_names.extend(list_process_name('moment_8'))
+    meta_vec_names.extend(list_process_name('moment_9'))
+    meta_vec_names.extend(list_process_name('moment_10'))
+
+    # note: this is for each dimension == the number of dimensions
+    skewness_list = skew(X).reshape(-1, 1)
+    skew_values = list_process(skewness_list)
+    meta_vec.extend(skew_values)
+    meta_vec_names.extend(list_process_name('skewness'))
+
+    # note: this is for each dimension == the number of dimensions
+    kurtosis_list = kurtosis(X)
+    kurtosis_values = list_process(kurtosis_list)
+    meta_vec.extend(kurtosis_values)
+    meta_vec_names.extend(list_process_name('kurtosis'))
+
+    correlation = np.nan_to_num(pd.DataFrame(X).corr(), nan=0)
+    correlation_list = flatten_diagonally(correlation)[
+                       0:int((n_features * n_features - n_features) / 2)]
+    correlation_values = list_process(correlation_list)
+    meta_vec.extend(correlation_values)
+    meta_vec_names.extend(list_process_name('correlation'))
+
+    covariance = np.cov(X.T)
+    covariance_list = flatten_diagonally(covariance)[
+                      0:int((n_features * n_features - n_features) / 2)]
+    covariance_values = list_process(covariance_list)
+    meta_vec.extend(covariance_values)
+    meta_vec_names.extend(list_process_name('covariance'))
+
+    # sparsity
+    rep_counts = []
+    for i in range(n_features):
+        rep_counts.append(len(np.unique(X[:, i])))
+    sparsity_list = np.asarray(rep_counts) / (n_samples)
+    sparsity = list_process(sparsity_list)
+    meta_vec.extend(sparsity)
+    meta_vec_names.extend(list_process_name('sparsity'))
+
+    # ANOVA p value
+    p_values_list = []
+    all_perm = list(itertools.combinations(list(range(n_features)), 2))
+    for j in all_perm:
+        p_values_list.append(f_oneway(X[:, j[0]], X[:, j[1]])[1])
+    anova_p_value = list_process(np.asarray(p_values_list))
+    # anova_p_value = np.mean(p_values_list)
+    # anova_p_value_exceed_thresh = np.mean((np.asarray(p_values_list)<0.05).astype(int))
+    meta_vec.extend(anova_p_value)
+    meta_vec_names.extend(list_process_name('anova_p_value'))
+
+    # pca
+    pca_transformer = sklearn_PCA(n_components=3)
+    X_transform = pca_transformer.fit_transform(X)
+
+    # first pc
+    pca_fpc = list_process(X_transform[0, :], r_min=False, r_max=False,
+                           r_mean=False,
+                           r_std=True, r_skew=True, r_kurtosis=True)
+    meta_vec.extend(pca_fpc)
+    meta_vec_names.extend(
+        ['first_pca_std', 'first_pca_skewness', 'first_pca_kurtosis'])
+
+    # entropy
+    entropy_list = []
+    for i in range(n_features):
+        counts = pd.Series(X[:, i]).value_counts()
+        entropy_list.append(entropy(counts) / n_samples)
+    entropy_values = list_process(entropy_list)
+    meta_vec.extend(entropy_values)
+    meta_vec_names.extend(list_process_name('entropy'))
+
+    # ##############################Landmarkers######################################
+    # # HBOS
+    # clf = HBOS(n_bins=10)
+    # clf.fit(X)
+    # HBOS_hists = clf.hist_
+    # HBOS_mean = np.mean(HBOS_hists, axis=0)
+    # HBOS_max = np.max(HBOS_hists, axis=0)
+    # HBOS_min = np.min(HBOS_hists, axis=0)
+    # meta_vec.extend(list_process(HBOS_mean))
+    # meta_vec.extend(list_process(HBOS_max))
+    # meta_vec.extend(list_process(HBOS_min))
+    # meta_vec_names.extend(list_process_name('HBOS_mean'))
+    # meta_vec_names.extend(list_process_name('HBOS_max'))
+    # meta_vec_names.extend(list_process_name('HBOS_min'))
+    #
+    # # IForest
+    # n_estimators = 100
+    # clf = IForest(n_estimators=n_estimators)
+    # clf.fit(X)
+    #
+    # n_leaves = []
+    # n_depth = []
+    # fi_mean = []
+    # fi_max = []
+    #
+    # # doing this for each sub-trees
+    # for i in range(n_estimators):
+    #     n_leaves.append(clf.estimators_[i].get_n_leaves())
+    #     n_depth.append(clf.estimators_[i].get_depth())
+    #     fi_mean.append(clf.estimators_[i].feature_importances_.mean())
+    #     fi_max.append(clf.estimators_[i].feature_importances_.max())
+    #     # print(clf.estimators_[i].tree_)
+    #
+    # meta_vec.extend(list_process(n_leaves))
+    # meta_vec.extend(list_process(n_depth))
+    # meta_vec.extend(list_process(fi_mean))
+    # meta_vec.extend(list_process(fi_max))
+    #
+    # meta_vec_names.extend(list_process_name('IForest_n_leaves'))
+    # meta_vec_names.extend(list_process_name('IForest_n_depth'))
+    # meta_vec_names.extend(list_process_name('IForest_fi_mean'))
+    # meta_vec_names.extend(list_process_name('IForest_fi_max'))
+    #
+    # # PCA
+    # clf = PCA(n_components=3)
+    # clf.fit(X)
+    # meta_vec.extend(clf.explained_variance_ratio_)
+    # meta_vec.extend(clf.singular_values_)
+    # meta_vec_names.extend(
+    #     ['pca_expl_ratio_1', 'pca_expl_ratio_2', 'pca_expl_ratio_3'])
+    # meta_vec_names.extend(['pca_sv_1', 'pca_sv_2', 'pca_sv_3'])
+    #
+    # # LODA
+    # n_bins = 10
+    # n_random_cuts = 100
+    #
+    # n_hists_mean = []
+    # n_hists_max = []
+    #
+    # n_cuts_mean = []
+    # n_cuts_max = []
+    #
+    # clf = LODA(n_bins=n_bins, n_random_cuts=n_random_cuts)
+    # clf.fit(X)
+    #
+    # for i in range(n_bins):
+    #     n_hists_mean.append(clf.histograms_[:, i].mean())
+    #     n_hists_max.append(clf.histograms_[:, i].max())
+    # for i in range(n_random_cuts):
+    #     n_cuts_mean.append(clf.histograms_[i, :].mean())
+    #     n_cuts_max.append(clf.histograms_[i, :].max())
+    #
+    # meta_vec.extend(list_process(n_hists_mean))
+    # meta_vec.extend(list_process(n_hists_max))
+    # meta_vec.extend(list_process(n_cuts_mean))
+    # meta_vec.extend(list_process(n_cuts_max))
+    #
+    # meta_vec_names.extend(list_process_name('LODA_n_hists_mean'))
+    # meta_vec_names.extend(list_process_name('LODA_n_hists_max'))
+    # meta_vec_names.extend(list_process_name('LODA_n_cuts_mean'))
+    # meta_vec_names.extend(list_process_name('LODA_n_cuts_max'))
+
+    return meta_vec, meta_vec_names
```

### Comparing `deepod-0.2.0/deepod/models/anogan.py` & `deepod-0.3.0/deepod/models/feawad.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,235 +1,212 @@
-# -*- coding: utf-8 -*-
-"""
-!! this is in development now. !!
-One-class classification
-this script is partially adapted from https://github.com/jmjeon94/AnoGAN-pytorch
-@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
-"""
-
-from deepod.core.base_model import BaseDeepAD
-from deepod.core.base_networks import MLPnet
-from torch.utils.data import DataLoader
-import torch
-import time
-
-
-class AnoGAN(BaseDeepAD):
-    """ AnoGAN for anomaly detection
-    See : for detail
-
-    Parameters
-    ----------
-    epochs: int, optional (default=100)
-        Number of training epochs
-
-    batch_size: int, optional (default=64)
-        Number of samples in a mini-batch
-
-    lr: float, optional (default=1e-3)
-        Learning rate
-
-    rep_dim: int, optional (default=128)
-        Dimensionality of the representation space
-
-    hidden_dims: list, str or int, optional (default='100,50')
-        Number of neural units in hidden layers
-            - If list, each item is a layer
-            - If str, neural units of hidden layers are split by comma
-            - If int, number of neural units of single hidden layer
-
-    act: str, optional (default='ReLU')
-        activation layer name
-        choice = ['ReLU', 'LeakyReLU', 'Sigmoid', 'Tanh']
-
-    bias: bool, optional (default=False)
-        Additive bias in linear layer
-
-    epoch_steps: int, optional (default=-1)
-        Maximum steps in an epoch
-            - If -1, all the batches will be processed
-
-    prt_steps: int, optional (default=10)
-        Number of epoch intervals per printing
-
-    device: str, optional (default='cuda')
-        torch device,
-
-    verbose: int, optional (default=1)
-        Verbosity mode
-
-    random_state： int, optional (default=42)
-        the seed used by the random
-
-    """
-    def __init__(self, epochs=100, batch_size=64, lr=1e-3,
-                 z_dim=128,
-                 rep_dim=128, hidden_dims='100,50', act='ReLU', bias=False,
-                 epoch_steps=-1, prt_steps=10, device='cuda',
-                 verbose=2, random_state=42):
-        super(AnoGAN, self).__init__(
-            model_name='AnoGAN', epochs=epochs, batch_size=batch_size, lr=lr,
-            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
-            verbose=verbose, random_state=random_state
-        )
-        self.z_dim = z_dim
-
-        self.hidden_dims = hidden_dims
-        self.rep_dim = rep_dim
-        self.act = act
-        self.bias = bias
-        return
-
-    def training_prepare(self, X, y):
-        train_loader = DataLoader(X, batch_size=self.batch_size, shuffle=True)
-
-        g_net = MLPnet(
-            n_features=self.z_dim,
-            n_hidden=self.hidden_dims,
-            n_output=self.n_features,
-            activation=self.act,
-            bias=self.bias,
-        ).to(self.device)
-        d_net = MLPnet(
-            n_features=self.n_features,
-            n_hidden = self.hidden_dims,
-            n_output = 1,
-            activation = self.act,
-            bias=self.bias
-        ).to(self.device)
-        net = (g_net, d_net)
-
-        criterion = torch.nn.BCELoss()
-
-        if self.verbose >= 2:
-            print(g_net)
-            print(d_net)
-
-        return train_loader, net, criterion
-
-    def _training(self):
-        optimizer_g = torch.optim.Adam(self.net[0].parameters(),
-                                       lr=self.lr,
-                                       weight_decay=1e-5)
-        optimizer_d = torch.optim.Adam(self.net[1].parameters(),
-                                       lr=self.lr,
-                                       weight_decay=1e-5)
-
-        for i in range(self.epochs):
-            t1 = time.time()
-            total_g_loss = 0
-            total_d_loss = 0
-            cnt = 0
-            for batch_x in self.train_loader:
-                b_size = batch_x.size(0)
-
-                # update discriminator network
-                self.net[1].zero_grad()
-
-                # for real
-                batch_x = batch_x.float().to(self.device)
-                label = torch.ones(b_size).to(self.device)
-                output_real = self.net[1](batch_x).view(-1)
-                output_real = torch.sigmoid(output_real)
-                err_real = self.criterion(output_real, label)
-                err_real.backward()
-
-                # for noise
-                fake = self.net[0](torch.randn(b_size, self.z_dim, device=self.device))
-                label = torch.zeros(b_size).to(self.device)
-                output_fake = self.net[1](fake.detach()).view(-1)
-                output_fake = torch.sigmoid(output_fake)
-                err_fake = self.criterion(output_fake, label)
-                err_fake.backward()
-
-                err_d = err_fake + err_real
-                optimizer_d.step()
-
-                # update generative network
-                self.net[0].zero_grad()
-                label.fill_(1.)
-                output = self.net[1](fake).view(-1)
-                output = torch.sigmoid(output)
-                err_g = self.criterion(output, label)
-
-                err_g.backward()
-                optimizer_g.step()
-
-                total_d_loss += err_d.item()
-                total_g_loss += err_g.item()
-                cnt += 1
-
-                # terminate this epoch when reaching assigned maximum steps per epoch
-                if cnt > self.epoch_steps != -1:
-                    break
-
-            t = time.time() - t1
-            if self.verbose >= 1 and (i == 0 or (i+1) % self.prt_steps == 0):
-                print(f'epoch{i+1}, '
-                      f'training loss (generative/discriminative): '
-                      f'{total_g_loss/cnt:.6f} / {total_d_loss/cnt:.6f}, '
-                      f'time: {t:.1f}s')
-
-            if i == 0:
-                self.epoch_time = t
-
-            self.epoch_update()
-
-        return
-
-    def inference_prepare(self, X):
-        test_loader = DataLoader(X, batch_size=self.batch_size,
-                                 drop_last=False, shuffle=False)
-        self.criterion.reduction = 'none'
-        return test_loader
-
-    def _inference(self):
-        self.net[1].eval()
-        with torch.no_grad():
-            z_lst = []
-            score_lst = []
-            for batch_x in self.test_loader:
-                batch_x = batch_x.float().to(self.device)
-                s = self.net[1](batch_x)
-                s = s.view(-1)
-
-                batch_z = batch_x
-
-                z_lst.append(batch_z)
-                score_lst.append(s)
-
-        z = torch.cat(z_lst).data.cpu().numpy()
-        scores = torch.cat(score_lst).data.cpu().numpy()
-
-        return z, scores
-
-    def training_forward(self, batch_x, net, criterion):
-        # implement in _training
-        pass
-
-    def inference_forward(self, batch_x, net, criterion):
-        # implement in _inference
-        pass
-
-if __name__ == '__main__':
-    import numpy as np
-
-    file = '../../data/38_thyroid.npz'
-    data = np.load(file, allow_pickle=True)
-    x, y = data['X'], data['y']
-    y = np.array(y, dtype=int)
-
-    anom_id = np.where(y==1)[0]
-    known_anom_id = np.random.choice(anom_id, 30)
-    y_semi = np.zeros_like(y)
-    y_semi[known_anom_id] = 1
-
-    clf = AnoGAN(device='cuda', prt_steps=1, epochs=100)
-    clf.fit(x, y_semi)
-
-    scores = clf.decision_function(x)
-
-    from sklearn.metrics import roc_auc_score
-
-    auc = roc_auc_score(y_score=scores, y_true=y)
-
-    print(auc)
+# -*- coding: utf-8 -*-
+"""
+Feature Encoding with AutoEncoders for Weakly-supervised Anomaly Detection
+PyTorch's implementation
+@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
+"""
+
+from deepod.core.base_model import BaseDeepAD
+from deepod.core.base_networks import get_network
+from torch.utils.data import DataLoader, TensorDataset
+from torch.utils.data.sampler import WeightedRandomSampler
+import torch
+import numpy as np
+
+
+class FeaWAD(BaseDeepAD):
+    """
+    Parameters
+    ----------
+    epochs: int, optional (default=100)
+        Number of training epochs
+
+    batch_size: int, optional (default=64)
+        Number of samples in a mini-batch
+
+    lr: float, optional (default=1e-3)
+        Learning rate
+
+    rep_dim: int, optional (default=128)
+        Dimensionality of the representation space
+
+    hidden_dims: list, str or int, optional (default='100,50')
+        Number of neural units in hidden layers
+            - If list, each item is a layer
+            - If str, neural units of hidden layers are split by comma
+            - If int, number of neural units of single hidden layer
+
+    act: str, optional (default='ReLU')
+        activation layer name
+        choice = ['ReLU', 'LeakyReLU', 'Sigmoid', 'Tanh']
+
+    bias: bool, optional (default=False)
+        Additive bias in linear layer
+
+    margin: float, optional (default=5.)
+        margin value used in the deviation loss function
+
+    epoch_steps: int, optional (default=-1)
+        Maximum steps in an epoch
+            - If -1, all the batches will be processed
+
+    prt_steps: int, optional (default=10)
+        Number of epoch intervals per printing
+
+    device: str, optional (default='cuda')
+        torch device,
+
+    verbose: int, optional (default=1)
+        Verbosity mode
+
+    random_state： int, optional (default=42)
+        the seed used by the random
+    """
+    def __init__(self, data_type='tabular', epochs=100, batch_size=64, lr=1e-3,
+                 network='MLP', seq_len=100, stride=1,
+                 rep_dim=128, hidden_dims='100,50', act='ReLU', bias=False,
+                 margin=5.,
+                 epoch_steps=-1, prt_steps=10, device='cuda',
+                 verbose=2, random_state=42):
+        super(FeaWAD, self).__init__(
+            data_type=data_type, model_name='FeaWAD', epochs=epochs, batch_size=batch_size, lr=lr,
+            network=network, seq_len=seq_len, stride=stride,
+            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
+            verbose=verbose, random_state=random_state
+        )
+
+        self.margin = margin
+
+        self.rep_dim = rep_dim
+        self.hidden_dims = hidden_dims
+        self.act = act
+        self.bias = bias
+
+        return
+
+    def training_prepare(self, X, y):
+        # loader: balanced loader, a mini-batch contains a half of normal data and a half of anomalies
+        n_anom = np.where(y == 1)[0].shape[0]
+        n_norm = self.n_samples - n_anom
+        weight_map = {0: 1. / n_norm, 1: 1. / n_anom}
+
+        dataset = TensorDataset(torch.from_numpy(X).float(), torch.from_numpy(y).long())
+        sampler = WeightedRandomSampler(weights=[weight_map[label.item()] for data, label in dataset],
+                                        num_samples=self.batch_size, replacement=True)
+        train_loader = DataLoader(dataset, batch_size=self.batch_size, sampler=sampler)
+
+        network_params = {
+            'n_features': self.n_features,
+            'network': self.network,
+            'n_emb': self.rep_dim,
+            'n_hidden': self.hidden_dims,
+            'n_hidden2': '256,32',
+            'activation': self.act,
+            'bias': self.bias
+        }
+
+        net = FeaWadNet(**network_params).to(self.device)
+        criterion = FeaWADLoss(margin=self.margin)
+        if self.verbose >= 2:
+            print(net)
+
+        return train_loader, net, criterion
+
+    def inference_prepare(self, X):
+        test_loader = DataLoader(X, batch_size=self.batch_size,
+                                 drop_last=False, shuffle=False)
+        self.criterion.reduction = 'none'
+        return test_loader
+
+    def training_forward(self, batch_x, net, criterion):
+        batch_x, batch_y = batch_x
+        batch_x = batch_x.float().to(self.device)
+        batch_y = batch_y.to(self.device)
+        pred, sub_result = net(batch_x)
+        loss = criterion(batch_y, pred, sub_result)
+        return loss
+
+    def inference_forward(self, batch_x, net, criterion):
+        batch_x = batch_x.float().to(self.device)
+        s, _ = net(batch_x)
+        s = s.view(-1)
+        batch_z = batch_x
+        return batch_z, s
+
+
+class FeaWadNet(torch.nn.Module):
+    def __init__(self, n_features, network, n_hidden='500,100', n_hidden2='256,32', n_emb=20,
+                 activation='ReLU', bias=False):
+        super(FeaWadNet, self).__init__()
+
+        if network == 'MLP':
+            AEmodel_class = get_network('MlpAE')
+            FWmodel = get_network('MLP')
+        elif network == 'TCN':
+            AEmodel_class = get_network('TcnAE')
+            FWmodel = get_network('MLP')
+        else:
+            raise NotImplementedError('')
+
+        self.AEmodel = AEmodel_class(n_features, n_hidden=n_hidden, n_emb=n_emb,
+                               activation=activation, bias=bias)
+        self.LinearModel = FWmodel(n_features+n_emb, n_hidden=n_hidden2, n_output=1,
+                                   activation=activation, bias=bias)
+
+    def forward(self, x):
+        x2, enc = self.AEmodel(x)
+        sub = x2 - x
+        sub_norm = torch.norm(sub, p=2, dim=-1)
+        sub_norm = torch.unsqueeze(sub_norm, -1)
+        sub_result = sub / sub_norm
+
+        concat = torch.concat([sub_result, enc], dim=-1)
+        if len(concat.shape) == 3:
+            concat = concat[:, -1]
+        out = self.LinearModel(concat)
+
+        return out, sub_result
+
+
+class FeaWADLoss(torch.nn.Module):
+    """
+    Deviation Loss
+
+    Parameters
+    ----------
+    margin: float, optional (default=5.)
+        Center of the pre-defined hyper-sphere in the representation space
+
+    l: int, optional (default=5000.)
+        the size of samples of the Gaussian distribution used in the deviation loss function
+
+    reduction: str, optional (default='mean')
+        choice = [``'none'`` | ``'mean'`` | ``'sum'``]
+            - If ``'none'``: no reduction will be applied;
+            - If ``'mean'``: the sum of the output will be divided by the number of
+            elements in the output;
+            - If ``'sum'``: the output will be summed
+
+    """
+    def __init__(self, margin=5., reduction='mean'):
+        super(FeaWADLoss, self).__init__()
+        self.margin = margin
+        self.reduction = reduction
+        return
+
+    def forward(self, y_true, y_pred, sub_result):
+        dev = y_pred
+        inlier_loss = torch.abs(dev)
+        outlier_loss = torch.abs(torch.maximum(self.margin - dev, torch.tensor(0.)))
+
+        sub_nor = torch.norm(sub_result, p=2, dim=1 if len(sub_result.shape)==2 else [1,2])
+        outlier_sub_loss = torch.abs(torch.maximum(self.margin-sub_nor, torch.tensor(0.)))
+        loss = (1 - y_true) * (inlier_loss + sub_nor) + y_true * (outlier_loss + outlier_sub_loss)
+
+        if self.reduction == 'mean':
+            return torch.mean(loss)
+        elif self.reduction == 'sum':
+            return torch.sum(loss)
+        elif self.reduction == 'none':
+            return loss
+
+        return loss
```

### Comparing `deepod-0.2.0/deepod/models/dsad.py` & `deepod-0.3.0/deepod/models/dsvdd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,214 +1,201 @@
-# -*- coding: utf-8 -*-
-"""
-One-class classification
-this is partially adapted from
-@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
-"""
-
-from deepod.core.base_model import BaseDeepAD
-from deepod.core.base_networks import MLPnet
-from torch.utils.data import DataLoader, TensorDataset
-import torch
-import numpy as np
-
-
-class DeepSAD(BaseDeepAD):
-    """ Deep Semi-supervised Anomaly Detection (Deep SAD)
-    See :cite:`ruff2020dsad` for details
-
-    Parameters
-    ----------
-    epochs: int, optional (default=100)
-        Number of training epochs
-
-    batch_size: int, optional (default=64)
-        Number of samples in a mini-batch
-
-    lr: float, optional (default=1e-3)
-        Learning rate
-
-    rep_dim: int, optional (default=128)
-        Dimensionality of the representation space
-
-    hidden_dims: list, str or int, optional (default='100,50')
-        Number of neural units in hidden layers
-            - If list, each item is a layer
-            - If str, neural units of hidden layers are split by comma
-            - If int, number of neural units of single hidden layer
-
-    act: str, optional (default='ReLU')
-        activation layer name
-        choice = ['ReLU', 'LeakyReLU', 'Sigmoid', 'Tanh']
-
-    bias: bool, optional (default=False)
-        Additive bias in linear layer
-
-    epoch_steps: int, optional (default=-1)
-        Maximum steps in an epoch
-            - If -1, all the batches will be processed
-
-    prt_steps: int, optional (default=10)
-        Number of epoch intervals per printing
-
-    device: str, optional (default='cuda')
-        torch device,
-
-    verbose: int, optional (default=1)
-        Verbosity mode
-
-    random_state： int, optional (default=42)
-        the seed used by the random
-
-    """
-
-    def __init__(self, epochs=100, batch_size=64, lr=1e-3,
-                 rep_dim=128, hidden_dims='100,50', act='ReLU', bias=False,
-                 epoch_steps=-1, prt_steps=10, device='cuda',
-                 verbose=2, random_state=42):
-        super(DeepSAD, self).__init__(
-            model_name='DeepSAD', epochs=epochs, batch_size=batch_size, lr=lr,
-            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
-            verbose=verbose, random_state=random_state
-        )
-
-        self.hidden_dims = hidden_dims
-        self.rep_dim = rep_dim
-        self.act = act
-        self.bias = bias
-
-        self.c = None
-
-        return
-
-    def training_prepare(self, X, y):
-
-        semi_y2 = y.copy()
-        semi_y2[np.where(y == 1)[0]] = -1
-        dataset = TensorDataset(torch.from_numpy(X).float(),
-                                torch.from_numpy(semi_y2).long())
-
-        train_loader = DataLoader(dataset, batch_size=self.batch_size, shuffle=True)
-
-        net = MLPnet(
-            n_features=self.n_features,
-            n_hidden=self.hidden_dims,
-            n_output=self.rep_dim,
-            activation=self.act,
-            bias=self.bias,
-        ).to(self.device)
-
-        # self.c = torch.randn(net.n_emb).to(self.device)
-        self.c = self._set_c(net, train_loader)
-        criterion = DSADLoss(c=self.c)
-
-        if self.verbose >= 2:
-            print(net)
-
-        return train_loader, net, criterion
-
-    def inference_prepare(self, X):
-        test_loader = DataLoader(X, batch_size=self.batch_size,
-                                 drop_last=False, shuffle=False)
-        self.criterion.reduction = 'none'
-        return test_loader
-
-    def training_forward(self, batch_x, net, criterion):
-        batch_x, batch_y = batch_x
-        batch_x = batch_x.float().to(self.device)
-        batch_y = batch_y.to(self.device)
-        z = net(batch_x)
-        loss = criterion(z, batch_y)
-        return loss
-
-    def inference_forward(self, batch_x, net, criterion):
-        batch_x = batch_x.float().to(self.device)
-        batch_z = net(batch_x)
-        s = criterion(batch_z)
-        return batch_z, s
-
-    def _set_c(self, net, dataloader, eps=0.1):
-        """Initializing the center for the hypersphere"""
-        net.eval()
-        z_ = []
-        with torch.no_grad():
-            for x, _ in dataloader:
-                x = x.float().to(self.device)
-                z = net(x)
-                z_.append(z.detach())
-        z_ = torch.cat(z_)
-        c = torch.mean(z_, dim=0)
-
-        # if c i s too close to zero, set to +- eps
-        # a zero unit can be trivially matched with zero weights
-        c[(abs(c) < eps) & (c < 0)] = -eps
-        c[(abs(c) < eps) & (c > 0)] = eps
-        return c
-
-
-class DSADLoss(torch.nn.Module):
-    """
-
-    Parameters
-    ----------
-    c: torch.Tensor
-        Center of the pre-defined hyper-sphere in the representation space
-
-    reduction: str, optional (default='mean')
-        choice = [``'none'`` | ``'mean'`` | ``'sum'``]
-            - If ``'none'``: no reduction will be applied;
-            - If ``'mean'``: the sum of the output will be divided by the number of
-            elements in the output;
-            - If ``'sum'``: the output will be summed
-
-    """
-
-    def __init__(self, c, eta=1.0, eps=1e-6, reduction='mean'):
-        super(DSADLoss, self).__init__()
-        self.c = c
-        self.reduction = reduction
-        self.eta = eta
-        self.eps = eps
-
-    def forward(self, rep, semi_targets=None, reduction=None):
-        dist = torch.sum((rep - self.c) ** 2, dim=1)
-
-        if semi_targets is not None:
-            loss = torch.where(semi_targets == 0, dist,
-                               self.eta * ((dist+self.eps) ** semi_targets.float()))
-        else:
-            loss = dist
-
-        if reduction is None:
-            reduction = self.reduction
-
-        if reduction == 'mean':
-            return torch.mean(loss)
-        elif reduction == 'sum':
-            return torch.sum(loss)
-        elif reduction == 'none':
-            return loss
-
-
-if __name__ == '__main__':
-    import numpy as np
-
-    file = '../../data/38_thyroid.npz'
-    data = np.load(file, allow_pickle=True)
-    x, y = data['X'], data['y']
-    y = np.array(y, dtype=int)
-
-    anom_id = np.where(y == 1)[0]
-    known_anom_id = np.random.choice(anom_id, 30)
-    y_semi = np.zeros_like(y)
-    y_semi[known_anom_id] = 1
-
-    clf = DeepSAD(device='cpu')
-    clf.fit(x, y_semi)
-
-    scores = clf.decision_function(x)
-
-    from sklearn.metrics import roc_auc_score
-
-    auc = roc_auc_score(y_score=scores, y_true=y)
-
-    print(auc)
+# -*- coding: utf-8 -*-
+"""
+One-class classification
+@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
+"""
+
+from deepod.core.base_model import BaseDeepAD
+from deepod.core.base_networks import get_network
+from torch.utils.data import DataLoader
+import torch
+
+
+class DeepSVDD(BaseDeepAD):
+    """ Deep One-class Classification (Deep SVDD) for anomaly detection
+    See :cite:`ruff2018deepsvdd` for details
+
+    Parameters
+    ----------
+    data_type: str, optional (default='tabular')
+        Data type, choice=['tabular', 'ts']
+
+    epochs: int, optional (default=100)
+        Number of training epochs
+
+    batch_size: int, optional (default=64)
+        Number of samples in a mini-batch
+
+    lr: float, optional (default=1e-3)
+        Learning rate
+
+    network: str, optional (default='MLP')
+        network structure for different data structures
+
+    seq_len: int, optional (default=100)
+        Size of window used to create subsequences from the data
+        deprecated when handling tabular data (network=='MLP')
+
+    stride: int, optional (default=1)
+        number of time points the window will move between two subsequences
+        deprecated when handling tabular data (network=='MLP')
+
+    rep_dim: int, optional (default=128)
+        Dimensionality of the representation space
+
+    hidden_dims: list, str or int, optional (default='100,50')
+        Number of neural units in hidden layers
+            - If list, each item is a layer
+            - If str, neural units of hidden layers are split by comma
+            - If int, number of neural units of single hidden layer
+
+    act: str, optional (default='ReLU')
+        activation layer name
+        choice = ['ReLU', 'LeakyReLU', 'Sigmoid', 'Tanh']
+
+    bias: bool, optional (default=False)
+        Additive bias in linear layer
+
+    epoch_steps: int, optional (default=-1)
+        Maximum steps in an epoch
+            - If -1, all the batches will be processed
+
+    prt_steps: int, optional (default=10)
+        Number of epoch intervals per printing
+
+    device: str, optional (default='cuda')
+        torch device,
+
+    verbose: int, optional (default=1)
+        Verbosity mode
+
+    random_state： int, optional (default=42)
+        the seed used by the random
+
+    """
+    def __init__(self, data_type='tabular', epochs=100, batch_size=64, lr=1e-3,
+                 network='MLP', seq_len=100, stride=1,
+                 rep_dim=128, hidden_dims='100,50', act='ReLU', bias=False,
+                 n_heads=8, d_model=512, attn='self_attn', pos_encoding='fixed', norm='LayerNorm',
+                 epoch_steps=-1, prt_steps=10, device='cuda',
+                 verbose=2, random_state=42):
+        super(DeepSVDD, self).__init__(
+            model_name='DeepSVDD', data_type=data_type, epochs=epochs, batch_size=batch_size, lr=lr,
+            network=network, seq_len=seq_len, stride=stride,
+            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
+            verbose=verbose, random_state=random_state
+        )
+
+        self.hidden_dims = hidden_dims
+        self.rep_dim = rep_dim
+        self.act = act
+        self.bias = bias
+
+        # parameters for Transformer
+        self.n_heads = n_heads
+        self.d_model = d_model
+        self.attn = attn
+        self.pos_encoding = pos_encoding
+        self.norm = norm
+        
+        self.c = None
+        return
+
+    def training_prepare(self, X, y):
+        train_loader = DataLoader(X, batch_size=self.batch_size, shuffle=True)
+
+        network_params = {
+            'n_features': self.n_features,
+            'n_hidden': self.hidden_dims,
+            'n_output': self.rep_dim,
+            'activation': self.act,
+            'bias': self.bias
+        }
+        if self.network == 'Transformer':
+            network_params['n_heads'] = self.n_heads
+            network_params['d_model'] = self.d_model
+            network_params['pos_encoding'] = self.pos_encoding
+            network_params['norm'] = self.norm
+            network_params['attn'] = self.attn
+            network_params['seq_len'] = self.seq_len
+        elif self.network == 'ConvSeq':
+            network_params['seq_len'] = self.seq_len
+        
+        network_class = get_network(self.network)
+        net = network_class(**network_params).to(self.device)
+
+        # self.c = torch.randn(net.n_emb).to(self.device)
+        self.c = self._set_c(net, train_loader)
+        criterion = DSVDDLoss(c=self.c)
+
+        if self.verbose >= 2:
+            print(net)
+
+        return train_loader, net, criterion
+
+    def inference_prepare(self, X):
+        test_loader = DataLoader(X, batch_size=self.batch_size,
+                                 drop_last=False, shuffle=False)
+        self.criterion.reduction = 'none'
+        return test_loader
+
+    def training_forward(self, batch_x, net, criterion):
+        batch_x = batch_x.float().to(self.device)
+        z = net(batch_x)
+        loss = criterion(z)
+        return loss
+
+    def inference_forward(self, batch_x, net, criterion):
+        batch_x = batch_x.float().to(self.device)
+        batch_z = net(batch_x)
+        s = criterion(batch_z)
+        return batch_z, s
+
+    def _set_c(self, net, dataloader, eps=0.1):
+        """Initializing the center for the hypersphere"""
+        net.eval()
+        z_ = []
+        with torch.no_grad():
+            for x in dataloader:
+                x = x.float().to(self.device)
+                z = net(x)
+                z_.append(z.detach())
+        z_ = torch.cat(z_)
+        c = torch.mean(z_, dim=0)
+        c[(abs(c) < eps) & (c < 0)] = -eps
+        c[(abs(c) < eps) & (c > 0)] = eps
+        return c
+
+
+class DSVDDLoss(torch.nn.Module):
+    """
+
+    Parameters
+    ----------
+    c: torch.Tensor
+        Center of the pre-defined hyper-sphere in the representation space
+
+    reduction: str, optional (default='mean')
+        choice = [``'none'`` | ``'mean'`` | ``'sum'``]
+            - If ``'none'``: no reduction will be applied;
+            - If ``'mean'``: the sum of the output will be divided by the number of
+            elements in the output;
+            - If ``'sum'``: the output will be summed
+
+    """
+    def __init__(self, c, reduction='mean'):
+        super(DSVDDLoss, self).__init__()
+        self.c = c
+        self.reduction = reduction
+
+    def forward(self, rep, reduction=None):
+        loss = torch.sum((rep - self.c) ** 2, dim=1)
+
+        if reduction is None:
+            reduction = self.reduction
+
+        if reduction == 'mean':
+            return torch.mean(loss)
+        elif reduction == 'sum':
+            return torch.sum(loss)
+        elif reduction == 'none':
+            return loss
```

### Comparing `deepod-0.2.0/deepod/models/dsvdd.py` & `deepod-0.3.0/deepod/models/rdp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,193 +1,140 @@
-# -*- coding: utf-8 -*-
-"""
-One-class classification
-@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
-"""
-
-from deepod.core.base_model import BaseDeepAD
-from deepod.core.base_networks import MLPnet
-from torch.utils.data import DataLoader
-import torch
-
-
-class DeepSVDD(BaseDeepAD):
-    """ Deep One-class Classification (Deep SVDD) for anomaly detection
-    See :cite:`ruff2018deepsvdd` for details
-
-    Parameters
-    ----------
-    epochs: int, optional (default=100)
-        Number of training epochs
-
-    batch_size: int, optional (default=64)
-        Number of samples in a mini-batch
-
-    lr: float, optional (default=1e-3)
-        Learning rate
-
-    rep_dim: int, optional (default=128)
-        Dimensionality of the representation space
-
-    hidden_dims: list, str or int, optional (default='100,50')
-        Number of neural units in hidden layers
-            - If list, each item is a layer
-            - If str, neural units of hidden layers are split by comma
-            - If int, number of neural units of single hidden layer
-
-    act: str, optional (default='ReLU')
-        activation layer name
-        choice = ['ReLU', 'LeakyReLU', 'Sigmoid', 'Tanh']
-
-    bias: bool, optional (default=False)
-        Additive bias in linear layer
-
-    epoch_steps: int, optional (default=-1)
-        Maximum steps in an epoch
-            - If -1, all the batches will be processed
-
-    prt_steps: int, optional (default=10)
-        Number of epoch intervals per printing
-
-    device: str, optional (default='cuda')
-        torch device,
-
-    verbose: int, optional (default=1)
-        Verbosity mode
-
-    random_state： int, optional (default=42)
-        the seed used by the random
-
-    """
-    def __init__(self, epochs=100, batch_size=64, lr=1e-3,
-                 rep_dim=128, hidden_dims='100,50', act='ReLU', bias=False,
-                 epoch_steps=-1, prt_steps=10, device='cuda',
-                 verbose=2, random_state=42):
-        super(DeepSVDD, self).__init__(
-            model_name='DeepSVDD', epochs=epochs, batch_size=batch_size, lr=lr,
-            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
-            verbose=verbose, random_state=random_state
-        )
-
-        self.hidden_dims = hidden_dims
-        self.rep_dim = rep_dim
-        self.act = act
-        self.bias = bias
-
-        self.c = None
-
-        # setattr(self,k,v)
-
-        return
-
-    def training_prepare(self, X, y):
-        train_loader = DataLoader(X, batch_size=self.batch_size, shuffle=True)
-
-        net = MLPnet(
-            n_features=self.n_features,
-            n_hidden=self.hidden_dims,
-            n_output=self.rep_dim,
-            activation=self.act,
-            bias=self.bias,
-        ).to(self.device)
-
-        # self.c = torch.randn(net.n_emb).to(self.device)
-        self.c = self._set_c(net, train_loader)
-        criterion = DSVDDLoss(c=self.c)
-
-        if self.verbose >= 2:
-            print(net)
-
-        return train_loader, net, criterion
-
-    def inference_prepare(self, X):
-        test_loader = DataLoader(X, batch_size=self.batch_size,
-                                 drop_last=False, shuffle=False)
-        self.criterion.reduction = 'none'
-        return test_loader
-
-    def training_forward(self, batch_x, net, criterion):
-        batch_x = batch_x.float().to(self.device)
-        z = net(batch_x)
-        loss = criterion(z)
-        return loss
-
-    def inference_forward(self, batch_x, net, criterion):
-        batch_x = batch_x.float().to(self.device)
-        batch_z = net(batch_x)
-        s = criterion(batch_z)
-        return batch_z, s
-
-    def _set_c(self, net, dataloader, eps=0.1):
-        """Initializing the center for the hypersphere"""
-        net.eval()
-        z_ = []
-        with torch.no_grad():
-            for x in dataloader:
-                x = x.float().to(self.device)
-                z = net(x)
-                z_.append(z.detach())
-        z_ = torch.cat(z_)
-        c = torch.mean(z_, dim=0)
-        c[(abs(c) < eps) & (c < 0)] = -eps
-        c[(abs(c) < eps) & (c > 0)] = eps
-        return c
-
-
-class DSVDDLoss(torch.nn.Module):
-    """
-
-    Parameters
-    ----------
-    c: torch.Tensor
-        Center of the pre-defined hyper-sphere in the representation space
-
-    reduction: str, optional (default='mean')
-        choice = [``'none'`` | ``'mean'`` | ``'sum'``]
-            - If ``'none'``: no reduction will be applied;
-            - If ``'mean'``: the sum of the output will be divided by the number of
-            elements in the output;
-            - If ``'sum'``: the output will be summed
-
-    """
-    def __init__(self, c, reduction='mean'):
-        super(DSVDDLoss, self).__init__()
-        self.c = c
-        self.reduction = reduction
-
-    def forward(self, rep, reduction=None):
-        loss = torch.sum((rep - self.c) ** 2, dim=1)
-
-        if reduction is None:
-            reduction = self.reduction
-
-        if reduction == 'mean':
-            return torch.mean(loss)
-        elif reduction == 'sum':
-            return torch.sum(loss)
-        elif reduction == 'none':
-            return loss
-
-
-if __name__ == '__main__':
-    import numpy as np
-
-    file = '../../data/38_thyroid.npz'
-    data = np.load(file, allow_pickle=True)
-    x, y = data['X'], data['y']
-    y = np.array(y, dtype=int)
-
-    anom_id = np.where(y==1)[0]
-    known_anom_id = np.random.choice(anom_id, 30)
-    y_semi = np.zeros_like(y)
-    y_semi[known_anom_id] = 1
-
-    clf = DeepSVDD(device='cpu')
-    clf.fit(x, y_semi)
-
-    scores = clf.decision_function(x)
-
-    from sklearn.metrics import roc_auc_score
-
-    auc = roc_auc_score(y_score=scores, y_true=y)
-
-    print(auc)
+# -*- coding: utf-8 -*-
+"""
+Random distance prediction-based anomaly detection
+this script is partially adapted from https://github.com/billhhh/RDP
+@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
+"""
+
+from deepod.core.base_model import BaseDeepAD
+from deepod.core.base_networks import MLPnet
+from torch.utils.data import DataLoader
+import torch.nn.functional as F
+import torch
+import copy
+
+
+class RDP(BaseDeepAD):
+    """
+    Parameters
+    ----------
+    epochs: int, optional (default=100)
+        Number of training epochs
+
+    batch_size: int, optional (default=64)
+        Number of samples in a mini-batch
+
+    lr: float, optional (default=1e-3)
+        Learning rate
+
+    rep_dim: int, optional (default=128)
+        Dimensionality of the representation space
+
+    hidden_dims: list, str or int, optional (default='100,50')
+        Number of neural units in hidden layers
+            - If list, each item is a layer
+            - If str, neural units of hidden layers are split by comma
+            - If int, number of neural units of single hidden layer
+
+    act: str, optional (default='ReLU')
+        activation layer name
+        choice = ['ReLU', 'LeakyReLU', 'Sigmoid', 'Tanh']
+
+    bias: bool, optional (default=False)
+        Additive bias in linear layer
+
+    epoch_steps: int, optional (default=-1)
+        Maximum steps in an epoch
+            - If -1, all the batches will be processed
+
+    prt_steps: int, optional (default=10)
+        Number of epoch intervals per printing
+
+    device: str, optional (default='cuda')
+        torch device,
+
+    verbose: int, optional (default=1)
+        Verbosity mode
+
+    random_state： int, optional (default=42)
+        the seed used by the random
+    """
+    def __init__(self, epochs=100, batch_size=64, lr=1e-3,
+                 rep_dim=128, hidden_dims='100,50', act='LeakyReLU', bias=False,
+                 epoch_steps=-1, prt_steps=10, device='cuda',
+                 verbose=2, random_state=42):
+        super(RDP, self).__init__(
+            model_name='RDP', epochs=epochs, batch_size=batch_size, lr=lr,
+            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
+            verbose=verbose, random_state=random_state
+        )
+
+        self.hidden_dims = hidden_dims
+        self.rep_dim = rep_dim
+        self.act = act
+        self.bias = bias
+        return
+
+    def training_prepare(self, X, y):
+        train_loader = DataLoader(X, batch_size=self.batch_size, shuffle=True)
+
+        net = MLPnet(
+            n_features=self.n_features,
+            n_hidden=self.hidden_dims, n_output=self.rep_dim,
+            activation=self.act, bias=self.bias,
+            skip_connection=None,
+        ).to(self.device)
+
+        rp_net = copy.deepcopy(net)
+        criterion = RDPLoss(rp_net)
+
+        if self.verbose >= 2:
+            print(net)
+
+        return train_loader, net, criterion
+
+    def inference_prepare(self, X):
+        test_loader = DataLoader(X, batch_size=self.batch_size, drop_last=False, shuffle=False)
+        self.criterion.reduction = 'none'
+        return test_loader
+
+    def training_forward(self, batch_x, net, criterion):
+        batch_x1 = batch_x[torch.randperm(batch_x.shape[0])]
+        batch_x = batch_x.float().to(self.device)
+        batch_x1 = batch_x1.float().to(self.device)
+        z, z1 = net(batch_x), net(batch_x1)
+        loss = criterion(z, z1, batch_x, batch_x1)
+        return loss
+
+    def inference_forward(self, batch_x, net, criterion):
+        batch_x = batch_x.float().to(self.device)
+        batch_x1 = batch_x[torch.randperm(batch_x.shape[0])]
+        batch_z, batch_z1 = net(batch_x), net(batch_x1)
+        s = criterion(batch_z, batch_z1, batch_x, batch_x1)
+        return batch_z, s
+
+
+class RDPLoss(torch.nn.Module):
+    def __init__(self, random_projection_net, reduction='mean'):
+        super(RDPLoss, self).__init__()
+        self.rp_net = random_projection_net
+        self.mse = torch.nn.MSELoss(reduction=reduction)
+        self.reduction = reduction
+
+    def forward(self, rep, rep1, x, x1):
+        rep_target = self.rp_net(x)
+        rep1_target = self.rp_net(x1)
+
+        d_target = torch.sum(F.normalize(rep_target, p=1, dim=1) *
+                             F.normalize(rep1_target, p=1, dim=1), dim=1)
+        d_pred = torch.sum(F.normalize(rep, p=1, dim=1) *
+                           F.normalize(rep1, p=1, dim=1), dim=1)
+
+        if self.reduction == 'mean' or self.reduction == 'sum':
+            gap_loss = self.mse(rep, rep_target)
+            rdp_loss = self.mse(d_target, d_pred)
+
+        else:
+            gap_loss = torch.mean(F.mse_loss(rep, rep_target, reduction='none'), dim=1)
+            rdp_loss = F.mse_loss(d_target, d_pred, reduction='none')
+
+        return gap_loss + rdp_loss
```

### Comparing `deepod-0.2.0/deepod/models/goad.py` & `deepod-0.3.0/deepod/models/goad.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,222 +1,194 @@
-# -*- coding: utf-8 -*-
-"""
-Classification-based anomaly detection
-this script is partially adapted from https://github.com/lironber/GOAD
-License: https://github.com/lironber/GOAD/blob/master/LICENSE
-@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
-"""
-
-from deepod.core.base_model import BaseDeepAD
-from deepod.core.base_networks import ConvNet
-from torch.utils.data import DataLoader, TensorDataset
-import torch.nn.functional as F
-import torch
-import numpy as np
-
-
-class GOAD(BaseDeepAD):
-    def __init__(self, epochs=100, batch_size=64, lr=1e-3,
-                 n_trans=256, trans_dim=32,
-                 alpha=0.1, margin=1., eps=0,
-                 kernel_size=1, hidden_dim=8, n_layers=5,
-                 act='LeakyReLU', bias=False,
-                 epoch_steps=-1, prt_steps=10, device='cuda',
-                 verbose=2, random_state=42):
-        super(GOAD, self).__init__(
-            model_name='GOAD', epochs=epochs, batch_size=batch_size, lr=lr,
-            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
-            verbose=verbose, random_state=random_state
-        )
-
-        self.n_trans = n_trans
-        self.trans_dim = trans_dim
-
-        self.alpha = alpha
-        self.margin = margin
-        self.eps = eps
-
-        self.kernel_size = kernel_size
-        self.hidden_dim = hidden_dim
-        self.n_layers = n_layers
-        self.act = act
-        self.bias = bias
-
-        self.affine_weights = None
-        self.rep_means = None
-        return
-
-    def training_prepare(self, X, y):
-        self.affine_weights = np.random.randn(self.n_trans, self.n_features, self.trans_dim)
-        x_trans = np.stack([X.dot(rot) for rot in self.affine_weights], 2) # shape: [n_samples, trans_dim, n_trans]
-        x_trans = torch.from_numpy(x_trans).float()
-        labels = torch.arange(self.n_trans).unsqueeze(0).expand((X.shape[0], self.n_trans))
-        labels = labels.long()
-
-        if self.verbose >= 2:
-            print(f'{self.n_trans} transformation done')
-
-        dataset = TensorDataset(x_trans, labels)
-        train_loader = DataLoader(dataset, batch_size=self.batch_size, shuffle=True)
-
-        net = GoadNet(
-            self.trans_dim,
-            kernel_size=self.kernel_size,
-            n_hidden=self.hidden_dim,
-            n_layers=self.n_layers,
-            n_output=self.n_trans,
-            activation=self.act, bias=False
-        ).to(self.device)
-        weights_init(net)
-
-        criterion = GoadLoss(alpha=self.alpha, margin=self.margin, device=self.device)
-
-        if self.verbose >= 2:
-            print(net)
-
-        return train_loader, net, criterion
-
-    def inference_prepare(self, X):
-        x_trans = np.stack([X.dot(rot) for rot in self.affine_weights], 2)
-        x_trans = torch.from_numpy(x_trans).float()
-
-        test_loader = DataLoader(x_trans,
-                                 batch_size=self.batch_size,
-                                 drop_last=False,
-                                 shuffle=False)
-
-        # # prepare means:
-        self.net.eval()
-        sum_reps = torch.zeros((self.hidden_dim, self.n_trans)).to(self.device)
-        with torch.no_grad():
-            nb = 0
-            for batch in self.train_loader:
-                batch_data, batch_target = batch
-                batch_data = batch_data.float().to(self.device)
-                rep, _ = self.net(batch_data)
-                sum_reps += rep.mean(0)
-                nb += 1
-
-        reps = sum_reps.t() / nb
-        reps = reps.unsqueeze(0)
-        self.rep_means = reps
-
-        # print(self.rep_means)
-
-        return test_loader
-
-    def training_forward(self, batch_x, net, criterion):
-        batch_data, batch_target = batch_x
-        batch_data = batch_data.float().to(self.device)
-        batch_target = batch_target.long().to(self.device)
-
-        batch_rep, batch_pred = net(batch_data)
-        batch_rep = batch_rep.permute(0, 2, 1)
-
-        loss = criterion(batch_rep, batch_pred, batch_target)
-        return loss
-
-    def inference_forward(self, batch_x, net, criterion):
-        batch_data = batch_x.float().to(self.device)
-
-        batch_rep, _ = net(batch_data)
-        batch_rep = batch_rep.permute(0, 2, 1)
-
-        diffs = ((batch_rep.unsqueeze(2) - self.rep_means) ** 2).sum(-1)
-        diffs_eps = self.eps * torch.ones_like(diffs)
-        diffs = torch.max(diffs, diffs_eps)
-
-        logp_sz = torch.nn.functional.log_softmax(-diffs, dim=2)
-        s = -torch.diagonal(logp_sz, 0, 1, 2)
-        s = s.sum(1)
-        return batch_rep, s
-
-
-class GoadNet(torch.nn.Module):
-    def __init__(self, n_input,
-                 kernel_size=1, n_hidden=8, n_layers=5, n_output=256,
-                 activation='LeakyReLU', bias=False):
-        super(GoadNet, self).__init__()
-
-        self.enc = ConvNet(
-            n_features=n_input,
-            kernel_size=kernel_size,
-            n_hidden=n_hidden,
-            n_layers=n_layers,
-            activation=activation,
-            bias=bias
-        )
-
-        self.head = torch.nn.Sequential(
-            torch.nn.LeakyReLU(negative_slope=0.2, inplace=True),
-            torch.nn.Conv1d(n_hidden, n_output,
-                            kernel_size=kernel_size, bias=True)
-        )
-        return
-
-    def forward(self, x):
-        rep = self.enc(x)
-        pred = self.head(rep)
-        return rep, pred
-
-
-class GoadLoss(torch.nn.Module):
-    def __init__(self, alpha=0.1, margin=1., device='cuda'):
-        super(GoadLoss, self).__init__()
-        self.ce_criterion = torch.nn.CrossEntropyLoss()
-        self.alpha = alpha
-        self.margin = margin
-        self.device = device
-        return 
-
-    def forward(self, rep, pred, labels):
-        loss_ce = self.ce_criterion(pred, labels)
-
-        means = rep.mean(0).unsqueeze(0)
-        res = ((rep.unsqueeze(2) - means.unsqueeze(1)) ** 2).sum(-1)
-        pos = torch.diagonal(res, dim1=1, dim2=2)
-        offset = torch.diagflat(torch.ones(rep.size(1))).unsqueeze(0).to(self.device) * 1e6
-        neg = (res + offset).min(-1)[0]
-        loss_tc = torch.clamp(pos + self.margin - neg, min=0).mean()
-
-        loss = self.alpha * loss_tc + loss_ce
-        return loss
-
-
-def weights_init(m):
-    classname = m.__class__.__name__
-    if isinstance(m, torch.nn.Linear):
-        torch.nn.init.xavier_normal_(m.weight, gain=np.sqrt(2.0))
-    elif classname.find('Conv') != -1:
-        torch.nn.init.xavier_normal_(m.weight, gain=np.sqrt(2.0))
-    elif classname.find('Linear') != -1:
-        torch.nn.init.eye_(m.weight)
-    elif classname.find('Emb') != -1:
-        torch.nn.init.normal(m.weight, mean=0, std=0.01)
-
-
-
-
-if __name__ == '__main__':
-    import pandas as pd
-    import numpy as np
-
-    file = '../../data/38_thyroid.npz'
-    data = np.load(file, allow_pickle=True)
-    x, y = data['X'], data['y']
-    y = np.array(y, dtype=int)
-
-    anom_id = np.where(y==1)[0]
-    known_anom_id = np.random.choice(anom_id, 30)
-    y_semi = np.zeros_like(y)
-    y_semi[known_anom_id] = 1
-
-    clf = GOAD(device='cpu', epochs=1)
-    clf.fit(x, y_semi)
-
-    scores = clf.decision_function(x)
-
-    from sklearn.metrics import roc_auc_score
-
-    auc = roc_auc_score(y_score=scores, y_true=y)
-
-    print(auc)
+# -*- coding: utf-8 -*-
+"""
+Classification-based anomaly detection
+this script is partially adapted from https://github.com/lironber/GOAD
+License: https://github.com/lironber/GOAD/blob/master/LICENSE
+@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
+"""
+
+from deepod.core.base_model import BaseDeepAD
+from deepod.core.base_networks import ConvNet
+from torch.utils.data import DataLoader, TensorDataset
+import torch.nn.functional as F
+import torch
+import numpy as np
+
+
+class GOAD(BaseDeepAD):
+    def __init__(self, epochs=100, batch_size=64, lr=1e-3,
+                 n_trans=256, trans_dim=32,
+                 alpha=0.1, margin=1., eps=0,
+                 kernel_size=1, hidden_dim=8, n_layers=5,
+                 act='LeakyReLU', bias=False,
+                 epoch_steps=-1, prt_steps=10, device='cuda',
+                 verbose=2, random_state=42):
+        super(GOAD, self).__init__(
+            model_name='GOAD', epochs=epochs, batch_size=batch_size, lr=lr,
+            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
+            verbose=verbose, random_state=random_state
+        )
+
+        self.n_trans = n_trans
+        self.trans_dim = trans_dim
+
+        self.alpha = alpha
+        self.margin = margin
+        self.eps = eps
+
+        self.kernel_size = kernel_size
+        self.hidden_dim = hidden_dim
+        self.n_layers = n_layers
+        self.act = act
+        self.bias = bias
+
+        self.affine_weights = None
+        self.rep_means = None
+        return
+
+    def training_prepare(self, X, y):
+        self.affine_weights = np.random.randn(self.n_trans, self.n_features, self.trans_dim)
+        x_trans = np.stack([X.dot(rot) for rot in self.affine_weights], 2) # shape: [n_samples, trans_dim, n_trans]
+        x_trans = torch.from_numpy(x_trans).float()
+        labels = torch.arange(self.n_trans).unsqueeze(0).expand((X.shape[0], self.n_trans))
+        labels = labels.long()
+
+        if self.verbose >= 2:
+            print(f'{self.n_trans} transformation done')
+
+        dataset = TensorDataset(x_trans, labels)
+        train_loader = DataLoader(dataset, batch_size=self.batch_size, shuffle=True)
+
+        net = GoadNet(
+            self.trans_dim,
+            kernel_size=self.kernel_size,
+            n_hidden=self.hidden_dim,
+            n_layers=self.n_layers,
+            n_output=self.n_trans,
+            activation=self.act, bias=False
+        ).to(self.device)
+        weights_init(net)
+
+        criterion = GoadLoss(alpha=self.alpha, margin=self.margin, device=self.device)
+
+        if self.verbose >= 2:
+            print(net)
+
+        return train_loader, net, criterion
+
+    def inference_prepare(self, X):
+        x_trans = np.stack([X.dot(rot) for rot in self.affine_weights], 2)
+        x_trans = torch.from_numpy(x_trans).float()
+
+        test_loader = DataLoader(x_trans,
+                                 batch_size=self.batch_size,
+                                 drop_last=False,
+                                 shuffle=False)
+
+        # # prepare means:
+        self.net.eval()
+        sum_reps = torch.zeros((self.hidden_dim, self.n_trans)).to(self.device)
+        with torch.no_grad():
+            nb = 0
+            for batch in self.train_loader:
+                batch_data, batch_target = batch
+                batch_data = batch_data.float().to(self.device)
+                rep, _ = self.net(batch_data)
+                sum_reps += rep.mean(0)
+                nb += 1
+
+        reps = sum_reps.t() / nb
+        reps = reps.unsqueeze(0)
+        self.rep_means = reps
+
+        # print(self.rep_means)
+
+        return test_loader
+
+    def training_forward(self, batch_x, net, criterion):
+        batch_data, batch_target = batch_x
+        batch_data = batch_data.float().to(self.device)
+        batch_target = batch_target.long().to(self.device)
+
+        batch_rep, batch_pred = net(batch_data)
+        batch_rep = batch_rep.permute(0, 2, 1)
+
+        loss = criterion(batch_rep, batch_pred, batch_target)
+        return loss
+
+    def inference_forward(self, batch_x, net, criterion):
+        batch_data = batch_x.float().to(self.device)
+
+        batch_rep, _ = net(batch_data)
+        batch_rep = batch_rep.permute(0, 2, 1)
+
+        diffs = ((batch_rep.unsqueeze(2) - self.rep_means) ** 2).sum(-1)
+        diffs_eps = self.eps * torch.ones_like(diffs)
+        diffs = torch.max(diffs, diffs_eps)
+
+        logp_sz = torch.nn.functional.log_softmax(-diffs, dim=2)
+        s = -torch.diagonal(logp_sz, 0, 1, 2)
+        s = s.sum(1)
+        return batch_rep, s
+
+
+class GoadNet(torch.nn.Module):
+    def __init__(self, n_input,
+                 kernel_size=1, n_hidden=8, n_layers=5, n_output=256,
+                 activation='LeakyReLU', bias=False):
+        super(GoadNet, self).__init__()
+
+        self.enc = ConvNet(
+            n_features=n_input,
+            kernel_size=kernel_size,
+            n_hidden=n_hidden,
+            n_layers=n_layers,
+            activation=activation,
+            bias=bias
+        )
+
+        self.head = torch.nn.Sequential(
+            torch.nn.LeakyReLU(negative_slope=0.2, inplace=True),
+            torch.nn.Conv1d(n_hidden, n_output,
+                            kernel_size=kernel_size, bias=True)
+        )
+        return
+
+    def forward(self, x):
+        rep = self.enc(x)
+        pred = self.head(rep)
+        return rep, pred
+
+
+class GoadLoss(torch.nn.Module):
+    def __init__(self, alpha=0.1, margin=1., device='cuda'):
+        super(GoadLoss, self).__init__()
+        self.ce_criterion = torch.nn.CrossEntropyLoss()
+        self.alpha = alpha
+        self.margin = margin
+        self.device = device
+        return 
+
+    def forward(self, rep, pred, labels):
+        loss_ce = self.ce_criterion(pred, labels)
+
+        means = rep.mean(0).unsqueeze(0)
+        res = ((rep.unsqueeze(2) - means.unsqueeze(1)) ** 2).sum(-1)
+        pos = torch.diagonal(res, dim1=1, dim2=2)
+        offset = torch.diagflat(torch.ones(rep.size(1))).unsqueeze(0).to(self.device) * 1e6
+        neg = (res + offset).min(-1)[0]
+        loss_tc = torch.clamp(pos + self.margin - neg, min=0).mean()
+
+        loss = self.alpha * loss_tc + loss_ce
+        return loss
+
+
+def weights_init(m):
+    classname = m.__class__.__name__
+    if isinstance(m, torch.nn.Linear):
+        torch.nn.init.xavier_normal_(m.weight, gain=np.sqrt(2.0))
+    elif classname.find('Conv') != -1:
+        torch.nn.init.xavier_normal_(m.weight, gain=np.sqrt(2.0))
+    elif classname.find('Linear') != -1:
+        torch.nn.init.eye_(m.weight)
+    elif classname.find('Emb') != -1:
+        torch.nn.init.normal(m.weight, mean=0, std=0.01)
```

### Comparing `deepod-0.2.0/deepod/models/icl.py` & `deepod-0.3.0/deepod/models/icl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,322 +1,281 @@
-# -*- coding: utf-8 -*-
-"""
-Anomaly Detection for Tabular Data with Internal Contrastive Learning
-this script is partially adapted from the supplementary material in
-https://openreview.net/forum?id=_hszZbt46bT
-@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
-"""
-
-from deepod.core.base_model import BaseDeepAD
-from deepod.core.base_networks import MLPnet
-from torch.utils.data import DataLoader
-import torch
-import torch.nn.functional as F
-import numpy as np
-
-
-class ICL(BaseDeepAD):
-    """ Anomaly Detection for Tabular Data with Internal Contrastive Learning (ICL for short)
-    See :cite:`shenkar2022internal` for details
-
-    Parameters
-    ----------
-    epochs: int, optional (default=100)
-        Number of training epochs
-
-    batch_size: int, optional (default=64)
-        Number of samples in a mini-batch
-
-    lr: float, optional (default=1e-3)
-        Learning rate
-
-    n_ensemble: int, optional (default=2)
-        Number of the ensemble size (make use of the bagging effect)
-
-    rep_dim: int, optional (default=128)
-        Dimensionality of the representation space
-
-    hidden_dims: List, str or int, optional (default='100,50')
-        Number of neural units in hidden layers
-            - If List, each item is a layer
-            - If str, neural units of hidden layers are split by comma
-            - If int, number of neural units of single hidden layer
-
-    act: str, optional (default='ReLU')
-        activation layer name
-        choice = ['ReLU', 'LeakyReLU', 'Sigmoid', 'Tanh']
-
-    bias: bool, optional (default=False)
-        Additive bias in linear layer
-
-    kernel_size: str or int, optional (default='auto')
-        the length of sub-vectors
-
-    temperature: float, optional (default=0.01)
-        tau in the cross-entropy function
-
-    max_negatives: int, optional (default=1000)
-        Maximum number of negatives (unmatched sub-vectors)
-
-    epoch_steps: int, optional (default=-1)
-        Maximum steps in an epoch
-            - If -1, all the batches will be processed
-
-    prt_steps: int, optional (default=10)
-        Number of epoch intervals per printing
-
-    device: str, optional (default='cuda')
-        torch device,
-
-    verbose: int, optional (default=1)
-        Verbosity mode
-
-    random_state： int, optional (default=42)
-        the seed used by the random
-
-    """
-    def __init__(self, epochs=100, batch_size=64, lr=1e-3, n_ensemble='auto',
-                 rep_dim=128, hidden_dims='100,50', act='LeakyReLU', bias=False,
-                 kernel_size='auto', temperature=0.01, max_negatives=1000,
-                 epoch_steps=-1, prt_steps=10, device='cuda',
-                 verbose=2, random_state=42):
-        super(ICL, self).__init__(
-            model_name='ICL', epochs=epochs, batch_size=batch_size,
-            lr=lr, n_ensemble=n_ensemble,
-            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
-            verbose=verbose, random_state=random_state
-        )
-
-        self.hidden_dims = hidden_dims
-        self.rep_dim = rep_dim
-        self.act = act
-        self.bias = bias
-
-        self.kernel_size = kernel_size
-        self.tau = temperature
-        self.max_negatives = max_negatives
-
-        return
-
-    def training_prepare(self, X, y):
-        train_loader = DataLoader(X, batch_size=self.batch_size,
-                                  shuffle=True, pin_memory=True)
-
-        if self.kernel_size == 'auto':
-            if self.n_features <= 40:
-                self.kernel_size = 2
-            elif 40 < self.n_features <= 160:
-                self.kernel_size = 10
-
-            # else:
-            #     self.kernel_size = self.n_features - 150
-
-            elif 160 < self.n_features <= 240:
-                self.kernel_size = self.n_features - 150
-            elif 240 < self.n_features <= 480:
-                self.kernel_size = self.n_features - 200
-            else:
-                self.kernel_size = self.n_features - 400
-
-            # elif 320 < self.n_features <= 480:
-            #     self.kernel_size = self.n_features - 300
-            #
-            # else:
-            #     self.kernel_size = self.n_features - 450
-
-        if self.verbose >= 1:
-            print(f'kernel size: {self.kernel_size}')
-
-        net = ICLNet(
-            n_features=self.n_features,
-            kernel_size=self.kernel_size,
-            hidden_dims=self.hidden_dims,
-            rep_dim=self.rep_dim,
-            activation=self.act,
-            bias=self.bias
-        ).to(self.device)
-
-        criterion = torch.nn.CrossEntropyLoss()
-
-        if self.verbose >= 2:
-            print(net)
-
-        return train_loader, net, criterion
-
-    def training_forward(self, batch_x, net, criterion):
-        batch_x = batch_x.float().to(self.device)
-
-        # positives are sub-vectors, query are their complements
-        positives, query = net(batch_x)
-
-        logit = self.cal_logit(query, positives)
-        logit = logit.permute(0, 2, 1)
-
-        correct_class = torch.zeros((logit.shape[0], logit.shape[2]),
-                                    dtype=torch.long).to(self.device)
-        loss = criterion(logit, correct_class)
-        return loss
-
-    def inference_prepare(self, X):
-        test_loader = DataLoader(X, batch_size=self.batch_size,
-                                 drop_last=False, shuffle=False)
-        self.criterion.reduction = 'none'
-        return test_loader
-
-    def inference_forward(self, batch_x, net, criterion):
-        loss = self.training_forward(batch_x, net, criterion)
-        batch_z = batch_x # for consistency
-        s = loss.mean(dim=1)
-        return batch_z, s
-
-    def cal_logit(self, query, pos):
-        n_pos = query.shape[1]
-        batch_size = query.shape[0]
-
-        # get negatives
-        negative_index = np.random.choice(np.arange(n_pos), min(self.max_negatives, n_pos), replace=False)
-        negative = pos.permute(0, 2, 1)[:, :, negative_index]
-
-        pos_multiplication = (query * pos).sum(dim=2).unsqueeze(2)
-
-        neg_multiplication = torch.matmul(query, negative)  # [batch_size, n_neg, n_neg]
-
-        # Removal of the diagonals
-        identity_matrix = torch.eye(n_pos).unsqueeze(0).to(self.device)
-        identity_matrix = identity_matrix.repeat(batch_size, 1, 1)
-        identity_matrix = identity_matrix[:, :, negative_index]
-
-        neg_multiplication.masked_fill_(identity_matrix==1, -float('inf'))
-
-        logit = torch.cat((pos_multiplication, neg_multiplication), dim=2)
-        logit = torch.div(logit, self.tau)
-        return logit
-
-
-class ICLNet(torch.nn.Module):
-    def __init__(self, n_features, kernel_size,
-                 hidden_dims='100,50', rep_dim=64,
-                 activation='ReLU', bias=False):
-        super(ICLNet, self).__init__()
-        self.n_features = n_features
-        self.kernel_size = kernel_size
-
-        # get consecutive subspace indices and the corresponding complement indices
-        start_idx = np.arange(n_features)[: -kernel_size + 1]  # [0,1,2,...,dim-kernel_size+1]
-        self.all_idx = start_idx[:, None] + np.arange(kernel_size)
-        self.all_idx_complement = np.array([np.setdiff1d(np.arange(n_features), row)
-                                            for row in self.all_idx])
-
-        if type(hidden_dims)==str:
-            hidden_dims = hidden_dims.split(',')
-            hidden_dims = [int(a) for a in hidden_dims]
-        n_layers = len(hidden_dims) # hidden layers
-        f_act = ['Tanh']
-        for _ in range(n_layers):
-            f_act.append(activation)
-
-        self.enc_f_net = MLPnet(
-            n_features=n_features-kernel_size,
-            n_hidden=hidden_dims,
-            n_output=rep_dim,
-            mid_channels=len(self.all_idx),
-            batch_norm=True,
-            activation=f_act,
-            bias=bias,
-        )
-
-        hidden_dims2 = [int(0.5*h) for h in hidden_dims]
-        g_act = []
-        for _ in range(n_layers+1):
-            g_act.append(activation)
-
-        self.enc_g_net = MLPnet(
-            n_features=kernel_size,
-            n_hidden=hidden_dims2,
-            n_output=rep_dim,
-            mid_channels=len(self.all_idx),
-            batch_norm=True,
-            activation=g_act,
-            bias=bias,
-        )
-
-        return
-
-    def forward(self, x):
-        x1, x2 = self.positive_matrix_builder(data=x)
-        x1 = self.enc_g_net(x1)
-        x2 = self.enc_f_net(x2)
-        x1 = F.normalize(x1)
-        x2 = F.normalize(x2)
-        return x1, x2
-
-    def positive_matrix_builder(self, data):
-        """
-        Generate matrix of sub-vectors and matrix of complement vectors (positive pairs)
-
-        Parameters
-        ----------
-        data: torch.Tensor shape (n_samples, n_features), required
-            The input data.
-
-        Returns
-        -------
-        matrix: torch.Tensor of shape [n_samples, number of sub-vectors, kernel_size]
-            Derived sub-vectors.
-
-        complement_matrix: torch.Tensor of shape [n_samples, number of sub-vectors, n_features-kernel_size]
-            Complement vector of derived sub-vectors.
-
-        """
-        dim = self.n_features
-
-        data = torch.unsqueeze(data, 1)  # [size, 1, dim]
-        data = data.repeat(1, dim, 1)  # [size, dim, dim]
-
-        matrix = data[:, np.arange(self.all_idx.shape[0])[:, None], self.all_idx]
-        complement_matrix = data[:, np.arange(self.all_idx.shape[0])[:, None], self.all_idx_complement]
-
-        return matrix, complement_matrix
-
-
-if __name__ == '__main__':
-    import numpy as np
-    import pandas as pd
-
-    file = '/home/xuhz/dataset/1-tabular/fmnist.inlier_var.3percent.5dup/fmnist_anom7_nnormal9_id9_1.csv'
-    df = pd.read_csv(file)
-    df.replace([np.inf, -np.inf], np.nan, inplace=True)
-    df.fillna(method='ffill', inplace=True)
-    x = df.values[:, :-1]
-    y = np.array(df.values[:, -1], dtype=int)
-
-    norm_idx = np.where(y == 0)[0]
-    anom_idx = np.where(y == 1)[0]
-    split = int(0.5 * len(norm_idx))
-    train_norm_idx, test_norm_idx = norm_idx[:split], norm_idx[split:]
-
-    x_train = x[train_norm_idx]
-    y_train = y[train_norm_idx]
-
-    x_test = x[np.hstack([test_norm_idx, anom_idx])]
-    y_test = y[np.hstack([test_norm_idx, anom_idx])]
-    x_train = x_train / 255
-    x_test = x_test / 255
-
-    # file = '../../data/38_thyroid.npz'
-    # data_ = np.load(file, allow_pickle=True)
-    # x, y = data_['X'], data_['y']
-    # y = np.array(y, dtype=int)
-    # x_train = x
-    # x_test = x
-    # y_test = y
-
-    clf = ICL(device='cuda', epochs=100, hidden_dims='100', act='LeakyReLU', verbose=2)
-    clf.fit(x_train)
-
-    scores = clf.decision_function(x_test)
-
-    from sklearn.metrics import roc_auc_score
-
-    auc = roc_auc_score(y_score=scores, y_true=y_test)
-
-    print(auc)
+# -*- coding: utf-8 -*-
+"""
+Anomaly Detection for Tabular Data with Internal Contrastive Learning
+this script is partially adapted from the supplementary material in
+https://openreview.net/forum?id=_hszZbt46bT
+@Author: Hongzuo Xu <hongzuoxu@126.com, xuhongzuo13@nudt.edu.cn>
+"""
+
+from deepod.core.base_model import BaseDeepAD
+from deepod.core.base_networks import MLPnet
+from torch.utils.data import DataLoader
+import torch
+import torch.nn.functional as F
+import numpy as np
+
+
+class ICL(BaseDeepAD):
+    """ Anomaly Detection for Tabular Data with Internal Contrastive Learning (ICL for short)
+    See :cite:`shenkar2022internal` for details
+
+    Parameters
+    ----------
+    epochs: int, optional (default=100)
+        Number of training epochs
+
+    batch_size: int, optional (default=64)
+        Number of samples in a mini-batch
+
+    lr: float, optional (default=1e-3)
+        Learning rate
+
+    n_ensemble: int, optional (default=2)
+        Number of the ensemble size (make use of the bagging effect)
+
+    rep_dim: int, optional (default=128)
+        Dimensionality of the representation space
+
+    hidden_dims: List, str or int, optional (default='100,50')
+        Number of neural units in hidden layers
+            - If List, each item is a layer
+            - If str, neural units of hidden layers are split by comma
+            - If int, number of neural units of single hidden layer
+
+    act: str, optional (default='ReLU')
+        activation layer name
+        choice = ['ReLU', 'LeakyReLU', 'Sigmoid', 'Tanh']
+
+    bias: bool, optional (default=False)
+        Additive bias in linear layer
+
+    kernel_size: str or int, optional (default='auto')
+        the length of sub-vectors
+
+    temperature: float, optional (default=0.01)
+        tau in the cross-entropy function
+
+    max_negatives: int, optional (default=1000)
+        Maximum number of negatives (unmatched sub-vectors)
+
+    epoch_steps: int, optional (default=-1)
+        Maximum steps in an epoch
+            - If -1, all the batches will be processed
+
+    prt_steps: int, optional (default=10)
+        Number of epoch intervals per printing
+
+    device: str, optional (default='cuda')
+        torch device,
+
+    verbose: int, optional (default=1)
+        Verbosity mode
+
+    random_state： int, optional (default=42)
+        the seed used by the random
+
+    """
+    def __init__(self, epochs=100, batch_size=64, lr=1e-3, n_ensemble='auto',
+                 rep_dim=128, hidden_dims='100,50', act='LeakyReLU', bias=False,
+                 kernel_size='auto', temperature=0.01, max_negatives=1000,
+                 epoch_steps=-1, prt_steps=10, device='cuda',
+                 verbose=2, random_state=42):
+        super(ICL, self).__init__(
+            model_name='ICL', epochs=epochs, batch_size=batch_size,
+            lr=lr, n_ensemble=n_ensemble,
+            epoch_steps=epoch_steps, prt_steps=prt_steps, device=device,
+            verbose=verbose, random_state=random_state
+        )
+
+        self.hidden_dims = hidden_dims
+        self.rep_dim = rep_dim
+        self.act = act
+        self.bias = bias
+
+        self.kernel_size = kernel_size
+        self.tau = temperature
+        self.max_negatives = max_negatives
+
+        return
+
+    def training_prepare(self, X, y):
+        train_loader = DataLoader(X, batch_size=self.batch_size,
+                                  shuffle=True, pin_memory=True)
+
+        if self.kernel_size == 'auto':
+            if self.n_features <= 40:
+                self.kernel_size = 2
+            elif 40 < self.n_features <= 160:
+                self.kernel_size = 10
+
+            # else:
+            #     self.kernel_size = self.n_features - 150
+
+            elif 160 < self.n_features <= 240:
+                self.kernel_size = self.n_features - 150
+            elif 240 < self.n_features <= 480:
+                self.kernel_size = self.n_features - 200
+            else:
+                self.kernel_size = self.n_features - 400
+
+            # elif 320 < self.n_features <= 480:
+            #     self.kernel_size = self.n_features - 300
+            #
+            # else:
+            #     self.kernel_size = self.n_features - 450
+
+        if self.verbose >= 1:
+            print(f'kernel size: {self.kernel_size}')
+
+        if self.n_features < 3:
+            raise ValueError('ICL model cannot handle the data that have less than three features.')
+
+        net = ICLNet(
+            n_features=self.n_features,
+            kernel_size=self.kernel_size,
+            hidden_dims=self.hidden_dims,
+            rep_dim=self.rep_dim,
+            activation=self.act,
+            bias=self.bias
+        ).to(self.device)
+
+        criterion = torch.nn.CrossEntropyLoss()
+
+        if self.verbose >= 2:
+            print(net)
+
+        return train_loader, net, criterion
+
+    def training_forward(self, batch_x, net, criterion):
+        batch_x = batch_x.float().to(self.device)
+
+        # positives are sub-vectors, query are their complements
+        positives, query = net(batch_x)
+
+        logit = self.cal_logit(query, positives)
+        logit = logit.permute(0, 2, 1)
+
+        correct_class = torch.zeros((logit.shape[0], logit.shape[2]),
+                                    dtype=torch.long).to(self.device)
+        loss = criterion(logit, correct_class)
+        return loss
+
+    def inference_prepare(self, X):
+        test_loader = DataLoader(X, batch_size=self.batch_size,
+                                 drop_last=False, shuffle=False)
+        self.criterion.reduction = 'none'
+        return test_loader
+
+    def inference_forward(self, batch_x, net, criterion):
+        loss = self.training_forward(batch_x, net, criterion)
+        batch_z = batch_x # for consistency
+        s = loss.mean(dim=1)
+        return batch_z, s
+
+    def cal_logit(self, query, pos):
+        n_pos = query.shape[1]
+        batch_size = query.shape[0]
+
+        # get negatives
+        negative_index = np.random.choice(np.arange(n_pos), min(self.max_negatives, n_pos), replace=False)
+        negative = pos.permute(0, 2, 1)[:, :, negative_index]
+
+        pos_multiplication = (query * pos).sum(dim=2).unsqueeze(2)
+
+        neg_multiplication = torch.matmul(query, negative)  # [batch_size, n_neg, n_neg]
+
+        # Removal of the diagonals
+        identity_matrix = torch.eye(n_pos).unsqueeze(0).to(self.device)
+        identity_matrix = identity_matrix.repeat(batch_size, 1, 1)
+        identity_matrix = identity_matrix[:, :, negative_index]
+
+        neg_multiplication.masked_fill_(identity_matrix==1, -float('inf'))
+
+        logit = torch.cat((pos_multiplication, neg_multiplication), dim=2)
+        logit = torch.div(logit, self.tau)
+        return logit
+
+
+class ICLNet(torch.nn.Module):
+    def __init__(self, n_features, kernel_size,
+                 hidden_dims='100,50', rep_dim=64,
+                 activation='ReLU', bias=False):
+        super(ICLNet, self).__init__()
+        self.n_features = n_features
+        self.kernel_size = kernel_size
+
+        # get consecutive subspace indices and the corresponding complement indices
+        start_idx = np.arange(n_features)[: -kernel_size + 1]  # [0,1,2,...,dim-kernel_size+1]
+        self.all_idx = start_idx[:, None] + np.arange(kernel_size)
+        self.all_idx_complement = np.array([np.setdiff1d(np.arange(n_features), row)
+                                            for row in self.all_idx])
+
+        if type(hidden_dims)==str:
+            hidden_dims = hidden_dims.split(',')
+            hidden_dims = [int(a) for a in hidden_dims]
+        n_layers = len(hidden_dims) # hidden layers
+        f_act = ['Tanh']
+        for _ in range(n_layers):
+            f_act.append(activation)
+
+        self.enc_f_net = MLPnet(
+            n_features=n_features-kernel_size,
+            n_hidden=hidden_dims,
+            n_output=rep_dim,
+            mid_channels=len(self.all_idx),
+            batch_norm=True,
+            activation=f_act,
+            bias=bias,
+        )
+
+        hidden_dims2 = [int(0.5*h) for h in hidden_dims]
+        g_act = []
+        for _ in range(n_layers+1):
+            g_act.append(activation)
+
+        self.enc_g_net = MLPnet(
+            n_features=kernel_size,
+            n_hidden=hidden_dims2,
+            n_output=rep_dim,
+            mid_channels=len(self.all_idx),
+            batch_norm=True,
+            activation=g_act,
+            bias=bias,
+        )
+
+        return
+
+    def forward(self, x):
+        x1, x2 = self.positive_matrix_builder(data=x)
+        x1 = self.enc_g_net(x1)
+        x2 = self.enc_f_net(x2)
+        x1 = F.normalize(x1)
+        x2 = F.normalize(x2)
+        return x1, x2
+
+    def positive_matrix_builder(self, data):
+        """
+        Generate matrix of sub-vectors and matrix of complement vectors (positive pairs)
+
+        Parameters
+        ----------
+        data: torch.Tensor shape (n_samples, n_features), required
+            The input data.
+
+        Returns
+        -------
+        matrix: torch.Tensor of shape [n_samples, number of sub-vectors, kernel_size]
+            Derived sub-vectors.
+
+        complement_matrix: torch.Tensor of shape [n_samples, number of sub-vectors, n_features-kernel_size]
+            Complement vector of derived sub-vectors.
+
+        """
+        dim = self.n_features
+
+        data = torch.unsqueeze(data, 1)  # [size, 1, dim]
+        data = data.repeat(1, dim, 1)  # [size, dim, dim]
+
+        matrix = data[:, np.arange(self.all_idx.shape[0])[:, None], self.all_idx]
+        complement_matrix = data[:, np.arange(self.all_idx.shape[0])[:, None], self.all_idx_complement]
+
+        return matrix, complement_matrix
```

### Comparing `deepod-0.2.0/deepod/test/test_devnet.py` & `deepod-0.3.0/deepod/test/test_icl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,164 +1,148 @@
-# -*- coding: utf-8 -*-
-from __future__ import division
-from __future__ import print_function
-
-import os
-import sys
-import unittest
-
-# noinspection PyProtectedMember
-from numpy.testing import assert_allclose
-from numpy.testing import assert_array_less
-from numpy.testing import assert_equal
-from numpy.testing import assert_raises
-from scipy.stats import rankdata
-from sklearn.base import clone
-from sklearn.metrics import roc_auc_score
-import torch
-
-# temporary solution for relative imports in case pyod is not installed
-# if deepod is installed, no need to use the following line
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-
-from deepod.models.devnet import DevNet
-from deepod.utils.data import generate_data
-import numpy as np
-
-
-class TestDevNet(unittest.TestCase):
-    def setUp(self):
-        self.n_train = 200
-        self.n_test = 100
-        self.contamination = 0.1
-        self.roc_floor = 0.8
-
-        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
-            n_train=self.n_train, n_test=self.n_test, n_features=10,
-            contamination=self.contamination, random_state=42)
-
-        # file = '../../data/38_thyroid.npz'
-        # data = np.load(file, allow_pickle=True)
-        # x, y = data['X'], data['y']
-        # y = np.array(y, dtype=int)
-
-        anom_id = np.where(self.y_train == 1)[0]
-        known_anom_id = np.random.choice(anom_id, 10, replace=False)
-        y_semi = np.zeros_like(self.y_train, dtype=int)
-        y_semi[known_anom_id] = 1
-
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        self.clf = DevNet(epochs=1, hidden_dims=20, device=device,
-                          random_state=42)
-        self.clf.fit(self.X_train, y_semi)
-
-    def test_parameters(self):
-        assert (hasattr(self.clf, 'decision_scores_') and
-                self.clf.decision_scores_ is not None)
-        assert (hasattr(self.clf, 'labels_') and
-                self.clf.labels_ is not None)
-        assert (hasattr(self.clf, 'threshold_') and
-                self.clf.threshold_ is not None)
-
-    # def test_train_scores(self):
-    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
-
-    def test_prediction_scores(self):
-        pred_scores = self.clf.decision_function(self.X_test)
-        print(pred_scores)
-        print(self.y_test)
-
-        # check score shapes
-        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
-
-        # check performance
-        auc = roc_auc_score(self.y_test, pred_scores)
-        assert (auc >= self.roc_floor), f'auc is {auc}'
-
-    def test_prediction_labels(self):
-        pred_labels = self.clf.predict(self.X_test)
-        assert_equal(pred_labels.shape, self.y_test.shape)
-
-    # def test_prediction_proba(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_linear(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_unify(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_parameter(self):
-    #     with assert_raises(ValueError):
-    #         self.clf.predict_proba(self.X_test, method='something')
-
-    def test_prediction_labels_confidence(self):
-        pred_labels, confidence = self.clf.predict(self.X_test,
-                                                   return_confidence=True)
-
-        assert_equal(pred_labels.shape, self.y_test.shape)
-        assert_equal(confidence.shape, self.y_test.shape)
-        assert (confidence.min() >= 0)
-        assert (confidence.max() <= 1)
-
-    # def test_prediction_proba_linear_confidence(self):
-    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
-    #                                                     method='linear',
-    #                                                     return_confidence=True)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    #     assert_equal(confidence.shape, self.y_test.shape)
-    #     assert (confidence.min() >= 0)
-    #     assert (confidence.max() <= 1)
-    #
-    # def test_fit_predict(self):
-    #     pred_labels = self.clf.fit_predict(self.X_train)
-    #     assert_equal(pred_labels.shape, self.y_train.shape)
-    #
-    # def test_fit_predict_score(self):
-    #     self.clf.fit_predict_score(self.X_test, self.y_test)
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='roc_auc_score')
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='prc_n_score')
-    #     with assert_raises(NotImplementedError):
-    #         self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                    scoring='something')
-    #
-    # def test_predict_rank(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
-    #     assert_array_less(-0.1, pred_ranks)
-    #
-    # def test_predict_rank_normalized(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, 1.01)
-    #     assert_array_less(-0.1, pred_ranks)
-
-    # def test_plot(self):
-    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
-    #     assert_array_less(0, os)
-
-    # def test_model_clone(self):
-    #     clone_clf = clone(self.clf)
-
-    def tearDown(self):
-        pass
-
-
-if __name__ == '__main__':
+# -*- coding: utf-8 -*-
+from __future__ import division
+from __future__ import print_function
+
+import os
+import sys
+import unittest
+
+# noinspection PyProtectedMember
+from numpy.testing import assert_allclose
+from numpy.testing import assert_array_less
+from numpy.testing import assert_equal
+from numpy.testing import assert_raises
+from scipy.stats import rankdata
+from sklearn.base import clone
+from sklearn.metrics import roc_auc_score
+import torch
+
+# temporary solution for relative imports in case pyod is not installed
+# if deepod is installed, no need to use the following line
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
+from deepod.models.icl import ICL
+from deepod.utils.data import generate_data
+
+
+class TestICL(unittest.TestCase):
+    def setUp(self):
+        self.n_train = 200
+        self.n_test = 100
+        self.contamination = 0.1
+        self.roc_floor = 0.8
+        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
+            n_train=self.n_train, n_test=self.n_test, n_features=10,
+            contamination=self.contamination, random_state=42)
+
+        device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        self.clf = ICL(device=device, n_ensemble='auto')
+        self.clf.fit(self.X_train)
+
+    def test_parameters(self):
+        assert (hasattr(self.clf, 'decision_scores_') and
+                self.clf.decision_scores_ is not None)
+        assert (hasattr(self.clf, 'labels_') and
+                self.clf.labels_ is not None)
+        assert (hasattr(self.clf, 'threshold_') and
+                self.clf.threshold_ is not None)
+
+    # def test_train_scores(self):
+    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
+
+    def test_prediction_scores(self):
+        pred_scores = self.clf.decision_function(self.X_test)
+
+        # check score shapes
+        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
+
+        # check performance
+        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
+
+    def test_prediction_labels(self):
+        pred_labels = self.clf.predict(self.X_test)
+        assert_equal(pred_labels.shape, self.y_test.shape)
+
+    # def test_prediction_proba(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_linear(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_unify(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_parameter(self):
+    #     with assert_raises(ValueError):
+    #         self.clf.predict_proba(self.X_test, method='something')
+
+    def test_prediction_labels_confidence(self):
+        pred_labels, confidence = self.clf.predict(self.X_test,
+                                                   return_confidence=True)
+
+        assert_equal(pred_labels.shape, self.y_test.shape)
+        assert_equal(confidence.shape, self.y_test.shape)
+        assert (confidence.min() >= 0)
+        assert (confidence.max() <= 1)
+
+    # def test_prediction_proba_linear_confidence(self):
+    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
+    #                                                     method='linear',
+    #                                                     return_confidence=True)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    #     assert_equal(confidence.shape, self.y_test.shape)
+    #     assert (confidence.min() >= 0)
+    #     assert (confidence.max() <= 1)
+    #
+    # def test_fit_predict(self):
+    #     pred_labels = self.clf.fit_predict(self.X_train)
+    #     assert_equal(pred_labels.shape, self.y_train.shape)
+    #
+    # def test_fit_predict_score(self):
+    #     self.clf.fit_predict_score(self.X_test, self.y_test)
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='roc_auc_score')
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='prc_n_score')
+    #     with assert_raises(NotImplementedError):
+    #         self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                    scoring='something')
+    #
+    # def test_predict_rank(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
+    #     assert_array_less(-0.1, pred_ranks)
+    #
+    # def test_predict_rank_normalized(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, 1.01)
+    #     assert_array_less(-0.1, pred_ranks)
+
+    # def test_plot(self):
+    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
+    #     assert_array_less(0, os)
+
+    # def test_model_clone(self):
+    #     clone_clf = clone(self.clf)
+
+    def tearDown(self):
+        pass
+
+
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `deepod-0.2.0/deepod/test/test_dsad.py` & `deepod-0.3.0/deepod/test/test_slad.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,162 +1,148 @@
-# -*- coding: utf-8 -*-
-from __future__ import division
-from __future__ import print_function
-
-import os
-import sys
-import unittest
-
-# noinspection PyProtectedMember
-from numpy.testing import assert_allclose
-from numpy.testing import assert_array_less
-from numpy.testing import assert_equal
-from numpy.testing import assert_raises
-from scipy.stats import rankdata
-from sklearn.base import clone
-from sklearn.metrics import roc_auc_score
-import torch
-
-# temporary solution for relative imports in case pyod is not installed
-# if deepod is installed, no need to use the following line
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-
-from deepod.models.dsad import DeepSAD
-from deepod.utils.data import generate_data
-import numpy as np
-
-
-class TestDSAD(unittest.TestCase):
-    def setUp(self):
-        self.n_train = 200
-        self.n_test = 100
-        self.contamination = 0.1
-        self.roc_floor = 0.8
-
-        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
-            n_train=self.n_train, n_test=self.n_test, n_features=10,
-            contamination=self.contamination, random_state=42)
-
-        # file = '../../data/38_thyroid.npz'
-        # data = np.load(file, allow_pickle=True)
-        # x, y = data['X'], data['y']
-        # y = np.array(y, dtype=int)
-
-        anom_id = np.where(self.y_train == 1)[0]
-        known_anom_id = np.random.choice(anom_id, 10, replace=False)
-        y_semi = np.zeros_like(self.y_train, dtype=int)
-        y_semi[known_anom_id] = 1
-
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        self.clf = DeepSAD(epochs=1, hidden_dims=20,
-                           device=device,
-                          random_state=42)
-        self.clf.fit(self.X_train, y_semi)
-
-    def test_parameters(self):
-        assert (hasattr(self.clf, 'decision_scores_') and
-                self.clf.decision_scores_ is not None)
-        assert (hasattr(self.clf, 'labels_') and
-                self.clf.labels_ is not None)
-        assert (hasattr(self.clf, 'threshold_') and
-                self.clf.threshold_ is not None)
-
-    # def test_train_scores(self):
-    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
-
-    def test_prediction_scores(self):
-        pred_scores = self.clf.decision_function(self.X_test)
-
-        # check score shapes
-        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
-
-        # check performance
-        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
-
-    def test_prediction_labels(self):
-        pred_labels = self.clf.predict(self.X_test)
-        assert_equal(pred_labels.shape, self.y_test.shape)
-
-    # def test_prediction_proba(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_linear(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_unify(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_parameter(self):
-    #     with assert_raises(ValueError):
-    #         self.clf.predict_proba(self.X_test, method='something')
-
-    def test_prediction_labels_confidence(self):
-        pred_labels, confidence = self.clf.predict(self.X_test,
-                                                   return_confidence=True)
-
-        assert_equal(pred_labels.shape, self.y_test.shape)
-        assert_equal(confidence.shape, self.y_test.shape)
-        assert (confidence.min() >= 0)
-        assert (confidence.max() <= 1)
-
-    # def test_prediction_proba_linear_confidence(self):
-    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
-    #                                                     method='linear',
-    #                                                     return_confidence=True)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    #     assert_equal(confidence.shape, self.y_test.shape)
-    #     assert (confidence.min() >= 0)
-    #     assert (confidence.max() <= 1)
-    #
-    # def test_fit_predict(self):
-    #     pred_labels = self.clf.fit_predict(self.X_train)
-    #     assert_equal(pred_labels.shape, self.y_train.shape)
-    #
-    # def test_fit_predict_score(self):
-    #     self.clf.fit_predict_score(self.X_test, self.y_test)
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='roc_auc_score')
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='prc_n_score')
-    #     with assert_raises(NotImplementedError):
-    #         self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                    scoring='something')
-    #
-    # def test_predict_rank(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
-    #     assert_array_less(-0.1, pred_ranks)
-    #
-    # def test_predict_rank_normalized(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, 1.01)
-    #     assert_array_less(-0.1, pred_ranks)
-
-    # def test_plot(self):
-    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
-    #     assert_array_less(0, os)
-
-    # def test_model_clone(self):
-    #     clone_clf = clone(self.clf)
-
-    def tearDown(self):
-        pass
-
-
-if __name__ == '__main__':
+# -*- coding: utf-8 -*-
+from __future__ import division
+from __future__ import print_function
+
+import os
+import sys
+import unittest
+
+# noinspection PyProtectedMember
+from numpy.testing import assert_allclose
+from numpy.testing import assert_array_less
+from numpy.testing import assert_equal
+from numpy.testing import assert_raises
+from scipy.stats import rankdata
+from sklearn.base import clone
+from sklearn.metrics import roc_auc_score
+import torch
+
+# temporary solution for relative imports in case pyod is not installed
+# if deepod is installed, no need to use the following line
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
+from deepod.models.slad import SLAD
+from deepod.utils.data import generate_data
+
+
+class TestSLAD(unittest.TestCase):
+    def setUp(self):
+        self.n_train = 200
+        self.n_test = 100
+        self.contamination = 0.1
+        self.roc_floor = 0.8
+        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
+            n_train=self.n_train, n_test=self.n_test, n_features=10,
+            contamination=self.contamination, random_state=42)
+
+        device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        self.clf = SLAD(epochs=20, device=device)
+        self.clf.fit(self.X_train)
+
+    def test_parameters(self):
+        assert (hasattr(self.clf, 'decision_scores_') and
+                self.clf.decision_scores_ is not None)
+        assert (hasattr(self.clf, 'labels_') and
+                self.clf.labels_ is not None)
+        assert (hasattr(self.clf, 'threshold_') and
+                self.clf.threshold_ is not None)
+
+    # def test_train_scores(self):
+    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
+
+    def test_prediction_scores(self):
+        pred_scores = self.clf.decision_function(self.X_test)
+
+        # check score shapes
+        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
+
+        # check performance
+        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
+
+    def test_prediction_labels(self):
+        pred_labels = self.clf.predict(self.X_test)
+        assert_equal(pred_labels.shape, self.y_test.shape)
+
+    # def test_prediction_proba(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_linear(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_unify(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_parameter(self):
+    #     with assert_raises(ValueError):
+    #         self.clf.predict_proba(self.X_test, method='something')
+
+    def test_prediction_labels_confidence(self):
+        pred_labels, confidence = self.clf.predict(self.X_test,
+                                                   return_confidence=True)
+
+        assert_equal(pred_labels.shape, self.y_test.shape)
+        assert_equal(confidence.shape, self.y_test.shape)
+        assert (confidence.min() >= 0)
+        assert (confidence.max() <= 1)
+
+    # def test_prediction_proba_linear_confidence(self):
+    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
+    #                                                     method='linear',
+    #                                                     return_confidence=True)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    #     assert_equal(confidence.shape, self.y_test.shape)
+    #     assert (confidence.min() >= 0)
+    #     assert (confidence.max() <= 1)
+    #
+    # def test_fit_predict(self):
+    #     pred_labels = self.clf.fit_predict(self.X_train)
+    #     assert_equal(pred_labels.shape, self.y_train.shape)
+    #
+    # def test_fit_predict_score(self):
+    #     self.clf.fit_predict_score(self.X_test, self.y_test)
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='roc_auc_score')
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='prc_n_score')
+    #     with assert_raises(NotImplementedError):
+    #         self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                    scoring='something')
+    #
+    # def test_predict_rank(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
+    #     assert_array_less(-0.1, pred_ranks)
+    #
+    # def test_predict_rank_normalized(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, 1.01)
+    #     assert_array_less(-0.1, pred_ranks)
+
+    # def test_plot(self):
+    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
+    #     assert_array_less(0, os)
+
+    # def test_model_clone(self):
+    #     clone_clf = clone(self.clf)
+
+    def tearDown(self):
+        pass
+
+
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `deepod-0.2.0/deepod/test/test_dsvdd.py` & `deepod-0.3.0/deepod/test/test_rca.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-# -*- coding: utf-8 -*-
-from __future__ import division
-from __future__ import print_function
-
-import os
-import sys
-import unittest
-
-# noinspection PyProtectedMember
-from numpy.testing import assert_allclose
-from numpy.testing import assert_array_less
-from numpy.testing import assert_equal
-from numpy.testing import assert_raises
-from scipy.stats import rankdata
-from sklearn.base import clone
-from sklearn.metrics import roc_auc_score
-import torch
-
-# temporary solution for relative imports in case pyod is not installed
-# if deepod is installed, no need to use the following line
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-
-from deepod.models.dsvdd import DeepSVDD
-from deepod.utils.data import generate_data
-
-
-class TestDeepSVDD(unittest.TestCase):
-    def setUp(self):
-        self.n_train = 200
-        self.n_test = 100
-        self.contamination = 0.1
-        self.roc_floor = 0.8
-        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
-            n_train=self.n_train, n_test=self.n_test, n_features=10,
-            contamination=self.contamination, random_state=42)
-
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        self.clf = DeepSVDD(device=device)
-        self.clf.fit(self.X_train)
-
-    def test_parameters(self):
-        assert (hasattr(self.clf, 'decision_scores_') and
-                self.clf.decision_scores_ is not None)
-        assert (hasattr(self.clf, 'labels_') and
-                self.clf.labels_ is not None)
-        assert (hasattr(self.clf, 'threshold_') and
-                self.clf.threshold_ is not None)
-
-    # def test_train_scores(self):
-    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
-
-    def test_prediction_scores(self):
-        pred_scores = self.clf.decision_function(self.X_test)
-
-        # check score shapes
-        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
-
-        # check performance
-        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
-
-    def test_prediction_labels(self):
-        pred_labels = self.clf.predict(self.X_test)
-        assert_equal(pred_labels.shape, self.y_test.shape)
-
-    # def test_prediction_proba(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_linear(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_unify(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_parameter(self):
-    #     with assert_raises(ValueError):
-    #         self.clf.predict_proba(self.X_test, method='something')
-
-    def test_prediction_labels_confidence(self):
-        pred_labels, confidence = self.clf.predict(self.X_test,
-                                                   return_confidence=True)
-
-        assert_equal(pred_labels.shape, self.y_test.shape)
-        assert_equal(confidence.shape, self.y_test.shape)
-        assert (confidence.min() >= 0)
-        assert (confidence.max() <= 1)
-
-    # def test_prediction_proba_linear_confidence(self):
-    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
-    #                                                     method='linear',
-    #                                                     return_confidence=True)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    #     assert_equal(confidence.shape, self.y_test.shape)
-    #     assert (confidence.min() >= 0)
-    #     assert (confidence.max() <= 1)
-    #
-    # def test_fit_predict(self):
-    #     pred_labels = self.clf.fit_predict(self.X_train)
-    #     assert_equal(pred_labels.shape, self.y_train.shape)
-    #
-    # def test_fit_predict_score(self):
-    #     self.clf.fit_predict_score(self.X_test, self.y_test)
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='roc_auc_score')
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='prc_n_score')
-    #     with assert_raises(NotImplementedError):
-    #         self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                    scoring='something')
-    #
-    # def test_predict_rank(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
-    #     assert_array_less(-0.1, pred_ranks)
-    #
-    # def test_predict_rank_normalized(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, 1.01)
-    #     assert_array_less(-0.1, pred_ranks)
-
-    # def test_plot(self):
-    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
-    #     assert_array_less(0, os)
-
-    # def test_model_clone(self):
-    #     clone_clf = clone(self.clf)
-
-    def tearDown(self):
-        pass
-
-
-if __name__ == '__main__':
+# -*- coding: utf-8 -*-
+from __future__ import division
+from __future__ import print_function
+
+import os
+import sys
+import unittest
+
+# noinspection PyProtectedMember
+from numpy.testing import assert_allclose
+from numpy.testing import assert_array_less
+from numpy.testing import assert_equal
+from numpy.testing import assert_raises
+from scipy.stats import rankdata
+from sklearn.base import clone
+from sklearn.metrics import roc_auc_score
+import torch
+
+# temporary solution for relative imports in case pyod is not installed
+# if deepod is installed, no need to use the following line
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
+from deepod.models.rca import RCA
+from deepod.utils.data import generate_data
+
+
+class TestRCA(unittest.TestCase):
+    def setUp(self):
+        self.n_train = 200
+        self.n_test = 100
+        self.contamination = 0.1
+        self.roc_floor = 0.8
+        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
+            n_train=self.n_train, n_test=self.n_test, n_features=10,
+            contamination=self.contamination, random_state=42)
+
+        device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        self.clf = RCA(device=device, act='LeakyReLU')
+        self.clf.fit(self.X_train)
+
+    def test_parameters(self):
+        assert (hasattr(self.clf, 'decision_scores_') and
+                self.clf.decision_scores_ is not None)
+        assert (hasattr(self.clf, 'labels_') and
+                self.clf.labels_ is not None)
+        assert (hasattr(self.clf, 'threshold_') and
+                self.clf.threshold_ is not None)
+
+    # def test_train_scores(self):
+    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
+
+    def test_prediction_scores(self):
+        pred_scores = self.clf.decision_function(self.X_test)
+
+        # check score shapes
+        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
+
+        # check performance
+        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
+
+    def test_prediction_labels(self):
+        pred_labels = self.clf.predict(self.X_test)
+        assert_equal(pred_labels.shape, self.y_test.shape)
+
+    # def test_prediction_proba(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_linear(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_unify(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_parameter(self):
+    #     with assert_raises(ValueError):
+    #         self.clf.predict_proba(self.X_test, method='something')
+
+    def test_prediction_labels_confidence(self):
+        pred_labels, confidence = self.clf.predict(self.X_test,
+                                                   return_confidence=True)
+
+        assert_equal(pred_labels.shape, self.y_test.shape)
+        assert_equal(confidence.shape, self.y_test.shape)
+        assert (confidence.min() >= 0)
+        assert (confidence.max() <= 1)
+
+    # def test_prediction_proba_linear_confidence(self):
+    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
+    #                                                     method='linear',
+    #                                                     return_confidence=True)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    #     assert_equal(confidence.shape, self.y_test.shape)
+    #     assert (confidence.min() >= 0)
+    #     assert (confidence.max() <= 1)
+    #
+    # def test_fit_predict(self):
+    #     pred_labels = self.clf.fit_predict(self.X_train)
+    #     assert_equal(pred_labels.shape, self.y_train.shape)
+    #
+    # def test_fit_predict_score(self):
+    #     self.clf.fit_predict_score(self.X_test, self.y_test)
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='roc_auc_score')
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='prc_n_score')
+    #     with assert_raises(NotImplementedError):
+    #         self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                    scoring='something')
+    #
+    # def test_predict_rank(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
+    #     assert_array_less(-0.1, pred_ranks)
+    #
+    # def test_predict_rank_normalized(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, 1.01)
+    #     assert_array_less(-0.1, pred_ranks)
+
+    # def test_plot(self):
+    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
+    #     assert_array_less(0, os)
+
+    # def test_model_clone(self):
+    #     clone_clf = clone(self.clf)
+
+    def tearDown(self):
+        pass
+
+
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `deepod-0.2.0/deepod/test/test_goad.py` & `deepod-0.3.0/deepod/test/test_neutral.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-# -*- coding: utf-8 -*-
-from __future__ import division
-from __future__ import print_function
-
-import os
-import sys
-import unittest
-
-# noinspection PyProtectedMember
-from numpy.testing import assert_allclose
-from numpy.testing import assert_array_less
-from numpy.testing import assert_equal
-from numpy.testing import assert_raises
-from scipy.stats import rankdata
-from sklearn.base import clone
-from sklearn.metrics import roc_auc_score
-import torch
-
-# temporary solution for relative imports in case pyod is not installed
-# if deepod is installed, no need to use the following line
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-
-from deepod.models import GOAD
-from deepod.utils.data import generate_data
-
-
-class TestGOAD(unittest.TestCase):
-    def setUp(self):
-        self.n_train = 200
-        self.n_test = 100
-        self.contamination = 0.1
-        self.roc_floor = 0.8
-        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
-            n_train=self.n_train, n_test=self.n_test, n_features=10,
-            contamination=self.contamination, random_state=42)
-
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        self.clf = GOAD(device=device)
-        self.clf.fit(self.X_train)
-
-    def test_parameters(self):
-        assert (hasattr(self.clf, 'decision_scores_') and
-                self.clf.decision_scores_ is not None)
-        assert (hasattr(self.clf, 'labels_') and
-                self.clf.labels_ is not None)
-        assert (hasattr(self.clf, 'threshold_') and
-                self.clf.threshold_ is not None)
-
-    # def test_train_scores(self):
-    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
-
-    def test_prediction_scores(self):
-        pred_scores = self.clf.decision_function(self.X_test)
-
-        # check score shapes
-        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
-
-        # check performance
-        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
-
-    def test_prediction_labels(self):
-        pred_labels = self.clf.predict(self.X_test)
-        assert_equal(pred_labels.shape, self.y_test.shape)
-
-    # def test_prediction_proba(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_linear(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_unify(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_parameter(self):
-    #     with assert_raises(ValueError):
-    #         self.clf.predict_proba(self.X_test, method='something')
-
-    def test_prediction_labels_confidence(self):
-        pred_labels, confidence = self.clf.predict(self.X_test,
-                                                   return_confidence=True)
-
-        assert_equal(pred_labels.shape, self.y_test.shape)
-        assert_equal(confidence.shape, self.y_test.shape)
-        assert (confidence.min() >= 0)
-        assert (confidence.max() <= 1)
-
-    # def test_prediction_proba_linear_confidence(self):
-    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
-    #                                                     method='linear',
-    #                                                     return_confidence=True)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    #     assert_equal(confidence.shape, self.y_test.shape)
-    #     assert (confidence.min() >= 0)
-    #     assert (confidence.max() <= 1)
-    #
-    # def test_fit_predict(self):
-    #     pred_labels = self.clf.fit_predict(self.X_train)
-    #     assert_equal(pred_labels.shape, self.y_train.shape)
-    #
-    # def test_fit_predict_score(self):
-    #     self.clf.fit_predict_score(self.X_test, self.y_test)
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='roc_auc_score')
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='prc_n_score')
-    #     with assert_raises(NotImplementedError):
-    #         self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                    scoring='something')
-    #
-    # def test_predict_rank(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
-    #     assert_array_less(-0.1, pred_ranks)
-    #
-    # def test_predict_rank_normalized(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, 1.01)
-    #     assert_array_less(-0.1, pred_ranks)
-
-    # def test_plot(self):
-    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
-    #     assert_array_less(0, os)
-
-    # def test_model_clone(self):
-    #     clone_clf = clone(self.clf)
-
-    def tearDown(self):
-        pass
-
-
-if __name__ == '__main__':
+# -*- coding: utf-8 -*-
+from __future__ import division
+from __future__ import print_function
+
+import os
+import sys
+import unittest
+
+# noinspection PyProtectedMember
+from numpy.testing import assert_allclose
+from numpy.testing import assert_array_less
+from numpy.testing import assert_equal
+from numpy.testing import assert_raises
+from scipy.stats import rankdata
+from sklearn.base import clone
+from sklearn.metrics import roc_auc_score
+import torch
+
+# temporary solution for relative imports in case pyod is not installed
+# if deepod is installed, no need to use the following line
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
+from deepod.models import NeuTraL
+from deepod.utils.data import generate_data
+
+
+class TestNeuTral(unittest.TestCase):
+    def setUp(self):
+        self.n_train = 200
+        self.n_test = 100
+        self.contamination = 0.1
+        self.roc_floor = 0.8
+        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
+            n_train=self.n_train, n_test=self.n_test, n_features=10,
+            contamination=self.contamination, random_state=42)
+
+        device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        self.clf = NeuTraL(device=device)
+        self.clf.fit(self.X_train)
+
+    def test_parameters(self):
+        assert (hasattr(self.clf, 'decision_scores_') and
+                self.clf.decision_scores_ is not None)
+        assert (hasattr(self.clf, 'labels_') and
+                self.clf.labels_ is not None)
+        assert (hasattr(self.clf, 'threshold_') and
+                self.clf.threshold_ is not None)
+
+    # def test_train_scores(self):
+    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
+
+    def test_prediction_scores(self):
+        pred_scores = self.clf.decision_function(self.X_test)
+
+        # check score shapes
+        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
+
+        # check performance
+        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
+
+    def test_prediction_labels(self):
+        pred_labels = self.clf.predict(self.X_test)
+        assert_equal(pred_labels.shape, self.y_test.shape)
+
+    # def test_prediction_proba(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_linear(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_unify(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_parameter(self):
+    #     with assert_raises(ValueError):
+    #         self.clf.predict_proba(self.X_test, method='something')
+
+    def test_prediction_labels_confidence(self):
+        pred_labels, confidence = self.clf.predict(self.X_test,
+                                                   return_confidence=True)
+
+        assert_equal(pred_labels.shape, self.y_test.shape)
+        assert_equal(confidence.shape, self.y_test.shape)
+        assert (confidence.min() >= 0)
+        assert (confidence.max() <= 1)
+
+    # def test_prediction_proba_linear_confidence(self):
+    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
+    #                                                     method='linear',
+    #                                                     return_confidence=True)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    #     assert_equal(confidence.shape, self.y_test.shape)
+    #     assert (confidence.min() >= 0)
+    #     assert (confidence.max() <= 1)
+    #
+    # def test_fit_predict(self):
+    #     pred_labels = self.clf.fit_predict(self.X_train)
+    #     assert_equal(pred_labels.shape, self.y_train.shape)
+    #
+    # def test_fit_predict_score(self):
+    #     self.clf.fit_predict_score(self.X_test, self.y_test)
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='roc_auc_score')
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='prc_n_score')
+    #     with assert_raises(NotImplementedError):
+    #         self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                    scoring='something')
+    #
+    # def test_predict_rank(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
+    #     assert_array_less(-0.1, pred_ranks)
+    #
+    # def test_predict_rank_normalized(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, 1.01)
+    #     assert_array_less(-0.1, pred_ranks)
+
+    # def test_plot(self):
+    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
+    #     assert_array_less(0, os)
+
+    # def test_model_clone(self):
+    #     clone_clf = clone(self.clf)
+
+    def tearDown(self):
+        pass
+
+
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `deepod-0.2.0/deepod/test/test_icl.py` & `deepod-0.3.0/deepod/test/test_rdp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-# -*- coding: utf-8 -*-
-from __future__ import division
-from __future__ import print_function
-
-import os
-import sys
-import unittest
-
-# noinspection PyProtectedMember
-from numpy.testing import assert_allclose
-from numpy.testing import assert_array_less
-from numpy.testing import assert_equal
-from numpy.testing import assert_raises
-from scipy.stats import rankdata
-from sklearn.base import clone
-from sklearn.metrics import roc_auc_score
-import torch
-
-# temporary solution for relative imports in case pyod is not installed
-# if deepod is installed, no need to use the following line
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-
-from deepod.models.icl import ICL
-from deepod.utils.data import generate_data
-
-
-class TestICL(unittest.TestCase):
-    def setUp(self):
-        self.n_train = 200
-        self.n_test = 100
-        self.contamination = 0.1
-        self.roc_floor = 0.8
-        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
-            n_train=self.n_train, n_test=self.n_test, n_features=10,
-            contamination=self.contamination, random_state=42)
-
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        self.clf = ICL(device=device, n_ensemble='auto')
-        self.clf.fit(self.X_train)
-
-    def test_parameters(self):
-        assert (hasattr(self.clf, 'decision_scores_') and
-                self.clf.decision_scores_ is not None)
-        assert (hasattr(self.clf, 'labels_') and
-                self.clf.labels_ is not None)
-        assert (hasattr(self.clf, 'threshold_') and
-                self.clf.threshold_ is not None)
-
-    # def test_train_scores(self):
-    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
-
-    def test_prediction_scores(self):
-        pred_scores = self.clf.decision_function(self.X_test)
-
-        # check score shapes
-        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
-
-        # check performance
-        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
-
-    def test_prediction_labels(self):
-        pred_labels = self.clf.predict(self.X_test)
-        assert_equal(pred_labels.shape, self.y_test.shape)
-
-    # def test_prediction_proba(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_linear(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_unify(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_parameter(self):
-    #     with assert_raises(ValueError):
-    #         self.clf.predict_proba(self.X_test, method='something')
-
-    def test_prediction_labels_confidence(self):
-        pred_labels, confidence = self.clf.predict(self.X_test,
-                                                   return_confidence=True)
-
-        assert_equal(pred_labels.shape, self.y_test.shape)
-        assert_equal(confidence.shape, self.y_test.shape)
-        assert (confidence.min() >= 0)
-        assert (confidence.max() <= 1)
-
-    # def test_prediction_proba_linear_confidence(self):
-    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
-    #                                                     method='linear',
-    #                                                     return_confidence=True)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    #     assert_equal(confidence.shape, self.y_test.shape)
-    #     assert (confidence.min() >= 0)
-    #     assert (confidence.max() <= 1)
-    #
-    # def test_fit_predict(self):
-    #     pred_labels = self.clf.fit_predict(self.X_train)
-    #     assert_equal(pred_labels.shape, self.y_train.shape)
-    #
-    # def test_fit_predict_score(self):
-    #     self.clf.fit_predict_score(self.X_test, self.y_test)
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='roc_auc_score')
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='prc_n_score')
-    #     with assert_raises(NotImplementedError):
-    #         self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                    scoring='something')
-    #
-    # def test_predict_rank(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
-    #     assert_array_less(-0.1, pred_ranks)
-    #
-    # def test_predict_rank_normalized(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, 1.01)
-    #     assert_array_less(-0.1, pred_ranks)
-
-    # def test_plot(self):
-    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
-    #     assert_array_less(0, os)
-
-    # def test_model_clone(self):
-    #     clone_clf = clone(self.clf)
-
-    def tearDown(self):
-        pass
-
-
-if __name__ == '__main__':
+# -*- coding: utf-8 -*-
+from __future__ import division
+from __future__ import print_function
+
+import os
+import sys
+import unittest
+
+# noinspection PyProtectedMember
+from numpy.testing import assert_allclose
+from numpy.testing import assert_array_less
+from numpy.testing import assert_equal
+from numpy.testing import assert_raises
+from scipy.stats import rankdata
+from sklearn.base import clone
+from sklearn.metrics import roc_auc_score
+import torch
+
+# temporary solution for relative imports in case pyod is not installed
+# if deepod is installed, no need to use the following line
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
+from deepod.models import RDP
+from deepod.utils.data import generate_data
+
+
+class TestRDP(unittest.TestCase):
+    def setUp(self):
+        self.n_train = 200
+        self.n_test = 100
+        self.contamination = 0.1
+        self.roc_floor = 0.8
+        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
+            n_train=self.n_train, n_test=self.n_test, n_features=10,
+            contamination=self.contamination, random_state=42)
+
+        device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        self.clf = RDP(hidden_dims=100, device=device)
+        self.clf.fit(self.X_train)
+
+    def test_parameters(self):
+        assert (hasattr(self.clf, 'decision_scores_') and
+                self.clf.decision_scores_ is not None)
+        assert (hasattr(self.clf, 'labels_') and
+                self.clf.labels_ is not None)
+        assert (hasattr(self.clf, 'threshold_') and
+                self.clf.threshold_ is not None)
+
+    # def test_train_scores(self):
+    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
+
+    def test_prediction_scores(self):
+        pred_scores = self.clf.decision_function(self.X_test)
+
+        # check score shapes
+        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
+
+        # check performance
+        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
+
+    def test_prediction_labels(self):
+        pred_labels = self.clf.predict(self.X_test)
+        assert_equal(pred_labels.shape, self.y_test.shape)
+
+    # def test_prediction_proba(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_linear(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_unify(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_parameter(self):
+    #     with assert_raises(ValueError):
+    #         self.clf.predict_proba(self.X_test, method='something')
+
+    def test_prediction_labels_confidence(self):
+        pred_labels, confidence = self.clf.predict(self.X_test,
+                                                   return_confidence=True)
+
+        assert_equal(pred_labels.shape, self.y_test.shape)
+        assert_equal(confidence.shape, self.y_test.shape)
+        assert (confidence.min() >= 0)
+        assert (confidence.max() <= 1)
+
+    # def test_prediction_proba_linear_confidence(self):
+    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
+    #                                                     method='linear',
+    #                                                     return_confidence=True)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    #     assert_equal(confidence.shape, self.y_test.shape)
+    #     assert (confidence.min() >= 0)
+    #     assert (confidence.max() <= 1)
+    #
+    # def test_fit_predict(self):
+    #     pred_labels = self.clf.fit_predict(self.X_train)
+    #     assert_equal(pred_labels.shape, self.y_train.shape)
+    #
+    # def test_fit_predict_score(self):
+    #     self.clf.fit_predict_score(self.X_test, self.y_test)
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='roc_auc_score')
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='prc_n_score')
+    #     with assert_raises(NotImplementedError):
+    #         self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                    scoring='something')
+    #
+    # def test_predict_rank(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
+    #     assert_array_less(-0.1, pred_ranks)
+    #
+    # def test_predict_rank_normalized(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, 1.01)
+    #     assert_array_less(-0.1, pred_ranks)
+
+    # def test_plot(self):
+    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
+    #     assert_array_less(0, os)
+
+    # def test_model_clone(self):
+    #     clone_clf = clone(self.clf)
+
+    def tearDown(self):
+        pass
+
+
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `deepod-0.2.0/deepod/test/test_neutral.py` & `deepod-0.3.0/deepod/test/test_goad.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-# -*- coding: utf-8 -*-
-from __future__ import division
-from __future__ import print_function
-
-import os
-import sys
-import unittest
-
-# noinspection PyProtectedMember
-from numpy.testing import assert_allclose
-from numpy.testing import assert_array_less
-from numpy.testing import assert_equal
-from numpy.testing import assert_raises
-from scipy.stats import rankdata
-from sklearn.base import clone
-from sklearn.metrics import roc_auc_score
-import torch
-
-# temporary solution for relative imports in case pyod is not installed
-# if deepod is installed, no need to use the following line
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-
-from deepod.models import NeuTraL
-from deepod.utils.data import generate_data
-
-
-class TestNeuTral(unittest.TestCase):
-    def setUp(self):
-        self.n_train = 200
-        self.n_test = 100
-        self.contamination = 0.1
-        self.roc_floor = 0.8
-        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
-            n_train=self.n_train, n_test=self.n_test, n_features=10,
-            contamination=self.contamination, random_state=42)
-
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        self.clf = NeuTraL(device=device)
-        self.clf.fit(self.X_train)
-
-    def test_parameters(self):
-        assert (hasattr(self.clf, 'decision_scores_') and
-                self.clf.decision_scores_ is not None)
-        assert (hasattr(self.clf, 'labels_') and
-                self.clf.labels_ is not None)
-        assert (hasattr(self.clf, 'threshold_') and
-                self.clf.threshold_ is not None)
-
-    # def test_train_scores(self):
-    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
-
-    def test_prediction_scores(self):
-        pred_scores = self.clf.decision_function(self.X_test)
-
-        # check score shapes
-        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
-
-        # check performance
-        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
-
-    def test_prediction_labels(self):
-        pred_labels = self.clf.predict(self.X_test)
-        assert_equal(pred_labels.shape, self.y_test.shape)
-
-    # def test_prediction_proba(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_linear(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_unify(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_parameter(self):
-    #     with assert_raises(ValueError):
-    #         self.clf.predict_proba(self.X_test, method='something')
-
-    def test_prediction_labels_confidence(self):
-        pred_labels, confidence = self.clf.predict(self.X_test,
-                                                   return_confidence=True)
-
-        assert_equal(pred_labels.shape, self.y_test.shape)
-        assert_equal(confidence.shape, self.y_test.shape)
-        assert (confidence.min() >= 0)
-        assert (confidence.max() <= 1)
-
-    # def test_prediction_proba_linear_confidence(self):
-    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
-    #                                                     method='linear',
-    #                                                     return_confidence=True)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    #     assert_equal(confidence.shape, self.y_test.shape)
-    #     assert (confidence.min() >= 0)
-    #     assert (confidence.max() <= 1)
-    #
-    # def test_fit_predict(self):
-    #     pred_labels = self.clf.fit_predict(self.X_train)
-    #     assert_equal(pred_labels.shape, self.y_train.shape)
-    #
-    # def test_fit_predict_score(self):
-    #     self.clf.fit_predict_score(self.X_test, self.y_test)
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='roc_auc_score')
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='prc_n_score')
-    #     with assert_raises(NotImplementedError):
-    #         self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                    scoring='something')
-    #
-    # def test_predict_rank(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
-    #     assert_array_less(-0.1, pred_ranks)
-    #
-    # def test_predict_rank_normalized(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, 1.01)
-    #     assert_array_less(-0.1, pred_ranks)
-
-    # def test_plot(self):
-    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
-    #     assert_array_less(0, os)
-
-    # def test_model_clone(self):
-    #     clone_clf = clone(self.clf)
-
-    def tearDown(self):
-        pass
-
-
-if __name__ == '__main__':
+# -*- coding: utf-8 -*-
+from __future__ import division
+from __future__ import print_function
+
+import os
+import sys
+import unittest
+
+# noinspection PyProtectedMember
+from numpy.testing import assert_allclose
+from numpy.testing import assert_array_less
+from numpy.testing import assert_equal
+from numpy.testing import assert_raises
+from scipy.stats import rankdata
+from sklearn.base import clone
+from sklearn.metrics import roc_auc_score
+import torch
+
+# temporary solution for relative imports in case pyod is not installed
+# if deepod is installed, no need to use the following line
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
+from deepod.models import GOAD
+from deepod.utils.data import generate_data
+
+
+class TestGOAD(unittest.TestCase):
+    def setUp(self):
+        self.n_train = 200
+        self.n_test = 100
+        self.contamination = 0.1
+        self.roc_floor = 0.8
+        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
+            n_train=self.n_train, n_test=self.n_test, n_features=10,
+            contamination=self.contamination, random_state=42)
+
+        device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        self.clf = GOAD(device=device, n_trans=64)
+        self.clf.fit(self.X_train)
+
+    def test_parameters(self):
+        assert (hasattr(self.clf, 'decision_scores_') and
+                self.clf.decision_scores_ is not None)
+        assert (hasattr(self.clf, 'labels_') and
+                self.clf.labels_ is not None)
+        assert (hasattr(self.clf, 'threshold_') and
+                self.clf.threshold_ is not None)
+
+    # def test_train_scores(self):
+    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
+
+    def test_prediction_scores(self):
+        pred_scores = self.clf.decision_function(self.X_test)
+
+        # check score shapes
+        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
+
+        # check performance
+        assert (roc_auc_score(self.y_test, pred_scores) >= self.roc_floor)
+
+    def test_prediction_labels(self):
+        pred_labels = self.clf.predict(self.X_test)
+        assert_equal(pred_labels.shape, self.y_test.shape)
+
+    # def test_prediction_proba(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_linear(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_unify(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_parameter(self):
+    #     with assert_raises(ValueError):
+    #         self.clf.predict_proba(self.X_test, method='something')
+
+    def test_prediction_labels_confidence(self):
+        pred_labels, confidence = self.clf.predict(self.X_test,
+                                                   return_confidence=True)
+
+        assert_equal(pred_labels.shape, self.y_test.shape)
+        assert_equal(confidence.shape, self.y_test.shape)
+        assert (confidence.min() >= 0)
+        assert (confidence.max() <= 1)
+
+    # def test_prediction_proba_linear_confidence(self):
+    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
+    #                                                     method='linear',
+    #                                                     return_confidence=True)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    #     assert_equal(confidence.shape, self.y_test.shape)
+    #     assert (confidence.min() >= 0)
+    #     assert (confidence.max() <= 1)
+    #
+    # def test_fit_predict(self):
+    #     pred_labels = self.clf.fit_predict(self.X_train)
+    #     assert_equal(pred_labels.shape, self.y_train.shape)
+    #
+    # def test_fit_predict_score(self):
+    #     self.clf.fit_predict_score(self.X_test, self.y_test)
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='roc_auc_score')
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='prc_n_score')
+    #     with assert_raises(NotImplementedError):
+    #         self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                    scoring='something')
+    #
+    # def test_predict_rank(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
+    #     assert_array_less(-0.1, pred_ranks)
+    #
+    # def test_predict_rank_normalized(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, 1.01)
+    #     assert_array_less(-0.1, pred_ranks)
+
+    # def test_plot(self):
+    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
+    #     assert_array_less(0, os)
+
+    # def test_model_clone(self):
+    #     clone_clf = clone(self.clf)
+
+    def tearDown(self):
+        pass
+
+
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `deepod-0.2.0/deepod/test/test_prenet.py` & `deepod-0.3.0/deepod/test/test_feawad.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,165 +1,187 @@
-# -*- coding: utf-8 -*-
-from __future__ import division
-from __future__ import print_function
-
-import os
-import sys
-import unittest
-
-# noinspection PyProtectedMember
-from numpy.testing import assert_allclose
-from numpy.testing import assert_array_less
-from numpy.testing import assert_equal
-from numpy.testing import assert_raises
-from scipy.stats import rankdata
-from sklearn.base import clone
-from sklearn.metrics import roc_auc_score
-import torch
-
-# temporary solution for relative imports in case pyod is not installed
-# if deepod is installed, no need to use the following line
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-
-from deepod.models.prenet import PReNet
-from deepod.utils.data import generate_data
-import numpy as np
-
-
-class TestPReNet(unittest.TestCase):
-    def setUp(self):
-        self.n_train = 200
-        self.n_test = 100
-        self.contamination = 0.1
-        self.roc_floor = 0.8
-
-        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
-            n_train=self.n_train, n_test=self.n_test, n_features=10,
-            contamination=self.contamination, random_state=42)
-
-        # file = '../../data/38_thyroid.npz'
-        # data = np.load(file, allow_pickle=True)
-        # x, y = data['X'], data['y']
-        # y = np.array(y, dtype=int)
-
-        anom_id = np.where(self.y_train == 1)[0]
-        known_anom_id = np.random.choice(anom_id, 10, replace=False)
-        y_semi = np.zeros_like(self.y_train, dtype=int)
-        y_semi[known_anom_id] = 1
-
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        self.clf = PReNet(epochs=50,
-                          epoch_steps=20,
-                          device=device,
-                          batch_size=256,
-                          lr=1e-5)
-        self.clf.fit(self.X_train, y_semi)
-
-    def test_parameters(self):
-        assert (hasattr(self.clf, 'decision_scores_') and
-                self.clf.decision_scores_ is not None)
-        assert (hasattr(self.clf, 'labels_') and
-                self.clf.labels_ is not None)
-        assert (hasattr(self.clf, 'threshold_') and
-                self.clf.threshold_ is not None)
-
-    # def test_train_scores(self):
-    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
-
-    def test_prediction_scores(self):
-        pred_scores = self.clf.decision_function(self.X_test)
-
-        # check score shapes
-        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
-
-        # # check performance
-        # auc = roc_auc_score(self.y_test, pred_scores)
-        # assert (auc >= self.roc_floor), f'auc is {auc}'
-
-    def test_prediction_labels(self):
-        pred_labels = self.clf.predict(self.X_test)
-        assert_equal(pred_labels.shape, self.y_test.shape)
-
-    # def test_prediction_proba(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_linear(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_unify(self):
-    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    # def test_prediction_proba_parameter(self):
-    #     with assert_raises(ValueError):
-    #         self.clf.predict_proba(self.X_test, method='something')
-
-    def test_prediction_labels_confidence(self):
-        pred_labels, confidence = self.clf.predict(self.X_test,
-                                                   return_confidence=True)
-
-        assert_equal(pred_labels.shape, self.y_test.shape)
-        assert_equal(confidence.shape, self.y_test.shape)
-        assert (confidence.min() >= 0)
-        assert (confidence.max() <= 1)
-
-    # def test_prediction_proba_linear_confidence(self):
-    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
-    #                                                     method='linear',
-    #                                                     return_confidence=True)
-    #     assert (pred_proba.min() >= 0)
-    #     assert (pred_proba.max() <= 1)
-    #
-    #     assert_equal(confidence.shape, self.y_test.shape)
-    #     assert (confidence.min() >= 0)
-    #     assert (confidence.max() <= 1)
-    #
-    # def test_fit_predict(self):
-    #     pred_labels = self.clf.fit_predict(self.X_train)
-    #     assert_equal(pred_labels.shape, self.y_train.shape)
-    #
-    # def test_fit_predict_score(self):
-    #     self.clf.fit_predict_score(self.X_test, self.y_test)
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='roc_auc_score')
-    #     self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                scoring='prc_n_score')
-    #     with assert_raises(NotImplementedError):
-    #         self.clf.fit_predict_score(self.X_test, self.y_test,
-    #                                    scoring='something')
-    #
-    # def test_predict_rank(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
-    #     assert_array_less(-0.1, pred_ranks)
-    #
-    # def test_predict_rank_normalized(self):
-    #     pred_socres = self.clf.decision_function(self.X_test)
-    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
-    #
-    #     # assert the order is reserved
-    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
-    #     assert_array_less(pred_ranks, 1.01)
-    #     assert_array_less(-0.1, pred_ranks)
-
-    # def test_plot(self):
-    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
-    #     assert_array_less(0, os)
-
-    # def test_model_clone(self):
-    #     clone_clf = clone(self.clf)
-
-    def tearDown(self):
-        pass
-
-
-if __name__ == '__main__':
+# -*- coding: utf-8 -*-
+from __future__ import division
+from __future__ import print_function
+
+import os
+import sys
+import unittest
+
+# noinspection PyProtectedMember
+from numpy.testing import assert_allclose
+from numpy.testing import assert_array_less
+from numpy.testing import assert_equal
+from numpy.testing import assert_raises
+from scipy.stats import rankdata
+from sklearn.base import clone
+from sklearn.metrics import roc_auc_score
+import torch
+
+# temporary solution for relative imports in case pyod is not installed
+# if deepod is installed, no need to use the following line
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
+from deepod.models.feawad import FeaWAD
+from deepod.utils.data import generate_data
+import numpy as np
+
+
+class TestFeaWAD(unittest.TestCase):
+    def setUp(self):
+        self.n_train = 200
+        self.n_test = 100
+        self.contamination = 0.1
+        self.roc_floor = 0.8
+
+        self.X_train, self.X_test, self.y_train, self.y_test = generate_data(
+            n_train=self.n_train, n_test=self.n_test, n_features=10,
+            contamination=self.contamination, random_state=42)
+
+        self.Xts_train = np.random.randn(1000, 19)
+        self.yts_train = np.zeros(1000, dtype=int)
+        self.yts_train[200:250] = 1
+        self.Xts_test = self.Xts_train.copy()
+        self.yts_test = self.yts_train.copy()
+
+
+        # file = '../../data/38_thyroid.npz'
+        # data = np.load(file, allow_pickle=True)
+        # x, y = data['X'], data['y']
+        # y = np.array(y, dtype=int)
+
+        anom_id = np.where(self.y_train == 1)[0]
+        known_anom_id = np.random.choice(anom_id, 10, replace=False)
+        y_semi = np.zeros_like(self.y_train, dtype=int)
+        y_semi[known_anom_id] = 1
+
+        device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        self.clf = FeaWAD(epochs=20, device=device)
+        self.clf.fit(self.X_train, y_semi)
+
+        self.clf2 = FeaWAD(data_type='ts', stride=50, seq_len=100, epochs=20,
+                            device=device, network='TCN')
+        self.clf2.fit(self.Xts_train, self.yts_train)
+
+    def test_parameters(self):
+        assert (hasattr(self.clf, 'decision_scores_') and
+                self.clf.decision_scores_ is not None)
+        assert (hasattr(self.clf, 'labels_') and
+                self.clf.labels_ is not None)
+        assert (hasattr(self.clf, 'threshold_') and
+                self.clf.threshold_ is not None)
+
+    # def test_train_scores(self):
+    #     assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
+
+    def test_train_scores(self):
+        assert_equal(len(self.clf2.decision_scores_), self.Xts_train.shape[0])
+        assert_equal(len(self.clf.decision_scores_), self.X_train.shape[0])
+
+    def test_prediction_scores(self):
+        pred_scores = self.clf.decision_function(self.X_test)
+        pred_scores2 = self.clf2.decision_function(self.Xts_test)
+
+        # check score shapes
+        assert_equal(pred_scores.shape[0], self.X_test.shape[0])
+        assert_equal(pred_scores2.shape[0], self.Xts_test.shape[0])
+
+        # # check performance
+        # auc = roc_auc_score(self.y_test, pred_scores)
+        # assert (auc >= self.roc_floor), f'auc is {auc}'
+
+    def test_prediction_labels(self):
+        pred_labels = self.clf.predict(self.X_test)
+        pred_labels2 = self.clf2.predict(self.Xts_test)
+        assert_equal(pred_labels.shape, self.y_test.shape)
+        assert_equal(pred_labels2.shape, self.yts_test.shape)
+
+    # def test_prediction_proba(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_linear(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='linear')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_unify(self):
+    #     pred_proba = self.clf.predict_proba(self.X_test, method='unify')
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    # def test_prediction_proba_parameter(self):
+    #     with assert_raises(ValueError):
+    #         self.clf.predict_proba(self.X_test, method='something')
+
+    def test_prediction_labels_confidence(self):
+        pred_labels, confidence = self.clf.predict(self.X_test,
+                                                   return_confidence=True)
+
+        assert_equal(pred_labels.shape, self.y_test.shape)
+        assert_equal(confidence.shape, self.y_test.shape)
+        assert (confidence.min() >= 0)
+        assert (confidence.max() <= 1)
+
+        pred_labels, confidence = self.clf2.predict(self.Xts_test,
+                                                    return_confidence=True)
+        assert_equal(pred_labels.shape, self.yts_test.shape)
+        assert_equal(confidence.shape, self.yts_test.shape)
+        assert (confidence.min() >= 0)
+        assert (confidence.max() <= 1)
+
+    # def test_prediction_proba_linear_confidence(self):
+    #     pred_proba, confidence = self.clf.predict_proba(self.X_test,
+    #                                                     method='linear',
+    #                                                     return_confidence=True)
+    #     assert (pred_proba.min() >= 0)
+    #     assert (pred_proba.max() <= 1)
+    #
+    #     assert_equal(confidence.shape, self.y_test.shape)
+    #     assert (confidence.min() >= 0)
+    #     assert (confidence.max() <= 1)
+    #
+    # def test_fit_predict(self):
+    #     pred_labels = self.clf.fit_predict(self.X_train)
+    #     assert_equal(pred_labels.shape, self.y_train.shape)
+    #
+    # def test_fit_predict_score(self):
+    #     self.clf.fit_predict_score(self.X_test, self.y_test)
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='roc_auc_score')
+    #     self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                scoring='prc_n_score')
+    #     with assert_raises(NotImplementedError):
+    #         self.clf.fit_predict_score(self.X_test, self.y_test,
+    #                                    scoring='something')
+    #
+    # def test_predict_rank(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, self.X_train.shape[0] + 1)
+    #     assert_array_less(-0.1, pred_ranks)
+    #
+    # def test_predict_rank_normalized(self):
+    #     pred_socres = self.clf.decision_function(self.X_test)
+    #     pred_ranks = self.clf._predict_rank(self.X_test, normalized=True)
+    #
+    #     # assert the order is reserved
+    #     assert_allclose(rankdata(pred_ranks), rankdata(pred_socres), atol=3)
+    #     assert_array_less(pred_ranks, 1.01)
+    #     assert_array_less(-0.1, pred_ranks)
+
+    # def test_plot(self):
+    #     os, cutoff1, cutoff2 = self.clf.explain_outlier(ind=1)
+    #     assert_array_less(0, os)
+
+    # def test_model_clone(self):
+    #     clone_clf = clone(self.clf)
+
+    def tearDown(self):
+        pass
+
+
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `deepod-0.2.0/deepod/utils/data.py` & `deepod-0.3.0/deepod/utils/data.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-# -*- coding: utf-8 -*-
-"""Utility functions for manipulating data
-"""
-# Author: Yue Zhao <zhaoy@cmu.edu>
-# Author: Yahya Almardeny <almardeny@gmail.com>
-# License: BSD 2 clause
-
-from warnings import warn
-from sklearn.utils import check_X_y
-from sklearn.utils import check_random_state
-from sklearn.utils import check_consistent_length
-import numpy as np
-
-
-def _generate_data(n_inliers, n_outliers, n_features, coef, offset,
-                   random_state, n_nan=0, n_inf=0):
-    """Internal function to generate data samples.
-
-    Parameters
-    ----------
-    n_inliers : int
-        The number of inliers.
-
-    n_outliers : int
-        The number of outliers.
-
-    n_features : int
-        The number of features (dimensions).
-
-    coef : float in range [0,1)+0.001
-        The coefficient of data generation.
-
-    offset : int
-        Adjust the value range of Gaussian and Uniform.
-
-    random_state : int, RandomState instance or None, optional (default=None)
-        If int, random_state is the seed used by the random number generator;
-        If RandomState instance, random_state is the random number generator;
-        If None, the random number generator is the RandomState instance used
-        by `np.random`.
-
-    n_nan : int
-        The number of values that are missing (np.NaN). Defaults to zero.
-
-    n_inf : int
-        The number of values that are infinite. (np.infty). Defaults to zero.
-
-    Returns
-    -------
-    X : numpy array of shape (n_train, n_features)
-        Data.
-
-    y : numpy array of shape (n_train,)
-        Ground truth.
-    """
-
-    inliers = coef * random_state.randn(n_inliers, n_features) + offset
-    outliers = random_state.uniform(low=-1 * offset, high=offset,
-                                    size=(n_outliers, n_features))
-    X = np.r_[inliers, outliers]
-
-    y = np.r_[np.zeros((n_inliers,)), np.ones((n_outliers,))]
-
-    if n_nan > 0:
-        X = np.r_[X, np.full((n_nan, n_features), np.NaN)]
-        y = np.r_[y, np.full((n_nan), np.NaN)]
-
-    if n_inf > 0:
-        X = np.r_[X, np.full((n_inf, n_features), np.infty)]
-        y = np.r_[y, np.full((n_inf), np.infty)]
-
-    return X, y
-
-
-
-def generate_data(n_train=1000, n_test=500, n_features=2, contamination=0.1,
-                  train_only=False, offset=10,
-                  random_state=None, n_nan=0, n_inf=0):
-    """Utility function to generate synthesized data.
-    Normal data is generated by a multivariate Gaussian distribution and
-    outliers are generated by a uniform distribution.
-    "X_train, X_test, y_train, y_test" are returned.
-
-    Parameters
-    ----------
-    n_train : int, (default=1000)
-        The number of training points to generate.
-
-    n_test : int, (default=500)
-        The number of test points to generate.
-
-    n_features : int, optional (default=2)
-        The number of features (dimensions).
-
-    contamination : float in (0., 0.5), optional (default=0.1)
-        The amount of contamination of the data set, i.e.
-        the proportion of outliers in the data set. Used when fitting to
-        define the threshold on the decision function.
-
-    train_only : bool, optional (default=False)
-        If true, generate train data only.
-
-    offset : int, optional (default=10)
-        Adjust the value range of Gaussian and Uniform.
-
-    random_state : int, RandomState instance or None, optional (default=None)
-        If int, random_state is the seed used by the random number generator;
-        If RandomState instance, random_state is the random number generator;
-        If None, the random number generator is the RandomState instance used
-        by `np.random`.
-
-    n_nan : int
-        The number of values that are missing (np.NaN). Defaults to zero.
-
-    n_inf : int
-        The number of values that are infinite. (np.infty). Defaults to zero.
-
-    Returns
-    -------
-    X_train : numpy array of shape (n_train, n_features)
-        Training data.
-
-    X_test : numpy array of shape (n_test, n_features)
-        Test data.
-
-    y_train : numpy array of shape (n_train,)
-        Training ground truth.
-
-    y_test : numpy array of shape (n_test,)
-        Test ground truth.
-
-    """
-
-    # initialize a random state and seeds for the instance
-    random_state = check_random_state(random_state)
-    offset_ = random_state.randint(low=offset)
-    coef_ = random_state.random_sample() + 0.001  # in case of underflow
-
-    n_outliers_train = int(n_train * contamination)
-    n_inliers_train = int(n_train - n_outliers_train)
-
-    X_train, y_train = _generate_data(n_inliers_train, n_outliers_train,
-                                      n_features, coef_, offset_, random_state,
-                                      n_nan, n_inf)
-
-    if train_only:
-        return X_train, y_train
-
-    n_outliers_test = int(n_test * contamination)
-    n_inliers_test = int(n_test - n_outliers_test)
-
-    X_test, y_test = _generate_data(n_inliers_test, n_outliers_test,
-                                    n_features, coef_, offset_, random_state,
-                                    n_nan, n_inf)
-
-    return X_train, X_test, y_train, y_test
-
+# -*- coding: utf-8 -*-
+"""Utility functions for manipulating data
+"""
+# Author: Yue Zhao <zhaoy@cmu.edu>
+# Author: Yahya Almardeny <almardeny@gmail.com>
+# License: BSD 2 clause
+
+from warnings import warn
+from sklearn.utils import check_X_y
+from sklearn.utils import check_random_state
+from sklearn.utils import check_consistent_length
+import numpy as np
+
+
+def _generate_data(n_inliers, n_outliers, n_features, coef, offset,
+                   random_state, n_nan=0, n_inf=0):
+    """Internal function to generate data samples.
+
+    Parameters
+    ----------
+    n_inliers : int
+        The number of inliers.
+
+    n_outliers : int
+        The number of outliers.
+
+    n_features : int
+        The number of features (dimensions).
+
+    coef : float in range [0,1)+0.001
+        The coefficient of data generation.
+
+    offset : int
+        Adjust the value range of Gaussian and Uniform.
+
+    random_state : int, RandomState instance or None, optional (default=None)
+        If int, random_state is the seed used by the random number generator;
+        If RandomState instance, random_state is the random number generator;
+        If None, the random number generator is the RandomState instance used
+        by `np.random`.
+
+    n_nan : int
+        The number of values that are missing (np.NaN). Defaults to zero.
+
+    n_inf : int
+        The number of values that are infinite. (np.infty). Defaults to zero.
+
+    Returns
+    -------
+    X : numpy array of shape (n_train, n_features)
+        Data.
+
+    y : numpy array of shape (n_train,)
+        Ground truth.
+    """
+
+    inliers = coef * random_state.randn(n_inliers, n_features) + offset
+    outliers = random_state.uniform(low=-1 * offset, high=offset,
+                                    size=(n_outliers, n_features))
+    X = np.r_[inliers, outliers]
+
+    y = np.r_[np.zeros((n_inliers,)), np.ones((n_outliers,))]
+
+    if n_nan > 0:
+        X = np.r_[X, np.full((n_nan, n_features), np.NaN)]
+        y = np.r_[y, np.full((n_nan), np.NaN)]
+
+    if n_inf > 0:
+        X = np.r_[X, np.full((n_inf, n_features), np.infty)]
+        y = np.r_[y, np.full((n_inf), np.infty)]
+
+    return X, y
+
+
+
+def generate_data(n_train=1000, n_test=500, n_features=2, contamination=0.1,
+                  train_only=False, offset=10,
+                  random_state=None, n_nan=0, n_inf=0):
+    """Utility function to generate synthesized data.
+    Normal data is generated by a multivariate Gaussian distribution and
+    outliers are generated by a uniform distribution.
+    "X_train, X_test, y_train, y_test" are returned.
+
+    Parameters
+    ----------
+    n_train : int, (default=1000)
+        The number of training points to generate.
+
+    n_test : int, (default=500)
+        The number of test points to generate.
+
+    n_features : int, optional (default=2)
+        The number of features (dimensions).
+
+    contamination : float in (0., 0.5), optional (default=0.1)
+        The amount of contamination of the data set, i.e.
+        the proportion of outliers in the data set. Used when fitting to
+        define the threshold on the decision function.
+
+    train_only : bool, optional (default=False)
+        If true, generate train data only.
+
+    offset : int, optional (default=10)
+        Adjust the value range of Gaussian and Uniform.
+
+    random_state : int, RandomState instance or None, optional (default=None)
+        If int, random_state is the seed used by the random number generator;
+        If RandomState instance, random_state is the random number generator;
+        If None, the random number generator is the RandomState instance used
+        by `np.random`.
+
+    n_nan : int
+        The number of values that are missing (np.NaN). Defaults to zero.
+
+    n_inf : int
+        The number of values that are infinite. (np.infty). Defaults to zero.
+
+    Returns
+    -------
+    X_train : numpy array of shape (n_train, n_features)
+        Training data.
+
+    X_test : numpy array of shape (n_test, n_features)
+        Test data.
+
+    y_train : numpy array of shape (n_train,)
+        Training ground truth.
+
+    y_test : numpy array of shape (n_test,)
+        Test ground truth.
+
+    """
+
+    # initialize a random state and seeds for the instance
+    random_state = check_random_state(random_state)
+    offset_ = random_state.randint(low=offset)
+    coef_ = random_state.random_sample() + 0.001  # in case of underflow
+
+    n_outliers_train = int(n_train * contamination)
+    n_inliers_train = int(n_train - n_outliers_train)
+
+    X_train, y_train = _generate_data(n_inliers_train, n_outliers_train,
+                                      n_features, coef_, offset_, random_state,
+                                      n_nan, n_inf)
+
+    if train_only:
+        return X_train, y_train
+
+    n_outliers_test = int(n_test * contamination)
+    n_inliers_test = int(n_test - n_outliers_test)
+
+    X_test, y_test = _generate_data(n_inliers_test, n_outliers_test,
+                                    n_features, coef_, offset_, random_state,
+                                    n_nan, n_inf)
+
+    return X_train, X_test, y_train, y_test
+
```

### Comparing `deepod-0.2.0/deepod.egg-info/SOURCES.txt` & `deepod-0.3.0/deepod.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,39 +6,53 @@
 deepod.egg-info/SOURCES.txt
 deepod.egg-info/dependency_links.txt
 deepod.egg-info/requires.txt
 deepod.egg-info/top_level.txt
 deepod/core/__init__.py
 deepod/core/base_model.py
 deepod/core/base_networks.py
+deepod/core/base_transformer_network.py
+deepod/core/base_transformer_network_dev.py
+deepod/core/network_utility.py
+deepod/core/transformer/__init__.py
+deepod/core/transformer/embed.py
+deepod/core/transformer/selfattention_family.py
 deepod/model_selection/__init__.py
 deepod/model_selection/fmms.py
 deepod/model_selection/gene_feature.py
 deepod/models/__init__.py
-deepod/models/anogan.py
+deepod/models/_local_test_.py
 deepod/models/devnet.py
+deepod/models/dif.py
 deepod/models/dsad.py
 deepod/models/dsvdd.py
+deepod/models/feawad.py
 deepod/models/goad.py
 deepod/models/icl.py
 deepod/models/neutral.py
 deepod/models/prenet.py
 deepod/models/rca.py
 deepod/models/rdp.py
 deepod/models/repen.py
+deepod/models/rosas.py
+deepod/models/slad.py
 deepod/test/__init__.py
 deepod/test/test_devnet.py
+deepod/test/test_dif.py
 deepod/test/test_dsad.py
 deepod/test/test_dsvdd.py
+deepod/test/test_feawad.py
 deepod/test/test_goad.py
 deepod/test/test_icl.py
 deepod/test/test_neutral.py
 deepod/test/test_prenet.py
 deepod/test/test_rca.py
 deepod/test/test_rdp.py
 deepod/test/test_repen.py
+deepod/test/test_slad.py
 deepod/utils/__init__.py
 deepod/utils/data.py
+deepod/utils/utility.py
 examples/__init__.py
 examples/detection_run_all.py
 examples/model_selection_fmms_example.py
 examples/utils.py
```

### Comparing `deepod-0.2.0/examples/detection_run_all.py` & `deepod-0.3.0/examples/detection_run_all.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import os
-import pickle
-import argparse
-import getpass
-import time
-import numpy as np
-import utils
-import importlib as imp
-
-
-dataset_root = f'/home/{getpass.getuser()}/dataset/1-tabular/'
-
-parser = argparse.ArgumentParser()
-parser.add_argument("--runs", type=int, default=5,
-                    help="how many times we repeat the experiments to obtain the average performance")
-parser.add_argument("--input_dir", type=str,
-                    default='ADBench-classical',
-                    help="the path of the data sets")
-parser.add_argument("--output_dir", type=str, default='@record/',
-                    help="the output file path")
-parser.add_argument("--dataset", type=str, default='FULL',
-                    help="FULL represents all the csv file in the folder, "
-                         "or a list of data set names splitted by comma")
-parser.add_argument("--model", type=str, default='DeepSVDD', help="",)
-parser.add_argument("--normalization", type=str, default='min-max', help="",)
-parser.add_argument('--silent_header', action='store_true')
-parser.add_argument("--flag", type=str, default='')
-args = parser.parse_args()
-
-
-os.makedirs(args.output_dir, exist_ok=True)
-data_lst = utils.get_data_lst(os.path.join(dataset_root, args.input_dir), args.dataset)
-print(os.path.join(dataset_root, args.input_dir))
-print(data_lst)
-
-module = imp.import_module('deepod.models')
-model_class = getattr(module, args.model)
-
-cur_time = time.strftime("%m-%d %H.%M.%S", time.localtime())
-result_file = os.path.join(args.output_dir, f'{args.model}.{args.input_dir}.{args.flag}.csv')
-
-if not args.silent_header:
-    f = open(result_file, 'a')
-    print('\n---------------------------------------------------------', file=f)
-    print(f'model: {args.model}, collection: {args.input_dir}, '
-          f'datasets: {args.dataset}, normalization: {args.normalization}, {args.runs}runs, ', file=f)
-    print('---------------------------------------------------------', file=f)
-    print('data, auc-roc, std, auc-pr, std, f1, std, time', file=f)
-    f.close()
-
-
-avg_auc_lst, avg_ap_lst, avg_f1_lst = [], [], []
-for file in data_lst:
-    dataset_name = os.path.splitext(os.path.split(file)[1])[0]
-
-    print(f'\n-------------------------{dataset_name}-----------------------')
-
-    split = '50%-normal'
-    print(f'train-test split: {split}, normalization: {args.normalization}')
-    x_train, y_train, x_test, y_test = utils.read_data(file=file,
-                                                       split=split,
-                                                       normalization=args.normalization,
-                                                       seed=42)
-    if x_train is None:
-        continue
-
-    auc_lst, ap_lst, f1_lst = np.zeros(args.runs), np.zeros(args.runs), np.zeros(args.runs)
-    t1_lst, t2_lst = np.zeros(args.runs), np.zeros(args.runs)
-    clf = None
-    for i in range(args.runs):
-        start_time = time.time()
-        print(f'\nRunning [{i+1}/{args.runs}] of [{args.model}] on Dataset [{dataset_name}]')
-
-        clf = model_class(epochs=50, random_state=42+i)
-        clf.fit(x_train)
-        train_time = time.time()
-        scores = clf.decision_function(x_test)
-        done_time = time.time()
-
-        auc, ap, f1 = utils.evaluate(y_test, scores)
-        auc_lst[i], ap_lst[i], f1_lst[i] = auc, ap, f1
-        t1_lst[i] = train_time - start_time
-        t2_lst[i] = done_time - start_time
-
-        print(f'{dataset_name}, {auc_lst[i]:.4f}, {ap_lst[i]:.4f}, {f1_lst[i]:.4f}, '
-              f'{t1_lst[i]:.1f}/{t2_lst[i]:.1f}, {args.model}')
-
-    avg_auc, avg_ap, avg_f1 = np.average(auc_lst), np.average(ap_lst), np.average(f1_lst)
-    std_auc, std_ap, std_f1 = np.std(auc_lst), np.std(ap_lst), np.std(f1_lst)
-    avg_time1 = np.average(t1_lst)
-    avg_time2 = np.average(t2_lst)
-
-    f = open(result_file, 'a')
-    txt = f'{dataset_name}, ' \
-          f'{avg_auc:.4f}, {std_auc:.4f}, ' \
-          f'{avg_ap:.4f}, {std_ap:.4f}, ' \
-          f'{avg_f1:.4f}, {std_f1:.4f}, ' \
-          f'{avg_time1:.1f}/{avg_time2:.1f}'
-    print(txt, file=f)
-    print(txt)
-    f.close()
-
-    avg_auc_lst.append(avg_auc)
-    avg_ap_lst.append(avg_ap)
-    avg_f1_lst.append(avg_f1)
-
-
+import os
+import pickle
+import argparse
+import getpass
+import time
+import numpy as np
+import utils
+import importlib as imp
+
+
+dataset_root = f'/home/{getpass.getuser()}/dataset/1-tabular/'
+
+parser = argparse.ArgumentParser()
+parser.add_argument("--runs", type=int, default=1,
+                    help="how many times we repeat the experiments to obtain the average performance")
+parser.add_argument("--input_dir", type=str,
+                    default='ADBench-classical',
+                    help="the path of the data sets")
+parser.add_argument("--output_dir", type=str, default='@record/',
+                    help="the output file path")
+parser.add_argument("--dataset", type=str, default='*thyroid*',
+                    help="FULL represents all the csv file in the folder, "
+                         "or a list of data set names splitted by comma")
+parser.add_argument("--model", type=str, default='SLAD', help="",)
+parser.add_argument("--normalization", type=str, default='min-max', help="",)
+parser.add_argument('--silent_header', action='store_true')
+parser.add_argument("--flag", type=str, default='')
+args = parser.parse_args()
+
+
+os.makedirs(args.output_dir, exist_ok=True)
+data_lst = utils.get_data_lst(os.path.join(dataset_root, args.input_dir), args.dataset)
+print(os.path.join(dataset_root, args.input_dir))
+print(data_lst)
+
+module = imp.import_module('deepod.models')
+model_class = getattr(module, args.model)
+
+cur_time = time.strftime("%m-%d %H.%M.%S", time.localtime())
+result_file = os.path.join(args.output_dir, f'{args.model}.{args.input_dir}.{args.flag}.csv')
+
+if not args.silent_header:
+    f = open(result_file, 'a')
+    print('\n---------------------------------------------------------', file=f)
+    print(f'model: {args.model}, collection: {args.input_dir}, '
+          f'datasets: {args.dataset}, normalization: {args.normalization}, {args.runs}runs, ', file=f)
+    print('---------------------------------------------------------', file=f)
+    print('data, auc-roc, std, auc-pr, std, f1, std, time', file=f)
+    f.close()
+
+
+avg_auc_lst, avg_ap_lst, avg_f1_lst = [], [], []
+for file in data_lst:
+    dataset_name = os.path.splitext(os.path.split(file)[1])[0]
+
+    print(f'\n-------------------------{dataset_name}-----------------------')
+
+    split = '50%-normal'
+    print(f'train-test split: {split}, normalization: {args.normalization}')
+    x_train, y_train, x_test, y_test = utils.read_data(file=file,
+                                                       split=split,
+                                                       normalization=args.normalization,
+                                                       seed=42)
+    if x_train is None:
+        continue
+
+    auc_lst, ap_lst, f1_lst = np.zeros(args.runs), np.zeros(args.runs), np.zeros(args.runs)
+    t1_lst, t2_lst = np.zeros(args.runs), np.zeros(args.runs)
+    clf = None
+    for i in range(args.runs):
+        start_time = time.time()
+        print(f'\nRunning [{i+1}/{args.runs}] of [{args.model}] on Dataset [{dataset_name}]')
+
+        clf = model_class(epochs=50, random_state=42+i)
+        clf.fit(x_train)
+        train_time = time.time()
+        scores = clf.decision_function(x_test)
+        done_time = time.time()
+
+        auc, ap, f1 = utils.evaluate(y_test, scores)
+        auc_lst[i], ap_lst[i], f1_lst[i] = auc, ap, f1
+        t1_lst[i] = train_time - start_time
+        t2_lst[i] = done_time - start_time
+
+        print(f'{dataset_name}, {auc_lst[i]:.4f}, {ap_lst[i]:.4f}, {f1_lst[i]:.4f}, '
+              f'{t1_lst[i]:.1f}/{t2_lst[i]:.1f}, {args.model}')
+
+    avg_auc, avg_ap, avg_f1 = np.average(auc_lst), np.average(ap_lst), np.average(f1_lst)
+    std_auc, std_ap, std_f1 = np.std(auc_lst), np.std(ap_lst), np.std(f1_lst)
+    avg_time1 = np.average(t1_lst)
+    avg_time2 = np.average(t2_lst)
+
+    f = open(result_file, 'a')
+    txt = f'{dataset_name}, ' \
+          f'{avg_auc:.4f}, {std_auc:.4f}, ' \
+          f'{avg_ap:.4f}, {std_ap:.4f}, ' \
+          f'{avg_f1:.4f}, {std_f1:.4f}, ' \
+          f'{avg_time1:.1f}/{avg_time2:.1f}'
+    print(txt, file=f)
+    print(txt)
+    f.close()
+
+    avg_auc_lst.append(avg_auc)
+    avg_ap_lst.append(avg_ap)
+    avg_f1_lst.append(avg_f1)
+
+
```

### Comparing `deepod-0.2.0/examples/model_selection_fmms_example.py` & `deepod-0.3.0/examples/model_selection_fmms_example.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from deepod.model_selection.fmms import FMMS
-import os
-import numpy as np
-import pandas as pd
-from sklearn.impute import SimpleImputer
-
-
-def get_data(feature_file, target_file):
-    df = pd.read_csv(target_file)
-    Y = df.values[:, 1:].astype(np.float64)
-    imp = SimpleImputer(missing_values=np.nan, strategy='mean')
-    Y = imp.fit(Y).transform(Y).T
-
-    df = pd.read_csv(feature_file)
-    df = df.drop(['Data'], axis=1)
-    df = df.fillna(0)
-
-    df = (df - df.min()) / (df.max() - df.min())
-    df = df.fillna(0)
-    X = df.values.astype(np.float32)
-
-    return Y, X
-
-
-if __name__ == '__main__':
-    random_state = 0
-    feature_f = os.path.join("data/feature.csv")
-    target_f = os.path.join("data/target.csv")
-    p_train, f_train = get_data(feature_f, target_f)
-    f_test = np.array([[1.227677502, 0.547297297, 0.25, 0.013513514, 0.234693979, 0.121621622, 8.222222222, 28.71360895, 9.512437578,
-                      -0.52749456, 13.58201658, 0.817380952, 0.758373016, 0.843551587, 0.829662698, 0.61265873, 0.54952381, -2.106840516,
-                      2.106840516, 2.890371758, 4.997212274, 15, 4, 18, 0, 148, 0, 0, 3, 0.446808511, -0.350354369, -0.558601676,
-                      0, 0, 0, 5, 0.2, 5.387046595, 2.302843498, 0.330402533, 2.208985222, 8, 2.933333333, 2, 1.569146973, 44]])
-    rfmms = FMMS()
-    rfmms.fit(f_train, p_train, save_path='./data/fmms.pt')
-    rfmms.predict(f=f_test, topn=5, load_path='./data/fmms.pt')
+from deepod.model_selection.fmms import FMMS
+import os
+import numpy as np
+import pandas as pd
+from sklearn.impute import SimpleImputer
+
+
+def get_data(feature_file, target_file):
+    df = pd.read_csv(target_file)
+    Y = df.values[:, 1:].astype(np.float64)
+    imp = SimpleImputer(missing_values=np.nan, strategy='mean')
+    Y = imp.fit(Y).transform(Y).T
+
+    df = pd.read_csv(feature_file)
+    df = df.drop(['Data'], axis=1)
+    df = df.fillna(0)
+
+    df = (df - df.min()) / (df.max() - df.min())
+    df = df.fillna(0)
+    X = df.values.astype(np.float32)
+
+    return Y, X
+
+
+if __name__ == '__main__':
+    random_state = 0
+    feature_f = os.path.join("data/feature.csv")
+    target_f = os.path.join("data/target.csv")
+    p_train, f_train = get_data(feature_f, target_f)
+    f_test = np.array([[1.227677502, 0.547297297, 0.25, 0.013513514, 0.234693979, 0.121621622, 8.222222222, 28.71360895, 9.512437578,
+                      -0.52749456, 13.58201658, 0.817380952, 0.758373016, 0.843551587, 0.829662698, 0.61265873, 0.54952381, -2.106840516,
+                      2.106840516, 2.890371758, 4.997212274, 15, 4, 18, 0, 148, 0, 0, 3, 0.446808511, -0.350354369, -0.558601676,
+                      0, 0, 0, 5, 0.2, 5.387046595, 2.302843498, 0.330402533, 2.208985222, 8, 2.933333333, 2, 1.569146973, 44]])
+    rfmms = FMMS()
+    rfmms.fit(f_train, p_train, save_path='./data/fmms.pt')
+    rfmms.predict(f=f_test, topn=5, load_path='./data/fmms.pt')
```

### Comparing `deepod-0.2.0/examples/utils.py` & `deepod-0.3.0/examples/utils.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-import os
-import sys
-import numpy as np
-import pandas as pd
-from tqdm import tqdm
-from sklearn.preprocessing import MinMaxScaler
-from sklearn import metrics
-from sklearn.model_selection import train_test_split
-from scipy.io import arff
-from glob import glob
-import datetime
-
-
-def read_data(file, split='50%-normal', normalization='z-score', seed=42):
-    """
-    read data from files, normalization, and perform train-test splitting
-
-    Parameters
-    ----------
-    file: str
-        file path of dataset
-
-    split: str (default='50%-normal', choice=['50%-normal', '60%', 'none'])
-        training-testing set splitting methods:
-            - if '50%-normal': use half of the normal data as training set,
-                and the other half attached with anomalies as testing set,
-                this splitting method is used in self-supervised studies GOAD [ICLR'20], NeuTraL [ICML'21]
-            - if 'none': use the whole set as both the training and testing set
-                This is commonly used in traditional methods.
-            - if '60%': use 60% data during training and the rest 40% data in testing,
-                while keeping the original anomaly ratio.
-
-    normalization: str (default='z-score', choice=['z-score', 'min-max'])
-
-    seed: int (default=42)
-        random seed
-    """
-
-    if file.endswith('.npz'):
-        data = np.load(file, allow_pickle=True)
-        x, y = data['X'], data['y']
-        y = np.array(y, dtype=int)
-    else:
-        if file.endswith('pkl'):
-            func = pd.read_pickle
-        elif file.endswith('csv'):
-            func = pd.read_csv
-        elif file.endswith('arff'):
-            def func(f):
-                df_ = pd.DataFrame(arff.loadarff(f)[0])
-                df_ = df_.replace({b'no': 0, b'yes': 1})
-                df_ = df_.drop('id', axis=1)
-                return df_
-        else:
-            raise NotImplementedError('')
-
-        df = func(file)
-        df.replace([np.inf, -np.inf], np.nan, inplace=True)
-        df.fillna(method='ffill', inplace=True)
-        x = df.values[:, :-1]
-        y = np.array(df.values[:, -1], dtype=int)
-
-    # train-test splitting
-    if split == '50%-normal':
-        rng = np.random.RandomState(seed)
-        idx = rng.permutation(np.arange(len(x)))
-        x, y = x[idx], y[idx]
-
-        norm_idx = np.where(y==0)[0]
-        anom_idx = np.where(y==1)[0]
-        split = int(0.5 * len(norm_idx))
-        train_norm_idx, test_norm_idx = norm_idx[:split], norm_idx[split:]
-
-        x_train = x[train_norm_idx]
-        y_train = y[train_norm_idx]
-
-        x_test = x[np.hstack([test_norm_idx, anom_idx])]
-        y_test = y[np.hstack([test_norm_idx, anom_idx])]
-
-        print(f'Original size: [{x.shape}], Normal/Anomaly: [{len(norm_idx)}/{len(anom_idx)}] \n'
-              f'After splitting: training/testing [{len(x_train)}/{len(x_test)}]')
-
-    elif split == '60%':
-        x_train, y_train, x_test, y_test = train_test_split(x, y, shuffle=True, random_state=seed,
-                                                            test_size=0.4, stratify=y)
-
-    else:
-        x_train, x_test = x.copy(), x.copy()
-        y_train, y_test = y.copy(), y.copy()
-
-    # normalization
-    if normalization == 'min-max':
-        minmax_scaler = MinMaxScaler()
-        minmax_scaler.fit(x_train)
-        x_train = minmax_scaler.transform(x_train)
-        x_test = minmax_scaler.transform(x_test)
-
-    elif normalization == 'z-score':
-        mus = np.mean(x_train, axis=0)
-        sds = np.std(x_train, axis=0)
-        sds[sds == 0] = 1
-        x_train = np.array([(xx - mus) / sds for xx in x_train])
-        x_test = np.array([(xx - mus) / sds for xx in x_test])
-
-    elif normalization == 'scale':
-        x_train = x_train / 255
-        x_test = x_test / 255
-
-    return x_train, y_train, x_test, y_test
-
-
-def min_max_normalize(x):
-    filter_lst = []
-    for k in range(x.shape[1]):
-        s = np.unique(x[:, k])
-        if len(s) <= 1:
-            filter_lst.append(k)
-    if len(filter_lst) > 0:
-        print('remove features', filter_lst)
-        x = np.delete(x, filter_lst, 1)
-
-    from sklearn.preprocessing import MinMaxScaler
-
-    scaler = MinMaxScaler()
-    scaler.fit(x)
-    x = scaler.transform(x)
-
-    return x
-
-
-def evaluate(y_true, scores):
-    """calculate evaluation metrics"""
-    roc_auc = metrics.roc_auc_score(y_true, scores)
-    ap = metrics.average_precision_score(y_true, scores)
-
-    # F1@k, using real percentage to calculate F1-score
-    ratio = 100.0 * len(np.where(y_true==0)[0]) / len(y_true)
-    thresh = np.percentile(scores, ratio)
-    y_pred = (scores >= thresh).astype(int)
-    y_true = y_true.astype(int)
-    precision, recall, f_score, support = metrics.precision_recall_fscore_support(y_true, y_pred, average='binary')
-
-    return roc_auc, ap, f_score
-
-
-def get_data_lst(dataset_dir, dataset):
-    if dataset == 'FULL':
-        print(os.path.join(dataset_dir, '*.*'))
-        data_lst = glob(os.path.join(dataset_dir, '*.*'))
-    else:
-        name_lst = dataset.split(',')
-        data_lst = []
-        for d in name_lst:
-            data_lst.extend(glob(os.path.join(dataset_dir, d + '.*')))
-    data_lst = sorted(data_lst)
-    return data_lst
-
-
-def add_irrelevant_features(x, ratio, seed=None):
-    n_samples, n_f = x.shape
-    size = int(ratio * n_f)
-
-    irr_new = np.zeros([n_samples, size])
-    np.random.seed(seed)
-    for i in tqdm(range(size)):
-        irr_new[:, i] = np.random.rand(n_samples)
-
-    # irr_new = np.zeros([n_samples, size])
-    # np.random.seed(seed)
-    # for i in range(size):
-    #     array = x[:, np.random.choice(x.shape[1], 1)]
-    #     new_array = array[np.random.permutation(n_samples)].flatten()
-    #     irr_new[:, i] = new_array
-
-    x_new = np.hstack([x, irr_new])
-
-    return x_new
-
-
-def adjust_contamination(x, y, contamination_r, swap_ratio=0.05, random_state=42):
-    """
-    add/remove anomalies in training data to replicate anomaly contaminated data sets.
-    randomly swap 5% features of two anomalies to avoid duplicate contaminated anomalies.
-    """
-    rng = np.random.RandomState(random_state)
-
-    anom_idx = np.where(y == 1)[0]
-    norm_idx = np.where(y == 0)[0]
-    n_cur_anom = len(anom_idx)
-    n_adj_anom = int(len(norm_idx) * contamination_r / (1. - contamination_r))
-
-    # x_train = np.delete(x_train, unknown_anom_idx, axis=0)
-    # y_train = np.delete(y_train, unknown_anom_idx, axis=0)
-    # noises = inject_noise(true_anoms, n_adj_noise, 42)
-    # x_train = np.append(x_train, noises, axis=0)
-    # y_train = np.append(y_train, np.zeros((noises.shape[0], 1)))
-
-    # inject noise
-    if n_cur_anom < n_adj_anom:
-        n_inj_noise = n_adj_anom - n_cur_anom
-        print(f'Control Contamination Rate: injecting [{n_inj_noise}] Noisy samples')
-
-        seed_anomalies = x[anom_idx]
-
-        n_sample, dim = seed_anomalies.shape
-        n_swap_feat = int(swap_ratio * dim)
-        inj_noise = np.empty((n_inj_noise, dim))
-        for i in np.arange(n_inj_noise):
-            idx = rng.choice(n_sample, 2, replace=False)
-            o1 = seed_anomalies[idx[0]]
-            o2 = seed_anomalies[idx[1]]
-            swap_feats = rng.choice(dim, n_swap_feat, replace=False)
-            inj_noise[i] = o1.copy()
-            inj_noise[i, swap_feats] = o2[swap_feats]
-
-        x = np.append(x, inj_noise, axis=0)
-        y = np.append(y, np.ones(n_inj_noise))
-
-    # remove noise
-    elif n_cur_anom > n_adj_anom:
-        n_remove = n_cur_anom - n_adj_anom
-        print(f'Control Contamination Rate: Removing [{n_remove}] Noise')
-
-        remove_id = anom_idx[rng.choice(n_cur_anom, n_remove, replace=False)]
-        print(x.shape)
-
-        x = np.delete(x, remove_id, 0)
-        y = np.delete(y, remove_id, 0)
-        print(x.shape)
-
-    return x, y
-
-
-def make_print_to_file(path='./'):
-
-    class Logger(object):
-        def __init__(self, filename="Default.log", path="./"):
-            self.terminal = sys.stdout
-            self.log = open(os.path.join(path, filename), "a", encoding='utf8', )
-
-        def write(self, message):
-            self.terminal.write(message)
-            self.log.write(message)
-
-        def flush(self):
-            pass
-
-    fileName = datetime.datetime.now().strftime('day' + '%Y_%m_%d')
-    sys.stdout = Logger(fileName + '.log', path=path)
-
-    #############################################################
-    # 这里输出之后的所有的输出的print 内容即将写入日志
-    #############################################################
-    print(fileName.center(60, '*'))
-
-
+import os
+import sys
+import numpy as np
+import pandas as pd
+from tqdm import tqdm
+from sklearn.preprocessing import MinMaxScaler
+from sklearn import metrics
+from sklearn.model_selection import train_test_split
+from scipy.io import arff
+from glob import glob
+import datetime
+
+
+def read_data(file, split='50%-normal', normalization='z-score', seed=42):
+    """
+    read data from files, normalization, and perform train-test splitting
+
+    Parameters
+    ----------
+    file: str
+        file path of dataset
+
+    split: str (default='50%-normal', choice=['50%-normal', '60%', 'none'])
+        training-testing set splitting methods:
+            - if '50%-normal': use half of the normal data as training set,
+                and the other half attached with anomalies as testing set,
+                this splitting method is used in self-supervised studies GOAD [ICLR'20], NeuTraL [ICML'21]
+            - if 'none': use the whole set as both the training and testing set
+                This is commonly used in traditional methods.
+            - if '60%': use 60% data during training and the rest 40% data in testing,
+                while keeping the original anomaly ratio.
+
+    normalization: str (default='z-score', choice=['z-score', 'min-max'])
+
+    seed: int (default=42)
+        random seed
+    """
+
+    if file.endswith('.npz'):
+        data = np.load(file, allow_pickle=True)
+        x, y = data['X'], data['y']
+        y = np.array(y, dtype=int)
+    else:
+        if file.endswith('pkl'):
+            func = pd.read_pickle
+        elif file.endswith('csv'):
+            func = pd.read_csv
+        elif file.endswith('arff'):
+            def func(f):
+                df_ = pd.DataFrame(arff.loadarff(f)[0])
+                df_ = df_.replace({b'no': 0, b'yes': 1})
+                df_ = df_.drop('id', axis=1)
+                return df_
+        else:
+            raise NotImplementedError('')
+
+        df = func(file)
+        df.replace([np.inf, -np.inf], np.nan, inplace=True)
+        df.fillna(method='ffill', inplace=True)
+        x = df.values[:, :-1]
+        y = np.array(df.values[:, -1], dtype=int)
+
+    # train-test splitting
+    if split == '50%-normal':
+        rng = np.random.RandomState(seed)
+        idx = rng.permutation(np.arange(len(x)))
+        x, y = x[idx], y[idx]
+
+        norm_idx = np.where(y==0)[0]
+        anom_idx = np.where(y==1)[0]
+        split = int(0.5 * len(norm_idx))
+        train_norm_idx, test_norm_idx = norm_idx[:split], norm_idx[split:]
+
+        x_train = x[train_norm_idx]
+        y_train = y[train_norm_idx]
+
+        x_test = x[np.hstack([test_norm_idx, anom_idx])]
+        y_test = y[np.hstack([test_norm_idx, anom_idx])]
+
+        print(f'Original size: [{x.shape}], Normal/Anomaly: [{len(norm_idx)}/{len(anom_idx)}] \n'
+              f'After splitting: training/testing [{len(x_train)}/{len(x_test)}]')
+
+    elif split == '60%':
+        x_train, y_train, x_test, y_test = train_test_split(x, y, shuffle=True, random_state=seed,
+                                                            test_size=0.4, stratify=y)
+
+    else:
+        x_train, x_test = x.copy(), x.copy()
+        y_train, y_test = y.copy(), y.copy()
+
+    # normalization
+    if normalization == 'min-max':
+        minmax_scaler = MinMaxScaler()
+        minmax_scaler.fit(x_train)
+        x_train = minmax_scaler.transform(x_train)
+        x_test = minmax_scaler.transform(x_test)
+
+    elif normalization == 'z-score':
+        mus = np.mean(x_train, axis=0)
+        sds = np.std(x_train, axis=0)
+        sds[sds == 0] = 1
+        x_train = np.array([(xx - mus) / sds for xx in x_train])
+        x_test = np.array([(xx - mus) / sds for xx in x_test])
+
+    elif normalization == 'scale':
+        x_train = x_train / 255
+        x_test = x_test / 255
+
+    return x_train, y_train, x_test, y_test
+
+
+def min_max_normalize(x):
+    filter_lst = []
+    for k in range(x.shape[1]):
+        s = np.unique(x[:, k])
+        if len(s) <= 1:
+            filter_lst.append(k)
+    if len(filter_lst) > 0:
+        print('remove features', filter_lst)
+        x = np.delete(x, filter_lst, 1)
+
+    from sklearn.preprocessing import MinMaxScaler
+
+    scaler = MinMaxScaler()
+    scaler.fit(x)
+    x = scaler.transform(x)
+
+    return x
+
+
+def evaluate(y_true, scores):
+    """calculate evaluation metrics"""
+    roc_auc = metrics.roc_auc_score(y_true, scores)
+    ap = metrics.average_precision_score(y_true, scores)
+
+    # F1@k, using real percentage to calculate F1-score
+    ratio = 100.0 * len(np.where(y_true==0)[0]) / len(y_true)
+    thresh = np.percentile(scores, ratio)
+    y_pred = (scores >= thresh).astype(int)
+    y_true = y_true.astype(int)
+    precision, recall, f_score, support = metrics.precision_recall_fscore_support(y_true, y_pred, average='binary')
+
+    return roc_auc, ap, f_score
+
+
+def get_data_lst(dataset_dir, dataset):
+    if dataset == 'FULL':
+        print(os.path.join(dataset_dir, '*.*'))
+        data_lst = glob(os.path.join(dataset_dir, '*.*'))
+    else:
+        name_lst = dataset.split(',')
+        data_lst = []
+        for d in name_lst:
+            data_lst.extend(glob(os.path.join(dataset_dir, d + '.*')))
+    data_lst = sorted(data_lst)
+    return data_lst
+
+
+def add_irrelevant_features(x, ratio, seed=None):
+    n_samples, n_f = x.shape
+    size = int(ratio * n_f)
+
+    irr_new = np.zeros([n_samples, size])
+    np.random.seed(seed)
+    for i in tqdm(range(size)):
+        irr_new[:, i] = np.random.rand(n_samples)
+
+    # irr_new = np.zeros([n_samples, size])
+    # np.random.seed(seed)
+    # for i in range(size):
+    #     array = x[:, np.random.choice(x.shape[1], 1)]
+    #     new_array = array[np.random.permutation(n_samples)].flatten()
+    #     irr_new[:, i] = new_array
+
+    x_new = np.hstack([x, irr_new])
+
+    return x_new
+
+
+def adjust_contamination(x, y, contamination_r, swap_ratio=0.05, random_state=42):
+    """
+    add/remove anomalies in training data to replicate anomaly contaminated data sets.
+    randomly swap 5% features of two anomalies to avoid duplicate contaminated anomalies.
+    """
+    rng = np.random.RandomState(random_state)
+
+    anom_idx = np.where(y == 1)[0]
+    norm_idx = np.where(y == 0)[0]
+    n_cur_anom = len(anom_idx)
+    n_adj_anom = int(len(norm_idx) * contamination_r / (1. - contamination_r))
+
+    # x_train = np.delete(x_train, unknown_anom_idx, axis=0)
+    # y_train = np.delete(y_train, unknown_anom_idx, axis=0)
+    # noises = inject_noise(true_anoms, n_adj_noise, 42)
+    # x_train = np.append(x_train, noises, axis=0)
+    # y_train = np.append(y_train, np.zeros((noises.shape[0], 1)))
+
+    # inject noise
+    if n_cur_anom < n_adj_anom:
+        n_inj_noise = n_adj_anom - n_cur_anom
+        print(f'Control Contamination Rate: injecting [{n_inj_noise}] Noisy samples')
+
+        seed_anomalies = x[anom_idx]
+
+        n_sample, dim = seed_anomalies.shape
+        n_swap_feat = int(swap_ratio * dim)
+        inj_noise = np.empty((n_inj_noise, dim))
+        for i in np.arange(n_inj_noise):
+            idx = rng.choice(n_sample, 2, replace=False)
+            o1 = seed_anomalies[idx[0]]
+            o2 = seed_anomalies[idx[1]]
+            swap_feats = rng.choice(dim, n_swap_feat, replace=False)
+            inj_noise[i] = o1.copy()
+            inj_noise[i, swap_feats] = o2[swap_feats]
+
+        x = np.append(x, inj_noise, axis=0)
+        y = np.append(y, np.ones(n_inj_noise))
+
+    # remove noise
+    elif n_cur_anom > n_adj_anom:
+        n_remove = n_cur_anom - n_adj_anom
+        print(f'Control Contamination Rate: Removing [{n_remove}] Noise')
+
+        remove_id = anom_idx[rng.choice(n_cur_anom, n_remove, replace=False)]
+        print(x.shape)
+
+        x = np.delete(x, remove_id, 0)
+        y = np.delete(y, remove_id, 0)
+        print(x.shape)
+
+    return x, y
+
+
+def make_print_to_file(path='./'):
+
+    class Logger(object):
+        def __init__(self, filename="Default.log", path="./"):
+            self.terminal = sys.stdout
+            self.log = open(os.path.join(path, filename), "a", encoding='utf8', )
+
+        def write(self, message):
+            self.terminal.write(message)
+            self.log.write(message)
+
+        def flush(self):
+            pass
+
+    fileName = datetime.datetime.now().strftime('day' + '%Y_%m_%d')
+    sys.stdout = Logger(fileName + '.log', path=path)
+
+    #############################################################
+    # 这里输出之后的所有的输出的print 内容即将写入日志
+    #############################################################
+    print(fileName.center(60, '*'))
+
+
```

