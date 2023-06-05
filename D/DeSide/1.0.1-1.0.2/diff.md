# Comparing `tmp/DeSide-1.0.1.tar.gz` & `tmp/DeSide-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeSide-1.0.1.tar", last modified: Thu May 11 15:47:48 2023, max compression
+gzip compressed data, was "DeSide-1.0.2.tar", last modified: Mon Jun  5 03:47:08 2023, max compression
```

## Comparing `DeSide-1.0.1.tar` & `DeSide-1.0.2.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.779008 DeSide-1.0.1/
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.412482 DeSide-1.0.1/DeSide.egg-info/
--rw-r--r--   0 belter     (502) staff       (20)     3771 2023-05-11 15:47:48.000000 DeSide-1.0.1/DeSide.egg-info/PKG-INFO
--rw-r--r--   0 belter     (502) staff       (20)     1253 2023-05-11 15:47:48.000000 DeSide-1.0.1/DeSide.egg-info/SOURCES.txt
--rw-r--r--   0 belter     (502) staff       (20)        1 2023-05-11 15:47:48.000000 DeSide-1.0.1/DeSide.egg-info/dependency_links.txt
--rw-r--r--   0 belter     (502) staff       (20)      162 2023-05-11 15:47:48.000000 DeSide-1.0.1/DeSide.egg-info/requires.txt
--rw-r--r--   0 belter     (502) staff       (20)        7 2023-05-11 15:47:48.000000 DeSide-1.0.1/DeSide.egg-info/top_level.txt
--rw-r--r--   0 belter     (502) staff       (20)   268413 2023-05-11 13:14:59.000000 DeSide-1.0.1/Fig.1a_b.svg
--rw-r--r--   0 belter     (502) staff       (20)     1087 2022-08-05 07:04:28.000000 DeSide-1.0.1/LICENSE
--rw-r--r--   0 belter     (502) staff       (20)       35 2023-05-11 15:29:01.000000 DeSide-1.0.1/MANIFEST.in
--rw-r--r--   0 belter     (502) staff       (20)     3771 2023-05-11 15:47:48.778731 DeSide-1.0.1/PKG-INFO
--rw-r--r--   0 belter     (502) staff       (20)     1585 2023-05-11 15:38:13.000000 DeSide-1.0.1/README.md
--rw-r--r--   0 belter     (502) staff       (20)        0 2022-01-24 03:11:46.000000 DeSide-1.0.1/README.rst
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.412891 DeSide-1.0.1/deside/
--rw-r--r--   0 belter     (502) staff       (20)      185 2022-08-05 07:50:43.000000 DeSide-1.0.1/deside/__init__.py
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.415309 DeSide-1.0.1/deside/bulk_cell/
--rw-r--r--   0 belter     (502) staff       (20)      386 2022-01-24 03:11:46.000000 DeSide-1.0.1/deside/bulk_cell/__init__.py
--rw-r--r--   0 belter     (502) staff       (20)    12936 2022-04-05 09:13:56.000000 DeSide-1.0.1/deside/bulk_cell/preprocessing.py
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.437516 DeSide-1.0.1/deside/decon_cf/
--rw-r--r--   0 belter     (502) staff       (20)       27 2022-08-06 08:53:38.000000 DeSide-1.0.1/deside/decon_cf/__init__.py
--rw-r--r--   0 belter     (502) staff       (20)    19538 2023-05-10 08:26:13.000000 DeSide-1.0.1/deside/decon_cf/deside.py
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.547011 DeSide-1.0.1/deside/plot/
--rw-r--r--   0 belter     (502) staff       (20)     1034 2023-02-16 03:55:25.000000 DeSide-1.0.1/deside/plot/__init__.py
--rw-r--r--   0 belter     (502) staff       (20)    36060 2023-05-11 09:12:03.000000 DeSide-1.0.1/deside/plot/evaluate_result.py
--rw-r--r--   0 belter     (502) staff       (20)    11225 2022-08-08 13:09:46.000000 DeSide-1.0.1/deside/plot/plot_clustering.py
--rw-r--r--   0 belter     (502) staff       (20)    24932 2022-08-09 09:42:30.000000 DeSide-1.0.1/deside/plot/plot_gene.py
--rw-r--r--   0 belter     (502) staff       (20)    14207 2022-08-09 10:47:39.000000 DeSide-1.0.1/deside/plot/plot_nn.py
--rw-r--r--   0 belter     (502) staff       (20)     2368 2022-08-08 13:09:46.000000 DeSide-1.0.1/deside/plot/plot_sample.py
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.583917 DeSide-1.0.1/deside/simulation/
--rw-r--r--   0 belter     (502) staff       (20)      399 2023-02-16 04:01:31.000000 DeSide-1.0.1/deside/simulation/__init__.py
--rw-r--r--   0 belter     (502) staff       (20)    88598 2023-05-11 09:12:03.000000 DeSide-1.0.1/deside/simulation/generate_data.py
--rw-r--r--   0 belter     (502) staff       (20)     2764 2022-01-24 03:11:46.000000 DeSide-1.0.1/deside/simulation/stats_test.py
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.617980 DeSide-1.0.1/deside/single_cell/
--rw-r--r--   0 belter     (502) staff       (20)      355 2022-11-07 14:05:55.000000 DeSide-1.0.1/deside/single_cell/__init__.py
--rw-r--r--   0 belter     (502) staff       (20)    37134 2023-02-16 04:01:31.000000 DeSide-1.0.1/deside/single_cell/preprocessing.py
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.697617 DeSide-1.0.1/deside/utility/
--rw-r--r--   0 belter     (502) staff       (20)     5199 2022-12-22 07:43:10.000000 DeSide-1.0.1/deside/utility/__init__.py
--rw-r--r--   0 belter     (502) staff       (20)    14535 2023-03-23 06:01:55.000000 DeSide-1.0.1/deside/utility/compare.py
--rw-r--r--   0 belter     (502) staff       (20)     6919 2023-02-16 04:01:31.000000 DeSide-1.0.1/deside/utility/core_obj.py
--rw-r--r--   0 belter     (502) staff       (20)     1337 2022-08-10 14:02:40.000000 DeSide-1.0.1/deside/utility/evaluation.py
--rw-r--r--   0 belter     (502) staff       (20)    39996 2023-03-19 07:58:41.000000 DeSide-1.0.1/deside/utility/pub_func.py
--rw-r--r--   0 belter     (502) staff       (20)    14824 2022-12-26 09:18:05.000000 DeSide-1.0.1/deside/utility/read_file.py
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.722457 DeSide-1.0.1/deside/workflow/
--rw-r--r--   0 belter     (502) staff       (20)      130 2022-08-06 08:30:55.000000 DeSide-1.0.1/deside/workflow/__init__.py
--rw-r--r--   0 belter     (502) staff       (20)    15411 2023-03-03 08:40:28.000000 DeSide-1.0.1/deside/workflow/workflow.py
-drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-05-11 15:47:48.778133 DeSide-1.0.1/docs/
--rw-r--r--   0 belter     (502) staff       (20)     6148 2022-08-05 07:13:41.000000 DeSide-1.0.1/docs/.DS_Store
--rw-r--r--   0 belter     (502) staff       (20)      634 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/Makefile
--rw-r--r--   0 belter     (502) staff       (20)     1549 2022-04-05 09:13:56.000000 DeSide-1.0.1/docs/changelog.md
--rw-r--r--   0 belter     (502) staff       (20)     2980 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/conf.py
--rw-r--r--   0 belter     (502) staff       (20)      100 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/contact.md
--rw-r--r--   0 belter     (502) staff       (20)       44 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/datasets.md
--rw-r--r--   0 belter     (502) staff       (20)      196 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/functions.md
--rw-r--r--   0 belter     (502) staff       (20)     1099 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/index.rst
--rw-r--r--   0 belter     (502) staff       (20)       57 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/installation.md
--rw-r--r--   0 belter     (502) staff       (20)      760 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/make.bat
--rw-r--r--   0 belter     (502) staff       (20)       52 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/requirements.txt
--rw-r--r--   0 belter     (502) staff       (20)       32 2022-01-24 03:11:46.000000 DeSide-1.0.1/docs/usage.md
--rw-r--r--   0 belter     (502) staff       (20)     1827 2023-05-11 15:47:15.000000 DeSide-1.0.1/pyproject.toml
--rw-r--r--   0 belter     (502) staff       (20)       38 2023-05-11 15:47:48.779096 DeSide-1.0.1/setup.cfg
--rw-r--r--   0 belter     (502) staff       (20)     1874 2023-05-11 14:50:56.000000 DeSide-1.0.1/setup.py
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.631914 DeSide-1.0.2/
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.466175 DeSide-1.0.2/DeSide.egg-info/
+-rw-r--r--   0 belter     (502) staff       (20)     5012 2023-06-05 03:47:08.000000 DeSide-1.0.2/DeSide.egg-info/PKG-INFO
+-rw-r--r--   0 belter     (502) staff       (20)     1095 2023-06-05 03:47:08.000000 DeSide-1.0.2/DeSide.egg-info/SOURCES.txt
+-rw-r--r--   0 belter     (502) staff       (20)        1 2023-06-05 03:47:08.000000 DeSide-1.0.2/DeSide.egg-info/dependency_links.txt
+-rw-r--r--   0 belter     (502) staff       (20)      249 2023-06-05 03:47:08.000000 DeSide-1.0.2/DeSide.egg-info/requires.txt
+-rw-r--r--   0 belter     (502) staff       (20)        7 2023-06-05 03:47:08.000000 DeSide-1.0.2/DeSide.egg-info/top_level.txt
+-rw-r--r--   0 belter     (502) staff       (20)   268413 2023-05-11 13:14:59.000000 DeSide-1.0.2/Fig.1a_b.svg
+-rw-r--r--   0 belter     (502) staff       (20)     1087 2022-08-05 07:04:28.000000 DeSide-1.0.2/LICENSE
+-rw-r--r--   0 belter     (502) staff       (20)       35 2023-05-11 15:29:01.000000 DeSide-1.0.2/MANIFEST.in
+-rw-r--r--   0 belter     (502) staff       (20)     5012 2023-06-05 03:47:08.631407 DeSide-1.0.2/PKG-INFO
+-rw-r--r--   0 belter     (502) staff       (20)     2985 2023-06-05 03:40:38.000000 DeSide-1.0.2/README.md
+-rw-r--r--   0 belter     (502) staff       (20)        0 2022-01-24 03:11:46.000000 DeSide-1.0.2/README.rst
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.466538 DeSide-1.0.2/deside/
+-rw-r--r--   0 belter     (502) staff       (20)      194 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/__init__.py
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.476925 DeSide-1.0.2/deside/bulk_cell/
+-rw-r--r--   0 belter     (502) staff       (20)      394 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/bulk_cell/__init__.py
+-rw-r--r--   0 belter     (502) staff       (20)    13209 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/bulk_cell/preprocessing.py
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.478713 DeSide-1.0.2/deside/decon_cf/
+-rw-r--r--   0 belter     (502) staff       (20)       28 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/decon_cf/__init__.py
+-rw-r--r--   0 belter     (502) staff       (20)    20691 2023-06-02 15:49:56.000000 DeSide-1.0.2/deside/decon_cf/deside.py
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.507013 DeSide-1.0.2/deside/plot/
+-rw-r--r--   0 belter     (502) staff       (20)     1054 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/plot/__init__.py
+-rw-r--r--   0 belter     (502) staff       (20)    36799 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/plot/evaluate_result.py
+-rw-r--r--   0 belter     (502) staff       (20)    11454 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/plot/plot_clustering.py
+-rw-r--r--   0 belter     (502) staff       (20)    25418 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/plot/plot_gene.py
+-rw-r--r--   0 belter     (502) staff       (20)    14501 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/plot/plot_nn.py
+-rw-r--r--   0 belter     (502) staff       (20)     2420 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/plot/plot_sample.py
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.536830 DeSide-1.0.2/deside/simulation/
+-rw-r--r--   0 belter     (502) staff       (20)      385 2023-05-30 12:30:28.000000 DeSide-1.0.2/deside/simulation/__init__.py
+-rw-r--r--   0 belter     (502) staff       (20)    91650 2023-05-30 12:53:48.000000 DeSide-1.0.2/deside/simulation/generate_data.py
+-rw-r--r--   0 belter     (502) staff       (20)     2843 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/simulation/stats_test.py
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.538662 DeSide-1.0.2/deside/single_cell/
+-rw-r--r--   0 belter     (502) staff       (20)      363 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/single_cell/__init__.py
+-rw-r--r--   0 belter     (502) staff       (20)    37807 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/single_cell/preprocessing.py
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.544260 DeSide-1.0.2/deside/utility/
+-rw-r--r--   0 belter     (502) staff       (20)     5291 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/utility/__init__.py
+-rw-r--r--   0 belter     (502) staff       (20)    14807 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/utility/compare.py
+-rw-r--r--   0 belter     (502) staff       (20)     7061 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/utility/core_obj.py
+-rw-r--r--   0 belter     (502) staff       (20)     1364 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/utility/evaluation.py
+-rw-r--r--   0 belter     (502) staff       (20)    40904 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/utility/pub_func.py
+-rw-r--r--   0 belter     (502) staff       (20)    16046 2023-05-30 13:01:42.000000 DeSide-1.0.2/deside/utility/read_file.py
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.566282 DeSide-1.0.2/deside/workflow/
+-rw-r--r--   0 belter     (502) staff       (20)      133 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/workflow/__init__.py
+-rw-r--r--   0 belter     (502) staff       (20)    15652 2023-05-30 07:37:38.000000 DeSide-1.0.2/deside/workflow/workflow.py
+drwxr-xr-x   0 belter     (502) staff       (20)        0 2023-06-05 03:47:08.615064 DeSide-1.0.2/docs/
+-rw-r--r--   0 belter     (502) staff       (20)     6148 2022-08-05 07:13:41.000000 DeSide-1.0.2/docs/.DS_Store
+-rw-r--r--   0 belter     (502) staff       (20)      634 2022-01-24 03:11:46.000000 DeSide-1.0.2/docs/Makefile
+-rw-r--r--   0 belter     (502) staff       (20)     1213 2023-06-05 02:55:08.000000 DeSide-1.0.2/docs/changelog.md
+-rw-r--r--   0 belter     (502) staff       (20)     3170 2023-06-02 15:49:56.000000 DeSide-1.0.2/docs/conf.py
+-rw-r--r--   0 belter     (502) staff       (20)      129 2023-06-02 15:49:56.000000 DeSide-1.0.2/docs/contact.md
+-rw-r--r--   0 belter     (502) staff       (20)     6396 2023-06-05 02:55:08.000000 DeSide-1.0.2/docs/datasets.md
+-rw-r--r--   0 belter     (502) staff       (20)      173 2023-05-30 10:05:24.000000 DeSide-1.0.2/docs/functions.md
+-rw-r--r--   0 belter     (502) staff       (20)     2079 2023-06-05 03:15:08.000000 DeSide-1.0.2/docs/index.rst
+-rw-r--r--   0 belter     (502) staff       (20)      914 2023-06-02 15:49:56.000000 DeSide-1.0.2/docs/installation.md
+-rw-r--r--   0 belter     (502) staff       (20)      760 2022-01-24 03:11:46.000000 DeSide-1.0.2/docs/make.bat
+-rw-r--r--   0 belter     (502) staff       (20)      274 2023-06-02 15:49:56.000000 DeSide-1.0.2/docs/requirements.txt
+-rw-r--r--   0 belter     (502) staff       (20)    15273 2023-06-02 15:56:16.000000 DeSide-1.0.2/docs/usage.md
+-rw-r--r--   0 belter     (502) staff       (20)     2131 2023-06-02 15:49:56.000000 DeSide-1.0.2/pyproject.toml
+-rw-r--r--   0 belter     (502) staff       (20)       38 2023-06-05 03:47:08.632085 DeSide-1.0.2/setup.cfg
```

### Comparing `DeSide-1.0.1/DeSide.egg-info/SOURCES.txt` & `DeSide-1.0.2/DeSide.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 Fig.1a_b.svg
 LICENSE
 MANIFEST.in
 README.md
 README.rst
 pyproject.toml
-setup.py
 DeSide.egg-info/PKG-INFO
 DeSide.egg-info/SOURCES.txt
 DeSide.egg-info/dependency_links.txt
 DeSide.egg-info/requires.txt
 DeSide.egg-info/top_level.txt
 deside/__init__.py
-deside.egg-info/PKG-INFO
-deside.egg-info/SOURCES.txt
-deside.egg-info/dependency_links.txt
-deside.egg-info/requires.txt
-deside.egg-info/top_level.txt
 deside/bulk_cell/__init__.py
 deside/bulk_cell/preprocessing.py
 deside/decon_cf/__init__.py
 deside/decon_cf/deside.py
 deside/plot/__init__.py
 deside/plot/evaluate_result.py
 deside/plot/plot_clustering.py
```

### Comparing `DeSide-1.0.1/Fig.1a_b.svg` & `DeSide-1.0.2/Fig.1a_b.svg`

 * *Files identical despite different names*

### Comparing `DeSide-1.0.1/LICENSE` & `DeSide-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DeSide-1.0.1/deside/bulk_cell/preprocessing.py` & `DeSide-1.0.2/deside/bulk_cell/preprocessing.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-import os
-import gzip
-import shutil
-import numpy as np
-import pandas as pd
-from tqdm import tqdm
-from ..utility import print_df, center_value, log2_transform, check_dir, get_sep
-# from ..utility import filter_gene_by_expression_min_max
-# from ..plot import plot_hcluster
-
-
-def get_data_from_firehose_raw(file_path, data_type):
-    """
-    get data from raw data file which is downloaded from firehose
-    http://gdac.broadinstitute.org/
-    :param file_path:
-    :param data_type: raw_count	or scaled_estimate
-    :return: a dataframe
-    """
-    print('>>> Start to read bulk expression file...')
-    bulk_raw_data = pd.read_csv(file_path, sep='\t', header=[0, 1], index_col=0)
-    idx = pd.IndexSlice
-    if data_type not in ['raw_count', 'scaled_estimate']:
-        raise TypeError('data_type should be raw_count or scaled_estimate')
-    bulk_exp = bulk_raw_data.loc[:, idx[:, data_type]]  # genes by samples
-    if data_type == 'scaled_estimate':
-        bulk_exp = bulk_exp * 1e6
-    bulk_exp.columns = bulk_exp.columns.get_level_values(0)
-    # print_df(bulk_exp)
-    return bulk_exp
-
-
-def get_gene_len(file_path):
-    """
-    get gene length (only exon)
-    gene info file downloaded from https://gdc.cancer.gov/about-data/gdc-data-processing/gdc-reference-files
-    - file TCGA.hg19.June2011.gaf
-    :param file_path:
-    :return:
-    """
-    gene_info = pd.read_csv(file_path, sep='\t', index_col='FeatureID')
-    gene_info['GeneLen'] = gene_info['FeatureCoordinates'].map(lambda x: int(x.split(',')[-1].split('-')[-1]))
-    return gene_info.loc[:, ['GeneLen']]
-
-
-def normalize_by_gene_len(bulk_exp, gene_len):
-    """
-    normalize bulk expression by gene length
-    :param bulk_exp: a data frame contains all expression data of each sample
-    :param gene_len: a data frame contains gene length information, 'GeneLen' is a column, bp
-    :return: normalized bulk expression
-    """
-    # common_genes = list(set(bulk_exp.index.to_list()) & set(gene_len.index.to_list()))
-    common_genes = [i for i in bulk_exp.index if i in gene_len.index]
-    bulk_exp = bulk_exp.loc[common_genes, :]
-    gene_len = gene_len.loc[common_genes, :]
-    bulk_norm_by_gene_len = bulk_exp / np.vstack(gene_len['GeneLen']) * 1000
-    return bulk_norm_by_gene_len
-
-
-def split_cancer_normal_samples(bulk_exp_fp, sample_info_fp):
-    """
-    split samples by sample information to cancer group and normal group
-    :param bulk_exp_fp:
-    :param sample_info_fp: get from http://gdac.broadinstitute.org/runs/stddata__latest/samples_report/HNSC.html
-    :return: dict
-           only cancer and normal tissue bulk expression data
-    """
-    bulk_exp = pd.read_csv(bulk_exp_fp, index_col=0)
-    sample_info = pd.read_csv(sample_info_fp, sep='\t')
-    sample_info = sample_info.loc[sample_info['Protocol'] == 'RSEM_genes', :].copy()
-    if '.' in bulk_exp.columns[0]:  # replaced '-' with '.' by R
-        bulk_exp.columns = [i.replace('.', '-') for i in bulk_exp.columns]
-    bulk_exp.index = bulk_exp.index.map(lambda x: x.split('|')[0] if x[0] != '?' else x)  # split and get gene name
-    # print_df(bulk_exp)
-    bulk_exp_normal_tissue = bulk_exp.loc[:, sample_info.loc[sample_info['sample type'] ==
-                                                             'Solid Tissue Normal', 'TCGA Barcode']]
-    # only keep Primary Solid Tumor
-    bulk_exp_cancer = bulk_exp.loc[:, sample_info.loc[sample_info['sample type'].isin(['Primary Solid Tumor']),
-                                                      'TCGA Barcode']]
-    bulk_exp_cancer = bulk_exp_cancer.loc[~bulk_exp_cancer.index.duplicated(keep='first')]
-    bulk_exp_normal_tissue = bulk_exp_normal_tissue.loc[~bulk_exp_normal_tissue.index.duplicated(keep='first')]
-    return {'cancer': bulk_exp_cancer, 'normal_tissue': bulk_exp_normal_tissue}
-
-
-def get_sample2subtype(bulk_exp, subtype_info_fp):
-    """
-    match subtype by the supplementary materials of HNSC marker paper
-    set the type of samples that don't include in marker paper as 'New'
-    :param bulk_exp: bulk expression dataframe, only use sample names in this bulk expression dataframe
-    :param subtype_info_fp: a file comes from the supplementary materials of HNSC marker paper
-    :return:
-    """
-    subtype = pd.read_excel(subtype_info_fp, index_col=0)
-    subtype.index = subtype.index.map(lambda x: x.replace('.', '-'))
-    sample2subtype = {}
-    for s in bulk_exp.columns.to_list():
-        _s = s[:12]
-        if _s in subtype.index:
-            _st = subtype.loc[_s, 'RNA']
-        else:
-            _st = 'New'
-        sample2subtype[s] = _st
-    sample2subtype_df = pd.DataFrame.from_dict(sample2subtype, orient='index')
-    # print('  >>> Shape of sample2subtype: {}'.format(sample2subtype_df.shape))
-    sample2subtype_df.rename(columns={0: 'subtype'}, inplace=True)
-    return sample2subtype_df
-
-
-def filter_by_corr_with_subclass(bulk_exp, subtype, corr_threshold=0.1):
-    """
-    filter samples by correlation with each subclass in marker paper
-
-    :param bulk_exp: pd.DataFrame
-        bulk cell expression value normalized by TMM (edgeR), don't need to log transform and center
-    :param subtype: pd.DataFrame
-        selected typical samples for each subtype, a dataframe with
-                     ['reordered_ind', 'cluster_id', 'subtype', 'reclass'] as columns, and 'sample_name' as index
-                     this information comes from the SI of marker paper
-                     Nature 517, 576–582 (2015). https://doi.org/10.1038/nature14129
-    :param corr_threshold:
-    :return:
-    """
-    # df_c = df_c.loc[:, ~df_c.index.isin(subtype.index)].copy()
-    mean_corr2each_subtype = pd.DataFrame(index=bulk_exp.columns)
-    # print_df(df_c)
-    _bulk_exp = bulk_exp.copy()
-    bulk_exp = log2_transform(bulk_exp)
-    bulk_exp = center_value(bulk_exp)
-    sample_corr = bulk_exp.corr()
-    for _st in subtype['subtype'].unique():
-        if _st != 'New':
-            print('current subtype: {}'.format(_st))
-            sample_corr2_with_st = sample_corr.loc[:, subtype[subtype['subtype'] == _st].index].copy()
-            print_df(sample_corr2_with_st)
-            mean_corr2each_subtype['mean_corr2{}'.format(_st.lower()[:3])] = sample_corr2_with_st.mean(axis=1)
-    samples_filtered = _bulk_exp.loc[:, np.sum(mean_corr2each_subtype.values >= corr_threshold, axis=1) == 1]
-    return samples_filtered
-
-
-def unzip_and_merge(sample_info_file_path: str, gdc_download_dir: str,
-                    result_dir: str, log_file_path: str,
-                    file_type='htseq.counts'):
-    """
-    Unzip and merge files downloaded from https://portal.gdc.cancer.gov/ by cancer types (Project ID).
-        And only keep "Primary Tumor" (one of Sample Type).
-
-    :param sample_info_file_path: gdc_sample_sheet, downloaded from GDC.
-        A .tsv file contains File ID, File Name, Data, Category, Data Type, Project ID, Case ID, Sample ID, Sample Type
-
-    :param gdc_download_dir: file folder contains downloaded data from GDC
-        One sample one .htseq.counts.gz file.
-    :param result_dir: where to save merged files
-
-    :param log_file_path: log file path
-
-    :param file_type: file type downloaded from GDC website
-
-    :return: None
-    """
-    print('Start to unzip downloaded files...')
-    check_dir(result_dir)
-    sample_info = pd.read_csv(sample_info_file_path, sep='\t')
-    # only keep primary tumor
-    sample_info = sample_info.loc[sample_info['Sample Type'] == 'Primary Tumor', :]
-    cancer_type2file_name = {}
-    file_name_counter = {}
-    file_name2new_path = {}
-    for _, row in tqdm(sample_info.iterrows()):
-        cancer_type = row['Project ID'].split('-')[1]
-        dir1 = row['File ID']
-        file_name = row['File Name']
-        file_path = os.path.join(gdc_download_dir, dir1, file_name)
-
-        if os.path.exists(file_path):
-            new_file_dir = os.path.join(result_dir, cancer_type)
-            check_dir(new_file_dir)
-            new_file_name = row['Sample ID'] + f'.{file_type}'
-            if new_file_name not in file_name_counter:
-                file_name_counter[new_file_name] = 0
-            file_name_counter[new_file_name] += 1
-            new_file_path = os.path.join(new_file_dir, new_file_name)
-            file_name2new_path[new_file_name] = new_file_path
-            if not os.path.exists(new_file_path):
-                with gzip.open(file_path, 'rb') as f_in:
-                    with open(new_file_path, 'wb') as f_out:
-                        shutil.copyfileobj(f_in, f_out)
-            if cancer_type not in cancer_type2file_name:
-                cancer_type2file_name[cancer_type] = []
-            cancer_type2file_name[cancer_type].append(new_file_name)
-        else:
-            with open(log_file_path, 'a') as f_log:
-                f_log.write(f'File path not found: {file_path}' + '\n')
-    for file_name, count in file_name_counter.items():
-        if count > 1:  # remove duplicate files (duplicate Sample ID)
-            if os.path.exists(file_name2new_path[file_name]):
-                os.remove(file_name2new_path[file_name])
-
-    # merge
-    print('Start to merge files by cancer type...')
-    for cancer_type, file_names in cancer_type2file_name.items():
-        merged_result_file_path = os.path.join(result_dir, cancer_type, f'merged_{cancer_type}_{file_type}.csv')
-        if not os.path.exists(merged_result_file_path):
-            current_files = []
-            for fn in file_names:
-                if file_name_counter[fn] == 1:
-                    current_df = pd.read_csv(file_name2new_path[fn], index_col=0, header=None, sep='\t')
-                    current_df.columns = [fn.split('.')[0]]
-                    current_df.index.name = 'gene_id'
-                    current_files.append(current_df)
-            merged_df = pd.concat(current_files, axis=1)
-            print(f'    {cancer_type}: {merged_df.shape}')
-            merged_df.to_csv(merged_result_file_path)
-
-
-def read_counts2tpm(read_counts_file_path: str, annotation_file_path: str,
-                    result_dir: str, file_type='htseq.counts', file_name_prefix: str = ''):
-    """
-    Convert read counts (htseq.counts) to TPM (transcript per million)
-
-    :param read_counts_file_path: the file path of merged read counts file (.htseq.counts),
-        separated by tab or comma, gene by sample
-
-    :param result_dir: the folder of saving result files
-
-    :param annotation_file_path:  file path of gencode.gene.info.v22.tsv
-        download from https://api.gdc.cancer.gov/data/b011ee3e-14d8-4a97-aed4-e0b10f6bbe82
-        or other annotation files, gene_type, gene_name and exon_length should be included
-
-    :param file_type: htseq.counts, raw data type downloaded from https://portal.gdc.cancer.gov/
-
-    :param file_name_prefix: prefix of result file, only for naming
-
-    :return: None
-    """
-    print(f'   Start to convert {file_type} to TPM...')
-    # current_result_dir = os.path.dirname(result_dir)
-    check_dir(result_dir)
-
-    sep = get_sep(read_counts_file_path)
-    read_counts = pd.read_csv(read_counts_file_path, index_col=0, sep=sep)
-    index_type = 'gene_name'
-    if 'ENSG' in read_counts.index[0]:
-        index_type = 'gene_id'
-    sep2 = get_sep(annotation_file_path, comment='#')
-    anno = pd.read_csv(annotation_file_path, index_col=index_type, sep=sep2, comment='#')
-    if index_type == 'gene_name':
-        anno['gene_name'] = anno.index
-    anno = anno.loc[anno['gene_type'] == 'protein_coding', ['gene_name', 'exon_length']]
-
-    # only keep protein coding genes and convert Ensembl gene id to gene symbol
-    filtered_read_counts_file_path = os.path.join(result_dir, f'{file_name_prefix}_{file_type}.csv')
-    tpm_file_path = os.path.join(result_dir, f'{file_name_prefix}_TPM.csv')
-    log2_trans_file_path = os.path.join(result_dir, f'{file_name_prefix}_log2tpm1p.csv')
-    if not os.path.exists(tpm_file_path):
-        merged_file = anno.merge(read_counts, left_index=True, right_index=True)
-        merged_file.set_index('gene_name', inplace=True)
-        duplicated_inx_bool = merged_file.index.duplicated(keep='first')
-        if np.any(duplicated_inx_bool):
-            print('   Remove duplicated genes by keeping the first row...')
-            merged_file = merged_file[~duplicated_inx_bool]
-        merged_file.iloc[:, 1:].to_csv(filtered_read_counts_file_path, float_format='%.3f')
-        norm_by_gene_len = merged_file.iloc[:, 1:] / np.vstack(merged_file['exon_length']) * 1000
-        tpm = norm_by_gene_len / np.hstack(norm_by_gene_len.sum(axis=0)) * 1e6
-        n, m = tpm.shape  # gene by sample
-        print('   There are {} genes and {} samples.'.format(n, m))
-        tpm.to_csv(tpm_file_path, float_format='%.3f')
-        tpm_t = tpm.T
-        log2tpm1p = log2_transform(tpm_t)
-        log2tpm1p.to_csv(log2_trans_file_path, float_format='%.3f')
-        print('   Converting finished.')
-    else:
-        print('   Previous result has existed in file {}.'.format(tpm_file_path))
+import os
+import gzip
+import shutil
+import numpy as np
+import pandas as pd
+from tqdm import tqdm
+from ..utility import print_df, center_value, log2_transform, check_dir, get_sep
+# from ..utility import filter_gene_by_expression_min_max
+# from ..plot import plot_hcluster
+
+
+def get_data_from_firehose_raw(file_path, data_type):
+    """
+    get data from raw data file which is downloaded from firehose
+    http://gdac.broadinstitute.org/
+    :param file_path:
+    :param data_type: raw_count	or scaled_estimate
+    :return: a dataframe
+    """
+    print('>>> Start to read bulk expression file...')
+    bulk_raw_data = pd.read_csv(file_path, sep='\t', header=[0, 1], index_col=0)
+    idx = pd.IndexSlice
+    if data_type not in ['raw_count', 'scaled_estimate']:
+        raise TypeError('data_type should be raw_count or scaled_estimate')
+    bulk_exp = bulk_raw_data.loc[:, idx[:, data_type]]  # genes by samples
+    if data_type == 'scaled_estimate':
+        bulk_exp = bulk_exp * 1e6
+    bulk_exp.columns = bulk_exp.columns.get_level_values(0)
+    # print_df(bulk_exp)
+    return bulk_exp
+
+
+def get_gene_len(file_path):
+    """
+    get gene length (only exon)
+    gene info file downloaded from https://gdc.cancer.gov/about-data/gdc-data-processing/gdc-reference-files
+    - file TCGA.hg19.June2011.gaf
+    :param file_path:
+    :return:
+    """
+    gene_info = pd.read_csv(file_path, sep='\t', index_col='FeatureID')
+    gene_info['GeneLen'] = gene_info['FeatureCoordinates'].map(lambda x: int(x.split(',')[-1].split('-')[-1]))
+    return gene_info.loc[:, ['GeneLen']]
+
+
+def normalize_by_gene_len(bulk_exp, gene_len):
+    """
+    normalize bulk expression by gene length
+    :param bulk_exp: a data frame contains all expression data of each sample
+    :param gene_len: a data frame contains gene length information, 'GeneLen' is a column, bp
+    :return: normalized bulk expression
+    """
+    # common_genes = list(set(bulk_exp.index.to_list()) & set(gene_len.index.to_list()))
+    common_genes = [i for i in bulk_exp.index if i in gene_len.index]
+    bulk_exp = bulk_exp.loc[common_genes, :]
+    gene_len = gene_len.loc[common_genes, :]
+    bulk_norm_by_gene_len = bulk_exp / np.vstack(gene_len['GeneLen']) * 1000
+    return bulk_norm_by_gene_len
+
+
+def split_cancer_normal_samples(bulk_exp_fp, sample_info_fp):
+    """
+    split samples by sample information to cancer group and normal group
+    :param bulk_exp_fp:
+    :param sample_info_fp: get from http://gdac.broadinstitute.org/runs/stddata__latest/samples_report/HNSC.html
+    :return: dict
+           only cancer and normal tissue bulk expression data
+    """
+    bulk_exp = pd.read_csv(bulk_exp_fp, index_col=0)
+    sample_info = pd.read_csv(sample_info_fp, sep='\t')
+    sample_info = sample_info.loc[sample_info['Protocol'] == 'RSEM_genes', :].copy()
+    if '.' in bulk_exp.columns[0]:  # replaced '-' with '.' by R
+        bulk_exp.columns = [i.replace('.', '-') for i in bulk_exp.columns]
+    bulk_exp.index = bulk_exp.index.map(lambda x: x.split('|')[0] if x[0] != '?' else x)  # split and get gene name
+    # print_df(bulk_exp)
+    bulk_exp_normal_tissue = bulk_exp.loc[:, sample_info.loc[sample_info['sample type'] ==
+                                                             'Solid Tissue Normal', 'TCGA Barcode']]
+    # only keep Primary Solid Tumor
+    bulk_exp_cancer = bulk_exp.loc[:, sample_info.loc[sample_info['sample type'].isin(['Primary Solid Tumor']),
+                                                      'TCGA Barcode']]
+    bulk_exp_cancer = bulk_exp_cancer.loc[~bulk_exp_cancer.index.duplicated(keep='first')]
+    bulk_exp_normal_tissue = bulk_exp_normal_tissue.loc[~bulk_exp_normal_tissue.index.duplicated(keep='first')]
+    return {'cancer': bulk_exp_cancer, 'normal_tissue': bulk_exp_normal_tissue}
+
+
+def get_sample2subtype(bulk_exp, subtype_info_fp):
+    """
+    match subtype by the supplementary materials of HNSC marker paper
+    set the type of samples that don't include in marker paper as 'New'
+    :param bulk_exp: bulk expression dataframe, only use sample names in this bulk expression dataframe
+    :param subtype_info_fp: a file comes from the supplementary materials of HNSC marker paper
+    :return:
+    """
+    subtype = pd.read_excel(subtype_info_fp, index_col=0)
+    subtype.index = subtype.index.map(lambda x: x.replace('.', '-'))
+    sample2subtype = {}
+    for s in bulk_exp.columns.to_list():
+        _s = s[:12]
+        if _s in subtype.index:
+            _st = subtype.loc[_s, 'RNA']
+        else:
+            _st = 'New'
+        sample2subtype[s] = _st
+    sample2subtype_df = pd.DataFrame.from_dict(sample2subtype, orient='index')
+    # print('  >>> Shape of sample2subtype: {}'.format(sample2subtype_df.shape))
+    sample2subtype_df.rename(columns={0: 'subtype'}, inplace=True)
+    return sample2subtype_df
+
+
+def filter_by_corr_with_subclass(bulk_exp, subtype, corr_threshold=0.1):
+    """
+    filter samples by correlation with each subclass in marker paper
+
+    :param bulk_exp: pd.DataFrame
+        bulk cell expression value normalized by TMM (edgeR), don't need to log transform and center
+    :param subtype: pd.DataFrame
+        selected typical samples for each subtype, a dataframe with
+                     ['reordered_ind', 'cluster_id', 'subtype', 'reclass'] as columns, and 'sample_name' as index
+                     this information comes from the SI of marker paper
+                     Nature 517, 576–582 (2015). https://doi.org/10.1038/nature14129
+    :param corr_threshold:
+    :return:
+    """
+    # df_c = df_c.loc[:, ~df_c.index.isin(subtype.index)].copy()
+    mean_corr2each_subtype = pd.DataFrame(index=bulk_exp.columns)
+    # print_df(df_c)
+    _bulk_exp = bulk_exp.copy()
+    bulk_exp = log2_transform(bulk_exp)
+    bulk_exp = center_value(bulk_exp)
+    sample_corr = bulk_exp.corr()
+    for _st in subtype['subtype'].unique():
+        if _st != 'New':
+            print('current subtype: {}'.format(_st))
+            sample_corr2_with_st = sample_corr.loc[:, subtype[subtype['subtype'] == _st].index].copy()
+            print_df(sample_corr2_with_st)
+            mean_corr2each_subtype['mean_corr2{}'.format(_st.lower()[:3])] = sample_corr2_with_st.mean(axis=1)
+    samples_filtered = _bulk_exp.loc[:, np.sum(mean_corr2each_subtype.values >= corr_threshold, axis=1) == 1]
+    return samples_filtered
+
+
+def unzip_and_merge(sample_info_file_path: str, gdc_download_dir: str,
+                    result_dir: str, log_file_path: str,
+                    file_type='htseq.counts'):
+    """
+    Unzip and merge files downloaded from https://portal.gdc.cancer.gov/ by cancer types (Project ID).
+        And only keep "Primary Tumor" (one of Sample Type).
+
+    :param sample_info_file_path: gdc_sample_sheet, downloaded from GDC.
+        A .tsv file contains File ID, File Name, Data, Category, Data Type, Project ID, Case ID, Sample ID, Sample Type
+
+    :param gdc_download_dir: file folder contains downloaded data from GDC
+        One sample one .htseq.counts.gz file.
+    :param result_dir: where to save merged files
+
+    :param log_file_path: log file path
+
+    :param file_type: file type downloaded from GDC website
+
+    :return: None
+    """
+    print('Start to unzip downloaded files...')
+    check_dir(result_dir)
+    sample_info = pd.read_csv(sample_info_file_path, sep='\t')
+    # only keep primary tumor
+    sample_info = sample_info.loc[sample_info['Sample Type'] == 'Primary Tumor', :]
+    cancer_type2file_name = {}
+    file_name_counter = {}
+    file_name2new_path = {}
+    for _, row in tqdm(sample_info.iterrows()):
+        cancer_type = row['Project ID'].split('-')[1]
+        dir1 = row['File ID']
+        file_name = row['File Name']
+        file_path = os.path.join(gdc_download_dir, dir1, file_name)
+
+        if os.path.exists(file_path):
+            new_file_dir = os.path.join(result_dir, cancer_type)
+            check_dir(new_file_dir)
+            new_file_name = row['Sample ID'] + f'.{file_type}'
+            if new_file_name not in file_name_counter:
+                file_name_counter[new_file_name] = 0
+            file_name_counter[new_file_name] += 1
+            new_file_path = os.path.join(new_file_dir, new_file_name)
+            file_name2new_path[new_file_name] = new_file_path
+            if not os.path.exists(new_file_path):
+                with gzip.open(file_path, 'rb') as f_in:
+                    with open(new_file_path, 'wb') as f_out:
+                        shutil.copyfileobj(f_in, f_out)
+            if cancer_type not in cancer_type2file_name:
+                cancer_type2file_name[cancer_type] = []
+            cancer_type2file_name[cancer_type].append(new_file_name)
+        else:
+            with open(log_file_path, 'a') as f_log:
+                f_log.write(f'File path not found: {file_path}' + '\n')
+    for file_name, count in file_name_counter.items():
+        if count > 1:  # remove duplicate files (duplicate Sample ID)
+            if os.path.exists(file_name2new_path[file_name]):
+                os.remove(file_name2new_path[file_name])
+
+    # merge
+    print('Start to merge files by cancer type...')
+    for cancer_type, file_names in cancer_type2file_name.items():
+        merged_result_file_path = os.path.join(result_dir, cancer_type, f'merged_{cancer_type}_{file_type}.csv')
+        if not os.path.exists(merged_result_file_path):
+            current_files = []
+            for fn in file_names:
+                if file_name_counter[fn] == 1:
+                    current_df = pd.read_csv(file_name2new_path[fn], index_col=0, header=None, sep='\t')
+                    current_df.columns = [fn.split('.')[0]]
+                    current_df.index.name = 'gene_id'
+                    current_files.append(current_df)
+            merged_df = pd.concat(current_files, axis=1)
+            print(f'    {cancer_type}: {merged_df.shape}')
+            merged_df.to_csv(merged_result_file_path)
+
+
+def read_counts2tpm(read_counts_file_path: str, annotation_file_path: str,
+                    result_dir: str, file_type='htseq.counts', file_name_prefix: str = ''):
+    """
+    Convert read counts (htseq.counts) to TPM (transcript per million)
+
+    :param read_counts_file_path: the file path of merged read counts file (.htseq.counts),
+        separated by tab or comma, gene by sample
+
+    :param result_dir: the folder of saving result files
+
+    :param annotation_file_path:  file path of gencode.gene.info.v22.tsv
+        download from https://api.gdc.cancer.gov/data/b011ee3e-14d8-4a97-aed4-e0b10f6bbe82
+        or other annotation files, gene_type, gene_name and exon_length should be included
+
+    :param file_type: htseq.counts, raw data type downloaded from https://portal.gdc.cancer.gov/
+
+    :param file_name_prefix: prefix of result file, only for naming
+
+    :return: None
+    """
+    print(f'   Start to convert {file_type} to TPM...')
+    # current_result_dir = os.path.dirname(result_dir)
+    check_dir(result_dir)
+
+    sep = get_sep(read_counts_file_path)
+    read_counts = pd.read_csv(read_counts_file_path, index_col=0, sep=sep)
+    index_type = 'gene_name'
+    if 'ENSG' in read_counts.index[0]:
+        index_type = 'gene_id'
+    sep2 = get_sep(annotation_file_path, comment='#')
+    anno = pd.read_csv(annotation_file_path, index_col=index_type, sep=sep2, comment='#')
+    if index_type == 'gene_name':
+        anno['gene_name'] = anno.index
+    anno = anno.loc[anno['gene_type'] == 'protein_coding', ['gene_name', 'exon_length']]
+
+    # only keep protein coding genes and convert Ensembl gene id to gene symbol
+    filtered_read_counts_file_path = os.path.join(result_dir, f'{file_name_prefix}_{file_type}.csv')
+    tpm_file_path = os.path.join(result_dir, f'{file_name_prefix}_TPM.csv')
+    log2_trans_file_path = os.path.join(result_dir, f'{file_name_prefix}_log2tpm1p.csv')
+    if not os.path.exists(tpm_file_path):
+        merged_file = anno.merge(read_counts, left_index=True, right_index=True)
+        merged_file.set_index('gene_name', inplace=True)
+        duplicated_inx_bool = merged_file.index.duplicated(keep='first')
+        if np.any(duplicated_inx_bool):
+            print('   Remove duplicated genes by keeping the first row...')
+            merged_file = merged_file[~duplicated_inx_bool]
+        merged_file.iloc[:, 1:].to_csv(filtered_read_counts_file_path, float_format='%.3f')
+        norm_by_gene_len = merged_file.iloc[:, 1:] / np.vstack(merged_file['exon_length']) * 1000
+        tpm = norm_by_gene_len / np.hstack(norm_by_gene_len.sum(axis=0)) * 1e6
+        n, m = tpm.shape  # gene by sample
+        print('   There are {} genes and {} samples.'.format(n, m))
+        tpm.to_csv(tpm_file_path, float_format='%.3f')
+        tpm_t = tpm.T
+        log2tpm1p = log2_transform(tpm_t)
+        log2tpm1p.to_csv(log2_trans_file_path, float_format='%.3f')
+        print('   Converting finished.')
+    else:
+        print('   Previous result has existed in file {}.'.format(tpm_file_path))
```

### Comparing `DeSide-1.0.1/deside/decon_cf/deside.py` & `DeSide-1.0.2/deside/decon_cf/deside.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,366 +1,390 @@
-import os
-import json
-import functools
-import numpy as np
-import pandas as pd
-from typing import Union
-import tensorflow as tf
-from tensorflow import keras
-from ..utility.read_file import ReadH5AD, ReadExp
-from ..utility import check_dir, print_msg
-from ..plot import plot_loss
-
-
-class DeSide(object):
-    def __init__(self, model_dir: str, log_file_path: str = None, model_name: str = 'DeSide'):
-        """
-        :param model_dir: the directory of saving well-trained model
-        :param log_file_path: the file path of log
-        :param model_name: only for naming
-        """
-        self.model_dir = model_dir
-        self.model = None
-        self.cell_types = None
-        self.gene_list = None
-        self.model_name = model_name
-        self.min_cell_fraction = 0.0001  # set to 0 if less than this value in predicted cell fractions
-        self.model_file_path = os.path.join(self.model_dir, f'model_{model_name}.h5')
-        self.cell_type_file_path = os.path.join(self.model_dir, 'celltypes.txt')
-        self.gene_list_file_path = os.path.join(self.model_dir, 'genes.txt')
-        self.training_set_file_path = None
-        self.hyper_params = None
-        self.one_minus_alpha = False
-        if log_file_path is None:
-            log_file_path = os.path.join(self.model_dir, 'log.txt')
-        self.log_file_path = log_file_path
-        check_dir(self.model_dir)
-
-    def build_model(self, input_shape, output_shape, hyper_params):
-        """
-        :param input_shape: the number of features (genes)
-        :param output_shape: the dimension of output (number of cell types to predict cell fraction)
-        :param hyper_params: pre-determined hyper-parameters for DeSide model
-        """
-        self.hyper_params = hyper_params
-        hidden_units = hyper_params['architecture'][0]
-        dropout_rates = hyper_params['architecture'][1]
-        using_batch_normalization = hyper_params['batch_normalization']
-        last_layer_activation_function = hyper_params['last_layer_activation']
-        if last_layer_activation_function == 'hard_sigmoid':
-            last_layer_activation_function = keras.activations.hard_sigmoid
-
-        # remove bias when using BatchNormalization
-        dense = functools.partial(keras.layers.Dense, use_bias=False, kernel_initializer='he_normal')
-        batch_normalization = keras.layers.BatchNormalization
-        activation = functools.partial(keras.layers.Activation, activation='relu')  # activate after BatchNormalization
-
-        if using_batch_normalization:
-            gep = keras.Input(shape=(input_shape,), name='input')
-            gep_normalized = batch_normalization()(gep)
-            features = dense(units=hidden_units[0])(gep_normalized)  # the first dense layer
-            features = batch_normalization()(features)
-            features = activation()(features)
-            for n_units in hidden_units[1:-1]:
-                features = dense(units=n_units)(features)
-                features = batch_normalization()(features)
-                features = activation()(features)
-            features = dense(units=hidden_units[-1], use_bias=True, activation='relu')(features)  # before output
-            y_pred = dense(units=output_shape, use_bias=True, activation=last_layer_activation_function)(features)
-            model = keras.Model(inputs=gep, outputs=y_pred, name='DeSide')
-        else:
-            gep = keras.Input(shape=(input_shape,), name='input')
-            features = dense(units=hidden_units[0], use_bias=True, activation='relu')(gep)  # the first dense layer
-            if dropout_rates[0] > 0:
-                features = keras.layers.Dropout(dropout_rates[0])(features)
-            hid_dropout = list(zip(hidden_units[1:], dropout_rates[1:]))
-            for n_units, dropout_rate in hid_dropout:
-                features = dense(units=n_units, use_bias=True, activation='relu')(features)
-                if dropout_rate > 0:
-                    features = keras.layers.Dropout(dropout_rate)(features)
-            y_pred = dense(units=output_shape, use_bias=True, activation=last_layer_activation_function)(features)
-            model = keras.Model(inputs=gep, outputs=y_pred, name='DeSide')
-        self.model = model
-
-    def train_model(self, training_set_file_path: Union[str, list], hyper_params: dict,
-                    cell_types: list = None, scaling_by_sample: bool = True, callback: bool = True,
-                    n_epoch: int = 10000, metrics: str = 'mse', n_patience: int = 100, scaling_by_constant=False,
-                    remove_cancer_cell=False, fine_tune=False, one_minus_alpha: bool = False, verbose=1):
-        """
-        :param training_set_file_path: the file path of training set, .h5ad file, log2cpm1p format, samples by genes
-        :param hyper_params: pre-determined hyper-parameters for DeSide model
-        :param cell_types: specific a list of cell types instead of using all cell types in training set
-        :param scaling_by_sample: whether to scale the expression values of each sample to [0, 1] by 'min_max'
-        :param callback: whether to use callback function when training model
-        :param n_epoch: the max number of epochs to train
-        :param metrics: mse (regression model) / accuracy (classifier)
-        :param n_patience: patience in early_stopping_callback
-        :param remove_cancer_cell: remove cancer cell from y if True, using "1-others"
-        :param fine_tune: fine tune pre-trained model
-        :param scaling_by_constant:
-        :param one_minus_alpha: use 1 - alpha for all cell types if True
-        :param verbose: 0: silent, 1: progress bar, 2: one line per epoch
-        """
-        self.one_minus_alpha = one_minus_alpha
-        if not os.path.exists(self.model_file_path):
-            print_msg('Start to training model...', log_file_path=self.log_file_path)
-            learning_rate = hyper_params['learning_rate']
-            loss_function = hyper_params['loss_function']
-            batch_size = hyper_params['batch_size']
-
-            # read training set
-            if type(training_set_file_path) == str:
-                training_set_file_path = [training_set_file_path]
-            x_list, y_list = [], []
-            print_msg('Start to reading training set...', log_file_path=self.log_file_path)
-            for file_path in training_set_file_path:
-                file_obj = ReadH5AD(file_path)
-                _x = file_obj.get_df()  # bulk cell GEPs, samples by genes
-                print('x shape:', _x.shape, file_path)
-                print('x head:', _x.head())
-                _y = file_obj.get_cell_fraction()  # cell fractions
-
-                x_list.append(_x.copy())
-                y_list.append(_y.copy())
-            x = pd.concat(x_list, join='inner', axis=0)
-            y = pd.concat(y_list)
-            if self.one_minus_alpha:
-                y = 1 - y
-            del file_obj, _x, _y, x_list, y_list
-
-            # scaling x
-            x_obj = ReadExp(x, exp_type='log_space')
-            if len(training_set_file_path) >= 2:
-                x_obj.to_tpm()  # if multiple training set, rescale to TPM, in case some genes were removed
-                x_obj.to_log2cpm1p()
-            if scaling_by_sample:
-                x_obj.do_scaling()
-            if scaling_by_constant:
-                # file_obj = ReadExp(_x, exp_type='log_space')
-                x_obj.do_scaling_by_constant()
-            x = x_obj.get_exp()
-
-            self.gene_list = x.columns.to_list()  # a list of all gene names
-
-            # filtering cell types in cell fraction file, for example removing the cell fraction of cancer cell
-            if cell_types is None:
-                self.cell_types = y.columns.to_list()  # a list
-            else:
-                self.cell_types = cell_types
-            if remove_cancer_cell:
-                self.cell_types = [i for i in self.cell_types if i != 'Cancer Cells']
-            y = y.loc[:, y.columns.isin(self.cell_types)]
-
-            # Save features and cell types
-            pd.DataFrame(self.cell_types).to_csv(self.cell_type_file_path, sep="\t")
-            pd.DataFrame(self.gene_list).to_csv(self.gene_list_file_path, sep="\t")
-
-            print(f'   Using cell types: {self.cell_types}')
-            print(f'   The shape of X is: {x.shape}, (n_sample, n_gene)')
-            print(f'   The shape of y is: {y.shape}, (n_sample, n_cell_type)')
-            if not fine_tune:
-                self.build_model(input_shape=len(self.gene_list), output_shape=len(self.cell_types),
-                                 hyper_params=hyper_params)
-            if self.model is None:
-                raise FileNotFoundError('pre-trained model should be assigned to self.model')
-            opt = keras.optimizers.Adam(learning_rate=learning_rate)
-            _loss_function = loss_function
-            _metrics = [metrics]
-            if loss_function == 'mae+rmse':
-                _loss_function = loss_fn_mae_rmse
-                _metrics = ['mae', keras.metrics.RootMeanSquaredError()]
-            self.model.compile(optimizer=opt, loss=_loss_function, metrics=_metrics)
-            print(self.model.summary())
-
-            # training model
-            if callback:
-                # Stop training when a monitored metric has stopped improving.
-                # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
-                early_stopping_callback = keras.callbacks.EarlyStopping(
-                    # patience=10,
-                    patience=n_patience,
-                    monitor='val_loss',
-                    mode='min',
-                    restore_best_weights=True)
-                history = self.model.fit(x.values, y.values, epochs=n_epoch,
-                                         batch_size=batch_size, verbose=verbose, validation_split=0.2,
-                                         callbacks=[early_stopping_callback])
-                # history = self.model.fit(x.values, y.values, epochs=n_epoch,
-                #                          batch_size=batch_size, verbose=2)
-
-            else:
-                history = self.model.fit(x.values, y.values, epochs=n_epoch,
-                                         batch_size=batch_size, verbose=verbose, validation_split=0.2)
-
-            hist = pd.DataFrame(history.history)
-            hist['epoch'] = history.epoch
-            hist.to_csv(os.path.join(self.model_dir, 'history_reg.csv'))
-
-            self.model.save(self.model_file_path)
-            plot_loss(hist, output_dir=self.model_dir, y_label=loss_function)
-            key_params_file_path = os.path.join(self.model_dir, 'key_params.txt')
-            print(f'   Key parameters during model training will be saved in {key_params_file_path}.')
-            self.save_params(key_params_file_path)
-            print_msg('Training done.', log_file_path=self.log_file_path)
-        else:
-            print(f'Previous model existed: {self.model_file_path}')
-
-    def get_x_before_predict(self, input_file, exp_type, transpose: bool = False, print_info: bool = True,
-                             scaling_by_sample: bool = False, scaling_by_constant: bool = True):
-        """
-        :param input_file: input file path
-        :param exp_type: 'log_space' or 'raw_space'
-        :param transpose: if True, transpose the input dataframe
-        :param print_info: if True, print info
-        :param scaling_by_sample: if True, scaling by sample
-        :param scaling_by_constant: if True, scaling by constant
-        :return: x
-        """
-        if self.gene_list is None:
-            self.gene_list = self.get_gene_list()
-        if exp_type not in ['TPM', 'log_space']:
-            raise ValueError(f'exp_type should be "TPM" or "log_space", "{exp_type}" is invalid.')
-        if '.h5ad' in input_file:
-            read_h5ad_obj = ReadH5AD(input_file)
-            _input_data = read_h5ad_obj.get_df()  # df, samples by genes
-            read_df_obj = ReadExp(_input_data, exp_type=exp_type, transpose=transpose)
-        elif np.any([i in input_file for i in ['.csv', '.txt', '.tsv']]) or (type(input_file) == pd.DataFrame):
-            read_df_obj = ReadExp(input_file, exp_type=exp_type, transpose=transpose)
-        else:
-            raise Exception(f'The current file path of raw data is {input_file}, '
-                            f'only "*_.csv", "*_.txt", "*_.tsv", or "*_.h5ad" is supported, ' 
-                            f'please check the file path and try again.')
-        # check gene list
-        read_df_obj.align_with_gene_list(gene_list=self.gene_list, fill_not_exist=True)
-        if exp_type != 'log_space':
-            read_df_obj.to_log2cpm1p()
-        if scaling_by_sample:
-            read_df_obj.do_scaling()
-        if scaling_by_constant:
-            read_df_obj.do_scaling_by_constant()
-        x = read_df_obj.get_exp()  # a DataFrame with log2(TPM + 1) gene expression values, samples by genes
-        # make sure that only genes in self.gene_list were used and keep the same order
-        # check duplication of gene names
-        _gene_list = x.columns.to_list()
-        if not (len(_gene_list) == len(set(_gene_list))):
-            Warning(
-                "Current input file contains duplicate genes! The first occurring gene will be kept.")
-            x = x.loc[:, ~x.columns.duplicated(keep='first')]
-        assert np.all(x.columns == self.gene_list), 'The gene list in input file is not the same as the ' \
-                                                    'gene list in pre-trained model.'
-        if print_info:
-            print(f'   > {len(self.gene_list)} genes included in pre-trained model and will be used for prediction.')
-            print(f'   The shape of X is: {x.shape}, (n_sample, n_gene)')
-        return x
-
-    def predict(self, input_file, exp_type, output_file_path: str = None,
-                transpose: bool = False, print_info: bool = True, add_cell_type: bool = False,
-                scaling_by_constant=False, scaling_by_sample=True, one_minus_alpha: bool = False):
-        """
-        :param input_file: the file path of input file (.csv / .h5ad / pd.Dataframe), samples x genes
-            simulated (or TCGA) bulk expression profiles, log2(TPM + 1) or TPM
-        :param output_file_path: the file path to save prediction result
-        :param exp_type: log_space or TPM, log_space means log2(TPM + 1)
-        :param transpose: transpose if exp_file formed as genes (index) by samples (columns)
-        :param print_info: print information during prediction
-        :param add_cell_type: only True when predicting cell types using classification model
-        :param scaling_by_constant: scaling log2(TPM + 1) by dividing 20
-        :param scaling_by_sample: scaling by sample, same as Scaden
-        :param one_minus_alpha: use 1 - alpha for all cell types if True
-        """
-        self.one_minus_alpha = one_minus_alpha
-        if print_info:
-            print('   Start to predict cell fractions by pre-trained model...')
-        if self.cell_types is None:
-            self.cell_types = self.get_cell_type()
-
-        # load input data
-        x = self.get_x_before_predict(input_file, exp_type, transpose=transpose, print_info=print_info,
-                                      scaling_by_constant=scaling_by_constant, scaling_by_sample=scaling_by_sample)
-
-        # load pre-trained model
-        if self.model is None:
-            try:
-                self.model = keras.models.load_model(self.model_file_path)
-            except ValueError:
-                self.model = keras.models.load_model(self.model_file_path,
-                                                     custom_objects={'loss_fn_mae_rmse': loss_fn_mae_rmse})
-            finally:
-                print(f'   Pre-trained model loaded from {self.model_file_path}.')
-        # predict using loaded model
-        pred_result = self.model.predict(x)
-        pred_df = pd.DataFrame(pred_result, index=x.index, columns=self.cell_types)
-        if self.one_minus_alpha:
-            pred_df = 1 - pred_df
-        pred_df[pred_df.values < self.min_cell_fraction] = 0
-        # pred_df.to_csv(out_name, sep="\t")
-        # rescaling to 1 if the sum of all cell types > 1
-        for sample_id, row in pred_df.iterrows():
-            if np.sum(row) > 1:
-                pred_df.loc[sample_id] = row / np.sum(row)
-
-        # Calculate 1-others
-        if 'Cancer Cells' not in pred_df.columns:
-            pred_df_with_1_others = pred_df.loc[:, [i for i in pred_df.columns if i != 'Cancer Cells']].copy()
-            pred_df_with_1_others['1-others'] = 1 - np.vstack(pred_df_with_1_others.sum(axis=1))
-            pred_df_with_1_others.loc[pred_df_with_1_others['1-others'] < 0, '1-others'] = 0
-            pred_df_with_1_others['Cancer Cells'] = pred_df_with_1_others['1-others']
-            pred_df = pred_df_with_1_others.copy()
-        # pred_df_with_1_others.to_csv(output_file_path, float_format='%.3f')
-        if add_cell_type:
-            pred_df['pred_cell_type'] = self.pred_cell_type_by_cell_frac(pred_cell_frac=pred_df)
-        if print_info:
-            print('   Model prediction done.')
-        if output_file_path is not None:
-            pred_df.to_csv(output_file_path, float_format='%.3f')
-        else:
-            return pred_df
-
-    def get_model(self):
-        if (self.model is None) and (os.path.exists(self.model_file_path)):
-            try:
-                self.model = keras.models.load_model(self.model_file_path)
-            except ValueError:
-                self.model = keras.models.load_model(self.model_file_path,
-                                                     custom_objects={'loss_fn_mae_rmse': loss_fn_mae_rmse})
-            finally:
-                print(f'   Pre-trained model loaded from {self.model_file_path}.')
-
-        return self.model
-
-    def get_parameters(self) -> dict:
-        key_params = {
-            'model_name': self.model_name, 'model_file_path': self.model_file_path,
-            'hyper_params': self.hyper_params, 'training_set_file_path': self.training_set_file_path,
-            'cell_type_file_path': self.cell_type_file_path,
-            'gene_list_file_path': self.gene_list_file_path, 'log_file_path': self.log_file_path
-        }
-        return key_params
-
-    def get_gene_list(self) -> list:
-        if (self.gene_list is None) and os.path.exists(self.gene_list_file_path):
-            self.gene_list = list(pd.read_csv(self.gene_list_file_path, sep='\t', index_col=0)['0'])
-        return self.gene_list
-
-    def get_cell_type(self) -> list:
-        if (self.cell_types is None) and os.path.exists(self.cell_type_file_path):
-            self.cell_types = list(pd.read_csv(self.cell_type_file_path, sep='\t', index_col=0)['0'])
-        return self.cell_types
-
-    def save_params(self, output_file_path: str):
-        key_params = self.get_parameters()
-        with open(output_file_path, 'w') as f_handle:
-            json.dump(key_params, fp=f_handle, indent=2)
-
-    def pred_cell_type_by_cell_frac(self, pred_cell_frac: pd.DataFrame) -> list:
-        """
-        convert predicted cell fractions to cell types
-        """
-        id2cell_type = {i: self.cell_types[i] for i in range(len(self.cell_types))}
-        pred_id = pred_cell_frac.values.argmax(axis=1)
-        return [id2cell_type[i] for i in pred_id]
-
-
-def loss_fn_mae_rmse(y_true, y_pred, alpha=0.8):
-    mae = keras.losses.MeanAbsoluteError()
-    mse = keras.losses.MeanSquaredError()
-    return alpha * mae(y_true, y_pred) + (1 - alpha) * tf.sqrt(mse(y_true, y_pred))
+import os
+import json
+import functools
+import numpy as np
+import pandas as pd
+from typing import Union
+import tensorflow as tf
+from tensorflow import keras
+from ..utility.read_file import ReadH5AD, ReadExp
+from ..utility import check_dir, print_msg
+from ..plot import plot_loss
+
+
+class DeSide(object):
+    """
+    DeSide model for predicting cell proportions in bulk RNA-seq data
+
+    :param model_dir: the directory of saving well-trained model
+    :param log_file_path: the file path of log
+    :param model_name: only for naming
+    """
+    def __init__(self, model_dir: str, log_file_path: str = None, model_name: str = 'DeSide'):
+        """
+        """
+        self.model_dir = model_dir
+        self.model = None
+        self.cell_types = None
+        self.gene_list = None
+        self.model_name = model_name
+        self.min_cell_fraction = 0.0001  # set to 0 if less than this value in predicted cell fractions
+        self.model_file_path = os.path.join(self.model_dir, f'model_{model_name}.h5')
+        self.cell_type_file_path = os.path.join(self.model_dir, 'celltypes.txt')
+        self.gene_list_file_path = os.path.join(self.model_dir, 'genes.txt')
+        self.training_set_file_path = None
+        self.hyper_params = None
+        self.one_minus_alpha = False
+        if log_file_path is None:
+            log_file_path = os.path.join(self.model_dir, 'log.txt')
+        self.log_file_path = log_file_path
+        check_dir(self.model_dir)
+
+    def _build_model(self, input_shape, output_shape, hyper_params):
+        """
+        :param input_shape: the number of features (genes)
+        :param output_shape: the dimension of output (number of cell types to predict cell fraction)
+        :param hyper_params: pre-determined hyper-parameters for DeSide model
+        """
+        self.hyper_params = hyper_params
+        hidden_units = hyper_params['architecture'][0]
+        dropout_rates = hyper_params['architecture'][1]
+        using_batch_normalization = hyper_params['batch_normalization']
+        last_layer_activation_function = hyper_params['last_layer_activation']
+        if last_layer_activation_function == 'hard_sigmoid':
+            last_layer_activation_function = keras.activations.hard_sigmoid
+
+        # remove bias when using BatchNormalization
+        dense = functools.partial(keras.layers.Dense, use_bias=False, kernel_initializer='he_normal')
+        batch_normalization = keras.layers.BatchNormalization
+        activation = functools.partial(keras.layers.Activation, activation='relu')  # activate after BatchNormalization
+
+        if using_batch_normalization:
+            gep = keras.Input(shape=(input_shape,), name='input')
+            gep_normalized = batch_normalization()(gep)
+            features = dense(units=hidden_units[0])(gep_normalized)  # the first dense layer
+            features = batch_normalization()(features)
+            features = activation()(features)
+            for n_units in hidden_units[1:-1]:
+                features = dense(units=n_units)(features)
+                features = batch_normalization()(features)
+                features = activation()(features)
+            features = dense(units=hidden_units[-1], use_bias=True, activation='relu')(features)  # before output
+            y_pred = dense(units=output_shape, use_bias=True, activation=last_layer_activation_function)(features)
+            model = keras.Model(inputs=gep, outputs=y_pred, name='DeSide')
+        else:
+            gep = keras.Input(shape=(input_shape,), name='input')
+            features = dense(units=hidden_units[0], use_bias=True, activation='relu')(gep)  # the first dense layer
+            if dropout_rates[0] > 0:
+                features = keras.layers.Dropout(dropout_rates[0])(features)
+            hid_dropout = list(zip(hidden_units[1:], dropout_rates[1:]))
+            for n_units, dropout_rate in hid_dropout:
+                features = dense(units=n_units, use_bias=True, activation='relu')(features)
+                if dropout_rate > 0:
+                    features = keras.layers.Dropout(dropout_rate)(features)
+            y_pred = dense(units=output_shape, use_bias=True, activation=last_layer_activation_function)(features)
+            model = keras.Model(inputs=gep, outputs=y_pred, name='DeSide')
+        self.model = model
+
+    def train_model(self, training_set_file_path: Union[str, list], hyper_params: dict,
+                    cell_types: list = None, scaling_by_sample: bool = True, callback: bool = True,
+                    n_epoch: int = 10000, metrics: str = 'mse', n_patience: int = 100, scaling_by_constant=False,
+                    remove_cancer_cell=False, fine_tune=False, one_minus_alpha: bool = False, verbose=1):
+        """
+        Training DeSide model
+
+        :param training_set_file_path: the file path of training set, .h5ad file, log2cpm1p format, samples by genes
+        :param hyper_params: pre-determined hyper-parameters for DeSide model
+        :param cell_types: specific a list of cell types instead of using all cell types in training set
+        :param scaling_by_sample: whether to scale the expression values of each sample to [0, 1] by 'min_max'
+        :param callback: whether to use callback function when training model
+        :param n_epoch: the max number of epochs to train
+        :param metrics: mse (regression model) / accuracy (classifier)
+        :param n_patience: patience in early_stopping_callback
+        :param remove_cancer_cell: remove cancer cell from y if True, using "1-others"
+        :param fine_tune: fine tune pre-trained model
+        :param scaling_by_constant: scaling GEP by dividing a constant in log space, default value is 20,
+            to make sure all expression values are in [0, 1) if True
+        :param one_minus_alpha: use 1 - alpha for all cell types if True
+        :param verbose: if printing progress during training, 0: silent, 1: progress bar, 2: one line per epoch
+        """
+        self.one_minus_alpha = one_minus_alpha
+        if not os.path.exists(self.model_file_path):
+            print_msg('Start to training model...', log_file_path=self.log_file_path)
+            learning_rate = hyper_params['learning_rate']
+            loss_function = hyper_params['loss_function']
+            batch_size = hyper_params['batch_size']
+
+            # read training set
+            if type(training_set_file_path) == str:
+                training_set_file_path = [training_set_file_path]
+            x_list, y_list = [], []
+            print_msg('Start to reading training set...', log_file_path=self.log_file_path)
+            for file_path in training_set_file_path:
+                file_obj = ReadH5AD(file_path)
+                _x = file_obj.get_df()  # bulk cell GEPs, samples by genes
+                print('x shape:', _x.shape, file_path)
+                print('x head:', _x.head())
+                _y = file_obj.get_cell_fraction()  # cell fractions
+
+                x_list.append(_x.copy())
+                y_list.append(_y.copy())
+            x = pd.concat(x_list, join='inner', axis=0)
+            y = pd.concat(y_list)
+            if self.one_minus_alpha:
+                y = 1 - y
+            del file_obj, _x, _y, x_list, y_list
+
+            # scaling x
+            x_obj = ReadExp(x, exp_type='log_space')
+            if len(training_set_file_path) >= 2:
+                x_obj.to_tpm()  # if multiple training set, rescale to TPM, in case some genes were removed
+                x_obj.to_log2cpm1p()
+            if scaling_by_sample:
+                x_obj.do_scaling()
+            if scaling_by_constant:
+                # file_obj = ReadExp(_x, exp_type='log_space')
+                x_obj.do_scaling_by_constant()
+            x = x_obj.get_exp()
+
+            self.gene_list = x.columns.to_list()  # a list of all gene names
+
+            # filtering cell types in cell fraction file, for example removing the cell fraction of cancer cell
+            if cell_types is None:
+                self.cell_types = y.columns.to_list()  # a list
+            else:
+                self.cell_types = cell_types
+            if remove_cancer_cell:
+                self.cell_types = [i for i in self.cell_types if i != 'Cancer Cells']
+            y = y.loc[:, y.columns.isin(self.cell_types)]
+
+            # Save features and cell types
+            pd.DataFrame(self.cell_types).to_csv(self.cell_type_file_path, sep="\t")
+            pd.DataFrame(self.gene_list).to_csv(self.gene_list_file_path, sep="\t")
+
+            print(f'   Using cell types: {self.cell_types}')
+            print(f'   The shape of X is: {x.shape}, (n_sample, n_gene)')
+            print(f'   The shape of y is: {y.shape}, (n_sample, n_cell_type)')
+            if not fine_tune:
+                self._build_model(input_shape=len(self.gene_list), output_shape=len(self.cell_types),
+                                  hyper_params=hyper_params)
+            if self.model is None:
+                raise FileNotFoundError('pre-trained model should be assigned to self.model')
+            opt = keras.optimizers.Adam(learning_rate=learning_rate)
+            _loss_function = loss_function
+            _metrics = [metrics]
+            if loss_function == 'mae+rmse':
+                _loss_function = loss_fn_mae_rmse
+                _metrics = ['mae', keras.metrics.RootMeanSquaredError()]
+            self.model.compile(optimizer=opt, loss=_loss_function, metrics=_metrics)
+            print(self.model.summary())
+
+            # training model
+            if callback:
+                # Stop training when a monitored metric has stopped improving.
+                # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
+                early_stopping_callback = keras.callbacks.EarlyStopping(
+                    # patience=10,
+                    patience=n_patience,
+                    monitor='val_loss',
+                    mode='min',
+                    restore_best_weights=True)
+                history = self.model.fit(x.values, y.values, epochs=n_epoch,
+                                         batch_size=batch_size, verbose=verbose, validation_split=0.2,
+                                         callbacks=[early_stopping_callback])
+                # history = self.model.fit(x.values, y.values, epochs=n_epoch,
+                #                          batch_size=batch_size, verbose=2)
+
+            else:
+                history = self.model.fit(x.values, y.values, epochs=n_epoch,
+                                         batch_size=batch_size, verbose=verbose, validation_split=0.2)
+
+            hist = pd.DataFrame(history.history)
+            hist['epoch'] = history.epoch
+            hist.to_csv(os.path.join(self.model_dir, 'history_reg.csv'))
+
+            self.model.save(self.model_file_path)
+            plot_loss(hist, output_dir=self.model_dir, y_label=loss_function)
+            key_params_file_path = os.path.join(self.model_dir, 'key_params.txt')
+            print(f'   Key parameters during model training will be saved in {key_params_file_path}.')
+            self.save_params(key_params_file_path)
+            print_msg('Training done.', log_file_path=self.log_file_path)
+        else:
+            print(f'Previous model existed: {self.model_file_path}')
+
+    def get_x_before_predict(self, input_file, exp_type, transpose: bool = False, print_info: bool = True,
+                             scaling_by_sample: bool = False, scaling_by_constant: bool = True):
+        """
+        :param input_file: input file path
+        :param exp_type: 'log_space' or 'raw_space'
+        :param transpose: if True, transpose the input dataframe
+        :param print_info: if True, print info
+        :param scaling_by_sample: if True, scaling by sample
+        :param scaling_by_constant: if True, scaling by constant
+        :return: x
+        """
+        if self.gene_list is None:
+            self.gene_list = self.get_gene_list()
+        if exp_type not in ['TPM', 'log_space']:
+            raise ValueError(f'exp_type should be "TPM" or "log_space", "{exp_type}" is invalid.')
+        if '.h5ad' in input_file:
+            read_h5ad_obj = ReadH5AD(input_file)
+            _input_data = read_h5ad_obj.get_df()  # df, samples by genes
+            read_df_obj = ReadExp(_input_data, exp_type=exp_type, transpose=transpose)
+        elif np.any([i in input_file for i in ['.csv', '.txt', '.tsv']]) or (type(input_file) == pd.DataFrame):
+            read_df_obj = ReadExp(input_file, exp_type=exp_type, transpose=transpose)
+        else:
+            raise Exception(f'The current file path of raw data is {input_file}, '
+                            f'only "*_.csv", "*_.txt", "*_.tsv", or "*_.h5ad" is supported, ' 
+                            f'please check the file path and try again.')
+        # check gene list
+        read_df_obj.align_with_gene_list(gene_list=self.gene_list, fill_not_exist=True)
+        if exp_type != 'log_space':
+            read_df_obj.to_log2cpm1p()
+        if scaling_by_sample:
+            read_df_obj.do_scaling()
+        if scaling_by_constant:
+            read_df_obj.do_scaling_by_constant()
+        x = read_df_obj.get_exp()  # a DataFrame with log2(TPM + 1) gene expression values, samples by genes
+        # make sure that only genes in self.gene_list were used and keep the same order
+        # check duplication of gene names
+        _gene_list = x.columns.to_list()
+        if not (len(_gene_list) == len(set(_gene_list))):
+            Warning(
+                "Current input file contains duplicate genes! The first occurring gene will be kept.")
+            x = x.loc[:, ~x.columns.duplicated(keep='first')]
+        assert np.all(x.columns == self.gene_list), 'The gene list in input file is not the same as the ' \
+                                                    'gene list in pre-trained model.'
+        if print_info:
+            print(f'   > {len(self.gene_list)} genes included in pre-trained model and will be used for prediction.')
+            print(f'   The shape of X is: {x.shape}, (n_sample, n_gene)')
+        return x
+
+    def predict(self, input_file, exp_type, output_file_path: str = None,
+                transpose: bool = False, print_info: bool = True, add_cell_type: bool = False,
+                scaling_by_constant=False, scaling_by_sample=True, one_minus_alpha: bool = False):
+        """
+        Predicting cell proportions using pre-trained model.
+
+        :param input_file: the file path of input file (.csv / .h5ad / pd.Dataframe), samples by genes
+            simulated (or TCGA) bulk expression profiles, log2(TPM + 1) or TPM
+        :param output_file_path: the file path to save prediction result
+        :param exp_type: log_space or TPM, log_space means log2(TPM + 1)
+        :param transpose: transpose if exp_file formed as genes (index) by samples (columns)
+        :param print_info: print information during prediction
+        :param add_cell_type: only True when predicting cell types using classification model
+        :param scaling_by_constant: scaling log2(TPM + 1) by dividing 20
+        :param scaling_by_sample: scaling by sample, same as Scaden
+        :param one_minus_alpha: use 1 - alpha for all cell types if True
+        """
+        self.one_minus_alpha = one_minus_alpha
+        if print_info:
+            print('   Start to predict cell fractions by pre-trained model...')
+        if self.cell_types is None:
+            self.cell_types = self.get_cell_type()
+
+        # load input data
+        x = self._get_x_before_predict(input_file, exp_type, transpose=transpose, print_info=print_info,
+                                       scaling_by_constant=scaling_by_constant, scaling_by_sample=scaling_by_sample)
+
+        # load pre-trained model
+        if self.model is None:
+            try:
+                self.model = keras.models.load_model(self.model_file_path)
+            except ValueError:
+                self.model = keras.models.load_model(self.model_file_path,
+                                                     custom_objects={'loss_fn_mae_rmse': loss_fn_mae_rmse})
+            finally:
+                print(f'   Pre-trained model loaded from {self.model_file_path}.')
+        # predict using loaded model
+        pred_result = self.model.predict(x)
+        pred_df = pd.DataFrame(pred_result, index=x.index, columns=self.cell_types)
+        if self.one_minus_alpha:
+            pred_df = 1 - pred_df
+        pred_df[pred_df.values < self.min_cell_fraction] = 0
+        # pred_df.to_csv(out_name, sep="\t")
+        # rescaling to 1 if the sum of all cell types > 1
+        for sample_id, row in pred_df.iterrows():
+            if np.sum(row) > 1:
+                pred_df.loc[sample_id] = row / np.sum(row)
+
+        # Calculate 1-others
+        if 'Cancer Cells' not in pred_df.columns:
+            pred_df_with_1_others = pred_df.loc[:, [i for i in pred_df.columns if i != 'Cancer Cells']].copy()
+            pred_df_with_1_others['1-others'] = 1 - np.vstack(pred_df_with_1_others.sum(axis=1))
+            pred_df_with_1_others.loc[pred_df_with_1_others['1-others'] < 0, '1-others'] = 0
+            pred_df_with_1_others['Cancer Cells'] = pred_df_with_1_others['1-others']
+            pred_df = pred_df_with_1_others.copy()
+        # pred_df_with_1_others.to_csv(output_file_path, float_format='%.3f')
+        if add_cell_type:
+            pred_df['pred_cell_type'] = self._pred_cell_type_by_cell_frac(pred_cell_frac=pred_df)
+        if print_info:
+            print('   Model prediction done.')
+        if output_file_path is not None:
+            pred_df.to_csv(output_file_path, float_format='%.3f')
+        else:
+            return pred_df
+
+    def get_model(self):
+        """
+        Load pre-trained model by `keras.models.load_model` if exists.
+
+        :return: pre-trained model
+        """
+        if (self.model is None) and (os.path.exists(self.model_file_path)):
+            try:
+                self.model = keras.models.load_model(self.model_file_path)
+            except ValueError:
+                self.model = keras.models.load_model(self.model_file_path,
+                                                     custom_objects={'loss_fn_mae_rmse': loss_fn_mae_rmse})
+            finally:
+                print(f'   Pre-trained model loaded from {self.model_file_path}.')
+
+        return self.model
+
+    def get_parameters(self) -> dict:
+        """
+        Get key parameters of the model.
+        """
+        key_params = {
+            'model_name': self.model_name, 'model_file_path': self.model_file_path,
+            'hyper_params': self.hyper_params, 'training_set_file_path': self.training_set_file_path,
+            'cell_type_file_path': self.cell_type_file_path,
+            'gene_list_file_path': self.gene_list_file_path, 'log_file_path': self.log_file_path
+        }
+        return key_params
+
+    def get_gene_list(self) -> list:
+        if (self.gene_list is None) and os.path.exists(self.gene_list_file_path):
+            self.gene_list = list(pd.read_csv(self.gene_list_file_path, sep='\t', index_col=0)['0'])
+        return self.gene_list
+
+    def get_cell_type(self) -> list:
+        if (self.cell_types is None) and os.path.exists(self.cell_type_file_path):
+            self.cell_types = list(pd.read_csv(self.cell_type_file_path, sep='\t', index_col=0)['0'])
+        return self.cell_types
+
+    def save_params(self, output_file_path: str):
+        key_params = self.get_parameters()
+        with open(output_file_path, 'w') as f_handle:
+            json.dump(key_params, fp=f_handle, indent=2)
+
+    def _pred_cell_type_by_cell_frac(self, pred_cell_frac: pd.DataFrame) -> list:
+        """
+        convert predicted cell fractions to cell types
+        """
+        id2cell_type = {i: self.cell_types[i] for i in range(len(self.cell_types))}
+        pred_id = pred_cell_frac.values.argmax(axis=1)
+        return [id2cell_type[i] for i in pred_id]
+
+
+def loss_fn_mae_rmse(y_true, y_pred, alpha=0.8):
+    """
+    Customized loss function for training the model. `alpha*MAE + (1-alpha)*RMSE`
+
+    :param y_true: true cell fractions
+    :param y_pred: predicted cell fractions
+    :param alpha: weight of MAE
+    """
+    mae = keras.losses.MeanAbsoluteError()
+    mse = keras.losses.MeanSquaredError()
+    return alpha * mae(y_true, y_pred) + (1 - alpha) * tf.sqrt(mse(y_true, y_pred))
```

### Comparing `DeSide-1.0.1/deside/plot/__init__.py` & `DeSide-1.0.2/deside/plot/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from .plot_clustering import plot_hcluster
-from .plot_gene import plot_single_gene_exp
-from .plot_gene import plot_gene_pdf
-from .plot_gene import plot_emt_gene_exp
-from .plot_nn import plot_loss, plot_paras, plot_paras_all_cell_types
-from .plot_nn import plot_corr_two_columns, plot_predicted_result
-from .evaluate_result import compare_y_y_pred_plot
-from .plot_clustering import t_sne_plot
-from .plot_gene import compare_exp_between_group, plot_cd8_marker
-from .evaluate_result import compare_exp_and_cell_fraction
-from .evaluate_result import compare_cell_fraction_across_cancer_type
-from .plot_gene import plot_gene_exp
-from .plot_gene import plot_marker_gene_in_cell_type
-from .plot_gene import plot_marker_exp
-from .plot_gene import plot_marker_ratio
-from .plot_sample import plot_sample_distribution
-from .evaluate_result import plot_pca, plot_clustermap
-from .evaluate_result import compare_mean_exp_with_cell_frac_across_algo
-from .evaluate_result import ScatterPlot
-from .evaluate_result import plot_pred_cell_prop_with_cpe
+from .plot_clustering import plot_hcluster
+from .plot_gene import plot_single_gene_exp
+from .plot_gene import plot_gene_pdf
+from .plot_gene import plot_emt_gene_exp
+from .plot_nn import plot_loss, plot_paras, plot_paras_all_cell_types
+from .plot_nn import plot_corr_two_columns, plot_predicted_result
+from .evaluate_result import compare_y_y_pred_plot
+from .plot_clustering import t_sne_plot
+from .plot_gene import compare_exp_between_group, plot_cd8_marker
+from .evaluate_result import compare_exp_and_cell_fraction
+from .evaluate_result import compare_cell_fraction_across_cancer_type
+from .plot_gene import plot_gene_exp
+from .plot_gene import plot_marker_gene_in_cell_type
+from .plot_gene import plot_marker_exp
+from .plot_gene import plot_marker_ratio
+from .plot_sample import plot_sample_distribution
+from .evaluate_result import plot_pca, plot_clustermap
+from .evaluate_result import compare_mean_exp_with_cell_frac_across_algo
+from .evaluate_result import ScatterPlot
+from .evaluate_result import plot_pred_cell_prop_with_cpe
```

### Comparing `DeSide-1.0.1/deside/plot/evaluate_result.py` & `DeSide-1.0.2/deside/plot/evaluate_result.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,739 +1,739 @@
-import os
-import pandas as pd
-import numpy as np
-from typing import Union
-import statsmodels.api as sm
-from sklearn.metrics import median_absolute_error
-from ..utility import (print_df, cal_relative_error, calculate_rmse, check_dir, get_corr,
-                       read_xy, read_df, get_inx2cell_type, log2_transform, get_core_zone_of_pca,
-                       get_ccc, read_cancer_purity, cancer_types)
-# from ..utility.read_file import ReadExp
-from .plot_nn import plot_corr_two_columns
-import matplotlib.patches as patches
-# import importlib
-import matplotlib.pyplot as plt
-import seaborn as sns
-import gc
-
-# set_fig_style()
-# sns.set(font_scale=1.5)
-# sns.set_style('white')
-
-
-class ScatterPlot(object):
-    def __init__(self, x: Union[str, pd.DataFrame], y: Union[str, pd.DataFrame],
-                 postfix: str = None, group_info: pd.DataFrame = None):
-        """
-        :param x:
-        :param y:
-        :param postfix: only for naming
-        """
-        self.x = read_xy(x)
-        self.y = read_xy(y)
-        common_inx = [i for i in self.x.index if i in self.y.index]
-        self.postfix = postfix
-        self.group_info = group_info
-        if group_info is not None:
-            common_inx = [i for i in group_info.index if i in common_inx]
-            self.group_info = self.group_info.loc[common_inx, :].copy()
-        self.show_columns = None
-        self.x = self.x.loc[common_inx, :].copy()
-        self.y = self.y.loc[common_inx, :].copy()
-        assert np.all(self.x.index == self.y.index)
-
-    def plot(self, show_columns: Union[list, dict], result_file_dir: str = None,
-             x_label: str = None, y_label: str = None, show_corr: bool = True, show_rmse: bool = False,
-             show_diag: bool = True, show_mae: bool = False, pred_by: str = None,
-             fig_size=(8, 8), group_by: str = None, show_reg_line: bool = False, s=6, order=1,
-             legend_loc: str = 'best'):
-        """
-        :param show_columns: a list of column names in both x and y, could be multiple common columns
-            or a dict {'x': '', 'y': ''}, only one column allowed
-        :param result_file_dir:
-        :param x_label:
-        :param y_label:
-        :param show_corr:
-        :param show_rmse:
-        :param show_mae: media absolute error
-        :param show_diag:
-        :param pred_by: algorithm name, will be showed in ylabel
-        :param fig_size:
-        :param group_by: one of the column name in self.group_info
-        :param show_reg_line: fit regression model
-        :param s:
-        :param legend_loc:
-        :param order: 1 for linear regression; 2 for Polynomial Regressions, y = alpha + beta1*x + beta2*x^2
-        """
-        plt.figure(figsize=fig_size)
-        ax = plt.axes()
-        # f, ax = plt.subplots(figsize=fig_size)
-
-        all_x = []
-        all_y = []
-        self.show_columns = show_columns
-        if type(show_columns) == dict:
-            self.x = self.x[show_columns['x']]
-            self.y = self.y[show_columns['y']]
-            all_x.append(self.x)
-            all_y.append(self.y)
-            if (self.group_info is not None) and (group_by in self.group_info.columns):
-                inx = self.group_info[group_by] == 1
-                plt.scatter(self.x[~inx], self.y[~inx], s=1, label='others')
-                plt.scatter(self.x[inx], self.y[inx], s=5, label=group_by, marker='x')
-            else:
-                plt.scatter(self.x, self.y, s=s, label=show_columns['x'], alpha=.4)  # only 1 vs 1 column
-            if show_reg_line:
-                self.fit_reg_model(ax=ax, order=order)
-        else:
-            show_columns = [i for i in show_columns if i in self.y.columns]
-            # for cell_type in show_columns:
-            #     if cell_type not in y_true.columns:
-            #         y_true[cell_type] = 0
-            show_columns_str = ', '.join(show_columns)
-            assert np.all([i in self.x.columns for i in show_columns]), \
-                f'All of elements in show_columns ({show_columns_str}) should exist in ' \
-                f'the columns of both x ({self.x.columns}) and y ({self.y.columns})'
-
-            # y_true = self.x.loc[:, show_columns]
-            # y_pred = self.y.loc[:, show_columns]
-            # sns.set(font_scale=font_scale)
-            # plt.figure(figsize=(8, 6))
-            for i, col in enumerate(show_columns):
-                _x = self.x.loc[:, col]
-                _y = self.y.loc[:, col]
-                all_x.append(_x)
-                all_y.append(_y)
-                plt.scatter(_x, _y, label=col, s=6, alpha=1 - 0.05 * i)
-        x_left, x_right = plt.xlim()
-        y_bottom, y_top = plt.ylim()
-        all_x = np.concatenate(all_x)
-        all_y = np.concatenate(all_y)
-        if show_diag:
-            _ = max(x_right, y_top)
-            plt.plot([0, _], [0, _], linestyle='--', color='tab:gray', linewidth=1, alpha=0.8)
-        if show_corr:  # show metrics in test set
-            corr = get_corr(all_x, all_y)
-            plt.text(x_right * 0.60, y_top * 0.10, 'corr = {:.2f}'.format(corr))
-        if show_mae:
-            mae = median_absolute_error(y_true=all_x, y_pred=all_y)
-            plt.text(x_right * 0.60, y_top * 0.07, 'MAE = {:.2f}'.format(mae))
-        if show_rmse and (not show_mae):
-            rmse = calculate_rmse(y_true=pd.DataFrame(all_x), y_pred=pd.DataFrame(all_y))
-            plt.text(x_right * 0.60, y_top * 0.07, 'RMSE = {:.2f}'.format(rmse))
-        if show_rmse and show_mae:
-            rmse = calculate_rmse(y_true=pd.DataFrame(all_x), y_pred=pd.DataFrame(all_y))
-            plt.text(x_right * 0.60, y_top * 0.04, 'RMSE = {:.2f}'.format(rmse))
-        if x_label:
-            plt.xlabel(x_label)
-        else:
-            plt.xlabel('y_true')
-        if y_label:
-            plt.ylabel(y_label)
-        elif pred_by:
-            plt.ylabel('Pred by {} (n={})'.format(pred_by, self.y.shape[0]))
-        else:
-            plt.ylabel('y_pred')
-        handles, labels = plt.gca().get_legend_handles_labels()
-        if len(labels) > 1:
-            plt.legend(handles[1:], labels[1:], loc=legend_loc)
-        plt.tight_layout()
-        if result_file_dir:
-            plt.savefig(os.path.join(result_file_dir,
-                                     'x_vs_y_{}.png'.format(self.postfix)), dpi=300)
-            # plt.savefig(os.path.join(result_file_dir,
-            #                          'x_vs_y_{}.svg'.format(self.postfix)), dpi=300)
-        plt.close()
-
-    def fit_reg_model(self, ax, alpha_ci=0.05, order=1):
-        """
-        only used 1vs1 comparing, show_columns should be a dict
-        :param ax
-        :param alpha_ci: 1 - alpha_ci confidence interval
-        :param order: 1 for linear regression; 2 for Polynomial Regressions, y = alpha + beta1*x + beta2*x^2
-        """
-
-        if type(self.x) == pd.Series:
-            self.x = self.x.to_frame()
-        self.x['intercept'] = 1  # add 1 as intercept column to fit `intercept`
-        x_col = self.show_columns['x']  # column name, a str
-        x_col_square = f'{x_col}^2'
-        if order == 2:
-            self.x[x_col_square] = self.x[x_col] ** 2
-            mod = sm.OLS(self.y, self.x.loc[:, ['intercept', x_col, x_col_square]])
-        else:  # order == 1
-            mod = sm.OLS(self.y, self.x.loc[:, ['intercept', x_col]])
-        res = mod.fit()
-        # print(res.summary())
-        ci = res.conf_int(alpha_ci)  # 95%, +/- 2*SD
-        x_lin = np.linspace(self.x[x_col].min(), self.x[x_col].max(), 20)
-        beta1 = res.params[x_col]
-        alpha = res.params['intercept']
-        beta2 = 0
-        if order == 2:
-            beta2 = res.params[x_col_square]
-        y_reg_line = x_lin * beta1 + alpha + np.power(x_lin, 2) * beta2
-        if order == 2:
-            y_lower_bound = x_lin * ci.loc[x_col, 0] + ci.loc['intercept', 0] + \
-                np.power(x_lin, 2) * ci.loc[x_col_square, 0]
-            y_upper_bound = x_lin * ci.loc[x_col, 1] + ci.loc['intercept', 1] + \
-                np.power(x_lin, 2) * ci.loc[x_col_square, 1]
-        else:
-            y_lower_bound = x_lin * ci.loc[x_col, 0] + ci.loc['intercept', 0]
-            y_upper_bound = x_lin * ci.loc[x_col, 1] + ci.loc['intercept', 1]
-        xy = self.x.copy()
-        xy['y_pred'] = self.x[x_col]
-        xy['y_true'] = self.y
-        sns.regplot(x='y_pred', y='y_true', data=xy, ax=ax, order=order,
-                    x_estimator=np.mean,
-                    scatter_kws={"s": 5}, color='tab:grey', x_bins=50,
-                    line_kws={'color': 'tab:orange', 'lw': 1, 'alpha': 0})
-        # p_value = res.pvalues[x_col]
-        # r2 = res.rsquared
-        # print(f'p_value: {p_value}', f'R^2: {r2}')
-        if alpha > 0:
-            if order == 2:
-                plt.plot(x_lin, y_reg_line, c='tab:orange',
-                         label=f'$y= {beta2: .2f}x^2 + {beta1: .2f}x + {alpha: .2f}$', linewidth=1)
-            else:
-                plt.plot(x_lin, y_reg_line, c='tab:orange',
-                         label=f'$y={beta1: .2f}x + {alpha: .2f}$', linewidth=1)
-        else:
-            if order == 2:
-                plt.plot(x_lin, y_reg_line, c='tab:orange',
-                         label=f'$y= {beta2: .2f}x^2 + {beta1: .2f}x - {abs(alpha): .2f}$', linewidth=1)
-            else:
-                plt.plot(x_lin, y_reg_line, c='tab:orange',
-                         label=f'$y={beta1: .2f}x - {abs(alpha): .2f}$', linewidth=1)
-        plt.plot(x_lin, y_lower_bound, c='tab:brown', label=f'{100 - alpha_ci * 100}% CI', linewidth=1)
-        plt.plot(x_lin, y_upper_bound, c='tab:brown', linewidth=1)
-
-
-def compare_y_y_pred_plot(y_true: Union[str, pd.DataFrame], y_pred: Union[str, pd.DataFrame],
-                          show_columns: list = None, result_file_dir=None, annotation: dict = None,
-                          y_label=None, x_label=None, model_name='average',
-                          show_metrics: bool = False, figsize: tuple = (8, 8)):
-    """
-    Plot y against y_pred to visualize the performance of prediction result
-
-    :param y_true: this file contains the ground truth of cell fractions when it was simulated
-
-    :param y_pred: this file contains the predicted value of y
-
-    :param show_columns: this list contains the name of columns that want to plot in figure
-
-    :param result_file_dir: where to save results
-
-    :param annotation: annotations that need to show in figure, {anno_name: {col1: value1, col2: value2, ...}, ...}
-
-    :param y_label: y label
-
-    :param x_label: x label
-
-    :param model_name: only for naming files
-
-    :param show_metrics: show correlation and RMSE
-
-    :param figsize: figure size
-
-    :return: None
-    """
-    if show_columns is None:
-        show_columns = []
-    if annotation is None:
-        annotation = {}
-    y_true = read_xy(a=y_true, xy='cell_frac')
-    y_pred = read_xy(a=y_pred, xy='cell_frac')
-    if '1-others' in show_columns:
-        if 'Cancer Cells' in y_true.columns:
-            y_true['1-others'] = y_true['Cancer Cells']
-        else:
-            y_true['1-others'] = 0
-    if ('T Cells' in y_pred.columns) and ('T Cells' not in y_true.columns):
-        y_true['T Cells'] = y_true.loc[:, ['CD4 T', 'CD8 T']].sum(axis=1)
-    # less cell type than show_columns for this dataset
-    show_columns = [i for i in show_columns if i in y_true.columns]
-    # for cell_type in show_columns:
-    #     if cell_type not in y_true.columns:
-    #         y_true[cell_type] = 0
-    show_columns_str = ', '.join(show_columns)
-    assert np.all([i in y_true.columns for i in show_columns]) and \
-           np.all([i in y_pred.columns for i in show_columns]), \
-           f'All of elements in show_columns ({show_columns_str}) should exist in ' \
-           f'the columns of both y_true ({y_true.columns}) and y_pred ({y_pred.columns})'
-    common_inx = [i for i in y_true.index if i in y_pred.index]
-
-    y_true = y_true.loc[common_inx, show_columns]
-    y_pred = y_pred.loc[common_inx, show_columns]
-    # sns.set(font_scale=font_scale)
-    plt.figure(figsize=figsize)
-    all_x = []
-    all_y = []
-    for i, col in enumerate(show_columns):
-        _x = y_true.loc[:, col]
-        _y = y_pred.loc[:, col]
-        all_x.append(_x)
-        all_y.append(_y)
-        plt.scatter(_x, _y, label=col, s=6, alpha=1 - 0.05 * i)
-        if annotation:
-            x_left, x_right = plt.xlim()
-            y_bottom, y_top = plt.ylim()
-            for k, v in annotation.items():
-                plt.text(x_left * 1.5, y_top * 0.8, 'k ({.4f})'.format(v[col]))
-    x_left, x_right = plt.xlim()
-    y_bottom, y_top = plt.ylim()
-    x_max = x_right + x_right * 0.01
-    y_max = y_top + y_top * 0.01
-    plt.plot([0, max(x_max, y_max)], [0, max(x_max, y_max)], linestyle='--', color='tab:gray')
-    if show_metrics:  # show metrics in test set
-        all_x = np.concatenate(all_x)
-        all_y = np.concatenate(all_y)
-        corr = get_corr(all_x, all_y)
-        rmse = calculate_rmse(y_true=pd.DataFrame(all_x), y_pred=pd.DataFrame(all_y))
-        plt.text(0.70 * x_max, 0.16 * y_max, 'corr = {:.3f}'.format(corr))
-        plt.text(0.70 * x_max, 0.10 * y_max, 'RMSE = {:.3f}'.format(rmse))
-    if x_label:
-        plt.xlabel(x_label)
-    else:
-        plt.xlabel('y_true')
-    if y_label:
-        plt.ylabel(y_label)
-    else:
-        plt.ylabel('y_predicted')
-    plt.legend()
-    plt.tight_layout()
-    if result_file_dir:
-        plt.savefig(os.path.join(result_file_dir, 'y_true_vs_y_pred_{}.png'.format(model_name)), dpi=200)
-    plt.close()
-
-
-def compare_exp_and_cell_fraction(merged_file_path, result_dir,
-                                  cell_types: list, clustering_ct: list = None,
-                                  outlier_file_path=None, predicted_by='DeSide', font_scale=1.5,
-                                  signature_score_method: str = 'mean_exp', update_figures=False):
-    """
-    Comparing the mean expression value (or gene signature score) of marker genes for each cell type
-      and the predicted cell fraction
-    :param merged_file_path: the file path of merged mean expression value of marker genes and predicted cell fractions,
-         sample by cell type, should contain `cancer_type` column to mark corresponding dataset
-    :param result_dir: where to save results
-    :param cell_types: all cell types used by DeSide
-    :param clustering_ct: cell types used for clustering of cancer types
-    :param outlier_file_path: the file path of outlier samples selected manually
-    :param predicted_by: the name of prediction algorithm, DeSide or Scaden
-    :param font_scale: font scaling
-    :param signature_score_method:
-    :param update_figures: if update figures
-    :return:
-    """
-    check_dir(result_dir)
-    # result_dir_scaled = result_dir + '_scaled'
-    # check_dir(result_dir_scaled)
-    cancer_type2corr_file_path = os.path.join(result_dir, 'cancer_type2corr.csv')
-    # print(merged_file_path)
-    merged_df = read_df(merged_file_path)
-    # merged_df = pd.read_csv(merged_file_path, index_col=0)
-    cancer_types = list(merged_df['cancer_type'].unique())
-    if 'T Cells' in cell_types and 'T Cells' not in merged_df.columns:
-        merged_df['T Cells'] = merged_df.loc[:, ['CD4 T', 'CD8 T']].sum(axis=1)
-    if (not os.path.exists(cancer_type2corr_file_path)) or update_figures:
-        if outlier_file_path is not None:
-            outlier_samples = pd.read_csv(outlier_file_path, index_col=0)
-            if outlier_samples.shape[0] > 0:  # remove outliers
-                print(f'   {outlier_samples.shape[0]} outlier samples will be removed...')
-                merged_df = merged_df.loc[~merged_df.index.isin(outlier_samples.index), :].copy()
-        cancer_type2corr = {}
-        for cancer_type in cancer_types:
-            print('----------------------------------------------------')
-            print(f'   Deal with cancer type: {cancer_type}...')
-            current_df = merged_df.loc[merged_df['cancer_type'] == cancer_type, :]
-            # print(current_df)
-            # plot predicted cell fraction against corresponding mean expression value of marker genes
-            current_result_dir = os.path.join(result_dir, cancer_type)
-            # current_result_dir_scaled = os.path.join(result_dir_scaled, cancer_type)
-            if cancer_type not in cancer_type2corr:
-                cancer_type2corr[cancer_type] = {}
-            for cell_type in cell_types:
-                # if cell_type != 'Cancer Cells':
-                if signature_score_method == 'mean_exp':
-                    method = 'marker_mean'
-                    if cell_type in ['B Cells'] and np.any(['max' in i for i in current_df.columns]):
-                        method = 'marker_max'
-                else:
-                    method = signature_score_method
-                col_name1 = cell_type + f'_{method}'
-                col_name2 = cell_type
-                cancer_type2corr[cancer_type][cell_type] = get_corr(current_df[col_name1], current_df[col_name2])
-                plot_corr_two_columns(df=current_df, col_name1=col_name1, col_name2=col_name2,
-                                      predicted_by=predicted_by, font_scale=font_scale, scale_exp=False,
-                                      output_dir=current_result_dir, diagonal=False, cancer_type=cancer_type,
-                                      update_figures=update_figures)
-
-            gc.collect()
-        cancer_type2corr_df = pd.DataFrame.from_dict(cancer_type2corr, orient='index')
-        cancer_type2corr_df.fillna(0, inplace=True)
-        cancer_type2corr_df.to_csv(cancer_type2corr_file_path, float_format='%.3f')
-    else:
-        print(f'   Using previous cancer_type2cor file from: {cancer_type2corr_file_path}.')
-        cancer_type2corr_df = pd.read_csv(cancer_type2corr_file_path, index_col=0)
-    # sns.set(font_scale=1.5)
-    if clustering_ct is not None:
-        c_ct = {'clustering_ct': clustering_ct}
-        other_ct = [ct for ct in cell_types if ct not in (clustering_ct + ['Cancer Cells'])]
-        if len(other_ct) >= 2:
-            c_ct = {'clustering_ct': clustering_ct, 'other_ct': other_ct}
-        for k, v in c_ct.items():
-            plot_clustermap(data=cancer_type2corr_df, columns=v,
-                            result_file_path=os.path.join(result_dir, f'cancer_type2corr_{k}.png'))
-
-
-def plot_clustermap(data: pd.DataFrame, columns: list, result_file_path: str):
-    """
-    plot cluster map for correlation table or cell fraction table
-    """
-    # sns.set(font_scale=1.5)
-    g = sns.clustermap(data.loc[:, columns], cmap="vlag")
-    plt.setp(g.ax_heatmap.xaxis.get_majorticklabels(), rotation=40)
-    plt.tight_layout()
-    plt.savefig(result_file_path, dpi=200)
-    # plt.show()
-    plt.close('all')
-
-
-def compare_cell_fraction_across_cancer_type(merged_cell_fraction: pd.DataFrame, result_dir='.', cell_type: str = '',
-                                             xlabel: str = 'Cancer Type',
-                                             ylabel: str = 'Tumor purity in each sample (CPE)',
-                                             outlier_file_path: str = None, cell_type2max: float = 0.0):
-    """
-    Specific plotting for file cancer_purity.csv, downloaded from Aran, D., Sirota, M. & Butte,
-    A. Systematic pan-cancer analysis of tumour purity. Nat Commun 6, 8971 (2015). https://doi.org/10.1038/ncomms9971
-
-    And other predicted cell fractions across all cancer types can be plotted.
-
-    :param merged_cell_fraction: merged cell fraction predicted by DeSide
-
-    :param cell_type: current cell type to plot
-
-    :param result_dir: where to save result
-
-    :param xlabel: x label
-
-    :param ylabel: y label
-
-    :param outlier_file_path:
-
-    :param cell_type2max: max cell fraction to keep when plotting
-
-    :return: None
-    """
-    x = 'cancer_type'
-    check_dir(result_dir)
-
-    if outlier_file_path is not None:
-        outlier_samples = pd.read_csv(outlier_file_path, index_col=0)
-        if outlier_samples.shape[0] > 0:  # remove outliers
-            print(f'   {outlier_samples.shape[0]} outlier samples will be removed...')
-            merged_cell_fraction = merged_cell_fraction.loc[~merged_cell_fraction.index.isin(outlier_samples.index),
-                                   :].copy()
-    # sns.set(font_scale=font_scale)
-    plt.figure(figsize=(10, 6))
-    # Draw a nested boxplot to show bills by day and time
-    # sns.set_color_codes('bright')
-    # sample_labels = list(purity['Cancer type'].unique())
-    current_cancer_type_frac = merged_cell_fraction.loc[:, [cell_type, 'cancer_type']]
-    if cell_type2max > 0:
-        current_cancer_type_frac.loc[current_cancer_type_frac[cell_type] > cell_type2max, cell_type] = cell_type2max
-    # mean cell fraction of each cancer type
-    mean_for_each_cancer_type = current_cancer_type_frac.groupby('cancer_type').mean().sort_values(by=cell_type)
-    cancer_type_order = mean_for_each_cancer_type.index.to_list()
-    # print(mean_for_each_cancer_type)
-    ax = sns.boxplot(x=x, y=cell_type, palette=sns.color_palette("muted"), whis=[0, 100],
-                     data=current_cancer_type_frac, showfliers=False, order=cancer_type_order)
-    # ax.tick_params(labelsize=11)
-    ax.set_xticklabels(ax.get_xticklabels(), rotation=25, ha='right')
-    # Add in points to show each observation, http://seaborn.pydata.org/examples/horizontal_boxplot.html
-    sns.stripplot(x=x, y=cell_type, data=current_cancer_type_frac,
-                  size=2, color=".4", linewidth=0, dodge=True, order=cancer_type_order, ax=ax)
-    ax.grid(True, axis='y')
-    # remove the top and right ticks
-    ax.tick_params(axis='x', which='both', top=False)
-    ax.tick_params(axis='y', which='both', right=False)
-    # sns.despine(offset=10, trim=True, left=True)
-
-    # handles, labels = ax.get_legend_handles_labels()
-    # n_half_label = int(len(labels)/2)
-    # plt.legend(handles[0:n_half_label], labels[0:n_half_label], bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
-    plt.xlabel(xlabel)
-    plt.ylabel(ylabel)
-    plt.tight_layout()
-    file_name = f'pred_{cell_type}_across_cancers.png'
-    plt.savefig(os.path.join(result_dir, file_name), dpi=200)
-    plt.close()
-
-
-def plot_pca(data: pd.DataFrame, result_fp=None, color_code=None, s=5, figsize=(8, 8),
-             color_code2label: dict = None, explained_variance_ratio: np.array = None, label_name='PC',
-             show_legend=True, show_xy_labels=True, anno=None, show_core_zone_of_tcga=False):
-    """
-    plot PCA result of simulated bulk cell dataset
-    :param data: PCA table, samples by PCs
-    :param result_fp:
-    :param color_code: a "np.array" to mark the label of each sample
-    :param color_code2label:
-    :param explained_variance_ratio: pca_model.explained_variance_ratio_
-    :param label_name: label name for x-axis
-    :param show_legend:
-    :param show_xy_labels:
-    :param anno: annotation for x-axis, which layer was used to generate the data
-    :param show_core_zone_of_tcga: whether to show the core zone of TCGA data
-    :return:
-    """
-    # sns.set_style('white')
-    # sns.set(font_scale=1.5)
-    if data.shape[1] >= 3:
-        pc_comb = [(0, 1), (1, 2), (0, 2)]
-    elif data.shape[1] == 2:
-        pc_comb = [(0, 1)]
-    else:
-        raise IndexError(f'data should have >= 2 columns, but {data.shape[1]} got')
-    if color_code is not None:
-        data['class'] = color_code
-    for pc1, pc2 in pc_comb:
-        # plt.figure(figsize=figsize)
-        if 'class' in data.columns:
-            col_x = f'{label_name}{pc1 + 1}'
-            col_y = f'{label_name}{pc2 + 1}'
-            g = sns.jointplot(x=col_x, y=col_y, data=data, kind='scatter', hue='class',
-                              s=s, space=0, height=figsize[1], alpha=0.5)
-            ax = g.ax_joint
-            n_tcga, n_non_tcga = 0, 0
-            q_lower, q_upper = 0.1, 0.9
-            if show_core_zone_of_tcga and 'TCGA' in data['class'].unique():
-                coord, n_tcga, n_non_tcga = get_core_zone_of_pca(pca_data=data, col_x=col_x, col_y=col_y,
-                                                                 q_lower=q_lower, q_upper=q_upper)
-                width = coord['x_upper'] - coord['x_lower']
-                height = coord['y_upper'] - coord['y_lower']
-                rect = patches.Rectangle((coord['x_lower'], coord['y_lower']), width, height,
-                                         fill=False, color='red', linewidth=1,
-                                         linestyle='dashed', label='Core Zone of TCGA')
-                ax.add_patch(rect)
-            if show_xy_labels:
-                x_label = col_x
-                y_label = col_y
-                if (explained_variance_ratio is not None) and (anno is not None):
-                    x_label = col_x + f' ({explained_variance_ratio[pc1] * 100:.1f}%, {anno})'
-                    y_label = col_y + f' ({explained_variance_ratio[pc2] * 100:.1f}%)'
-                elif explained_variance_ratio is not None:
-                    x_label = col_x + f' ({explained_variance_ratio[pc1] * 100:.1f}%)'
-                    y_label = col_y + f' ({explained_variance_ratio[pc2] * 100:.1f}%)'
-                elif anno is not None:
-                    x_label = col_x + f' ({anno})'
-                if show_core_zone_of_tcga:
-                    q_range = f'$q_{{{q_lower * 100:.0f}}}-q_{{{q_upper * 100:.0f}}}$'
-                    x_label += f'\nCore Zone ({q_range}): TCGA ({n_tcga}), Non-TCGA ({n_non_tcga})'
-                ax.set(xlabel=x_label, ylabel=y_label)
-            else:
-                ax.set(xlabel=None, ylabel=None)
-            # Put the legend out of the figure
-            if show_legend:
-                # g_legend = ax.legend(loc='lower center', bbox_to_anchor=(0.5, -0.2 - 0.1 * n_class), ncol=2)
-                g_legend = ax.legend(loc='best', ncol=2)
-                for _ in g_legend.legendHandles:
-                    _.set_linewidth(1)
-            else:
-                ax.legend([], [], frameon=False)
-            # remove the top and right ticks
-            g.ax_marg_x.tick_params(axis='x', which='both', top=False)
-            g.ax_marg_x.grid(False)
-            g.ax_marg_y.tick_params(axis='y', which='both', right=False)
-            g.ax_marg_y.grid(False)
-        else:
-            fig = plt.figure(figsize=figsize)
-            ax = fig.add_subplot(111)
-            for i in np.unique(color_code)[::-1]:
-                current_part = data.loc[color_code == i, :].copy()
-                if color_code2label is None:
-                    ax.scatter(current_part.iloc[:, pc1], current_part.iloc[:, pc2], label=i, alpha=.3)
-                else:
-                    ax.scatter(current_part.iloc[:, pc1], current_part.iloc[:, pc2],
-                               label=color_code2label[i], alpha=.3)
-
-            # plt.title(title, fontsize=18)
-            if explained_variance_ratio is None:
-                plt.xlabel(f'{label_name}{pc1 + 1}')
-                plt.ylabel(f'{label_name}{pc2 + 1}')
-            else:
-                plt.xlabel(f'{label_name}{pc1 + 1} ({(explained_variance_ratio[pc1] * 100): .1f}%)')
-                plt.ylabel(f'{label_name}{pc2 + 1} ({(explained_variance_ratio[pc2] * 100): .1f}%)')
-
-            plt.legend()
-            plt.tight_layout()
-        if result_fp is not None:
-            if '.png' in result_fp:
-                plt.savefig(result_fp.replace('.png', f'_{label_name}{pc1}_{label_name}{pc2}.png'),
-                            bbox_inches='tight', dpi=300)
-            if '.pdf' in result_fp:
-                plt.savefig(result_fp.replace('.pdf', f'_{label_name}{pc1}_{label_name}{pc2}.pdf'),
-                            bbox_inches='tight', dpi=300)
-
-
-def compare_mean_exp_with_cell_frac_across_algo(cancer_type: str, algo2merged_fp: dict, signature_score_fp: str,
-                                                cell_type: str, inx2plot: dict,
-                                                outliers_fp: str = None, cancer_type2max_frac=None,
-                                                result_file_name_prefix: str = '', result_dir='./figures'):
-    """
-    compare predicted cell fraction of each cell type with corresponding mean expression value of marker genes in TPM
-        one cancer type and one cell type, 2 x 3 plots, 6 different algorithms
-    :param cancer_type:
-    :param algo2merged_fp: file path of merged cell fractions for each algo
-    :param signature_score_fp: file path of mean expression of marker genes for each cell type (all cancer types)
-        samples by cell types
-    :param cell_type: current cell type (CD8 T/ CD4 T/ B Cells)
-    :param outliers_fp: outliers in each cancer type selected manually
-    :param inx2plot:
-    :param cancer_type2max_frac:
-    :param result_file_name_prefix:
-    :param result_dir:
-    :return:
-    """
-    check_dir(result_dir)
-    mean_exp = pd.read_csv(signature_score_fp, index_col=0)
-    if outliers_fp is not None and os.path.exists(outliers_fp):
-        outliers = pd.read_csv(outliers_fp, index_col=0)
-        mean_exp = mean_exp.loc[~mean_exp.index.isin(outliers.index), :].copy()
-    # mean_exp = mean_exp.loc[mean_exp['cancer_type'] == cancer_type, [f'{cell_type}_marker_mean']].copy()
-
-    corr_list = [None] * len(inx2plot)
-    max_cell_frac = 0
-    fig, ax = plt.subplots(2, 3, sharex='col', sharey='row', figsize=(3.5, 2.5), constrained_layout=True)
-    n_sample = 0
-    for i in range(2):
-        for j in range(3):
-            plot_target = inx2plot[(i, j)]
-            if plot_target:
-                algo, ref = plot_target.split('-')
-                merged_result = pd.read_csv(algo2merged_fp[algo], index_col=0)
-                if cell_type in merged_result.columns:
-                    merged_result = merged_result.loc[(merged_result['reference_dataset'] == ref) &
-                                                      (merged_result['cancer_type'] == cancer_type)].copy()
-                    merged_result.set_index('sample_id', inplace=True)
-                    if algo == 'EPIC' and 'otherCells' in merged_result.columns:
-                        merged_result['Cancer Cells'] = merged_result.loc[:, ['Cancer Cells', 'otherCells']].sum(axis=1)
-                    df = merged_result.merge(mean_exp, left_index=True, right_index=True)
-                    n_sample = df.shape[0]
-                    # print(df.shape, algo)
-                    col_name1 = f'{cell_type}_marker_mean'  # mean of marker gene expression values
-                    col_name2 = cell_type  # predicted cell fraction
-                    corr = np.corrcoef(df[col_name1], df[col_name2])
-                    if df[cell_type].max() > max_cell_frac:
-                        max_cell_frac = df[cell_type].max()
-
-                    if cancer_type2max_frac is not None:
-                        ax[i, j].set_ylim([-0.01, cancer_type2max_frac[cancer_type] + 0.02])
-                    else:
-                        if cell_type in ['CD8 T', 'CD4 T', 'B Cells']:
-                            _max_exp = 0.25
-                        else:
-                            _max_exp = 0.6
-                        ax[i, j].set_ylim([-0.01, _max_exp + 0.02])
-                        df.loc[df[cell_type] > _max_exp, cell_type] = _max_exp  # set max fraction to 0.25
-                    # mae = median_absolute_error(y_true=df[col_name1], y_pred=df[col_name2])
-                    ax[i, j].scatter(df[col_name1], df[col_name2], s=1, alpha=0.8)
-                    # x_left, x_right = ax[i, j].get_xlim()
-                    y_bottom, y_top = ax[i, j].get_ylim()
-                    if 'CIBERSORT' in algo:
-                        algo = 'C.SORT'
-                    elif 'Scaden' in algo:
-                        algo = 'Scaden'
-                    elif 'EPIC' in algo:
-                        algo = 'EPIC'
-                    if 'simu_bulk' in ref:
-                        ref = 'simu_2ds'
-                    ax[i, j].set_xlabel('{} - {}'.format(algo, ref.replace('_ref', '')), fontsize=8)
-                    ax[i, j].text(1, y_top * 0.8, 'corr = {:.2f}'.format(corr[0, 1]), fontsize=6)
-                    corr_list[i * 3 + j] = round(corr[0, 1], 3)
-    fig.supylabel('Predicted cell fraction of {}'.format(f'{cell_type}'))
-    fig.supxlabel('mean expression of marker genes in {} (n={})'.format(cancer_type, n_sample))
-    # plt.tight_layout()
-    plt.savefig(os.path.join(result_dir, f'{result_file_name_prefix}_in_{cancer_type}.png'), dpi=300)
-    print('  Max cell fraction: {}'.format(max_cell_frac))
-    return {'corr': corr_list}
-
-
-def compare_y_y_pred_plot_cpe(y_true: pd.Series, y_pred: pd.Series, inx=tuple(), cancer_type='',
-                              show_metrics: bool = False, ax=None):
-    """
-    Plot y against y_pred to visualize the performance of prediction result
-
-    :param y_true: CPE
-
-    :param y_pred: this file contains the predicted value of y
-
-    :param inx: a tuple of two elements, the first element is the index of y_true, the second element is the index of y_pred
-
-    :param cancer_type: cancer type
-
-    :param show_metrics: show correlation and RMSE
-
-    :param ax: matplotlib axis
-
-    :return: None
-    """
-    # Use the pyplot interface to change just one subplot...
-    plt.sca(ax)
-
-    plt.scatter(y_pred, y_true, s=1, alpha=0.75, rasterized=True)
-    plt.xlim([-0.05, 1.05])
-    plt.ylim([-0.05, 1.05])
-    plt.xticks([0, 1])
-    plt.yticks([0, 0.5, 1])
-    x_left, x_right = plt.xlim()
-    y_bottom, y_top = plt.ylim()
-    x_max = x_right
-    y_max = y_top
-    plt.plot([0, max(x_max, y_max)], [0, max(x_max, y_max)], linestyle='--', color='tab:gray')
-    corr = 0
-    rmse = 0
-    ccc = 0
-    if show_metrics:  # show metrics in test set
-        corr = get_corr(y_pred, y_true)
-        rmse = calculate_rmse(y_true=pd.DataFrame(y_true), y_pred=pd.DataFrame(y_pred))
-        ccc = get_ccc(y_pred.values, y_true.values)
-        plt.text(0.3 * x_max, 0.2 * y_max, 'corr = {:.2f}'.format(corr), fontsize=6)
-        plt.text(0.3 * x_max, 0.1 * y_max, 'RMSE = {:.2f}'.format(rmse), fontsize=6)
-        plt.text(0.3 * x_max, 0.0 * y_max, 'CCC = {:.2f}'.format(ccc), fontsize=6)
-    if inx:
-        plt.ylabel(f'{cancer_type} ({y_true.shape[0]})', fontsize=6)
-    # if inx and inx[0] == 8:
-    #     plt.xlabel(f'{algo}', fontsize=6)
-    # plt.legend()
-    return corr, rmse, ccc
-
-
-def plot_pred_cell_prop_with_cpe(cpe_file_path, pred_cell_prop_file_path, result_dir, save_metrics: bool = True):
-    all_cancer_types = sorted([i for i in cancer_types if i != 'PAAD'])
-    fig, axes = plt.subplots(6, 3, sharex='all', sharey='all', figsize=(5, 6))
-    pred_cell_prop = pd.read_csv(pred_cell_prop_file_path, index_col=0)
-    cpe = read_cancer_purity(cpe_file_path, sample_names=pred_cell_prop.index)
-    pred_cell_prop = pred_cell_prop.merge(cpe['CPE'], left_index=True, right_index=True)
-    metrics_value = {}
-    for j in range(3):
-        for i in range(6):
-            current_cancer_type = all_cancer_types[i + j * 6]
-            current_data = pred_cell_prop.loc[pred_cell_prop['cancer_type'] == current_cancer_type, :]
-            corr, rmse, ccc = compare_y_y_pred_plot_cpe(y_pred=current_data['Cancer Cells'], y_true=current_data['CPE'],
-                                                        show_metrics=True, ax=axes[i, j], cancer_type=current_cancer_type,
-                                                        inx=(i, j))
-            metrics_value[current_cancer_type] = {'corr': corr, 'rmse': rmse, 'ccc': ccc}
-
-    # add a big axis, hide frame
-    fig.add_subplot(111, frameon=False)
-    # hide tick and tick label of the big axis
-    plt.tick_params(labelcolor='none', which='both', top=False, bottom=False, left=False, right=False)
-    plt.xlabel('Predicted cancer cell proportions by DeSide', labelpad=5)
-    plt.ylabel("CPE", labelpad=15)
-
-    plt.tight_layout(h_pad=0.02, w_pad=0.15)
-    plt.savefig(os.path.join(result_dir, 'pred_cancer_cell_prop_vs_cpe-deside.png'), dpi=300)
-    if save_metrics:
-        metrics_value_df = pd.DataFrame.from_dict(metrics_value, orient='index')
-        metrics_value_df.to_csv(os.path.join(result_dir, 'pred_cancer_cell_prop_vs_cpe-deside-metrics.csv'))
+import os
+import pandas as pd
+import numpy as np
+from typing import Union
+import statsmodels.api as sm
+from sklearn.metrics import median_absolute_error
+from ..utility import (print_df, cal_relative_error, calculate_rmse, check_dir, get_corr,
+                       read_xy, read_df, get_inx2cell_type, log2_transform, get_core_zone_of_pca,
+                       get_ccc, read_cancer_purity, cancer_types)
+# from ..utility.read_file import ReadExp
+from .plot_nn import plot_corr_two_columns
+import matplotlib.patches as patches
+# import importlib
+import matplotlib.pyplot as plt
+import seaborn as sns
+import gc
+
+# set_fig_style()
+# sns.set(font_scale=1.5)
+# sns.set_style('white')
+
+
+class ScatterPlot(object):
+    def __init__(self, x: Union[str, pd.DataFrame], y: Union[str, pd.DataFrame],
+                 postfix: str = None, group_info: pd.DataFrame = None):
+        """
+        :param x:
+        :param y:
+        :param postfix: only for naming
+        """
+        self.x = read_xy(x)
+        self.y = read_xy(y)
+        common_inx = [i for i in self.x.index if i in self.y.index]
+        self.postfix = postfix
+        self.group_info = group_info
+        if group_info is not None:
+            common_inx = [i for i in group_info.index if i in common_inx]
+            self.group_info = self.group_info.loc[common_inx, :].copy()
+        self.show_columns = None
+        self.x = self.x.loc[common_inx, :].copy()
+        self.y = self.y.loc[common_inx, :].copy()
+        assert np.all(self.x.index == self.y.index)
+
+    def plot(self, show_columns: Union[list, dict], result_file_dir: str = None,
+             x_label: str = None, y_label: str = None, show_corr: bool = True, show_rmse: bool = False,
+             show_diag: bool = True, show_mae: bool = False, pred_by: str = None,
+             fig_size=(8, 8), group_by: str = None, show_reg_line: bool = False, s=6, order=1,
+             legend_loc: str = 'best'):
+        """
+        :param show_columns: a list of column names in both x and y, could be multiple common columns
+            or a dict {'x': '', 'y': ''}, only one column allowed
+        :param result_file_dir:
+        :param x_label:
+        :param y_label:
+        :param show_corr:
+        :param show_rmse:
+        :param show_mae: media absolute error
+        :param show_diag:
+        :param pred_by: algorithm name, will be showed in ylabel
+        :param fig_size:
+        :param group_by: one of the column name in self.group_info
+        :param show_reg_line: fit regression model
+        :param s:
+        :param legend_loc:
+        :param order: 1 for linear regression; 2 for Polynomial Regressions, y = alpha + beta1*x + beta2*x^2
+        """
+        plt.figure(figsize=fig_size)
+        ax = plt.axes()
+        # f, ax = plt.subplots(figsize=fig_size)
+
+        all_x = []
+        all_y = []
+        self.show_columns = show_columns
+        if type(show_columns) == dict:
+            self.x = self.x[show_columns['x']]
+            self.y = self.y[show_columns['y']]
+            all_x.append(self.x)
+            all_y.append(self.y)
+            if (self.group_info is not None) and (group_by in self.group_info.columns):
+                inx = self.group_info[group_by] == 1
+                plt.scatter(self.x[~inx], self.y[~inx], s=1, label='others')
+                plt.scatter(self.x[inx], self.y[inx], s=5, label=group_by, marker='x')
+            else:
+                plt.scatter(self.x, self.y, s=s, label=show_columns['x'], alpha=.4)  # only 1 vs 1 column
+            if show_reg_line:
+                self.fit_reg_model(ax=ax, order=order)
+        else:
+            show_columns = [i for i in show_columns if i in self.y.columns]
+            # for cell_type in show_columns:
+            #     if cell_type not in y_true.columns:
+            #         y_true[cell_type] = 0
+            show_columns_str = ', '.join(show_columns)
+            assert np.all([i in self.x.columns for i in show_columns]), \
+                f'All of elements in show_columns ({show_columns_str}) should exist in ' \
+                f'the columns of both x ({self.x.columns}) and y ({self.y.columns})'
+
+            # y_true = self.x.loc[:, show_columns]
+            # y_pred = self.y.loc[:, show_columns]
+            # sns.set(font_scale=font_scale)
+            # plt.figure(figsize=(8, 6))
+            for i, col in enumerate(show_columns):
+                _x = self.x.loc[:, col]
+                _y = self.y.loc[:, col]
+                all_x.append(_x)
+                all_y.append(_y)
+                plt.scatter(_x, _y, label=col, s=6, alpha=1 - 0.05 * i)
+        x_left, x_right = plt.xlim()
+        y_bottom, y_top = plt.ylim()
+        all_x = np.concatenate(all_x)
+        all_y = np.concatenate(all_y)
+        if show_diag:
+            _ = max(x_right, y_top)
+            plt.plot([0, _], [0, _], linestyle='--', color='tab:gray', linewidth=1, alpha=0.8)
+        if show_corr:  # show metrics in test set
+            corr = get_corr(all_x, all_y)
+            plt.text(x_right * 0.60, y_top * 0.10, 'corr = {:.2f}'.format(corr))
+        if show_mae:
+            mae = median_absolute_error(y_true=all_x, y_pred=all_y)
+            plt.text(x_right * 0.60, y_top * 0.07, 'MAE = {:.2f}'.format(mae))
+        if show_rmse and (not show_mae):
+            rmse = calculate_rmse(y_true=pd.DataFrame(all_x), y_pred=pd.DataFrame(all_y))
+            plt.text(x_right * 0.60, y_top * 0.07, 'RMSE = {:.2f}'.format(rmse))
+        if show_rmse and show_mae:
+            rmse = calculate_rmse(y_true=pd.DataFrame(all_x), y_pred=pd.DataFrame(all_y))
+            plt.text(x_right * 0.60, y_top * 0.04, 'RMSE = {:.2f}'.format(rmse))
+        if x_label:
+            plt.xlabel(x_label)
+        else:
+            plt.xlabel('y_true')
+        if y_label:
+            plt.ylabel(y_label)
+        elif pred_by:
+            plt.ylabel('Pred by {} (n={})'.format(pred_by, self.y.shape[0]))
+        else:
+            plt.ylabel('y_pred')
+        handles, labels = plt.gca().get_legend_handles_labels()
+        if len(labels) > 1:
+            plt.legend(handles[1:], labels[1:], loc=legend_loc)
+        plt.tight_layout()
+        if result_file_dir:
+            plt.savefig(os.path.join(result_file_dir,
+                                     'x_vs_y_{}.png'.format(self.postfix)), dpi=300)
+            # plt.savefig(os.path.join(result_file_dir,
+            #                          'x_vs_y_{}.svg'.format(self.postfix)), dpi=300)
+        plt.close()
+
+    def fit_reg_model(self, ax, alpha_ci=0.05, order=1):
+        """
+        only used 1vs1 comparing, show_columns should be a dict
+        :param ax
+        :param alpha_ci: 1 - alpha_ci confidence interval
+        :param order: 1 for linear regression; 2 for Polynomial Regressions, y = alpha + beta1*x + beta2*x^2
+        """
+
+        if type(self.x) == pd.Series:
+            self.x = self.x.to_frame()
+        self.x['intercept'] = 1  # add 1 as intercept column to fit `intercept`
+        x_col = self.show_columns['x']  # column name, a str
+        x_col_square = f'{x_col}^2'
+        if order == 2:
+            self.x[x_col_square] = self.x[x_col] ** 2
+            mod = sm.OLS(self.y, self.x.loc[:, ['intercept', x_col, x_col_square]])
+        else:  # order == 1
+            mod = sm.OLS(self.y, self.x.loc[:, ['intercept', x_col]])
+        res = mod.fit()
+        # print(res.summary())
+        ci = res.conf_int(alpha_ci)  # 95%, +/- 2*SD
+        x_lin = np.linspace(self.x[x_col].min(), self.x[x_col].max(), 20)
+        beta1 = res.params[x_col]
+        alpha = res.params['intercept']
+        beta2 = 0
+        if order == 2:
+            beta2 = res.params[x_col_square]
+        y_reg_line = x_lin * beta1 + alpha + np.power(x_lin, 2) * beta2
+        if order == 2:
+            y_lower_bound = x_lin * ci.loc[x_col, 0] + ci.loc['intercept', 0] + \
+                np.power(x_lin, 2) * ci.loc[x_col_square, 0]
+            y_upper_bound = x_lin * ci.loc[x_col, 1] + ci.loc['intercept', 1] + \
+                np.power(x_lin, 2) * ci.loc[x_col_square, 1]
+        else:
+            y_lower_bound = x_lin * ci.loc[x_col, 0] + ci.loc['intercept', 0]
+            y_upper_bound = x_lin * ci.loc[x_col, 1] + ci.loc['intercept', 1]
+        xy = self.x.copy()
+        xy['y_pred'] = self.x[x_col]
+        xy['y_true'] = self.y
+        sns.regplot(x='y_pred', y='y_true', data=xy, ax=ax, order=order,
+                    x_estimator=np.mean,
+                    scatter_kws={"s": 5}, color='tab:grey', x_bins=50,
+                    line_kws={'color': 'tab:orange', 'lw': 1, 'alpha': 0})
+        # p_value = res.pvalues[x_col]
+        # r2 = res.rsquared
+        # print(f'p_value: {p_value}', f'R^2: {r2}')
+        if alpha > 0:
+            if order == 2:
+                plt.plot(x_lin, y_reg_line, c='tab:orange',
+                         label=f'$y= {beta2: .2f}x^2 + {beta1: .2f}x + {alpha: .2f}$', linewidth=1)
+            else:
+                plt.plot(x_lin, y_reg_line, c='tab:orange',
+                         label=f'$y={beta1: .2f}x + {alpha: .2f}$', linewidth=1)
+        else:
+            if order == 2:
+                plt.plot(x_lin, y_reg_line, c='tab:orange',
+                         label=f'$y= {beta2: .2f}x^2 + {beta1: .2f}x - {abs(alpha): .2f}$', linewidth=1)
+            else:
+                plt.plot(x_lin, y_reg_line, c='tab:orange',
+                         label=f'$y={beta1: .2f}x - {abs(alpha): .2f}$', linewidth=1)
+        plt.plot(x_lin, y_lower_bound, c='tab:brown', label=f'{100 - alpha_ci * 100}% CI', linewidth=1)
+        plt.plot(x_lin, y_upper_bound, c='tab:brown', linewidth=1)
+
+
+def compare_y_y_pred_plot(y_true: Union[str, pd.DataFrame], y_pred: Union[str, pd.DataFrame],
+                          show_columns: list = None, result_file_dir=None, annotation: dict = None,
+                          y_label=None, x_label=None, model_name='average',
+                          show_metrics: bool = False, figsize: tuple = (8, 8)):
+    """
+    Plot y against y_pred to visualize the performance of prediction result
+
+    :param y_true: this file contains the ground truth of cell fractions when it was simulated
+
+    :param y_pred: this file contains the predicted value of y
+
+    :param show_columns: this list contains the name of columns that want to plot in figure
+
+    :param result_file_dir: where to save results
+
+    :param annotation: annotations that need to show in figure, {anno_name: {col1: value1, col2: value2, ...}, ...}
+
+    :param y_label: y label
+
+    :param x_label: x label
+
+    :param model_name: only for naming files
+
+    :param show_metrics: show correlation and RMSE
+
+    :param figsize: figure size
+
+    :return: None
+    """
+    if show_columns is None:
+        show_columns = []
+    if annotation is None:
+        annotation = {}
+    y_true = read_xy(a=y_true, xy='cell_frac')
+    y_pred = read_xy(a=y_pred, xy='cell_frac')
+    if '1-others' in show_columns:
+        if 'Cancer Cells' in y_true.columns:
+            y_true['1-others'] = y_true['Cancer Cells']
+        else:
+            y_true['1-others'] = 0
+    if ('T Cells' in y_pred.columns) and ('T Cells' not in y_true.columns):
+        y_true['T Cells'] = y_true.loc[:, ['CD4 T', 'CD8 T']].sum(axis=1)
+    # less cell type than show_columns for this dataset
+    show_columns = [i for i in show_columns if i in y_true.columns]
+    # for cell_type in show_columns:
+    #     if cell_type not in y_true.columns:
+    #         y_true[cell_type] = 0
+    show_columns_str = ', '.join(show_columns)
+    assert np.all([i in y_true.columns for i in show_columns]) and \
+           np.all([i in y_pred.columns for i in show_columns]), \
+           f'All of elements in show_columns ({show_columns_str}) should exist in ' \
+           f'the columns of both y_true ({y_true.columns}) and y_pred ({y_pred.columns})'
+    common_inx = [i for i in y_true.index if i in y_pred.index]
+
+    y_true = y_true.loc[common_inx, show_columns]
+    y_pred = y_pred.loc[common_inx, show_columns]
+    # sns.set(font_scale=font_scale)
+    plt.figure(figsize=figsize)
+    all_x = []
+    all_y = []
+    for i, col in enumerate(show_columns):
+        _x = y_true.loc[:, col]
+        _y = y_pred.loc[:, col]
+        all_x.append(_x)
+        all_y.append(_y)
+        plt.scatter(_x, _y, label=col, s=6, alpha=1 - 0.05 * i)
+        if annotation:
+            x_left, x_right = plt.xlim()
+            y_bottom, y_top = plt.ylim()
+            for k, v in annotation.items():
+                plt.text(x_left * 1.5, y_top * 0.8, 'k ({.4f})'.format(v[col]))
+    x_left, x_right = plt.xlim()
+    y_bottom, y_top = plt.ylim()
+    x_max = x_right + x_right * 0.01
+    y_max = y_top + y_top * 0.01
+    plt.plot([0, max(x_max, y_max)], [0, max(x_max, y_max)], linestyle='--', color='tab:gray')
+    if show_metrics:  # show metrics in test set
+        all_x = np.concatenate(all_x)
+        all_y = np.concatenate(all_y)
+        corr = get_corr(all_x, all_y)
+        rmse = calculate_rmse(y_true=pd.DataFrame(all_x), y_pred=pd.DataFrame(all_y))
+        plt.text(0.70 * x_max, 0.16 * y_max, 'corr = {:.3f}'.format(corr))
+        plt.text(0.70 * x_max, 0.10 * y_max, 'RMSE = {:.3f}'.format(rmse))
+    if x_label:
+        plt.xlabel(x_label)
+    else:
+        plt.xlabel('y_true')
+    if y_label:
+        plt.ylabel(y_label)
+    else:
+        plt.ylabel('y_predicted')
+    plt.legend()
+    plt.tight_layout()
+    if result_file_dir:
+        plt.savefig(os.path.join(result_file_dir, 'y_true_vs_y_pred_{}.png'.format(model_name)), dpi=200)
+    plt.close()
+
+
+def compare_exp_and_cell_fraction(merged_file_path, result_dir,
+                                  cell_types: list, clustering_ct: list = None,
+                                  outlier_file_path=None, predicted_by='DeSide', font_scale=1.5,
+                                  signature_score_method: str = 'mean_exp', update_figures=False):
+    """
+    Comparing the mean expression value (or gene signature score) of marker genes for each cell type
+      and the predicted cell fraction
+    :param merged_file_path: the file path of merged mean expression value of marker genes and predicted cell fractions,
+         sample by cell type, should contain `cancer_type` column to mark corresponding dataset
+    :param result_dir: where to save results
+    :param cell_types: all cell types used by DeSide
+    :param clustering_ct: cell types used for clustering of cancer types
+    :param outlier_file_path: the file path of outlier samples selected manually
+    :param predicted_by: the name of prediction algorithm, DeSide or Scaden
+    :param font_scale: font scaling
+    :param signature_score_method:
+    :param update_figures: if update figures
+    :return:
+    """
+    check_dir(result_dir)
+    # result_dir_scaled = result_dir + '_scaled'
+    # check_dir(result_dir_scaled)
+    cancer_type2corr_file_path = os.path.join(result_dir, 'cancer_type2corr.csv')
+    # print(merged_file_path)
+    merged_df = read_df(merged_file_path)
+    # merged_df = pd.read_csv(merged_file_path, index_col=0)
+    cancer_types = list(merged_df['cancer_type'].unique())
+    if 'T Cells' in cell_types and 'T Cells' not in merged_df.columns:
+        merged_df['T Cells'] = merged_df.loc[:, ['CD4 T', 'CD8 T']].sum(axis=1)
+    if (not os.path.exists(cancer_type2corr_file_path)) or update_figures:
+        if outlier_file_path is not None:
+            outlier_samples = pd.read_csv(outlier_file_path, index_col=0)
+            if outlier_samples.shape[0] > 0:  # remove outliers
+                print(f'   {outlier_samples.shape[0]} outlier samples will be removed...')
+                merged_df = merged_df.loc[~merged_df.index.isin(outlier_samples.index), :].copy()
+        cancer_type2corr = {}
+        for cancer_type in cancer_types:
+            print('----------------------------------------------------')
+            print(f'   Deal with cancer type: {cancer_type}...')
+            current_df = merged_df.loc[merged_df['cancer_type'] == cancer_type, :]
+            # print(current_df)
+            # plot predicted cell fraction against corresponding mean expression value of marker genes
+            current_result_dir = os.path.join(result_dir, cancer_type)
+            # current_result_dir_scaled = os.path.join(result_dir_scaled, cancer_type)
+            if cancer_type not in cancer_type2corr:
+                cancer_type2corr[cancer_type] = {}
+            for cell_type in cell_types:
+                # if cell_type != 'Cancer Cells':
+                if signature_score_method == 'mean_exp':
+                    method = 'marker_mean'
+                    if cell_type in ['B Cells'] and np.any(['max' in i for i in current_df.columns]):
+                        method = 'marker_max'
+                else:
+                    method = signature_score_method
+                col_name1 = cell_type + f'_{method}'
+                col_name2 = cell_type
+                cancer_type2corr[cancer_type][cell_type] = get_corr(current_df[col_name1], current_df[col_name2])
+                plot_corr_two_columns(df=current_df, col_name1=col_name1, col_name2=col_name2,
+                                      predicted_by=predicted_by, font_scale=font_scale, scale_exp=False,
+                                      output_dir=current_result_dir, diagonal=False, cancer_type=cancer_type,
+                                      update_figures=update_figures)
+
+            gc.collect()
+        cancer_type2corr_df = pd.DataFrame.from_dict(cancer_type2corr, orient='index')
+        cancer_type2corr_df.fillna(0, inplace=True)
+        cancer_type2corr_df.to_csv(cancer_type2corr_file_path, float_format='%.3f')
+    else:
+        print(f'   Using previous cancer_type2cor file from: {cancer_type2corr_file_path}.')
+        cancer_type2corr_df = pd.read_csv(cancer_type2corr_file_path, index_col=0)
+    # sns.set(font_scale=1.5)
+    if clustering_ct is not None:
+        c_ct = {'clustering_ct': clustering_ct}
+        other_ct = [ct for ct in cell_types if ct not in (clustering_ct + ['Cancer Cells'])]
+        if len(other_ct) >= 2:
+            c_ct = {'clustering_ct': clustering_ct, 'other_ct': other_ct}
+        for k, v in c_ct.items():
+            plot_clustermap(data=cancer_type2corr_df, columns=v,
+                            result_file_path=os.path.join(result_dir, f'cancer_type2corr_{k}.png'))
+
+
+def plot_clustermap(data: pd.DataFrame, columns: list, result_file_path: str):
+    """
+    plot cluster map for correlation table or cell fraction table
+    """
+    # sns.set(font_scale=1.5)
+    g = sns.clustermap(data.loc[:, columns], cmap="vlag")
+    plt.setp(g.ax_heatmap.xaxis.get_majorticklabels(), rotation=40)
+    plt.tight_layout()
+    plt.savefig(result_file_path, dpi=200)
+    # plt.show()
+    plt.close('all')
+
+
+def compare_cell_fraction_across_cancer_type(merged_cell_fraction: pd.DataFrame, result_dir='.', cell_type: str = '',
+                                             xlabel: str = 'Cancer Type',
+                                             ylabel: str = 'Tumor purity in each sample (CPE)',
+                                             outlier_file_path: str = None, cell_type2max: float = 0.0):
+    """
+    Specific plotting for file cancer_purity.csv, downloaded from Aran, D., Sirota, M. & Butte,
+    A. Systematic pan-cancer analysis of tumour purity. Nat Commun 6, 8971 (2015). https://doi.org/10.1038/ncomms9971
+
+    And other predicted cell fractions across all cancer types can be plotted.
+
+    :param merged_cell_fraction: merged cell fraction predicted by DeSide
+
+    :param cell_type: current cell type to plot
+
+    :param result_dir: where to save result
+
+    :param xlabel: x label
+
+    :param ylabel: y label
+
+    :param outlier_file_path:
+
+    :param cell_type2max: max cell fraction to keep when plotting
+
+    :return: None
+    """
+    x = 'cancer_type'
+    check_dir(result_dir)
+
+    if outlier_file_path is not None:
+        outlier_samples = pd.read_csv(outlier_file_path, index_col=0)
+        if outlier_samples.shape[0] > 0:  # remove outliers
+            print(f'   {outlier_samples.shape[0]} outlier samples will be removed...')
+            merged_cell_fraction = merged_cell_fraction.loc[~merged_cell_fraction.index.isin(outlier_samples.index),
+                                   :].copy()
+    # sns.set(font_scale=font_scale)
+    plt.figure(figsize=(10, 6))
+    # Draw a nested boxplot to show bills by day and time
+    # sns.set_color_codes('bright')
+    # sample_labels = list(purity['Cancer type'].unique())
+    current_cancer_type_frac = merged_cell_fraction.loc[:, [cell_type, 'cancer_type']]
+    if cell_type2max > 0:
+        current_cancer_type_frac.loc[current_cancer_type_frac[cell_type] > cell_type2max, cell_type] = cell_type2max
+    # mean cell fraction of each cancer type
+    mean_for_each_cancer_type = current_cancer_type_frac.groupby('cancer_type').mean().sort_values(by=cell_type)
+    cancer_type_order = mean_for_each_cancer_type.index.to_list()
+    # print(mean_for_each_cancer_type)
+    ax = sns.boxplot(x=x, y=cell_type, palette=sns.color_palette("muted"), whis=[0, 100],
+                     data=current_cancer_type_frac, showfliers=False, order=cancer_type_order)
+    # ax.tick_params(labelsize=11)
+    ax.set_xticklabels(ax.get_xticklabels(), rotation=25, ha='right')
+    # Add in points to show each observation, http://seaborn.pydata.org/examples/horizontal_boxplot.html
+    sns.stripplot(x=x, y=cell_type, data=current_cancer_type_frac,
+                  size=2, color=".4", linewidth=0, dodge=True, order=cancer_type_order, ax=ax)
+    ax.grid(True, axis='y')
+    # remove the top and right ticks
+    ax.tick_params(axis='x', which='both', top=False)
+    ax.tick_params(axis='y', which='both', right=False)
+    # sns.despine(offset=10, trim=True, left=True)
+
+    # handles, labels = ax.get_legend_handles_labels()
+    # n_half_label = int(len(labels)/2)
+    # plt.legend(handles[0:n_half_label], labels[0:n_half_label], bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
+    plt.xlabel(xlabel)
+    plt.ylabel(ylabel)
+    plt.tight_layout()
+    file_name = f'pred_{cell_type}_across_cancers.png'
+    plt.savefig(os.path.join(result_dir, file_name), dpi=200)
+    plt.close()
+
+
+def plot_pca(data: pd.DataFrame, result_fp=None, color_code=None, s=5, figsize=(8, 8),
+             color_code2label: dict = None, explained_variance_ratio: np.array = None, label_name='PC',
+             show_legend=True, show_xy_labels=True, anno=None, show_core_zone_of_tcga=False):
+    """
+    plot PCA result of simulated bulk cell dataset
+    :param data: PCA table, samples by PCs
+    :param result_fp:
+    :param color_code: a "np.array" to mark the label of each sample
+    :param color_code2label:
+    :param explained_variance_ratio: pca_model.explained_variance_ratio_
+    :param label_name: label name for x-axis
+    :param show_legend:
+    :param show_xy_labels:
+    :param anno: annotation for x-axis, which layer was used to generate the data
+    :param show_core_zone_of_tcga: whether to show the core zone of TCGA data
+    :return:
+    """
+    # sns.set_style('white')
+    # sns.set(font_scale=1.5)
+    if data.shape[1] >= 3:
+        pc_comb = [(0, 1), (1, 2), (0, 2)]
+    elif data.shape[1] == 2:
+        pc_comb = [(0, 1)]
+    else:
+        raise IndexError(f'data should have >= 2 columns, but {data.shape[1]} got')
+    if color_code is not None:
+        data['class'] = color_code
+    for pc1, pc2 in pc_comb:
+        # plt.figure(figsize=figsize)
+        if 'class' in data.columns:
+            col_x = f'{label_name}{pc1 + 1}'
+            col_y = f'{label_name}{pc2 + 1}'
+            g = sns.jointplot(x=col_x, y=col_y, data=data, kind='scatter', hue='class',
+                              s=s, space=0, height=figsize[1], alpha=0.5)
+            ax = g.ax_joint
+            n_tcga, n_non_tcga = 0, 0
+            q_lower, q_upper = 0.1, 0.9
+            if show_core_zone_of_tcga and 'TCGA' in data['class'].unique():
+                coord, n_tcga, n_non_tcga = get_core_zone_of_pca(pca_data=data, col_x=col_x, col_y=col_y,
+                                                                 q_lower=q_lower, q_upper=q_upper)
+                width = coord['x_upper'] - coord['x_lower']
+                height = coord['y_upper'] - coord['y_lower']
+                rect = patches.Rectangle((coord['x_lower'], coord['y_lower']), width, height,
+                                         fill=False, color='red', linewidth=1,
+                                         linestyle='dashed', label='Core Zone of TCGA')
+                ax.add_patch(rect)
+            if show_xy_labels:
+                x_label = col_x
+                y_label = col_y
+                if (explained_variance_ratio is not None) and (anno is not None):
+                    x_label = col_x + f' ({explained_variance_ratio[pc1] * 100:.1f}%, {anno})'
+                    y_label = col_y + f' ({explained_variance_ratio[pc2] * 100:.1f}%)'
+                elif explained_variance_ratio is not None:
+                    x_label = col_x + f' ({explained_variance_ratio[pc1] * 100:.1f}%)'
+                    y_label = col_y + f' ({explained_variance_ratio[pc2] * 100:.1f}%)'
+                elif anno is not None:
+                    x_label = col_x + f' ({anno})'
+                if show_core_zone_of_tcga:
+                    q_range = f'$q_{{{q_lower * 100:.0f}}}-q_{{{q_upper * 100:.0f}}}$'
+                    x_label += f'\nCore Zone ({q_range}): TCGA ({n_tcga}), Non-TCGA ({n_non_tcga})'
+                ax.set(xlabel=x_label, ylabel=y_label)
+            else:
+                ax.set(xlabel=None, ylabel=None)
+            # Put the legend out of the figure
+            if show_legend:
+                # g_legend = ax.legend(loc='lower center', bbox_to_anchor=(0.5, -0.2 - 0.1 * n_class), ncol=2)
+                g_legend = ax.legend(loc='best', ncol=2)
+                for _ in g_legend.legendHandles:
+                    _.set_linewidth(1)
+            else:
+                ax.legend([], [], frameon=False)
+            # remove the top and right ticks
+            g.ax_marg_x.tick_params(axis='x', which='both', top=False)
+            g.ax_marg_x.grid(False)
+            g.ax_marg_y.tick_params(axis='y', which='both', right=False)
+            g.ax_marg_y.grid(False)
+        else:
+            fig = plt.figure(figsize=figsize)
+            ax = fig.add_subplot(111)
+            for i in np.unique(color_code)[::-1]:
+                current_part = data.loc[color_code == i, :].copy()
+                if color_code2label is None:
+                    ax.scatter(current_part.iloc[:, pc1], current_part.iloc[:, pc2], label=i, alpha=.3)
+                else:
+                    ax.scatter(current_part.iloc[:, pc1], current_part.iloc[:, pc2],
+                               label=color_code2label[i], alpha=.3)
+
+            # plt.title(title, fontsize=18)
+            if explained_variance_ratio is None:
+                plt.xlabel(f'{label_name}{pc1 + 1}')
+                plt.ylabel(f'{label_name}{pc2 + 1}')
+            else:
+                plt.xlabel(f'{label_name}{pc1 + 1} ({(explained_variance_ratio[pc1] * 100): .1f}%)')
+                plt.ylabel(f'{label_name}{pc2 + 1} ({(explained_variance_ratio[pc2] * 100): .1f}%)')
+
+            plt.legend()
+            plt.tight_layout()
+        if result_fp is not None:
+            if '.png' in result_fp:
+                plt.savefig(result_fp.replace('.png', f'_{label_name}{pc1}_{label_name}{pc2}.png'),
+                            bbox_inches='tight', dpi=300)
+            if '.pdf' in result_fp:
+                plt.savefig(result_fp.replace('.pdf', f'_{label_name}{pc1}_{label_name}{pc2}.pdf'),
+                            bbox_inches='tight', dpi=300)
+
+
+def compare_mean_exp_with_cell_frac_across_algo(cancer_type: str, algo2merged_fp: dict, signature_score_fp: str,
+                                                cell_type: str, inx2plot: dict,
+                                                outliers_fp: str = None, cancer_type2max_frac=None,
+                                                result_file_name_prefix: str = '', result_dir='./figures'):
+    """
+    compare predicted cell fraction of each cell type with corresponding mean expression value of marker genes in TPM
+        one cancer type and one cell type, 2 x 3 plots, 6 different algorithms
+    :param cancer_type:
+    :param algo2merged_fp: file path of merged cell fractions for each algo
+    :param signature_score_fp: file path of mean expression of marker genes for each cell type (all cancer types)
+        samples by cell types
+    :param cell_type: current cell type (CD8 T/ CD4 T/ B Cells)
+    :param outliers_fp: outliers in each cancer type selected manually
+    :param inx2plot:
+    :param cancer_type2max_frac:
+    :param result_file_name_prefix:
+    :param result_dir:
+    :return:
+    """
+    check_dir(result_dir)
+    mean_exp = pd.read_csv(signature_score_fp, index_col=0)
+    if outliers_fp is not None and os.path.exists(outliers_fp):
+        outliers = pd.read_csv(outliers_fp, index_col=0)
+        mean_exp = mean_exp.loc[~mean_exp.index.isin(outliers.index), :].copy()
+    # mean_exp = mean_exp.loc[mean_exp['cancer_type'] == cancer_type, [f'{cell_type}_marker_mean']].copy()
+
+    corr_list = [None] * len(inx2plot)
+    max_cell_frac = 0
+    fig, ax = plt.subplots(2, 3, sharex='col', sharey='row', figsize=(3.5, 2.5), constrained_layout=True)
+    n_sample = 0
+    for i in range(2):
+        for j in range(3):
+            plot_target = inx2plot[(i, j)]
+            if plot_target:
+                algo, ref = plot_target.split('-')
+                merged_result = pd.read_csv(algo2merged_fp[algo], index_col=0)
+                if cell_type in merged_result.columns:
+                    merged_result = merged_result.loc[(merged_result['reference_dataset'] == ref) &
+                                                      (merged_result['cancer_type'] == cancer_type)].copy()
+                    merged_result.set_index('sample_id', inplace=True)
+                    if algo == 'EPIC' and 'otherCells' in merged_result.columns:
+                        merged_result['Cancer Cells'] = merged_result.loc[:, ['Cancer Cells', 'otherCells']].sum(axis=1)
+                    df = merged_result.merge(mean_exp, left_index=True, right_index=True)
+                    n_sample = df.shape[0]
+                    # print(df.shape, algo)
+                    col_name1 = f'{cell_type}_marker_mean'  # mean of marker gene expression values
+                    col_name2 = cell_type  # predicted cell fraction
+                    corr = np.corrcoef(df[col_name1], df[col_name2])
+                    if df[cell_type].max() > max_cell_frac:
+                        max_cell_frac = df[cell_type].max()
+
+                    if cancer_type2max_frac is not None:
+                        ax[i, j].set_ylim([-0.01, cancer_type2max_frac[cancer_type] + 0.02])
+                    else:
+                        if cell_type in ['CD8 T', 'CD4 T', 'B Cells']:
+                            _max_exp = 0.25
+                        else:
+                            _max_exp = 0.6
+                        ax[i, j].set_ylim([-0.01, _max_exp + 0.02])
+                        df.loc[df[cell_type] > _max_exp, cell_type] = _max_exp  # set max fraction to 0.25
+                    # mae = median_absolute_error(y_true=df[col_name1], y_pred=df[col_name2])
+                    ax[i, j].scatter(df[col_name1], df[col_name2], s=1, alpha=0.8)
+                    # x_left, x_right = ax[i, j].get_xlim()
+                    y_bottom, y_top = ax[i, j].get_ylim()
+                    if 'CIBERSORT' in algo:
+                        algo = 'C.SORT'
+                    elif 'Scaden' in algo:
+                        algo = 'Scaden'
+                    elif 'EPIC' in algo:
+                        algo = 'EPIC'
+                    if 'simu_bulk' in ref:
+                        ref = 'simu_2ds'
+                    ax[i, j].set_xlabel('{} - {}'.format(algo, ref.replace('_ref', '')), fontsize=8)
+                    ax[i, j].text(1, y_top * 0.8, 'corr = {:.2f}'.format(corr[0, 1]), fontsize=6)
+                    corr_list[i * 3 + j] = round(corr[0, 1], 3)
+    fig.supylabel('Predicted cell fraction of {}'.format(f'{cell_type}'))
+    fig.supxlabel('mean expression of marker genes in {} (n={})'.format(cancer_type, n_sample))
+    # plt.tight_layout()
+    plt.savefig(os.path.join(result_dir, f'{result_file_name_prefix}_in_{cancer_type}.png'), dpi=300)
+    print('  Max cell fraction: {}'.format(max_cell_frac))
+    return {'corr': corr_list}
+
+
+def compare_y_y_pred_plot_cpe(y_true: pd.Series, y_pred: pd.Series, inx=tuple(), cancer_type='',
+                              show_metrics: bool = False, ax=None):
+    """
+    Plot y against y_pred to visualize the performance of prediction result
+
+    :param y_true: CPE
+
+    :param y_pred: this file contains the predicted value of y
+
+    :param inx: a tuple of two elements, the first element is the index of y_true, the second element is the index of y_pred
+
+    :param cancer_type: cancer type
+
+    :param show_metrics: show correlation and RMSE
+
+    :param ax: matplotlib axis
+
+    :return: None
+    """
+    # Use the pyplot interface to change just one subplot...
+    plt.sca(ax)
+
+    plt.scatter(y_pred, y_true, s=1, alpha=0.75, rasterized=True)
+    plt.xlim([-0.05, 1.05])
+    plt.ylim([-0.05, 1.05])
+    plt.xticks([0, 1])
+    plt.yticks([0, 0.5, 1])
+    x_left, x_right = plt.xlim()
+    y_bottom, y_top = plt.ylim()
+    x_max = x_right
+    y_max = y_top
+    plt.plot([0, max(x_max, y_max)], [0, max(x_max, y_max)], linestyle='--', color='tab:gray')
+    corr = 0
+    rmse = 0
+    ccc = 0
+    if show_metrics:  # show metrics in test set
+        corr = get_corr(y_pred, y_true)
+        rmse = calculate_rmse(y_true=pd.DataFrame(y_true), y_pred=pd.DataFrame(y_pred))
+        ccc = get_ccc(y_pred.values, y_true.values)
+        plt.text(0.3 * x_max, 0.2 * y_max, 'corr = {:.2f}'.format(corr), fontsize=6)
+        plt.text(0.3 * x_max, 0.1 * y_max, 'RMSE = {:.2f}'.format(rmse), fontsize=6)
+        plt.text(0.3 * x_max, 0.0 * y_max, 'CCC = {:.2f}'.format(ccc), fontsize=6)
+    if inx:
+        plt.ylabel(f'{cancer_type} ({y_true.shape[0]})', fontsize=6)
+    # if inx and inx[0] == 8:
+    #     plt.xlabel(f'{algo}', fontsize=6)
+    # plt.legend()
+    return corr, rmse, ccc
+
+
+def plot_pred_cell_prop_with_cpe(cpe_file_path, pred_cell_prop_file_path, result_dir, save_metrics: bool = True):
+    all_cancer_types = sorted([i for i in cancer_types if i != 'PAAD'])
+    fig, axes = plt.subplots(6, 3, sharex='all', sharey='all', figsize=(5, 6))
+    pred_cell_prop = pd.read_csv(pred_cell_prop_file_path, index_col=0)
+    cpe = read_cancer_purity(cpe_file_path, sample_names=pred_cell_prop.index)
+    pred_cell_prop = pred_cell_prop.merge(cpe['CPE'], left_index=True, right_index=True)
+    metrics_value = {}
+    for j in range(3):
+        for i in range(6):
+            current_cancer_type = all_cancer_types[i + j * 6]
+            current_data = pred_cell_prop.loc[pred_cell_prop['cancer_type'] == current_cancer_type, :]
+            corr, rmse, ccc = compare_y_y_pred_plot_cpe(y_pred=current_data['Cancer Cells'], y_true=current_data['CPE'],
+                                                        show_metrics=True, ax=axes[i, j], cancer_type=current_cancer_type,
+                                                        inx=(i, j))
+            metrics_value[current_cancer_type] = {'corr': corr, 'rmse': rmse, 'ccc': ccc}
+
+    # add a big axis, hide frame
+    fig.add_subplot(111, frameon=False)
+    # hide tick and tick label of the big axis
+    plt.tick_params(labelcolor='none', which='both', top=False, bottom=False, left=False, right=False)
+    plt.xlabel('Predicted cancer cell proportions by DeSide', labelpad=5)
+    plt.ylabel("CPE", labelpad=15)
+
+    plt.tight_layout(h_pad=0.02, w_pad=0.15)
+    plt.savefig(os.path.join(result_dir, 'pred_cancer_cell_prop_vs_cpe-deside.png'), dpi=300)
+    if save_metrics:
+        metrics_value_df = pd.DataFrame.from_dict(metrics_value, orient='index')
+        metrics_value_df.to_csv(os.path.join(result_dir, 'pred_cancer_cell_prop_vs_cpe-deside-metrics.csv'))
```

### Comparing `DeSide-1.0.1/deside/plot/plot_clustering.py` & `DeSide-1.0.2/deside/plot/plot_clustering.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-import os
-import time
-import scipy
-import numpy as np
-import pandas as pd
-from sklearn.manifold import TSNE
-from scipy.spatial import distance
-from scipy.cluster import hierarchy
-from ..utility import print_df, log2_transform, center_value, set_fig_style
-import matplotlib.colors as mcolors
-import matplotlib.pyplot as plt
-import seaborn as sns
-# sns.set()
-
-set_fig_style()
-
-
-def plot_hcluster(exp_df, sample2subtype=None, method='sample_corr',
-                  color_threshold=4.0, result_dir='', sample_type='', p=8,
-                  leaf_font_size=6, min_sample_in_cluster=15, log_transform=True, center=True):
-    """
-    plot heatmap and dendrogram after hierarchy clustering
-    :param exp_df: expression dataframe, gene x samples, non-log and non-centered values
-        - can be centered by genes after log2 normalized for calculating sample correlation
-        - or clustering by gene expression directly
-    :param sample2subtype: dataframe, sample x subtype
-        sample annotation, must contain 'subtype' column and use sample name as index
-    :param method: str
-        sample_corr (correlation between each sample) or distance (between genes <row-wise> and samples <col-wise>)
-    :param color_threshold: color threshold for dendrogram graph
-    :param result_dir:
-    :param sample_type: only for naming result file or naming subtype if sample2subtype is None
-    :param p:  int, optional
-        The ``p`` parameter for ``truncate_mode`` in hierarchy.dendrogram.
-    :param leaf_font_size: leaf_font_size
-    :param min_sample_in_cluster: if the number of samples in a cluster < this number, this cluster will be removed
-    :param log_transform: if logarithm
-    :param center: if center data
-    :return: reordered samples in each cluster and cluster id
-    """
-    if sample2subtype is None:
-        sample2subtype = pd.DataFrame(index=exp_df.columns, columns=['subtype'])
-        sample2subtype['subtype'] = sample_type
-    else:
-        assert 'subtype' in sample2subtype.columns
-    sample2subtype = sample2subtype.loc[:, ['subtype']].copy()
-    subtype = np.unique(list(sample2subtype['subtype']))
-    _colors = [i for i in mcolors.TABLEAU_COLORS.keys()]
-    if len(subtype) > 10:
-        print('There are more than 10 subtypes, some colors may used more than 1 time.')
-        _colors = _colors * (len(subtype)//10 + 1)
-    color = _colors[:len(subtype)]
-    lut = dict(zip(subtype, color))
-    print('subtype2color: {}'.format(lut))
-    row_colors = sample2subtype['subtype'].map(lut)
-    if log_transform:
-        exp_df = log2_transform(exp_df)
-
-    if method == 'sample_corr':
-        # center log-transformed data before calculate correlation
-        if center:
-            exp_df = center_value(exp_df)
-        sample_corr = exp_df.corr()
-        row_linkage = hierarchy.linkage(
-            distance.pdist(sample_corr), method='centroid')
-
-        col_linkage = hierarchy.linkage(
-            distance.pdist(sample_corr.T), method='centroid')
-        if len(subtype) >= 2:
-            g1 = sns.clustermap(sample_corr,
-                                row_linkage=row_linkage, col_linkage=col_linkage,
-                                row_colors=row_colors, col_colors=row_colors,
-                                method="centroid", figsize=(15, 15), cmap='vlag')
-        else:
-            g1 = sns.clustermap(sample_corr,
-                                row_linkage=row_linkage, col_linkage=col_linkage,
-                                method="centroid", figsize=(15, 15), cmap='vlag')
-    else:
-        # distance between gene pairs, treat each row as a sample
-        # row_linkage = hierarchy.linkage(
-        #     distance.pdist(exp_df), metric='euclidean', method='centroid')
-
-        # distance between sample pairs
-        col_linkage = hierarchy.linkage(
-            distance.pdist(exp_df.T), metric='euclidean', method='centroid')
-        g1 = sns.clustermap(exp_df, row_linkage=None, col_linkage=col_linkage,
-                            col_colors=row_colors, z_score=0,
-                            method="centroid", figsize=(18, 18), cmap='vlag')
-    if not os.path.exists(result_dir):
-        os.makedirs(result_dir)
-    g1.savefig(os.path.join(result_dir, '{}_hierarchy_clustering.png'.format(sample_type)), dpi=200)
-    plt.close()
-
-    plt.figure(figsize=(18, 6))
-    hierarchy.dendrogram(col_linkage, show_leaf_counts=True, p=p, truncate_mode='level', leaf_font_size=leaf_font_size,
-                         leaf_rotation=50, color_threshold=color_threshold)
-    plt.savefig(os.path.join(result_dir, '{}_dendrogram.png'.format(sample_type)), dpi=200)
-    plt.close()
-    # return {'row_linkage': row_linkage, 'col_linkage': col_linkage, 'g1': g1}
-
-    # get sub cluster info: reordered samples in each cluster and cluster id
-    node_id2sub_cluster = cut_cluster_by_distance(col_linkage, threshold=color_threshold)
-    reordered_ind2sample_name = {}
-    # g1 = linkage['g1']
-    # sample_corr = bulk_tpm_log_c.corr()
-    for ind in g1.dendrogram_col.reordered_ind:
-        reordered_ind2sample_name[ind] = exp_df.columns[ind]
-    reordered_ind2sample_name_df = pd.DataFrame.from_dict(data=reordered_ind2sample_name, orient='index',
-                                                          columns=['sample_name'])
-    # reordered_ind2sample_name_df.head(2)
-    reordered_ind2sample_name_df['cluster_id'] = reordered_ind2sample_name_df.index.map(node_id2sub_cluster)
-    reordered_ind2sample_name_df2 = reordered_ind2sample_name_df.merge(sample2subtype, left_on='sample_name',
-                                                                       right_index=True)
-    reordered_ind2sample_name_df2.index.name = 'reordered_inx'
-    print_df(reordered_ind2sample_name_df2)
-    reordered_ind2sample_name_df2['color'] = reordered_ind2sample_name_df2['subtype'].map(lut)
-
-    subtype_pivot = reordered_ind2sample_name_df2.pivot_table(index=['cluster_id'], columns='subtype',
-                                                              aggfunc='size', fill_value=0)
-    non_new = subtype_pivot.loc[:, [i for i in subtype_pivot.columns if i != 'New']]
-    max_inx = np.where(non_new == np.vstack(non_new.max(axis=1)))
-    cluster_id2max_col_inx = dict(zip(max_inx[0], max_inx[1]))  # prevent multiple values equal to max
-    subtype_pivot.columns = subtype_pivot.columns.astype(str)
-    subtype_pivot['predicted_subtype'] = [subtype_pivot.columns[cluster_id2max_col_inx[x]]
-                                          for x in range(subtype_pivot.shape[0])]
-    # subtype_pivot['predicted_subtype'] = np.vstack(
-    #     non_new.columns[np.where(non_new == np.vstack(non_new.max(axis=1)))[1]].to_list())
-    _main_subtype_percent_name = 'main_subtype%'
-    if 'New' in subtype_pivot.columns:
-        _main_subtype_percent_name = 'main_subtype_with_new%'
-        subtype_pivot[_main_subtype_percent_name] = (non_new.max(axis=1) + subtype_pivot['New']) / subtype_pivot.sum(axis=1)
-
-    else:
-        subtype_pivot[_main_subtype_percent_name] = non_new.max(axis=1) / subtype_pivot.sum(axis=1)
-        # subtype_pivot['keep'] = (non_new.max(axis=1) >= 5) &
-    subtype_pivot['keep'] = (non_new.max(axis=1) >= min_sample_in_cluster) & \
-                            (subtype_pivot[_main_subtype_percent_name] >= 0.8)
-    subtype_pivot['keep'] = subtype_pivot['keep'].map({True: 1, False: 0})
-    reordered_ind2sample_name_df2 = reordered_ind2sample_name_df2.merge(subtype_pivot[['predicted_subtype',
-                                                                                       _main_subtype_percent_name,
-                                                                                       'keep']],
-                                                                        left_on='cluster_id', right_index=True)
-
-    subtype_pivot.to_csv(os.path.join(result_dir, 'subtype_pivot.csv'))
-    reordered_ind2sample_name_df2.to_csv(os.path.join(result_dir, 'reordered_ind2sample_name.csv'),
-                                         index=False, float_format='%.3f')
-    with open(os.path.join(result_dir, 'color_threshold.txt'), 'w') as f:
-        f.write(str(color_threshold) + '\n')
-    return reordered_ind2sample_name_df2
-
-
-def split_tree_by_distance(node, threshold):
-    assert type(node) == scipy.cluster.hierarchy.ClusterNode
-    if node.count < 2:
-        return [node]
-    else:
-        if node.dist <= threshold:
-            return [node]
-        else:
-            return split_tree_by_distance(node.left, threshold) + split_tree_by_distance(node.right, threshold)
-
-
-def cut_cluster_by_distance(linkage_matrix, threshold):
-    """
-    linkage_matrix: the matrix comes from hierarchy.linkage,
-    https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage
-    threshold: a float, max distance of clusters in the tree at the cut point
-    """
-    node_id2sub_cluster = {}
-    root_node = hierarchy.to_tree(linkage_matrix)
-    root_node_in_sub_clusters = split_tree_by_distance(root_node, threshold=threshold)
-    for i, sub_rootnodes in enumerate(root_node_in_sub_clusters):
-        subcluster_nodes = get_node_id(sub_rootnodes)
-        for _node_id in subcluster_nodes:
-            node_id2sub_cluster[_node_id] = i
-    return node_id2sub_cluster
-
-
-def get_node_id(node):
-    assert type(node) == scipy.cluster.hierarchy.ClusterNode
-    if node.count == 1:
-        return [node.id]
-    else:
-        left_node = node.left
-        right_node = node.right
-        return get_node_id(left_node) + get_node_id(right_node)
-
-
-def t_sne_plot(exp_profile, group2sample, result_file=None, n_jobs=4,
-               n_iter=3000, perplexity=10):
-    """
-    plot expression profiles by t-SNE
-    :param exp_profile: a dataFrame, gene x sample
-        the expression profiles of single cell or bulk cell
-    :param group2sample: dict
-        cell type with all sample names in this cell type, {'': [], '': [], ...}
-    :param result_file: where to save figure
-    :param n_jobs:
-    :param n_iter:
-    :param perplexity:
-    :return:
-    """
-    t0 = time.time()
-    exp_profile = exp_profile.T  # convert to sample by gene
-    tsne = TSNE(n_components=2, n_jobs=n_jobs, learning_rate=200, metric='euclidean',
-                n_iter=n_iter, init='pca', verbose=1, perplexity=perplexity)
-    x_reduced = tsne.fit_transform(exp_profile)
-    # X_reduced_tsne = tsne.fit(x)
-    print(x_reduced.shape)
-    # np.save('X_reduced_tsne_pca_first', X_reduced_tsne2)
-    t1 = time.time()
-    print("t-SNE took {:.1f}s.".format(t1 - t0))
-    x_reduced = pd.DataFrame(data=x_reduced, index=exp_profile.index)
-    # groups = np.unique(list(group2sample.values()))
-    plt.figure(figsize=(8, 6))
-    for g, current_samples in group2sample.items():
-        # current_samples = [i for i, j in group2sample.items() if j == g]
-        current_corr = x_reduced.loc[x_reduced.index.isin(current_samples), :]
-        plt.scatter(current_corr[0], current_corr[1], label=g, s=6)
-    plt.xlabel('t-SNE1')
-    plt.ylabel('t-SNE2')
-    plt.legend()
-    plt.tight_layout()
-    if result_file:
-        plt.savefig(result_file, dpi=200)
-        plt.close()
-        x_reduced.to_csv(result_file.replace('.png', '.csv'))
-    else:
-        return plt
+import os
+import time
+import scipy
+import numpy as np
+import pandas as pd
+from sklearn.manifold import TSNE
+from scipy.spatial import distance
+from scipy.cluster import hierarchy
+from ..utility import print_df, log2_transform, center_value, set_fig_style
+import matplotlib.colors as mcolors
+import matplotlib.pyplot as plt
+import seaborn as sns
+# sns.set()
+
+set_fig_style()
+
+
+def plot_hcluster(exp_df, sample2subtype=None, method='sample_corr',
+                  color_threshold=4.0, result_dir='', sample_type='', p=8,
+                  leaf_font_size=6, min_sample_in_cluster=15, log_transform=True, center=True):
+    """
+    plot heatmap and dendrogram after hierarchy clustering
+    :param exp_df: expression dataframe, gene x samples, non-log and non-centered values
+        - can be centered by genes after log2 normalized for calculating sample correlation
+        - or clustering by gene expression directly
+    :param sample2subtype: dataframe, sample x subtype
+        sample annotation, must contain 'subtype' column and use sample name as index
+    :param method: str
+        sample_corr (correlation between each sample) or distance (between genes <row-wise> and samples <col-wise>)
+    :param color_threshold: color threshold for dendrogram graph
+    :param result_dir:
+    :param sample_type: only for naming result file or naming subtype if sample2subtype is None
+    :param p:  int, optional
+        The ``p`` parameter for ``truncate_mode`` in hierarchy.dendrogram.
+    :param leaf_font_size: leaf_font_size
+    :param min_sample_in_cluster: if the number of samples in a cluster < this number, this cluster will be removed
+    :param log_transform: if logarithm
+    :param center: if center data
+    :return: reordered samples in each cluster and cluster id
+    """
+    if sample2subtype is None:
+        sample2subtype = pd.DataFrame(index=exp_df.columns, columns=['subtype'])
+        sample2subtype['subtype'] = sample_type
+    else:
+        assert 'subtype' in sample2subtype.columns
+    sample2subtype = sample2subtype.loc[:, ['subtype']].copy()
+    subtype = np.unique(list(sample2subtype['subtype']))
+    _colors = [i for i in mcolors.TABLEAU_COLORS.keys()]
+    if len(subtype) > 10:
+        print('There are more than 10 subtypes, some colors may used more than 1 time.')
+        _colors = _colors * (len(subtype)//10 + 1)
+    color = _colors[:len(subtype)]
+    lut = dict(zip(subtype, color))
+    print('subtype2color: {}'.format(lut))
+    row_colors = sample2subtype['subtype'].map(lut)
+    if log_transform:
+        exp_df = log2_transform(exp_df)
+
+    if method == 'sample_corr':
+        # center log-transformed data before calculate correlation
+        if center:
+            exp_df = center_value(exp_df)
+        sample_corr = exp_df.corr()
+        row_linkage = hierarchy.linkage(
+            distance.pdist(sample_corr), method='centroid')
+
+        col_linkage = hierarchy.linkage(
+            distance.pdist(sample_corr.T), method='centroid')
+        if len(subtype) >= 2:
+            g1 = sns.clustermap(sample_corr,
+                                row_linkage=row_linkage, col_linkage=col_linkage,
+                                row_colors=row_colors, col_colors=row_colors,
+                                method="centroid", figsize=(15, 15), cmap='vlag')
+        else:
+            g1 = sns.clustermap(sample_corr,
+                                row_linkage=row_linkage, col_linkage=col_linkage,
+                                method="centroid", figsize=(15, 15), cmap='vlag')
+    else:
+        # distance between gene pairs, treat each row as a sample
+        # row_linkage = hierarchy.linkage(
+        #     distance.pdist(exp_df), metric='euclidean', method='centroid')
+
+        # distance between sample pairs
+        col_linkage = hierarchy.linkage(
+            distance.pdist(exp_df.T), metric='euclidean', method='centroid')
+        g1 = sns.clustermap(exp_df, row_linkage=None, col_linkage=col_linkage,
+                            col_colors=row_colors, z_score=0,
+                            method="centroid", figsize=(18, 18), cmap='vlag')
+    if not os.path.exists(result_dir):
+        os.makedirs(result_dir)
+    g1.savefig(os.path.join(result_dir, '{}_hierarchy_clustering.png'.format(sample_type)), dpi=200)
+    plt.close()
+
+    plt.figure(figsize=(18, 6))
+    hierarchy.dendrogram(col_linkage, show_leaf_counts=True, p=p, truncate_mode='level', leaf_font_size=leaf_font_size,
+                         leaf_rotation=50, color_threshold=color_threshold)
+    plt.savefig(os.path.join(result_dir, '{}_dendrogram.png'.format(sample_type)), dpi=200)
+    plt.close()
+    # return {'row_linkage': row_linkage, 'col_linkage': col_linkage, 'g1': g1}
+
+    # get sub cluster info: reordered samples in each cluster and cluster id
+    node_id2sub_cluster = cut_cluster_by_distance(col_linkage, threshold=color_threshold)
+    reordered_ind2sample_name = {}
+    # g1 = linkage['g1']
+    # sample_corr = bulk_tpm_log_c.corr()
+    for ind in g1.dendrogram_col.reordered_ind:
+        reordered_ind2sample_name[ind] = exp_df.columns[ind]
+    reordered_ind2sample_name_df = pd.DataFrame.from_dict(data=reordered_ind2sample_name, orient='index',
+                                                          columns=['sample_name'])
+    # reordered_ind2sample_name_df.head(2)
+    reordered_ind2sample_name_df['cluster_id'] = reordered_ind2sample_name_df.index.map(node_id2sub_cluster)
+    reordered_ind2sample_name_df2 = reordered_ind2sample_name_df.merge(sample2subtype, left_on='sample_name',
+                                                                       right_index=True)
+    reordered_ind2sample_name_df2.index.name = 'reordered_inx'
+    print_df(reordered_ind2sample_name_df2)
+    reordered_ind2sample_name_df2['color'] = reordered_ind2sample_name_df2['subtype'].map(lut)
+
+    subtype_pivot = reordered_ind2sample_name_df2.pivot_table(index=['cluster_id'], columns='subtype',
+                                                              aggfunc='size', fill_value=0)
+    non_new = subtype_pivot.loc[:, [i for i in subtype_pivot.columns if i != 'New']]
+    max_inx = np.where(non_new == np.vstack(non_new.max(axis=1)))
+    cluster_id2max_col_inx = dict(zip(max_inx[0], max_inx[1]))  # prevent multiple values equal to max
+    subtype_pivot.columns = subtype_pivot.columns.astype(str)
+    subtype_pivot['predicted_subtype'] = [subtype_pivot.columns[cluster_id2max_col_inx[x]]
+                                          for x in range(subtype_pivot.shape[0])]
+    # subtype_pivot['predicted_subtype'] = np.vstack(
+    #     non_new.columns[np.where(non_new == np.vstack(non_new.max(axis=1)))[1]].to_list())
+    _main_subtype_percent_name = 'main_subtype%'
+    if 'New' in subtype_pivot.columns:
+        _main_subtype_percent_name = 'main_subtype_with_new%'
+        subtype_pivot[_main_subtype_percent_name] = (non_new.max(axis=1) + subtype_pivot['New']) / subtype_pivot.sum(axis=1)
+
+    else:
+        subtype_pivot[_main_subtype_percent_name] = non_new.max(axis=1) / subtype_pivot.sum(axis=1)
+        # subtype_pivot['keep'] = (non_new.max(axis=1) >= 5) &
+    subtype_pivot['keep'] = (non_new.max(axis=1) >= min_sample_in_cluster) & \
+                            (subtype_pivot[_main_subtype_percent_name] >= 0.8)
+    subtype_pivot['keep'] = subtype_pivot['keep'].map({True: 1, False: 0})
+    reordered_ind2sample_name_df2 = reordered_ind2sample_name_df2.merge(subtype_pivot[['predicted_subtype',
+                                                                                       _main_subtype_percent_name,
+                                                                                       'keep']],
+                                                                        left_on='cluster_id', right_index=True)
+
+    subtype_pivot.to_csv(os.path.join(result_dir, 'subtype_pivot.csv'))
+    reordered_ind2sample_name_df2.to_csv(os.path.join(result_dir, 'reordered_ind2sample_name.csv'),
+                                         index=False, float_format='%.3f')
+    with open(os.path.join(result_dir, 'color_threshold.txt'), 'w') as f:
+        f.write(str(color_threshold) + '\n')
+    return reordered_ind2sample_name_df2
+
+
+def split_tree_by_distance(node, threshold):
+    assert type(node) == scipy.cluster.hierarchy.ClusterNode
+    if node.count < 2:
+        return [node]
+    else:
+        if node.dist <= threshold:
+            return [node]
+        else:
+            return split_tree_by_distance(node.left, threshold) + split_tree_by_distance(node.right, threshold)
+
+
+def cut_cluster_by_distance(linkage_matrix, threshold):
+    """
+    linkage_matrix: the matrix comes from hierarchy.linkage,
+    https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage
+    threshold: a float, max distance of clusters in the tree at the cut point
+    """
+    node_id2sub_cluster = {}
+    root_node = hierarchy.to_tree(linkage_matrix)
+    root_node_in_sub_clusters = split_tree_by_distance(root_node, threshold=threshold)
+    for i, sub_rootnodes in enumerate(root_node_in_sub_clusters):
+        subcluster_nodes = get_node_id(sub_rootnodes)
+        for _node_id in subcluster_nodes:
+            node_id2sub_cluster[_node_id] = i
+    return node_id2sub_cluster
+
+
+def get_node_id(node):
+    assert type(node) == scipy.cluster.hierarchy.ClusterNode
+    if node.count == 1:
+        return [node.id]
+    else:
+        left_node = node.left
+        right_node = node.right
+        return get_node_id(left_node) + get_node_id(right_node)
+
+
+def t_sne_plot(exp_profile, group2sample, result_file=None, n_jobs=4,
+               n_iter=3000, perplexity=10):
+    """
+    plot expression profiles by t-SNE
+    :param exp_profile: a dataFrame, gene x sample
+        the expression profiles of single cell or bulk cell
+    :param group2sample: dict
+        cell type with all sample names in this cell type, {'': [], '': [], ...}
+    :param result_file: where to save figure
+    :param n_jobs:
+    :param n_iter:
+    :param perplexity:
+    :return:
+    """
+    t0 = time.time()
+    exp_profile = exp_profile.T  # convert to sample by gene
+    tsne = TSNE(n_components=2, n_jobs=n_jobs, learning_rate=200, metric='euclidean',
+                n_iter=n_iter, init='pca', verbose=1, perplexity=perplexity)
+    x_reduced = tsne.fit_transform(exp_profile)
+    # X_reduced_tsne = tsne.fit(x)
+    print(x_reduced.shape)
+    # np.save('X_reduced_tsne_pca_first', X_reduced_tsne2)
+    t1 = time.time()
+    print("t-SNE took {:.1f}s.".format(t1 - t0))
+    x_reduced = pd.DataFrame(data=x_reduced, index=exp_profile.index)
+    # groups = np.unique(list(group2sample.values()))
+    plt.figure(figsize=(8, 6))
+    for g, current_samples in group2sample.items():
+        # current_samples = [i for i, j in group2sample.items() if j == g]
+        current_corr = x_reduced.loc[x_reduced.index.isin(current_samples), :]
+        plt.scatter(current_corr[0], current_corr[1], label=g, s=6)
+    plt.xlabel('t-SNE1')
+    plt.ylabel('t-SNE2')
+    plt.legend()
+    plt.tight_layout()
+    if result_file:
+        plt.savefig(result_file, dpi=200)
+        plt.close()
+        x_reduced.to_csv(result_file.replace('.png', '.csv'))
+    else:
+        return plt
```

### Comparing `DeSide-1.0.1/deside/plot/plot_nn.py` & `DeSide-1.0.2/deside/plot/plot_nn.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-import os
-# import importlib
-# import umap
-import numpy as np
-import pandas as pd
-import seaborn as sns
-# import scipy.stats as stats
-import matplotlib.pyplot as plt
-# from joblib import dump, load
-from .plot_gene import compare_exp_between_group
-from ..utility import read_cancer_purity, check_dir, read_df, log2_transform, set_fig_style
-from sklearn.metrics import median_absolute_error
-# sns.set()
-# sns.set(font_scale=1.5)
-# plt.rcParams.update({'font.size': 20})
-set_fig_style()
-
-
-def plot_loss(history_df, output_dir=None, x_label='n_epoch', y_label='MSE', file_name=None):
-    """
-    :param history_df:
-    :param output_dir:
-    :param x_label:
-    :param y_label:
-    :param file_name:
-    :return:
-    """
-    # sns.set(font_scale=1.5)
-    plt.figure(figsize=(8, 6))
-    if 'loss' in history_df.columns:
-        plt.plot(history_df['epoch'], history_df['loss'], label='loss')
-    if 'val_loss' in history_df.columns:
-        plt.plot(history_df['epoch'], history_df['val_loss'], label='val_loss')
-    if 'total_loss' in history_df.columns:
-        plt.plot(history_df['epoch'], history_df['total_loss'], label='total_loss')
-    if 'val_total_loss' in history_df.columns:
-        plt.plot(history_df['epoch'], history_df['val_total_loss'], label='val_total_loss')
-    plt.legend()
-    plt.xlabel(x_label)
-    plt.ylabel(y_label.upper())
-    plt.tight_layout()
-    if output_dir:
-        if file_name is not None:
-            plt.savefig(os.path.join(output_dir, file_name), dpi=200)
-        else:
-            plt.savefig(os.path.join(output_dir, 'loss.png'), dpi=200)
-        plt.close()
-    else:
-        return plt
-
-
-def plot_corr_two_columns(df: pd.DataFrame, output_dir: str, col_name1: str = 'CPE',
-                          col_name2: str = 'cancer_cell', cancer_type: str = '', diagonal: bool = True,
-                          predicted_by: str = None, font_scale: float = 1.5, scale_exp=False, update_figures=False):
-    """
-    Plot the relation between two columns in DataFrame `df`
-
-    :param df: a dataFrame which contains CPE (cancer purity) and cancer_fraction
-
-    :param output_dir: result folder
-
-    :param col_name1: column name, such as CPE (cancer purity), x axis
-
-    :param col_name2: column name, such as cancer cell fraction (predicted cancer purity), y axis
-
-    :param cancer_type: mark x axis / y axis label
-
-    :param diagonal: if plot diagonal
-
-    :param predicted_by: model name
-
-    :param font_scale: scale font size
-
-    :param scale_exp: if scale all expression values to range [0, 10] by x_i/max(x) * 10
-
-    :param update_figures: if update figures in output_dir
-
-    :return: None
-    """
-    check_dir(output_dir)
-    result_file_path = os.path.join(output_dir, '{}_vs_predicted_{}_proportion.png'.format(col_name1, col_name2))
-    if (not os.path.exists(result_file_path)) or update_figures:
-        # sns.set(font_scale=font_scale)
-        # plt.rcParams['font.sans-serif'] = ['Arial Unicode MS']  # show Chinese characters
-        plt.figure(figsize=(8, 8))
-        df_col1 = df[col_name1].copy()
-        df_col2 = df[col_name2].copy()
-        if np.any(df_col1 > 2) and scale_exp:
-            df_col1 = df_col1 / df_col1.max() * 10
-        if np.any(df_col2 > 2) and scale_exp:
-            df_col2 = df_col2 / df_col2.max() * 10
-
-        corr = np.corrcoef(df_col1, df_col2)
-        # print(corr)
-        if np.isnan(corr[0, 1]):
-            corr[0, 1] = 0  # when all predicted cell fraction are 0, set corr to 0
-        # corr2 = stats.pearsonr(df[col_name1], df[col_name2])
-        mae = median_absolute_error(y_true=df_col1, y_pred=df_col2)
-        plt.scatter(df_col1, df_col2, s=8)
-        plt.xlabel('{} ({})'.format(col_name1, cancer_type))
-        # plt.xlabel('{} (头颈癌)'.format(col_name1))
-        # plt.ylabel('预测 {} 比例 (样本数={})'.format(col_name2, df.shape[0]))
-        x_left, x_right = plt.xlim()
-        y_bottom, y_top = plt.ylim()
-        if '_true' in col_name2:
-            plt.ylabel('{} prop. (n={})'.format(col_name2, df.shape[0]))
-        elif predicted_by:
-            plt.ylabel('Predicted {} prop. by {} (n={})'.format(col_name2, predicted_by, df.shape[0]))
-            # plt.ylabel('{}预测值 (样本数={})'.format(predicted_by, df.shape[0]))
-        else:
-            plt.ylabel('{} prop. (n={})'.format(col_name2, df.shape[0]))
-        if 'CPE' in [col_name1, col_name2]:
-            plt.text(0.05, 0.95, 'corr = {:.3f}'.format(corr[0, 1]))
-            plt.text(0.05, 0.90, '$MAE$ = {:.3f}'.format(mae))
-        elif ('CD8A' in [col_name1, col_name2]) or ('CD8A+CD8B' in [col_name1, col_name2]):
-            plt.text(x_left + 1.5, y_top * 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
-        elif 'CD3E' in [col_name1, col_name2]:
-            plt.text(x_left + 1.5, y_top * 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
-        elif 'y_pred' in [col_name1, col_name2]:
-            plt.text(0.2, 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
-            plt.text(0.2, 0.85, '$MAE$ = {:.3f}'.format(mae))
-            # plt.title()
-        elif '_true' in col_name1 or '_true' in col_name2:
-            plt.text(0.1, 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
-            plt.text(0.1, 0.85, '$MAE$ = {:.3f}'.format(mae))
-        elif ('_marker_mean' in col_name1) or ('_marker_max' in col_name1):
-            # compare mean expression of marker genes and predicted cell fraction
-            plt.text(x_right * 0.05, y_top * 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
-        elif '_gene_signature_score' in col_name1:
-            # compare mean expression of marker genes and predicted cell fraction
-            plt.text(x_right * 0.05, y_top * 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
-        if diagonal:
-            plt.plot([0, 1], [0, 1], linestyle='--', color='tab:gray')
-        plt.tight_layout()
-        plt.savefig(result_file_path, dpi=200)
-        plt.close('all')
-    else:
-        print(f'   Using previous figure, {result_file_path}')
-
-
-def plot_predicted_result(cell_frac_result_fp, bulk_exp_fp, cancer_type,
-                          model_name, result_dir, cancer_purity_fp: str = None,
-                          font_scale=2.0, update_figures=False):
-    """
-    Plot and evaluate predicted results of DeSide or Scaden model for TCGA data
-
-    :param cell_frac_result_fp: the file path of predicted cell fraction
-
-    :param bulk_exp_fp: the file path of bulk cell expression profile or pd.Dataframe, TPM, gene by sample
-
-    :param cancer_type: only for naming or mark x / y label when plotting
-
-    :param model_name: model name, DeSide or Scaden
-
-    :param result_dir: where to save result
-
-    :param cancer_purity_fp: estimated tumor purity for TCGA, download from
-        Aran, D. et al., Nat Commun 6, 8971 (2015), Supplementary Data 1
-
-    :param font_scale: scale font size
-
-    :param update_figures: whether to update figures
-
-    :return: None
-    """
-    y_pred = read_df(cell_frac_result_fp)  # cell fraction, sample by cell type
-    # sep = get_sep(bulk_exp_fp)
-    bulk_exp_cpm = read_df(bulk_exp_fp)
-    # bulk_exp_cpm = log_exp2cpm(bulk_exp_log2cpm1p)
-
-    # plot CD8 T cell fraction against CD8A expression value
-    merged_df1 = y_pred.merge(bulk_exp_cpm.T, left_index=True, right_index=True)
-    plot_corr_two_columns(df=merged_df1, col_name2='CD8 T', col_name1='CD8A',
-                          predicted_by=model_name, font_scale=font_scale,
-                          output_dir=result_dir, diagonal=False, cancer_type=cancer_type, update_figures=update_figures)
-
-    if cancer_purity_fp is not None:
-        # read cancer purity file
-        cancer_purity = read_cancer_purity(cancer_purity_fp, sample_names=list(y_pred.index))
-        merged_df = y_pred.merge(cancer_purity, left_index=True, right_index=True)
-        # plot CPE vs cell fraction of cancer cell / 1-others
-        if merged_df.shape[0] > 0:
-            merged_df.to_csv(os.path.join(result_dir,
-                                          f'cancer_purity_merged_{model_name}_predicted_result.csv'))
-            plot_corr_two_columns(df=merged_df, col_name1='CPE', col_name2='Cancer Cells',
-                                  output_dir=result_dir, font_scale=font_scale,
-                                  cancer_type=cancer_type, predicted_by=model_name, update_figures=update_figures)
-            # plot_corr_two_columns(df=merged_df, col_name1='CPE', col_name2='1-others',
-            #                       output_dir=result_dir, font_scale=font_scale,
-            #                       cancer_type=cancer_type, predicted_by=model_name)
-        else:
-            print('   There is no any samples in cancer purity about this cancer type ({})'.format(cancer_type))
-    # plot cell fraction of each cell type before decon_cf
-    y_pred['labels'] = 1
-    # if 'DeSide' in model_name:
-    #     y_pred.drop(columns='Cancer Cells', inplace=True)
-    #     # remove labels and the last cell type
-    #     cell_types = sorted(y_pred.columns.to_list())
-    #     cell_types = [i for i in cell_types if i not in ['1-others', 'labels']]
-    #     cell_types = cell_types + ['1-others']
-    # else:
-    #     y_pred.drop(columns='1-others', inplace=True)
-    #     cell_types = sorted(y_pred.columns.to_list()[:-2]) + ['Cancer Cells']
-    cell_types = sorted(y_pred.columns.to_list())
-    cell_types = [i for i in cell_types if i not in ['1-others', 'labels']]
-    # cell_types =
-    print('   Cell types: ', ', '.join(cell_types))
-    compare_exp_between_group(exp=y_pred, group_list=tuple(cell_types),
-                              result_dir=result_dir, xlabel=f'Cell Type ({cancer_type})',
-                              ylabel=f'Cell prop. predicted by {model_name}',
-                              file_name='pred_cell_prop_before_decon.png', font_scale=font_scale - 0.4,
-                              xticks_rotation=50)
-
-
-def plot_paras(paras_file_path, vae_cla_model, latent_z_pos,
-               current_cell_types, sampled_sc_id_file=None, sample_id: str = None, result_file=None):
-    """
-    plot parameters of regression model (deconvolved GEP) in latent z space
-    :param paras_file_path: w, weights of regression model which represent valid GEPs for each cell type
-    :param vae_cla_model:
-    :param latent_z_pos: latent z for all training set of VAEClassifier model (encoder)
-    :param current_cell_types
-    :param sample_id: only provide if plot this sample
-    :param sampled_sc_id_file: selected single cell id for each simulated GEP
-    :param result_file:
-    """
-
-    latent_z_pos = read_df(latent_z_pos)
-    paras = read_df(paras_file_path)
-    if paras.shape[0] > paras.shape[1]:  # sample by cell type
-        paras = paras.loc[:, current_cell_types].T
-    else:
-        paras = paras.loc[current_cell_types, :]
-    paras = log2_transform(paras)
-
-    _, _, latent_z_paras, _ = vae_cla_model.encoder_predict(paras.values)
-
-    plt.figure(figsize=(8, 8))
-    plt.scatter(latent_z_pos.loc[:, 'z1'], latent_z_pos.loc[:, 'z2'], color='gray')
-    if sample_id is not None:  # the location of ground truth
-        if sampled_sc_id_file is None:
-            raise FileNotFoundError('sampled_sc_id_file should be provided with sample_id to plot this sample')
-        sampled_sc_id_file = read_df(sampled_sc_id_file)
-        current_sc_ids = sampled_sc_id_file.loc[sample_id, :].copy()
-        sc_ids = dict(zip(current_sc_ids['cell_type'], current_sc_ids['selected_cell_id']))
-        sc_id_list = [sc_ids[_] for _ in current_cell_types]
-        plt.scatter(latent_z_pos.loc[sc_id_list, 'z1'], latent_z_pos.loc[sc_id_list, 'z2'], marker='x', color='red')
-    plt.scatter(latent_z_paras[:, 0], latent_z_paras[:, 1], marker='*', color='green')
-    if result_file is not None:
-        plt.savefig(result_file, dpi=200)
-    plt.close()
-
-
-def plot_paras_all_cell_types(latent_z_paras_file, latent_z_pos_file, current_cell_types,
-                              sampled_sc_id_file=None, sample_id: str = None, result_file=None):
-    """
-    plot parameters of regression model (deconvolved GEP) in latent z space
-    :param latent_z_paras_file: latent z of all cell types which represent valid GEPs for each cell type
-        - generated by VAEDecon model (encoder), n_cell_type x latent_dim
-    :param latent_z_pos_file: latent z for all training set of VAEClassifier model (encoder)
-    :param current_cell_types:
-    :param sample_id: only provide if plot this sample
-    :param sampled_sc_id_file: selected single cell id for each simulated GEP
-    :param result_file:
-    """
-
-    latent_z_pos_file = read_df(latent_z_pos_file)
-    if type(latent_z_paras_file) == str:
-        paras = pd.read_csv(latent_z_paras_file, index_col=[0, 1])
-    else:  # pd.Dataframe
-        paras = latent_z_paras_file
-    sample_inx = [(sample_id, ct) for ct in current_cell_types]
-    latent_z_paras = paras.loc[sample_inx, :].copy()  # n_cell_type x latent_dim
-    plt.figure(figsize=(8, 8))
-    col_names = latent_z_pos_file.columns.to_list()
-    plt.scatter(latent_z_pos_file.iloc[:, 0], latent_z_pos_file.iloc[:, 1], color='gray')
-    if sample_id is not None:  # the location of ground truth
-        if sampled_sc_id_file is None:
-            raise FileNotFoundError('sampled_sc_id_file should be provided with sample_id to plot this sample')
-        if type(sampled_sc_id_file) == str:
-            sampled_sc_id_file = pd.read_csv(sampled_sc_id_file, index_col=[0, 1])
-        # sample_inx = list(zip([sample_id] * len(current_cell_types), current_cell_types))
-        current_sc_ids = sampled_sc_id_file.loc[sample_inx, 'selected_cell_id'].to_list()
-        # sc_ids = dict(zip(current_sc_ids['cell_type'], current_sc_ids['selected_cell_id']))
-        # sc_id_list = [sc_ids[_] for _ in current_cell_types]
-        plt.scatter(latent_z_pos_file.loc[current_sc_ids, col_names[0]],
-                    latent_z_pos_file.loc[current_sc_ids, col_names[1]],
-                    marker='x', color='red')
-    plt.scatter(latent_z_paras.loc[:, col_names[0]], latent_z_paras.loc[:, col_names[1]], marker='*', color='green')
-    plt.xlabel(f'{col_names[0]} of latent space')
-    plt.ylabel(f'{col_names[1]} of latent space')
-    if result_file is not None:
-        plt.savefig(result_file, dpi=200)
-    plt.close()
+import os
+# import importlib
+# import umap
+import numpy as np
+import pandas as pd
+import seaborn as sns
+# import scipy.stats as stats
+import matplotlib.pyplot as plt
+# from joblib import dump, load
+from .plot_gene import compare_exp_between_group
+from ..utility import read_cancer_purity, check_dir, read_df, log2_transform, set_fig_style
+from sklearn.metrics import median_absolute_error
+# sns.set()
+# sns.set(font_scale=1.5)
+# plt.rcParams.update({'font.size': 20})
+set_fig_style()
+
+
+def plot_loss(history_df, output_dir=None, x_label='n_epoch', y_label='MSE', file_name=None):
+    """
+    :param history_df:
+    :param output_dir:
+    :param x_label:
+    :param y_label:
+    :param file_name:
+    :return:
+    """
+    # sns.set(font_scale=1.5)
+    plt.figure(figsize=(8, 6))
+    if 'loss' in history_df.columns:
+        plt.plot(history_df['epoch'], history_df['loss'], label='loss')
+    if 'val_loss' in history_df.columns:
+        plt.plot(history_df['epoch'], history_df['val_loss'], label='val_loss')
+    if 'total_loss' in history_df.columns:
+        plt.plot(history_df['epoch'], history_df['total_loss'], label='total_loss')
+    if 'val_total_loss' in history_df.columns:
+        plt.plot(history_df['epoch'], history_df['val_total_loss'], label='val_total_loss')
+    plt.legend()
+    plt.xlabel(x_label)
+    plt.ylabel(y_label.upper())
+    plt.tight_layout()
+    if output_dir:
+        if file_name is not None:
+            plt.savefig(os.path.join(output_dir, file_name), dpi=200)
+        else:
+            plt.savefig(os.path.join(output_dir, 'loss.png'), dpi=200)
+        plt.close()
+    else:
+        return plt
+
+
+def plot_corr_two_columns(df: pd.DataFrame, output_dir: str, col_name1: str = 'CPE',
+                          col_name2: str = 'cancer_cell', cancer_type: str = '', diagonal: bool = True,
+                          predicted_by: str = None, font_scale: float = 1.5, scale_exp=False, update_figures=False):
+    """
+    Plot the relation between two columns in DataFrame `df`
+
+    :param df: a dataFrame which contains CPE (cancer purity) and cancer_fraction
+
+    :param output_dir: result folder
+
+    :param col_name1: column name, such as CPE (cancer purity), x axis
+
+    :param col_name2: column name, such as cancer cell fraction (predicted cancer purity), y axis
+
+    :param cancer_type: mark x axis / y axis label
+
+    :param diagonal: if plot diagonal
+
+    :param predicted_by: model name
+
+    :param font_scale: scale font size
+
+    :param scale_exp: if scale all expression values to range [0, 10] by x_i/max(x) * 10
+
+    :param update_figures: if update figures in output_dir
+
+    :return: None
+    """
+    check_dir(output_dir)
+    result_file_path = os.path.join(output_dir, '{}_vs_predicted_{}_proportion.png'.format(col_name1, col_name2))
+    if (not os.path.exists(result_file_path)) or update_figures:
+        # sns.set(font_scale=font_scale)
+        # plt.rcParams['font.sans-serif'] = ['Arial Unicode MS']  # show Chinese characters
+        plt.figure(figsize=(8, 8))
+        df_col1 = df[col_name1].copy()
+        df_col2 = df[col_name2].copy()
+        if np.any(df_col1 > 2) and scale_exp:
+            df_col1 = df_col1 / df_col1.max() * 10
+        if np.any(df_col2 > 2) and scale_exp:
+            df_col2 = df_col2 / df_col2.max() * 10
+
+        corr = np.corrcoef(df_col1, df_col2)
+        # print(corr)
+        if np.isnan(corr[0, 1]):
+            corr[0, 1] = 0  # when all predicted cell fraction are 0, set corr to 0
+        # corr2 = stats.pearsonr(df[col_name1], df[col_name2])
+        mae = median_absolute_error(y_true=df_col1, y_pred=df_col2)
+        plt.scatter(df_col1, df_col2, s=8)
+        plt.xlabel('{} ({})'.format(col_name1, cancer_type))
+        # plt.xlabel('{} (头颈癌)'.format(col_name1))
+        # plt.ylabel('预测 {} 比例 (样本数={})'.format(col_name2, df.shape[0]))
+        x_left, x_right = plt.xlim()
+        y_bottom, y_top = plt.ylim()
+        if '_true' in col_name2:
+            plt.ylabel('{} prop. (n={})'.format(col_name2, df.shape[0]))
+        elif predicted_by:
+            plt.ylabel('Predicted {} prop. by {} (n={})'.format(col_name2, predicted_by, df.shape[0]))
+            # plt.ylabel('{}预测值 (样本数={})'.format(predicted_by, df.shape[0]))
+        else:
+            plt.ylabel('{} prop. (n={})'.format(col_name2, df.shape[0]))
+        if 'CPE' in [col_name1, col_name2]:
+            plt.text(0.05, 0.95, 'corr = {:.3f}'.format(corr[0, 1]))
+            plt.text(0.05, 0.90, '$MAE$ = {:.3f}'.format(mae))
+        elif ('CD8A' in [col_name1, col_name2]) or ('CD8A+CD8B' in [col_name1, col_name2]):
+            plt.text(x_left + 1.5, y_top * 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
+        elif 'CD3E' in [col_name1, col_name2]:
+            plt.text(x_left + 1.5, y_top * 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
+        elif 'y_pred' in [col_name1, col_name2]:
+            plt.text(0.2, 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
+            plt.text(0.2, 0.85, '$MAE$ = {:.3f}'.format(mae))
+            # plt.title()
+        elif '_true' in col_name1 or '_true' in col_name2:
+            plt.text(0.1, 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
+            plt.text(0.1, 0.85, '$MAE$ = {:.3f}'.format(mae))
+        elif ('_marker_mean' in col_name1) or ('_marker_max' in col_name1):
+            # compare mean expression of marker genes and predicted cell fraction
+            plt.text(x_right * 0.05, y_top * 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
+        elif '_gene_signature_score' in col_name1:
+            # compare mean expression of marker genes and predicted cell fraction
+            plt.text(x_right * 0.05, y_top * 0.92, 'corr = {:.3f}'.format(corr[0, 1]))
+        if diagonal:
+            plt.plot([0, 1], [0, 1], linestyle='--', color='tab:gray')
+        plt.tight_layout()
+        plt.savefig(result_file_path, dpi=200)
+        plt.close('all')
+    else:
+        print(f'   Using previous figure, {result_file_path}')
+
+
+def plot_predicted_result(cell_frac_result_fp, bulk_exp_fp, cancer_type,
+                          model_name, result_dir, cancer_purity_fp: str = None,
+                          font_scale=2.0, update_figures=False):
+    """
+    Plot and evaluate predicted results of DeSide or Scaden model for TCGA data
+
+    :param cell_frac_result_fp: the file path of predicted cell fraction
+
+    :param bulk_exp_fp: the file path of bulk cell expression profile or pd.Dataframe, TPM, gene by sample
+
+    :param cancer_type: only for naming or mark x / y label when plotting
+
+    :param model_name: model name, DeSide or Scaden
+
+    :param result_dir: where to save result
+
+    :param cancer_purity_fp: estimated tumor purity for TCGA, download from
+        Aran, D. et al., Nat Commun 6, 8971 (2015), Supplementary Data 1
+
+    :param font_scale: scale font size
+
+    :param update_figures: whether to update figures
+
+    :return: None
+    """
+    y_pred = read_df(cell_frac_result_fp)  # cell fraction, sample by cell type
+    # sep = get_sep(bulk_exp_fp)
+    bulk_exp_cpm = read_df(bulk_exp_fp)
+    # bulk_exp_cpm = log_exp2cpm(bulk_exp_log2cpm1p)
+
+    # plot CD8 T cell fraction against CD8A expression value
+    merged_df1 = y_pred.merge(bulk_exp_cpm.T, left_index=True, right_index=True)
+    plot_corr_two_columns(df=merged_df1, col_name2='CD8 T', col_name1='CD8A',
+                          predicted_by=model_name, font_scale=font_scale,
+                          output_dir=result_dir, diagonal=False, cancer_type=cancer_type, update_figures=update_figures)
+
+    if cancer_purity_fp is not None:
+        # read cancer purity file
+        cancer_purity = read_cancer_purity(cancer_purity_fp, sample_names=list(y_pred.index))
+        merged_df = y_pred.merge(cancer_purity, left_index=True, right_index=True)
+        # plot CPE vs cell fraction of cancer cell / 1-others
+        if merged_df.shape[0] > 0:
+            merged_df.to_csv(os.path.join(result_dir,
+                                          f'cancer_purity_merged_{model_name}_predicted_result.csv'))
+            plot_corr_two_columns(df=merged_df, col_name1='CPE', col_name2='Cancer Cells',
+                                  output_dir=result_dir, font_scale=font_scale,
+                                  cancer_type=cancer_type, predicted_by=model_name, update_figures=update_figures)
+            # plot_corr_two_columns(df=merged_df, col_name1='CPE', col_name2='1-others',
+            #                       output_dir=result_dir, font_scale=font_scale,
+            #                       cancer_type=cancer_type, predicted_by=model_name)
+        else:
+            print('   There is no any samples in cancer purity about this cancer type ({})'.format(cancer_type))
+    # plot cell fraction of each cell type before decon_cf
+    y_pred['labels'] = 1
+    # if 'DeSide' in model_name:
+    #     y_pred.drop(columns='Cancer Cells', inplace=True)
+    #     # remove labels and the last cell type
+    #     cell_types = sorted(y_pred.columns.to_list())
+    #     cell_types = [i for i in cell_types if i not in ['1-others', 'labels']]
+    #     cell_types = cell_types + ['1-others']
+    # else:
+    #     y_pred.drop(columns='1-others', inplace=True)
+    #     cell_types = sorted(y_pred.columns.to_list()[:-2]) + ['Cancer Cells']
+    cell_types = sorted(y_pred.columns.to_list())
+    cell_types = [i for i in cell_types if i not in ['1-others', 'labels']]
+    # cell_types =
+    print('   Cell types: ', ', '.join(cell_types))
+    compare_exp_between_group(exp=y_pred, group_list=tuple(cell_types),
+                              result_dir=result_dir, xlabel=f'Cell Type ({cancer_type})',
+                              ylabel=f'Cell prop. predicted by {model_name}',
+                              file_name='pred_cell_prop_before_decon.png', font_scale=font_scale - 0.4,
+                              xticks_rotation=50)
+
+
+def plot_paras(paras_file_path, vae_cla_model, latent_z_pos,
+               current_cell_types, sampled_sc_id_file=None, sample_id: str = None, result_file=None):
+    """
+    plot parameters of regression model (deconvolved GEP) in latent z space
+    :param paras_file_path: w, weights of regression model which represent valid GEPs for each cell type
+    :param vae_cla_model:
+    :param latent_z_pos: latent z for all training set of VAEClassifier model (encoder)
+    :param current_cell_types
+    :param sample_id: only provide if plot this sample
+    :param sampled_sc_id_file: selected single cell id for each simulated GEP
+    :param result_file:
+    """
+
+    latent_z_pos = read_df(latent_z_pos)
+    paras = read_df(paras_file_path)
+    if paras.shape[0] > paras.shape[1]:  # sample by cell type
+        paras = paras.loc[:, current_cell_types].T
+    else:
+        paras = paras.loc[current_cell_types, :]
+    paras = log2_transform(paras)
+
+    _, _, latent_z_paras, _ = vae_cla_model.encoder_predict(paras.values)
+
+    plt.figure(figsize=(8, 8))
+    plt.scatter(latent_z_pos.loc[:, 'z1'], latent_z_pos.loc[:, 'z2'], color='gray')
+    if sample_id is not None:  # the location of ground truth
+        if sampled_sc_id_file is None:
+            raise FileNotFoundError('sampled_sc_id_file should be provided with sample_id to plot this sample')
+        sampled_sc_id_file = read_df(sampled_sc_id_file)
+        current_sc_ids = sampled_sc_id_file.loc[sample_id, :].copy()
+        sc_ids = dict(zip(current_sc_ids['cell_type'], current_sc_ids['selected_cell_id']))
+        sc_id_list = [sc_ids[_] for _ in current_cell_types]
+        plt.scatter(latent_z_pos.loc[sc_id_list, 'z1'], latent_z_pos.loc[sc_id_list, 'z2'], marker='x', color='red')
+    plt.scatter(latent_z_paras[:, 0], latent_z_paras[:, 1], marker='*', color='green')
+    if result_file is not None:
+        plt.savefig(result_file, dpi=200)
+    plt.close()
+
+
+def plot_paras_all_cell_types(latent_z_paras_file, latent_z_pos_file, current_cell_types,
+                              sampled_sc_id_file=None, sample_id: str = None, result_file=None):
+    """
+    plot parameters of regression model (deconvolved GEP) in latent z space
+    :param latent_z_paras_file: latent z of all cell types which represent valid GEPs for each cell type
+        - generated by VAEDecon model (encoder), n_cell_type x latent_dim
+    :param latent_z_pos_file: latent z for all training set of VAEClassifier model (encoder)
+    :param current_cell_types:
+    :param sample_id: only provide if plot this sample
+    :param sampled_sc_id_file: selected single cell id for each simulated GEP
+    :param result_file:
+    """
+
+    latent_z_pos_file = read_df(latent_z_pos_file)
+    if type(latent_z_paras_file) == str:
+        paras = pd.read_csv(latent_z_paras_file, index_col=[0, 1])
+    else:  # pd.Dataframe
+        paras = latent_z_paras_file
+    sample_inx = [(sample_id, ct) for ct in current_cell_types]
+    latent_z_paras = paras.loc[sample_inx, :].copy()  # n_cell_type x latent_dim
+    plt.figure(figsize=(8, 8))
+    col_names = latent_z_pos_file.columns.to_list()
+    plt.scatter(latent_z_pos_file.iloc[:, 0], latent_z_pos_file.iloc[:, 1], color='gray')
+    if sample_id is not None:  # the location of ground truth
+        if sampled_sc_id_file is None:
+            raise FileNotFoundError('sampled_sc_id_file should be provided with sample_id to plot this sample')
+        if type(sampled_sc_id_file) == str:
+            sampled_sc_id_file = pd.read_csv(sampled_sc_id_file, index_col=[0, 1])
+        # sample_inx = list(zip([sample_id] * len(current_cell_types), current_cell_types))
+        current_sc_ids = sampled_sc_id_file.loc[sample_inx, 'selected_cell_id'].to_list()
+        # sc_ids = dict(zip(current_sc_ids['cell_type'], current_sc_ids['selected_cell_id']))
+        # sc_id_list = [sc_ids[_] for _ in current_cell_types]
+        plt.scatter(latent_z_pos_file.loc[current_sc_ids, col_names[0]],
+                    latent_z_pos_file.loc[current_sc_ids, col_names[1]],
+                    marker='x', color='red')
+    plt.scatter(latent_z_paras.loc[:, col_names[0]], latent_z_paras.loc[:, col_names[1]], marker='*', color='green')
+    plt.xlabel(f'{col_names[0]} of latent space')
+    plt.ylabel(f'{col_names[1]} of latent space')
+    if result_file is not None:
+        plt.savefig(result_file, dpi=200)
+    plt.close()
```

### Comparing `DeSide-1.0.1/deside/plot/plot_sample.py` & `DeSide-1.0.2/deside/plot/plot_sample.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import os
-# import seaborn as sns
-from ..utility import check_dir, set_fig_style
-import matplotlib.pyplot as plt
-# sns.set(palette='muted', font_scale=1.5)
-set_fig_style()
-
-
-def plot_sample_distribution(re_sampled_df, marker_ratio_tcga, marker_ratio_simu_bulk,
-                             cell_type, bins=10, density: bool = True, fig_dir=None, mark_name=''):
-    """
-    plot the marker ratio distribution of a single cell type in a simulated bulk cell dataset
-    :param re_sampled_df: marker ratio of each cell type after resampled
-    :param marker_ratio_tcga: marker gene ratios of each cell type in TCGA
-    :param marker_ratio_simu_bulk: marker ratio of each cell type before resampled
-    :param cell_type: current cell type
-    :param bins:
-    :param density:
-    :param fig_dir:
-    :param mark_name: only for naming .png file
-    :return:
-    """
-    if re_sampled_df is None:
-        fig, ax = plt.subplots(2, 1, sharex='col', figsize=(10, 10))
-        ax[0].hist(marker_ratio_tcga[cell_type], bins=bins, density=density, label='TCGA')
-        ax[1].hist(marker_ratio_simu_bulk[cell_type], bins=bins, density=density, label='Before sampling')
-        for j in range(2):
-            ax[j].legend(loc='upper right')
-        fig_name = f'marker_gene_ratio_{cell_type}_without_filtering{mark_name}.png'
-    else:
-        fig, ax = plt.subplots(2, 1, sharex='col', figsize=(10, 10))
-        ax[0].hist(marker_ratio_tcga[cell_type], bins=bins, density=density, label='TCGA')
-        # ax[1].hist(marker_ratio_simu_bulk[cell_type], bins=bins, density=density, label='Before sampling')
-        ax[1].hist(re_sampled_df[cell_type], bins=bins, density=density, label='After sampling')
-        for j in range(2):
-            ax[j].legend(loc='upper right')
-        fig_name = f'marker_gene_ratio_{cell_type}_with_filtering{mark_name}.png'
-
-    # add a big axis, hide frame
-    fig.add_subplot(111, frameon=False)
-    # hide tick and tick label of the big axis
-    plt.tick_params(labelcolor='none', which='both', top=False, bottom=False, left=False, right=False)
-    plt.xlabel("Marker gene ratio")
-    plt.ylabel("Density")
-    plt.title(f'Marker gene ratio of {cell_type} in simu bulk')
-    # plt.legend()
-    plt.tight_layout()
-
-    if fig_dir is not None:
-        check_dir(fig_dir)
-        plt.savefig(os.path.join(fig_dir, fig_name), dpi=200)
-    plt.close()
+import os
+# import seaborn as sns
+from ..utility import check_dir, set_fig_style
+import matplotlib.pyplot as plt
+# sns.set(palette='muted', font_scale=1.5)
+set_fig_style()
+
+
+def plot_sample_distribution(re_sampled_df, marker_ratio_tcga, marker_ratio_simu_bulk,
+                             cell_type, bins=10, density: bool = True, fig_dir=None, mark_name=''):
+    """
+    plot the marker ratio distribution of a single cell type in a simulated bulk cell dataset
+    :param re_sampled_df: marker ratio of each cell type after resampled
+    :param marker_ratio_tcga: marker gene ratios of each cell type in TCGA
+    :param marker_ratio_simu_bulk: marker ratio of each cell type before resampled
+    :param cell_type: current cell type
+    :param bins:
+    :param density:
+    :param fig_dir:
+    :param mark_name: only for naming .png file
+    :return:
+    """
+    if re_sampled_df is None:
+        fig, ax = plt.subplots(2, 1, sharex='col', figsize=(10, 10))
+        ax[0].hist(marker_ratio_tcga[cell_type], bins=bins, density=density, label='TCGA')
+        ax[1].hist(marker_ratio_simu_bulk[cell_type], bins=bins, density=density, label='Before sampling')
+        for j in range(2):
+            ax[j].legend(loc='upper right')
+        fig_name = f'marker_gene_ratio_{cell_type}_without_filtering{mark_name}.png'
+    else:
+        fig, ax = plt.subplots(2, 1, sharex='col', figsize=(10, 10))
+        ax[0].hist(marker_ratio_tcga[cell_type], bins=bins, density=density, label='TCGA')
+        # ax[1].hist(marker_ratio_simu_bulk[cell_type], bins=bins, density=density, label='Before sampling')
+        ax[1].hist(re_sampled_df[cell_type], bins=bins, density=density, label='After sampling')
+        for j in range(2):
+            ax[j].legend(loc='upper right')
+        fig_name = f'marker_gene_ratio_{cell_type}_with_filtering{mark_name}.png'
+
+    # add a big axis, hide frame
+    fig.add_subplot(111, frameon=False)
+    # hide tick and tick label of the big axis
+    plt.tick_params(labelcolor='none', which='both', top=False, bottom=False, left=False, right=False)
+    plt.xlabel("Marker gene ratio")
+    plt.ylabel("Density")
+    plt.title(f'Marker gene ratio of {cell_type} in simu bulk')
+    # plt.legend()
+    plt.tight_layout()
+
+    if fig_dir is not None:
+        check_dir(fig_dir)
+        plt.savefig(os.path.join(fig_dir, fig_name), dpi=200)
+    plt.close()
```

### Comparing `DeSide-1.0.1/deside/simulation/generate_data.py` & `DeSide-1.0.2/deside/simulation/generate_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1467 +1,1495 @@
-import os
-import gc
-import json
-import numpy as np
-import pandas as pd
-from scipy import stats
-import scanpy as sc
-from typing import Union
-from tqdm import tqdm
-import multiprocessing
-
-from joblib import dump, load
-from sklearn.utils import shuffle
-from ..utility import (create_h5ad_dataset, check_dir, cal_corr_gene_exp_with_cell_frac,
-                       ExpObj, QueryNeighbors, log2_transform, print_msg, get_cell_num,
-                       sorted_cell_types, do_pca_analysis, non_log2cpm)
-from ..utility.read_file import ReadH5AD, read_single_cell_type_dataset, ReadExp
-from ..single_cell import get_sample_id
-from ..plot import plot_pca
-
-
-def segment_generation_fraction(n_samples: int = None, max_value: int = 10000,
-                                cell_types: list = None, sample_prefix: str = None,
-                                cell_prop_prior: dict = None) -> pd.DataFrame:
-    """
-    Generate cell fraction by fixing a specific percentage (gradient) range (i.e. from 1% to 100%)
-        for each specific cell type, and n samples for each gradient of each cell type
-
-    :param n_samples: the number of samples need to generate in total
-
-    :param max_value: cell proportion will be sampled from U(0, max_value), and then scaled to [0, 1]
-
-    :param cell_types: None or a list of cell types. Using all valid cell types if None. All valid cell types can be
-        found by `list(deside.utility.cell_type2abbr.keys())`.
-
-    :param sample_prefix: only for naming
-
-    :param cell_prop_prior: the prior range of cell proportion for each cell type, {'cell_type': (0, 0.1), '': (0, 0.2), ...}
-
-    :return: generated cell fraction, sample by cell type
-    """
-    if sample_prefix is None:
-        sample_prefix = 'seg'
-
-    n_cell_type = len(cell_types)
-    # all_samples = []
-    all_samples_tmp = []
-    while len(all_samples_tmp) < n_samples:
-        frag_for_one_sample = []
-        current_max_value = max_value  # 100%
-        current_sample_valid = True
-        for j in range(n_cell_type - 1):
-            if current_max_value > 1:  # > 1 left
-                _frag = np.random.randint(current_max_value)
-                current_max_value -= _frag
-                frag_for_one_sample.append(_frag)
-            elif current_max_value == 1:  # 1 left
-                frag_for_one_sample.append(current_max_value)
-                current_max_value = 0
-            else:  # current_max_value == 0, 0 left
-                frag_for_one_sample.append(0)
-        frag_for_one_sample.append(current_max_value)  # for last fragment (0 or > 0)
-        assert np.sum(frag_for_one_sample) == max_value
-        np.random.shuffle(frag_for_one_sample)
-        # if max_value == 0:
-        #     all_samples_tmp.append(dict(zip(cell_types, frag_for_one_sample)))
-        # else:
-        #     if max_value > n_cell_type:  # the most common situation
-        #         # cell fraction equals to 0 for at least 4 cell types or none, avoid too much 0 for any cell types
-        #         if (np.sum(np.array(frag_for_one_sample) == 0) >= 4) or \
-        #                 (np.sum(np.array(frag_for_one_sample) == 0) <= 1):
-        #             current_sample_valid = True
-        #     else:   # 0 < max_value <= len(cell_types), don't check, more zeros will be included
-        #         current_sample_valid = True
-        #     if current_sample_valid:
-        frag_for_one_sample = np.array(frag_for_one_sample) / max_value  # normalize to sum to 1
-        cell_type2frag = dict(zip(cell_types, frag_for_one_sample))
-        if cell_prop_prior is not None:
-            for cell_type, frag in cell_type2frag.items():
-                # check if the cell fraction is in the prior range
-                if (frag < cell_prop_prior[cell_type][0]) or (frag > cell_prop_prior[cell_type][1]):
-                    current_sample_valid = False
-                    break
-        if current_sample_valid:
-            all_samples_tmp.append(cell_type2frag)
-        # frag_for_one_sample = np.array(frag_for_one_sample) / max_value  # normalize to decimal
-        # all_samples_tmp.append(dict(zip(cell_types, frag_for_one_sample)))
-
-    index = [sample_prefix + '_' + str(i + 1) for i in range(len(all_samples_tmp))]
-    all_samples_df = pd.DataFrame(all_samples_tmp, index=index)
-    all_samples_df = all_samples_df.loc[:, cell_types]
-    return all_samples_df.round(4)
-
-
-def seg_random_generation_fraction(n_samples: int = None, cell_types: list = None,
-                                   sample_prefix: str = None) -> pd.DataFrame:
-    """
-    Generate cell fraction by combining segment and random sampling method
-
-    :param n_samples: the number of samples need to generate in total
-
-    :param cell_types: None or a list of cell types. Using all valid cell types if None. All valid cell types can be
-        found by `list(deside.utility.cell_type2abbr.keys())`.
-
-    :param sample_prefix: only for naming
-
-    :return: generated cell fraction, sample by cell type
-    """
-    if sample_prefix is None:
-        sample_prefix = 'seg_random'
-
-    # all_samples = []
-    all_samples_tmp = []
-    while len(all_samples_tmp) < n_samples:
-        # get the first fraction
-        first_segment = np.random.rand()
-        others_fraction = np.random.rand(len(cell_types)-1)
-        # scaling sum to 1 and then rescaling to (1-first_segment)
-        others_fraction = others_fraction / others_fraction.sum() * (1 - first_segment)
-        frag_for_one_sample = np.concatenate([np.array([first_segment]), others_fraction])
-        frag_for_one_sample = frag_for_one_sample / frag_for_one_sample.sum()  # scaling again
-        np.random.shuffle(frag_for_one_sample)
-        all_samples_tmp.append(dict(zip(cell_types, frag_for_one_sample)))
-
-    index = [sample_prefix + '_' + str(i + 1) for i in range(len(all_samples_tmp))]
-    all_samples_df = pd.DataFrame(all_samples_tmp, index=index)
-    all_samples_df = all_samples_df.loc[:, cell_types]
-    # all_samples.append(current_df)
-    return all_samples_df.round(4)
-
-
-def fragment_generation_fraction(n_samples: int = None, cell_types: list = None,
-                                 sample_prefix: str = None, reference_distribution: dict = None,
-                                 bins: int = 10, minimal_prop: float = 0.005) -> pd.DataFrame:
-    """
-    Generate cell fraction by fragment sampling method
-
-    :param n_samples: the number of samples need to generate in total
-
-    :param cell_types: None or a list of cell types. Using all valid cell types if None. All valid cell types can be
-        found by `list(deside.utility.cell_type2abbr.keys())`.
-
-    :param sample_prefix: only for naming
-
-    :param reference_distribution: reference distribution for each cell type, seperated to 10 bins for [0, 1]
-        {'B Cells': [0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1], '': [], '': [], ...}
-
-    :param bins: the number of bins for each distribution
-
-    :param minimal_prop: set to 0 if less than this value
-
-    :return: generated cell fraction, sample by cell type
-    """
-    if sample_prefix is None:
-        sample_prefix = 'fragment'
-    bin_lower_edges = np.linspace(0, 1 - 1/bins, bins)  # array([0. , 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9])
-    ct2prop = {}
-    if reference_distribution is None:
-        reference_distribution = {}
-        for ct in cell_types:
-            reference_distribution[ct] = np.ones(bins) * (1 / bins)  # uniform distribution
-    for ct in cell_types:
-        # get cell proportions for each cell type
-        current_ref_dis = reference_distribution[ct]
-        current_prop = np.random.choice(bin_lower_edges, n_samples, p=current_ref_dis)  # sampling depending on ref dis
-        # lower edge + x ~ U(0, 0.1) -> [lower_edge, lower_edge + 0.1]
-        noise_for_each_prop = 0.1 * np.random.rand(n_samples)
-        current_prop += noise_for_each_prop
-        ct2prop[ct] = current_prop
-
-    index = [sample_prefix + '_' + str(i + 1) for i in range(n_samples)]
-    all_samples_df = pd.DataFrame.from_dict(ct2prop, orient='columns')
-    all_samples_df.index = index
-    # scaling sum to 1
-    all_samples_df = all_samples_df / np.sum(all_samples_df.values, axis=1).reshape(-1, 1)
-    all_samples_df[all_samples_df < minimal_prop] = 0
-    all_samples_df = all_samples_df / np.sum(all_samples_df.values, axis=1).reshape(-1, 1)  # scale again
-    all_samples_df = all_samples_df.loc[:, cell_types]
-    # all_samples.append(current_df)
-    return all_samples_df.round(4)
-
-
-def _create_fractions(n_cell_types, fixed_range: dict = None):
-    """
-    generate (pure) random fractions
-    :param n_cell_types: number of fractions to create
-    :param fixed_range: the range of cell fraction for each cell type, {'cell_type': (0, 100), '': (), ...}
-    :return: list of random fracs with the length n_cell_types
-    """
-    if (fixed_range is None) or (len(fixed_range) < n_cell_types):
-        fracs = np.random.rand(n_cell_types)  # uniform distribution over [0, 1)
-    else:
-        fracs = []
-        for cell_type, ct_range in fixed_range.items():
-            _frac = np.random.randint(ct_range[0], ct_range[1]) / 100
-            fracs.append(_frac)
-        fracs = np.array(fracs)
-    fracs_sum = np.sum(fracs)
-    fracs = np.divide(fracs, fracs_sum)
-    return fracs
-
-
-def random_generation_fraction(n_samples: int = 100, cell_types: list = (),
-                               sample_prefix: str = None, fixed_range: dict = None) -> pd.DataFrame:
-    """
-    Create pure random cell fractions, same as `Scaden`
-
-    :param n_samples: number of samples to create
-
-    :param cell_types: a list of cell types
-
-    :param sample_prefix: prefix of sample names
-
-    :param fixed_range: the range of cell fraction for each cell type, {'cell_type': (0, 100), '': (), ...}
-
-    :return:  generated cell fraction, sample by cell type
-    """
-    if sample_prefix is None:
-        sample_prefix = 's_random'
-    n_cell_types = len(cell_types)
-    id2cell_frac = {}
-
-    for i in range(n_samples):
-        sample_name = sample_prefix + '_' + str(i)
-        id2cell_frac[sample_name] = _create_fractions(n_cell_types, fixed_range=fixed_range)
-    generated_frac_df = pd.DataFrame.from_dict(id2cell_frac, orient='index', columns=cell_types)
-    return generated_frac_df.round(2)
-
-
-def map_cell_id2exp(sc_exp, selected_cell_id):
-    """
-
-    :param sc_exp: a AnnData object, log2(CPM + 1), samples by genes
-    :param selected_cell_id: a dataFrame which contains cell_type, n_cell, selected_cell_id
-    :return: a DataFrame, log2(CPM + 1), samples by genes
-    """
-    # sc_exp = an.read_h5ad(sc_exp)
-    adata_df = pd.DataFrame(sc_exp.X.A, index=sc_exp.obs.index, columns=sc_exp.var.index)
-    adata_df = np.power(2, adata_df) - 1  # convert to non-log values
-    simulated_exp = {}
-
-    for sample_id, group in selected_cell_id.groupby(by=selected_cell_id.index):
-        cell_ids = []
-        for i, row in group.iterrows():
-            if row['n_cell'] > 0:
-                cell_ids += row['selected_cell_id'].split(';')
-        current_merged = adata_df.loc[cell_ids, :].copy()
-        simulated_exp[sample_id] = current_merged.mean(axis=0)  # single simulated bulk expression profile
-
-    simulated_exp_df = pd.DataFrame.from_dict(data=simulated_exp, orient='index')
-    # simu_adata = an.AnnData(simulated_exp_df)
-    # simu_adata.X = np.log2(simu_adata.X + 1)  # log2(CPM + 1)
-    # simulated_exp_df.rename(index={i: j for i, j in enumerate(filtered_single_cell_exp.index)}, inplace=True)
-    log2cpm = np.log2(simulated_exp_df.values + 1)
-    return pd.DataFrame(log2cpm, index=simulated_exp_df.index, columns=sc_exp.var.index).round(2)
-
-
-# def simulate_bulk_expression(cell_frac: pd.DataFrame, sc_exp_file_path: str,
-#                              n_threads: int = 2, result_dir=None,
-#                              prefix='simu_bulk_exp', step_size: int = 201, total_cell_number: int = 500):
-#     """
-#     Mix single cell expression profile to simulated bulk expression profile according to `cell_frac`. at large scale
-#
-#     :param cell_frac: dataFrame, generated cell fraction for each cell type, samples by cell types
-#
-#     :param sc_exp_file_path: string, .h5ad file, single cell n5000 dataset, log2(CPM + 1)
-#         the file path of single cell expression profiles classified by cell types
-#
-#     :param n_threads: how many thread to use
-#
-#     :param result_dir:
-#
-#     :param prefix: only for naming output files
-#
-#     :param step_size: separate to multiple steps when memory is not enough
-#
-#     :param total_cell_number: N, the total number of cells in single cell dataset
-#                               averagedd to simulate a single bulk RNA-seq sample
-#
-#     :return: simulated bulk expression profiles, sample by gene, log2(CPM + 1), .h5ad file
-#     """
-#
-#     # cell_type2sample_name
-#     # single cell dataset, .h5ad file, samples by genes, log2(CPM + 1)
-#     cell_num = get_cell_num(cell_type_frac=cell_frac, total_num=total_cell_number)
-#     sc_exp = sc.read_h5ad(sc_exp_file_path)
-#     obs_df = sc_exp.obs
-#     # adata_df = pd.DataFrame(sc_exp.X.A, index=sc_exp.obs.index, columns=sc_exp.var.index)
-#     # adata_df = np.power(2, adata_df) - 1  # convert to non-log values
-#     print('   Start to select cells randomly based on cell types for generating each bulk expression profile...')
-#     selected_cell_id = []
-#     # step = 201
-#     n_parts = cell_frac.shape[0] // step_size
-#     for inx in tqdm(range(n_parts+1)):
-#         if inx == n_parts:
-#             current_part = cell_num.iloc[inx * step_size:, :]
-#             if current_part.shape[0] == 0:
-#                 break
-#         else:
-#             # continue
-#             current_part = cell_num.iloc[inx * step_size: (inx + 1) * step_size, :]
-#         current_part_flatten = []
-#         for cell_type in current_part.columns:
-#             _part = pd.DataFrame(index=current_part.index)
-#             _part['cell_type'] = cell_type
-#             _part['n_cell'] = current_part[cell_type]
-#             current_part_flatten.append(_part)
-#         current_part_flatten = pd.concat(current_part_flatten)
-#         # contains all cell types for each single simulated bulk expression
-#         paras = [(obs_df, 1, row['cell_type'], row['n_cell'], 'cell_type')
-#                  for i, row in current_part_flatten.iterrows()]
-#         # https://pythonspeed.com/articles/python-multiprocessing/
-#         with multiprocessing.get_context('spawn').Pool(n_threads) as p:
-#             results = p.starmap(get_sample_id, paras)
-#         # print(results)
-#         results_str = [';'.join(i) for i in results]
-#         current_part_flatten['selected_cell_id'] = results_str
-#         current_part_flatten.sort_index(inplace=True)
-#         if result_dir is not None:
-#             current_exp = map_cell_id2exp(sc_exp=sc_exp, selected_cell_id=current_part_flatten)
-#             cell_id_fp = os.path.join(result_dir, prefix + '_selected_cell_id.csv')
-#             exp_fp = os.path.join(result_dir, prefix + '_log2cpm1p.csv')
-#             if not os.path.exists(cell_id_fp):
-#                 current_part_flatten.to_csv(cell_id_fp)
-#             else:
-#                 current_part_flatten.to_csv(cell_id_fp, header=False, mode='a')
-#             if not os.path.exists(exp_fp):
-#                 current_exp.to_csv(exp_fp)
-#             else:
-#                 current_exp.to_csv(exp_fp, header=False, mode='a')
-#             gc.collect()
-#         else:
-#             selected_cell_id.append(current_part_flatten)
-#
-#     if selected_cell_id:
-#         selected_cell_df = pd.concat(selected_cell_id)
-#         return selected_cell_df
-
-
-class BulkGEPGenerator(object):
-    def __init__(self, simu_bulk_dir, merged_sc_dataset_file_path, sct_dataset_file_path,
-                 cell_types: list, sc_dataset_ids: list, bulk_dataset_name: str = None,
-                 check_basic_info: bool = True, zero_ratio_threshold: float = 0.97,
-                 sc_dataset_gep_type: str = 'log_space', tcga2cancer_type_file_path: str = None):
-        """
-        :param simu_bulk_dir: the directory to save simulated bulk cell GEPs
-        :param merged_sc_dataset_file_path: the file path of pre-merged single cell datasets
-        :param cell_types: cell types used when generating bulk GEPs
-        :param sc_dataset_ids: single cell datasets used when generating bulk GEPs
-        :param bulk_dataset_name: the name of generated bulk dataset, only for naming
-        """
-        self.simu_bulk_dir = simu_bulk_dir  # result dir
-        check_dir(simu_bulk_dir)
-        self.merged_sc_fp = merged_sc_dataset_file_path
-        self.cell_type_in_sc = None  # cell types in merged single cell datasets
-        self.dataset_in_sc = None  # single cell datasets were merged together
-        self.cell_type_used = cell_types
-        self.sc_dataset_used = sc_dataset_ids
-        self.merged_sc_dataset = None
-        self.generated_sc_fp = None  # the file path of generated single cell dataset
-        # self.generated_sc_dataset = None
-        self.generated_sc_dataset_obs = None
-        self.generated_sc_dataset_df = None  # CPM GEPs of generated single cell dataset
-        self.bulk_dataset_name = bulk_dataset_name
-        self.n_samples = None  # the number of generated bulk cell GEPs
-        self.generated_bulk_gep = None
-        # self.generated_bulk_gep_fp = None  # .h5ad file path of generated bulk GEPs, log2(TPM+1)
-        self.generated_bulk_gep_counter = 0
-        self.n_round = 0
-        self.generated_cell_frac = None
-        self.total_cell_number = None  # N, average to form a bulk GEP
-        self.q_dis_nn_ref_upper: float = 0  # the quantile of distance for each pair in reference dataset, such as TCGA
-        self.q_dis_nn_ref_lower: float = 0  # the quantile of distance for each pair in reference dataset, such as TCGA
-        self.filtering_quantile_upper = 0  # the upper quantile used to determine q_dis_nn_ref for sample filtering
-        self.filtering_quantile_lower = None  # the lower quantile used to determine q_dis_nn_ref for sample filtering
-        self.marker_ratio_ref = None  # the marker gene ratios of reference dataset
-        prefix = f'simu_bulk_exp_{self.bulk_dataset_name}'
-        self.generated_cell_fraction_fp = os.path.join(self.simu_bulk_dir,
-                                                       f'generated_frac_{self.bulk_dataset_name}.csv')
-        self.ref_neighbor_counter_fp = os.path.join(self.simu_bulk_dir, f'ref2n_neighbors_{self.bulk_dataset_name}.csv')
-        self.generated_bulk_gep_csv_fp = os.path.join(self.simu_bulk_dir, prefix + f'_log2cpm1p.csv')
-        self.sampled_sc_cell_id_file_path = os.path.join(self.simu_bulk_dir, prefix + '_sampled_sc_cell_id.csv')
-        self.generated_bulk_gep_fp = self.generated_bulk_gep_csv_fp.replace('.csv', '.h5ad')  # final result
-        self.n_neighbors_each_ref = 1  # control the distribution of marker ratio by reference dataset
-        self.ref_neighbor_counter = {}
-        self.merged_sc_dataset_obs = None
-        self.merged_sc_dataset_df = None  # CPM GEPs of merged single cell dataset
-        self.obs_df = None  # used for sampling
-        self.sct_dataset_df = None  # only used in subclass "BulkGEPGeneratorSCT"
-        self.zero_ratio_threshold = zero_ratio_threshold
-        self.sct_dataset_file_path = sct_dataset_file_path
-        self.sct_dataset_obs = None
-        self.m_gep_ref = None  # median / mean GEP of reference dataset
-        # unique expression values in scRNA-seq dataset saved in merged_7_sc_dataset_log2cpm1p.h5ad
-        self.unique_exp_value_in_s0 = None  # {'cell_type1': {'gene1': np.array([]), ...}, 'cell_type2': {}, ...}
-        self.sc_dataset_gep_type = sc_dataset_gep_type
-        self.tcga2cancer_type_file_path = tcga2cancer_type_file_path
-        if check_basic_info and not os.path.exists(self.generated_bulk_gep_fp):
-            self.check_basic_info()
-
-    def _generate_cell_fraction(self, sampling_method: str, n_cell_frac: int, sampling_range: dict = None,
-                                sample_prefix: str = None, ref_distribution: dict = None,
-                                random_n_cell_type: list = None, cell_prop_prior: dict = None):
-        """
-        generate cell proportions for each simulated bulk GEP
-        :param sampling_method: 'segment' or 'random'
-        :param n_cell_frac: the number of GEPs to generate
-        :param sampling_range: the range of sampling, such as {'cell_type1': [0.1, 0.9], 'cell_type2': [0.1, 0.9], ...}
-        :param sample_prefix: the prefix of sample name, such as 'sample1', 'sample2', ...
-        :param ref_distribution: the reference distribution of cell fractions, such as {'cell_type1': [0.1, 0.2, 0.3], ...}
-        :param random_n_cell_type: the number of cell types to randomly select from reference distribution
-        :param cell_prop_prior: the prior of cell proportions, such as {'cell_type1': 0.1, 'cell_type2': 0.2, ...}
-        """
-        if sampling_method == 'segment':
-            gen_cell_fracs = segment_generation_fraction(n_samples=n_cell_frac,
-                                                         max_value=10000,
-                                                         sample_prefix=sample_prefix,
-                                                         cell_types=self.cell_type_used,
-                                                         cell_prop_prior=cell_prop_prior)
-
-        elif sampling_method == 'seg_random':
-            gen_cell_fracs = seg_random_generation_fraction(n_samples=n_cell_frac,
-                                                            sample_prefix=sample_prefix,
-                                                            cell_types=self.cell_type_used)
-
-        elif sampling_method == 'fragment':
-            if random_n_cell_type is None:
-                gen_cell_fracs = fragment_generation_fraction(n_samples=n_cell_frac,
-                                                              sample_prefix=sample_prefix,
-                                                              cell_types=self.cell_type_used,
-                                                              reference_distribution=ref_distribution)
-            else:
-                gen_cell_frac_list = []
-                n_sample_for_each_n_cell_type = int(n_cell_frac / len(random_n_cell_type))
-                for n_cell_type in random_n_cell_type:
-                    if 2 <= n_cell_type <= len(self.cell_type_used):
-                        cell_types = self.cell_type_used[:n_cell_type]  # generate by fixed cell types, then shuffle
-                        _gen_cell_fracs = fragment_generation_fraction(n_samples=n_sample_for_each_n_cell_type,
-                                                                       sample_prefix=f'{sample_prefix}_{n_cell_type}',
-                                                                       cell_types=cell_types,
-                                                                       reference_distribution=ref_distribution)
-                        gen_cell_frac_list.append(_gen_cell_fracs)
-                    else:
-                        raise ValueError(f'All numbers in "random_n_cell_type" should be >= 2 and '
-                                         f'<= the number of used cell types,  {n_cell_type} got.')
-                gen_cell_fracs_total = pd.concat(gen_cell_frac_list)
-                gen_cell_fracs_total = gen_cell_fracs_total.fillna(0)
-                # shuffle_inx = np.zeros(gen_cell_fracs.shape, dtype=np.int16)
-                inx2cell_frac = {}
-                for i in range(gen_cell_fracs_total.shape[0]):
-                    shuffle_inx = shuffle(np.arange(gen_cell_fracs_total.shape[1]))
-                    inx2cell_frac[i] = gen_cell_fracs_total.values[i, shuffle_inx]  # shuffle each row
-                gen_cell_fracs = pd.DataFrame.from_dict(inx2cell_frac, orient='index',
-                                                        columns=gen_cell_fracs_total.columns)
-                gen_cell_fracs.index = gen_cell_fracs_total.index
-
-        elif sampling_method == 'random':
-            if sampling_range is not None:
-                # gradient_range = sampling_range.copy()
-                if len(sampling_range) < len(self.cell_type_used):
-                    print('   * Since the length of gradient_range is less than cell types, gradient range '
-                          'will not be used. Instead, [0, 1] range will be used for all cell types...')
-                    sampling_range = None
-            gen_cell_fracs = random_generation_fraction(n_samples=n_cell_frac, cell_types=self.cell_type_used,
-                                                        sample_prefix=sample_prefix,
-                                                        fixed_range=sampling_range)
-        else:
-            raise ValueError(
-                f'Only "segment" and "random" were supported for parameter "sampling_method", '
-                f'{sampling_method} is invalid')
-        return gen_cell_fracs
-
-    def generate_gep(self, n_samples, sampling_range: dict = None, sampling_method: str = 'segment',
-                     total_cell_number: int = 100, n_threads: int = 10, filtering: bool = True,
-                     reference_file: Union[str, pd.DataFrame] = None, ref_exp_type: str = None,
-                     gep_filtering_quantile: tuple = (None, 0.95), log_file_path: str = None,
-                     n_top: int = 20, simu_method='mul', filtering_method='media_gep',
-                     add_noise: bool = False, noise_params: tuple = (), filtering_ref_types: list = None,
-                     show_filtering_info: bool = False, cell_prop_prior: dict = None,
-                     high_corr_gene_list: list = None, filtering_by_gene_range: bool = False,
-                     min_percentage_within_gene_range: float = 0.95, gene_quantile_range: list = None):
-        """
-        :param n_samples: the number of GEPs to generate
-        :param total_cell_number: N, the total number of cells sampled from merged single cell dataset
-                                      and averaged to simulate a single bulk RNA-seq sample
-        :param sampling_method: segment or random, method to generate cell fractions
-        :param sampling_range:
-        :param n_threads: number of threads used for parallel computing
-        :param filtering: whether filtering generated GEPs
-        :param reference_file: the file path of reference dataset for filtering
-        :param ref_exp_type: the type of expression values in reference dataset, TPM / log_space
-        :param gep_filtering_quantile: quantile of nearest distance of each pair in reference,
-            smaller quantile gives smaller radius and fewer simulated GEPs will be kept
-        :param log_file_path:
-        :param n_top: if too many neighbors were founded for one single sample, only keep n_top neighbors,
-            used in marker ratio filtering
-        :param simu_method: the method to generate simulated bulk GEPs,
-            ave (average all selected single cell GEPs), mul (multiple GEP by cell fractions)
-        :param filtering_method: marker_ratio (l2 distance with marker gene ratio) or
-            median_gep (l1 distance with median expression value for each gene)
-        :param add_noise: whether add noise to generated bulk GEPs
-        :param noise_params: parameters for noise generation, (f, max_sum),
-            ref: Hao, Yuning, et al. PLoS Computational Biology, 2019
-        :param filtering_ref_types: the cancer types used for filtering
-        :param show_filtering_info: whether show filtering information
-        :param cell_prop_prior: a prior range of cell proportions for each cell type in solid tumors
-        :param high_corr_gene_list: a list of genes that the expression values have high correlation with
-            the cell proportions for at least one cell type
-        :param filtering_by_gene_range: whether filtering GEPs by gene expression range,
-            the percentage of genes within a specific quantile range in TCGA
-        :param min_percentage_within_gene_range: the minimal percentage of genes within a specific quantile range in TCGA
-        :param gene_quantile_range: the quantile range of gene expression values in TCGA for gene based filtering
-        """
-        n_total_cpus = multiprocessing.cpu_count()
-        n_threads = min(n_total_cpus - 1, n_threads)
-        self.n_samples = n_samples
-        self.total_cell_number = total_cell_number
-        self.filtering_quantile_lower, self.filtering_quantile_upper = gep_filtering_quantile
-        # print(f'   > filtering quantile is {self.filtering_quantile * 100}%')
-        # simulating bulk cell GEP by mixing GEPs of different cell types
-        if filtering:
-            min_n_cell_frac = np.min([5000, n_samples])  # bigger number of samples for filtering
-        else:
-            min_n_cell_frac = np.min([1000, n_samples])  # smaller number of samples without filtering
-        if not os.path.exists(self.generated_bulk_gep_fp):
-            # read generated single cell dataset into self.generated_sc_dataset
-            self.check_intermediate_generated_gep()
-            # using merged single cell dataset directly
-            obs_df = self.merged_sc_dataset_obs
-            sc_dataset = 'merged_sc_dataset'
-            gene_list_in_sc_ds = []
-            if (self.merged_sc_fp is None) and (self.sct_dataset_file_path is None):
-                raise FileNotFoundError('Either "merged_sc_dataset_file_path" or '
-                                        '"sct_dataset_file_path" should be provided')
-            if (self.merged_sc_fp is not None) and (self.merged_sc_dataset_df is None):
-                if self.sc_dataset_gep_type == 'log_space':
-                    self.merged_sc_dataset_df = ReadH5AD(self.merged_sc_fp).get_df(convert_to_tpm=True)
-                else:  # non log space
-                    self.merged_sc_dataset_df = ReadH5AD(self.merged_sc_fp).get_df()
-                gene_list_in_sc_ds = self.merged_sc_dataset_df.columns.to_list()
-            if simu_method == 'mul':  # mul, using either merged_sc_dataset or sct_dataset
-                self.total_cell_number = 1  # only 1 sample for each cell type
-                if (self.sct_dataset_file_path is not None) and (self.sct_dataset_df is None):
-                    self.sct_dataset_obs, self.sct_dataset_df = self.read_sct_dataset()
-                    sc_dataset = 'sct_dataset'
-                    obs_df = self.sct_dataset_obs
-                    gene_list_in_sc_ds = self.sct_dataset_df.columns.to_list()
-            if sc_dataset == 'merged_sc_dataset':
-                min_n_cell_frac = 300  # since some cell types only have a small number of cells
-            # n_round = 0
-            sample_id_for_filtering = []
-            tcga_gene_info = None
-            exp_ref_df = None
-            if filtering and filtering_ref_types is not None:
-                s2c = pd.read_csv(self.tcga2cancer_type_file_path, index_col=0)  # sample id to cancer type in TCGA
-                sample_id_for_filtering = s2c.loc[s2c['cancer_type'].isin(filtering_ref_types), :].index.to_list()
-                _str = ', '.join(filtering_ref_types)
-                print(f'   > {len(sample_id_for_filtering)} samples in {_str} are used '
-                      f'for {filtering_method} filtering.')
-            if not filtering:
-                cell_prop_prior = None
-            with tqdm(total=self.n_samples) as pbar:
-                if self.generated_bulk_gep_counter != 0:
-                    pbar.update(self.generated_bulk_gep_counter)
-                while self.generated_bulk_gep_counter < self.n_samples:
-                    generated_cell_frac = self._generate_cell_fraction(
-                        sampling_method=sampling_method, n_cell_frac=min_n_cell_frac,
-                        sampling_range=sampling_range, sample_prefix=f's_{sampling_method}_{self.n_round}',
-                        cell_prop_prior=cell_prop_prior)
-                    # setting step_size equals to n_cell_frac, so n_parts equals to 1
-                    selected_cell_ids = self._sc_sampling(cell_frac=generated_cell_frac,
-                                                          n_threads=n_threads, obs_df=obs_df)
-                    simulated_gep = self._map_cell_id2exp(selected_cell_id=selected_cell_ids,
-                                                          simu_method=simu_method,
-                                                          sc_dataset=sc_dataset,
-                                                          cell_frac=generated_cell_frac,
-                                                          add_noise=add_noise, noise_params=noise_params)
-                    if filtering:
-                        if reference_file is None or ref_exp_type is None:
-                            raise ValueError('Both "reference_file" and "ref_exp_type" should not be None '
-                                             'when "filtering" is True')
-                        if high_corr_gene_list is not None:
-                            assert np.all([i in gene_list_in_sc_ds for i in high_corr_gene_list])
-                            gene_list_in_sc_ds = high_corr_gene_list
-                            print(f'   > {len(gene_list_in_sc_ds)} high corr genes are used for filtering.')
-                            simulated_gep = simulated_gep.loc[:, gene_list_in_sc_ds]
-                            simulated_gep = non_log2cpm(simulated_gep)
-                        if exp_ref_df is None:
-                            exp_obj_ref = ExpObj(exp_file=reference_file, exp_type=ref_exp_type)
-                            exp_obj_ref.align_with_gene_list(gene_list=gene_list_in_sc_ds, fill_not_exist=True)
-                            exp_ref_df = exp_obj_ref.get_exp()
-                            exp_ref_df = exp_ref_df.loc[exp_ref_df.index.isin(sample_id_for_filtering), :]
-
-                    if filtering and filtering_method == 'marker_ratio':
-                        # print('   Filtering simulated bulk cell GEPs by marker gene ratio of TCGA...')
-                        if self.marker_ratio_ref is None:
-                            exp_obj_ref = ExpObj(exp_file=reference_file, exp_type=ref_exp_type)
-                            exp_obj_ref.cal_marker_gene_ratio(agg_methods={'CD4 T': 'max', 'B Cells': 'max'},
-                                                              cell_types=self.cell_type_used, show_marker_gene=True)
-                            self.marker_ratio_ref = exp_obj_ref.get_marker_ratios()
-                            n_ref = self.marker_ratio_ref.shape[0]
-                            if n_ref < self.n_samples:
-                                # skip some reference samples (1000) since non-epithelial cancers exist
-                                self.n_neighbors_each_ref = int(np.ceil(self.n_samples / (n_ref - 1000)))
-                            if not self.ref_neighbor_counter:
-                                self.ref_neighbor_counter = {i: 0 for i in self.marker_ratio_ref.index}
-                            n_top = min(n_top, self.n_neighbors_each_ref)
-
-                        simulated_gep = self.filter_gep_by_reference(simulated_gep=simulated_gep,
-                                                                     n_top=n_top)
-                        if (simulated_gep is None) or (simulated_gep.shape[0] < 50):
-                            if self.filtering_quantile_upper < 0.999:
-                                # larger filtering_quantile to get more neighbors
-                                self.filtering_quantile_upper += 0.001
-                            else:
-                                self.filtering_quantile_upper += 0.0001
-                            qn1 = QueryNeighbors(df_file=self.marker_ratio_ref)
-                            self.q_dis_nn_ref_upper = qn1.get_quantile_of_nn_distance(
-                                quantile=self.filtering_quantile_upper)  # quantile of distance
-                            print(f'   > Larger filtering_quantile will be used to get more neighbors.')
-                            print(f'   > Quantile distance of {self.filtering_quantile_upper * 100}% is: {self.q_dis_nn_ref_upper}')
-                    if filtering and filtering_by_gene_range:
-                        if tcga_gene_info is None:
-                            if gene_quantile_range is None:
-                                quantile_range = [0.005, 0.5, 0.995]
-                            else:
-                                quantile_range = gene_quantile_range
-                            q_col_name = ['q_' + str(int(q * 1000) / 10) for q in quantile_range]
-                            tcga_gene_info = get_quantile(exp_ref_df, quantile_range=quantile_range,
-                                                          col_name=q_col_name)
-                        valid_gep_list = []
-                        for inx, row in simulated_gep.iterrows():
-                            valid = True
-                            current_gene_list = \
-                                get_gene_list_filtered_by_quantile_range(bulk_exp=row, tcga_exp=exp_ref_df,
-                                                                         tcga_gene_info=tcga_gene_info,
-                                                                         quantile_range=quantile_range,
-                                                                         q_col_name=q_col_name)
-                            if len(current_gene_list) / exp_ref_df.shape[1] < min_percentage_within_gene_range:
-                                valid = False
-                            valid_gep_list.append(valid)
-                        if show_filtering_info:
-                            print(f'   > {np.sum(valid_gep_list)} were kept after filtering by gene range.')
-                        simulated_gep = simulated_gep.loc[valid_gep_list, :].copy()
-
-                    if filtering and (filtering_method == 'median_gep' or
-                                      filtering_method == 'mean_gep') and (simulated_gep is not None):
-                        if self.m_gep_ref is None:
-                            if filtering_method == 'median_gep':
-                                self.m_gep_ref = exp_ref_df.median(axis=0).values.reshape(1, -1)  # TPM
-                            elif filtering_method == 'mean_gep':
-                                self.m_gep_ref = exp_ref_df.mean(axis=0).values.reshape(1, -1)
-                            else:
-                                raise ValueError(f'filtering_method {filtering_method} is invalid')
-                            l1_distance_with_center_ref = np.linalg.norm(exp_ref_df - self.m_gep_ref,
-                                                                         ord=1, axis=1)
-                            self.q_dis_nn_ref_upper = np.quantile(l1_distance_with_center_ref,
-                                                                  self.filtering_quantile_upper)
-                        assert np.all(exp_ref_df.columns == simulated_gep.columns)
-
-                        l1_dis_ref_simu_gep = np.linalg.norm(simulated_gep.values - self.m_gep_ref, ord=1, axis=1)
-                        if self.filtering_quantile_lower is not None:
-                            self.q_dis_nn_ref_lower = np.quantile(l1_distance_with_center_ref,
-                                                                  self.filtering_quantile_lower)
-                            if show_filtering_info:
-                                print(f'   > Quantile distance of {self.filtering_quantile_lower * 100}% is: '
-                                      f'{self.q_dis_nn_ref_lower}, {np.sum(l1_dis_ref_simu_gep < self.q_dis_nn_ref_lower)} were removed')
-                                print(f'   > Quantile distance of {self.filtering_quantile_upper * 100}% is: '
-                                      f'{self.q_dis_nn_ref_upper}, {np.sum(l1_dis_ref_simu_gep > self.q_dis_nn_ref_upper)} were removed')
-                            simulated_gep = simulated_gep.loc[(l1_dis_ref_simu_gep <= self.q_dis_nn_ref_upper) &
-                                                              (l1_dis_ref_simu_gep >= self.q_dis_nn_ref_lower), :]
-                        else:
-                            simulated_gep = simulated_gep.loc[l1_dis_ref_simu_gep <= self.q_dis_nn_ref_upper, :].copy()
-
-                    if simulated_gep is not None:
-                        if (self.generated_bulk_gep_counter + simulated_gep.shape[0]) > self.n_samples:
-                            n_last_part = self.n_samples - self.generated_bulk_gep_counter
-                            simulated_gep = simulated_gep.iloc[range(n_last_part)].copy()
-                        simulated_gep = log2_transform(simulated_gep)
-                        self.generated_bulk_gep_counter += simulated_gep.shape[0]
-                        pbar.update(simulated_gep.shape[0])
-                        generated_cell_frac = generated_cell_frac.loc[simulated_gep.index, :].copy()
-                        selected_cell_ids = selected_cell_ids.loc[simulated_gep.index, :].copy()
-                        self._save_simulated_bulk_gep(gep=simulated_gep, cell_id=selected_cell_ids,
-                                                      cell_fraction=generated_cell_frac)
-                    self.n_round += 1
-            msg = f'   > Got {self.generated_bulk_gep_counter} samples from {self.n_round * min_n_cell_frac}'
-            if sampling_method in ['segment', 'seg_random']:
-                q_dis = 'radius' if filtering_method == 'marker_ratio' else 'l1 distance'
-                if self.q_dis_nn_ref_lower is not None:
-                    msg = f'   > Got {self.generated_bulk_gep_counter} samples from {self.n_round * min_n_cell_frac} ' \
-                          f'within {q_dis} between {self.q_dis_nn_ref_lower} and {self.q_dis_nn_ref_upper} ' \
-                          f'by quantile {self.filtering_quantile_lower * 100}%-{self.filtering_quantile_upper * 100}%'
-                else:
-                    msg = f'   > Got {self.generated_bulk_gep_counter} samples from {self.n_round * min_n_cell_frac} ' \
-                          f'within {q_dis} {self.q_dis_nn_ref_upper} by quantile {self.filtering_quantile_upper * 100}%'
-            print(msg)
-            data_info = f'Simulated {self.generated_bulk_gep_counter} bulk cell gene expression profiles ' \
-                        f'by {sampling_method}, log2(TPM + 1)'
-            create_h5ad_dataset(simulated_bulk_exp_file_path=self.generated_bulk_gep_csv_fp,
-                                cell_fraction_file_path=self.generated_cell_fraction_fp,
-                                dataset_info=data_info,
-                                result_file_path=self.generated_bulk_gep_fp)
-            if log_file_path is not None:
-                obj_info = self.__str__()
-                print_msg(obj_info, log_file_path=log_file_path)
-        else:
-            print(f'   Previous result existed: {self.generated_bulk_gep_fp}')
-            print(self.__str__())
-
-    def filter_gep_by_reference(self, simulated_gep, n_top: int = None) -> Union[pd.DataFrame, None]:
-        """
-        filter generated GEP by reference dataset, such as TCGA
-        :param simulated_gep: simulated GEPs that need to filter by reference, TPM
-        :param n_top: if too many neighbors were founded for one single sample, only keep n_top neighbors
-        """
-
-        # print(marker_ratio_ref.head(2))
-        exp_obj_simu_gep = ExpObj(exp_file=simulated_gep, exp_type='TPM')
-        exp_obj_simu_gep.cal_marker_gene_ratio(agg_methods={'CD4 T': 'max', 'B Cells': 'max'},
-                                               cell_types=self.cell_type_used)
-        marker_ratio_simu_gep = exp_obj_simu_gep.get_marker_ratios()
-
-        # the distance of nearest neighbor for each sample
-        # quantile = 0.999
-        if self.q_dis_nn_ref_upper == 0:
-            qn1 = QueryNeighbors(df_file=self.marker_ratio_ref)
-            # quantile of distance
-            self.q_dis_nn_ref_upper = qn1.get_quantile_of_nn_distance(quantile=self.filtering_quantile_upper)
-            print(f'   > Quantile distance of {self.filtering_quantile_upper * 100}% is: {self.q_dis_nn_ref_upper}')
-        # nn_dis = qn1.get_nn()
-
-        qn2 = QueryNeighbors(df_file=marker_ratio_simu_gep)
-        current_ref_nc = sorted(self.ref_neighbor_counter.items(), key=lambda x: x[1])
-        _keep_ref = [i for i, j in current_ref_nc if j < self.n_neighbors_each_ref]
-        ref_neighbors_within_radius = qn2.get_neighbors_by_radius(
-            radius=self.q_dis_nn_ref_upper, n_top=n_top, share_neighbors=False,
-            q_df_file=self.marker_ratio_ref.loc[_keep_ref, :].copy(),
-            )
-        ref2n_neighbors = ref_neighbors_within_radius.groupby(ref_neighbors_within_radius.index).count()
-        _keep_neighbors = []
-        for i, n_n in ref2n_neighbors.iterrows():
-            self.ref_neighbor_counter[i] += n_n['nn']
-        # print(f'   There are {ref_neighbors_within_radius.shape[0]} simulated GEPs left after filtering.')
-        if ref_neighbors_within_radius.shape[0] > 0:
-            return simulated_gep.loc[ref_neighbors_within_radius['nn'], :].copy()
-        else:
-            return None
-
-    def read_merged_single_cell_dataset(self):
-        if self.merged_sc_dataset is None:
-            self.merged_sc_dataset = ReadH5AD(self.merged_sc_fp).get_h5ad()
-
-    def read_generated_single_cell_dataset(self):
-        if self.generated_sc_fp is None or (not os.path.exists(self.generated_sc_fp)):
-            raise FileNotFoundError('   Please generate single cell dataset first '
-                                    'using function "generate_single_cell_dataset", and try again.')
-        generated_sc_dataset_obj = ReadH5AD(self.generated_sc_fp)
-        generated_sc_dataset = generated_sc_dataset_obj.get_h5ad()
-        self.generated_sc_dataset_obs = generated_sc_dataset.obs.copy()
-        self.generated_sc_dataset_df = generated_sc_dataset_obj.get_df(convert_to_tpm=True)
-
-    def get_info_in_merged_single_cell_dataset(self, check_zero_ratio: bool = True,
-                                               zero_ratio_threshold: float = 0.95):
-        if self.merged_sc_dataset is None:
-            self.read_merged_single_cell_dataset()
-        self.cell_type_in_sc = list(self.merged_sc_dataset.obs['cell_type'].unique())
-        self.dataset_in_sc = list(self.merged_sc_dataset.obs['dataset_id'].unique())
-        # self.merged_sc_dataset_obs = self.merged_sc_dataset.obs.copy()
-        # always removing this part: marker genes of CD4 T cells expressed high in CD8 T cells
-        self.merged_sc_dataset_obs = \
-            self.merged_sc_dataset.obs.loc[~((self.merged_sc_dataset.obs['cell_type'] == 'CD8 T')
-                                           & (self.merged_sc_dataset.obs['m_cd4/m_cd8 group'] == 'high')), :].copy()
-        self.merged_sc_dataset_obs['sample_id'] = \
-            self.merged_sc_dataset_obs['sample_id'].cat.add_categories('pan_cancer')
-        # add sample_id for pan_cancer_07 dataset to use groupby later
-        self.merged_sc_dataset_obs.loc[self.merged_sc_dataset_obs['dataset_id'] == 'pan_cancer_07',
-                                       'sample_id'] = 'pan_cancer'
-        # The unique gene expression values of each gene in different cell types (merged scRNA-seq dataset)
-        self.unique_exp_value_in_s0 = self.merged_sc_dataset.uns['unique_exp_values']
-        self.merged_sc_dataset = None
-        if check_zero_ratio:
-            if self.sc_dataset_gep_type == 'log_space':
-                self.merged_sc_dataset_df = ReadH5AD(self.merged_sc_fp).get_df(convert_to_tpm=True)
-            else:
-                self.merged_sc_dataset_df = ReadH5AD(self.merged_sc_fp).get_df()
-            zero_ratio = np.sum(self.merged_sc_dataset_df < 1, axis=1) / self.merged_sc_dataset_df.shape[1]
-            high_zero_ratio_cells = zero_ratio[zero_ratio > zero_ratio_threshold].index.to_list()
-            # remove high zero ratio cells
-            print(f'   The zero ratio of {len(high_zero_ratio_cells)} cells '
-                  f'> {zero_ratio_threshold} and will be removed.')
-            self.merged_sc_dataset_obs = self.merged_sc_dataset_obs.loc[
-                                         ~self.merged_sc_dataset_obs.index.isin(high_zero_ratio_cells), :].copy()
-
-    def _sc_sampling(self, cell_frac: pd.DataFrame, obs_df: pd.DataFrame,
-                     n_threads: int = 10, total_cell_number: int = None, sep_by_patient=False):
-        """
-        Mix single cell expression profiles to simulated bulk expression profile according to `cell_frac`.
-
-        :param cell_frac: dataFrame, generated cell fraction for each cell type, samples by cell types
-
-        :param n_threads: how many thread to use
-
-        :param obs_df: a dataFrame of sample info for sampling
-
-        :param total_cell_number: N, total cell number to sample for each simulated bulk sample
-
-        :param sep_by_patient: whether to separate samples by patient or not during sampling
-
-        :return: sampled cell_ids
-        """
-        if total_cell_number is not None:
-            self.total_cell_number = total_cell_number
-        # if self.obs_df is None:
-        #     self.obs_df = obs_df
-        cell_num = get_cell_num(cell_type_frac=cell_frac, total_num=self.total_cell_number)
-        # print('   Start to select cells randomly based on cell types for generating each bulk expression profile...')
-        # all cell types of each cell only need to select one SCT from self.obs_df
-        # all_cell_num_is_one = np.all(cell_num == 1)
-        cell_num_flatten = []
-        # n_samples = cell_frac.shape[0]
-        for cell_type in cell_num.columns:
-            _part = pd.DataFrame(index=cell_num.index)
-            _part['cell_type'] = cell_type
-            _part['n_cell'] = cell_num[cell_type]
-            # if all_cell_num_is_one:
-            #     _selected_cell_ids = self.obs_df.loc[self.obs_df['cell_type'] == cell_type,
-            #                                          :].sample(n=n_samples).index.to_list()
-            #     _part['selected_cell_id'] = _selected_cell_ids
-            cell_num_flatten.append(_part)
-        sampled_cell_ids = pd.concat(cell_num_flatten)
-        # contains all cell types for each single simulated bulk expression profile
-        # if not all_cell_num_is_one:
-        paras = [(obs_df, 1, row['cell_type'], row['n_cell'], 'cell_type', sep_by_patient)
-                 for i, row in sampled_cell_ids.iterrows()]
-        n_threads = min(multiprocessing.cpu_count()-2, n_threads)
-        # https://pythonspeed.com/articles/python-multiprocessing/
-        with multiprocessing.get_context('spawn').Pool(n_threads) as p:
-            results = p.starmap(get_sample_id, paras)
-        # print(results)
-        results_str = [';'.join(i) for i in results]
-        sampled_cell_ids['selected_cell_id'] = results_str
-        sampled_cell_ids.index.name = 'sample_id'
-        sampled_cell_ids.sort_values(by=['sample_id', 'cell_type'], inplace=True)
-
-        return sampled_cell_ids
-
-    @staticmethod
-    def sample_noise(miu=0, s=566.1, f=0.25, n_samples=10000) -> np.ndarray:
-        """
-        generate noise for each gene in one bulk GEP,
-            Modified by Hao, Yuning, et al. PLoS Computational Biology, 2019
-        miu: mean of normal distribution
-        s: the mean std of all samples in TCGA with TPM values, LGG and GBM were excluded
-        """
-        sigma = f * np.log2(s)
-        norm_dis = stats.norm(miu, sigma)
-        x = norm_dis.rvs(size=n_samples)
-        return np.power(2, x)
-
-    def _map_cell_id2exp(self, selected_cell_id, sc_dataset: str = 'merged_sc_dataset',
-                         simu_method: str = 'ave', cell_frac: pd.DataFrame = None,
-                         gep_type='MCT', add_noise: bool = False, noise_params: tuple = ()) -> pd.DataFrame:
-        """
-        mapping sampled cell_ids to the corresponding GEPs
-        :param selected_cell_id: a dataFrame which contains cell_type, n_cell, selected_cell_id
-        :param sc_dataset: merged_sc_dataset, generated_sc_dataset or sct_dataset
-        :param simu_method: ave (average all selected single cell GEPs), mul (multiple GEP by cell fractions)
-        :param gep_type: MCT means multiple cell types (bulk GEP), SCT means single cell type
-        :return: a DataFrame, TPM, samples by genes
-        """
-        if sc_dataset == 'sct_dataset':
-            sc_ds_df = self.sct_dataset_df
-        elif sc_dataset == 'merged_sc_dataset':
-            sc_ds_df = self.merged_sc_dataset_df
-        else:  # generated single cell dataset
-            sc_ds_df = self.generated_sc_dataset_df
-        simulated_exp = {}
-        if gep_type == 'SCT':  # each sample id only contains single cell type
-            selected_cell_id = selected_cell_id.loc[selected_cell_id['n_cell'] > 1, :].copy()
-            # n_non_zero = 1000
-            n_genes = sc_ds_df.shape[1]
-            for cell_type, group in selected_cell_id.groupby('cell_type'):
-                for sample_id, row in group.iterrows():
-                    cell_ids = row['selected_cell_id'].split(';')
-                    # simulated_exp[sample_id] = sc_ds_df.loc[cell_ids, :].mean(axis=0)  # average
-                    current_gene_exp = sc_ds_df.loc[cell_ids, :].mean(axis=0)  # average
-                    if simu_method == 'random_replacement':
-                        # long_tail_noise_non_zero = np.random.random(n_non_zero) * 2
-                        # n_zero = np.random.randint(n_non_zero/10, n_non_zero)
-                        # long_tail_noise = np.append(long_tail_noise_non_zero, np.zeros(n_zero))
-                        long_tail_noise = np.random.random(size=n_genes)
-                        # replace the values < 1 with random selected values
-                        mask = (current_gene_exp < 1).values.astype(int)
-                        current_gene_exp = current_gene_exp + long_tail_noise * mask
-                    simulated_exp[sample_id] = pd.Series(current_gene_exp.values, index=current_gene_exp.index)
-        else:
-            assert simu_method == 'mul', 'Only support matrix multiplication for generating MCT'
-            for sample_id, group in selected_cell_id.groupby(by=selected_cell_id.index):
-                all_n_cell_is_one = np.all(group['n_cell'] == 1)
-                assert all_n_cell_is_one, 'n_cell should be 1 for all cell types'
-                cell_ids = group['selected_cell_id'].to_list()
-                current_merged = sc_ds_df.loc[cell_ids, :].copy()
-                # using merged single cell dataset directly
-
-                # sort by cell types to make sure the correction of matrix multiplication
-                _cell_types = group['cell_type'].to_list()
-                current_cell_frac = cell_frac.loc[sample_id, _cell_types].copy().to_frame()
-                # current_cell_frac = current_cell_frac.loc[group['cell_type'].to_list(), :]
-                simulated_exp[sample_id] = pd.Series((current_merged.values.T @ current_cell_frac.values).reshape(-1),
-                                                     index=current_merged.columns)
-                if add_noise:
-                    assert len(noise_params) == 2, 'noise_params should be a tuple of (f, total_max)'
-                    noise = self.sample_noise(n_samples=len(simulated_exp[sample_id]), f=noise_params[0])
-                    if noise.sum() > noise_params[1]:
-                        noise = noise / np.sum(noise) * noise_params[1]
-                    simulated_exp[sample_id] = simulated_exp[sample_id] + noise
-
-        simulated_exp_df = pd.DataFrame.from_dict(data=simulated_exp, orient='index')
-        simulated_exp_df = non_log2cpm(simulated_exp_df, sum_exp=1e6)  # convert to TPM
-        return simulated_exp_df.round(3)
-
-    def _save_simulated_bulk_gep(self, gep: pd.DataFrame, cell_id: pd.DataFrame, cell_fraction: pd.DataFrame = None):
-
-        if not os.path.exists(self.generated_bulk_gep_csv_fp):
-            gep.to_csv(self.generated_bulk_gep_csv_fp, float_format='%g')
-        else:
-            gep.to_csv(self.generated_bulk_gep_csv_fp, header=False, mode='a', float_format='%g')
-
-        if not os.path.exists(self.sampled_sc_cell_id_file_path):
-            cell_id.to_csv(self.sampled_sc_cell_id_file_path)
-        else:
-            cell_id.to_csv(self.sampled_sc_cell_id_file_path, header=False, mode='a')
-
-        if cell_fraction is not None:
-            if not os.path.exists(self.generated_cell_fraction_fp):
-                cell_fraction.to_csv(self.generated_cell_fraction_fp, float_format='%g')
-            else:
-                cell_fraction.to_csv(self.generated_cell_fraction_fp, header=False, mode='a', float_format='%g')
-
-        if self.ref_neighbor_counter:
-            pd.DataFrame.from_dict(self.ref_neighbor_counter, orient='index').to_csv(self.ref_neighbor_counter_fp)
-
-    def check_intermediate_generated_gep(self):
-        """
-        if the generation process broke accidentally,
-        generated intermediate result can be used to recovery generation process
-        """
-        if os.path.exists(self.generated_cell_fraction_fp):
-            gen_cell_frac = pd.read_csv(self.generated_cell_fraction_fp, index_col=0)
-            gen_cell_frac = gen_cell_frac[~gen_cell_frac.index.duplicated(keep='first')].copy()
-            if os.path.exists(self.generated_bulk_gep_csv_fp):
-                gen_bulk_gep = pd.read_csv(self.generated_bulk_gep_csv_fp, index_col=0, usecols=[0, 1])
-                gen_bulk_gep = gen_bulk_gep[~gen_bulk_gep.index.duplicated(keep='first')].copy()
-                common_inx = [i for i in gen_cell_frac.index if i in gen_bulk_gep.index]
-                if (len(common_inx) == gen_bulk_gep.shape[0]) and (len(common_inx) == gen_cell_frac.shape[0]):
-                    self.generated_bulk_gep_counter = len(common_inx)
-                    if 'seg_random' in gen_cell_frac.iloc[-1].name:
-                        n_round = int(gen_cell_frac.iloc[-1].name.split('_')[3])
-                    else:
-                        n_round = int(gen_cell_frac.iloc[-1].name.split('_')[2])
-                    self.n_round = n_round + 1
-                    print(f'   The following intermediate generated result will be reused: \n'
-                          f'{self.generated_cell_fraction_fp}, {self.generated_bulk_gep_csv_fp}.\n'
-                          f'self.n_round will be reset to {self.n_round}, '
-                          f'self.generated_bulk_gep_counter will be reset to {self.generated_bulk_gep_counter}')
-                    if os.path.exists(self.ref_neighbor_counter_fp):
-                        ref2n_neighbors = pd.read_csv(self.ref_neighbor_counter_fp, index_col=0).to_dict()['0']
-                        self.ref_neighbor_counter = ref2n_neighbors.copy()
-                else:
-                    os.remove(self.generated_cell_fraction_fp)
-                    os.remove(self.generated_bulk_gep_csv_fp)
-                    os.remove(self.sampled_sc_cell_id_file_path)
-
-    def check_basic_info(self):
-        """
-        check cell types and dataset
-        """
-        self.get_info_in_merged_single_cell_dataset(zero_ratio_threshold=self.zero_ratio_threshold)
-        cell_type_not_in_sc = [i for i in self.cell_type_used if i not in self.cell_type_in_sc]
-        dataset_not_in_sc = [i for i in self.sc_dataset_used if i not in self.dataset_in_sc]
-        if len(cell_type_not_in_sc) > 0:
-            invalid_cell_types = ', '.join(cell_type_not_in_sc)
-            valid_cell_types = ', '.join(self.cell_type_in_sc)
-            raise ValueError(f'   Invalid cell types: {invalid_cell_types}, '
-                             f'only the following cell types existed in single cell dataset: {valid_cell_types}')
-        else:
-            used_cell_types = ', '.join(self.cell_type_used)
-            print(f'   The following cell types will be used: {used_cell_types}')
-
-        if len(dataset_not_in_sc) > 0:
-            invalid_datasets = ', '.join(dataset_not_in_sc)
-            valid_datasets = ', '.join(self.dataset_in_sc)
-            raise ValueError(f'   Invalid datasets: {invalid_datasets}, '
-                             f'only the following datasets existed in single cell dataset: {valid_datasets}')
-        else:
-            used_datasets = ', '.join(self.sc_dataset_used)
-            print(f'   The following datasets will be used: {used_datasets}')
-
-    def read_sct_dataset(self, latent_z_nn_info_file=None):
-        """
-        positive samples of SCT (single cell type), generated by SingleCellTypeGEPGenerator
-        :param latent_z_nn_info_file: neighbor information of latent z for all samples, used for QC
-        """
-        sct_dataset_obs, sct_dataset_df = \
-            read_single_cell_type_dataset(sct_dataset_file_path=self.sct_dataset_file_path,
-                                          latent_z_nn_info_file=latent_z_nn_info_file)
-        return sct_dataset_obs, sct_dataset_df
-
-    def __str__(self):
-        _dict = {k: v for k, v in self.__dict__.items() if type(v) in [list, str, int, float]}
-        return str(self.__class__) + ':\n' + json.dumps(_dict, indent=2)
-
-
-class SingleCellTypeGEPGenerator(BulkGEPGenerator):
-    def __init__(self, merged_sc_dataset_file_path, cell_types, sc_dataset_ids,
-                 simu_bulk_dir, bulk_dataset_name, zero_ratio_threshold: float = 0.97,
-                 sc_dataset_gep_type: str = 'log_space'):
-        super().__init__(merged_sc_dataset_file_path=merged_sc_dataset_file_path, simu_bulk_dir=simu_bulk_dir,
-                         cell_types=cell_types, sc_dataset_ids=sc_dataset_ids, bulk_dataset_name=bulk_dataset_name,
-                         zero_ratio_threshold=zero_ratio_threshold, sct_dataset_file_path=None,
-                         sc_dataset_gep_type=sc_dataset_gep_type)
-
-    def generate_samples(self, n_sample_each_cell_type: int = 10000,
-                         n_base_for_positive_samples: int = 1,
-                         sample_type: str = 'positive', sep_by_patient=False,
-                         simu_method='ave', cell_type2subgroup_id: dict = None, subgroup_by: list = None):
-        """
-        :param n_sample_each_cell_type:
-        :param n_base_for_positive_samples: the number of single cells to average
-        :param sample_type: positive means only 1 cell type is used, negative means more than 1 cell types are used
-        :param sep_by_patient: only sampling from one patient in original dataset if True
-        :param simu_method: 'ave': averaging all GEPs,
-            or 'scale_by_mGEP': scaling by the mean GEP of all samples in the TCGA dataset
-            or 'random_replacement': replacing the gene expression value (<1) by another value within the same cell type
-             selected randomly
-        :param cell_type2subgroup_id: a dict, key is cell type, value is a list of subgroup ids
-        :parma subgroup_by: a list of column names in the merged single cell dataset, used to group samples
-        """
-        if not os.path.exists(self.generated_bulk_gep_fp):
-            if subgroup_by is None:
-                subgroup_by = ['dataset_id', 'leiden']
-            self.n_samples = n_sample_each_cell_type * len(self.cell_type_used)
-            if not os.path.exists(self.generated_cell_fraction_fp):
-                print(f'   Generate cell proportions for single cell type (SCT) samples in {self.bulk_dataset_name}')
-                generated_cell_frac = self.generate_frac_sc(
-                    sample_type=sample_type, sample_prefix=f'sct_{self.bulk_dataset_name}_{sample_type[:3]}'
-                )
-                generated_cell_frac.to_csv(self.generated_cell_fraction_fp, float_format='%g')
-            else:
-                print(f'   Previous result exists: {self.generated_cell_fraction_fp}')
-            # DC has 543 cells, larger chunk_size can cause error if set 'replace=False' and 'n_base=1' while sampling
-            chunk_size_factor = max([len(v) for k, v in cell_type2subgroup_id.items()])
-            if chunk_size_factor <= 10:
-                chunk_size_factor = 10
-            elif 10 < chunk_size_factor <= 20:
-                chunk_size_factor = 20
-            elif 20 < chunk_size_factor <= 50:
-                chunk_size_factor = 50
-            chunk_size = int(n_sample_each_cell_type / chunk_size_factor)
-            # if n_base_for_positive_samples == 1:
-            #     chunk_size = 300
-            # else:
-            #     chunk_size = 1000
-            chunk_counter = 0
-            with pd.read_csv(self.generated_cell_fraction_fp, chunksize=chunk_size, index_col=0) as reader:
-                simu_method = simu_method  # average single cell GEPs for both positive and negative sampling
-                for rows in tqdm(reader):
-                    if sample_type == 'positive' and n_base_for_positive_samples > 1:
-                        total_cell_number = n_base_for_positive_samples
-                    else:  # negative sampling (multiple cell types are used) or positive sampling with n_base=1
-                        total_cell_number = 0  # assign 1 for the cell types with non-zero cell fractions
-                    if sample_type == 'positive' and cell_type2subgroup_id is not None:
-                        # change subgroup for each chunk based on cell_type2subgroup_id
-                        all_cell_types = rows.columns[np.argmax(rows.values, axis=1)].unique()
-                        if len(all_cell_types) > 1:
-                            raise ValueError(f'   More than one cell types are selected: {all_cell_types}')
-                        cell_type = all_cell_types[0]
-                        current_subgroups = cell_type2subgroup_id[cell_type]
-                        selected_subgroup = current_subgroups[chunk_counter % chunk_size_factor % len(current_subgroups)]
-                        if len(subgroup_by) == 1 and subgroup_by[0] in self.merged_sc_dataset_obs.columns:
-                            current_obs_df = self.merged_sc_dataset_obs.loc[
-                                             self.merged_sc_dataset_obs[subgroup_by[0]].isin(selected_subgroup),
-                                             :].copy()
-                        elif len(subgroup_by) == 2 and set(subgroup_by).issubset(self.merged_sc_dataset_obs.columns):
-                            current_obs_df = self.merged_sc_dataset_obs.loc[
-                                             (self.merged_sc_dataset_obs[subgroup_by[0]].isin([selected_subgroup[0]])) &
-                                             (self.merged_sc_dataset_obs[subgroup_by[1]].isin([selected_subgroup[1]])),
-                                             :].copy()
-                        else:
-                            raise ValueError(f'   subgroup_by {subgroup_by} is not valid')
-                    else:
-                        current_obs_df = self.merged_sc_dataset_obs.copy()
-                    selected_cell_ids = self._sc_sampling(cell_frac=rows, total_cell_number=total_cell_number,
-                                                          obs_df=current_obs_df,
-                                                          sep_by_patient=sep_by_patient)
-                    simulated_gep = self._map_cell_id2exp(selected_cell_id=selected_cell_ids, simu_method=simu_method,
-                                                          cell_frac=rows, sc_dataset='merged_sc_dataset', gep_type='SCT')
-                    simulated_gep = log2_transform(simulated_gep)
-                    self.generated_bulk_gep_counter += simulated_gep.shape[0]
-                    # generated_cell_frac = generated_cell_frac.loc[simulated_gep.index, :].copy()
-                    selected_cell_ids = selected_cell_ids.loc[simulated_gep.index, :].copy()
-                    self._save_simulated_bulk_gep(gep=simulated_gep, cell_id=selected_cell_ids)
-                    chunk_counter += 1
-
-            data_info = f'Simulated {self.generated_bulk_gep_counter} gene expression profiles ' \
-                        f'for each cell type, log2(TPM + 1)'
-            create_h5ad_dataset(simulated_bulk_exp_file_path=self.generated_bulk_gep_csv_fp,
-                                cell_fraction_file_path=self.generated_cell_fraction_fp,
-                                dataset_info=data_info,
-                                result_file_path=self.generated_bulk_gep_fp)
-        else:
-            print(f'   Previous result exists: {self.generated_bulk_gep_fp}')
-
-    def generate_frac_sc(self, sample_prefix: str = None, sample_type: str = 'positive') -> pd.DataFrame:
-        """
-        Generate cell fractions for single cell samples, positive samples only contain one specific cell type,
-        negative samples contain >= 2 cell types with equal proportion
-
-        :param sample_prefix: prefix of sample names
-
-        :param sample_type: positive samples (one specific cell type) or negative samples (>= 2 cell types)
-
-        :return:  generated cell fraction, sample by cell type
-        """
-        if sample_prefix is None:
-            sample_prefix = f's_sc_{sample_type}'
-        n_cell_types = len(self.cell_type_used)
-        generated_frac_df = pd.DataFrame(index=[f'{sample_prefix}_{i}' for i in range(self.n_samples)],
-                                         columns=self.cell_type_used,
-                                         data=np.zeros((self.n_samples, n_cell_types)))
-        if sample_type == 'positive':
-            n_for_each_cell_type = int(self.n_samples / n_cell_types)
-            for i, cell_type in enumerate(self.cell_type_used):
-                inx_start = i * n_for_each_cell_type
-                inx_end = min((i+1) * n_for_each_cell_type, self.n_samples)
-                generated_frac_df.iloc[inx_start:inx_end, i] = 1
-        else:  # negative samples
-            n_for_each_n_ct = int(self.n_samples / (n_cell_types - 1))
-            for n_ct in range(2, n_cell_types+1):  # the number of cell types used (=2)
-                inx_start = (n_ct-2) * n_for_each_n_ct
-                inx_end = min((n_ct-1) * n_for_each_n_ct, self.n_samples)
-                frac = 1 / n_ct
-                for inx in range(inx_start, inx_end):
-                    if n_ct < n_cell_types:
-                        current_cell_type_inx = np.random.choice(range(n_cell_types), size=n_ct, replace=False)
-                    else:
-                        current_cell_type_inx = np.array(range(n_cell_types))
-                    generated_frac_df.iloc[inx, current_cell_type_inx] = frac
-        return generated_frac_df.round(4)
-
-
-class BulkGEPGeneratorSCT(BulkGEPGenerator):
-    """
-    generate bulk GEPs by cell proportion x single GEP of single cell type (SCT)
-    """
-    def __init__(self, sct_dataset_file_path, cell_types, simu_bulk_dir, bulk_dataset_name):
-        super().__init__(simu_bulk_dir=simu_bulk_dir, cell_types=cell_types, bulk_dataset_name=bulk_dataset_name,
-                         merged_sc_dataset_file_path=None, check_basic_info=False, sc_dataset_ids=[],
-                         sct_dataset_file_path=sct_dataset_file_path)
-        # self.sct_dataset_file_path = sct_dataset_file_path
-        # self.sct_dataset_obs = None
-        # self.sct_dataset_df = None
-
-    def generate_samples(self, n_samples, latent_z_nn_file_path: str = None,
-                         ref_distribution: dict = None, sampling_method: str = 'fragment',
-                         total_cell_number: int = 1, n_threads: int = 10,
-                         log_file_path: str = None, cell_prop_file_path: str = None, add_token_cell_type: bool = False,
-                         random_n_cell_type: list = None):
-        """
-        :param n_samples: the number of GEPs to generate
-        :param latent_z_nn_file_path: neighbor information of latent z for all samples, used for QC and sampling
-        :param total_cell_number: N, the total number of cells sampled from merged single cell dataset
-                                      and averaged to simulate a single bulk RNA-seq sample
-        :param sampling_method: segment or random, method to generate cell fractions
-        :param ref_distribution: reference distribution for each cell type, seperated to 10 bins for [0, 1]
-            {'B Cells': [0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1], '': [], '': [], ...}
-            only used for fragment sampling method when call function self._generate_cell_fraction
-        :param n_threads: number of threads used for parallel computing
-        :param log_file_path:
-        :param cell_prop_file_path: file path of pre-generated cell proportion, use this file if provided
-        :param add_token_cell_type: add all cell types in generated_cell_frac.csv file,
-             even if some cell types take 0% in all samples, only for keeping same format for all dataset
-        :param random_n_cell_type: a list of the number of cell types (selected randomly) used for simulating bulk GEPs
-        """
-        n_total_cpus = multiprocessing.cpu_count()
-        n_threads = min(n_total_cpus - 1, n_threads)
-        self.n_samples = n_samples
-        self.total_cell_number = total_cell_number  # set 1 for all cell types
-        # simulating bulk cell GEP by mixing GEPs of different cell types
-        min_n_cell_frac = np.min([100, n_samples])  # smaller number of samples without filtering
-        if cell_prop_file_path is not None:
-            self.generated_cell_fraction_fp = cell_prop_file_path
-        if not os.path.exists(self.generated_bulk_gep_fp):
-            self.sct_dataset_obs, self.sct_dataset_df = self.read_sct_dataset(latent_z_nn_info_file=
-                                                                              latent_z_nn_file_path)
-
-            if not os.path.exists(self.generated_cell_fraction_fp):
-                print(f'   Generate cell proportions for bulk samples in {self.bulk_dataset_name}')
-                generated_cell_frac = self._generate_cell_fraction(
-                    sampling_method=sampling_method, n_cell_frac=self.n_samples,
-                    sample_prefix=f's_{self.bulk_dataset_name}_{sampling_method}_0',
-                    ref_distribution=ref_distribution,
-                    random_n_cell_type=random_n_cell_type,
-                )
-                if add_token_cell_type:
-                    for ct in sorted_cell_types:
-                        if ct not in generated_cell_frac.columns:
-                            generated_cell_frac[ct] = 0
-                    generated_cell_frac = generated_cell_frac.loc[:, sorted_cell_types]
-                generated_cell_frac.to_csv(self.generated_cell_fraction_fp, float_format='%g')
-            else:
-                print(f'   Previous result exists: {self.generated_cell_fraction_fp}')
-
-            chunk_size = int(self.n_samples / min_n_cell_frac)
-            chunk_size = max(chunk_size, 100)
-            chunk_counter = 0
-            with pd.read_csv(self.generated_cell_fraction_fp, chunksize=chunk_size, index_col=0) as reader:
-                simu_method = 'mul'  # matrix multiplication
-                for rows in tqdm(reader):
-
-                    selected_cell_ids = self._sc_sampling(cell_frac=rows,
-                                                          n_threads=n_threads, obs_df=self.sct_dataset_obs)
-                    simulated_gep = self._map_cell_id2exp(selected_cell_id=selected_cell_ids, cell_frac=rows,
-                                                          sc_dataset='sct_dataset', simu_method=simu_method)
-
-                    simulated_gep = log2_transform(simulated_gep)
-                    self.generated_bulk_gep_counter += simulated_gep.shape[0]
-                    # generated_cell_frac = generated_cell_frac.loc[simulated_gep.index, :].copy()
-                    selected_cell_ids = selected_cell_ids.loc[simulated_gep.index, :].copy()
-                    self._save_simulated_bulk_gep(gep=simulated_gep, cell_id=selected_cell_ids)
-                    chunk_counter += 1
-
-            data_info = f'Simulated {self.generated_bulk_gep_counter} bulk cell gene expression profiles ' \
-                        f'by sampling method: {sampling_method}, simulation method: {simu_method}, log2(TPM + 1)'
-            create_h5ad_dataset(simulated_bulk_exp_file_path=self.generated_bulk_gep_csv_fp,
-                                cell_fraction_file_path=self.generated_cell_fraction_fp,
-                                dataset_info=data_info,
-                                result_file_path=self.generated_bulk_gep_fp)
-            if log_file_path is not None:
-                obj_info = self.__str__()
-                print_msg(obj_info, log_file_path=log_file_path)
-        else:
-            print(f'   Previous result existed: {self.generated_bulk_gep_fp}')
-            print(self.__str__())
-
-
-# for gene-level filtering
-def get_quantile(exp_df, quantile_range, col_name: list = None) -> pd.DataFrame:
-    """
-    Get quantile
-    :param exp_df:
-    :param quantile_range:
-    :param col_name:
-    :return:
-    """
-    quantile_df = pd.DataFrame(index=exp_df.columns, columns=col_name)
-    quantile_df[col_name[0]] = exp_df.quantile(quantile_range[0], axis=0)
-    quantile_df[col_name[1]] = exp_df.quantile(quantile_range[1], axis=0)
-    quantile_df[col_name[2]] = exp_df.quantile(quantile_range[2], axis=0)
-    return quantile_df
-
-
-def get_gene_list_for_filtering(bulk_exp_file, tcga_file, result_file_path, q_col_name: list = None,
-                                filtering_type: str = 'quantile_range',
-                                corr_threshold: float = 0.3, n_gene_max: int = 1000,
-                                corr_result_fp: str = None, quantile_range: list = None):
-    """
-    Gene-level filtering based on the filtering type
-    :param bulk_exp_file:
-    :param tcga_file:
-    :param filtering_type: high_corr_gene, quantile_range, all_genes, high_corr_gene_and_quantile_range
-      - high_corr_gene: expression values with high correlation with the cell proportions of any cell types
-      - quantile_range: the median of expression values within the [q_5, q_95] quantile range
-    :param corr_result_fp:
-    :param quantile_range: median gene expression (quantile_range[1], expected as 0.5) of simulated bulk cell GEPs that
-        is less than quantile_range[0] or greater than quantile_range[2] of the quantile expression value
-        of corresponding gene in TCGA dataset will be removed
-    :param result_file_path:
-    :param q_col_name:
-    :param corr_threshold: correlation threshold for gene filtering
-    :param n_gene_max: maximum number of genes for each cell type during gene filtering
-    :return:
-    """
-
-    assert filtering_type in ['high_corr_gene', 'quantile_range', 'all_genes', 'high_corr_gene_and_quantile_range'], \
-        f'filtering_type: {filtering_type} is not supported, only support high_corr_gene, quantile_range, all_genes, ' \
-        f'high_corr_gene_and_quantile_range'
-    if not os.path.exists(result_file_path):
-        bulk_exp = ReadH5AD(bulk_exp_file).get_df()
-        tcga_obj = ReadExp(tcga_file, exp_type='TPM')
-        tcga_obj.align_with_gene_list(
-            gene_list=bulk_exp.columns.to_list(),
-        )
-        tcga_obj.to_log2cpm1p()
-        tcga = tcga_obj.get_exp()
-        gene_list = []
-        if 'high_corr_gene' in filtering_type:
-            h5_obj = ReadH5AD(bulk_exp_file)
-            gene_exp = h5_obj.get_df(convert_to_tpm=True)
-            cell_frac = h5_obj.get_cell_fraction()
-            corr_df = cal_corr_gene_exp_with_cell_frac(gene_exp=gene_exp, cell_frac=cell_frac,
-                                                       result_file_path=corr_result_fp, filtered_by_corr=corr_threshold,
-                                                       filter_by_num=n_gene_max)
-            del gene_exp
-            gene_list = corr_df.index.to_list()
-            print(f'{len(gene_list)} genes are selected by high correlation')
-        if 'quantile_range' in filtering_type:
-            # both bulk_exp and tcga are in log-space
-            gene_list_qr = get_gene_list_filtered_by_quantile_range(bulk_exp=bulk_exp, tcga_exp=tcga,
-                                                                    quantile_range=quantile_range,
-                                                                    q_col_name=q_col_name)
-            print(f'{len(gene_list_qr)} genes are selected by quantile range')
-            if len(gene_list) > 0:  # if there is high correlation gene, then filter by high correlation gene
-                gene_list = [gene for gene in gene_list if gene in gene_list_qr]
-                print(f'{len(gene_list)} genes are selected by both high correlation and quantile range')
-            else:
-                gene_list = gene_list_qr
-        if filtering_type == 'all_genes':
-            gene_list = bulk_exp.columns.to_list()
-            print(f'All {len(gene_list)} genes will be used')
-
-        gene_list_df = pd.DataFrame(columns=['gene_name'])
-        gene_list_df['gene_name'] = gene_list
-        gene_list_df.to_csv(result_file_path, index=False)
-    else:
-        print(f'Loading the gene list from file: {result_file_path}')
-        gene_list_df = pd.read_csv(result_file_path)
-        gene_list = gene_list_df['gene_name'].to_list()
-    return gene_list
-
-
-def get_gene_list_filtered_by_quantile_range(bulk_exp, tcga_exp, quantile_range: list = None,
-                                             q_col_name: list = None, tcga_gene_info=None):
-    """
-    Get gene list filtered by quantile range
-    :param bulk_exp: bulk expression, TPM
-    :param tcga_exp: TCGA expression data, TPM
-    :param quantile_range: lower boundary, median, upper boundary, such as [0.025, 0.5, 0.975]
-    :param q_col_name: column names for quantile range
-    :param tcga_gene_info: gene quantile values in TCGA
-    """
-    if quantile_range is None:
-        quantile_range = [0.025, 0.5, 0.975]
-        q_col_name = ['q_' + str(int(q * 1000) / 10) for q in quantile_range]
-    if tcga_gene_info is None:
-        tcga_gene_info = get_quantile(tcga_exp, quantile_range=quantile_range, col_name=q_col_name)
-    if type(bulk_exp) is pd.DataFrame and bulk_exp.shape[0] > 1:
-        bulk_gene_info = get_quantile(bulk_exp, quantile_range=quantile_range, col_name=q_col_name)
-        gene_inx = (bulk_gene_info[q_col_name[1]] >= tcga_gene_info[q_col_name[0]]) & \
-                   (bulk_gene_info[q_col_name[1]] <= tcga_gene_info[q_col_name[2]])
-        gene_list_qr = bulk_exp.loc[:, gene_inx].columns.to_list()
-    else:  # if bulk_exp is a series
-        gene_inx = (bulk_exp >= tcga_gene_info[q_col_name[0]]) & (bulk_exp <= tcga_gene_info[q_col_name[2]])
-        gene_list_qr = bulk_exp.loc[gene_inx].index.to_list()
-    return gene_list_qr
-
-
-def cal_loading_by_pca(pca, gene_list, loading_matrix_file_path=None):
-    """
-    Cal loading by PCA
-    :param pca:
-    :param gene_list:
-    :param loading_matrix_file_path:
-    :return:
-    """
-    loading = pca.components_.T * np.sqrt(pca.explained_variance_)
-    # loading = loading.loc[:, gene_list]
-    com_matrix = pd.DataFrame(data=loading[:, 0:3], index=gene_list, columns=['PC1', 'PC2', 'PC3'])
-    com_matrix['PC1_abs'] = com_matrix['PC1'].abs()
-    com_matrix['PC2_abs'] = com_matrix['PC2'].abs()
-    com_matrix['PC3_abs'] = com_matrix['PC3'].abs()
-    com_matrix['PC_top3_sum'] = com_matrix.loc[:, ['PC1_abs', 'PC2_abs', 'PC3_abs']].sum(axis=1)
-    if loading_matrix_file_path is not None:
-        print(f'Saving loading matrix to file: {loading_matrix_file_path}')
-        com_matrix.to_csv(loading_matrix_file_path, index_label='gene_name')
-    return loading
-
-
-def filtering_by_gene_list_and_pca_plot(bulk_exp, tcga_exp, gene_list, result_dir, simu_dataset_name,
-                                        n_components=5, pca_model_name_postfix='', bulk_exp_type='log_space',
-                                        tcga_exp_type='TPM', pca_model_file_path=None, pca_data_file_path=None,
-                                        h5ad_file_path=None, cell_frac_file=None, figsize=(5, 5)):
-    """
-    Filtering by gene list and pca plot
-    :param bulk_exp: log2cpm1p
-    :param tcga_exp: TPM
-    :param gene_list:
-    :param result_dir:
-    :param n_components:
-    :param pca_model_name_postfix:
-    :param bulk_exp_type:
-    :param tcga_exp_type:
-    :param pca_model_file_path:
-    :param pca_data_file_path:
-    :param simu_dataset_name:
-    :param h5ad_file_path: save simulated bulk GEPs depending on filtered gene list to .h5ad file if not None
-    :param cell_frac_file:
-    :return:
-    """
-    bulk_obj = ReadExp(bulk_exp, exp_type=bulk_exp_type)
-    bulk_obj.align_with_gene_list(gene_list=gene_list)
-    bulk_exp = bulk_obj.get_exp()
-    tcga_obj = ReadExp(tcga_exp, exp_type=tcga_exp_type)
-    tcga_obj.align_with_gene_list(gene_list=gene_list)
-    tcga_obj.to_log2cpm1p()
-    tcga_exp = tcga_obj.get_exp()
-
-    # PCA and plot
-    check_dir(result_dir)
-    assert n_components >= 2, 'n_components must be >= 2'
-    if not os.path.exists(pca_data_file_path):
-        # combine both simulated bulk cell GEPs and TCGA dataset together
-        simu_bulk_with_tcga = pd.concat([bulk_exp, tcga_exp])
-        pca_model = do_pca_analysis(exp_df=simu_bulk_with_tcga, n_components=n_components,
-                                    pca_result_fp=pca_model_file_path)
-        pcs = pca_model.transform(simu_bulk_with_tcga)
-        if n_components >= 3:
-            pca_df = pd.DataFrame(pcs[:, range(3)], index=simu_bulk_with_tcga.index, columns=['PC1', 'PC2', 'PC3'])
-        else:
-            pca_df = pd.DataFrame(pcs[:, range(2)], index=simu_bulk_with_tcga.index, columns=['PC1', 'PC2'])
-        pca_df.to_csv(pca_data_file_path)
-    else:
-        print(f'{pca_data_file_path} already exists, skip PCA analysis')
-        pca_df = pd.read_csv(pca_data_file_path, index_col=0)
-        pca_model = load(pca_model_file_path)
-
-    # plot
-    title = f'{simu_dataset_name}_PCA_with_TCGA_{pca_model_name_postfix}'
-    color_code = np.array([simu_dataset_name] * bulk_exp.shape[0] + ['TCGA'] * tcga_exp.shape[0])
-    # cumsum = np.cumsum(pca_model.explained_variance_ratio_)
-    # pca_df['class'] = color_code
-    plot_pca(data=pca_df, figsize=figsize,
-             result_fp=os.path.join(result_dir, title + '.png'),
-             color_code=color_code, explained_variance_ratio=pca_model.explained_variance_ratio_)
-    if h5ad_file_path is not None:
-        assert cell_frac_file is not None, 'cell_frac_file should be provided if h5ad_file_path is not None'
-        print(f'Saving filtered bulk exp to file: {h5ad_file_path}')
-        if not os.path.exists(h5ad_file_path):
-            print('Saving as .h5ad file...')
-            dataset_info = f'Some genes were removed from this dataset for increasing the similarity ' \
-                           f'between TCGA and simulated bulk cell GEPs. This similarity was evaluated by PCA analysis.'
-            create_h5ad_dataset(simulated_bulk_exp_file_path=bulk_exp,
-                                cell_fraction_file_path=cell_frac_file, dataset_info=dataset_info,
-                                result_file_path=h5ad_file_path)
-
-
-if __name__ == '__main__':
-    # pass
-    # gene_samples = gradient_generation_fraction(n=2)
-    root_dir = r'F:\projects\001EMT-infiltration\analysis_result\014_test\nn_model'
-    # cell_frac = pd.read_csv(os.path.join(root_dir, 'generated_frac_n1.csv'), index_col=0)
-    # sc_fp = os.path.join(os.path.join(r'F:\projects\001EMT-infiltration\raw_data\single cells',
-    #                                   'generated_11_cell_type_n1000.h5ad'))
-    # simu_bulk_exp = simulate_bulk_expression(cell_frac=cell_frac, sc_exp_file_path=sc_fp)
-    # simu_bulk_exp.write(os.path.join(root_dir, 'simu_bulk_exp_n1.h5ad'))
-    # simu_bulk_n100_fp = os.path.join(root_dir, 'simu_bulk_exp_n100.h5ad')
-    # prefix = 'simu_bulk_exp_n10'
-    # simu_bulk_exp_fp = os.path.join(root_dir, prefix + '_log2cpm1p.csv')
-    # sc_fp = os.path.join(os.path.join(r'F:\projects\001EMT-infiltration\raw_data\single cells',
-    #                                   'generated_11_cell_type_n5000.h5ad'))
-    # cell_frac_fp = os.path.join(root_dir, 'generated_frac_test_set_n10.csv')
-    # if not os.path.exists(simu_bulk_exp_fp):
-    #     cell_frac = pd.read_csv(cell_frac_fp, index_col=0)
-    #     simulate_bulk_expression(cell_frac=cell_frac, sc_exp_file_path=sc_fp,
-    #                              n_threads=4, result_dir=root_dir, prefix=prefix)
-    #     simu_bulk_exp.to_csv(simu_bulk_n100_selected_id_fp)
+import os
+import gc
+import json
+import numpy as np
+import pandas as pd
+from scipy import stats
+import scanpy as sc
+from typing import Union
+from tqdm import tqdm
+import multiprocessing
+
+from joblib import dump, load
+from sklearn.utils import shuffle
+from ..utility import (create_h5ad_dataset, check_dir, cal_corr_gene_exp_with_cell_frac,
+                       ExpObj, QueryNeighbors, log2_transform, print_msg, get_cell_num,
+                       sorted_cell_types, do_pca_analysis, non_log2cpm)
+from ..utility.read_file import ReadH5AD, read_single_cell_type_dataset, ReadExp
+from ..single_cell import get_sample_id
+from ..plot import plot_pca
+
+
+def segment_generation_fraction(n_samples: int = None, max_value: int = 10000,
+                                cell_types: list = None, sample_prefix: str = None,
+                                cell_prop_prior: dict = None) -> pd.DataFrame:
+    """
+    Generate cell fraction by fixing a specific percentage (gradient) range (i.e. from 1% to 100%)
+        for each specific cell type, and n samples for each gradient of each cell type
+
+    :param n_samples: the number of samples need to generate in total
+
+    :param max_value: cell proportion will be sampled from U(0, max_value), and then scaled to [0, 1]
+
+    :param cell_types: None or a list of cell types. Using all valid cell types if None. All valid cell types can be
+        found by `list(deside.utility.cell_type2abbr.keys())`.
+
+    :param sample_prefix: only for naming
+
+    :param cell_prop_prior: the prior range of cell proportion for each cell type, {'cell_type': (0, 0.1), '': (0, 0.2), ...}
+
+    :return: generated cell fraction, sample by cell type
+    """
+    if sample_prefix is None:
+        sample_prefix = 'seg'
+
+    n_cell_type = len(cell_types)
+    # all_samples = []
+    all_samples_tmp = []
+    while len(all_samples_tmp) < n_samples:
+        frag_for_one_sample = []
+        current_max_value = max_value  # 100%
+        current_sample_valid = True
+        for j in range(n_cell_type - 1):
+            if current_max_value > 1:  # > 1 left
+                _frag = np.random.randint(current_max_value)
+                current_max_value -= _frag
+                frag_for_one_sample.append(_frag)
+            elif current_max_value == 1:  # 1 left
+                frag_for_one_sample.append(current_max_value)
+                current_max_value = 0
+            else:  # current_max_value == 0, 0 left
+                frag_for_one_sample.append(0)
+        frag_for_one_sample.append(current_max_value)  # for last fragment (0 or > 0)
+        assert np.sum(frag_for_one_sample) == max_value
+        np.random.shuffle(frag_for_one_sample)
+        # if max_value == 0:
+        #     all_samples_tmp.append(dict(zip(cell_types, frag_for_one_sample)))
+        # else:
+        #     if max_value > n_cell_type:  # the most common situation
+        #         # cell fraction equals to 0 for at least 4 cell types or none, avoid too much 0 for any cell types
+        #         if (np.sum(np.array(frag_for_one_sample) == 0) >= 4) or \
+        #                 (np.sum(np.array(frag_for_one_sample) == 0) <= 1):
+        #             current_sample_valid = True
+        #     else:   # 0 < max_value <= len(cell_types), don't check, more zeros will be included
+        #         current_sample_valid = True
+        #     if current_sample_valid:
+        frag_for_one_sample = np.array(frag_for_one_sample) / max_value  # normalize to sum to 1
+        cell_type2frag = dict(zip(cell_types, frag_for_one_sample))
+        if cell_prop_prior is not None:
+            for cell_type, frag in cell_type2frag.items():
+                # check if the cell fraction is in the prior range
+                if (frag < cell_prop_prior[cell_type][0]) or (frag > cell_prop_prior[cell_type][1]):
+                    current_sample_valid = False
+                    break
+        if current_sample_valid:
+            all_samples_tmp.append(cell_type2frag)
+        # frag_for_one_sample = np.array(frag_for_one_sample) / max_value  # normalize to decimal
+        # all_samples_tmp.append(dict(zip(cell_types, frag_for_one_sample)))
+
+    index = [sample_prefix + '_' + str(i + 1) for i in range(len(all_samples_tmp))]
+    all_samples_df = pd.DataFrame(all_samples_tmp, index=index)
+    all_samples_df = all_samples_df.loc[:, cell_types]
+    return all_samples_df.round(4)
+
+
+def seg_random_generation_fraction(n_samples: int = None, cell_types: list = None,
+                                   sample_prefix: str = None) -> pd.DataFrame:
+    """
+    Generate cell fraction by combining segment and random sampling method
+
+    :param n_samples: the number of samples need to generate in total
+
+    :param cell_types: None or a list of cell types. Using all valid cell types if None. All valid cell types can be
+        found by `list(deside.utility.cell_type2abbr.keys())`.
+
+    :param sample_prefix: only for naming
+
+    :return: generated cell fraction, sample by cell type
+    """
+    if sample_prefix is None:
+        sample_prefix = 'seg_random'
+
+    # all_samples = []
+    all_samples_tmp = []
+    while len(all_samples_tmp) < n_samples:
+        # get the first fraction
+        first_segment = np.random.rand()
+        others_fraction = np.random.rand(len(cell_types)-1)
+        # scaling sum to 1 and then rescaling to (1-first_segment)
+        others_fraction = others_fraction / others_fraction.sum() * (1 - first_segment)
+        frag_for_one_sample = np.concatenate([np.array([first_segment]), others_fraction])
+        frag_for_one_sample = frag_for_one_sample / frag_for_one_sample.sum()  # scaling again
+        np.random.shuffle(frag_for_one_sample)
+        all_samples_tmp.append(dict(zip(cell_types, frag_for_one_sample)))
+
+    index = [sample_prefix + '_' + str(i + 1) for i in range(len(all_samples_tmp))]
+    all_samples_df = pd.DataFrame(all_samples_tmp, index=index)
+    all_samples_df = all_samples_df.loc[:, cell_types]
+    # all_samples.append(current_df)
+    return all_samples_df.round(4)
+
+
+def fragment_generation_fraction(n_samples: int = None, cell_types: list = None,
+                                 sample_prefix: str = None, reference_distribution: dict = None,
+                                 bins: int = 10, minimal_prop: float = 0.005) -> pd.DataFrame:
+    """
+    Generate cell fraction by fragment sampling method
+
+    :param n_samples: the number of samples need to generate in total
+
+    :param cell_types: None or a list of cell types. Using all valid cell types if None. All valid cell types can be
+        found by `list(deside.utility.cell_type2abbr.keys())`.
+
+    :param sample_prefix: only for naming
+
+    :param reference_distribution: reference distribution for each cell type, seperated to 10 bins for [0, 1]
+        {'B Cells': [0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1], '': [], '': [], ...}
+
+    :param bins: the number of bins for each distribution
+
+    :param minimal_prop: set to 0 if less than this value
+
+    :return: generated cell fraction, sample by cell type
+    """
+    if sample_prefix is None:
+        sample_prefix = 'fragment'
+    bin_lower_edges = np.linspace(0, 1 - 1/bins, bins)  # array([0. , 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9])
+    ct2prop = {}
+    if reference_distribution is None:
+        reference_distribution = {}
+        for ct in cell_types:
+            reference_distribution[ct] = np.ones(bins) * (1 / bins)  # uniform distribution
+    for ct in cell_types:
+        # get cell proportions for each cell type
+        current_ref_dis = reference_distribution[ct]
+        current_prop = np.random.choice(bin_lower_edges, n_samples, p=current_ref_dis)  # sampling depending on ref dis
+        # lower edge + x ~ U(0, 0.1) -> [lower_edge, lower_edge + 0.1]
+        noise_for_each_prop = 0.1 * np.random.rand(n_samples)
+        current_prop += noise_for_each_prop
+        ct2prop[ct] = current_prop
+
+    index = [sample_prefix + '_' + str(i + 1) for i in range(n_samples)]
+    all_samples_df = pd.DataFrame.from_dict(ct2prop, orient='columns')
+    all_samples_df.index = index
+    # scaling sum to 1
+    all_samples_df = all_samples_df / np.sum(all_samples_df.values, axis=1).reshape(-1, 1)
+    all_samples_df[all_samples_df < minimal_prop] = 0
+    all_samples_df = all_samples_df / np.sum(all_samples_df.values, axis=1).reshape(-1, 1)  # scale again
+    all_samples_df = all_samples_df.loc[:, cell_types]
+    # all_samples.append(current_df)
+    return all_samples_df.round(4)
+
+
+def _create_fractions(n_cell_types, fixed_range: dict = None):
+    """
+    generate (pure) random fractions
+    :param n_cell_types: number of fractions to create
+    :param fixed_range: the range of cell fraction for each cell type, {'cell_type': (0, 100), '': (), ...}
+    :return: list of random fracs with the length n_cell_types
+    """
+    if (fixed_range is None) or (len(fixed_range) < n_cell_types):
+        fracs = np.random.rand(n_cell_types)  # uniform distribution over [0, 1)
+    else:
+        fracs = []
+        for cell_type, ct_range in fixed_range.items():
+            _frac = np.random.randint(ct_range[0], ct_range[1]) / 100
+            fracs.append(_frac)
+        fracs = np.array(fracs)
+    fracs_sum = np.sum(fracs)
+    fracs = np.divide(fracs, fracs_sum)
+    return fracs
+
+
+def random_generation_fraction(n_samples: int = 100, cell_types: list = (),
+                               sample_prefix: str = None, fixed_range: dict = None) -> pd.DataFrame:
+    """
+    Create pure random cell fractions, same as `Scaden`
+
+    :param n_samples: number of samples to create
+
+    :param cell_types: a list of cell types
+
+    :param sample_prefix: prefix of sample names
+
+    :param fixed_range: the range of cell fraction for each cell type, {'cell_type': (0, 100), '': (), ...}
+
+    :return:  generated cell fraction, sample by cell type
+    """
+    if sample_prefix is None:
+        sample_prefix = 's_random'
+    n_cell_types = len(cell_types)
+    id2cell_frac = {}
+
+    for i in range(n_samples):
+        sample_name = sample_prefix + '_' + str(i)
+        id2cell_frac[sample_name] = _create_fractions(n_cell_types, fixed_range=fixed_range)
+    generated_frac_df = pd.DataFrame.from_dict(id2cell_frac, orient='index', columns=cell_types)
+    return generated_frac_df.round(2)
+
+
+def map_cell_id2exp(sc_exp, selected_cell_id):
+    """
+
+    :param sc_exp: a AnnData object, log2(CPM + 1), samples by genes
+    :param selected_cell_id: a dataFrame which contains cell_type, n_cell, selected_cell_id
+    :return: a DataFrame, log2(CPM + 1), samples by genes
+    """
+    # sc_exp = an.read_h5ad(sc_exp)
+    adata_df = pd.DataFrame(sc_exp.X.A, index=sc_exp.obs.index, columns=sc_exp.var.index)
+    adata_df = np.power(2, adata_df) - 1  # convert to non-log values
+    simulated_exp = {}
+
+    for sample_id, group in selected_cell_id.groupby(by=selected_cell_id.index):
+        cell_ids = []
+        for i, row in group.iterrows():
+            if row['n_cell'] > 0:
+                cell_ids += row['selected_cell_id'].split(';')
+        current_merged = adata_df.loc[cell_ids, :].copy()
+        simulated_exp[sample_id] = current_merged.mean(axis=0)  # single simulated bulk expression profile
+
+    simulated_exp_df = pd.DataFrame.from_dict(data=simulated_exp, orient='index')
+    # simu_adata = an.AnnData(simulated_exp_df)
+    # simu_adata.X = np.log2(simu_adata.X + 1)  # log2(CPM + 1)
+    # simulated_exp_df.rename(index={i: j for i, j in enumerate(filtered_single_cell_exp.index)}, inplace=True)
+    log2cpm = np.log2(simulated_exp_df.values + 1)
+    return pd.DataFrame(log2cpm, index=simulated_exp_df.index, columns=sc_exp.var.index).round(2)
+
+
+# def simulate_bulk_expression(cell_frac: pd.DataFrame, sc_exp_file_path: str,
+#                              n_threads: int = 2, result_dir=None,
+#                              prefix='simu_bulk_exp', step_size: int = 201, total_cell_number: int = 500):
+#     """
+#     Mix single cell expression profile to simulated bulk expression profile according to `cell_frac`. at large scale
+#
+#     :param cell_frac: dataFrame, generated cell fraction for each cell type, samples by cell types
+#
+#     :param sc_exp_file_path: string, .h5ad file, single cell n5000 dataset, log2(CPM + 1)
+#         the file path of single cell expression profiles classified by cell types
+#
+#     :param n_threads: how many thread to use
+#
+#     :param result_dir:
+#
+#     :param prefix: only for naming output files
+#
+#     :param step_size: separate to multiple steps when memory is not enough
+#
+#     :param total_cell_number: N, the total number of cells in single cell dataset
+#                               averagedd to simulate a single bulk RNA-seq sample
+#
+#     :return: simulated bulk expression profiles, sample by gene, log2(CPM + 1), .h5ad file
+#     """
+#
+#     # cell_type2sample_name
+#     # single cell dataset, .h5ad file, samples by genes, log2(CPM + 1)
+#     cell_num = get_cell_num(cell_type_frac=cell_frac, total_num=total_cell_number)
+#     sc_exp = sc.read_h5ad(sc_exp_file_path)
+#     obs_df = sc_exp.obs
+#     # adata_df = pd.DataFrame(sc_exp.X.A, index=sc_exp.obs.index, columns=sc_exp.var.index)
+#     # adata_df = np.power(2, adata_df) - 1  # convert to non-log values
+#     print('   Start to select cells randomly based on cell types for generating each bulk expression profile...')
+#     selected_cell_id = []
+#     # step = 201
+#     n_parts = cell_frac.shape[0] // step_size
+#     for inx in tqdm(range(n_parts+1)):
+#         if inx == n_parts:
+#             current_part = cell_num.iloc[inx * step_size:, :]
+#             if current_part.shape[0] == 0:
+#                 break
+#         else:
+#             # continue
+#             current_part = cell_num.iloc[inx * step_size: (inx + 1) * step_size, :]
+#         current_part_flatten = []
+#         for cell_type in current_part.columns:
+#             _part = pd.DataFrame(index=current_part.index)
+#             _part['cell_type'] = cell_type
+#             _part['n_cell'] = current_part[cell_type]
+#             current_part_flatten.append(_part)
+#         current_part_flatten = pd.concat(current_part_flatten)
+#         # contains all cell types for each single simulated bulk expression
+#         paras = [(obs_df, 1, row['cell_type'], row['n_cell'], 'cell_type')
+#                  for i, row in current_part_flatten.iterrows()]
+#         # https://pythonspeed.com/articles/python-multiprocessing/
+#         with multiprocessing.get_context('spawn').Pool(n_threads) as p:
+#             results = p.starmap(get_sample_id, paras)
+#         # print(results)
+#         results_str = [';'.join(i) for i in results]
+#         current_part_flatten['selected_cell_id'] = results_str
+#         current_part_flatten.sort_index(inplace=True)
+#         if result_dir is not None:
+#             current_exp = map_cell_id2exp(sc_exp=sc_exp, selected_cell_id=current_part_flatten)
+#             cell_id_fp = os.path.join(result_dir, prefix + '_selected_cell_id.csv')
+#             exp_fp = os.path.join(result_dir, prefix + '_log2cpm1p.csv')
+#             if not os.path.exists(cell_id_fp):
+#                 current_part_flatten.to_csv(cell_id_fp)
+#             else:
+#                 current_part_flatten.to_csv(cell_id_fp, header=False, mode='a')
+#             if not os.path.exists(exp_fp):
+#                 current_exp.to_csv(exp_fp)
+#             else:
+#                 current_exp.to_csv(exp_fp, header=False, mode='a')
+#             gc.collect()
+#         else:
+#             selected_cell_id.append(current_part_flatten)
+#
+#     if selected_cell_id:
+#         selected_cell_df = pd.concat(selected_cell_id)
+#         return selected_cell_df
+
+
+class BulkGEPGenerator(object):
+    """
+    Generate bulk GEPs from single cell datasets
+
+    :param simu_bulk_dir: the directory to save simulated bulk cell GEPs
+    :param merged_sc_dataset_file_path: the file path of pre-merged single cell datasets
+    :param sct_dataset_file_path: the file path of single cell datasets (scGEP, dataset `S1`)
+    :param cell_types: cell types used when generating bulk GEPs
+    :param sc_dataset_ids: single cell dataset id used when generating bulk GEPs
+    :param bulk_dataset_name: the name of generated bulk dataset, only for naming
+    :param check_basic_info: whether to check basic information of single cell datasets
+    :param zero_ratio_threshold: the threshold of zero ratio of genes in single cell GEPs, remove the GEP if zero ratio > threshold
+    :param sc_dataset_gep_type: the type of single cell GEPs, `log_space` or `linear_space`
+    :param tcga2cancer_type_file_path: the file path of `tcga_sample_id2cancer_type.csv`, which contains the cancer type of TCGA samples
+    """
+    def __init__(self, simu_bulk_dir, merged_sc_dataset_file_path, sct_dataset_file_path,
+                 cell_types: list, sc_dataset_ids: list, bulk_dataset_name: str = None,
+                 check_basic_info: bool = True, zero_ratio_threshold: float = 0.97,
+                 sc_dataset_gep_type: str = 'log_space', tcga2cancer_type_file_path: str = None):
+        """
+        """
+        self.simu_bulk_dir = simu_bulk_dir  # result dir
+        check_dir(simu_bulk_dir)
+        self.merged_sc_fp = merged_sc_dataset_file_path
+        self.cell_type_in_sc = None  # cell types in merged single cell datasets
+        self.dataset_in_sc = None  # single cell datasets were merged together
+        self.cell_type_used = cell_types
+        self.sc_dataset_used = sc_dataset_ids
+        self.merged_sc_dataset = None
+        self.generated_sc_fp = None  # the file path of generated single cell dataset
+        # self.generated_sc_dataset = None
+        self.generated_sc_dataset_obs = None
+        self.generated_sc_dataset_df = None  # CPM GEPs of generated single cell dataset
+        self.bulk_dataset_name = bulk_dataset_name
+        self.n_samples = None  # the number of generated bulk cell GEPs
+        self.generated_bulk_gep = None
+        # self.generated_bulk_gep_fp = None  # .h5ad file path of generated bulk GEPs, log2(TPM+1)
+        self.generated_bulk_gep_counter = 0
+        self.n_round = 0
+        self.generated_cell_frac = None
+        self.total_cell_number = None  # N, average to form a bulk GEP
+        self.q_dis_nn_ref_upper: float = 0  # the quantile of distance for each pair in reference dataset, such as TCGA
+        self.q_dis_nn_ref_lower: float = 0  # the quantile of distance for each pair in reference dataset, such as TCGA
+        self.filtering_quantile_upper = 0  # the upper quantile used to determine q_dis_nn_ref for sample filtering
+        self.filtering_quantile_lower = None  # the lower quantile used to determine q_dis_nn_ref for sample filtering
+        self.marker_ratio_ref = None  # the marker gene ratios of reference dataset
+        prefix = f'simu_bulk_exp_{self.bulk_dataset_name}'
+        self.generated_cell_fraction_fp = os.path.join(self.simu_bulk_dir,
+                                                       f'generated_frac_{self.bulk_dataset_name}.csv')
+        self.ref_neighbor_counter_fp = os.path.join(self.simu_bulk_dir, f'ref2n_neighbors_{self.bulk_dataset_name}.csv')
+        self.generated_bulk_gep_csv_fp = os.path.join(self.simu_bulk_dir, prefix + f'_log2cpm1p.csv')
+        self.sampled_sc_cell_id_file_path = os.path.join(self.simu_bulk_dir, prefix + '_sampled_sc_cell_id.csv')
+        self.generated_bulk_gep_fp = self.generated_bulk_gep_csv_fp.replace('.csv', '.h5ad')  # final result
+        self.n_neighbors_each_ref = 1  # control the distribution of marker ratio by reference dataset
+        self.ref_neighbor_counter = {}
+        self.merged_sc_dataset_obs = None
+        self.merged_sc_dataset_df = None  # CPM GEPs of merged single cell dataset
+        self.obs_df = None  # used for sampling
+        self.sct_dataset_df = None  # only used in subclass "BulkGEPGeneratorSCT"
+        self.zero_ratio_threshold = zero_ratio_threshold
+        self.sct_dataset_file_path = sct_dataset_file_path
+        self.sct_dataset_obs = None
+        self.m_gep_ref = None  # median / mean GEP of reference dataset
+        # unique expression values in scRNA-seq dataset saved in merged_7_sc_dataset_log2cpm1p.h5ad
+        self.unique_exp_value_in_s0 = None  # {'cell_type1': {'gene1': np.array([]), ...}, 'cell_type2': {}, ...}
+        self.sc_dataset_gep_type = sc_dataset_gep_type
+        self.tcga2cancer_type_file_path = tcga2cancer_type_file_path
+        if check_basic_info and not os.path.exists(self.generated_bulk_gep_fp):
+            self._check_basic_info()
+
+    def _generate_cell_fraction(self, sampling_method: str, n_cell_frac: int, sampling_range: dict = None,
+                                sample_prefix: str = None, ref_distribution: dict = None,
+                                random_n_cell_type: list = None, cell_prop_prior: dict = None):
+        """
+        Generate cell proportions for each simulated bulk GEP
+
+        :param sampling_method: 'segment' or 'random'
+        :param n_cell_frac: the number of GEPs to generate
+        :param sampling_range: the range of sampling, such as {'cell_type1': [0.1, 0.9], 'cell_type2': [0.1, 0.9], ...}
+        :param sample_prefix: the prefix of sample name, such as 'sample1', 'sample2', ...
+        :param ref_distribution: the reference distribution of cell fractions, such as {'cell_type1': [0.1, 0.2, 0.3], ...}
+        :param random_n_cell_type: the number of cell types to randomly select from reference distribution
+        :param cell_prop_prior: the prior of cell proportions, such as {'cell_type1': 0.1, 'cell_type2': 0.2, ...}
+        """
+        if sampling_method == 'segment':
+            gen_cell_fracs = segment_generation_fraction(n_samples=n_cell_frac,
+                                                         max_value=10000,
+                                                         sample_prefix=sample_prefix,
+                                                         cell_types=self.cell_type_used,
+                                                         cell_prop_prior=cell_prop_prior)
+
+        elif sampling_method == 'seg_random':
+            gen_cell_fracs = seg_random_generation_fraction(n_samples=n_cell_frac,
+                                                            sample_prefix=sample_prefix,
+                                                            cell_types=self.cell_type_used)
+
+        elif sampling_method == 'fragment':
+            if random_n_cell_type is None:
+                gen_cell_fracs = fragment_generation_fraction(n_samples=n_cell_frac,
+                                                              sample_prefix=sample_prefix,
+                                                              cell_types=self.cell_type_used,
+                                                              reference_distribution=ref_distribution)
+            else:
+                gen_cell_frac_list = []
+                n_sample_for_each_n_cell_type = int(n_cell_frac / len(random_n_cell_type))
+                for n_cell_type in random_n_cell_type:
+                    if 2 <= n_cell_type <= len(self.cell_type_used):
+                        cell_types = self.cell_type_used[:n_cell_type]  # generate by fixed cell types, then shuffle
+                        _gen_cell_fracs = fragment_generation_fraction(n_samples=n_sample_for_each_n_cell_type,
+                                                                       sample_prefix=f'{sample_prefix}_{n_cell_type}',
+                                                                       cell_types=cell_types,
+                                                                       reference_distribution=ref_distribution)
+                        gen_cell_frac_list.append(_gen_cell_fracs)
+                    else:
+                        raise ValueError(f'All numbers in "random_n_cell_type" should be >= 2 and '
+                                         f'<= the number of used cell types,  {n_cell_type} got.')
+                gen_cell_fracs_total = pd.concat(gen_cell_frac_list)
+                gen_cell_fracs_total = gen_cell_fracs_total.fillna(0)
+                # shuffle_inx = np.zeros(gen_cell_fracs.shape, dtype=np.int16)
+                inx2cell_frac = {}
+                for i in range(gen_cell_fracs_total.shape[0]):
+                    shuffle_inx = shuffle(np.arange(gen_cell_fracs_total.shape[1]))
+                    inx2cell_frac[i] = gen_cell_fracs_total.values[i, shuffle_inx]  # shuffle each row
+                gen_cell_fracs = pd.DataFrame.from_dict(inx2cell_frac, orient='index',
+                                                        columns=gen_cell_fracs_total.columns)
+                gen_cell_fracs.index = gen_cell_fracs_total.index
+
+        elif sampling_method == 'random':
+            if sampling_range is not None:
+                # gradient_range = sampling_range.copy()
+                if len(sampling_range) < len(self.cell_type_used):
+                    print('   * Since the length of gradient_range is less than cell types, gradient range '
+                          'will not be used. Instead, [0, 1] range will be used for all cell types...')
+                    sampling_range = None
+            gen_cell_fracs = random_generation_fraction(n_samples=n_cell_frac, cell_types=self.cell_type_used,
+                                                        sample_prefix=sample_prefix,
+                                                        fixed_range=sampling_range)
+        else:
+            raise ValueError(
+                f'Only "segment" and "random" were supported for parameter "sampling_method", '
+                f'{sampling_method} is invalid')
+        return gen_cell_fracs
+
+    def generate_gep(self, n_samples, sampling_range: dict = None, sampling_method: str = 'segment',
+                     total_cell_number: int = 100, n_threads: int = 10, filtering: bool = True,
+                     reference_file: Union[str, pd.DataFrame] = None, ref_exp_type: str = None,
+                     gep_filtering_quantile: tuple = (None, 0.95), log_file_path: str = None,
+                     n_top: int = 20, simu_method='mul', filtering_method='media_gep',
+                     add_noise: bool = False, noise_params: tuple = (), filtering_ref_types: list = None,
+                     show_filtering_info: bool = False, cell_prop_prior: dict = None,
+                     high_corr_gene_list: list = None, filtering_by_gene_range: bool = False,
+                     min_percentage_within_gene_range: float = 0.95, gene_quantile_range: list = None):
+        """
+        Generating simulated bulk GEPs from scGEP dataset (`S1`)
+
+        :param n_samples: the number of GEPs to generate
+        :param total_cell_number: N, the total number of cells sampled from merged single cell dataset
+                                      and averaged to simulate a single bulk RNA-seq sample
+        :param sampling_method: segment or random, method to generate cell fractions
+        :param sampling_range: the range of sampling, such as {'cell_type1': [0.1, 0.9], 'cell_type2': [0.1, 0.9], ...},
+            optional, only used when sampling_method is `random`
+        :param n_threads: number of threads used for parallel computing
+        :param filtering: whether filtering generated GEPs
+        :param reference_file: the file path of reference dataset for filtering
+        :param ref_exp_type: the type of expression values in reference dataset, TPM / log_space
+        :param gep_filtering_quantile: quantile of nearest distance of each pair in reference,
+            smaller quantile gives smaller radius and fewer simulated GEPs will be kept
+        :param log_file_path: the path of log file
+        :param n_top: if too many neighbors were founded for one single sample, only keep n_top neighbors,
+            used in marker ratio filtering
+        :param simu_method: the method to generate simulated bulk GEPs,
+            ave (average all selected single cell GEPs), mul (multiple GEP by cell fractions)
+        :param filtering_method: marker_ratio (l2 distance with marker gene ratio) or
+            median_gep (`l1` distance with median expression value for each gene)
+        :param add_noise: whether add noise to generated bulk GEPs
+        :param noise_params: parameters for noise generation, (f, max_sum),
+            ref: Hao, Yuning, et al. PLoS Computational Biology, 2019
+        :param filtering_ref_types: the cancer types used for filtering
+        :param show_filtering_info: whether show filtering information
+        :param cell_prop_prior: a prior range of cell proportions for each cell type in solid tumors
+        :param high_corr_gene_list: a list of genes that the expression values have high correlation with
+            the cell proportions for at least one cell type
+        :param filtering_by_gene_range: whether filtering GEPs by gene expression range,
+            the percentage of genes within a specific quantile range in TCGA
+        :param min_percentage_within_gene_range: the minimal percentage of genes within a specific quantile range in TCGA
+        :param gene_quantile_range: the quantile range of gene expression values in TCGA for gene based filtering
+        """
+        n_total_cpus = multiprocessing.cpu_count()
+        n_threads = min(n_total_cpus - 1, n_threads)
+        self.n_samples = n_samples
+        self.total_cell_number = total_cell_number
+        self.filtering_quantile_lower, self.filtering_quantile_upper = gep_filtering_quantile
+        # print(f'   > filtering quantile is {self.filtering_quantile * 100}%')
+        # simulating bulk cell GEP by mixing GEPs of different cell types
+        if filtering:
+            min_n_cell_frac = np.min([5000, n_samples])  # bigger number of samples for filtering
+        else:
+            min_n_cell_frac = np.min([1000, n_samples])  # smaller number of samples without filtering
+        if not os.path.exists(self.generated_bulk_gep_fp):
+            # read generated single cell dataset into self.generated_sc_dataset
+            self._check_intermediate_generated_gep()
+            # using merged single cell dataset directly
+            obs_df = self.merged_sc_dataset_obs
+            sc_dataset = 'merged_sc_dataset'
+            gene_list_in_sc_ds = []
+            if (self.merged_sc_fp is None) and (self.sct_dataset_file_path is None):
+                raise FileNotFoundError('Either "merged_sc_dataset_file_path" or '
+                                        '"sct_dataset_file_path" should be provided')
+            if (self.merged_sc_fp is not None) and (self.merged_sc_dataset_df is None):
+                if self.sc_dataset_gep_type == 'log_space':
+                    self.merged_sc_dataset_df = ReadH5AD(self.merged_sc_fp).get_df(convert_to_tpm=True)
+                else:  # non log space
+                    self.merged_sc_dataset_df = ReadH5AD(self.merged_sc_fp).get_df()
+                gene_list_in_sc_ds = self.merged_sc_dataset_df.columns.to_list()
+            if simu_method == 'mul':  # mul, using either merged_sc_dataset or sct_dataset
+                self.total_cell_number = 1  # only 1 sample for each cell type
+                if (self.sct_dataset_file_path is not None) and (self.sct_dataset_df is None):
+                    self.sct_dataset_obs, self.sct_dataset_df = self._read_sct_dataset()
+                    sc_dataset = 'sct_dataset'
+                    obs_df = self.sct_dataset_obs
+                    gene_list_in_sc_ds = self.sct_dataset_df.columns.to_list()
+            if sc_dataset == 'merged_sc_dataset':
+                min_n_cell_frac = 300  # since some cell types only have a small number of cells
+            # n_round = 0
+            sample_id_for_filtering = []
+            tcga_gene_info = None
+            exp_ref_df = None
+            if filtering and filtering_ref_types is not None:
+                s2c = pd.read_csv(self.tcga2cancer_type_file_path, index_col=0)  # sample id to cancer type in TCGA
+                sample_id_for_filtering = s2c.loc[s2c['cancer_type'].isin(filtering_ref_types), :].index.to_list()
+                _str = ', '.join(filtering_ref_types)
+                print(f'   > {len(sample_id_for_filtering)} samples in {_str} are used '
+                      f'for {filtering_method} filtering.')
+            if not filtering:
+                cell_prop_prior = None
+            with tqdm(total=self.n_samples) as pbar:
+                if self.generated_bulk_gep_counter != 0:
+                    pbar.update(self.generated_bulk_gep_counter)
+                while self.generated_bulk_gep_counter < self.n_samples:
+                    generated_cell_frac = self._generate_cell_fraction(
+                        sampling_method=sampling_method, n_cell_frac=min_n_cell_frac,
+                        sampling_range=sampling_range, sample_prefix=f's_{sampling_method}_{self.n_round}',
+                        cell_prop_prior=cell_prop_prior)
+                    # setting step_size equals to n_cell_frac, so n_parts equals to 1
+                    selected_cell_ids = self._sc_sampling(cell_frac=generated_cell_frac,
+                                                          n_threads=n_threads, obs_df=obs_df)
+                    simulated_gep = self._map_cell_id2exp(selected_cell_id=selected_cell_ids,
+                                                          simu_method=simu_method,
+                                                          sc_dataset=sc_dataset,
+                                                          cell_frac=generated_cell_frac,
+                                                          add_noise=add_noise, noise_params=noise_params)
+                    if filtering:
+                        if reference_file is None or ref_exp_type is None:
+                            raise ValueError('Both "reference_file" and "ref_exp_type" should not be None '
+                                             'when "filtering" is True')
+                        if high_corr_gene_list is not None:
+                            assert np.all([i in gene_list_in_sc_ds for i in high_corr_gene_list])
+                            gene_list_in_sc_ds = high_corr_gene_list
+                            print(f'   > {len(gene_list_in_sc_ds)} high corr genes are used for filtering.')
+                            simulated_gep = simulated_gep.loc[:, gene_list_in_sc_ds]
+                            simulated_gep = non_log2cpm(simulated_gep)
+                        if exp_ref_df is None:
+                            exp_obj_ref = ExpObj(exp_file=reference_file, exp_type=ref_exp_type)
+                            exp_obj_ref.align_with_gene_list(gene_list=gene_list_in_sc_ds, fill_not_exist=True)
+                            exp_ref_df = exp_obj_ref.get_exp()
+                            exp_ref_df = exp_ref_df.loc[exp_ref_df.index.isin(sample_id_for_filtering), :]
+
+                    if filtering and filtering_method == 'marker_ratio':
+                        # print('   Filtering simulated bulk cell GEPs by marker gene ratio of TCGA...')
+                        if self.marker_ratio_ref is None:
+                            exp_obj_ref = ExpObj(exp_file=reference_file, exp_type=ref_exp_type)
+                            exp_obj_ref.cal_marker_gene_ratio(agg_methods={'CD4 T': 'max', 'B Cells': 'max'},
+                                                              cell_types=self.cell_type_used, show_marker_gene=True)
+                            self.marker_ratio_ref = exp_obj_ref.get_marker_ratios()
+                            n_ref = self.marker_ratio_ref.shape[0]
+                            if n_ref < self.n_samples:
+                                # skip some reference samples (1000) since non-epithelial cancers exist
+                                self.n_neighbors_each_ref = int(np.ceil(self.n_samples / (n_ref - 1000)))
+                            if not self.ref_neighbor_counter:
+                                self.ref_neighbor_counter = {i: 0 for i in self.marker_ratio_ref.index}
+                            n_top = min(n_top, self.n_neighbors_each_ref)
+
+                        simulated_gep = self._filter_gep_by_reference(simulated_gep=simulated_gep,
+                                                                      n_top=n_top)
+                        if (simulated_gep is None) or (simulated_gep.shape[0] < 50):
+                            if self.filtering_quantile_upper < 0.999:
+                                # larger filtering_quantile to get more neighbors
+                                self.filtering_quantile_upper += 0.001
+                            else:
+                                self.filtering_quantile_upper += 0.0001
+                            qn1 = QueryNeighbors(df_file=self.marker_ratio_ref)
+                            self.q_dis_nn_ref_upper = qn1.get_quantile_of_nn_distance(
+                                quantile=self.filtering_quantile_upper)  # quantile of distance
+                            print(f'   > Larger filtering_quantile will be used to get more neighbors.')
+                            print(f'   > Quantile distance of {self.filtering_quantile_upper * 100}% is: {self.q_dis_nn_ref_upper}')
+                    if filtering and filtering_by_gene_range:
+                        if tcga_gene_info is None:
+                            if gene_quantile_range is None:
+                                quantile_range = [0.005, 0.5, 0.995]
+                            else:
+                                quantile_range = gene_quantile_range
+                            q_col_name = ['q_' + str(int(q * 1000) / 10) for q in quantile_range]
+                            tcga_gene_info = get_quantile(exp_ref_df, quantile_range=quantile_range,
+                                                          col_name=q_col_name)
+                        valid_gep_list = []
+                        for inx, row in simulated_gep.iterrows():
+                            valid = True
+                            current_gene_list = \
+                                get_gene_list_filtered_by_quantile_range(bulk_exp=row, tcga_exp=exp_ref_df,
+                                                                         tcga_gene_info=tcga_gene_info,
+                                                                         quantile_range=quantile_range,
+                                                                         q_col_name=q_col_name)
+                            if len(current_gene_list) / exp_ref_df.shape[1] < min_percentage_within_gene_range:
+                                valid = False
+                            valid_gep_list.append(valid)
+                        if show_filtering_info:
+                            print(f'   > {np.sum(valid_gep_list)} were kept after filtering by gene range.')
+                        simulated_gep = simulated_gep.loc[valid_gep_list, :].copy()
+
+                    if filtering and (filtering_method == 'median_gep' or
+                                      filtering_method == 'mean_gep') and (simulated_gep is not None):
+                        if self.m_gep_ref is None:
+                            if filtering_method == 'median_gep':
+                                self.m_gep_ref = exp_ref_df.median(axis=0).values.reshape(1, -1)  # TPM
+                            elif filtering_method == 'mean_gep':
+                                self.m_gep_ref = exp_ref_df.mean(axis=0).values.reshape(1, -1)
+                            else:
+                                raise ValueError(f'filtering_method {filtering_method} is invalid')
+                            l1_distance_with_center_ref = np.linalg.norm(exp_ref_df - self.m_gep_ref,
+                                                                         ord=1, axis=1)
+                            self.q_dis_nn_ref_upper = np.quantile(l1_distance_with_center_ref,
+                                                                  self.filtering_quantile_upper)
+                        assert np.all(exp_ref_df.columns == simulated_gep.columns)
+
+                        l1_dis_ref_simu_gep = np.linalg.norm(simulated_gep.values - self.m_gep_ref, ord=1, axis=1)
+                        if self.filtering_quantile_lower is not None:
+                            self.q_dis_nn_ref_lower = np.quantile(l1_distance_with_center_ref,
+                                                                  self.filtering_quantile_lower)
+                            if show_filtering_info:
+                                print(f'   > Quantile distance of {self.filtering_quantile_lower * 100}% is: '
+                                      f'{self.q_dis_nn_ref_lower}, {np.sum(l1_dis_ref_simu_gep < self.q_dis_nn_ref_lower)} were removed')
+                                print(f'   > Quantile distance of {self.filtering_quantile_upper * 100}% is: '
+                                      f'{self.q_dis_nn_ref_upper}, {np.sum(l1_dis_ref_simu_gep > self.q_dis_nn_ref_upper)} were removed')
+                            simulated_gep = simulated_gep.loc[(l1_dis_ref_simu_gep <= self.q_dis_nn_ref_upper) &
+                                                              (l1_dis_ref_simu_gep >= self.q_dis_nn_ref_lower), :]
+                        else:
+                            simulated_gep = simulated_gep.loc[l1_dis_ref_simu_gep <= self.q_dis_nn_ref_upper, :].copy()
+
+                    if simulated_gep is not None:
+                        if (self.generated_bulk_gep_counter + simulated_gep.shape[0]) > self.n_samples:
+                            n_last_part = self.n_samples - self.generated_bulk_gep_counter
+                            simulated_gep = simulated_gep.iloc[range(n_last_part)].copy()
+                        simulated_gep = log2_transform(simulated_gep)
+                        self.generated_bulk_gep_counter += simulated_gep.shape[0]
+                        pbar.update(simulated_gep.shape[0])
+                        generated_cell_frac = generated_cell_frac.loc[simulated_gep.index, :].copy()
+                        selected_cell_ids = selected_cell_ids.loc[simulated_gep.index, :].copy()
+                        self._save_simulated_bulk_gep(gep=simulated_gep, cell_id=selected_cell_ids,
+                                                      cell_fraction=generated_cell_frac)
+                    self.n_round += 1
+            msg = f'   > Got {self.generated_bulk_gep_counter} samples from {self.n_round * min_n_cell_frac}'
+            if sampling_method in ['segment', 'seg_random']:
+                q_dis = 'radius' if filtering_method == 'marker_ratio' else 'l1 distance'
+                if self.q_dis_nn_ref_lower is not None:
+                    msg = f'   > Got {self.generated_bulk_gep_counter} samples from {self.n_round * min_n_cell_frac} ' \
+                          f'within {q_dis} between {self.q_dis_nn_ref_lower} and {self.q_dis_nn_ref_upper} ' \
+                          f'by quantile {self.filtering_quantile_lower * 100}%-{self.filtering_quantile_upper * 100}%'
+                else:
+                    msg = f'   > Got {self.generated_bulk_gep_counter} samples from {self.n_round * min_n_cell_frac} ' \
+                          f'within {q_dis} {self.q_dis_nn_ref_upper} by quantile {self.filtering_quantile_upper * 100}%'
+            print(msg)
+            data_info = f'Simulated {self.generated_bulk_gep_counter} bulk cell gene expression profiles ' \
+                        f'by {sampling_method}, log2(TPM + 1)'
+            create_h5ad_dataset(simulated_bulk_exp_file_path=self.generated_bulk_gep_csv_fp,
+                                cell_fraction_file_path=self.generated_cell_fraction_fp,
+                                dataset_info=data_info,
+                                result_file_path=self.generated_bulk_gep_fp)
+            if log_file_path is not None:
+                obj_info = self.__str__()
+                print_msg(obj_info, log_file_path=log_file_path)
+        else:
+            print(f'   Previous result existed: {self.generated_bulk_gep_fp}')
+            print(self.__str__())
+
+    def _filter_gep_by_reference(self, simulated_gep, n_top: int = None) -> Union[pd.DataFrame, None]:
+        """
+        Filtering generated GEP by reference dataset, such as TCGA
+
+        :param simulated_gep: simulated GEPs that need to filter by reference, TPM
+        :param n_top: if too many neighbors were founded for one single sample, only keep n_top neighbors
+        """
+
+        # print(marker_ratio_ref.head(2))
+        exp_obj_simu_gep = ExpObj(exp_file=simulated_gep, exp_type='TPM')
+        exp_obj_simu_gep.cal_marker_gene_ratio(agg_methods={'CD4 T': 'max', 'B Cells': 'max'},
+                                               cell_types=self.cell_type_used)
+        marker_ratio_simu_gep = exp_obj_simu_gep.get_marker_ratios()
+
+        # the distance of nearest neighbor for each sample
+        # quantile = 0.999
+        if self.q_dis_nn_ref_upper == 0:
+            qn1 = QueryNeighbors(df_file=self.marker_ratio_ref)
+            # quantile of distance
+            self.q_dis_nn_ref_upper = qn1.get_quantile_of_nn_distance(quantile=self.filtering_quantile_upper)
+            print(f'   > Quantile distance of {self.filtering_quantile_upper * 100}% is: {self.q_dis_nn_ref_upper}')
+        # nn_dis = qn1.get_nn()
+
+        qn2 = QueryNeighbors(df_file=marker_ratio_simu_gep)
+        current_ref_nc = sorted(self.ref_neighbor_counter.items(), key=lambda x: x[1])
+        _keep_ref = [i for i, j in current_ref_nc if j < self.n_neighbors_each_ref]
+        ref_neighbors_within_radius = qn2.get_neighbors_by_radius(
+            radius=self.q_dis_nn_ref_upper, n_top=n_top, share_neighbors=False,
+            q_df_file=self.marker_ratio_ref.loc[_keep_ref, :].copy(),
+            )
+        ref2n_neighbors = ref_neighbors_within_radius.groupby(ref_neighbors_within_radius.index).count()
+        _keep_neighbors = []
+        for i, n_n in ref2n_neighbors.iterrows():
+            self.ref_neighbor_counter[i] += n_n['nn']
+        # print(f'   There are {ref_neighbors_within_radius.shape[0]} simulated GEPs left after filtering.')
+        if ref_neighbors_within_radius.shape[0] > 0:
+            return simulated_gep.loc[ref_neighbors_within_radius['nn'], :].copy()
+        else:
+            return None
+
+    def read_merged_single_cell_dataset(self):
+        if self.merged_sc_dataset is None:
+            self.merged_sc_dataset = ReadH5AD(self.merged_sc_fp).get_h5ad()
+
+    def read_generated_single_cell_dataset(self):
+        if self.generated_sc_fp is None or (not os.path.exists(self.generated_sc_fp)):
+            raise FileNotFoundError('   Please generate single cell dataset first '
+                                    'using function "generate_single_cell_dataset", and try again.')
+        generated_sc_dataset_obj = ReadH5AD(self.generated_sc_fp)
+        generated_sc_dataset = generated_sc_dataset_obj.get_h5ad()
+        self.generated_sc_dataset_obs = generated_sc_dataset.obs.copy()
+        self.generated_sc_dataset_df = generated_sc_dataset_obj.get_df(convert_to_tpm=True)
+
+    def get_info_in_merged_single_cell_dataset(self, check_zero_ratio: bool = True,
+                                               zero_ratio_threshold: float = 0.95):
+        if self.merged_sc_dataset is None:
+            self.read_merged_single_cell_dataset()
+        self.cell_type_in_sc = list(self.merged_sc_dataset.obs['cell_type'].unique())
+        self.dataset_in_sc = list(self.merged_sc_dataset.obs['dataset_id'].unique())
+        # self.merged_sc_dataset_obs = self.merged_sc_dataset.obs.copy()
+        # always removing this part: marker genes of CD4 T cells expressed high in CD8 T cells
+        self.merged_sc_dataset_obs = \
+            self.merged_sc_dataset.obs.loc[~((self.merged_sc_dataset.obs['cell_type'] == 'CD8 T')
+                                           & (self.merged_sc_dataset.obs['m_cd4/m_cd8 group'] == 'high')), :].copy()
+        self.merged_sc_dataset_obs['sample_id'] = \
+            self.merged_sc_dataset_obs['sample_id'].cat.add_categories('pan_cancer')
+        # add sample_id for pan_cancer_07 dataset to use groupby later
+        self.merged_sc_dataset_obs.loc[self.merged_sc_dataset_obs['dataset_id'] == 'pan_cancer_07',
+                                       'sample_id'] = 'pan_cancer'
+        # The unique gene expression values of each gene in different cell types (merged scRNA-seq dataset)
+        self.unique_exp_value_in_s0 = self.merged_sc_dataset.uns['unique_exp_values']
+        self.merged_sc_dataset = None
+        if check_zero_ratio:
+            if self.sc_dataset_gep_type == 'log_space':
+                self.merged_sc_dataset_df = ReadH5AD(self.merged_sc_fp).get_df(convert_to_tpm=True)
+            else:
+                self.merged_sc_dataset_df = ReadH5AD(self.merged_sc_fp).get_df()
+            zero_ratio = np.sum(self.merged_sc_dataset_df < 1, axis=1) / self.merged_sc_dataset_df.shape[1]
+            high_zero_ratio_cells = zero_ratio[zero_ratio > zero_ratio_threshold].index.to_list()
+            # remove high zero ratio cells
+            print(f'   The zero ratio of {len(high_zero_ratio_cells)} cells '
+                  f'> {zero_ratio_threshold} and will be removed.')
+            self.merged_sc_dataset_obs = self.merged_sc_dataset_obs.loc[
+                                         ~self.merged_sc_dataset_obs.index.isin(high_zero_ratio_cells), :].copy()
+
+    def _sc_sampling(self, cell_frac: pd.DataFrame, obs_df: pd.DataFrame,
+                     n_threads: int = 10, total_cell_number: int = None, sep_by_patient=False):
+        """
+        Mix single cell expression profiles to simulated bulk expression profile according to `cell_frac`.
+
+        :param cell_frac: dataFrame, generated cell fraction for each cell type, samples by cell types
+
+        :param n_threads: how many thread to use
+
+        :param obs_df: a dataFrame of sample info for sampling
+
+        :param total_cell_number: N, total cell number to sample for each simulated bulk sample
+
+        :param sep_by_patient: whether to separate samples by patient or not during sampling
+
+        :return: sampled cell_ids
+        """
+        if total_cell_number is not None:
+            self.total_cell_number = total_cell_number
+        # if self.obs_df is None:
+        #     self.obs_df = obs_df
+        cell_num = get_cell_num(cell_type_frac=cell_frac, total_num=self.total_cell_number)
+        # print('   Start to select cells randomly based on cell types for generating each bulk expression profile...')
+        # all cell types of each cell only need to select one SCT from self.obs_df
+        # all_cell_num_is_one = np.all(cell_num == 1)
+        cell_num_flatten = []
+        # n_samples = cell_frac.shape[0]
+        for cell_type in cell_num.columns:
+            _part = pd.DataFrame(index=cell_num.index)
+            _part['cell_type'] = cell_type
+            _part['n_cell'] = cell_num[cell_type]
+            # if all_cell_num_is_one:
+            #     _selected_cell_ids = self.obs_df.loc[self.obs_df['cell_type'] == cell_type,
+            #                                          :].sample(n=n_samples).index.to_list()
+            #     _part['selected_cell_id'] = _selected_cell_ids
+            cell_num_flatten.append(_part)
+        sampled_cell_ids = pd.concat(cell_num_flatten)
+        # contains all cell types for each single simulated bulk expression profile
+        # if not all_cell_num_is_one:
+        paras = [(obs_df, 1, row['cell_type'], row['n_cell'], 'cell_type', sep_by_patient)
+                 for i, row in sampled_cell_ids.iterrows()]
+        n_threads = min(multiprocessing.cpu_count()-2, n_threads)
+        # https://pythonspeed.com/articles/python-multiprocessing/
+        with multiprocessing.get_context('spawn').Pool(n_threads) as p:
+            results = p.starmap(get_sample_id, paras)
+        # print(results)
+        results_str = [';'.join(i) for i in results]
+        sampled_cell_ids['selected_cell_id'] = results_str
+        sampled_cell_ids.index.name = 'sample_id'
+        sampled_cell_ids.sort_values(by=['sample_id', 'cell_type'], inplace=True)
+
+        return sampled_cell_ids
+
+    @staticmethod
+    def _sample_noise(miu=0, s=566.1, f=0.25, n_samples=10000) -> np.ndarray:
+        """
+        Generate noise for each gene in one bulk GEP, modified from Hao, Yuning, et al. PLoS Computational Biology, 2019
+
+        :param miu: mean of normal distribution
+        :param s: the mean std of all samples in TCGA with TPM values, LGG and GBM were excluded
+        """
+        sigma = f * np.log2(s)
+        norm_dis = stats.norm(miu, sigma)
+        x = norm_dis.rvs(size=n_samples)
+        return np.power(2, x)
+
+    def _map_cell_id2exp(self, selected_cell_id, sc_dataset: str = 'merged_sc_dataset',
+                         simu_method: str = 'ave', cell_frac: pd.DataFrame = None,
+                         gep_type='MCT', add_noise: bool = False, noise_params: tuple = ()) -> pd.DataFrame:
+        """
+        mapping sampled cell_ids to the corresponding GEPs
+        :param selected_cell_id: a dataFrame which contains cell_type, n_cell, selected_cell_id
+        :param sc_dataset: merged_sc_dataset, generated_sc_dataset or sct_dataset
+        :param simu_method: ave (average all selected single cell GEPs), mul (multiple GEP by cell fractions)
+        :param gep_type: MCT means multiple cell types (bulk GEP), SCT means single cell type
+        :return: a DataFrame, TPM, samples by genes
+        """
+        if sc_dataset == 'sct_dataset':
+            sc_ds_df = self.sct_dataset_df
+        elif sc_dataset == 'merged_sc_dataset':
+            sc_ds_df = self.merged_sc_dataset_df
+        else:  # generated single cell dataset
+            sc_ds_df = self.generated_sc_dataset_df
+        simulated_exp = {}
+        if gep_type == 'SCT':  # each sample id only contains single cell type
+            selected_cell_id = selected_cell_id.loc[selected_cell_id['n_cell'] > 1, :].copy()
+            # n_non_zero = 1000
+            n_genes = sc_ds_df.shape[1]
+            for cell_type, group in selected_cell_id.groupby('cell_type'):
+                for sample_id, row in group.iterrows():
+                    cell_ids = row['selected_cell_id'].split(';')
+                    # simulated_exp[sample_id] = sc_ds_df.loc[cell_ids, :].mean(axis=0)  # average
+                    current_gene_exp = sc_ds_df.loc[cell_ids, :].mean(axis=0)  # average
+                    if simu_method == 'random_replacement':
+                        # long_tail_noise_non_zero = np.random.random(n_non_zero) * 2
+                        # n_zero = np.random.randint(n_non_zero/10, n_non_zero)
+                        # long_tail_noise = np.append(long_tail_noise_non_zero, np.zeros(n_zero))
+                        long_tail_noise = np.random.random(size=n_genes)
+                        # replace the values < 1 with random selected values
+                        mask = (current_gene_exp < 1).values.astype(int)
+                        current_gene_exp = current_gene_exp + long_tail_noise * mask
+                    simulated_exp[sample_id] = pd.Series(current_gene_exp.values, index=current_gene_exp.index)
+        else:
+            assert simu_method == 'mul', 'Only support matrix multiplication for generating MCT'
+            for sample_id, group in selected_cell_id.groupby(by=selected_cell_id.index):
+                all_n_cell_is_one = np.all(group['n_cell'] == 1)
+                assert all_n_cell_is_one, 'n_cell should be 1 for all cell types'
+                cell_ids = group['selected_cell_id'].to_list()
+                current_merged = sc_ds_df.loc[cell_ids, :].copy()
+                # using merged single cell dataset directly
+
+                # sort by cell types to make sure the correction of matrix multiplication
+                _cell_types = group['cell_type'].to_list()
+                current_cell_frac = cell_frac.loc[sample_id, _cell_types].copy().to_frame()
+                # current_cell_frac = current_cell_frac.loc[group['cell_type'].to_list(), :]
+                simulated_exp[sample_id] = pd.Series((current_merged.values.T @ current_cell_frac.values).reshape(-1),
+                                                     index=current_merged.columns)
+                if add_noise:
+                    assert len(noise_params) == 2, 'noise_params should be a tuple of (f, total_max)'
+                    noise = self._sample_noise(n_samples=len(simulated_exp[sample_id]), f=noise_params[0])
+                    if noise.sum() > noise_params[1]:
+                        noise = noise / np.sum(noise) * noise_params[1]
+                    simulated_exp[sample_id] = simulated_exp[sample_id] + noise
+
+        simulated_exp_df = pd.DataFrame.from_dict(data=simulated_exp, orient='index')
+        simulated_exp_df = non_log2cpm(simulated_exp_df, sum_exp=1e6)  # convert to TPM
+        return simulated_exp_df.round(3)
+
+    def _save_simulated_bulk_gep(self, gep: pd.DataFrame, cell_id: pd.DataFrame, cell_fraction: pd.DataFrame = None):
+
+        if not os.path.exists(self.generated_bulk_gep_csv_fp):
+            gep.to_csv(self.generated_bulk_gep_csv_fp, float_format='%g')
+        else:
+            gep.to_csv(self.generated_bulk_gep_csv_fp, header=False, mode='a', float_format='%g')
+
+        if not os.path.exists(self.sampled_sc_cell_id_file_path):
+            cell_id.to_csv(self.sampled_sc_cell_id_file_path)
+        else:
+            cell_id.to_csv(self.sampled_sc_cell_id_file_path, header=False, mode='a')
+
+        if cell_fraction is not None:
+            if not os.path.exists(self.generated_cell_fraction_fp):
+                cell_fraction.to_csv(self.generated_cell_fraction_fp, float_format='%g')
+            else:
+                cell_fraction.to_csv(self.generated_cell_fraction_fp, header=False, mode='a', float_format='%g')
+
+        if self.ref_neighbor_counter:
+            pd.DataFrame.from_dict(self.ref_neighbor_counter, orient='index').to_csv(self.ref_neighbor_counter_fp)
+
+    def _check_intermediate_generated_gep(self):
+        """
+        if the generation process broke accidentally,
+        generated intermediate result can be used to recovery generation process
+        """
+        if os.path.exists(self.generated_cell_fraction_fp):
+            gen_cell_frac = pd.read_csv(self.generated_cell_fraction_fp, index_col=0)
+            gen_cell_frac = gen_cell_frac[~gen_cell_frac.index.duplicated(keep='first')].copy()
+            if os.path.exists(self.generated_bulk_gep_csv_fp):
+                gen_bulk_gep = pd.read_csv(self.generated_bulk_gep_csv_fp, index_col=0, usecols=[0, 1])
+                gen_bulk_gep = gen_bulk_gep[~gen_bulk_gep.index.duplicated(keep='first')].copy()
+                common_inx = [i for i in gen_cell_frac.index if i in gen_bulk_gep.index]
+                if (len(common_inx) == gen_bulk_gep.shape[0]) and (len(common_inx) == gen_cell_frac.shape[0]):
+                    self.generated_bulk_gep_counter = len(common_inx)
+                    if 'seg_random' in gen_cell_frac.iloc[-1].name:
+                        n_round = int(gen_cell_frac.iloc[-1].name.split('_')[3])
+                    else:
+                        n_round = int(gen_cell_frac.iloc[-1].name.split('_')[2])
+                    self.n_round = n_round + 1
+                    print(f'   The following intermediate generated result will be reused: \n'
+                          f'{self.generated_cell_fraction_fp}, {self.generated_bulk_gep_csv_fp}.\n'
+                          f'self.n_round will be reset to {self.n_round}, '
+                          f'self.generated_bulk_gep_counter will be reset to {self.generated_bulk_gep_counter}')
+                    if os.path.exists(self.ref_neighbor_counter_fp):
+                        ref2n_neighbors = pd.read_csv(self.ref_neighbor_counter_fp, index_col=0).to_dict()['0']
+                        self.ref_neighbor_counter = ref2n_neighbors.copy()
+                else:
+                    os.remove(self.generated_cell_fraction_fp)
+                    os.remove(self.generated_bulk_gep_csv_fp)
+                    os.remove(self.sampled_sc_cell_id_file_path)
+
+    def _check_basic_info(self):
+        """
+        check cell types and dataset
+        """
+        self.get_info_in_merged_single_cell_dataset(zero_ratio_threshold=self.zero_ratio_threshold)
+        cell_type_not_in_sc = [i for i in self.cell_type_used if i not in self.cell_type_in_sc]
+        dataset_not_in_sc = [i for i in self.sc_dataset_used if i not in self.dataset_in_sc]
+        if len(cell_type_not_in_sc) > 0:
+            invalid_cell_types = ', '.join(cell_type_not_in_sc)
+            valid_cell_types = ', '.join(self.cell_type_in_sc)
+            raise ValueError(f'   Invalid cell types: {invalid_cell_types}, '
+                             f'only the following cell types existed in single cell dataset: {valid_cell_types}')
+        else:
+            used_cell_types = ', '.join(self.cell_type_used)
+            print(f'   The following cell types will be used: {used_cell_types}')
+
+        if len(dataset_not_in_sc) > 0:
+            invalid_datasets = ', '.join(dataset_not_in_sc)
+            valid_datasets = ', '.join(self.dataset_in_sc)
+            raise ValueError(f'   Invalid datasets: {invalid_datasets}, '
+                             f'only the following datasets existed in single cell dataset: {valid_datasets}')
+        else:
+            used_datasets = ', '.join(self.sc_dataset_used)
+            print(f'   The following datasets will be used: {used_datasets}')
+
+    def _read_sct_dataset(self, latent_z_nn_info_file=None):
+        """
+        positive samples of SCT (single cell type), generated by BulkGEPGeneratorSCT
+        :param latent_z_nn_info_file: neighbor information of latent z for all samples, used for QC
+        """
+        sct_dataset_obs, sct_dataset_df = \
+            read_single_cell_type_dataset(sct_dataset_file_path=self.sct_dataset_file_path,
+                                          latent_z_nn_info_file=latent_z_nn_info_file)
+        return sct_dataset_obs, sct_dataset_df
+
+    def __str__(self):
+        _dict = {k: v for k, v in self.__dict__.items() if type(v) in [list, str, int, float]}
+        return str(self.__class__) + ':\n' + json.dumps(_dict, indent=2)
+
+
+class SingleCellTypeGEPGenerator(BulkGEPGenerator):
+    """
+    Generating single cell GEPs (scGEPs)
+
+    :param simu_bulk_dir: the directory to save simulated bulk cell GEPs
+    :param merged_sc_dataset_file_path: the file path of pre-merged single cell datasets
+    :param cell_types: cell types used when generating bulk GEPs
+    :param sc_dataset_ids: single cell dataset id used when generating bulk GEPs
+    :param bulk_dataset_name: the name of generated bulk dataset, only for naming
+    :param zero_ratio_threshold: the threshold of zero ratio of genes in single cell GEPs, remove the GEP if zero ratio > threshold
+    :param sc_dataset_gep_type: the type of single cell GEPs, `log_space` or `linear_space`
+    """
+    def __init__(self, merged_sc_dataset_file_path, cell_types, sc_dataset_ids,
+                 simu_bulk_dir, bulk_dataset_name, zero_ratio_threshold: float = 0.97,
+                 sc_dataset_gep_type: str = 'log_space'):
+        super().__init__(merged_sc_dataset_file_path=merged_sc_dataset_file_path, simu_bulk_dir=simu_bulk_dir,
+                         cell_types=cell_types, sc_dataset_ids=sc_dataset_ids, bulk_dataset_name=bulk_dataset_name,
+                         zero_ratio_threshold=zero_ratio_threshold, sct_dataset_file_path=None,
+                         sc_dataset_gep_type=sc_dataset_gep_type)
+
+    def generate_samples(self, n_sample_each_cell_type: int = 10000,
+                         n_base_for_positive_samples: int = 100,
+                         sample_type: str = 'positive', sep_by_patient=False,
+                         simu_method='ave', cell_type2subgroup_id: dict = None, subgroup_by: list = None):
+        """
+        :param n_sample_each_cell_type: the number of samples to generate for each cell type
+
+        :param n_base_for_positive_samples: the number of single cells to average
+
+        :param sample_type: positive means only 1 cell type is used, negative means more than 1 cell types are used
+
+        :param sep_by_patient: only sampling from one patient in original dataset if True
+
+        :param simu_method: `ave`: averaging all GEPs, or `scale_by_mGEP`: scaling by the mean GEP of all samples in the TCGA dataset
+            or `random_replacement`: replacing the gene expression value (<1) by another value within the same cell type selected randomly
+
+        :param cell_type2subgroup_id: a dict, key is cell type, value is a list of subgroup ids
+        :param subgroup_by: a list of column names in the merged single cell dataset, used to group samples
+        """
+        if not os.path.exists(self.generated_bulk_gep_fp):
+            if subgroup_by is None:
+                subgroup_by = ['dataset_id', 'leiden']
+            self.n_samples = n_sample_each_cell_type * len(self.cell_type_used)
+            if not os.path.exists(self.generated_cell_fraction_fp):
+                print(f'   Generate cell proportions for single cell type (SCT) samples in {self.bulk_dataset_name}')
+                generated_cell_frac = self.generate_frac_sc(
+                    sample_type=sample_type, sample_prefix=f'sct_{self.bulk_dataset_name}_{sample_type[:3]}'
+                )
+                generated_cell_frac.to_csv(self.generated_cell_fraction_fp, float_format='%g')
+            else:
+                print(f'   Previous result exists: {self.generated_cell_fraction_fp}')
+            # DC has 543 cells, larger chunk_size can cause error if set 'replace=False' and 'n_base=1' while sampling
+            chunk_size_factor = max([len(v) for k, v in cell_type2subgroup_id.items()])
+            if chunk_size_factor <= 10:
+                chunk_size_factor = 10
+            elif 10 < chunk_size_factor <= 20:
+                chunk_size_factor = 20
+            elif 20 < chunk_size_factor <= 50:
+                chunk_size_factor = 50
+            chunk_size = int(n_sample_each_cell_type / chunk_size_factor)
+            # if n_base_for_positive_samples == 1:
+            #     chunk_size = 300
+            # else:
+            #     chunk_size = 1000
+            chunk_counter = 0
+            with pd.read_csv(self.generated_cell_fraction_fp, chunksize=chunk_size, index_col=0) as reader:
+                simu_method = simu_method  # average single cell GEPs for both positive and negative sampling
+                for rows in tqdm(reader):
+                    if sample_type == 'positive' and n_base_for_positive_samples > 1:
+                        total_cell_number = n_base_for_positive_samples
+                    else:  # negative sampling (multiple cell types are used) or positive sampling with n_base=1
+                        total_cell_number = 0  # assign 1 for the cell types with non-zero cell fractions
+                    if sample_type == 'positive' and cell_type2subgroup_id is not None:
+                        # change subgroup for each chunk based on cell_type2subgroup_id
+                        all_cell_types = rows.columns[np.argmax(rows.values, axis=1)].unique()
+                        if len(all_cell_types) > 1:
+                            raise ValueError(f'   More than one cell types are selected: {all_cell_types}')
+                        cell_type = all_cell_types[0]
+                        current_subgroups = cell_type2subgroup_id[cell_type]
+                        selected_subgroup = current_subgroups[chunk_counter % chunk_size_factor % len(current_subgroups)]
+                        if len(subgroup_by) == 1 and subgroup_by[0] in self.merged_sc_dataset_obs.columns:
+                            current_obs_df = self.merged_sc_dataset_obs.loc[
+                                             self.merged_sc_dataset_obs[subgroup_by[0]].isin(selected_subgroup),
+                                             :].copy()
+                        elif len(subgroup_by) == 2 and set(subgroup_by).issubset(self.merged_sc_dataset_obs.columns):
+                            current_obs_df = self.merged_sc_dataset_obs.loc[
+                                             (self.merged_sc_dataset_obs[subgroup_by[0]].isin([selected_subgroup[0]])) &
+                                             (self.merged_sc_dataset_obs[subgroup_by[1]].isin([selected_subgroup[1]])),
+                                             :].copy()
+                        else:
+                            raise ValueError(f'   subgroup_by {subgroup_by} is not valid')
+                    else:
+                        current_obs_df = self.merged_sc_dataset_obs.copy()
+                    selected_cell_ids = self._sc_sampling(cell_frac=rows, total_cell_number=total_cell_number,
+                                                          obs_df=current_obs_df,
+                                                          sep_by_patient=sep_by_patient)
+                    simulated_gep = self._map_cell_id2exp(selected_cell_id=selected_cell_ids, simu_method=simu_method,
+                                                          cell_frac=rows, sc_dataset='merged_sc_dataset', gep_type='SCT')
+                    simulated_gep = log2_transform(simulated_gep)
+                    self.generated_bulk_gep_counter += simulated_gep.shape[0]
+                    # generated_cell_frac = generated_cell_frac.loc[simulated_gep.index, :].copy()
+                    selected_cell_ids = selected_cell_ids.loc[simulated_gep.index, :].copy()
+                    self._save_simulated_bulk_gep(gep=simulated_gep, cell_id=selected_cell_ids)
+                    chunk_counter += 1
+
+            data_info = f'Simulated {self.generated_bulk_gep_counter} gene expression profiles ' \
+                        f'for each cell type, log2(TPM + 1)'
+            create_h5ad_dataset(simulated_bulk_exp_file_path=self.generated_bulk_gep_csv_fp,
+                                cell_fraction_file_path=self.generated_cell_fraction_fp,
+                                dataset_info=data_info,
+                                result_file_path=self.generated_bulk_gep_fp)
+        else:
+            print(f'   Previous result exists: {self.generated_bulk_gep_fp}')
+
+    def generate_frac_sc(self, sample_prefix: str = None, sample_type: str = 'positive') -> pd.DataFrame:
+        """
+        Generate cell fractions for single cell samples, positive samples only contain one specific cell type,
+        negative samples contain >= 2 cell types with equal proportion
+
+        :param sample_prefix: prefix of sample names
+
+        :param sample_type: positive samples (one specific cell type) or negative samples (>= 2 cell types)
+
+        :return:  generated cell fraction, sample by cell type
+        """
+        if sample_prefix is None:
+            sample_prefix = f's_sc_{sample_type}'
+        n_cell_types = len(self.cell_type_used)
+        generated_frac_df = pd.DataFrame(index=[f'{sample_prefix}_{i}' for i in range(self.n_samples)],
+                                         columns=self.cell_type_used,
+                                         data=np.zeros((self.n_samples, n_cell_types)))
+        if sample_type == 'positive':
+            n_for_each_cell_type = int(self.n_samples / n_cell_types)
+            for i, cell_type in enumerate(self.cell_type_used):
+                inx_start = i * n_for_each_cell_type
+                inx_end = min((i+1) * n_for_each_cell_type, self.n_samples)
+                generated_frac_df.iloc[inx_start:inx_end, i] = 1
+        else:  # negative samples
+            n_for_each_n_ct = int(self.n_samples / (n_cell_types - 1))
+            for n_ct in range(2, n_cell_types+1):  # the number of cell types used (=2)
+                inx_start = (n_ct-2) * n_for_each_n_ct
+                inx_end = min((n_ct-1) * n_for_each_n_ct, self.n_samples)
+                frac = 1 / n_ct
+                for inx in range(inx_start, inx_end):
+                    if n_ct < n_cell_types:
+                        current_cell_type_inx = np.random.choice(range(n_cell_types), size=n_ct, replace=False)
+                    else:
+                        current_cell_type_inx = np.array(range(n_cell_types))
+                    generated_frac_df.iloc[inx, current_cell_type_inx] = frac
+        return generated_frac_df.round(4)
+
+
+class BulkGEPGeneratorSCT(BulkGEPGenerator):
+    """
+    generate bulk GEPs by cell proportion x single GEP of single cell type (SCT)
+    """
+    def __init__(self, sct_dataset_file_path, cell_types, simu_bulk_dir, bulk_dataset_name):
+        super().__init__(simu_bulk_dir=simu_bulk_dir, cell_types=cell_types, bulk_dataset_name=bulk_dataset_name,
+                         merged_sc_dataset_file_path=None, check_basic_info=False, sc_dataset_ids=[],
+                         sct_dataset_file_path=sct_dataset_file_path)
+        # self.sct_dataset_file_path = sct_dataset_file_path
+        # self.sct_dataset_obs = None
+        # self.sct_dataset_df = None
+
+    def generate_samples(self, n_samples, latent_z_nn_file_path: str = None,
+                         ref_distribution: dict = None, sampling_method: str = 'fragment',
+                         total_cell_number: int = 1, n_threads: int = 10,
+                         log_file_path: str = None, cell_prop_file_path: str = None, add_token_cell_type: bool = False,
+                         random_n_cell_type: list = None):
+        """
+        :param n_samples: the number of GEPs to generate
+        :param latent_z_nn_file_path: neighbor information of latent z for all samples, used for QC and sampling
+        :param total_cell_number: N, the total number of cells sampled from merged single cell dataset
+                                      and averaged to simulate a single bulk RNA-seq sample
+        :param sampling_method: segment or random, method to generate cell fractions
+        :param ref_distribution: reference distribution for each cell type, seperated to 10 bins for [0, 1]
+            {'B Cells': [0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1], '': [], '': [], ...}
+            only used for fragment sampling method when call function self._generate_cell_fraction
+        :param n_threads: number of threads used for parallel computing
+        :param log_file_path:
+        :param cell_prop_file_path: file path of pre-generated cell proportion, use this file if provided
+        :param add_token_cell_type: add all cell types in generated_cell_frac.csv file,
+             even if some cell types take 0% in all samples, only for keeping same format for all dataset
+        :param random_n_cell_type: a list of the number of cell types (selected randomly) used for simulating bulk GEPs
+        """
+        n_total_cpus = multiprocessing.cpu_count()
+        n_threads = min(n_total_cpus - 1, n_threads)
+        self.n_samples = n_samples
+        self.total_cell_number = total_cell_number  # set 1 for all cell types
+        # simulating bulk cell GEP by mixing GEPs of different cell types
+        min_n_cell_frac = np.min([100, n_samples])  # smaller number of samples without filtering
+        if cell_prop_file_path is not None:
+            self.generated_cell_fraction_fp = cell_prop_file_path
+        if not os.path.exists(self.generated_bulk_gep_fp):
+            self.sct_dataset_obs, self.sct_dataset_df = self._read_sct_dataset(latent_z_nn_info_file=
+                                                                              latent_z_nn_file_path)
+
+            if not os.path.exists(self.generated_cell_fraction_fp):
+                print(f'   Generate cell proportions for bulk samples in {self.bulk_dataset_name}')
+                generated_cell_frac = self._generate_cell_fraction(
+                    sampling_method=sampling_method, n_cell_frac=self.n_samples,
+                    sample_prefix=f's_{self.bulk_dataset_name}_{sampling_method}_0',
+                    ref_distribution=ref_distribution,
+                    random_n_cell_type=random_n_cell_type,
+                )
+                if add_token_cell_type:
+                    for ct in sorted_cell_types:
+                        if ct not in generated_cell_frac.columns:
+                            generated_cell_frac[ct] = 0
+                    generated_cell_frac = generated_cell_frac.loc[:, sorted_cell_types]
+                generated_cell_frac.to_csv(self.generated_cell_fraction_fp, float_format='%g')
+            else:
+                print(f'   Previous result exists: {self.generated_cell_fraction_fp}')
+
+            chunk_size = int(self.n_samples / min_n_cell_frac)
+            chunk_size = max(chunk_size, 100)
+            chunk_counter = 0
+            with pd.read_csv(self.generated_cell_fraction_fp, chunksize=chunk_size, index_col=0) as reader:
+                simu_method = 'mul'  # matrix multiplication
+                for rows in tqdm(reader):
+
+                    selected_cell_ids = self._sc_sampling(cell_frac=rows,
+                                                          n_threads=n_threads, obs_df=self.sct_dataset_obs)
+                    simulated_gep = self._map_cell_id2exp(selected_cell_id=selected_cell_ids, cell_frac=rows,
+                                                          sc_dataset='sct_dataset', simu_method=simu_method)
+
+                    simulated_gep = log2_transform(simulated_gep)
+                    self.generated_bulk_gep_counter += simulated_gep.shape[0]
+                    # generated_cell_frac = generated_cell_frac.loc[simulated_gep.index, :].copy()
+                    selected_cell_ids = selected_cell_ids.loc[simulated_gep.index, :].copy()
+                    self._save_simulated_bulk_gep(gep=simulated_gep, cell_id=selected_cell_ids)
+                    chunk_counter += 1
+
+            data_info = f'Simulated {self.generated_bulk_gep_counter} bulk cell gene expression profiles ' \
+                        f'by sampling method: {sampling_method}, simulation method: {simu_method}, log2(TPM + 1)'
+            create_h5ad_dataset(simulated_bulk_exp_file_path=self.generated_bulk_gep_csv_fp,
+                                cell_fraction_file_path=self.generated_cell_fraction_fp,
+                                dataset_info=data_info,
+                                result_file_path=self.generated_bulk_gep_fp)
+            if log_file_path is not None:
+                obj_info = self.__str__()
+                print_msg(obj_info, log_file_path=log_file_path)
+        else:
+            print(f'   Previous result existed: {self.generated_bulk_gep_fp}')
+            print(self.__str__())
+
+
+# for gene-level filtering
+def get_quantile(exp_df, quantile_range, col_name: list = None) -> pd.DataFrame:
+    """
+    Get quantile
+    :param exp_df:
+    :param quantile_range:
+    :param col_name:
+    :return:
+    """
+    quantile_df = pd.DataFrame(index=exp_df.columns, columns=col_name)
+    quantile_df[col_name[0]] = exp_df.quantile(quantile_range[0], axis=0)
+    quantile_df[col_name[1]] = exp_df.quantile(quantile_range[1], axis=0)
+    quantile_df[col_name[2]] = exp_df.quantile(quantile_range[2], axis=0)
+    return quantile_df
+
+
+def get_gene_list_for_filtering(bulk_exp_file, tcga_file, result_file_path, q_col_name: list = None,
+                                filtering_type: str = 'quantile_range',
+                                corr_threshold: float = 0.3, n_gene_max: int = 1000,
+                                corr_result_fp: str = None, quantile_range: list = None):
+    """
+    Gene-level filtering based on the filtering type
+    :param bulk_exp_file:
+    :param tcga_file:
+    :param filtering_type: high_corr_gene, quantile_range, all_genes, high_corr_gene_and_quantile_range
+      - high_corr_gene: expression values with high correlation with the cell proportions of any cell types
+      - quantile_range: the median of expression values within the [q_5, q_95] quantile range
+    :param corr_result_fp:
+    :param quantile_range: median gene expression (quantile_range[1], expected as 0.5) of simulated bulk cell GEPs that
+        is less than quantile_range[0] or greater than quantile_range[2] of the quantile expression value
+        of corresponding gene in TCGA dataset will be removed
+    :param result_file_path:
+    :param q_col_name:
+    :param corr_threshold: correlation threshold for gene filtering
+    :param n_gene_max: maximum number of genes for each cell type during gene filtering
+    :return:
+    """
+
+    assert filtering_type in ['high_corr_gene', 'quantile_range', 'all_genes', 'high_corr_gene_and_quantile_range'], \
+        f'filtering_type: {filtering_type} is not supported, only support high_corr_gene, quantile_range, all_genes, ' \
+        f'high_corr_gene_and_quantile_range'
+    if not os.path.exists(result_file_path):
+        bulk_exp = ReadH5AD(bulk_exp_file).get_df()
+        tcga_obj = ReadExp(tcga_file, exp_type='TPM')
+        tcga_obj.align_with_gene_list(
+            gene_list=bulk_exp.columns.to_list(),
+        )
+        tcga_obj.to_log2cpm1p()
+        tcga = tcga_obj.get_exp()
+        gene_list = []
+        if 'high_corr_gene' in filtering_type:
+            h5_obj = ReadH5AD(bulk_exp_file)
+            gene_exp = h5_obj.get_df(convert_to_tpm=True)
+            cell_frac = h5_obj.get_cell_fraction()
+            corr_df = cal_corr_gene_exp_with_cell_frac(gene_exp=gene_exp, cell_frac=cell_frac,
+                                                       result_file_path=corr_result_fp, filtered_by_corr=corr_threshold,
+                                                       filter_by_num=n_gene_max)
+            del gene_exp
+            gene_list = corr_df.index.to_list()
+            print(f'{len(gene_list)} genes are selected by high correlation')
+        if 'quantile_range' in filtering_type:
+            # both bulk_exp and tcga are in log-space
+            gene_list_qr = get_gene_list_filtered_by_quantile_range(bulk_exp=bulk_exp, tcga_exp=tcga,
+                                                                    quantile_range=quantile_range,
+                                                                    q_col_name=q_col_name)
+            print(f'{len(gene_list_qr)} genes are selected by quantile range')
+            if len(gene_list) > 0:  # if there is high correlation gene, then filter by high correlation gene
+                gene_list = [gene for gene in gene_list if gene in gene_list_qr]
+                print(f'{len(gene_list)} genes are selected by both high correlation and quantile range')
+            else:
+                gene_list = gene_list_qr
+        if filtering_type == 'all_genes':
+            gene_list = bulk_exp.columns.to_list()
+            print(f'All {len(gene_list)} genes will be used')
+
+        gene_list_df = pd.DataFrame(columns=['gene_name'])
+        gene_list_df['gene_name'] = gene_list
+        gene_list_df.to_csv(result_file_path, index=False)
+    else:
+        print(f'Loading the gene list from file: {result_file_path}')
+        gene_list_df = pd.read_csv(result_file_path)
+        gene_list = gene_list_df['gene_name'].to_list()
+    return gene_list
+
+
+def get_gene_list_filtered_by_quantile_range(bulk_exp, tcga_exp, quantile_range: list = None,
+                                             q_col_name: list = None, tcga_gene_info=None):
+    """
+    Get gene list filtered by quantile range
+    :param bulk_exp: bulk expression, TPM
+    :param tcga_exp: TCGA expression data, TPM
+    :param quantile_range: lower boundary, median, upper boundary, such as [0.025, 0.5, 0.975]
+    :param q_col_name: column names for quantile range
+    :param tcga_gene_info: gene quantile values in TCGA
+    """
+    if quantile_range is None:
+        quantile_range = [0.025, 0.5, 0.975]
+        q_col_name = ['q_' + str(int(q * 1000) / 10) for q in quantile_range]
+    if tcga_gene_info is None:
+        tcga_gene_info = get_quantile(tcga_exp, quantile_range=quantile_range, col_name=q_col_name)
+    if type(bulk_exp) is pd.DataFrame and bulk_exp.shape[0] > 1:
+        bulk_gene_info = get_quantile(bulk_exp, quantile_range=quantile_range, col_name=q_col_name)
+        gene_inx = (bulk_gene_info[q_col_name[1]] >= tcga_gene_info[q_col_name[0]]) & \
+                   (bulk_gene_info[q_col_name[1]] <= tcga_gene_info[q_col_name[2]])
+        gene_list_qr = bulk_exp.loc[:, gene_inx].columns.to_list()
+    else:  # if bulk_exp is a series
+        gene_inx = (bulk_exp >= tcga_gene_info[q_col_name[0]]) & (bulk_exp <= tcga_gene_info[q_col_name[2]])
+        gene_list_qr = bulk_exp.loc[gene_inx].index.to_list()
+    return gene_list_qr
+
+
+def cal_loading_by_pca(pca, gene_list, loading_matrix_file_path=None):
+    """
+    Cal loading by PCA
+    :param pca:
+    :param gene_list:
+    :param loading_matrix_file_path:
+    :return:
+    """
+    loading = pca.components_.T * np.sqrt(pca.explained_variance_)
+    # loading = loading.loc[:, gene_list]
+    com_matrix = pd.DataFrame(data=loading[:, 0:3], index=gene_list, columns=['PC1', 'PC2', 'PC3'])
+    com_matrix['PC1_abs'] = com_matrix['PC1'].abs()
+    com_matrix['PC2_abs'] = com_matrix['PC2'].abs()
+    com_matrix['PC3_abs'] = com_matrix['PC3'].abs()
+    com_matrix['PC_top3_sum'] = com_matrix.loc[:, ['PC1_abs', 'PC2_abs', 'PC3_abs']].sum(axis=1)
+    if loading_matrix_file_path is not None:
+        print(f'Saving loading matrix to file: {loading_matrix_file_path}')
+        com_matrix.to_csv(loading_matrix_file_path, index_label='gene_name')
+    return loading
+
+
+def filtering_by_gene_list_and_pca_plot(bulk_exp, tcga_exp, gene_list, result_dir, simu_dataset_name,
+                                        n_components=5, pca_model_name_postfix='', bulk_exp_type='log_space',
+                                        tcga_exp_type='TPM', pca_model_file_path=None, pca_data_file_path=None,
+                                        h5ad_file_path=None, cell_frac_file=None, figsize=(5, 5)):
+    """
+    Filtering by gene list and pca plot
+    :param bulk_exp: log2cpm1p
+    :param tcga_exp: TPM
+    :param gene_list:
+    :param result_dir:
+    :param n_components:
+    :param pca_model_name_postfix:
+    :param bulk_exp_type:
+    :param tcga_exp_type:
+    :param pca_model_file_path:
+    :param pca_data_file_path:
+    :param simu_dataset_name:
+    :param h5ad_file_path: save simulated bulk GEPs depending on filtered gene list to .h5ad file if not None
+    :param cell_frac_file:
+    :return:
+    """
+    bulk_obj = ReadExp(bulk_exp, exp_type=bulk_exp_type)
+    bulk_obj.align_with_gene_list(gene_list=gene_list)
+    bulk_exp = bulk_obj.get_exp()
+    tcga_obj = ReadExp(tcga_exp, exp_type=tcga_exp_type)
+    tcga_obj.align_with_gene_list(gene_list=gene_list)
+    tcga_obj.to_log2cpm1p()
+    tcga_exp = tcga_obj.get_exp()
+
+    # PCA and plot
+    check_dir(result_dir)
+    assert n_components >= 2, 'n_components must be >= 2'
+    if not os.path.exists(pca_data_file_path):
+        # combine both simulated bulk cell GEPs and TCGA dataset together
+        simu_bulk_with_tcga = pd.concat([bulk_exp, tcga_exp])
+        pca_model = do_pca_analysis(exp_df=simu_bulk_with_tcga, n_components=n_components,
+                                    pca_result_fp=pca_model_file_path)
+        pcs = pca_model.transform(simu_bulk_with_tcga)
+        if n_components >= 3:
+            pca_df = pd.DataFrame(pcs[:, range(3)], index=simu_bulk_with_tcga.index, columns=['PC1', 'PC2', 'PC3'])
+        else:
+            pca_df = pd.DataFrame(pcs[:, range(2)], index=simu_bulk_with_tcga.index, columns=['PC1', 'PC2'])
+        pca_df.to_csv(pca_data_file_path)
+    else:
+        print(f'{pca_data_file_path} already exists, skip PCA analysis')
+        pca_df = pd.read_csv(pca_data_file_path, index_col=0)
+        pca_model = load(pca_model_file_path)
+
+    # plot
+    title = f'{simu_dataset_name}_PCA_with_TCGA_{pca_model_name_postfix}'
+    color_code = np.array([simu_dataset_name] * bulk_exp.shape[0] + ['TCGA'] * tcga_exp.shape[0])
+    # cumsum = np.cumsum(pca_model.explained_variance_ratio_)
+    # pca_df['class'] = color_code
+    plot_pca(data=pca_df, figsize=figsize,
+             result_fp=os.path.join(result_dir, title + '.png'),
+             color_code=color_code, explained_variance_ratio=pca_model.explained_variance_ratio_)
+    if h5ad_file_path is not None:
+        assert cell_frac_file is not None, 'cell_frac_file should be provided if h5ad_file_path is not None'
+        print(f'Saving filtered bulk exp to file: {h5ad_file_path}')
+        if not os.path.exists(h5ad_file_path):
+            print('Saving as .h5ad file...')
+            dataset_info = f'Some genes were removed from this dataset for increasing the similarity ' \
+                           f'between TCGA and simulated bulk cell GEPs. This similarity was evaluated by PCA analysis.'
+            create_h5ad_dataset(simulated_bulk_exp_file_path=bulk_exp,
+                                cell_fraction_file_path=cell_frac_file, dataset_info=dataset_info,
+                                result_file_path=h5ad_file_path)
+
+
+if __name__ == '__main__':
+    # pass
+    # gene_samples = gradient_generation_fraction(n=2)
+    root_dir = r'F:\projects\001EMT-infiltration\analysis_result\014_test\nn_model'
+    # cell_frac = pd.read_csv(os.path.join(root_dir, 'generated_frac_n1.csv'), index_col=0)
+    # sc_fp = os.path.join(os.path.join(r'F:\projects\001EMT-infiltration\raw_data\single cells',
+    #                                   'generated_11_cell_type_n1000.h5ad'))
+    # simu_bulk_exp = simulate_bulk_expression(cell_frac=cell_frac, sc_exp_file_path=sc_fp)
+    # simu_bulk_exp.write(os.path.join(root_dir, 'simu_bulk_exp_n1.h5ad'))
+    # simu_bulk_n100_fp = os.path.join(root_dir, 'simu_bulk_exp_n100.h5ad')
+    # prefix = 'simu_bulk_exp_n10'
+    # simu_bulk_exp_fp = os.path.join(root_dir, prefix + '_log2cpm1p.csv')
+    # sc_fp = os.path.join(os.path.join(r'F:\projects\001EMT-infiltration\raw_data\single cells',
+    #                                   'generated_11_cell_type_n5000.h5ad'))
+    # cell_frac_fp = os.path.join(root_dir, 'generated_frac_test_set_n10.csv')
+    # if not os.path.exists(simu_bulk_exp_fp):
+    #     cell_frac = pd.read_csv(cell_frac_fp, index_col=0)
+    #     simulate_bulk_expression(cell_frac=cell_frac, sc_exp_file_path=sc_fp,
+    #                              n_threads=4, result_dir=root_dir, prefix=prefix)
+    #     simu_bulk_exp.to_csv(simu_bulk_n100_selected_id_fp)
```

### Comparing `DeSide-1.0.1/deside/simulation/stats_test.py` & `DeSide-1.0.2/deside/simulation/stats_test.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import numpy as np
-import pandas as pd
-import seaborn as sns
-import scipy.stats as stats
-from ..utility import print_df
-sns.set()
-
-
-def split_and_shuffle(exp_df, n):
-    """
-    Yield successive n-sized split_and_shuffle from a dataframe.
-    https://stackoverflow.com/a/48791962/2803344
-    :param exp_df: pandas.DataFrame
-        expression profile, genes x samples
-    :param n: how many samples in each subgroup
-    :return: a list of subgroup dataframe
-    """
-    sample_names = exp_df.columns.to_list()
-    np.random.shuffle(sample_names)
-    split_l = []
-    n_subgroup = []
-    for i in range(0, len(sample_names), n):
-        sub_group_sample_names = sample_names[i:i+n]
-        n_subgroup.append(len(sub_group_sample_names))
-        split_l.append(exp_df.loc[:, sub_group_sample_names])
-    print('>>> There are {} subgroups, each subgroup has {} samples.'.format(len(split_l),
-                                                                             ', '.join([str(i) for i in n_subgroup])))
-    return split_l
-
-
-def two_group_ttest(group_a, group_b):
-    """
-    T-test between two groups
-    :param group_a: pd.DataFrame
-        group A, genes x samples
-    :param group_b: pd.DataFrame
-        group B, genes x samples
-    :return: p-value of each gene between two groups
-    """
-    assert np.all(group_a.index == group_b.index), 'The order of genes in two groups should be same'
-    result = pd.DataFrame(index=group_a.index, columns=['pvalue'])
-    _, pvalue = stats.ttest_ind(group_a, group_b, axis=1, equal_var=False)
-    result['pvalue'] = np.round(pvalue, 4)
-    return result
-
-
-def test_normality(exp_df):
-    """
-    test the normality of each gene across all samples by Shapiro test
-    p >= 0.05 obey normal distribution
-    :param exp_df: genes x samples
-    :return:
-    """
-    exp_normality = pd.DataFrame(index=exp_df.index)
-    print_df(exp_df)
-    for gene in exp_df.index:
-        gene_exp = exp_df.loc[gene, :]
-        shapiro_test = stats.shapiro(gene_exp.values)
-        # exp_normality.loc[gene, 'Shapiro_Tn'] = shapiro_test.statistic
-        exp_normality.loc[gene, 'pvalue'] = shapiro_test.pvalue
-    return exp_normality
-
-
-def alpha_confidence_interval(gene_exp, alpha=0.05):
-    """
-    confidence interval (CI) of 1 - alpha in normal distribution
-    :param gene_exp: a single gene expression across all samples
-    :param alpha: significance level
-    :return: CI
-    """
-    norm_dis = stats.norm(np.mean(gene_exp), np.std(gene_exp))
-    min_ci = np.max([0, norm_dis.isf(1-alpha/2)])
-    max_ci = norm_dis.isf(alpha/2)
-    return [np.round(i, 3) for i in [min_ci, max_ci]]
-
-
-if __name__ == '__main__':
-    my_data = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K']
-    # print(split_and_shuffle(my_data, 4))
+import numpy as np
+import pandas as pd
+import seaborn as sns
+import scipy.stats as stats
+from ..utility import print_df
+sns.set()
+
+
+def split_and_shuffle(exp_df, n):
+    """
+    Yield successive n-sized split_and_shuffle from a dataframe.
+    https://stackoverflow.com/a/48791962/2803344
+    :param exp_df: pandas.DataFrame
+        expression profile, genes x samples
+    :param n: how many samples in each subgroup
+    :return: a list of subgroup dataframe
+    """
+    sample_names = exp_df.columns.to_list()
+    np.random.shuffle(sample_names)
+    split_l = []
+    n_subgroup = []
+    for i in range(0, len(sample_names), n):
+        sub_group_sample_names = sample_names[i:i+n]
+        n_subgroup.append(len(sub_group_sample_names))
+        split_l.append(exp_df.loc[:, sub_group_sample_names])
+    print('>>> There are {} subgroups, each subgroup has {} samples.'.format(len(split_l),
+                                                                             ', '.join([str(i) for i in n_subgroup])))
+    return split_l
+
+
+def two_group_ttest(group_a, group_b):
+    """
+    T-test between two groups
+    :param group_a: pd.DataFrame
+        group A, genes x samples
+    :param group_b: pd.DataFrame
+        group B, genes x samples
+    :return: p-value of each gene between two groups
+    """
+    assert np.all(group_a.index == group_b.index), 'The order of genes in two groups should be same'
+    result = pd.DataFrame(index=group_a.index, columns=['pvalue'])
+    _, pvalue = stats.ttest_ind(group_a, group_b, axis=1, equal_var=False)
+    result['pvalue'] = np.round(pvalue, 4)
+    return result
+
+
+def test_normality(exp_df):
+    """
+    test the normality of each gene across all samples by Shapiro test
+    p >= 0.05 obey normal distribution
+    :param exp_df: genes x samples
+    :return:
+    """
+    exp_normality = pd.DataFrame(index=exp_df.index)
+    print_df(exp_df)
+    for gene in exp_df.index:
+        gene_exp = exp_df.loc[gene, :]
+        shapiro_test = stats.shapiro(gene_exp.values)
+        # exp_normality.loc[gene, 'Shapiro_Tn'] = shapiro_test.statistic
+        exp_normality.loc[gene, 'pvalue'] = shapiro_test.pvalue
+    return exp_normality
+
+
+def alpha_confidence_interval(gene_exp, alpha=0.05):
+    """
+    confidence interval (CI) of 1 - alpha in normal distribution
+    :param gene_exp: a single gene expression across all samples
+    :param alpha: significance level
+    :return: CI
+    """
+    norm_dis = stats.norm(np.mean(gene_exp), np.std(gene_exp))
+    min_ci = np.max([0, norm_dis.isf(1-alpha/2)])
+    max_ci = norm_dis.isf(alpha/2)
+    return [np.round(i, 3) for i in [min_ci, max_ci]]
+
+
+if __name__ == '__main__':
+    my_data = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K']
+    # print(split_and_shuffle(my_data, 4))
```

### Comparing `DeSide-1.0.1/deside/single_cell/preprocessing.py` & `DeSide-1.0.2/deside/single_cell/preprocessing.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,673 +1,673 @@
-import os
-import numpy as np
-import pandas as pd
-import scanpy as sc
-import matplotlib.pyplot as plt
-import seaborn as sns
-from ..utility import (extract_gz_file, log_exp2cpm, cal_exp_by_gene_list)
-import anndata as an
-sc.settings.set_figure_params(dpi=200)
-sns.set()
-
-
-def check_by_stable_genes(sc_exp, stable_gene_list):
-    """
-    check single cell samples (each cell) by stable genes in bulk expression profiles
-    :param sc_exp: pandas.DataFrame
-        genes x cells of single cell, gene name as index of this df
-    :param stable_gene_list: pandas.DataFrame
-        gene with 95% confidence interval (95%_CI_left, 95%_CI_right)
-    :return: percentage of genes in CI, cells x stable genes,
-        -1: < 95%_CI_left,
-        0: [95%_CI_left, 95%_CI_right]
-        1: > 95%_CI_right
-    """
-    common_genes = [i for i in stable_gene_list.index if i in sc_exp.index]
-    sc_exp = sc_exp.loc[common_genes, :].T
-    stable_gene_list = stable_gene_list.loc[common_genes, :]
-    result = pd.DataFrame(index=sc_exp.index, columns=sc_exp.columns)
-    for sample in sc_exp.index:
-        current_exp = sc_exp.loc[sample, :]
-        for gene in current_exp.index:
-            if current_exp[gene] > stable_gene_list.loc[gene, '95%_CI_right']:
-                result.loc[sample, gene] = 1
-            elif current_exp[gene] < stable_gene_list.loc[gene, '95%_CI_left']:
-                result.loc[sample, gene] = -1
-            else:
-                result.loc[sample, gene] = 0
-    result['in_CI_%'] = np.sum(result == 0, axis=1) / len(common_genes)
-    result['<_CI_left_%'] = np.sum(result == -1, axis=1) / len(common_genes)
-    result['>_CI_right_%'] = np.sum(result == 1, axis=1) / len(common_genes)
-    return result
-
-
-def get_10x_mtx(file_dir, prefix=None, min_genes=200, min_cells=3, result_dir=None,
-                target_sum=1e4, log_base=None, max_n_genes_by_counts=2500, max_pct_counts_mt=5,
-                max_total_counts=None, filter_genes: bool = True, fig_prefix=None, dense_file=False):
-    """
-
-    :param file_dir: contains three files: barcodes.tsv  genes.tsv  matrix.mtx
-    :param prefix:
-    :param min_genes: min genes in each cell
-    :param min_cells: min cells for each gene expressed
-    :param target_sum: normalized total reads
-    :param log_base: logarithmize the data, usually is 2
-    :param max_n_genes_by_counts: filtering n_genes_by_counts
-    :param max_pct_counts_mt: filtering pct_counts_mt
-    :param max_total_counts: filtering total_counts
-    :param filter_genes: bool, if need to filter genes
-    :param fig_prefix:
-    :param result_dir:
-    :param dense_file: bool, if input data is stored in dense format
-    :return:
-    """
-    for _file in ['barcodes.tsv', 'genes.tsv', 'matrix.mtx']:
-        file_name = prefix + _file + '.gz'
-        # print(os.path.join(file_dir, file_name))
-        if os.path.exists(os.path.join(file_dir, file_name)):
-            # print('...')
-            extract_gz_file(file_dir=file_dir, file_name=file_name)
-    if dense_file:
-        adata = sc.read_csv(file_dir)  # file_dir is file path now
-    else:
-        adata = sc.read_10x_mtx(file_dir, prefix=prefix, var_names='gene_symbols')
-    adata = normalize_mtx(adata=adata, prefix=prefix, min_genes=min_genes, min_cells=min_cells,
-                          result_dir=result_dir, target_sum=target_sum, log_base=log_base,
-                          max_n_genes_by_counts=max_n_genes_by_counts, max_pct_counts_mt=max_pct_counts_mt,
-                          max_total_counts=max_total_counts, filter_genes=filter_genes, fig_prefix=fig_prefix)
-    return adata
-
-
-def normalize_mtx(adata, prefix=None, min_genes=200, min_cells=3, result_dir=None,
-                  target_sum=1e4, log_base=None, max_n_genes_by_counts=2500, max_pct_counts_mt=5,
-                  max_total_counts=None, filter_genes: bool = True, fig_prefix=None):
-    """
-
-    :param adata: an AnnData object which contains a single sample data (cells by genes)
-    :param prefix:
-    :param min_genes: min genes in each cell
-    :param min_cells: min cells for each gene expressed
-    :param target_sum: normalized total reads
-    :param log_base: logarithmize the data, usually is 2
-    :param max_n_genes_by_counts: filtering n_genes_by_counts
-    :param max_pct_counts_mt: filtering pct_counts_mt
-    :param max_total_counts: filtering total_counts
-    :param filter_genes: bool, if need to filter genes
-    :param fig_prefix:
-    :param result_dir:
-    :return: log2(CPM + 1) after filtering
-    """
-    adata.var_names_make_unique()
-    print('   The shape of adata before filtering is: {}'.format(adata.shape))
-    # filtering cells and genes
-    sc.pp.filter_cells(adata, min_genes=min_genes)
-    if filter_genes:
-        sc.pp.filter_genes(adata, min_cells=min_cells)
-    # QC
-    adata.var['mt'] = adata.var_names.str.startswith('MT-')  # annotate the group of mitochondrial genes as 'mt'
-    sc.pp.calculate_qc_metrics(adata, qc_vars=['mt'], percent_top=None, log1p=False, inplace=True)
-    if fig_prefix is not None:
-        prefix = fig_prefix
-    if result_dir is not None:
-        if not os.path.exists(result_dir):
-            os.makedirs(result_dir)
-        # plot QC metrics
-        plt.figure(figsize=(15, 3))
-        sc.settings.figdir = result_dir
-        sc.pl.violin(adata, ['n_genes_by_counts', 'total_counts', 'pct_counts_mt'],
-                     jitter=0.4, multi_panel=True, save=prefix + 'qc_metrics.png')
-
-        # plot total counts vs percentage of counts in mitochondrial genes
-        plt.figure(figsize=(8, 6))
-        sc.pl.scatter(adata, x='total_counts', y='pct_counts_mt', save=prefix + 'total_counts_vs_pct_counts_mt.png')
-
-        # plot total counts vs the number of genes expressed in the count matrix
-        plt.figure(figsize=(8, 6))
-        sc.pl.scatter(adata, x='total_counts', y='n_genes_by_counts',
-                      save=prefix + 'total_counts_vs_n_genes_by_counts.png')
-
-    # filtering cells
-    adata = adata[adata.obs.n_genes_by_counts <= max_n_genes_by_counts, :]
-    adata = adata[adata.obs.pct_counts_mt <= max_pct_counts_mt, :]
-    if max_total_counts is not None:
-        adata = adata[adata.obs.total_counts <= max_total_counts, :]
-    if target_sum is not None:
-        sc.pp.normalize_total(adata, target_sum=target_sum)
-    if log_base is not None and adata.shape[0] >= 1:
-        sc.pp.log1p(adata, base=log_base)
-        # sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
-        # print('   The number of highly variable genes: {}'.format(sum(adata.var['highly_variable'])))
-        # if result_dir is not None:
-        #     plt.figure(figsize=(10, 4))
-        #     sc.pl.highly_variable_genes(adata, save=prefix + 'highly_variable_genes.png')
-
-    print('   The shape of adata after filtering is: {}'.format(adata.shape))
-    return adata
-
-
-def get_sample_id(obs_df, n, cell_type, n_base, class_by='leiden', sep_by_patient=False):
-    """
-    select sample id by random sampling
-    :param obs_df: adata.obs in .h5ad file
-    :param n: the number of cells to be generated
-    :param cell_type: sampling only within this cell types (cell_type) or sub cell types (leiden)
-    :param n_base: the number of single cells to average
-    :param class_by: leiden or cell_type, the column name of cell type (or subtype) in .h5ad file
-    :param sep_by_patient: only sampling from one patient in original dataset if True
-    :return: a tuple of tuples  (('s1', 's2'), ('s3', 's5')), each tuple contains n_base ids for a single sample
-    """
-    if n_base == 0:
-        return tuple()
-    obs_df = obs_df.loc[obs_df[class_by] == cell_type, :].copy()
-    all_samples_id = obs_df.index.to_list()
-    groupby_patient_count = None
-    if sep_by_patient:
-        groupby_patient_count = obs_df.groupby(['sample_id']).count()
-        groupby_patient_count = groupby_patient_count.loc[groupby_patient_count['leiden'] > n_base + 10, :].copy()
-    selected_samples = {}
-    while len(selected_samples) < n:
-        _s = tuple()
-        if (groupby_patient_count is not None) and (groupby_patient_count.shape[0] > 1):
-            selected_patient_id = groupby_patient_count.sample(1).index.to_list()[0]
-            all_samples_id = obs_df.loc[obs_df['sample_id'] == selected_patient_id, :].index.to_list()
-        if len(all_samples_id) < n_base:
-            print(cell_type, len(all_samples_id), n_base)
-        _s = np.random.choice(all_samples_id, n_base, replace=False)
-        _s = tuple(sorted(_s))
-        if _s not in selected_samples:
-            selected_samples[_s] = 1
-    if n == 1:
-        return tuple(selected_samples.keys())[0]  # return a tuple  ('s1', 's2', ...)
-    return tuple(selected_samples.keys())  # return a tuple of tuples  (('s1', 's2'), ('s3', 's5'))
-
-
-# def generate_sc(adata, n, cell_type, n_base=3, log_base=2, group_by='leiden',
-#                 return_cell_id=False, filtering: bool = False, marker_genes=None,
-#                 cell_type_scope: list = None):
-#     """
-#     Generate single cell expression data by averaging `n_base` cells from a specific `cell_type`
-#
-#     :param adata: AnnData object which contains multiple merged single cell datasets, GEPs stored by log2(CPM + 1),
-#         CPM means counts per million, similar to TPM.
-#
-#     :param n: the number of cells to be generated
-#
-#     :param cell_type: sampling only within this cell types or sub cell types
-#
-#     :param n_base: the number of single cells to average
-#
-#     :param log_base: if None, don't do log transform
-#
-#     :param group_by: `leiden` (sub cell type) or `cell_type`, the column name of cell type in .h5ad file
-#
-#     :param return_cell_id: if return selected sample id directly without GEP
-#
-#     :param filtering: whether filter CD8 T and CD4 T based on the expression of corresponding marker genes
-#
-#     :param marker_genes: marker genes for each cell type, only for filtering
-#
-#     :param cell_type_scope: filter generated bulk cell expression profile only among these cell types
-#
-#     :return: a tuple of selected sample ids or an AnnData object with log2(CPM + 1) GEP
-#     """
-#     exp_threshold_low = 50
-#     exp_threshold_up = 100
-#     if marker_genes is None:
-#         marker_genes = default_core_marker_genes
-#     round_counter = 0
-#     # only keep current cell type
-#     adata = adata[adata.obs[group_by] == cell_type, :].copy()
-#     adata_df = pd.DataFrame(adata.X.A, index=adata.obs.index, columns=adata.var.index)
-#     adata_df = log_exp2cpm(adata_df)  # convert to CPM
-#     g_sample2exp = {}
-#     g_sample2id = {}
-#     while len(g_sample2exp) < n:
-#         # get sample_id for 100 samples each time
-#         _selected_samples = get_sample_id(obs_df=adata.obs, n=100, n_base=n_base,
-#                                           cell_type=cell_type, class_by=group_by)
-#         for i, _s in enumerate(_selected_samples):
-#             keep_this_exp = True
-#             unique_inx = i + round_counter * 100
-#             # expression profile of one generated single cell expression
-#             exp_sc = adata_df.loc[_s, :].mean(axis=0)
-#             # cell_type_abbr = ''
-#             if cell_type in subcell_type2abbr:
-#                 cell_type_abbr = subcell_type2abbr[cell_type]
-#             elif cell_type in cell_type2abbr:
-#                 cell_type_abbr = cell_type2abbr[cell_type]
-#             else:
-#                 raise KeyError('Unknown cell type')
-#             gen_id = 'gen_' + cell_type_abbr + '_' + str(unique_inx)
-#             if group_by == 'leiden':
-#                 par_ct_name = cell_type_mapping[cell_type]  # the name of parent cell type
-#             else:
-#                 par_ct_name = cell_type
-#             if filtering:
-#                 exp_sc_df = exp_sc.to_frame(name=gen_id).T
-#                 t_marker_mean_cpm = cal_exp_by_gene_list(exp_sc_df, gene_list=marker_genes['T Cells'], min_exp_value=1)
-#                 if par_ct_name not in ['CD4 T', 'CD8 T']:
-#                     if t_marker_mean_cpm >= exp_threshold_low:
-#                         keep_this_exp = False
-#                 else:
-#                     if t_marker_mean_cpm < exp_threshold_up:
-#                         keep_this_exp = False
-#                 if not keep_this_exp:
-#                     continue
-#
-#                 # filter by the expression value of marker genes
-#                 marker_mean = {}
-#                 if cell_type_scope is None:
-#                     cell_type_scope = list(cell_type2abbr.keys())
-#                 for _cell_type in cell_type_scope:
-#                     if _cell_type in marker_genes.keys():  # non-cancer cell
-#                         marker_mean[_cell_type] = cal_exp_by_gene_list(exp_sc_df, gene_list=marker_genes[_cell_type])
-#                         if _cell_type == par_ct_name:
-#                             # the mean expression of marker genes for current cell type should >= exp_threshold_up
-#                             if marker_mean[_cell_type] < exp_threshold_up:
-#                                 keep_this_exp = False
-#                         else:  # the mean expression of marker genes for other cell types should < exp_threshold_low
-#                             if marker_mean[_cell_type] >= exp_threshold_low:
-#                                 keep_this_exp = False
-#                         if not keep_this_exp:
-#                             break
-#
-#             if keep_this_exp:
-#                 g_sample2exp[gen_id] = exp_sc
-#                 g_sample2id[gen_id] = _s
-#         round_counter += 1
-#     # selected_samples = get_sample_id(obs_df=adata.obs, n=n, n_base=n_base, cell_type=cell_type, class_by=group_by)
-#     if return_cell_id:
-#         return tuple(list(g_sample2id.values())[:n])
-#
-#     generated_samples = pd.DataFrame.from_dict(g_sample2exp, orient='index', columns=adata_df.columns)
-#     if len(g_sample2exp) > n:
-#         generated_samples = generated_samples.iloc[range(n), :].copy()
-#     adata = an.AnnData(generated_samples)
-#     if adata.shape[0] > 1:
-#         adata.X = csr_matrix(adata.X)
-#     adata.obs['dataset_id'] = 'generated'
-#     adata.obs[group_by] = cell_type
-#     g_sample2id = {i: ','.join(j) for i, j in g_sample2id.items()}
-#     adata.obs['original_sample_ids'] = adata.obs.index.map(g_sample2id)
-#     if group_by == 'leiden':
-#         adata.obs['cell_type'] = cell_type_mapping.get(cell_type)
-#     sc.pp.log1p(adata, base=log_base)
-#     return adata
-
-
-def merge_adata(adata_list: list, keep_index=True):
-    """
-    merge a list of AnnData objects
-    :param adata_list:
-    :param keep_index:
-    :return:
-    """
-    # all_dataset_id = list(cell_type2dataset_n.keys())
-    merged = None
-    if keep_index:
-        index_unique = None
-    else:
-        index_unique = "-"
-    for i in range(len(adata_list)-1):
-        # print('>>> deale with {}'.format(all_dataset_id[i]))
-        next_dataset = adata_list[i+1]
-        if merged is None:
-            current_dataset = adata_list[i]
-            merged = current_dataset.concatenate(next_dataset, index_unique=index_unique)
-        else:
-            merged = merged.concatenate(next_dataset, index_unique=index_unique)
-    return merged
-
-
-# def generate_sc_dataset2(merged_ds, n_samples: int = 5000, cell_types: list = None,
-#                          result_file_path=None, group_by='leiden', n_base=3, filtering: bool = False,
-#                          cd4_high_in_cd8: str = None):
-#     """
-#     Simple version of `generate_sc_dataset`,
-#     generate single cell dataset by averaging the GEP of `n_base` (3 or 5) cells
-#     from the same cell type (or sub cell type, leiden) from merged scRNA-seq dataset
-#
-#     :param merged_ds: all or parts of file 6_dataset_merged_after_batch_correction_filtered.h5ad
-#
-#     :param n_samples: number of samples for each cell type (or sub cell type)
-#
-#     :param cell_types:
-#
-#     :param result_file_path:
-#
-#     :param group_by: group by `cell_type` or `leiden` (sub cell type) when generating single cell dataset
-#
-#     :param n_base: the number of single cells to average
-#
-#     :param filtering: whether filter CD8 T and CD4 T based on the expression of corresponding marker genes
-#
-#     :param cd4_high_in_cd8: how to deal with the CD8 T cells that CD4 markers are highly expressed
-#         (remove, CD4, CD8)
-#
-#     :return: a file of an AnnData object with log2(CPM + 1) GEP
-#     """
-#     if not os.path.exists(result_file_path):
-#         cell_type2sc = {}
-#         cells_cd4_high_in_cd8 = merged_ds.obs.loc[(merged_ds.obs['cell_type'] == 'CD8 T') &
-#                                                   (merged_ds.obs['m_cd4/m_cd8 group'] == 'middle'), :].index.to_list()
-#         if cd4_high_in_cd8 == 'remove':
-#             merged_ds = merged_ds[~merged_ds.obs.index.isin(cells_cd4_high_in_cd8), :].copy()
-#             print('   The CD8 T cells with highly expressed CD4 T markers will be removed...')
-#         elif cd4_high_in_cd8 == 'CD4':
-#             merged_ds.obs['leiden'].cat.add_categories(['CD4-high (1)', 'CD4-high (2)'], inplace=True)
-#             merged_ds.obs.loc[merged_ds.obs.index.isin(cells_cd4_high_in_cd8), 'leiden'] = \
-#                 merged_ds.obs.loc[merged_ds.obs.index.isin(cells_cd4_high_in_cd8),
-#                                   'leiden'].replace({'CD8 T (1)': 'CD4-high (1)', 'CD8 T (2)': 'CD4-high (2)'})
-#             merged_ds.obs.loc[merged_ds.obs.index.isin(cells_cd4_high_in_cd8), ['cell_type']] = \
-#                 merged_ds.obs.loc[merged_ds.obs.index.isin(cells_cd4_high_in_cd8), 'cell_type'].replace('CD8 T', 'CD4 T')
-#         print(merged_ds)
-#         print(merged_ds.obs.loc[:, 'leiden'].value_counts())
-#         # print(merged_ds.obs.loc[merged_ds.obs['cell_type'] == 'CD4 T', 'leiden'].value_counts())
-#         for ct in cell_types:
-#             print('   >>> deal with cell type {}'.format(ct))
-#             if group_by == 'leiden':
-#                 sub_cell_types = sorted(list(merged_ds.obs.loc[merged_ds.obs['cell_type'] == ct, 'leiden'].unique()))
-#                 # print(sub_cell_types)
-#                 for sct in sub_cell_types:
-#                     print('       deal with sub cell type {}'.format(sct))
-#                     current_adata = merged_ds[merged_ds.obs['leiden'] == sct, :].copy()
-#                     generated = generate_sc(current_adata, n=n_samples, cell_type=sct, group_by=group_by,
-#                                             n_base=n_base, filtering=filtering, cell_type_scope=cell_types)
-#                     cell_type2sc[sct] = generated
-#             elif group_by == 'cell_type':
-#                 current_adata = merged_ds[merged_ds.obs['cell_type'] == ct, :].copy()
-#                 generated = generate_sc(current_adata, n=n_samples, cell_type=ct, group_by=group_by,
-#                                         n_base=n_base, filtering=filtering, cell_type_scope=cell_types)
-#                 cell_type2sc[ct] = generated
-#             else:
-#                 raise ValueError('Unrecognized parameter group_by {}, group_by should be "leiden" for sub cell type '
-#                                  'or "cell_type" for cell type'.format(group_by))
-#         all_adata = list(cell_type2sc.values())
-#         all_generated_data = merge_adata(all_adata)
-#         print(all_generated_data.obs['cell_type'].value_counts())
-#
-#         # clustering
-#         print('   >>> clustering generated single cell dataset...')
-#         if 'leiden' in all_generated_data.obs.columns:
-#             all_generated_data.obs['sub_cell_type'] = all_generated_data.obs['leiden'].copy()
-#         # sc_file_dir = os.path.dirname(sc_file_path)
-#         sc.tl.pca(all_generated_data, svd_solver='arpack', n_comps=100, use_highly_variable=False, zero_center=False)
-#         # sc.pl.pca_variance_ratio(sc_dataset, n_pcs=30)
-#         sc.pp.neighbors(all_generated_data, n_neighbors=10, n_pcs=40)
-#         sc.tl.umap(all_generated_data)
-#         sc.tl.leiden(all_generated_data)
-#         all_generated_data.write(result_file_path)
-#     else:
-#         print(f'   Previous result has existed: {result_file_path}')
-
-
-def filter_cells_by_marker_gene(single_cell_dataset, cell_types: list = None, cell_type2markers: dict = None,
-                                exp_range: tuple = (50, 320), dataset_id: str = '', groupby: str = 'leiden',
-                                max_exp: float = 0.0):
-    """
-
-    :param single_cell_dataset:
-    :param cell_types:
-    :param cell_type2markers:
-    :param exp_range: (low_exp_threshold, middle_exp_threshold)
-    :param dataset_id:
-    :param groupby: index of groupby
-    :param max_exp: max expression to plot
-    :return:
-    """
-    cd4_cd8_ratio = 10
-    assert type(single_cell_dataset) == an.AnnData
-    all_removed_cells = []
-    dataset2filter_info = pd.DataFrame(columns=['n_before_filtering', 'n_after_filtering', 'hit_cell_type'],
-                                       index=list(single_cell_dataset.obs['leiden'].unique()))
-    dataset2filter_info.index.name = 'leiden'
-    cell_type_exp_value_collector_total = []
-    for gi, group in single_cell_dataset.obs.groupby([groupby]):
-        print(gi, group.shape)
-        # cell_type2exp_value_collector_current_gi = []
-        current_part_data = single_cell_dataset[single_cell_dataset.obs.index.isin(group.index), :].copy()
-        gene_exp = pd.DataFrame(current_part_data.X.A, columns=current_part_data.var.index,
-                                index=current_part_data.obs.index)
-        gene_exp = log_exp2cpm(gene_exp)  # convert the expression values from log2(CPM + 1) to CPM
-
-        cell_type_marker_exp = pd.DataFrame(index=gene_exp.index, columns=cell_types)  # sample by cell_type
-        cell_type_quantile = pd.DataFrame(index=['q_10', 'q_25', 'q_50', 'q_75', 'q_90', 'q_95'],
-                                          columns=cell_types)
-
-        # cell_type2exp_flatten = {}
-
-        for k, _cell_type in enumerate(cell_types):
-            if _cell_type in cell_type2markers.keys():
-                current_marker_gene = cell_type2markers[_cell_type]
-                # cell_type2marker_exp[_cell_type] = gene_exp.loc[:, current_marker_gene].copy()  # a dataFrame
-                method = 'mean'
-                if _cell_type in ['B Cells', 'CD4 T']:
-                    method = 'max'
-                cell_type_marker_exp[_cell_type] = \
-                    cal_exp_by_gene_list(gene_exp, gene_list=current_marker_gene, method=method, min_exp_value=1)
-                _values = cell_type_marker_exp[_cell_type].values
-                cell_type_quantile[_cell_type] = [np.quantile(_values, 0.1),
-                                                  np.quantile(_values, 0.25),
-                                                  np.quantile(_values, 0.50),
-                                                  np.quantile(_values, 0.75),
-                                                  np.quantile(_values, 0.90),
-                                                  np.quantile(_values, 0.95)]
-        if max_exp > 0:
-            cell_type_marker_exp[cell_type_marker_exp > max_exp] = max_exp
-        cell_type_marker_exp['m_max_cd4/mean_cd8'] = cell_type_marker_exp['CD4 T'] / cell_type_marker_exp['CD8 T']
-        # ct2e_gi['m_max_cd4/mean_cd8'] = ct2e_gi['m_max_CD4 T'] / ct2e_gi['m_mean_CD8 T']
-        cell_type_marker_exp['m_cd4/m_cd8 group'] = 'middle'
-        cell_type_marker_exp.loc[cell_type_marker_exp['m_max_cd4/mean_cd8'] > cd4_cd8_ratio,
-                                 'm_cd4/m_cd8 group'] = 'high'
-        cell_type_marker_exp.loc[cell_type_marker_exp['m_max_cd4/mean_cd8'] < (1 / cd4_cd8_ratio),
-                                 'm_cd4/m_cd8 group'] = 'low'
-        cell_type_exp_value_collector_total.append(cell_type_marker_exp.copy())
-
-        n_cells = gene_exp.shape[0]
-        t_cell_marker = 'low'
-        removed_cells = {}
-        hit_cell_type = None
-        dataset2filter_info.loc[gi, 'n_before_filtering'] = n_cells
-        for k, _cell_type in enumerate(cell_types):
-            if _cell_type in cell_type2markers.keys():
-                q50_current_cell_type = cell_type_quantile.loc['q_50', _cell_type]
-                # q90_current_cell_type = cell_type_quantile.loc['q_90', _cell_type]
-                if q50_current_cell_type < exp_range[1]:  # Q50 in low or middle expression range
-                    # 50% cells are expressed low as current cell type
-                    if _cell_type not in ['CD4 T', 'CD8 T']:
-                        # don't check CD4 T since the markers of CD4 may express in other cell types
-                        removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type=_cell_type,
-                                                             cell_type_marker_exp=cell_type_marker_exp,
-                                                             filter_upper=exp_range[1])
-                    elif _cell_type == 'CD8 T':
-                        if t_cell_marker != 'high':
-                            # only filter CD8 T when t_cell_marker is not high
-                            removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type=_cell_type,
-                                                                 cell_type_marker_exp=cell_type_marker_exp,
-                                                                 filter_upper=exp_range[1])
-                        else:  # t_cell_marker == 'high'
-                            if (q50_current_cell_type >= exp_range[0]) and (q50_current_cell_type < exp_range[1]):
-                                # Q50 quantile in middle expression range
-                                # Treat this cell type as CD8 T (may be CD8 Tex)
-                                # filtering by CD4 T / CD8 T
-                                _result = filter_cd4_cd8(removed_cells=removed_cells, cell_type=_cell_type,
-                                                         cell_type_marker_exp=cell_type_marker_exp,
-                                                         cell_type_quantile=cell_type_quantile,
-                                                         exp_range=exp_range)
-                                removed_cells = update_removed_cells(removed_cells=_result['removed_cells'],
-                                                                     cell_type=_cell_type,
-                                                                     cell_type_marker_exp=cell_type_marker_exp,
-                                                                     filter_lower=_result['filter_lower'],
-                                                                     filter_upper=_result['filter_upper'])
-                                hit_cell_type = 'CD8 T'
-                                break
-
-                else:  # the marker genes of current cell type are highly expressed (Q50 in high expression range)
-                    if _cell_type == 'T Cells':
-                        t_cell_marker = 'high'
-
-                    if (n_cells - len(removed_cells)) >= 3000:  # remove 35% since too many cells in this cluster
-                        filter_lower = cell_type_quantile.loc['q_25', _cell_type]
-                        filter_upper = cell_type_quantile.loc['q_90', _cell_type]
-                    else:  # remove 15% since a few cells
-                        filter_lower = cell_type_quantile.loc['q_10', _cell_type]
-                        filter_upper = cell_type_quantile.loc['q_95', _cell_type]
-
-                    if t_cell_marker != 'high':  # filtering by quantile, t_cell_marker is low or middle
-                        if _cell_type not in ['CD4 T', 'NK']:
-                            removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type=_cell_type,
-                                                                 cell_type_marker_exp=cell_type_marker_exp,
-                                                                 filter_lower=filter_lower, filter_upper=filter_upper)
-                        elif _cell_type == 'NK':  # don't check CD4 T when t_cell_marker is low or middle
-                            # filtering by CD4 T / CD8 T
-                            _result = filter_cd4_cd8(removed_cells=removed_cells, cell_type=_cell_type,
-                                                     cell_type_marker_exp=cell_type_marker_exp,
-                                                     cell_type_quantile=cell_type_quantile,
-                                                     exp_range=exp_range)
-                            removed_cells = update_removed_cells(removed_cells=_result['removed_cells'],
-                                                                 cell_type=_cell_type,
-                                                                 cell_type_marker_exp=cell_type_marker_exp,
-                                                                 filter_lower=_result['filter_lower'],
-                                                                 filter_upper=_result['filter_upper'])
-                        else:  # don't check CD4 T when t_cell_marker is low or middle
-                            continue
-
-                    else:  # t_cell_marker is high
-                        _result = None
-                        if _cell_type == 'T Cells':
-                            pass
-                        elif _cell_type in ['CD8 T', 'CD4 T', 'NK']:
-                            # filtering by CD4 T / CD8 T
-                            _result = filter_cd4_cd8(removed_cells=removed_cells, cell_type=_cell_type,
-                                                     cell_type_marker_exp=cell_type_marker_exp,
-                                                     cell_type_quantile=cell_type_quantile, exp_range=exp_range)
-                            removed_cells = update_removed_cells(removed_cells=_result['removed_cells'],
-                                                                 cell_type=_cell_type,
-                                                                 cell_type_marker_exp=cell_type_marker_exp,
-                                                                 filter_lower=_result['filter_lower'],
-                                                                 filter_upper=_result['filter_upper'])
-
-                    if _cell_type != 'T Cells':
-                        hit_cell_type = _cell_type
-                        break  # first hit except "T Cells", filtering by this cell type and stopped
-        dataset2filter_info.loc[gi, 'n_after_filtering'] = n_cells - len(removed_cells)
-        dataset2filter_info.loc[gi, 'hit_cell_type'] = hit_cell_type
-        if len(removed_cells) > 0:
-            _cell_ids = list(removed_cells.keys())
-            all_removed_cells += _cell_ids
-    cell_type_exp_value_collector_total_df = pd.concat(cell_type_exp_value_collector_total)
-    cell_type_exp_value_collector_total_df = cell_type_exp_value_collector_total_df.loc[single_cell_dataset.obs.index, :]
-    assert np.all(single_cell_dataset.obs.index == cell_type_exp_value_collector_total_df.index)
-    single_cell_dataset.obs['m_max_cd4/mean_cd8'] = cell_type_exp_value_collector_total_df['m_max_cd4/mean_cd8']
-    single_cell_dataset.obs['m_cd4/m_cd8 group'] = cell_type_exp_value_collector_total_df['m_cd4/m_cd8 group']
-    filtered_dataset = single_cell_dataset[~single_cell_dataset.obs.index.isin(all_removed_cells), :].copy()
-    dataset2filter_info['dataset_id'] = dataset_id
-    return filtered_dataset, dataset2filter_info
-
-
-def update_removed_cells(removed_cells: dict = None, cell_type_marker_exp: pd.DataFrame = None,
-                         filter_upper: float = None, filter_lower: float = None, cell_type: str = '') -> dict:
-    """
-
-    :param removed_cells:
-    :param cell_type_marker_exp:
-    :param filter_upper: filter_upper > filter_lower
-    :param filter_lower:
-    :param cell_type
-    :return:
-    """
-    if (filter_lower is not None) and (filter_upper is not None):
-        _removed = cell_type_marker_exp.loc[(cell_type_marker_exp[cell_type] > filter_upper) |
-                                            (cell_type_marker_exp[cell_type] <= filter_lower), :].index.to_list()
-    elif filter_lower is None:
-        _removed = cell_type_marker_exp.loc[(cell_type_marker_exp[cell_type] > filter_upper), :].index.to_list()
-    elif filter_upper is None:
-        _removed = cell_type_marker_exp.loc[(cell_type_marker_exp[cell_type] <= filter_lower), :].index.to_list()
-    else:
-        raise KeyError('Both filter_lower and filter_upper are None')
-    if len(_removed) > 0:
-        for _ in _removed:
-            removed_cells[_] = 1
-
-    return removed_cells
-
-
-def filter_by_cd8_marker(removed_cells: dict = None, cell_type_marker_exp: pd.DataFrame = None,
-                         cell_type_quantile: pd.DataFrame = None, cell_type: str = '',
-                         exp_range: tuple = None):
-    removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type='CD8 T',
-                                         cell_type_marker_exp=cell_type_marker_exp,
-                                         filter_upper=exp_range[0])
-    n_cells = cell_type_marker_exp.shape[0]
-    # check n_cells - len(removed_cells) again
-    if (n_cells - len(removed_cells)) >= 3000:  # remove 35% since too many cells
-        filter_lower = cell_type_quantile.loc['q_25', cell_type]
-        filter_upper = cell_type_quantile.loc['q_90', cell_type]
-    else:  # remove 15% since a few cells
-        filter_lower = cell_type_quantile.loc['q_10', cell_type]
-        filter_upper = cell_type_quantile.loc['q_95', cell_type]
-    return {'removed_cells': removed_cells, 'filter_lower': filter_lower, 'filter_upper': filter_upper}
-
-
-def filter_by_cd4_marker(removed_cells: dict = None, cell_type_marker_exp: pd.DataFrame = None,
-                         cell_type_quantile: pd.DataFrame = None, cell_type: str = '', exp_range: tuple = None):
-    q50 = cell_type_quantile.loc['q_50', 'CD4 T']
-    filter_upper = min(q50, exp_range[1])
-    removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type='CD4 T',
-                                         cell_type_marker_exp=cell_type_marker_exp,
-                                         filter_upper=filter_upper)
-    n_cells = cell_type_marker_exp.shape[0]
-    # check n_cells - len(removed_cells) again
-    if (n_cells - len(removed_cells)) >= 3000:  # remove 35% since too many cells
-        filter_lower = cell_type_quantile.loc['q_25', cell_type]
-        filter_upper = cell_type_quantile.loc['q_90', cell_type]
-    else:  # remove 15% since a few cells
-        filter_lower = cell_type_quantile.loc['q_10', cell_type]
-        filter_upper = cell_type_quantile.loc['q_95', cell_type]
-    return {'removed_cells': removed_cells, 'filter_lower': filter_lower, 'filter_upper': filter_upper}
-
-
-def filter_cd4_cd8(removed_cells: dict = None, cell_type: str = '', exp_range: tuple = (),
-                   cell_type_marker_exp: pd.DataFrame = None, cell_type_quantile: pd.DataFrame = None):
-    """
-    filter cells by the ratio of marker genes expression between CD4 T and CD8 T (max CD4 T / mean CD8 T) or
-    the expression value
-    :param removed_cells:
-    :param cell_type: current cell type with high expression of it's marker genes
-    :param exp_range:
-    :param cell_type_marker_exp:
-    :param cell_type_quantile:
-    :return:
-    """
-    # q50 = cell_type_quantile.loc['q_50', 'CD4 T']
-    # filter_upper = min(q50, exp_range[1])
-    # removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type='CD4 T',
-    #                                      cell_type_marker_exp=cell_type_marker_exp,
-    #                                      filter_upper=filter_upper)
-    _removed = []
-    if cell_type == 'CD4 T':
-        _removed = cell_type_marker_exp.loc[cell_type_marker_exp['m_cd4/m_cd8 group'] != 'high', :].index.to_list()
-    elif cell_type == 'CD8 T':
-        _removed = cell_type_marker_exp.loc[cell_type_marker_exp['m_cd4/m_cd8 group'] == 'high', :].index.to_list()
-        # _removed = cell_type_marker_exp.loc[cell_type_marker_exp['m_cd4/m_cd8 group'] != 'low', :].index.to_list()
-    elif cell_type == 'NK':  # both CD4 T marker and CD8 T marker should be low
-        _removed = cell_type_marker_exp.loc[(cell_type_marker_exp['CD8 T'] > exp_range[1]) |
-                                            (cell_type_marker_exp['CD4 T'] > exp_range[1]), :].index.to_list()
-
-    if len(_removed) > 0:
-        for _ in _removed:
-            removed_cells[_] = 1
-
-    n_cells = cell_type_marker_exp.shape[0]
-    # check n_cells - len(removed_cells) again
-    if (n_cells - len(removed_cells)) >= 3000:  # remove 35% since too many cells
-        filter_lower = cell_type_quantile.loc['q_25', cell_type]
-        filter_upper = cell_type_quantile.loc['q_90', cell_type]
-    else:  # remove 15% since a few cells
-        filter_lower = cell_type_quantile.loc['q_10', cell_type]
-        filter_upper = cell_type_quantile.loc['q_95', cell_type]
-    return {'removed_cells': removed_cells, 'filter_lower': filter_lower, 'filter_upper': filter_upper}
-
-
-if __name__ == '__main__':
-    pass
+import os
+import numpy as np
+import pandas as pd
+import scanpy as sc
+import matplotlib.pyplot as plt
+import seaborn as sns
+from ..utility import (extract_gz_file, log_exp2cpm, cal_exp_by_gene_list)
+import anndata as an
+sc.settings.set_figure_params(dpi=200)
+sns.set()
+
+
+def check_by_stable_genes(sc_exp, stable_gene_list):
+    """
+    check single cell samples (each cell) by stable genes in bulk expression profiles
+    :param sc_exp: pandas.DataFrame
+        genes x cells of single cell, gene name as index of this df
+    :param stable_gene_list: pandas.DataFrame
+        gene with 95% confidence interval (95%_CI_left, 95%_CI_right)
+    :return: percentage of genes in CI, cells x stable genes,
+        -1: < 95%_CI_left,
+        0: [95%_CI_left, 95%_CI_right]
+        1: > 95%_CI_right
+    """
+    common_genes = [i for i in stable_gene_list.index if i in sc_exp.index]
+    sc_exp = sc_exp.loc[common_genes, :].T
+    stable_gene_list = stable_gene_list.loc[common_genes, :]
+    result = pd.DataFrame(index=sc_exp.index, columns=sc_exp.columns)
+    for sample in sc_exp.index:
+        current_exp = sc_exp.loc[sample, :]
+        for gene in current_exp.index:
+            if current_exp[gene] > stable_gene_list.loc[gene, '95%_CI_right']:
+                result.loc[sample, gene] = 1
+            elif current_exp[gene] < stable_gene_list.loc[gene, '95%_CI_left']:
+                result.loc[sample, gene] = -1
+            else:
+                result.loc[sample, gene] = 0
+    result['in_CI_%'] = np.sum(result == 0, axis=1) / len(common_genes)
+    result['<_CI_left_%'] = np.sum(result == -1, axis=1) / len(common_genes)
+    result['>_CI_right_%'] = np.sum(result == 1, axis=1) / len(common_genes)
+    return result
+
+
+def get_10x_mtx(file_dir, prefix=None, min_genes=200, min_cells=3, result_dir=None,
+                target_sum=1e4, log_base=None, max_n_genes_by_counts=2500, max_pct_counts_mt=5,
+                max_total_counts=None, filter_genes: bool = True, fig_prefix=None, dense_file=False):
+    """
+
+    :param file_dir: contains three files: barcodes.tsv  genes.tsv  matrix.mtx
+    :param prefix:
+    :param min_genes: min genes in each cell
+    :param min_cells: min cells for each gene expressed
+    :param target_sum: normalized total reads
+    :param log_base: logarithmize the data, usually is 2
+    :param max_n_genes_by_counts: filtering n_genes_by_counts
+    :param max_pct_counts_mt: filtering pct_counts_mt
+    :param max_total_counts: filtering total_counts
+    :param filter_genes: bool, if need to filter genes
+    :param fig_prefix:
+    :param result_dir:
+    :param dense_file: bool, if input data is stored in dense format
+    :return:
+    """
+    for _file in ['barcodes.tsv', 'genes.tsv', 'matrix.mtx']:
+        file_name = prefix + _file + '.gz'
+        # print(os.path.join(file_dir, file_name))
+        if os.path.exists(os.path.join(file_dir, file_name)):
+            # print('...')
+            extract_gz_file(file_dir=file_dir, file_name=file_name)
+    if dense_file:
+        adata = sc.read_csv(file_dir)  # file_dir is file path now
+    else:
+        adata = sc.read_10x_mtx(file_dir, prefix=prefix, var_names='gene_symbols')
+    adata = normalize_mtx(adata=adata, prefix=prefix, min_genes=min_genes, min_cells=min_cells,
+                          result_dir=result_dir, target_sum=target_sum, log_base=log_base,
+                          max_n_genes_by_counts=max_n_genes_by_counts, max_pct_counts_mt=max_pct_counts_mt,
+                          max_total_counts=max_total_counts, filter_genes=filter_genes, fig_prefix=fig_prefix)
+    return adata
+
+
+def normalize_mtx(adata, prefix=None, min_genes=200, min_cells=3, result_dir=None,
+                  target_sum=1e4, log_base=None, max_n_genes_by_counts=2500, max_pct_counts_mt=5,
+                  max_total_counts=None, filter_genes: bool = True, fig_prefix=None):
+    """
+
+    :param adata: an AnnData object which contains a single sample data (cells by genes)
+    :param prefix:
+    :param min_genes: min genes in each cell
+    :param min_cells: min cells for each gene expressed
+    :param target_sum: normalized total reads
+    :param log_base: logarithmize the data, usually is 2
+    :param max_n_genes_by_counts: filtering n_genes_by_counts
+    :param max_pct_counts_mt: filtering pct_counts_mt
+    :param max_total_counts: filtering total_counts
+    :param filter_genes: bool, if need to filter genes
+    :param fig_prefix:
+    :param result_dir:
+    :return: log2(CPM + 1) after filtering
+    """
+    adata.var_names_make_unique()
+    print('   The shape of adata before filtering is: {}'.format(adata.shape))
+    # filtering cells and genes
+    sc.pp.filter_cells(adata, min_genes=min_genes)
+    if filter_genes:
+        sc.pp.filter_genes(adata, min_cells=min_cells)
+    # QC
+    adata.var['mt'] = adata.var_names.str.startswith('MT-')  # annotate the group of mitochondrial genes as 'mt'
+    sc.pp.calculate_qc_metrics(adata, qc_vars=['mt'], percent_top=None, log1p=False, inplace=True)
+    if fig_prefix is not None:
+        prefix = fig_prefix
+    if result_dir is not None:
+        if not os.path.exists(result_dir):
+            os.makedirs(result_dir)
+        # plot QC metrics
+        plt.figure(figsize=(15, 3))
+        sc.settings.figdir = result_dir
+        sc.pl.violin(adata, ['n_genes_by_counts', 'total_counts', 'pct_counts_mt'],
+                     jitter=0.4, multi_panel=True, save=prefix + 'qc_metrics.png')
+
+        # plot total counts vs percentage of counts in mitochondrial genes
+        plt.figure(figsize=(8, 6))
+        sc.pl.scatter(adata, x='total_counts', y='pct_counts_mt', save=prefix + 'total_counts_vs_pct_counts_mt.png')
+
+        # plot total counts vs the number of genes expressed in the count matrix
+        plt.figure(figsize=(8, 6))
+        sc.pl.scatter(adata, x='total_counts', y='n_genes_by_counts',
+                      save=prefix + 'total_counts_vs_n_genes_by_counts.png')
+
+    # filtering cells
+    adata = adata[adata.obs.n_genes_by_counts <= max_n_genes_by_counts, :]
+    adata = adata[adata.obs.pct_counts_mt <= max_pct_counts_mt, :]
+    if max_total_counts is not None:
+        adata = adata[adata.obs.total_counts <= max_total_counts, :]
+    if target_sum is not None:
+        sc.pp.normalize_total(adata, target_sum=target_sum)
+    if log_base is not None and adata.shape[0] >= 1:
+        sc.pp.log1p(adata, base=log_base)
+        # sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
+        # print('   The number of highly variable genes: {}'.format(sum(adata.var['highly_variable'])))
+        # if result_dir is not None:
+        #     plt.figure(figsize=(10, 4))
+        #     sc.pl.highly_variable_genes(adata, save=prefix + 'highly_variable_genes.png')
+
+    print('   The shape of adata after filtering is: {}'.format(adata.shape))
+    return adata
+
+
+def get_sample_id(obs_df, n, cell_type, n_base, class_by='leiden', sep_by_patient=False):
+    """
+    select sample id by random sampling
+    :param obs_df: adata.obs in .h5ad file
+    :param n: the number of cells to be generated
+    :param cell_type: sampling only within this cell types (cell_type) or sub cell types (leiden)
+    :param n_base: the number of single cells to average
+    :param class_by: leiden or cell_type, the column name of cell type (or subtype) in .h5ad file
+    :param sep_by_patient: only sampling from one patient in original dataset if True
+    :return: a tuple of tuples  (('s1', 's2'), ('s3', 's5')), each tuple contains n_base ids for a single sample
+    """
+    if n_base == 0:
+        return tuple()
+    obs_df = obs_df.loc[obs_df[class_by] == cell_type, :].copy()
+    all_samples_id = obs_df.index.to_list()
+    groupby_patient_count = None
+    if sep_by_patient:
+        groupby_patient_count = obs_df.groupby(['sample_id']).count()
+        groupby_patient_count = groupby_patient_count.loc[groupby_patient_count['leiden'] > n_base + 10, :].copy()
+    selected_samples = {}
+    while len(selected_samples) < n:
+        _s = tuple()
+        if (groupby_patient_count is not None) and (groupby_patient_count.shape[0] > 1):
+            selected_patient_id = groupby_patient_count.sample(1).index.to_list()[0]
+            all_samples_id = obs_df.loc[obs_df['sample_id'] == selected_patient_id, :].index.to_list()
+        if len(all_samples_id) < n_base:
+            print(cell_type, len(all_samples_id), n_base)
+        _s = np.random.choice(all_samples_id, n_base, replace=False)
+        _s = tuple(sorted(_s))
+        if _s not in selected_samples:
+            selected_samples[_s] = 1
+    if n == 1:
+        return tuple(selected_samples.keys())[0]  # return a tuple  ('s1', 's2', ...)
+    return tuple(selected_samples.keys())  # return a tuple of tuples  (('s1', 's2'), ('s3', 's5'))
+
+
+# def generate_sc(adata, n, cell_type, n_base=3, log_base=2, group_by='leiden',
+#                 return_cell_id=False, filtering: bool = False, marker_genes=None,
+#                 cell_type_scope: list = None):
+#     """
+#     Generate single cell expression data by averaging `n_base` cells from a specific `cell_type`
+#
+#     :param adata: AnnData object which contains multiple merged single cell datasets, GEPs stored by log2(CPM + 1),
+#         CPM means counts per million, similar to TPM.
+#
+#     :param n: the number of cells to be generated
+#
+#     :param cell_type: sampling only within this cell types or sub cell types
+#
+#     :param n_base: the number of single cells to average
+#
+#     :param log_base: if None, don't do log transform
+#
+#     :param group_by: `leiden` (sub cell type) or `cell_type`, the column name of cell type in .h5ad file
+#
+#     :param return_cell_id: if return selected sample id directly without GEP
+#
+#     :param filtering: whether filter CD8 T and CD4 T based on the expression of corresponding marker genes
+#
+#     :param marker_genes: marker genes for each cell type, only for filtering
+#
+#     :param cell_type_scope: filter generated bulk cell expression profile only among these cell types
+#
+#     :return: a tuple of selected sample ids or an AnnData object with log2(CPM + 1) GEP
+#     """
+#     exp_threshold_low = 50
+#     exp_threshold_up = 100
+#     if marker_genes is None:
+#         marker_genes = default_core_marker_genes
+#     round_counter = 0
+#     # only keep current cell type
+#     adata = adata[adata.obs[group_by] == cell_type, :].copy()
+#     adata_df = pd.DataFrame(adata.X.A, index=adata.obs.index, columns=adata.var.index)
+#     adata_df = log_exp2cpm(adata_df)  # convert to CPM
+#     g_sample2exp = {}
+#     g_sample2id = {}
+#     while len(g_sample2exp) < n:
+#         # get sample_id for 100 samples each time
+#         _selected_samples = get_sample_id(obs_df=adata.obs, n=100, n_base=n_base,
+#                                           cell_type=cell_type, class_by=group_by)
+#         for i, _s in enumerate(_selected_samples):
+#             keep_this_exp = True
+#             unique_inx = i + round_counter * 100
+#             # expression profile of one generated single cell expression
+#             exp_sc = adata_df.loc[_s, :].mean(axis=0)
+#             # cell_type_abbr = ''
+#             if cell_type in subcell_type2abbr:
+#                 cell_type_abbr = subcell_type2abbr[cell_type]
+#             elif cell_type in cell_type2abbr:
+#                 cell_type_abbr = cell_type2abbr[cell_type]
+#             else:
+#                 raise KeyError('Unknown cell type')
+#             gen_id = 'gen_' + cell_type_abbr + '_' + str(unique_inx)
+#             if group_by == 'leiden':
+#                 par_ct_name = cell_type_mapping[cell_type]  # the name of parent cell type
+#             else:
+#                 par_ct_name = cell_type
+#             if filtering:
+#                 exp_sc_df = exp_sc.to_frame(name=gen_id).T
+#                 t_marker_mean_cpm = cal_exp_by_gene_list(exp_sc_df, gene_list=marker_genes['T Cells'], min_exp_value=1)
+#                 if par_ct_name not in ['CD4 T', 'CD8 T']:
+#                     if t_marker_mean_cpm >= exp_threshold_low:
+#                         keep_this_exp = False
+#                 else:
+#                     if t_marker_mean_cpm < exp_threshold_up:
+#                         keep_this_exp = False
+#                 if not keep_this_exp:
+#                     continue
+#
+#                 # filter by the expression value of marker genes
+#                 marker_mean = {}
+#                 if cell_type_scope is None:
+#                     cell_type_scope = list(cell_type2abbr.keys())
+#                 for _cell_type in cell_type_scope:
+#                     if _cell_type in marker_genes.keys():  # non-cancer cell
+#                         marker_mean[_cell_type] = cal_exp_by_gene_list(exp_sc_df, gene_list=marker_genes[_cell_type])
+#                         if _cell_type == par_ct_name:
+#                             # the mean expression of marker genes for current cell type should >= exp_threshold_up
+#                             if marker_mean[_cell_type] < exp_threshold_up:
+#                                 keep_this_exp = False
+#                         else:  # the mean expression of marker genes for other cell types should < exp_threshold_low
+#                             if marker_mean[_cell_type] >= exp_threshold_low:
+#                                 keep_this_exp = False
+#                         if not keep_this_exp:
+#                             break
+#
+#             if keep_this_exp:
+#                 g_sample2exp[gen_id] = exp_sc
+#                 g_sample2id[gen_id] = _s
+#         round_counter += 1
+#     # selected_samples = get_sample_id(obs_df=adata.obs, n=n, n_base=n_base, cell_type=cell_type, class_by=group_by)
+#     if return_cell_id:
+#         return tuple(list(g_sample2id.values())[:n])
+#
+#     generated_samples = pd.DataFrame.from_dict(g_sample2exp, orient='index', columns=adata_df.columns)
+#     if len(g_sample2exp) > n:
+#         generated_samples = generated_samples.iloc[range(n), :].copy()
+#     adata = an.AnnData(generated_samples)
+#     if adata.shape[0] > 1:
+#         adata.X = csr_matrix(adata.X)
+#     adata.obs['dataset_id'] = 'generated'
+#     adata.obs[group_by] = cell_type
+#     g_sample2id = {i: ','.join(j) for i, j in g_sample2id.items()}
+#     adata.obs['original_sample_ids'] = adata.obs.index.map(g_sample2id)
+#     if group_by == 'leiden':
+#         adata.obs['cell_type'] = cell_type_mapping.get(cell_type)
+#     sc.pp.log1p(adata, base=log_base)
+#     return adata
+
+
+def merge_adata(adata_list: list, keep_index=True):
+    """
+    merge a list of AnnData objects
+    :param adata_list:
+    :param keep_index:
+    :return:
+    """
+    # all_dataset_id = list(cell_type2dataset_n.keys())
+    merged = None
+    if keep_index:
+        index_unique = None
+    else:
+        index_unique = "-"
+    for i in range(len(adata_list)-1):
+        # print('>>> deale with {}'.format(all_dataset_id[i]))
+        next_dataset = adata_list[i+1]
+        if merged is None:
+            current_dataset = adata_list[i]
+            merged = current_dataset.concatenate(next_dataset, index_unique=index_unique)
+        else:
+            merged = merged.concatenate(next_dataset, index_unique=index_unique)
+    return merged
+
+
+# def generate_sc_dataset2(merged_ds, n_samples: int = 5000, cell_types: list = None,
+#                          result_file_path=None, group_by='leiden', n_base=3, filtering: bool = False,
+#                          cd4_high_in_cd8: str = None):
+#     """
+#     Simple version of `generate_sc_dataset`,
+#     generate single cell dataset by averaging the GEP of `n_base` (3 or 5) cells
+#     from the same cell type (or sub cell type, leiden) from merged scRNA-seq dataset
+#
+#     :param merged_ds: all or parts of file 6_dataset_merged_after_batch_correction_filtered.h5ad
+#
+#     :param n_samples: number of samples for each cell type (or sub cell type)
+#
+#     :param cell_types:
+#
+#     :param result_file_path:
+#
+#     :param group_by: group by `cell_type` or `leiden` (sub cell type) when generating single cell dataset
+#
+#     :param n_base: the number of single cells to average
+#
+#     :param filtering: whether filter CD8 T and CD4 T based on the expression of corresponding marker genes
+#
+#     :param cd4_high_in_cd8: how to deal with the CD8 T cells that CD4 markers are highly expressed
+#         (remove, CD4, CD8)
+#
+#     :return: a file of an AnnData object with log2(CPM + 1) GEP
+#     """
+#     if not os.path.exists(result_file_path):
+#         cell_type2sc = {}
+#         cells_cd4_high_in_cd8 = merged_ds.obs.loc[(merged_ds.obs['cell_type'] == 'CD8 T') &
+#                                                   (merged_ds.obs['m_cd4/m_cd8 group'] == 'middle'), :].index.to_list()
+#         if cd4_high_in_cd8 == 'remove':
+#             merged_ds = merged_ds[~merged_ds.obs.index.isin(cells_cd4_high_in_cd8), :].copy()
+#             print('   The CD8 T cells with highly expressed CD4 T markers will be removed...')
+#         elif cd4_high_in_cd8 == 'CD4':
+#             merged_ds.obs['leiden'].cat.add_categories(['CD4-high (1)', 'CD4-high (2)'], inplace=True)
+#             merged_ds.obs.loc[merged_ds.obs.index.isin(cells_cd4_high_in_cd8), 'leiden'] = \
+#                 merged_ds.obs.loc[merged_ds.obs.index.isin(cells_cd4_high_in_cd8),
+#                                   'leiden'].replace({'CD8 T (1)': 'CD4-high (1)', 'CD8 T (2)': 'CD4-high (2)'})
+#             merged_ds.obs.loc[merged_ds.obs.index.isin(cells_cd4_high_in_cd8), ['cell_type']] = \
+#                 merged_ds.obs.loc[merged_ds.obs.index.isin(cells_cd4_high_in_cd8), 'cell_type'].replace('CD8 T', 'CD4 T')
+#         print(merged_ds)
+#         print(merged_ds.obs.loc[:, 'leiden'].value_counts())
+#         # print(merged_ds.obs.loc[merged_ds.obs['cell_type'] == 'CD4 T', 'leiden'].value_counts())
+#         for ct in cell_types:
+#             print('   >>> deal with cell type {}'.format(ct))
+#             if group_by == 'leiden':
+#                 sub_cell_types = sorted(list(merged_ds.obs.loc[merged_ds.obs['cell_type'] == ct, 'leiden'].unique()))
+#                 # print(sub_cell_types)
+#                 for sct in sub_cell_types:
+#                     print('       deal with sub cell type {}'.format(sct))
+#                     current_adata = merged_ds[merged_ds.obs['leiden'] == sct, :].copy()
+#                     generated = generate_sc(current_adata, n=n_samples, cell_type=sct, group_by=group_by,
+#                                             n_base=n_base, filtering=filtering, cell_type_scope=cell_types)
+#                     cell_type2sc[sct] = generated
+#             elif group_by == 'cell_type':
+#                 current_adata = merged_ds[merged_ds.obs['cell_type'] == ct, :].copy()
+#                 generated = generate_sc(current_adata, n=n_samples, cell_type=ct, group_by=group_by,
+#                                         n_base=n_base, filtering=filtering, cell_type_scope=cell_types)
+#                 cell_type2sc[ct] = generated
+#             else:
+#                 raise ValueError('Unrecognized parameter group_by {}, group_by should be "leiden" for sub cell type '
+#                                  'or "cell_type" for cell type'.format(group_by))
+#         all_adata = list(cell_type2sc.values())
+#         all_generated_data = merge_adata(all_adata)
+#         print(all_generated_data.obs['cell_type'].value_counts())
+#
+#         # clustering
+#         print('   >>> clustering generated single cell dataset...')
+#         if 'leiden' in all_generated_data.obs.columns:
+#             all_generated_data.obs['sub_cell_type'] = all_generated_data.obs['leiden'].copy()
+#         # sc_file_dir = os.path.dirname(sc_file_path)
+#         sc.tl.pca(all_generated_data, svd_solver='arpack', n_comps=100, use_highly_variable=False, zero_center=False)
+#         # sc.pl.pca_variance_ratio(sc_dataset, n_pcs=30)
+#         sc.pp.neighbors(all_generated_data, n_neighbors=10, n_pcs=40)
+#         sc.tl.umap(all_generated_data)
+#         sc.tl.leiden(all_generated_data)
+#         all_generated_data.write(result_file_path)
+#     else:
+#         print(f'   Previous result has existed: {result_file_path}')
+
+
+def filter_cells_by_marker_gene(single_cell_dataset, cell_types: list = None, cell_type2markers: dict = None,
+                                exp_range: tuple = (50, 320), dataset_id: str = '', groupby: str = 'leiden',
+                                max_exp: float = 0.0):
+    """
+
+    :param single_cell_dataset:
+    :param cell_types:
+    :param cell_type2markers:
+    :param exp_range: (low_exp_threshold, middle_exp_threshold)
+    :param dataset_id:
+    :param groupby: index of groupby
+    :param max_exp: max expression to plot
+    :return:
+    """
+    cd4_cd8_ratio = 10
+    assert type(single_cell_dataset) == an.AnnData
+    all_removed_cells = []
+    dataset2filter_info = pd.DataFrame(columns=['n_before_filtering', 'n_after_filtering', 'hit_cell_type'],
+                                       index=list(single_cell_dataset.obs['leiden'].unique()))
+    dataset2filter_info.index.name = 'leiden'
+    cell_type_exp_value_collector_total = []
+    for gi, group in single_cell_dataset.obs.groupby([groupby]):
+        print(gi, group.shape)
+        # cell_type2exp_value_collector_current_gi = []
+        current_part_data = single_cell_dataset[single_cell_dataset.obs.index.isin(group.index), :].copy()
+        gene_exp = pd.DataFrame(current_part_data.X.A, columns=current_part_data.var.index,
+                                index=current_part_data.obs.index)
+        gene_exp = log_exp2cpm(gene_exp)  # convert the expression values from log2(CPM + 1) to CPM
+
+        cell_type_marker_exp = pd.DataFrame(index=gene_exp.index, columns=cell_types)  # sample by cell_type
+        cell_type_quantile = pd.DataFrame(index=['q_10', 'q_25', 'q_50', 'q_75', 'q_90', 'q_95'],
+                                          columns=cell_types)
+
+        # cell_type2exp_flatten = {}
+
+        for k, _cell_type in enumerate(cell_types):
+            if _cell_type in cell_type2markers.keys():
+                current_marker_gene = cell_type2markers[_cell_type]
+                # cell_type2marker_exp[_cell_type] = gene_exp.loc[:, current_marker_gene].copy()  # a dataFrame
+                method = 'mean'
+                if _cell_type in ['B Cells', 'CD4 T']:
+                    method = 'max'
+                cell_type_marker_exp[_cell_type] = \
+                    cal_exp_by_gene_list(gene_exp, gene_list=current_marker_gene, method=method, min_exp_value=1)
+                _values = cell_type_marker_exp[_cell_type].values
+                cell_type_quantile[_cell_type] = [np.quantile(_values, 0.1),
+                                                  np.quantile(_values, 0.25),
+                                                  np.quantile(_values, 0.50),
+                                                  np.quantile(_values, 0.75),
+                                                  np.quantile(_values, 0.90),
+                                                  np.quantile(_values, 0.95)]
+        if max_exp > 0:
+            cell_type_marker_exp[cell_type_marker_exp > max_exp] = max_exp
+        cell_type_marker_exp['m_max_cd4/mean_cd8'] = cell_type_marker_exp['CD4 T'] / cell_type_marker_exp['CD8 T']
+        # ct2e_gi['m_max_cd4/mean_cd8'] = ct2e_gi['m_max_CD4 T'] / ct2e_gi['m_mean_CD8 T']
+        cell_type_marker_exp['m_cd4/m_cd8 group'] = 'middle'
+        cell_type_marker_exp.loc[cell_type_marker_exp['m_max_cd4/mean_cd8'] > cd4_cd8_ratio,
+                                 'm_cd4/m_cd8 group'] = 'high'
+        cell_type_marker_exp.loc[cell_type_marker_exp['m_max_cd4/mean_cd8'] < (1 / cd4_cd8_ratio),
+                                 'm_cd4/m_cd8 group'] = 'low'
+        cell_type_exp_value_collector_total.append(cell_type_marker_exp.copy())
+
+        n_cells = gene_exp.shape[0]
+        t_cell_marker = 'low'
+        removed_cells = {}
+        hit_cell_type = None
+        dataset2filter_info.loc[gi, 'n_before_filtering'] = n_cells
+        for k, _cell_type in enumerate(cell_types):
+            if _cell_type in cell_type2markers.keys():
+                q50_current_cell_type = cell_type_quantile.loc['q_50', _cell_type]
+                # q90_current_cell_type = cell_type_quantile.loc['q_90', _cell_type]
+                if q50_current_cell_type < exp_range[1]:  # Q50 in low or middle expression range
+                    # 50% cells are expressed low as current cell type
+                    if _cell_type not in ['CD4 T', 'CD8 T']:
+                        # don't check CD4 T since the markers of CD4 may express in other cell types
+                        removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type=_cell_type,
+                                                             cell_type_marker_exp=cell_type_marker_exp,
+                                                             filter_upper=exp_range[1])
+                    elif _cell_type == 'CD8 T':
+                        if t_cell_marker != 'high':
+                            # only filter CD8 T when t_cell_marker is not high
+                            removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type=_cell_type,
+                                                                 cell_type_marker_exp=cell_type_marker_exp,
+                                                                 filter_upper=exp_range[1])
+                        else:  # t_cell_marker == 'high'
+                            if (q50_current_cell_type >= exp_range[0]) and (q50_current_cell_type < exp_range[1]):
+                                # Q50 quantile in middle expression range
+                                # Treat this cell type as CD8 T (may be CD8 Tex)
+                                # filtering by CD4 T / CD8 T
+                                _result = filter_cd4_cd8(removed_cells=removed_cells, cell_type=_cell_type,
+                                                         cell_type_marker_exp=cell_type_marker_exp,
+                                                         cell_type_quantile=cell_type_quantile,
+                                                         exp_range=exp_range)
+                                removed_cells = update_removed_cells(removed_cells=_result['removed_cells'],
+                                                                     cell_type=_cell_type,
+                                                                     cell_type_marker_exp=cell_type_marker_exp,
+                                                                     filter_lower=_result['filter_lower'],
+                                                                     filter_upper=_result['filter_upper'])
+                                hit_cell_type = 'CD8 T'
+                                break
+
+                else:  # the marker genes of current cell type are highly expressed (Q50 in high expression range)
+                    if _cell_type == 'T Cells':
+                        t_cell_marker = 'high'
+
+                    if (n_cells - len(removed_cells)) >= 3000:  # remove 35% since too many cells in this cluster
+                        filter_lower = cell_type_quantile.loc['q_25', _cell_type]
+                        filter_upper = cell_type_quantile.loc['q_90', _cell_type]
+                    else:  # remove 15% since a few cells
+                        filter_lower = cell_type_quantile.loc['q_10', _cell_type]
+                        filter_upper = cell_type_quantile.loc['q_95', _cell_type]
+
+                    if t_cell_marker != 'high':  # filtering by quantile, t_cell_marker is low or middle
+                        if _cell_type not in ['CD4 T', 'NK']:
+                            removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type=_cell_type,
+                                                                 cell_type_marker_exp=cell_type_marker_exp,
+                                                                 filter_lower=filter_lower, filter_upper=filter_upper)
+                        elif _cell_type == 'NK':  # don't check CD4 T when t_cell_marker is low or middle
+                            # filtering by CD4 T / CD8 T
+                            _result = filter_cd4_cd8(removed_cells=removed_cells, cell_type=_cell_type,
+                                                     cell_type_marker_exp=cell_type_marker_exp,
+                                                     cell_type_quantile=cell_type_quantile,
+                                                     exp_range=exp_range)
+                            removed_cells = update_removed_cells(removed_cells=_result['removed_cells'],
+                                                                 cell_type=_cell_type,
+                                                                 cell_type_marker_exp=cell_type_marker_exp,
+                                                                 filter_lower=_result['filter_lower'],
+                                                                 filter_upper=_result['filter_upper'])
+                        else:  # don't check CD4 T when t_cell_marker is low or middle
+                            continue
+
+                    else:  # t_cell_marker is high
+                        _result = None
+                        if _cell_type == 'T Cells':
+                            pass
+                        elif _cell_type in ['CD8 T', 'CD4 T', 'NK']:
+                            # filtering by CD4 T / CD8 T
+                            _result = filter_cd4_cd8(removed_cells=removed_cells, cell_type=_cell_type,
+                                                     cell_type_marker_exp=cell_type_marker_exp,
+                                                     cell_type_quantile=cell_type_quantile, exp_range=exp_range)
+                            removed_cells = update_removed_cells(removed_cells=_result['removed_cells'],
+                                                                 cell_type=_cell_type,
+                                                                 cell_type_marker_exp=cell_type_marker_exp,
+                                                                 filter_lower=_result['filter_lower'],
+                                                                 filter_upper=_result['filter_upper'])
+
+                    if _cell_type != 'T Cells':
+                        hit_cell_type = _cell_type
+                        break  # first hit except "T Cells", filtering by this cell type and stopped
+        dataset2filter_info.loc[gi, 'n_after_filtering'] = n_cells - len(removed_cells)
+        dataset2filter_info.loc[gi, 'hit_cell_type'] = hit_cell_type
+        if len(removed_cells) > 0:
+            _cell_ids = list(removed_cells.keys())
+            all_removed_cells += _cell_ids
+    cell_type_exp_value_collector_total_df = pd.concat(cell_type_exp_value_collector_total)
+    cell_type_exp_value_collector_total_df = cell_type_exp_value_collector_total_df.loc[single_cell_dataset.obs.index, :]
+    assert np.all(single_cell_dataset.obs.index == cell_type_exp_value_collector_total_df.index)
+    single_cell_dataset.obs['m_max_cd4/mean_cd8'] = cell_type_exp_value_collector_total_df['m_max_cd4/mean_cd8']
+    single_cell_dataset.obs['m_cd4/m_cd8 group'] = cell_type_exp_value_collector_total_df['m_cd4/m_cd8 group']
+    filtered_dataset = single_cell_dataset[~single_cell_dataset.obs.index.isin(all_removed_cells), :].copy()
+    dataset2filter_info['dataset_id'] = dataset_id
+    return filtered_dataset, dataset2filter_info
+
+
+def update_removed_cells(removed_cells: dict = None, cell_type_marker_exp: pd.DataFrame = None,
+                         filter_upper: float = None, filter_lower: float = None, cell_type: str = '') -> dict:
+    """
+
+    :param removed_cells:
+    :param cell_type_marker_exp:
+    :param filter_upper: filter_upper > filter_lower
+    :param filter_lower:
+    :param cell_type
+    :return:
+    """
+    if (filter_lower is not None) and (filter_upper is not None):
+        _removed = cell_type_marker_exp.loc[(cell_type_marker_exp[cell_type] > filter_upper) |
+                                            (cell_type_marker_exp[cell_type] <= filter_lower), :].index.to_list()
+    elif filter_lower is None:
+        _removed = cell_type_marker_exp.loc[(cell_type_marker_exp[cell_type] > filter_upper), :].index.to_list()
+    elif filter_upper is None:
+        _removed = cell_type_marker_exp.loc[(cell_type_marker_exp[cell_type] <= filter_lower), :].index.to_list()
+    else:
+        raise KeyError('Both filter_lower and filter_upper are None')
+    if len(_removed) > 0:
+        for _ in _removed:
+            removed_cells[_] = 1
+
+    return removed_cells
+
+
+def filter_by_cd8_marker(removed_cells: dict = None, cell_type_marker_exp: pd.DataFrame = None,
+                         cell_type_quantile: pd.DataFrame = None, cell_type: str = '',
+                         exp_range: tuple = None):
+    removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type='CD8 T',
+                                         cell_type_marker_exp=cell_type_marker_exp,
+                                         filter_upper=exp_range[0])
+    n_cells = cell_type_marker_exp.shape[0]
+    # check n_cells - len(removed_cells) again
+    if (n_cells - len(removed_cells)) >= 3000:  # remove 35% since too many cells
+        filter_lower = cell_type_quantile.loc['q_25', cell_type]
+        filter_upper = cell_type_quantile.loc['q_90', cell_type]
+    else:  # remove 15% since a few cells
+        filter_lower = cell_type_quantile.loc['q_10', cell_type]
+        filter_upper = cell_type_quantile.loc['q_95', cell_type]
+    return {'removed_cells': removed_cells, 'filter_lower': filter_lower, 'filter_upper': filter_upper}
+
+
+def filter_by_cd4_marker(removed_cells: dict = None, cell_type_marker_exp: pd.DataFrame = None,
+                         cell_type_quantile: pd.DataFrame = None, cell_type: str = '', exp_range: tuple = None):
+    q50 = cell_type_quantile.loc['q_50', 'CD4 T']
+    filter_upper = min(q50, exp_range[1])
+    removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type='CD4 T',
+                                         cell_type_marker_exp=cell_type_marker_exp,
+                                         filter_upper=filter_upper)
+    n_cells = cell_type_marker_exp.shape[0]
+    # check n_cells - len(removed_cells) again
+    if (n_cells - len(removed_cells)) >= 3000:  # remove 35% since too many cells
+        filter_lower = cell_type_quantile.loc['q_25', cell_type]
+        filter_upper = cell_type_quantile.loc['q_90', cell_type]
+    else:  # remove 15% since a few cells
+        filter_lower = cell_type_quantile.loc['q_10', cell_type]
+        filter_upper = cell_type_quantile.loc['q_95', cell_type]
+    return {'removed_cells': removed_cells, 'filter_lower': filter_lower, 'filter_upper': filter_upper}
+
+
+def filter_cd4_cd8(removed_cells: dict = None, cell_type: str = '', exp_range: tuple = (),
+                   cell_type_marker_exp: pd.DataFrame = None, cell_type_quantile: pd.DataFrame = None):
+    """
+    filter cells by the ratio of marker genes expression between CD4 T and CD8 T (max CD4 T / mean CD8 T) or
+    the expression value
+    :param removed_cells:
+    :param cell_type: current cell type with high expression of it's marker genes
+    :param exp_range:
+    :param cell_type_marker_exp:
+    :param cell_type_quantile:
+    :return:
+    """
+    # q50 = cell_type_quantile.loc['q_50', 'CD4 T']
+    # filter_upper = min(q50, exp_range[1])
+    # removed_cells = update_removed_cells(removed_cells=removed_cells, cell_type='CD4 T',
+    #                                      cell_type_marker_exp=cell_type_marker_exp,
+    #                                      filter_upper=filter_upper)
+    _removed = []
+    if cell_type == 'CD4 T':
+        _removed = cell_type_marker_exp.loc[cell_type_marker_exp['m_cd4/m_cd8 group'] != 'high', :].index.to_list()
+    elif cell_type == 'CD8 T':
+        _removed = cell_type_marker_exp.loc[cell_type_marker_exp['m_cd4/m_cd8 group'] == 'high', :].index.to_list()
+        # _removed = cell_type_marker_exp.loc[cell_type_marker_exp['m_cd4/m_cd8 group'] != 'low', :].index.to_list()
+    elif cell_type == 'NK':  # both CD4 T marker and CD8 T marker should be low
+        _removed = cell_type_marker_exp.loc[(cell_type_marker_exp['CD8 T'] > exp_range[1]) |
+                                            (cell_type_marker_exp['CD4 T'] > exp_range[1]), :].index.to_list()
+
+    if len(_removed) > 0:
+        for _ in _removed:
+            removed_cells[_] = 1
+
+    n_cells = cell_type_marker_exp.shape[0]
+    # check n_cells - len(removed_cells) again
+    if (n_cells - len(removed_cells)) >= 3000:  # remove 35% since too many cells
+        filter_lower = cell_type_quantile.loc['q_25', cell_type]
+        filter_upper = cell_type_quantile.loc['q_90', cell_type]
+    else:  # remove 15% since a few cells
+        filter_lower = cell_type_quantile.loc['q_10', cell_type]
+        filter_upper = cell_type_quantile.loc['q_95', cell_type]
+    return {'removed_cells': removed_cells, 'filter_lower': filter_lower, 'filter_upper': filter_upper}
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `DeSide-1.0.1/deside/utility/__init__.py` & `DeSide-1.0.2/deside/utility/__init__.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from .pub_func import print_df
-from .pub_func import filter_gene_by_expression_log_mean, filter_gene_by_expression_min_max, filter_sample_by_expression
-from .pub_func import log2_transform, center_value
-from .pub_func import filter_gene_by_variance
-from .pub_func import read_exp_from_hcluster
-from .pub_func import read_cancer_purity
-from .pub_func import cal_relative_error
-from .pub_func import calculate_rmse, calculate_r2
-from .pub_func import check_dir, parse_log_file, write_to_log
-from .pub_func import correct_gene_list
-from .pub_func import extract_gz_file
-from .pub_func import read_data_from_h5ad, create_h5ad_dataset
-from .pub_func import log_exp2cpm, ciber_exp, non_log2log_cpm, non_log2cpm
-from .pub_func import get_corr, get_sep
-from .pub_func import read_marker_gene
-from .pub_func import cal_exp_by_gene_list
-from .pub_func import print_msg, save_key_params
-from .pub_func import read_xy, read_df
-from .pub_func import cal_corr_gene_exp_with_cell_frac
-from .pub_func import aggregate_marker_gene_exp
-from .pub_func import cal_marker_ratio
-from .core_obj import QueryNeighbors, ExpObj
-from .pub_func import default_core_marker_genes
-from .pub_func import get_cell_num
-from .pub_func import sorted_cell_types, get_inx2cell_type
-from .pub_func import do_pca_analysis, do_umap_analysis
-from .pub_func import set_fig_style
-from .evaluation import get_core_zone_of_pca
-from .pub_func import get_ccc
-
-
-subcell_type2abbr = {'B Cells (1)': 'B1', 'B Cells (2)': 'B2', 'B Cells (3)': 'B3', 'B Cells (4)': 'B4',
-                     'Epithelial Cells (1)': 'CC1', 'Epithelial Cells (2)': 'CC2', 'Epithelial Cells (3)': 'CC3',
-                     'CD4 T (1)': 'CD4T1', 'CD4 T (2)': 'CD4T2', 'CD4 T (3)': 'CD4T3',
-                     'CD8 T': 'CD8T', 'CD8 Tex': 'CD8Tex',
-                     'pDC': 'pDC', 'mDC': 'mDC', 'Fibroblasts (1)': 'F1', 'Fibroblasts (2)': 'F2',
-                     'Mast Cells': 'MC', 'NK': 'NK',
-                     'Macrophages (1)': 'MP1', 'Macrophages (2)': 'MP2',
-                     'Macrophages (3)': 'MP3', 'Macrophages (4)': 'MP4',
-                     'Neutrophils': 'NEU', 'Endothelial Cells': 'EC'}
-
-
-cell_type2abbr = {'B Cells': 'B', 'CD4 T': 'CD4T', 'CD8 T': 'CD8T', 'Cancer Cells': 'CC', 'DC': 'DC',
-                  'Endothelial Cells': 'EC', 'Fibroblasts': 'F', 'Macrophages': 'MP', 'Mast Cells': 'MC',
-                  'NK': 'NK', 'Neutrophils': 'NEU'}
-
-cell_type_mapping = {'B Cells (1)': 'B Cells', 'B Cells (2)': 'B Cells', 'B Cells (3)': 'B Cells',
-                     'B Cells (4)': 'B Cells',
-                     'Cancer Cells (1)': 'Cancer Cells', 'Cancer Cells (2)': 'Cancer Cells',
-                     'Epithelial Cells (1)': 'Cancer Cells', 'Epithelial Cells (2)': 'Cancer Cells',
-                     'Epithelial Cells (3)': 'Cancer Cells',
-                     'CD4 T (1)': 'CD4 T', 'CD4 T (2)': 'CD4 T', 'CD4 T (3)': 'CD4 T',
-                     'CD8 T': 'CD8 T', 'CD8 T (1)': 'CD8 T', 'CD8 T (2)': 'CD8 T', 'CD8 Tex': 'CD8 T',
-                     'pDC': 'DC', 'mDC': 'DC',
-                     'Fibroblasts': 'Fibroblasts', 'Fibroblasts (1)': 'Fibroblasts', 'Fibroblasts (2)': 'Fibroblasts',
-                     'Mast Cells': 'Mast Cells', 'NK': 'NK',
-                     'Macrophages': 'Macrophages', 'Macrophages (1)': 'Macrophages', 'Macrophages (2)': 'Macrophages',
-                     'Macrophages (3)': 'Macrophages', 'Macrophages (4)': 'Macrophages',
-                     'Monocyte/Macrophages (1)': 'Macrophages',
-                     'Monocytes/Macrophages (2)': 'Macrophages',
-                     'Neutrophils': 'Neutrophils', 'Endothelial Cells': 'Endothelial Cells'}
-
-
-cancer_types = ['ACC', 'BLCA', 'BRCA', 'GBM', 'HNSC', 'LGG', 'LIHC', 'LUAD', 'PAAD', 'PRAD',
-                'CESC', 'COAD', 'KICH', 'KIRC', 'KIRP', 'LUSC', 'READ', 'THCA', 'UCEC']
-
-
-# used in the function "get_purified_gep" of decon_cf.reg_model and plot.evaluate_result
-error_type = {2: 'both less', 3: 'z_score outlier', 7: 'relative error outlier', 8: 'both greater'}
-
-# core marker genes, ref to file "DeSide_example/01single_cell/selected_marker_genes.csv"
-default_core_marker_genes_old = {'CD4 T': ['MAL', 'CD40LG', 'FBLN7', 'IL7R', 'FOXP3'],
-                                 'CD8 T': ['CD8A', 'CD8B'], 'T Cells': ['CD2', 'CD3D', 'CD3E'],
-                                 'B Cells': ['VPREB3', 'POU2AF1', 'BANK1', 'CD19', 'CD22', 'CD79A', 'FCRL5', 'MS4A1'],
-                                 'DC': ['LAMP3', 'FLT3', 'IRF7', 'PPP1R14B', 'SMPD3'],
-                                 'Endothelial Cells': ['CLDN5', 'ENG', 'PLVAP', 'VWF'],
-                                 'Fibroblasts': ['COL1A1', 'COL1A2', 'COL3A1', 'MYL9'],
-                                 'Macrophages': ['AIF1', 'CD14', 'CD163', 'MS4A7', 'C1QC', 'C1QB'],
-                                 'Mast Cells': ['CPA3', 'HPGDS', 'GATA2'],
-                                 'NK': ['KLRD1', 'CEP78'],
-                                 'Neutrophils': ['CSF3R', 'CXCR2', 'FPR1']}
-
-
-inx2single_cell_dataset_id = {
-    1: 'hnscc_cillo_01',
-    2: 'pdac_pengj_02',
-    3: 'hnscc_puram_03',
-    4: 'pdac_steele_04',
-    5: 'luad_kim_05',
-    6: 'nsclc_guo_06',
-    7: 'pan_cancer_07'
-}
+from .pub_func import print_df
+from .pub_func import filter_gene_by_expression_log_mean, filter_gene_by_expression_min_max, filter_sample_by_expression
+from .pub_func import log2_transform, center_value
+from .pub_func import filter_gene_by_variance
+from .pub_func import read_exp_from_hcluster
+from .pub_func import read_cancer_purity
+from .pub_func import cal_relative_error
+from .pub_func import calculate_rmse, calculate_r2
+from .pub_func import check_dir, parse_log_file, write_to_log
+from .pub_func import correct_gene_list
+from .pub_func import extract_gz_file
+from .pub_func import read_data_from_h5ad, create_h5ad_dataset
+from .pub_func import log_exp2cpm, ciber_exp, non_log2log_cpm, non_log2cpm
+from .pub_func import get_corr, get_sep
+from .pub_func import read_marker_gene
+from .pub_func import cal_exp_by_gene_list
+from .pub_func import print_msg, save_key_params
+from .pub_func import read_xy, read_df
+from .pub_func import cal_corr_gene_exp_with_cell_frac
+from .pub_func import aggregate_marker_gene_exp
+from .pub_func import cal_marker_ratio
+from .core_obj import QueryNeighbors, ExpObj
+from .pub_func import default_core_marker_genes
+from .pub_func import get_cell_num
+from .pub_func import sorted_cell_types, get_inx2cell_type
+from .pub_func import do_pca_analysis, do_umap_analysis
+from .pub_func import set_fig_style
+from .evaluation import get_core_zone_of_pca
+from .pub_func import get_ccc
+
+
+subcell_type2abbr = {'B Cells (1)': 'B1', 'B Cells (2)': 'B2', 'B Cells (3)': 'B3', 'B Cells (4)': 'B4',
+                     'Epithelial Cells (1)': 'CC1', 'Epithelial Cells (2)': 'CC2', 'Epithelial Cells (3)': 'CC3',
+                     'CD4 T (1)': 'CD4T1', 'CD4 T (2)': 'CD4T2', 'CD4 T (3)': 'CD4T3',
+                     'CD8 T': 'CD8T', 'CD8 Tex': 'CD8Tex',
+                     'pDC': 'pDC', 'mDC': 'mDC', 'Fibroblasts (1)': 'F1', 'Fibroblasts (2)': 'F2',
+                     'Mast Cells': 'MC', 'NK': 'NK',
+                     'Macrophages (1)': 'MP1', 'Macrophages (2)': 'MP2',
+                     'Macrophages (3)': 'MP3', 'Macrophages (4)': 'MP4',
+                     'Neutrophils': 'NEU', 'Endothelial Cells': 'EC'}
+
+
+cell_type2abbr = {'B Cells': 'B', 'CD4 T': 'CD4T', 'CD8 T': 'CD8T', 'Cancer Cells': 'CC', 'DC': 'DC',
+                  'Endothelial Cells': 'EC', 'Fibroblasts': 'F', 'Macrophages': 'MP', 'Mast Cells': 'MC',
+                  'NK': 'NK', 'Neutrophils': 'NEU'}
+
+cell_type_mapping = {'B Cells (1)': 'B Cells', 'B Cells (2)': 'B Cells', 'B Cells (3)': 'B Cells',
+                     'B Cells (4)': 'B Cells',
+                     'Cancer Cells (1)': 'Cancer Cells', 'Cancer Cells (2)': 'Cancer Cells',
+                     'Epithelial Cells (1)': 'Cancer Cells', 'Epithelial Cells (2)': 'Cancer Cells',
+                     'Epithelial Cells (3)': 'Cancer Cells',
+                     'CD4 T (1)': 'CD4 T', 'CD4 T (2)': 'CD4 T', 'CD4 T (3)': 'CD4 T',
+                     'CD8 T': 'CD8 T', 'CD8 T (1)': 'CD8 T', 'CD8 T (2)': 'CD8 T', 'CD8 Tex': 'CD8 T',
+                     'pDC': 'DC', 'mDC': 'DC',
+                     'Fibroblasts': 'Fibroblasts', 'Fibroblasts (1)': 'Fibroblasts', 'Fibroblasts (2)': 'Fibroblasts',
+                     'Mast Cells': 'Mast Cells', 'NK': 'NK',
+                     'Macrophages': 'Macrophages', 'Macrophages (1)': 'Macrophages', 'Macrophages (2)': 'Macrophages',
+                     'Macrophages (3)': 'Macrophages', 'Macrophages (4)': 'Macrophages',
+                     'Monocyte/Macrophages (1)': 'Macrophages',
+                     'Monocytes/Macrophages (2)': 'Macrophages',
+                     'Neutrophils': 'Neutrophils', 'Endothelial Cells': 'Endothelial Cells'}
+
+
+cancer_types = ['ACC', 'BLCA', 'BRCA', 'GBM', 'HNSC', 'LGG', 'LIHC', 'LUAD', 'PAAD', 'PRAD',
+                'CESC', 'COAD', 'KICH', 'KIRC', 'KIRP', 'LUSC', 'READ', 'THCA', 'UCEC']
+
+
+# used in the function "get_purified_gep" of decon_cf.reg_model and plot.evaluate_result
+error_type = {2: 'both less', 3: 'z_score outlier', 7: 'relative error outlier', 8: 'both greater'}
+
+# core marker genes, ref to file "DeSide_example/01single_cell/selected_marker_genes.csv"
+default_core_marker_genes_old = {'CD4 T': ['MAL', 'CD40LG', 'FBLN7', 'IL7R', 'FOXP3'],
+                                 'CD8 T': ['CD8A', 'CD8B'], 'T Cells': ['CD2', 'CD3D', 'CD3E'],
+                                 'B Cells': ['VPREB3', 'POU2AF1', 'BANK1', 'CD19', 'CD22', 'CD79A', 'FCRL5', 'MS4A1'],
+                                 'DC': ['LAMP3', 'FLT3', 'IRF7', 'PPP1R14B', 'SMPD3'],
+                                 'Endothelial Cells': ['CLDN5', 'ENG', 'PLVAP', 'VWF'],
+                                 'Fibroblasts': ['COL1A1', 'COL1A2', 'COL3A1', 'MYL9'],
+                                 'Macrophages': ['AIF1', 'CD14', 'CD163', 'MS4A7', 'C1QC', 'C1QB'],
+                                 'Mast Cells': ['CPA3', 'HPGDS', 'GATA2'],
+                                 'NK': ['KLRD1', 'CEP78'],
+                                 'Neutrophils': ['CSF3R', 'CXCR2', 'FPR1']}
+
+
+inx2single_cell_dataset_id = {
+    1: 'hnscc_cillo_01',
+    2: 'pdac_pengj_02',
+    3: 'hnscc_puram_03',
+    4: 'pdac_steele_04',
+    5: 'luad_kim_05',
+    6: 'nsclc_guo_06',
+    7: 'pan_cancer_07'
+}
```

### Comparing `DeSide-1.0.1/deside/utility/compare.py` & `DeSide-1.0.2/deside/utility/compare.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-import os
-import warnings
-import pandas as pd
-from scipy.stats import percentileofscore
-from .pub_func import check_dir, read_marker_gene, read_df, sorted_cell_types
-from ..utility import log_exp2cpm, non_log2cpm, aggregate_marker_gene_exp
-
-name_mapping_CIBERSORT = {"B cells": 'B Cells', "T cells CD8": 'CD8 T', "T cells CD4": 'CD4 T',
-                          "Macrophages": 'Macrophages', "Dendritic cells": 'DC',
-                          "Mast cells": 'Mast Cells', "Myocytes": 'myocyte', "CAFs": 'Fibroblasts',
-                          "Endothelial cells": 'Endothelial cells', "Malignant cells": 'Cancer Cells'}
-
-
-def parse_result_from_cibersort(result_file_path):
-    """
-
-    :param result_file_path:
-    :return:
-    """
-    name_mapping_reverse = {}
-    for i, j in name_mapping_CIBERSORT.items():
-        if j not in name_mapping_reverse:
-            name_mapping_reverse[j] = []
-        name_mapping_reverse[j].append(i)
-    result_from_cibersort = pd.read_csv(result_file_path, index_col=0)
-    result = pd.DataFrame(index=result_from_cibersort.index, columns=list(name_mapping_reverse.keys()))
-    for col in result.columns:
-        result[col] = result_from_cibersort.loc[:, name_mapping_reverse[col]].sum(axis=1)
-    cell_types = [i for i in sorted_cell_types if i in result.columns]
-    return result.loc[:, cell_types]
-
-
-def _read_result(file_path, cell_type_name_mapping, cell_types, algo=None):
-    """
-    read a single result file from different algorithms for performance comparison ()
-    :param file_path:
-    :param cell_type_name_mapping: mapping from cell type names of current algo to cell type names in DeSide
-    :param algo: the name of each algorithm, CIBERSORT, MuSiC, EPIC, Scaden, Scaden-web and DeSide
-    :return:
-    """
-    predicted_result = read_df(file_path)
-    predicted_result.rename(columns=cell_type_name_mapping, inplace=True)
-    predicted_result.index = predicted_result.index.map(lambda x: x.replace('.', '-'))
-    return predicted_result.loc[:, cell_types]
-
-
-def read_and_merge_result(raw_result_dir: str, cell_type_name_mapping: dict, algo: str,
-                          result_file_path=None, tcga_sample2cancer_type_file_path=None) -> pd.DataFrame:
-    """
-    read and merge predicted cell fractions of each algorithm
-    :param raw_result_dir:
-    :param cell_type_name_mapping: mapping from cell type names of current algo to cell type names in DeSide
-    :param algo: EPIC, CIBERSORT, MuSiC, DeSide and Scaden
-    :param result_file_path:
-    :param tcga_sample2cancer_type_file_path: the file path of sample id to cancer type mapping file in TCGA
-    :return:
-    """
-    cell_types = [i for i in sorted_cell_types if i in list(cell_type_name_mapping.values())]
-    cancer_dataset2file_path = {}
-    cancer_type = ''
-    ds = ''  # reference dataset
-    assert os.path.exists(raw_result_dir), '{} does not exist'.format(raw_result_dir)
-    for root, dirs, files in os.walk(raw_result_dir):
-        for file_name in files:
-            if (('.txt' in file_name) or (f'.csv' in file_name)) and \
-                    ('cancer_purity' not in file_name) and ('signature_score' not in file_name):
-                if 'CIBERSORT' in algo:
-                    _, _, _, cancer_type, ds, _ = file_name.split('_')
-                elif algo == 'MuSiC':
-                    cancer_type, ds, _ = file_name.split('_')
-                    ds = ds.replace('LUAD1', 'LUAD')
-                elif 'EPIC' in algo:
-                    if 'NOref' in file_name:
-                        _, cancer_type, ds = file_name.split('_')
-                    else:
-                        cancer_type, _ = file_name.split('.')
-                    if algo == 'EPIC':
-                        ds = '46sig'
-                    else:  # EPIC_self_ref
-                        ds = 'self'
-                elif algo == 'Scaden_ascites':
-                    cancer_type = file_name.split('_')[-1].replace('.txt', '')
-                    ds = 'Ascites'
-                elif algo == 'Scaden_simu_bulk':
-                    cancer_type = file_name.split('_')[-1].replace('.txt', '')
-                    ds = 'simu_bulk_2ds'
-                elif 'DeSide' in algo:
-                    cancer_type = root.split(os.path.sep)[-1]
-                    if '/' in cancer_type:
-                        cancer_type = cancer_type.split('/')[-1]
-                    ds = 'simu_bulk_2ds'
-                    if algo == 'DeSide_softmax':
-                        ds = 'simu_bulk_2ds_softmax'
-                elif algo == 'Kassandra_self':
-                    cancer_type = 'all'
-                    ds = 'self'
-                if '.txt' in ds:
-                    ds = ds.replace('.txt', '')
-                cancer_type = cancer_type.replace('HNSCC', 'HNSC')
-                ds = ds.replace('HNSCC', 'HNSC')
-                assert os.path.exists(os.path.join(root, file_name)), f'{os.path.join(root, file_name)} does not exist'
-                cancer_dataset2file_path[cancer_type + '-' + ds + '_ref'] = os.path.join(root, file_name)
-    # print(cancer_dataset2file_path)
-    sample2cell_frac = {}
-    counter = 0
-    columns = ['sample_id', 'cancer_type', 'reference_dataset'] + cell_types
-
-    for cancer_dataset, file_path in cancer_dataset2file_path.items():
-        # print(cancer_dataset, file_path)
-        cancer_type, ref_dataset = cancer_dataset.split('-')
-        if 'Scaden' in algo:
-            ref_dataset = ref_dataset.replace('Scaden_', '')
-        elif algo == 'DeSide':
-            ref_dataset = ref_dataset.replace('DeSide_', '')
-        if ref_dataset == 'ref':
-            ref_dataset = 'Mixed_ref'
-        current_result = _read_result(file_path, cell_type_name_mapping=cell_type_name_mapping,
-                                      cell_types=cell_types, algo=algo)
-        if algo == 'Kassandra_self':
-            current_result = current_result / 100
-        for row in current_result.iterrows():
-            sample_id = row[0]
-            sample2cell_frac[counter] = [sample_id, cancer_type, ref_dataset] + list(row[1].values)
-            counter += 1
-    merged_result = pd.DataFrame.from_dict(sample2cell_frac, orient='index', columns=columns)
-    if algo == 'Kassandra_self':
-        tcga_sample2cancer_type = pd.read_csv(tcga_sample2cancer_type_file_path, index_col=0)
-        tcga_sample2cancer_type.index = tcga_sample2cancer_type.index.map(lambda x: x.replace('.', '-'))
-        tcga_sample2cancer_type = tcga_sample2cancer_type.to_dict()['cancer_type']
-        merged_result.drop(columns=['cancer_type'], inplace=True)
-        merged_result['cancer_type'] = merged_result['sample_id'].map(lambda x: tcga_sample2cancer_type[x])
-        merged_result = merged_result.loc[:, columns].copy()
-    if result_file_path:
-        if os.path.exists(result_file_path):
-            merged_result.to_csv(result_file_path, mode='a', header=False, float_format='%.3f')
-        else:
-            merged_result.to_csv(result_file_path, float_format='%.3f')
-    else:
-        return merged_result
-
-
-def mean_exp_of_marker_gene(marker_gene_file_path, bulk_tpm_file_path, result_file_path: str = None,
-                            cancer_type: str = None, debug=False, trans=False, cell_types: list = None,
-                            log_exp: bool = False, gene_list_in_model: list = None):
-    """
-    mean expression value of marker genes for each cell type (max expression value for B Cells and CD4 T Cells)
-    :param marker_gene_file_path: file path of selected marker gene for each cell type
-    :param bulk_tpm_file_path: file path of bulk cell TPM, should be gene by sample
-    :param result_file_path
-    :param cancer_type: tumor type / cancer type / test set name
-    :param debug: if output intermediate result for debug
-    :param trans: taking transposition if the bulk cell TPM is organized with sample by gene
-    :param cell_types: cell types
-    :param log_exp: TPM is need. If the expression values are log transformed, it should be transformed to TPM
-    :param gene_list_in_model: filtering bulk_tpm and rescaling to TPM if not None
-    :return: a dataframe, sample by cell type (mean expression of marker genes), and save to file
-    """
-    if result_file_path is not None:
-        result_dir = os.path.dirname(result_file_path)
-        check_dir(result_dir)
-    else:
-        result_dir = '.'
-    temporal_dir = os.path.join(result_dir, 'debug_temp', cancer_type)
-    if debug:
-        check_dir(temporal_dir)
-    include_t_cell = False
-    if (cell_types is not None) and ('T Cells' in cell_types):
-        include_t_cell = True
-        cell_types += ['CD8 T', 'CD4 T']
-    cell_type2marker = read_marker_gene(marker_gene_file_path, include_t_cell=include_t_cell,
-                                        use_cancer_cell=True, corr_mean=True)
-    cell_type2marker = {k: v for k, v in cell_type2marker.items() if k in cell_types}
-    # if ('Cancer Cells' not in cell_type2marker) and ('Epithelial Cells' in cell_type2marker):
-    #     cell_type2marker['Cancer Cells'] = cell_type2marker['Epithelial Cells']
-    # sep = get_sep(bulk_tpm_file_path)
-    # tpm = pd.read_csv(bulk_tpm_file_path, index_col=0, sep=sep)
-    tpm = read_df(bulk_tpm_file_path)
-    if trans:
-        tpm = tpm.T
-    if log_exp:
-        tpm = log_exp2cpm(tpm)
-    if gene_list_in_model is not None:
-        intersection_genes = [i for i in gene_list_in_model if i in tpm.index]
-        if len(intersection_genes) != len(gene_list_in_model):
-            n_diff = len(gene_list_in_model) - len(intersection_genes)
-            warnings.warn(f'There are {n_diff} genes don\'t include in current bulk TPM dataset')
-        tpm = tpm.loc[tpm.index.isin(intersection_genes), :].copy()
-        tpm = non_log2cpm(tpm.T).T  # rescaling to TPM after filtering by gene list in model
-        # print(tpm.sum(axis=0))
-
-    marker_exp = aggregate_marker_gene_exp(exp_df=tpm.T, marker_genes=cell_type2marker)
-    return marker_exp
-
-
-def cal_gene_signature_score(marker_gene_file_path, bulk_tpm_file_path, result_file_path: str = None,
-                             cancer_type: str = None, trans=False, cell_types: list = None):
-    """
-    gene signature score for each cell type,
-      ref to Combes et al., 2022, Cell185, 184–203 (METHOD DETAILS, Gene Signature Score)
-    :param marker_gene_file_path: file path of selected marker gene for each cell type
-    :param bulk_tpm_file_path: file path of bulk cell TPM, should be gene by sample
-    :param result_file_path
-    :param cancer_type: tumor type / cancer type / test set name
-    :param trans: taking transposition if the bulk cell TPM is organized with sample by gene
-    :param cell_types: cell types
-    :return: a dataframe, sample by cell type (gene signature score for each cell type of each sample),
-      and save to file
-    """
-
-    include_t_cell = False
-    if (cell_types is not None) and ('T Cells' in cell_types):
-        include_t_cell = True
-        cell_types += ['CD8 T', 'CD4 T']
-    cell_type2marker = read_marker_gene(marker_gene_file_path, include_t_cell=include_t_cell,
-                                        use_cancer_cell=True)
-    # sep = get_sep(bulk_tpm_file_path)
-    # tpm = pd.read_csv(bulk_tpm_file_path, index_col=0, sep=sep)
-    tpm = read_df(bulk_tpm_file_path)
-    if trans:
-        tpm = tpm.T
-
-    cell_type2signature_score = {}
-    if cell_types is None:
-        cell_types = list(cell_type2marker.keys())
-    for ct in cell_types:
-        marker = cell_type2marker[ct]
-        current_tpm = tpm.loc[tpm.index.isin(marker), :]  # gene by sample, E, m x n matrix of gene expression
-        current_valid_marker = current_tpm.index.to_list()
-        if len(current_valid_marker) > 0:
-            current_marker_str = ', '.join(current_valid_marker)
-            print(f'   Using {len(current_valid_marker)} marker genes for cell type {ct}: {current_marker_str}')
-            # cell_type2mean_exp[ct + '_marker_mean'] = current_tpm.mean(axis=0)
-            p = pd.DataFrame(index=current_tpm.index, columns=current_tpm.columns)
-            for inx, _row in current_tpm.iterrows():
-                p.loc[inx] = [percentileofscore(_row, g_exp) for g_exp in _row]
-            p = p.mean(axis=0)
-            cell_type2signature_score[ct + f'_gene_signature_score'] = \
-                pd.Series(data=[percentileofscore(p, _) for _ in p], index=p.index)
-        else:
-            Warning(f'No any marker genes in bulk cell TPM for cell type {ct}, '
-                    f'this cell type will be ignored in later analysis.')
-    signature_score = pd.DataFrame.from_dict(cell_type2signature_score, orient='columns')
-    if cancer_type is not None:
-        signature_score['cancer_type'] = cancer_type
-    if result_file_path is not None:
-        signature_score.to_csv(result_file_path, float_format='%.3f')
-    return signature_score.round(3)
-
-
-if __name__ == '__main__':
-    pass
-    # algo2merged_file_path = {
-    #     # 'CIBERSORT': './merged_result/CIBERSORT_predicted_cell_fraction.csv',
-    #                          'DeSide': './merged_result/DeSide_predicted_cell_fraction.csv',
-    #                          # 'EPIC': './merged_result/EPIC_predicted_cell_fraction.csv',
-    #                          # 'Scaden': './merged_result/Scaden_predicted_cell_fraction.csv',
-    #                          # 'MuSiC': './merged_result/MuSiC_predicted_cell_fraction.csv'
-    # }
-    # algo2raw_result_dir = {'CIBERSORT': r'D:\project001_data\DeSide_example\04predict_and_compare\CIBERSORT_result',
-    #                        'DeSide': r'D:\project001_data\DeSide_example\04predict_and_compare\DeSide_result',
-    #                        'EPIC': r'D:\project001_data\DeSide_example\04predict_and_compare\EPIC_result-sig-top-30',
-    #                        'Scaden': r'D:\project001_data\DeSide_example\04predict_and_compare\Scaden_result',
-    #                        'MuSiC': r'D:\project001_data\DeSide_example\04predict_and_compare\MuSiC_result'}
-    # algo2cell_types = {'CIBERSORT': ['CD8 T', 'Cancer Cells'],
-    #                    'DeSide': ['CD8 T', 'Cancer Cells', '1-others'],
-    #                    'EPIC': ['CD8 T', 'Cancer Cells', 'otherCells'],
-    #                    'Scaden': ['CD8 T', 'Cancer Cells'],
-    #                    'MuSiC': ['CD8 T', 'Cancer Cells']}
-    # for algo, m_fp in algo2merged_file_path.items():
-    #     print(f'Merge the results of {algo}...')
-    #     read_and_merge_result(raw_result_dir=algo2raw_result_dir[algo], algo=algo,
-    #                           cell_type=algo2cell_types[algo])
+import os
+import warnings
+import pandas as pd
+from scipy.stats import percentileofscore
+from .pub_func import check_dir, read_marker_gene, read_df, sorted_cell_types
+from ..utility import log_exp2cpm, non_log2cpm, aggregate_marker_gene_exp
+
+name_mapping_CIBERSORT = {"B cells": 'B Cells', "T cells CD8": 'CD8 T', "T cells CD4": 'CD4 T',
+                          "Macrophages": 'Macrophages', "Dendritic cells": 'DC',
+                          "Mast cells": 'Mast Cells', "Myocytes": 'myocyte', "CAFs": 'Fibroblasts',
+                          "Endothelial cells": 'Endothelial cells', "Malignant cells": 'Cancer Cells'}
+
+
+def parse_result_from_cibersort(result_file_path):
+    """
+
+    :param result_file_path:
+    :return:
+    """
+    name_mapping_reverse = {}
+    for i, j in name_mapping_CIBERSORT.items():
+        if j not in name_mapping_reverse:
+            name_mapping_reverse[j] = []
+        name_mapping_reverse[j].append(i)
+    result_from_cibersort = pd.read_csv(result_file_path, index_col=0)
+    result = pd.DataFrame(index=result_from_cibersort.index, columns=list(name_mapping_reverse.keys()))
+    for col in result.columns:
+        result[col] = result_from_cibersort.loc[:, name_mapping_reverse[col]].sum(axis=1)
+    cell_types = [i for i in sorted_cell_types if i in result.columns]
+    return result.loc[:, cell_types]
+
+
+def _read_result(file_path, cell_type_name_mapping, cell_types, algo=None):
+    """
+    read a single result file from different algorithms for performance comparison ()
+    :param file_path:
+    :param cell_type_name_mapping: mapping from cell type names of current algo to cell type names in DeSide
+    :param algo: the name of each algorithm, CIBERSORT, MuSiC, EPIC, Scaden, Scaden-web and DeSide
+    :return:
+    """
+    predicted_result = read_df(file_path)
+    predicted_result.rename(columns=cell_type_name_mapping, inplace=True)
+    predicted_result.index = predicted_result.index.map(lambda x: x.replace('.', '-'))
+    return predicted_result.loc[:, cell_types]
+
+
+def read_and_merge_result(raw_result_dir: str, cell_type_name_mapping: dict, algo: str,
+                          result_file_path=None, tcga_sample2cancer_type_file_path=None) -> pd.DataFrame:
+    """
+    read and merge predicted cell fractions of each algorithm
+    :param raw_result_dir:
+    :param cell_type_name_mapping: mapping from cell type names of current algo to cell type names in DeSide
+    :param algo: EPIC, CIBERSORT, MuSiC, DeSide and Scaden
+    :param result_file_path:
+    :param tcga_sample2cancer_type_file_path: the file path of sample id to cancer type mapping file in TCGA
+    :return:
+    """
+    cell_types = [i for i in sorted_cell_types if i in list(cell_type_name_mapping.values())]
+    cancer_dataset2file_path = {}
+    cancer_type = ''
+    ds = ''  # reference dataset
+    assert os.path.exists(raw_result_dir), '{} does not exist'.format(raw_result_dir)
+    for root, dirs, files in os.walk(raw_result_dir):
+        for file_name in files:
+            if (('.txt' in file_name) or (f'.csv' in file_name)) and \
+                    ('cancer_purity' not in file_name) and ('signature_score' not in file_name):
+                if 'CIBERSORT' in algo:
+                    _, _, _, cancer_type, ds, _ = file_name.split('_')
+                elif algo == 'MuSiC':
+                    cancer_type, ds, _ = file_name.split('_')
+                    ds = ds.replace('LUAD1', 'LUAD')
+                elif 'EPIC' in algo:
+                    if 'NOref' in file_name:
+                        _, cancer_type, ds = file_name.split('_')
+                    else:
+                        cancer_type, _ = file_name.split('.')
+                    if algo == 'EPIC':
+                        ds = '46sig'
+                    else:  # EPIC_self_ref
+                        ds = 'self'
+                elif algo == 'Scaden_ascites':
+                    cancer_type = file_name.split('_')[-1].replace('.txt', '')
+                    ds = 'Ascites'
+                elif algo == 'Scaden_simu_bulk':
+                    cancer_type = file_name.split('_')[-1].replace('.txt', '')
+                    ds = 'simu_bulk_2ds'
+                elif 'DeSide' in algo:
+                    cancer_type = root.split(os.path.sep)[-1]
+                    if '/' in cancer_type:
+                        cancer_type = cancer_type.split('/')[-1]
+                    ds = 'simu_bulk_2ds'
+                    if algo == 'DeSide_softmax':
+                        ds = 'simu_bulk_2ds_softmax'
+                elif algo == 'Kassandra_self':
+                    cancer_type = 'all'
+                    ds = 'self'
+                if '.txt' in ds:
+                    ds = ds.replace('.txt', '')
+                cancer_type = cancer_type.replace('HNSCC', 'HNSC')
+                ds = ds.replace('HNSCC', 'HNSC')
+                assert os.path.exists(os.path.join(root, file_name)), f'{os.path.join(root, file_name)} does not exist'
+                cancer_dataset2file_path[cancer_type + '-' + ds + '_ref'] = os.path.join(root, file_name)
+    # print(cancer_dataset2file_path)
+    sample2cell_frac = {}
+    counter = 0
+    columns = ['sample_id', 'cancer_type', 'reference_dataset'] + cell_types
+
+    for cancer_dataset, file_path in cancer_dataset2file_path.items():
+        # print(cancer_dataset, file_path)
+        cancer_type, ref_dataset = cancer_dataset.split('-')
+        if 'Scaden' in algo:
+            ref_dataset = ref_dataset.replace('Scaden_', '')
+        elif algo == 'DeSide':
+            ref_dataset = ref_dataset.replace('DeSide_', '')
+        if ref_dataset == 'ref':
+            ref_dataset = 'Mixed_ref'
+        current_result = _read_result(file_path, cell_type_name_mapping=cell_type_name_mapping,
+                                      cell_types=cell_types, algo=algo)
+        if algo == 'Kassandra_self':
+            current_result = current_result / 100
+        for row in current_result.iterrows():
+            sample_id = row[0]
+            sample2cell_frac[counter] = [sample_id, cancer_type, ref_dataset] + list(row[1].values)
+            counter += 1
+    merged_result = pd.DataFrame.from_dict(sample2cell_frac, orient='index', columns=columns)
+    if algo == 'Kassandra_self':
+        tcga_sample2cancer_type = pd.read_csv(tcga_sample2cancer_type_file_path, index_col=0)
+        tcga_sample2cancer_type.index = tcga_sample2cancer_type.index.map(lambda x: x.replace('.', '-'))
+        tcga_sample2cancer_type = tcga_sample2cancer_type.to_dict()['cancer_type']
+        merged_result.drop(columns=['cancer_type'], inplace=True)
+        merged_result['cancer_type'] = merged_result['sample_id'].map(lambda x: tcga_sample2cancer_type[x])
+        merged_result = merged_result.loc[:, columns].copy()
+    if result_file_path:
+        if os.path.exists(result_file_path):
+            merged_result.to_csv(result_file_path, mode='a', header=False, float_format='%.3f')
+        else:
+            merged_result.to_csv(result_file_path, float_format='%.3f')
+    else:
+        return merged_result
+
+
+def mean_exp_of_marker_gene(marker_gene_file_path, bulk_tpm_file_path, result_file_path: str = None,
+                            cancer_type: str = None, debug=False, trans=False, cell_types: list = None,
+                            log_exp: bool = False, gene_list_in_model: list = None):
+    """
+    mean expression value of marker genes for each cell type (max expression value for B Cells and CD4 T Cells)
+    :param marker_gene_file_path: file path of selected marker gene for each cell type
+    :param bulk_tpm_file_path: file path of bulk cell TPM, should be gene by sample
+    :param result_file_path
+    :param cancer_type: tumor type / cancer type / test set name
+    :param debug: if output intermediate result for debug
+    :param trans: taking transposition if the bulk cell TPM is organized with sample by gene
+    :param cell_types: cell types
+    :param log_exp: TPM is need. If the expression values are log transformed, it should be transformed to TPM
+    :param gene_list_in_model: filtering bulk_tpm and rescaling to TPM if not None
+    :return: a dataframe, sample by cell type (mean expression of marker genes), and save to file
+    """
+    if result_file_path is not None:
+        result_dir = os.path.dirname(result_file_path)
+        check_dir(result_dir)
+    else:
+        result_dir = '.'
+    temporal_dir = os.path.join(result_dir, 'debug_temp', cancer_type)
+    if debug:
+        check_dir(temporal_dir)
+    include_t_cell = False
+    if (cell_types is not None) and ('T Cells' in cell_types):
+        include_t_cell = True
+        cell_types += ['CD8 T', 'CD4 T']
+    cell_type2marker = read_marker_gene(marker_gene_file_path, include_t_cell=include_t_cell,
+                                        use_cancer_cell=True, corr_mean=True)
+    cell_type2marker = {k: v for k, v in cell_type2marker.items() if k in cell_types}
+    # if ('Cancer Cells' not in cell_type2marker) and ('Epithelial Cells' in cell_type2marker):
+    #     cell_type2marker['Cancer Cells'] = cell_type2marker['Epithelial Cells']
+    # sep = get_sep(bulk_tpm_file_path)
+    # tpm = pd.read_csv(bulk_tpm_file_path, index_col=0, sep=sep)
+    tpm = read_df(bulk_tpm_file_path)
+    if trans:
+        tpm = tpm.T
+    if log_exp:
+        tpm = log_exp2cpm(tpm)
+    if gene_list_in_model is not None:
+        intersection_genes = [i for i in gene_list_in_model if i in tpm.index]
+        if len(intersection_genes) != len(gene_list_in_model):
+            n_diff = len(gene_list_in_model) - len(intersection_genes)
+            warnings.warn(f'There are {n_diff} genes don\'t include in current bulk TPM dataset')
+        tpm = tpm.loc[tpm.index.isin(intersection_genes), :].copy()
+        tpm = non_log2cpm(tpm.T).T  # rescaling to TPM after filtering by gene list in model
+        # print(tpm.sum(axis=0))
+
+    marker_exp = aggregate_marker_gene_exp(exp_df=tpm.T, marker_genes=cell_type2marker)
+    return marker_exp
+
+
+def cal_gene_signature_score(marker_gene_file_path, bulk_tpm_file_path, result_file_path: str = None,
+                             cancer_type: str = None, trans=False, cell_types: list = None):
+    """
+    gene signature score for each cell type,
+      ref to Combes et al., 2022, Cell185, 184–203 (METHOD DETAILS, Gene Signature Score)
+    :param marker_gene_file_path: file path of selected marker gene for each cell type
+    :param bulk_tpm_file_path: file path of bulk cell TPM, should be gene by sample
+    :param result_file_path
+    :param cancer_type: tumor type / cancer type / test set name
+    :param trans: taking transposition if the bulk cell TPM is organized with sample by gene
+    :param cell_types: cell types
+    :return: a dataframe, sample by cell type (gene signature score for each cell type of each sample),
+      and save to file
+    """
+
+    include_t_cell = False
+    if (cell_types is not None) and ('T Cells' in cell_types):
+        include_t_cell = True
+        cell_types += ['CD8 T', 'CD4 T']
+    cell_type2marker = read_marker_gene(marker_gene_file_path, include_t_cell=include_t_cell,
+                                        use_cancer_cell=True)
+    # sep = get_sep(bulk_tpm_file_path)
+    # tpm = pd.read_csv(bulk_tpm_file_path, index_col=0, sep=sep)
+    tpm = read_df(bulk_tpm_file_path)
+    if trans:
+        tpm = tpm.T
+
+    cell_type2signature_score = {}
+    if cell_types is None:
+        cell_types = list(cell_type2marker.keys())
+    for ct in cell_types:
+        marker = cell_type2marker[ct]
+        current_tpm = tpm.loc[tpm.index.isin(marker), :]  # gene by sample, E, m x n matrix of gene expression
+        current_valid_marker = current_tpm.index.to_list()
+        if len(current_valid_marker) > 0:
+            current_marker_str = ', '.join(current_valid_marker)
+            print(f'   Using {len(current_valid_marker)} marker genes for cell type {ct}: {current_marker_str}')
+            # cell_type2mean_exp[ct + '_marker_mean'] = current_tpm.mean(axis=0)
+            p = pd.DataFrame(index=current_tpm.index, columns=current_tpm.columns)
+            for inx, _row in current_tpm.iterrows():
+                p.loc[inx] = [percentileofscore(_row, g_exp) for g_exp in _row]
+            p = p.mean(axis=0)
+            cell_type2signature_score[ct + f'_gene_signature_score'] = \
+                pd.Series(data=[percentileofscore(p, _) for _ in p], index=p.index)
+        else:
+            Warning(f'No any marker genes in bulk cell TPM for cell type {ct}, '
+                    f'this cell type will be ignored in later analysis.')
+    signature_score = pd.DataFrame.from_dict(cell_type2signature_score, orient='columns')
+    if cancer_type is not None:
+        signature_score['cancer_type'] = cancer_type
+    if result_file_path is not None:
+        signature_score.to_csv(result_file_path, float_format='%.3f')
+    return signature_score.round(3)
+
+
+if __name__ == '__main__':
+    pass
+    # algo2merged_file_path = {
+    #     # 'CIBERSORT': './merged_result/CIBERSORT_predicted_cell_fraction.csv',
+    #                          'DeSide': './merged_result/DeSide_predicted_cell_fraction.csv',
+    #                          # 'EPIC': './merged_result/EPIC_predicted_cell_fraction.csv',
+    #                          # 'Scaden': './merged_result/Scaden_predicted_cell_fraction.csv',
+    #                          # 'MuSiC': './merged_result/MuSiC_predicted_cell_fraction.csv'
+    # }
+    # algo2raw_result_dir = {'CIBERSORT': r'D:\project001_data\DeSide_example\04predict_and_compare\CIBERSORT_result',
+    #                        'DeSide': r'D:\project001_data\DeSide_example\04predict_and_compare\DeSide_result',
+    #                        'EPIC': r'D:\project001_data\DeSide_example\04predict_and_compare\EPIC_result-sig-top-30',
+    #                        'Scaden': r'D:\project001_data\DeSide_example\04predict_and_compare\Scaden_result',
+    #                        'MuSiC': r'D:\project001_data\DeSide_example\04predict_and_compare\MuSiC_result'}
+    # algo2cell_types = {'CIBERSORT': ['CD8 T', 'Cancer Cells'],
+    #                    'DeSide': ['CD8 T', 'Cancer Cells', '1-others'],
+    #                    'EPIC': ['CD8 T', 'Cancer Cells', 'otherCells'],
+    #                    'Scaden': ['CD8 T', 'Cancer Cells'],
+    #                    'MuSiC': ['CD8 T', 'Cancer Cells']}
+    # for algo, m_fp in algo2merged_file_path.items():
+    #     print(f'Merge the results of {algo}...')
+    #     read_and_merge_result(raw_result_dir=algo2raw_result_dir[algo], algo=algo,
+    #                           cell_type=algo2cell_types[algo])
```

### Comparing `DeSide-1.0.1/deside/utility/core_obj.py` & `DeSide-1.0.2/deside/utility/core_obj.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import numpy as np
-import pandas as pd
-from typing import Union
-from .read_file import ReadExp
-from sklearn.neighbors import NearestNeighbors
-from .pub_func import default_core_marker_genes, aggregate_marker_gene_exp, read_df
-
-
-class ExpObj(ReadExp):
-    """
-    An object to save gene expression profiles
-    """
-    def __init__(self, exp_file, exp_type: str, transpose: bool = False):
-        super().__init__(exp_file, exp_type=exp_type, transpose=transpose)
-        self.marker_ratio = None
-
-    def cal_marker_gene_ratio(self, cell_types: list, marker_genes: dict = None,
-                              agg_methods: dict = None, show_marker_gene: bool = False):
-        if marker_genes is None:
-            marker_genes = {k: v for k, v in default_core_marker_genes.items() if k in cell_types}
-
-        self.marker_ratio = aggregate_marker_gene_exp(exp_df=self.exp, marker_genes=marker_genes,
-                                                      return_ratio=True,
-                                                      agg_methods=agg_methods,
-                                                      show_marker_gene=show_marker_gene)
-
-    def get_marker_ratios(self):
-        if self.marker_ratio is not None:
-            return self.marker_ratio
-        else:
-            raise ValueError('"marker_ratio" is None, please calculate marker ratios first '
-                             'by calling function "cal_marker_gene_ratio".')
-
-
-class QueryNeighbors(object):
-    def __init__(self, df_file: Union[str, pd.DataFrame]):
-        """
-        :param df_file: a file path or DataFrame of marker ratios for cell types, samples by cell types
-        """
-        self.df = read_df(df_file)
-
-    def fit_nn_model(self, n_neighbors: int = 2, radius: float = None):
-        """
-        fit a NearestNeighbors model
-        - if radius is None, fit a model with specific n_neighbors
-        - if radius is not None, fit a model with specific radius
-        """
-        if radius is not None:
-            nn_model = NearestNeighbors(radius=radius)
-        else:
-            nn_model = NearestNeighbors(n_neighbors=n_neighbors, algorithm='ball_tree')
-        nn_model.fit(self.df.values)
-        return nn_model
-
-    def get_nn(self, q_df_file: Union[str, pd.DataFrame] = None, n_neighbors: int = 1) -> pd.DataFrame:
-        """
-        query nearest neighbors (NN) from the NN model which is fitted on self.df
-        :param q_df_file: query NN for all samples in this dataset
-        - if None: query the distance of nearest neighbor for all samples in the same df, self.df
-        :param n_neighbors: the number of nearest neighbors to query
-        :return: the nearest neighbor and corresponding distance ['nn', 'nn_dis']
-        """
-        assert n_neighbors >= 1, 'n_neighbors should >= 1'
-        nn_model = self.fit_nn_model(n_neighbors=n_neighbors + 1)
-        if q_df_file is not None:
-            q_df = read_df(q_df_file)
-            nn_index = 0  # 0 is queried NN from fitted nn_model
-        else:
-            q_df = self.df.copy()
-            nn_index = 1  # 0 is itself
-        assert np.all(self.df.columns == q_df.columns), 'self.df and q_df should have the same columns with same order'
-        dis, indices = nn_model.kneighbors(q_df.values)
-        # the distance of nearest neighbor for each sample of q_df
-        result = pd.DataFrame(index=q_df.index)
-        if n_neighbors == 1:
-            result['nn'] = self.df.iloc[indices[:, nn_index], 0].index.to_list()  # the index or sample_name of NN
-            result['nn_dis'] = dis[:, nn_index]
-        else:  # > 1
-            nn_cols = [f'nn_{i}' for i in range(n_neighbors)]
-            nn_dis_cols = [f'nn_dis_{i}' for i in range(n_neighbors)]
-            for j in range(n_neighbors):
-                result[nn_cols[j]] = self.df.iloc[indices[:, nn_index + j], 0].index.to_list()
-                result[nn_dis_cols[j]] = np.round(dis[:, nn_index + j], 3)
-        result.index.name = 'query_sample_id'
-        return result
-
-    def get_neighbors_by_radius(self, radius: float, q_df_file: Union[str, pd.DataFrame] = None,
-                                share_neighbors: bool = False, n_top: int = None) -> pd.DataFrame:
-        """
-        query neighbors by a specific radius
-        :param radius: only find neighbors within this radius
-        :param q_df_file: query NN for all samples in this dataset
-        :param share_neighbors: if share neighbors between different query samples
-        - False: duplicated neighbors will be removed among different query samples
-        - True: duplicated neighbors will be kept
-        :param n_top: if too many neighbors were founded for one single sample, only keep n_top neighbors
-        return: the nearest neighbors within the fixed radius and corresponding distance ['nn', 'nn_dis']
-        """
-        nn_model = self.fit_nn_model(radius=radius)
-        if q_df_file is not None:
-            q_df = read_df(q_df_file)
-        else:
-            q_df = self.df.copy()  # query in the same dataset, self.df
-
-        t2s_neighbors = []
-        inx_collector = {}
-        inx2sample_id_df = {i: sample_id for i, sample_id in enumerate(self.df.index.to_list())}
-        for q_inx in q_df.index:
-            query_ratio = q_df.loc[[q_inx], :]
-            dis, res_index = nn_model.radius_neighbors(query_ratio)
-            res_inx2dis = dict(zip(res_index[0], dis[0]))
-            if res_inx2dis:
-                res_inx2dis = {k: v for k, v in res_inx2dis.items()}
-                res_inx2dis = sorted(res_inx2dis.items(), key=lambda x: x[1])  # a list here
-                if not share_neighbors:
-                    res_inx2dis = [_ for _ in res_inx2dis if _[0] not in inx_collector]
-                if (n_top is not None) and len(res_inx2dis) > n_top:
-                    res_inx2dis = res_inx2dis[:n_top]
-                current_neighbors_df = pd.DataFrame.from_dict(dict(
-                    [(inx2sample_id_df[inx], dis) for inx, dis in res_inx2dis],
-                ), orient='index', columns=['nn_dis'])
-                current_neighbors_df['query_sample_id'] = q_inx
-                t2s_neighbors.append(current_neighbors_df)
-                for each_item in res_inx2dis:
-                    inx_collector[each_item[0]] = 1
-        if t2s_neighbors:
-            results = pd.concat(t2s_neighbors)
-            results.index.name = 'nn'
-            results.reset_index(inplace=True)
-            results.set_index('query_sample_id', inplace=True)
-        else:
-            results = pd.DataFrame()
-        return results
-
-    def get_quantile_of_nn_distance(self, quantile: float, q_df_file: Union[str, pd.DataFrame] = None):
-        """
-        get the quantile of NN distance
-        """
-        nn_distance = self.get_nn(q_df_file=q_df_file)
-        q_dis = np.quantile(nn_distance['nn_dis'], quantile)
-        # print(f'   {quantile} quantile distance is: {q_dis}')
-        return q_dis
+import numpy as np
+import pandas as pd
+from typing import Union
+from .read_file import ReadExp
+from sklearn.neighbors import NearestNeighbors
+from .pub_func import default_core_marker_genes, aggregate_marker_gene_exp, read_df
+
+
+class ExpObj(ReadExp):
+    """
+    An object to save gene expression profiles
+    """
+    def __init__(self, exp_file, exp_type: str, transpose: bool = False):
+        super().__init__(exp_file, exp_type=exp_type, transpose=transpose)
+        self.marker_ratio = None
+
+    def cal_marker_gene_ratio(self, cell_types: list, marker_genes: dict = None,
+                              agg_methods: dict = None, show_marker_gene: bool = False):
+        if marker_genes is None:
+            marker_genes = {k: v for k, v in default_core_marker_genes.items() if k in cell_types}
+
+        self.marker_ratio = aggregate_marker_gene_exp(exp_df=self.exp, marker_genes=marker_genes,
+                                                      return_ratio=True,
+                                                      agg_methods=agg_methods,
+                                                      show_marker_gene=show_marker_gene)
+
+    def get_marker_ratios(self):
+        if self.marker_ratio is not None:
+            return self.marker_ratio
+        else:
+            raise ValueError('"marker_ratio" is None, please calculate marker ratios first '
+                             'by calling function "cal_marker_gene_ratio".')
+
+
+class QueryNeighbors(object):
+    def __init__(self, df_file: Union[str, pd.DataFrame]):
+        """
+        :param df_file: a file path or DataFrame of marker ratios for cell types, samples by cell types
+        """
+        self.df = read_df(df_file)
+
+    def fit_nn_model(self, n_neighbors: int = 2, radius: float = None):
+        """
+        fit a NearestNeighbors model
+        - if radius is None, fit a model with specific n_neighbors
+        - if radius is not None, fit a model with specific radius
+        """
+        if radius is not None:
+            nn_model = NearestNeighbors(radius=radius)
+        else:
+            nn_model = NearestNeighbors(n_neighbors=n_neighbors, algorithm='ball_tree')
+        nn_model.fit(self.df.values)
+        return nn_model
+
+    def get_nn(self, q_df_file: Union[str, pd.DataFrame] = None, n_neighbors: int = 1) -> pd.DataFrame:
+        """
+        query nearest neighbors (NN) from the NN model which is fitted on self.df
+        :param q_df_file: query NN for all samples in this dataset
+        - if None: query the distance of nearest neighbor for all samples in the same df, self.df
+        :param n_neighbors: the number of nearest neighbors to query
+        :return: the nearest neighbor and corresponding distance ['nn', 'nn_dis']
+        """
+        assert n_neighbors >= 1, 'n_neighbors should >= 1'
+        nn_model = self.fit_nn_model(n_neighbors=n_neighbors + 1)
+        if q_df_file is not None:
+            q_df = read_df(q_df_file)
+            nn_index = 0  # 0 is queried NN from fitted nn_model
+        else:
+            q_df = self.df.copy()
+            nn_index = 1  # 0 is itself
+        assert np.all(self.df.columns == q_df.columns), 'self.df and q_df should have the same columns with same order'
+        dis, indices = nn_model.kneighbors(q_df.values)
+        # the distance of nearest neighbor for each sample of q_df
+        result = pd.DataFrame(index=q_df.index)
+        if n_neighbors == 1:
+            result['nn'] = self.df.iloc[indices[:, nn_index], 0].index.to_list()  # the index or sample_name of NN
+            result['nn_dis'] = dis[:, nn_index]
+        else:  # > 1
+            nn_cols = [f'nn_{i}' for i in range(n_neighbors)]
+            nn_dis_cols = [f'nn_dis_{i}' for i in range(n_neighbors)]
+            for j in range(n_neighbors):
+                result[nn_cols[j]] = self.df.iloc[indices[:, nn_index + j], 0].index.to_list()
+                result[nn_dis_cols[j]] = np.round(dis[:, nn_index + j], 3)
+        result.index.name = 'query_sample_id'
+        return result
+
+    def get_neighbors_by_radius(self, radius: float, q_df_file: Union[str, pd.DataFrame] = None,
+                                share_neighbors: bool = False, n_top: int = None) -> pd.DataFrame:
+        """
+        query neighbors by a specific radius
+        :param radius: only find neighbors within this radius
+        :param q_df_file: query NN for all samples in this dataset
+        :param share_neighbors: if share neighbors between different query samples
+        - False: duplicated neighbors will be removed among different query samples
+        - True: duplicated neighbors will be kept
+        :param n_top: if too many neighbors were founded for one single sample, only keep n_top neighbors
+        return: the nearest neighbors within the fixed radius and corresponding distance ['nn', 'nn_dis']
+        """
+        nn_model = self.fit_nn_model(radius=radius)
+        if q_df_file is not None:
+            q_df = read_df(q_df_file)
+        else:
+            q_df = self.df.copy()  # query in the same dataset, self.df
+
+        t2s_neighbors = []
+        inx_collector = {}
+        inx2sample_id_df = {i: sample_id for i, sample_id in enumerate(self.df.index.to_list())}
+        for q_inx in q_df.index:
+            query_ratio = q_df.loc[[q_inx], :]
+            dis, res_index = nn_model.radius_neighbors(query_ratio)
+            res_inx2dis = dict(zip(res_index[0], dis[0]))
+            if res_inx2dis:
+                res_inx2dis = {k: v for k, v in res_inx2dis.items()}
+                res_inx2dis = sorted(res_inx2dis.items(), key=lambda x: x[1])  # a list here
+                if not share_neighbors:
+                    res_inx2dis = [_ for _ in res_inx2dis if _[0] not in inx_collector]
+                if (n_top is not None) and len(res_inx2dis) > n_top:
+                    res_inx2dis = res_inx2dis[:n_top]
+                current_neighbors_df = pd.DataFrame.from_dict(dict(
+                    [(inx2sample_id_df[inx], dis) for inx, dis in res_inx2dis],
+                ), orient='index', columns=['nn_dis'])
+                current_neighbors_df['query_sample_id'] = q_inx
+                t2s_neighbors.append(current_neighbors_df)
+                for each_item in res_inx2dis:
+                    inx_collector[each_item[0]] = 1
+        if t2s_neighbors:
+            results = pd.concat(t2s_neighbors)
+            results.index.name = 'nn'
+            results.reset_index(inplace=True)
+            results.set_index('query_sample_id', inplace=True)
+        else:
+            results = pd.DataFrame()
+        return results
+
+    def get_quantile_of_nn_distance(self, quantile: float, q_df_file: Union[str, pd.DataFrame] = None):
+        """
+        get the quantile of NN distance
+        """
+        nn_distance = self.get_nn(q_df_file=q_df_file)
+        q_dis = np.quantile(nn_distance['nn_dis'], quantile)
+        # print(f'   {quantile} quantile distance is: {q_dis}')
+        return q_dis
```

### Comparing `DeSide-1.0.1/deside/utility/evaluation.py` & `DeSide-1.0.2/deside/utility/evaluation.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import numpy as np
-import pandas as pd
-
-
-def get_core_zone_of_pca(pca_data: pd.DataFrame, col_x, col_y, q_lower, q_upper):
-    """
-    get core zone of TCGA in PCA plot
-    :param pca_data: PCA data
-    :param col_x: x axis column name
-    :param col_y: y axis column name
-    :param q_lower: lower quantile
-    :param q_upper: upper quantile
-    :return: coordinate_core_zone, n_tcga_in_core_zone, n_non_tcga_in_core_zone
-    """
-    assert 'TCGA' in pca_data['class'].unique()
-    x_tcga = pca_data.loc[pca_data['class'] == 'TCGA', col_x]
-    y_tcga = pca_data.loc[pca_data['class'] == 'TCGA', col_y]
-    x_q_lower = np.quantile(x_tcga, q_lower)
-    x_q_upper = np.quantile(x_tcga, q_upper)
-    y_q_lower = np.quantile(y_tcga, q_lower)
-    y_q_upper = np.quantile(y_tcga, q_upper)
-    core_zone = pca_data.loc[(pca_data[col_x] >= x_q_lower) & (pca_data[col_x] <= x_q_upper) &
-                             (pca_data[col_y] >= y_q_lower) & (pca_data[col_y] <= y_q_upper), :]
-    coordinate_core_zone = {'x_lower': x_q_lower, 'x_upper': x_q_upper, 'y_lower': y_q_lower, 'y_upper': y_q_upper}
-    n_tcga_in_core_zone = core_zone.loc[core_zone['class'] == 'TCGA', :].shape[0]
-    n_non_tcga_in_core_zone = core_zone.loc[core_zone['class'] != 'TCGA', :].shape[0]
-    return coordinate_core_zone, n_tcga_in_core_zone, n_non_tcga_in_core_zone
+import numpy as np
+import pandas as pd
+
+
+def get_core_zone_of_pca(pca_data: pd.DataFrame, col_x, col_y, q_lower, q_upper):
+    """
+    get core zone of TCGA in PCA plot
+    :param pca_data: PCA data
+    :param col_x: x axis column name
+    :param col_y: y axis column name
+    :param q_lower: lower quantile
+    :param q_upper: upper quantile
+    :return: coordinate_core_zone, n_tcga_in_core_zone, n_non_tcga_in_core_zone
+    """
+    assert 'TCGA' in pca_data['class'].unique()
+    x_tcga = pca_data.loc[pca_data['class'] == 'TCGA', col_x]
+    y_tcga = pca_data.loc[pca_data['class'] == 'TCGA', col_y]
+    x_q_lower = np.quantile(x_tcga, q_lower)
+    x_q_upper = np.quantile(x_tcga, q_upper)
+    y_q_lower = np.quantile(y_tcga, q_lower)
+    y_q_upper = np.quantile(y_tcga, q_upper)
+    core_zone = pca_data.loc[(pca_data[col_x] >= x_q_lower) & (pca_data[col_x] <= x_q_upper) &
+                             (pca_data[col_y] >= y_q_lower) & (pca_data[col_y] <= y_q_upper), :]
+    coordinate_core_zone = {'x_lower': x_q_lower, 'x_upper': x_q_upper, 'y_lower': y_q_lower, 'y_upper': y_q_upper}
+    n_tcga_in_core_zone = core_zone.loc[core_zone['class'] == 'TCGA', :].shape[0]
+    n_non_tcga_in_core_zone = core_zone.loc[core_zone['class'] != 'TCGA', :].shape[0]
+    return coordinate_core_zone, n_tcga_in_core_zone, n_non_tcga_in_core_zone
```

### Comparing `DeSide-1.0.1/deside/utility/pub_func.py` & `DeSide-1.0.2/deside/utility/pub_func.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,908 +1,908 @@
-import os
-import csv
-import json
-import time
-import umap
-from typing import Union
-import numpy as np
-import pandas as pd
-# import anndata as an
-import seaborn as sns
-import matplotlib as mpl
-from pathlib import Path
-import scipy.stats as stats
-from joblib import dump, load
-import matplotlib.pyplot as plt
-from scipy.sparse import csr_matrix
-from sklearn.decomposition import PCA
-from anndata import AnnData, read_h5ad
-from sklearn.metrics import mean_squared_error, r2_score
-import gzip
-import shutil
-
-
-default_core_marker_genes = {'Cancer Cells': ['KRT19', 'KRT18', 'KRT8', 'EPCAM'],
-                             'CD4 T': ['BATF', 'ICOS', 'CD4', 'IL7R', 'FOXP3', 'TIGIT'],
-                             'CD8 T': ['CD8A', 'CD8B'],
-                             'T Cells': ['CD2', 'CD3D', 'CD3E'],
-                             'B Cells': ['BANK1', 'CD79A', 'FCRL5', 'MS4A1'],
-                             'DC': ['GZMB', 'CCR7', 'LAMP3', 'IRF7', 'IRF8'],
-                             'Endothelial Cells': ['CLDN5', 'ENG', 'PLVAP', 'VWF'],
-                             'Fibroblasts': ['COL1A1', 'COL1A2', 'COL3A1', 'MYL9'],
-                             'Macrophages': ['AIF1', 'CD14', 'CD68', 'MS4A7'],
-                             'Mast Cells': ['CPA3', 'HPGDS', 'GATA2'],
-                             'NK': ['GNLY', 'NKG7', 'KLRD1'],
-                             'Neutrophils': ['CSF3R', 'CXCR2', 'FPR1', 'SLC25A37']}
-
-
-sorted_cell_types = ['B Cells', 'CD4 T', 'CD8 T', 'Cancer Cells', 'DC', 'Endothelial Cells',
-                     'Fibroblasts', 'Macrophages', 'Mast Cells', 'NK', 'Neutrophils']
-
-
-def get_inx2cell_type() -> dict:
-    inx2cell_type = {_i: ct for _i, ct in enumerate(sorted_cell_types)}
-    inx2cell_type[-1] = 'Neg'
-    return inx2cell_type
-
-
-def print_df(df):
-    assert type(df) == pd.DataFrame
-    print('  >>  <<  ')
-    print(df.shape)
-    print(df.head(2))
-
-
-def set_fig_style(font_family=None, font_size=None):
-    fig, ax = plt.subplots()
-    sns.set_style("white")
-    try:
-        plt.style.use(['science', 'no-latex'])
-    except:
-        print('No science style')
-        sns.set(palette='muted', font_scale=1.5)
-
-    mpl.rcParams['figure.dpi'] = 300
-    mpl.rcParams['figure.facecolor'] = 'white'
-    mpl.rcParams['pdf.fonttype'] = 42
-    mpl.rcParams['ps.fonttype'] = 42
-    plt.rcParams['svg.fonttype'] = 'none'
-    if font_family:
-        mpl.rcParams['font.family'] = font_family
-    if font_size:
-        mpl.rcParams['font.size'] = font_size
-    # print('figure.dpi will be set to', mpl.rcParams['figure.dpi'])
-    plt.close('all')
-
-
-def filter_gene_by_expression_log_mean(exp_df, min_exp_value=3, max_exp_value=10, min_exp_percent=0.8):
-    """
-    Ea(i)=log2(ave(TPM(i)1..k)+1), excluded genes with Ea<threshold
-
-    "As genes with high expression can bias deconvolution results,
-     we excluded the genes whose expression exceeded 700 TPM",
-     Finotello, F. et al., Genome Med 11, 34 (2019). https://doi.org/10.1186/s13073-019-0638-6
-
-    :param exp_df: expression values of each gene, non-log2 values, a dataframe
-    :param min_exp_value: minimum log2 mean expression value of each gene across all samples
-    :param max_exp_value: max log2 mean expression value of each gene across all samples
-    :param min_exp_percent: minimum expression percentage of each gene in all samples
-    :return: filtered genes in each sample
-    """
-    # assert type(exp_df) == pd.
-    n_gene = exp_df.shape[0]
-    n_sample = exp_df.shape[1]
-    print('>>> Total gene: {}'.format(n_gene))
-    log_mean_exp = np.log2(exp_df.mean(axis=1) + 1)
-    above_min_exp_inx = log_mean_exp >= min_exp_value
-    below_max_exp_inx = log_mean_exp <= max_exp_value
-    exp_filtered_by_min_exp = exp_df.loc[above_min_exp_inx & below_max_exp_inx, :]
-    print('>>> Number of gene below min_exp_value: {}'.format(n_gene - sum(above_min_exp_inx)))
-    print('>>> Number of gene above max_exp_value: {}'.format(n_gene - sum(below_max_exp_inx)))
-    # remove genes that does not express in high percentage samples
-    keep_inx = (np.sum(exp_filtered_by_min_exp < min_exp_value, axis=1) / n_sample) < min_exp_percent
-    return exp_filtered_by_min_exp.loc[keep_inx, :].copy()
-
-
-def filter_gene_by_expression_min_max(exp_df, min_exp_value=3, max_exp_value=1000,
-                                      min_exp_percent=0.8, high_exp_min_percent=0.2,
-                                      min_num_sample=50):
-    """
-    exclude genes with E < min_exp_value among more than 20% (1-min_exp_percent) samples
-    exclude genes with E > max_exp_value among less than 20% (high_exp_min_percent) samples
-
-    "As genes with high expression can bias deconvolution results,
-     we excluded the genes whose expression exceeded 700 TPM",
-     Finotello, F. et al., Genome Med 11, 34 (2019). https://doi.org/10.1186/s13073-019-0638-6
-
-    :param exp_df: expression values of each gene, non-log2 values, a dataframe
-    :param min_exp_value: minimum expression value of each gene across all samples
-    :param max_exp_value: max expression value of each gene across all samples
-    :param min_exp_percent: float
-        the min expression value of each gene should >=min_exp_value in all samples higher than this percent,
-        otherwise will be exclude (treat as no expression in all samples), at least 0.8
-    :param high_exp_min_percent: float
-        the max expression value of each gene should >=max_exp_value in all samples higher than this percent,
-        otherwise will be exclude (treat as only having extremely high expression in a few samples)
-    :param min_num_sample: the minimum number of samples needs to fulfil above conditions instead of using percentage
-
-    :return: filtered genes in each sample
-    """
-    n_gene = exp_df.shape[0]
-    n_sample = exp_df.shape[1]
-    print('>>> Total gene: {}'.format(n_gene))
-    # log_mean_exp = np.log2(exp_df.mean(axis=1) + 1)
-    # no expression in the most of samples
-    if n_sample > min_num_sample / (1 - min_exp_percent):
-        min_exp_percent = 1 - min_num_sample / n_sample  # bigger min_exp_percent in big n_sample
-    nm_exp_inx = (np.sum(exp_df < min_exp_value, axis=1) / n_sample) > min_exp_percent
-    # exist extremely high expression in a few samples
-    if n_sample >= min_num_sample / high_exp_min_percent:
-        high_exp_min_percent = min_num_sample / n_sample
-    ehf_exp_inx = ((np.sum(exp_df > max_exp_value, axis=1) / n_sample) < high_exp_min_percent) & \
-                  ((np.sum(exp_df > max_exp_value, axis=1) / n_sample) > 0)
-
-    print('>>> Number of gene which no expression in the most of samples: {}'.format(sum(nm_exp_inx)))
-    print('>>> Number of gene which extremely high expression in a few samples: {}'.format(sum(ehf_exp_inx)))
-    return exp_df.loc[~(nm_exp_inx | ehf_exp_inx), :].copy()
-
-
-def filter_sample_by_expression(exp_df, max_mean_exp=100, plot_cdf=True, fig_file_path=""):
-    """
-    remove samples have high mean expression, usually contain some extremely high expressed genes
-    :param exp_df:
-    :param max_mean_exp:
-    :param plot_cdf: plot CDF of sample mean expression
-    :param fig_file_path: where to save cdf figure
-    """
-    sample_mean_exp = exp_df.mean()
-    n_sample = exp_df.shape[1]
-    if plot_cdf:
-        plt.figure(figsize=(8, 6))
-        plt.hist(sample_mean_exp, density=True, cumulative=True, histtype='step', color='k')
-        if fig_file_path:
-            plt.savefig(fig_file_path, dpi=200)
-        plt.show()
-    below_max_inx = sample_mean_exp <= max_mean_exp
-    print('>>> Number of sample above max_mean_exp: {}'.format(n_sample - sum(below_max_inx)))
-    return exp_df.loc[:, below_max_inx].copy()
-
-
-def log2_transform(df):
-    """
-    log2 transform expression values (plus 1)
-    :param df:
-    :return:
-    """
-    df = df.astype(np.float64)
-    df = np.log2(df + 1)
-    df = df.astype(np.float32)
-    return df
-
-
-def center_value(df, return_mean=False):
-    """
-    exp - mean(exp) for each genes
-    :param df: expression dataframe, gene x sample
-    :param return_mean: if return df_mean
-    :return:
-    """
-    df_mean = df.mean(axis=1)
-    if return_mean:
-        return df - np.vstack(df_mean), df_mean.to_frame('gene_mean')
-    return df - np.vstack(df_mean)
-
-
-def filter_gene_by_variance(exp_df, threshold=0.1):
-    """
-    remove genes which variation is < threshold
-    :param exp_df:
-    :param threshold:
-    :return:
-    """
-    n_gene_before_filter = exp_df.shape[0]
-    exp_var = exp_df.var(axis=1)
-    exp_df = exp_df.loc[exp_var >= threshold, :].copy()
-    n_gene_after_filter = exp_df.shape[0]
-    print('>>> there are {} removed by lower variation than {}'.format(n_gene_before_filter - n_gene_after_filter,
-                                                                       threshold))
-    return exp_df
-
-
-def read_exp_from_hcluster(filtered_exp_file_path, reordered_ind2sample_name_file_path):
-    """
-    read expression profiles from the result of hcluster
-    :param filtered_exp_file_path: gene by sample
-        filtered expression profiles
-    :param reordered_ind2sample_name_file_path: one of result files of hluster
-    :return: {"filtered_exp": filtered_exp, 'cell_type2sample_name': cell_type2sample_name}
-    """
-    cell_type2sample_name = {}  # {'cancer_cell': ['sample1', 'sample8'], '': [], ...}
-    filtered_exp = pd.read_csv(filtered_exp_file_path, index_col=0)
-    reordered_ind2sample_name = pd.read_csv(reordered_ind2sample_name_file_path, index_col=0)
-    reordered_ind2sample_name = reordered_ind2sample_name.loc[reordered_ind2sample_name['keep'] == 1, :]
-    filtered_exp = filtered_exp.loc[:, reordered_ind2sample_name.index].copy()
-    for sample_name in reordered_ind2sample_name.index:
-        cell_type = reordered_ind2sample_name.loc[sample_name, 'subtype']
-        if cell_type not in cell_type2sample_name.keys():
-            cell_type2sample_name[cell_type] = []
-        cell_type2sample_name[cell_type].append(sample_name)
-    return {"filtered_exp": filtered_exp, 'cell_type2sample_name': cell_type2sample_name}
-
-
-def read_cancer_purity(cancer_purity_file_path, sample_names: list):
-    """
-    Tumor purity estimates for TCGA samples
-    Aran, D., Sirota, M. & Butte, A. Systematic pan-cancer analysis of tumour purity. Nat Commun 6, 8971 (2015).
-    https://doi.org/10.1038/ncomms9971
-    :param cancer_purity_file_path:
-    :param sample_names: all sample names need to compare
-    :return:
-    """
-    cancer_purity = pd.read_csv(cancer_purity_file_path, index_col=0)
-    cancer_purity = cancer_purity.loc[~cancer_purity['CPE'].isnull()].copy()
-    # print_df(cancer_purity)
-    sample_name_mapping = {i[0:16]: i for i in sample_names}
-    common_sample = set(list(sample_name_mapping.keys())) & set(cancer_purity.index)
-    cancer_purity = cancer_purity.loc[common_sample, :].copy()
-    cancer_purity.index = cancer_purity.index.map(sample_name_mapping)
-    return cancer_purity
-
-
-def cal_relative_error(y_true, y_pred, max_error=None, min_error=None):
-    """
-    calculate relative error between two dataFrame
-    relative error = (y_pred - y_true) / y_true
-    :param y_true: dataframe
-    :param y_pred: dataframe, two dataframe have same index and columns (also same order)
-    :param max_error: float
-        all errors should <= this value
-    :param min_error: float
-        all errors should >= this value
-    :return:
-    """
-    relative_error = (y_pred - y_true) / y_true
-    if max_error:
-        relative_error[relative_error > max_error] = max_error
-    if min_error:
-        relative_error[relative_error < min_error] = min_error
-    return relative_error
-
-
-def calculate_rmse(y_true: pd.DataFrame, y_pred: pd.DataFrame):
-    """
-    https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_squared_error.html
-    calculate the RMSE of each cell types by columns
-    :param y_true: a dataFrame
-        shape: number of samples x number of cell types
-    :param y_pred: a dataFrame
-    :return:
-    """
-    if y_true.shape[1] == 1:  # only one feature
-        multioutput = 'uniform_average'
-    else:  # multiple cell types
-        multioutput = 'raw_values'
-    return mean_squared_error(y_true=y_true, y_pred=y_pred, multioutput=multioutput, squared=False)
-
-
-def calculate_r2(y_true, y_pred):
-    """
-    https://scikit-learn.org/stable/modules/generated/sklearn.metrics.r2_score.html
-    calculate the R^2 (coefficient of determination) of each cell types by columns
-    :param y_true:
-    :param y_pred:
-    :return:
-    """
-    return r2_score(y_true=y_true, y_pred=y_pred, multioutput='raw_values')
-
-
-def check_dir(path):
-    """
-    check if a path exist, create if not exist
-    :param path:
-    :return:
-    """
-    if not os.path.exists(path):
-        os.makedirs(path)
-
-
-def parse_log_file(log_file_path, search_type='sample'):
-    """
-    parse log file, @sample xxx, ...
-    :param log_file_path:
-    :param search_type: search gene or sample in log file
-    :return: list
-        a list of sample names
-    """
-    sample_names = []
-    if os.path.exists(log_file_path):
-        with open(log_file_path, 'r') as f:
-            for i in f:
-                i = i.strip()
-                _sample_name = i.split(',')[0].replace(f'@{search_type} ', '')
-                sample_names.append(_sample_name)
-    return sample_names
-
-
-def write_to_log(log_file_path, template, sample_names, n_round):
-    """
-
-    :param log_file_path:
-    :param template: '@sample {}, removed, ..., round {}', only two {} for sample name and n_round
-    :param sample_names:
-    :param n_round:
-    :return:
-    """
-    sample_names_in_log_file = parse_log_file(log_file_path)
-    with open(log_file_path, 'a') as f:
-        for s in sample_names:
-            _info = template.format(s, n_round)
-            if s not in sample_names_in_log_file:
-                f.write(_info + '\n')
-            print(_info)
-
-
-def correct_gene_list(exp_profile: pd.DataFrame, gene_list: list) -> pd.DataFrame:
-    """
-    add 0 to expression profile for genes which not exist and sort gene according to the order in gene_list
-    :param exp_profile: expression profiles of bulk data, sample by gene
-    :param gene_list: a gene list with same order as training set (kNN scaden or Scaden scaden, single cell data)
-    :return:
-    """
-    gene_not_in_bulk = [i for i in gene_list if i not in exp_profile.columns]
-    n_not_in = len(gene_not_in_bulk)
-    n_sample, _ = exp_profile.shape
-    if n_not_in >= 1:
-        # print(f'   > there are {n_not_in} genes not in gene list, 0 will be added for these genes')
-        add_zero_expression = pd.DataFrame(data=np.zeros((n_sample, n_not_in)),
-                                           index=exp_profile.index, columns=gene_not_in_bulk)
-        exp_profile = pd.concat([exp_profile, add_zero_expression], axis=1)
-    exp_profile = exp_profile.loc[:, gene_list]  # only use genes in gene_list
-    return exp_profile
-
-
-def extract_gz_file(file_dir: str, file_name: str):
-    file_path = os.path.join(file_dir, file_name)
-    file_path_out = os.path.join(file_dir, file_name.replace('.gz', ''))
-    if os.path.exists(file_path) and file_name.endswith('.gz'):
-        if not os.path.exists(file_path_out):
-            with gzip.open(file_path, 'rb') as f_in:
-                with open(file_path_out, 'wb') as f_out:
-                    shutil.copyfileobj(f_in, f_out)
-
-
-def create_h5ad_dataset(simulated_bulk_exp_file_path, cell_fraction_file_path,
-                        dataset_info, result_file_path: str,
-                        filtering: bool = False, merge_t_cell: bool = False, gep_type='bulk'):
-    """
-    create .h5ad file according to cell fraction and simulated bulk expression profiles
-    https://anndata.readthedocs.io/en/latest/index.html
-    :param simulated_bulk_exp_file_path: simulated bulk expression profile, samples by genes
-        .csv file or .h5ad file
-    :param cell_fraction_file_path: .csv file, samples by cell types
-    :param dataset_info: str
-    :param result_file_path:
-    :param filtering: if filtered by marker ratio
-    :param merge_t_cell: whether merge the cell fraction of CD8 T and CD4 T cells
-    :param gep_type: bulk (mixture contains >= 2 cell types) / sct (single cell type)
-    :return:
-    """
-    try:
-        if filtering:
-            simulated_bulk_exp_file_path = simulated_bulk_exp_file_path.replace('_log2cpm1p.csv',
-                                                                                '_log2cpm1p_filtered.csv')
-            cell_fraction_file_path = cell_fraction_file_path.replace('.csv', '_filtered.csv')
-        simu_bulk_exp_raw = read_df(simulated_bulk_exp_file_path)
-    except UnicodeDecodeError:
-        simu_bulk_exp_raw = read_h5ad(simulated_bulk_exp_file_path)
-    # simu_bulk_exp.index = simu_bulk_exp.index.astype(str)
-    cell_frac = read_df(cell_fraction_file_path)
-    if merge_t_cell:
-        if 'T Cells' not in cell_frac.columns:
-            cell_frac['T Cells'] = cell_frac.loc[:, ['CD4 T', 'CD8 T']].sum(axis=1)
-        cell_frac.drop(columns=['CD4 T', 'CD8 T'], inplace=True)
-    sample_list = cell_frac.index.to_list()
-    # cell_frac.index = cell_frac.index.astype(str)
-    uns = {'cell_types': cell_frac.columns.to_list(),
-           'dataset_info': dataset_info}
-    simu_bulk_exp = pd.DataFrame()
-    if type(simu_bulk_exp_raw) == pd.DataFrame:
-        simu_bulk_exp = simu_bulk_exp_raw.loc[sample_list, :]
-    elif type(simu_bulk_exp_raw) == AnnData:
-        simu_bulk_exp_df = pd.DataFrame(simu_bulk_exp_raw.X, index=simu_bulk_exp_raw.obs.index,
-                                        columns=simu_bulk_exp_raw.var.index)
-        simu_bulk_exp_df = simu_bulk_exp_df.loc[sample_list, :]
-        simu_bulk_exp = simu_bulk_exp_df.copy()
-    if (cell_frac.shape[0] == simu_bulk_exp.shape[0]) and not np.all(simu_bulk_exp.index == cell_frac.index):
-        cell_frac = cell_frac.loc[simu_bulk_exp.index, :].copy()
-    elif cell_frac.shape[0] != simu_bulk_exp.shape[0]:
-        print(f'   The shape of simu_bulk_exp: {simu_bulk_exp.shape}, the shape of cell_frac: {cell_frac.shape}')
-        cell_frac = cell_frac[~cell_frac.index.duplicated(keep='first')].copy()
-        simu_bulk_exp = simu_bulk_exp[~simu_bulk_exp.index.duplicated(keep='first')].copy()
-        intersection_inx = [i for i in simu_bulk_exp.index if i in cell_frac.index]
-        print(f'   The length of intersections in both cell_frac and simu_bulk_exp: {len(intersection_inx)}')
-        cell_frac = cell_frac.loc[intersection_inx, :].copy()
-        simu_bulk_exp = simu_bulk_exp.loc[intersection_inx, :].copy()
-    # print(cell_frac.index)
-    # print(simu_bulk_exp.index)
-    if np.all(simu_bulk_exp.index == cell_frac.index):
-        var = pd.DataFrame(index=simu_bulk_exp.columns, columns=[f'in_{gep_type}'])
-        var[f'in_{gep_type}'] = 1
-        adata = AnnData(X=simu_bulk_exp.values.astype('float32'), obs=cell_frac, uns=uns,
-                        var=var, dtype=np.dtype('float32'))
-        adata.write_h5ad(filename=Path(result_file_path), compression='gzip')
-    else:
-        raise KeyError('simu_bulk_exp and cell_frac file should have same sample order')
-
-
-def read_data_from_h5ad(h5ad_file_path: str) -> dict:
-    """
-    Read simulated bulk gene expression profiles (GEPs) from .h5ad file
-
-    :param h5ad_file_path: the file path of simulated bulk GEPs file (.h5ad)
-
-    :return: a dict contains bulk GEPs (bulk_exp) and cell fractions (cell_frac) used to generate this dataset
-    """
-    raw_input = read_h5ad(h5ad_file_path)
-    cell_fraction = raw_input.obs.round(3)
-    if type(raw_input.X) == csr_matrix:
-        x_data = raw_input.X.A.astype(np.float32)  # convert sparse matrix to dense matrix
-    else:
-        x_data = raw_input.X.astype(np.float32)  # samples x genes (eg: 6000 x 18863)
-    bulk_exp = pd.DataFrame(data=x_data, index=raw_input.obs.index, columns=raw_input.var.index).round(3)
-    return {'bulk_exp': bulk_exp, 'cell_frac': cell_fraction}
-
-
-def ciber_exp(bulk_exp_fp, index_sample=True, log_transformed=True, result_fp=None):
-    """
-    generate expression file format of CIBERSORT, gene by sample, non-log space, tab-delimited format
-    :param bulk_exp_fp: .csv file, log2(CPM + 1)
-    :param index_sample: sample by gene if True, or gene by sample if False
-    :param log_transformed: input dataset is log transformed if True
-    :param result_fp:
-    :return: gene by sample, non-log space values (CPM/TPM) and tab-delimited
-    """
-    bulk_exp = pd.read_csv(bulk_exp_fp, index_col=0)
-    if index_sample:
-        bulk_exp = bulk_exp.T
-    if log_transformed:
-        bulk_exp = log_exp2cpm(bulk_exp)
-    if result_fp is not None:
-        bulk_exp.round(2).to_csv(result_fp, sep='\t')
-
-
-def log_exp2cpm(exp_df: Union[pd.DataFrame, np.array], log_base=2, correct=1) -> Union[pd.DataFrame, np.array]:
-    """
-    Convert log2(CPM + 1) to non-log space values (CPM / TPM)
-
-    :param exp_df: samples by genes
-
-    :param log_base: the base of log transform
-
-    :param correct: plus 1 for avoiding log transform 0
-
-    :return: counts per million (CPM) or transcript per million (TPM)
-    """
-    exp = np.power(log_base, exp_df) - correct
-    # exp = exp.astype(np.float64)
-    cpm = exp / np.vstack(exp.sum(axis=1)) * 1e6
-    # cpm = cpm.astype(np.float32)
-    return cpm
-
-
-def non_log2log_cpm(input_file_path: Union[str, pd.DataFrame], result_file_path: str = None,
-                    transpose: bool = True, correct: int = 1):
-    """
-    Convert non-log expression data to log2(CPM + 1) or log2(TPM + 1)
-
-    :param input_file_path: non-log space expression file
-
-    :param result_file_path: file path, samples by genes
-
-    :param transpose: if input file is samples by genes, set to False, otherwise set to True
-
-    :param correct: plus 1 for avoiding log transform 0
-
-    :return: log2(CPM + 1) or save result to file
-    """
-
-    bulk_exp = pd.DataFrame()
-    if type(input_file_path) is str:
-        sep = get_sep(input_file_path)
-        bulk_exp = pd.read_csv(input_file_path, index_col=0, sep=sep)
-    elif type(input_file_path) is pd.DataFrame:
-        bulk_exp = input_file_path
-    if transpose:
-        bulk_exp = bulk_exp.T  # transpose to samples by genes
-    bulk_exp = non_log2cpm(bulk_exp)  # CPM/TPM
-    bulk_exp = np.log2(bulk_exp + correct)
-    if result_file_path is not None:
-        bulk_exp.round(3).to_csv(result_file_path)
-    else:
-        return bulk_exp.round(3)
-
-
-def non_log2cpm(exp_df, sum_exp=1e6) -> pd.DataFrame:
-    """
-    Normalize gene expression to CPM / TPM for non-log space
-
-    :param exp_df: gene expression profile in non-log space, sample by gene
-
-    :param sum_exp: sum of gene expression for each sample, default is 1e6
-
-    :return: counts per million (CPM) or transcript per million (TPM)
-    """
-    return exp_df / np.vstack(exp_df.sum(axis=1)) * sum_exp
-
-
-def get_corr(df_col1, df_col2, return_p_value=False) -> Union[float, tuple]:
-    """
-    calculate the correlation between two columns of dataframe
-    :param df_col1: series, column1
-    :param df_col2: series, column2
-    :param return_p_value: if return p-value
-    :return:
-    """
-    # correlation = np.corrcoef(df_col1, df_col2)
-    corr, p_value = stats.pearsonr(df_col1, df_col2)
-    if return_p_value:
-        return corr, p_value
-    else:
-        return corr
-    # return correlation[0, 1]
-
-
-def get_sep(file_path, comment: str = None):
-    """
-    check the separater (`\t` or `,`) in this file
-    :param file_path:
-    :param comment: if remove comment lines start with ''
-    :return:
-    """
-    sep = '\t'
-    with open(file_path, 'r') as f_handle:
-        # first_line = ''
-        while True:
-            first_line = f_handle.readline()
-            if comment is not None:
-                if first_line.startswith(comment):
-                    continue
-                else:
-                    break
-            break
-        if ',' in first_line:
-            sep = ','
-    return sep
-
-
-def read_marker_gene(marker_gene_file_path: str, include_t_cell: bool = False,
-                     include_cd8_nk_marker: bool = False, use_cancer_cell: bool = False,
-                     add_top_corr_gene: bool = False, corr_mean: bool = False) -> dict:
-    """
-    read marker genes for each cell type
-    :param marker_gene_file_path: file path of selected marker genes for each cell type
-    :param include_t_cell: if include the marker genes of T Cells for both CD4 and CD8 T
-    :param include_cd8_nk_marker: if remain "CD8 T / NK" marker genes
-    :param use_cancer_cell: if use "Cancer Cells" to replace "Epithelial Cells"
-    :param add_top_corr_gene: add top correlated genes from the corr between cell fraction and gene expression value
-    :param corr_mean: only two genes for CD4 T Cells and two genes for B Cells, others are same as core_marker
-    :return: a dict of cell type to marker genes, {'': []}
-    """
-    cell_type2marker = {}
-    marker_gene = pd.read_csv(marker_gene_file_path)
-    if 'corr_mean' in marker_gene.columns and corr_mean:
-        marker_gene = marker_gene.loc[marker_gene['corr_mean'] == 1, :].copy()
-    if 'core_marker' in marker_gene.columns:
-        if add_top_corr_gene:
-            marker_gene = marker_gene.loc[marker_gene['core_marker'].isin([1, 2]), :].copy()
-        else:
-            marker_gene = marker_gene.loc[marker_gene['core_marker'] == 1, :].copy()
-        if not include_cd8_nk_marker:
-            marker_gene = marker_gene.loc[marker_gene['cell_type'] != 'CD8 T / NK', :].copy()
-    cell_types = sorted(marker_gene['cell_type'].unique())
-    for ct in cell_types:
-        if include_t_cell:
-            cell_type2marker[ct] = list(marker_gene.loc[marker_gene['cell_type'] == ct, 'marker_gene'].unique())
-        else:
-            if ct != 'T Cells':
-                cell_type2marker[ct] = list(marker_gene.loc[marker_gene['cell_type'] == ct, 'marker_gene'].unique())
-    if include_cd8_nk_marker and cell_type2marker.get('CD8 T / NK', ''):
-        cell_type2marker['NK'] += cell_type2marker['CD8 T / NK']
-        cell_type2marker['CD8 T'] += cell_type2marker['CD8 T / NK']
-    if use_cancer_cell and 'Epithelial Cells' in cell_type2marker:
-        cell_type2marker['Cancer Cells'] = cell_type2marker['Epithelial Cells']
-        del cell_type2marker['Epithelial Cells']
-    return cell_type2marker
-
-
-def cal_exp_by_gene_list(exp_df, gene_list, min_exp_value=0, method='mean'):
-    """
-    calculate mean expression (or max) of a gene list (for single cell type)
-    :param exp_df: sample by gene, usually in CPM / TPM
-    :param gene_list: a list of genes which all are included in exp_df
-    :param min_exp_value: min mean expression of the gene list
-    :param method: mean or max
-    :return: mean or max expression value of marker genes for each sample
-    """
-    for gene in gene_list:
-        if gene not in exp_df.columns:
-            raise KeyError(f'Gene {gene} not include in exp_df')
-    current_exp = exp_df.loc[:, gene_list].copy()
-    if method == 'mean':
-        current_value = current_exp.mean(axis=1)
-    elif method == 'max':
-        current_value = current_exp.max(axis=1)
-    else:
-        raise KeyError('Only "mean" or "max" allowed')
-    current_value[current_value < min_exp_value] = min_exp_value
-    if exp_df.shape[0] == 1:
-        return round(float(current_value), 3)  # float
-    return current_value.round(3)  # pd.Series
-
-
-def save_key_params(all_vars: dict, save_to_file_path=None):
-    if save_to_file_path is None:
-        k_params_path = os.path.join(all_vars['result_dir'], 'key_parames.txt')
-    else:
-        k_params_path = save_to_file_path
-    if not os.path.exists(k_params_path):
-        key_paths = ['result_dir', 'merged_sc_dataset_file_path', 'simu_bulk_exp_dir', 'generated_sc_dataset_dir',
-                     'test_set_dir', 'tcga_data_dir', 'cancer_purity_file_path', 'marker_gene_file_path',
-                     'pre_trained_model_dir', 'pred_cell_frac_tcga_dir']
-        model_names = ['DeSide']
-        log_file_path = all_vars.get('log_file_path', '')
-        hyper_params = all_vars['deside_parameters']
-        other_params = ['all_cell_types', 'dataset2parameters', 'cd4_high_in_cd8', 'n_base',
-                        'total_cell_number', 'removed_cell_types', 'merge_t_cell', 'filter_simulated_bulk_cell',
-                        'remove_cancer_cell_when_training', 'one_minus_alpha', 'remove_cancer_cell']
-        key_paths_dict = {k: all_vars[k] for k in key_paths if k in all_vars}
-        other_params_dict = {k: all_vars[k] for k in other_params if k in all_vars}
-
-        all_key_params = {'model_names': model_names, 'key_paths_dict': key_paths_dict, 'hyper_params': hyper_params,
-                          'other_params': other_params_dict, 'key_params_path': k_params_path,
-                          'log_file_path': log_file_path}
-        with open(k_params_path, 'w', encoding='utf-8') as f:
-            json.dump(all_key_params, f, ensure_ascii=False, indent=4)
-
-
-def print_msg(p_str, log_file_path=None):
-    print()
-    current_info = f'---->>> {p_str} <<<----'
-    current_time = time.ctime()
-    print(current_info)
-    print(current_time)
-    if log_file_path is not None:
-        with open(log_file_path, 'a') as f_handle:
-            f_handle.write(current_info + '\n')
-            f_handle.write(current_time + '\n')
-            f_handle.write('\n')
-
-
-def read_xy(a: Union[str, pd.DataFrame], xy='cell_frac') -> pd.DataFrame:
-    """
-    read cell fraction or bulk expression
-    :param a: a file path or a DataFrame
-    :param xy: cell_frac or bulk_exp, only for .h5ad file
-    """
-    if (type(a) == str) and ('.h5ad' in a):
-        raw_data = read_data_from_h5ad(a)
-        exp = raw_data[xy]
-    else:
-        exp = read_df(a)
-    return exp
-
-
-def cal_corr_gene_exp_with_cell_frac(gene_exp: pd.DataFrame, cell_frac: pd.DataFrame,
-                                     result_file_path=None, filtered_by_corr: float = None,
-                                     filter_by_num: int = None):
-    """
-    calculate correlation between gene expression values and cell fractions for each cell type
-    :param gene_exp: non-log space, tpm/cpm, samples by genes
-    :param cell_frac: samples by cell types
-    :param result_file_path:
-    :param filtered_by_corr: threshold of correlation, only keep genes with higher corr than this value
-    :param filter_by_num: the max number of genes to keep for each cell type
-    :return: correlation, genes by cell types, filtered or all gene list
-    """
-    if not os.path.exists(result_file_path):
-        _, n_cell_type = cell_frac.shape
-        _, n_gene = gene_exp.shape
-        print(f'The shape of cell_frac: {cell_frac.shape}')
-        print(f'The shape of gene_exp: {gene_exp.shape}')
-        corr = np.corrcoef(cell_frac.values, gene_exp.values, rowvar=False)
-        corr_df = pd.DataFrame(data=corr[:n_cell_type, n_cell_type:].T,
-                               columns=cell_frac.columns, index=gene_exp.columns)
-    else:
-        print(f'Previous correlation file will be used: {result_file_path}')
-        corr_df = pd.read_csv(result_file_path, index_col=0)
-    if (filtered_by_corr is not None) and (filter_by_num is not None):
-        for cell_type in corr_df.columns:
-            if corr_df.loc[corr_df[cell_type] >= filtered_by_corr, cell_type].shape[0] > filter_by_num:
-                corr_df2 = corr_df.sort_values(by=[cell_type], ascending=False)
-                # set to 0 if there are too many high corr genes for the cell fraction of this cell type
-                corr_df.loc[corr_df.index.isin(corr_df2.iloc[filter_by_num:, :].index), cell_type] = 0
-        corr_df[f'n_at_least_one'] = np.sum(corr_df >= filtered_by_corr, axis=1)
-    elif filtered_by_corr is not None:
-        corr_df[f'n_at_least_one'] = np.sum(corr_df >= filtered_by_corr, axis=1)
-    elif filter_by_num is not None:
-        for cell_type in corr_df.columns:
-            corr_df2 = corr_df.sort_values(by=[cell_type], ascending=False)
-            # set to 0 if there are too many genes than filter_by_num of this cell type
-            corr_df.loc[corr_df.index.isin(corr_df2.iloc[filter_by_num:, :].index), cell_type] = 0
-        corr_df[f'n_at_least_one'] = np.sum(corr_df > 0, axis=1)
-    if (filtered_by_corr is not None) or (filter_by_num is not None):
-        corr_df_filtered = corr_df.loc[corr_df[f'n_at_least_one'] >= 1,
-                                       [i for i in corr_df.columns if i != 'n_at_least_one']].copy()
-        corr_df_filtered.to_csv(result_file_path, float_format='%g')
-        return corr_df_filtered
-    else:
-        corr_df.to_csv(result_file_path, float_format='%g')
-        return corr_df
-
-
-def read_df(df_file: Union[str, pd.DataFrame, np.ndarray]) -> Union[pd.DataFrame, np.ndarray]:
-    """
-    check the type of df_file
-    - if df_file is a file path, read this file
-    - if df_file is a DataFrame, return directly
-    """
-    if type(df_file) == str:  # the file path of current file
-        sep = get_sep(df_file)  # separated by '\t' or ','
-        df = pd.read_csv(df_file, index_col=0, sep=sep)
-    elif type(df_file) == pd.DataFrame:
-        return df_file  # return DataFrame directly
-    elif type(df_file) == np.ndarray:
-        return df_file  # return np.ndarray directly
-    else:
-        raise TypeError(
-            f'Only file path or pd.DataFrame was supported by df_file, {type(df_file)} is not supported.')
-    return df
-
-
-def aggregate_marker_gene_exp(exp_df: pd.DataFrame, marker_genes: dict = None,
-                              agg_methods: dict = None, return_ratio: bool = False,
-                              show_marker_gene: bool = True):
-    """
-    aggregate marker genes by the corresponding method in agg_methods (mean or max)
-    :param exp_df: a DataFrame of gene expression profiles, TPM, samples by genes
-    :param marker_genes:
-    :param agg_methods: aggregate multiple marker genes of a cell type by `mean` or `max`
-    :param return_ratio: return the ratio of aggregated marker gene exp for each cell type if True
-    :param show_marker_gene: whether printing marker genes or not
-    """
-    if marker_genes is None:
-        marker_genes = default_core_marker_genes.copy()
-    if agg_methods is None:
-        agg_methods = {}
-    for k, _ in marker_genes.items():
-        if k not in agg_methods:
-            agg_methods[k] = 'mean'
-
-    cell_type2marker_exp = {}
-    for ct, marker in marker_genes.items():
-        method = agg_methods[ct]
-        current_tpm = exp_df.loc[:, exp_df.columns.isin(marker)].copy()  # sample by gene
-        current_valid_marker = current_tpm.columns.to_list()
-        if len(current_valid_marker) > 0:
-            current_marker_str = ', '.join(current_valid_marker)
-            if show_marker_gene:
-                print(f'   Using {len(current_valid_marker)} marker genes for cell type {ct}: {current_marker_str}')
-            # cell_type2mean_exp[ct + '_marker_mean'] = current_tpm.mean(axis=0)
-            cell_type2marker_exp[ct + f'_marker_{method}'] = cal_exp_by_gene_list(exp_df=exp_df, method=method,
-                                                                                  gene_list=current_valid_marker,
-                                                                                  min_exp_value=1)
-        else:
-            Warning(f'No any marker genes in bulk cell TPM for cell type {ct}, '
-                    f'this cell type will be ignored in later analysis.')
-    marker_exp = pd.DataFrame.from_dict(cell_type2marker_exp, orient='columns')
-    if return_ratio:
-        return marker_exp / marker_exp.sum(axis=1).values.reshape(-1, 1)
-    else:
-        return marker_exp.round(3)
-
-
-def cal_marker_ratio(bulk_exp_file_path: str, marker_genes: dict, marker_ratio_file_path: str,
-                     agg_methods: dict = None, log_transformed: bool = True):
-    """
-    calculate marker ratio of each sample by gene expression values at large scale
-    :param bulk_exp_file_path: log2cpm1p or TPM/CPM
-    :param marker_genes:
-    :param log_transformed: whether log2cpm1p or TPM/CPM
-    :param marker_ratio_file_path: result file path
-    :param agg_methods: aggregate multiple marker genes of a cell type by `mean` or `max`
-    """
-    if not os.path.exists(marker_ratio_file_path):
-        # cell_frac = pd.read_csv(cell_frac_file_path, index_col=0)
-        cell_types = list(marker_genes.keys())  # cell types in current dataset
-        # only keep cell types in current dataset
-        marker_genes = {k: v for k, v in marker_genes.items() if k in cell_types}
-        # marker_ratio_dict = {}
-        # col_names = None
-
-        with open(marker_ratio_file_path, 'w') as write_file_handle:
-            csv_writer = csv.writer(write_file_handle)
-            csv_writer.writerow(['sample_id'] + list(marker_genes.keys()))
-        with pd.read_csv(bulk_exp_file_path, chunksize=1000, index_col=0) as f_handle:
-            for chunk in f_handle:
-                if 'cancer_type' in chunk.columns:
-                    chunk = chunk.drop(columns=['cancer_type'])
-                if log_transformed:
-                    current_exp = log_exp2cpm(chunk)  # convert log2cpm1p to CPM / TPM
-                else:
-                    current_exp = chunk
-                current_marker_ratio = aggregate_marker_gene_exp(exp_df=current_exp, marker_genes=marker_genes,
-                                                                 agg_methods=agg_methods, return_ratio=True)
-                current_marker_ratio.to_csv(marker_ratio_file_path, mode='a', header=False, float_format='%g')
-    else:
-        print(f'   Previous result has existed: {marker_ratio_file_path}')
-
-
-def get_cell_num(cell_type_frac, total_num=500):
-    """
-    calculate the number of cells to choose for each cell type based on the total number of cells
-    and fraction of each cell type
-    :param cell_type_frac: dataFrame
-        the fraction of each cell type, sum to 1 for each row, samples by cell types
-    :param total_num: the total number of cells contributing to one simulated RNA-seq sample
-    :return:
-    """
-    assert type(cell_type_frac) is pd.DataFrame
-    cell_num = cell_type_frac * total_num
-    if total_num == 1:  # assign 1 for all cell types for matrix multiplication
-        cell_num = cell_type_frac * 0 + 1
-    elif total_num == 0:
-        cell_num = np.ceil(cell_type_frac)  # assign 1 for the cell types with non-zero cell fractions
-    return cell_num.round(0).astype(int)
-
-
-def do_pca_analysis(exp_df, n_components=5, pca_result_fp=None, save_model: bool = False):
-    """
-    PCA analysis
-    :param exp_df:
-    :param n_components:
-    :param pca_result_fp:
-    :param save_model:
-    :return: fitted PCA model
-    """
-    if os.path.exists(pca_result_fp):
-        print(f'Loading PCA result from file: {pca_result_fp}')
-        pca = load(pca_result_fp)
-    else:
-        pca = PCA(n_components=n_components)
-        pca.fit(exp_df)
-        if save_model:
-            dump(pca, pca_result_fp)
-    return pca
-
-
-def do_umap_analysis(exp_df, n_components=5, n_neighbors=15, min_dist=0.1,
-                     umap_model_result_fp=None, save_model: bool = False):
-    """
-    t-SNE analysis
-    :param exp_df:
-    :param n_components:
-    :param n_neighbors:
-    :param min_dist:
-    :param umap_model_result_fp:
-    :param save_model:
-    :return:
-    """
-    if os.path.exists(umap_model_result_fp):
-        print(f'Loading UMAP result from file: {umap_model_result_fp}')
-        umap_model = load(umap_model_result_fp)
-    else:
-        umap_model = umap.UMAP(n_neighbors=n_neighbors, min_dist=min_dist, n_components=n_components)
-        umap_model.fit(exp_df)
-        if save_model:
-            dump(umap_model, umap_model_result_fp)
-    return umap_model
-
-
-def get_ccc(x, y):
-    # Concordance Correlation Coefficient(CCC), https://en.wikipedia.org/wiki/Concordance_correlation_coefficient
-    vx, cov_xy, cov_xy, vy = np.cov(x, y, bias=True).flatten()
-    mx, my = x.mean(), y.mean()
-    return 2*cov_xy / (vx + vy + (mx-my)**2)
-
-
-if __name__ == '__main__':
-    pass
+import os
+import csv
+import json
+import time
+import umap
+from typing import Union
+import numpy as np
+import pandas as pd
+# import anndata as an
+import seaborn as sns
+import matplotlib as mpl
+from pathlib import Path
+import scipy.stats as stats
+from joblib import dump, load
+import matplotlib.pyplot as plt
+from scipy.sparse import csr_matrix
+from sklearn.decomposition import PCA
+from anndata import AnnData, read_h5ad
+from sklearn.metrics import mean_squared_error, r2_score
+import gzip
+import shutil
+
+
+default_core_marker_genes = {'Cancer Cells': ['KRT19', 'KRT18', 'KRT8', 'EPCAM'],
+                             'CD4 T': ['BATF', 'ICOS', 'CD4', 'IL7R', 'FOXP3', 'TIGIT'],
+                             'CD8 T': ['CD8A', 'CD8B'],
+                             'T Cells': ['CD2', 'CD3D', 'CD3E'],
+                             'B Cells': ['BANK1', 'CD79A', 'FCRL5', 'MS4A1'],
+                             'DC': ['GZMB', 'CCR7', 'LAMP3', 'IRF7', 'IRF8'],
+                             'Endothelial Cells': ['CLDN5', 'ENG', 'PLVAP', 'VWF'],
+                             'Fibroblasts': ['COL1A1', 'COL1A2', 'COL3A1', 'MYL9'],
+                             'Macrophages': ['AIF1', 'CD14', 'CD68', 'MS4A7'],
+                             'Mast Cells': ['CPA3', 'HPGDS', 'GATA2'],
+                             'NK': ['GNLY', 'NKG7', 'KLRD1'],
+                             'Neutrophils': ['CSF3R', 'CXCR2', 'FPR1', 'SLC25A37']}
+
+
+sorted_cell_types = ['B Cells', 'CD4 T', 'CD8 T', 'Cancer Cells', 'DC', 'Endothelial Cells',
+                     'Fibroblasts', 'Macrophages', 'Mast Cells', 'NK', 'Neutrophils']
+
+
+def get_inx2cell_type() -> dict:
+    inx2cell_type = {_i: ct for _i, ct in enumerate(sorted_cell_types)}
+    inx2cell_type[-1] = 'Neg'
+    return inx2cell_type
+
+
+def print_df(df):
+    assert type(df) == pd.DataFrame
+    print('  >>  <<  ')
+    print(df.shape)
+    print(df.head(2))
+
+
+def set_fig_style(font_family=None, font_size=None):
+    fig, ax = plt.subplots()
+    sns.set_style("white")
+    try:
+        plt.style.use(['science', 'no-latex'])
+    except:
+        print('No science style')
+        sns.set(palette='muted', font_scale=1.5)
+
+    mpl.rcParams['figure.dpi'] = 300
+    mpl.rcParams['figure.facecolor'] = 'white'
+    mpl.rcParams['pdf.fonttype'] = 42
+    mpl.rcParams['ps.fonttype'] = 42
+    plt.rcParams['svg.fonttype'] = 'none'
+    if font_family:
+        mpl.rcParams['font.family'] = font_family
+    if font_size:
+        mpl.rcParams['font.size'] = font_size
+    # print('figure.dpi will be set to', mpl.rcParams['figure.dpi'])
+    plt.close('all')
+
+
+def filter_gene_by_expression_log_mean(exp_df, min_exp_value=3, max_exp_value=10, min_exp_percent=0.8):
+    """
+    Ea(i)=log2(ave(TPM(i)1..k)+1), excluded genes with Ea<threshold
+
+    "As genes with high expression can bias deconvolution results,
+     we excluded the genes whose expression exceeded 700 TPM",
+     Finotello, F. et al., Genome Med 11, 34 (2019). https://doi.org/10.1186/s13073-019-0638-6
+
+    :param exp_df: expression values of each gene, non-log2 values, a dataframe
+    :param min_exp_value: minimum log2 mean expression value of each gene across all samples
+    :param max_exp_value: max log2 mean expression value of each gene across all samples
+    :param min_exp_percent: minimum expression percentage of each gene in all samples
+    :return: filtered genes in each sample
+    """
+    # assert type(exp_df) == pd.
+    n_gene = exp_df.shape[0]
+    n_sample = exp_df.shape[1]
+    print('>>> Total gene: {}'.format(n_gene))
+    log_mean_exp = np.log2(exp_df.mean(axis=1) + 1)
+    above_min_exp_inx = log_mean_exp >= min_exp_value
+    below_max_exp_inx = log_mean_exp <= max_exp_value
+    exp_filtered_by_min_exp = exp_df.loc[above_min_exp_inx & below_max_exp_inx, :]
+    print('>>> Number of gene below min_exp_value: {}'.format(n_gene - sum(above_min_exp_inx)))
+    print('>>> Number of gene above max_exp_value: {}'.format(n_gene - sum(below_max_exp_inx)))
+    # remove genes that does not express in high percentage samples
+    keep_inx = (np.sum(exp_filtered_by_min_exp < min_exp_value, axis=1) / n_sample) < min_exp_percent
+    return exp_filtered_by_min_exp.loc[keep_inx, :].copy()
+
+
+def filter_gene_by_expression_min_max(exp_df, min_exp_value=3, max_exp_value=1000,
+                                      min_exp_percent=0.8, high_exp_min_percent=0.2,
+                                      min_num_sample=50):
+    """
+    exclude genes with E < min_exp_value among more than 20% (1-min_exp_percent) samples
+    exclude genes with E > max_exp_value among less than 20% (high_exp_min_percent) samples
+
+    "As genes with high expression can bias deconvolution results,
+     we excluded the genes whose expression exceeded 700 TPM",
+     Finotello, F. et al., Genome Med 11, 34 (2019). https://doi.org/10.1186/s13073-019-0638-6
+
+    :param exp_df: expression values of each gene, non-log2 values, a dataframe
+    :param min_exp_value: minimum expression value of each gene across all samples
+    :param max_exp_value: max expression value of each gene across all samples
+    :param min_exp_percent: float
+        the min expression value of each gene should >=min_exp_value in all samples higher than this percent,
+        otherwise will be exclude (treat as no expression in all samples), at least 0.8
+    :param high_exp_min_percent: float
+        the max expression value of each gene should >=max_exp_value in all samples higher than this percent,
+        otherwise will be exclude (treat as only having extremely high expression in a few samples)
+    :param min_num_sample: the minimum number of samples needs to fulfil above conditions instead of using percentage
+
+    :return: filtered genes in each sample
+    """
+    n_gene = exp_df.shape[0]
+    n_sample = exp_df.shape[1]
+    print('>>> Total gene: {}'.format(n_gene))
+    # log_mean_exp = np.log2(exp_df.mean(axis=1) + 1)
+    # no expression in the most of samples
+    if n_sample > min_num_sample / (1 - min_exp_percent):
+        min_exp_percent = 1 - min_num_sample / n_sample  # bigger min_exp_percent in big n_sample
+    nm_exp_inx = (np.sum(exp_df < min_exp_value, axis=1) / n_sample) > min_exp_percent
+    # exist extremely high expression in a few samples
+    if n_sample >= min_num_sample / high_exp_min_percent:
+        high_exp_min_percent = min_num_sample / n_sample
+    ehf_exp_inx = ((np.sum(exp_df > max_exp_value, axis=1) / n_sample) < high_exp_min_percent) & \
+                  ((np.sum(exp_df > max_exp_value, axis=1) / n_sample) > 0)
+
+    print('>>> Number of gene which no expression in the most of samples: {}'.format(sum(nm_exp_inx)))
+    print('>>> Number of gene which extremely high expression in a few samples: {}'.format(sum(ehf_exp_inx)))
+    return exp_df.loc[~(nm_exp_inx | ehf_exp_inx), :].copy()
+
+
+def filter_sample_by_expression(exp_df, max_mean_exp=100, plot_cdf=True, fig_file_path=""):
+    """
+    remove samples have high mean expression, usually contain some extremely high expressed genes
+    :param exp_df:
+    :param max_mean_exp:
+    :param plot_cdf: plot CDF of sample mean expression
+    :param fig_file_path: where to save cdf figure
+    """
+    sample_mean_exp = exp_df.mean()
+    n_sample = exp_df.shape[1]
+    if plot_cdf:
+        plt.figure(figsize=(8, 6))
+        plt.hist(sample_mean_exp, density=True, cumulative=True, histtype='step', color='k')
+        if fig_file_path:
+            plt.savefig(fig_file_path, dpi=200)
+        plt.show()
+    below_max_inx = sample_mean_exp <= max_mean_exp
+    print('>>> Number of sample above max_mean_exp: {}'.format(n_sample - sum(below_max_inx)))
+    return exp_df.loc[:, below_max_inx].copy()
+
+
+def log2_transform(df):
+    """
+    log2 transform expression values (plus 1)
+    :param df:
+    :return:
+    """
+    df = df.astype(np.float64)
+    df = np.log2(df + 1)
+    df = df.astype(np.float32)
+    return df
+
+
+def center_value(df, return_mean=False):
+    """
+    exp - mean(exp) for each genes
+    :param df: expression dataframe, gene x sample
+    :param return_mean: if return df_mean
+    :return:
+    """
+    df_mean = df.mean(axis=1)
+    if return_mean:
+        return df - np.vstack(df_mean), df_mean.to_frame('gene_mean')
+    return df - np.vstack(df_mean)
+
+
+def filter_gene_by_variance(exp_df, threshold=0.1):
+    """
+    remove genes which variation is < threshold
+    :param exp_df:
+    :param threshold:
+    :return:
+    """
+    n_gene_before_filter = exp_df.shape[0]
+    exp_var = exp_df.var(axis=1)
+    exp_df = exp_df.loc[exp_var >= threshold, :].copy()
+    n_gene_after_filter = exp_df.shape[0]
+    print('>>> there are {} removed by lower variation than {}'.format(n_gene_before_filter - n_gene_after_filter,
+                                                                       threshold))
+    return exp_df
+
+
+def read_exp_from_hcluster(filtered_exp_file_path, reordered_ind2sample_name_file_path):
+    """
+    read expression profiles from the result of hcluster
+    :param filtered_exp_file_path: gene by sample
+        filtered expression profiles
+    :param reordered_ind2sample_name_file_path: one of result files of hluster
+    :return: {"filtered_exp": filtered_exp, 'cell_type2sample_name': cell_type2sample_name}
+    """
+    cell_type2sample_name = {}  # {'cancer_cell': ['sample1', 'sample8'], '': [], ...}
+    filtered_exp = pd.read_csv(filtered_exp_file_path, index_col=0)
+    reordered_ind2sample_name = pd.read_csv(reordered_ind2sample_name_file_path, index_col=0)
+    reordered_ind2sample_name = reordered_ind2sample_name.loc[reordered_ind2sample_name['keep'] == 1, :]
+    filtered_exp = filtered_exp.loc[:, reordered_ind2sample_name.index].copy()
+    for sample_name in reordered_ind2sample_name.index:
+        cell_type = reordered_ind2sample_name.loc[sample_name, 'subtype']
+        if cell_type not in cell_type2sample_name.keys():
+            cell_type2sample_name[cell_type] = []
+        cell_type2sample_name[cell_type].append(sample_name)
+    return {"filtered_exp": filtered_exp, 'cell_type2sample_name': cell_type2sample_name}
+
+
+def read_cancer_purity(cancer_purity_file_path, sample_names: list):
+    """
+    Tumor purity estimates for TCGA samples
+    Aran, D., Sirota, M. & Butte, A. Systematic pan-cancer analysis of tumour purity. Nat Commun 6, 8971 (2015).
+    https://doi.org/10.1038/ncomms9971
+    :param cancer_purity_file_path:
+    :param sample_names: all sample names need to compare
+    :return:
+    """
+    cancer_purity = pd.read_csv(cancer_purity_file_path, index_col=0)
+    cancer_purity = cancer_purity.loc[~cancer_purity['CPE'].isnull()].copy()
+    # print_df(cancer_purity)
+    sample_name_mapping = {i[0:16]: i for i in sample_names}
+    common_sample = set(list(sample_name_mapping.keys())) & set(cancer_purity.index)
+    cancer_purity = cancer_purity.loc[common_sample, :].copy()
+    cancer_purity.index = cancer_purity.index.map(sample_name_mapping)
+    return cancer_purity
+
+
+def cal_relative_error(y_true, y_pred, max_error=None, min_error=None):
+    """
+    calculate relative error between two dataFrame
+    relative error = (y_pred - y_true) / y_true
+    :param y_true: dataframe
+    :param y_pred: dataframe, two dataframe have same index and columns (also same order)
+    :param max_error: float
+        all errors should <= this value
+    :param min_error: float
+        all errors should >= this value
+    :return:
+    """
+    relative_error = (y_pred - y_true) / y_true
+    if max_error:
+        relative_error[relative_error > max_error] = max_error
+    if min_error:
+        relative_error[relative_error < min_error] = min_error
+    return relative_error
+
+
+def calculate_rmse(y_true: pd.DataFrame, y_pred: pd.DataFrame):
+    """
+    https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_squared_error.html
+    calculate the RMSE of each cell types by columns
+    :param y_true: a dataFrame
+        shape: number of samples x number of cell types
+    :param y_pred: a dataFrame
+    :return:
+    """
+    if y_true.shape[1] == 1:  # only one feature
+        multioutput = 'uniform_average'
+    else:  # multiple cell types
+        multioutput = 'raw_values'
+    return mean_squared_error(y_true=y_true, y_pred=y_pred, multioutput=multioutput, squared=False)
+
+
+def calculate_r2(y_true, y_pred):
+    """
+    https://scikit-learn.org/stable/modules/generated/sklearn.metrics.r2_score.html
+    calculate the R^2 (coefficient of determination) of each cell types by columns
+    :param y_true:
+    :param y_pred:
+    :return:
+    """
+    return r2_score(y_true=y_true, y_pred=y_pred, multioutput='raw_values')
+
+
+def check_dir(path):
+    """
+    check if a path exist, create if not exist
+    :param path:
+    :return:
+    """
+    if not os.path.exists(path):
+        os.makedirs(path)
+
+
+def parse_log_file(log_file_path, search_type='sample'):
+    """
+    parse log file, @sample xxx, ...
+    :param log_file_path:
+    :param search_type: search gene or sample in log file
+    :return: list
+        a list of sample names
+    """
+    sample_names = []
+    if os.path.exists(log_file_path):
+        with open(log_file_path, 'r') as f:
+            for i in f:
+                i = i.strip()
+                _sample_name = i.split(',')[0].replace(f'@{search_type} ', '')
+                sample_names.append(_sample_name)
+    return sample_names
+
+
+def write_to_log(log_file_path, template, sample_names, n_round):
+    """
+
+    :param log_file_path:
+    :param template: '@sample {}, removed, ..., round {}', only two {} for sample name and n_round
+    :param sample_names:
+    :param n_round:
+    :return:
+    """
+    sample_names_in_log_file = parse_log_file(log_file_path)
+    with open(log_file_path, 'a') as f:
+        for s in sample_names:
+            _info = template.format(s, n_round)
+            if s not in sample_names_in_log_file:
+                f.write(_info + '\n')
+            print(_info)
+
+
+def correct_gene_list(exp_profile: pd.DataFrame, gene_list: list) -> pd.DataFrame:
+    """
+    add 0 to expression profile for genes which not exist and sort gene according to the order in gene_list
+    :param exp_profile: expression profiles of bulk data, sample by gene
+    :param gene_list: a gene list with same order as training set (kNN scaden or Scaden scaden, single cell data)
+    :return:
+    """
+    gene_not_in_bulk = [i for i in gene_list if i not in exp_profile.columns]
+    n_not_in = len(gene_not_in_bulk)
+    n_sample, _ = exp_profile.shape
+    if n_not_in >= 1:
+        # print(f'   > there are {n_not_in} genes not in gene list, 0 will be added for these genes')
+        add_zero_expression = pd.DataFrame(data=np.zeros((n_sample, n_not_in)),
+                                           index=exp_profile.index, columns=gene_not_in_bulk)
+        exp_profile = pd.concat([exp_profile, add_zero_expression], axis=1)
+    exp_profile = exp_profile.loc[:, gene_list]  # only use genes in gene_list
+    return exp_profile
+
+
+def extract_gz_file(file_dir: str, file_name: str):
+    file_path = os.path.join(file_dir, file_name)
+    file_path_out = os.path.join(file_dir, file_name.replace('.gz', ''))
+    if os.path.exists(file_path) and file_name.endswith('.gz'):
+        if not os.path.exists(file_path_out):
+            with gzip.open(file_path, 'rb') as f_in:
+                with open(file_path_out, 'wb') as f_out:
+                    shutil.copyfileobj(f_in, f_out)
+
+
+def create_h5ad_dataset(simulated_bulk_exp_file_path, cell_fraction_file_path,
+                        dataset_info, result_file_path: str,
+                        filtering: bool = False, merge_t_cell: bool = False, gep_type='bulk'):
+    """
+    create .h5ad file according to cell fraction and simulated bulk expression profiles
+    https://anndata.readthedocs.io/en/latest/index.html
+    :param simulated_bulk_exp_file_path: simulated bulk expression profile, samples by genes
+        .csv file or .h5ad file
+    :param cell_fraction_file_path: .csv file, samples by cell types
+    :param dataset_info: str
+    :param result_file_path:
+    :param filtering: if filtered by marker ratio
+    :param merge_t_cell: whether merge the cell fraction of CD8 T and CD4 T cells
+    :param gep_type: bulk (mixture contains >= 2 cell types) / sct (single cell type)
+    :return:
+    """
+    try:
+        if filtering:
+            simulated_bulk_exp_file_path = simulated_bulk_exp_file_path.replace('_log2cpm1p.csv',
+                                                                                '_log2cpm1p_filtered.csv')
+            cell_fraction_file_path = cell_fraction_file_path.replace('.csv', '_filtered.csv')
+        simu_bulk_exp_raw = read_df(simulated_bulk_exp_file_path)
+    except UnicodeDecodeError:
+        simu_bulk_exp_raw = read_h5ad(simulated_bulk_exp_file_path)
+    # simu_bulk_exp.index = simu_bulk_exp.index.astype(str)
+    cell_frac = read_df(cell_fraction_file_path)
+    if merge_t_cell:
+        if 'T Cells' not in cell_frac.columns:
+            cell_frac['T Cells'] = cell_frac.loc[:, ['CD4 T', 'CD8 T']].sum(axis=1)
+        cell_frac.drop(columns=['CD4 T', 'CD8 T'], inplace=True)
+    sample_list = cell_frac.index.to_list()
+    # cell_frac.index = cell_frac.index.astype(str)
+    uns = {'cell_types': cell_frac.columns.to_list(),
+           'dataset_info': dataset_info}
+    simu_bulk_exp = pd.DataFrame()
+    if type(simu_bulk_exp_raw) == pd.DataFrame:
+        simu_bulk_exp = simu_bulk_exp_raw.loc[sample_list, :]
+    elif type(simu_bulk_exp_raw) == AnnData:
+        simu_bulk_exp_df = pd.DataFrame(simu_bulk_exp_raw.X, index=simu_bulk_exp_raw.obs.index,
+                                        columns=simu_bulk_exp_raw.var.index)
+        simu_bulk_exp_df = simu_bulk_exp_df.loc[sample_list, :]
+        simu_bulk_exp = simu_bulk_exp_df.copy()
+    if (cell_frac.shape[0] == simu_bulk_exp.shape[0]) and not np.all(simu_bulk_exp.index == cell_frac.index):
+        cell_frac = cell_frac.loc[simu_bulk_exp.index, :].copy()
+    elif cell_frac.shape[0] != simu_bulk_exp.shape[0]:
+        print(f'   The shape of simu_bulk_exp: {simu_bulk_exp.shape}, the shape of cell_frac: {cell_frac.shape}')
+        cell_frac = cell_frac[~cell_frac.index.duplicated(keep='first')].copy()
+        simu_bulk_exp = simu_bulk_exp[~simu_bulk_exp.index.duplicated(keep='first')].copy()
+        intersection_inx = [i for i in simu_bulk_exp.index if i in cell_frac.index]
+        print(f'   The length of intersections in both cell_frac and simu_bulk_exp: {len(intersection_inx)}')
+        cell_frac = cell_frac.loc[intersection_inx, :].copy()
+        simu_bulk_exp = simu_bulk_exp.loc[intersection_inx, :].copy()
+    # print(cell_frac.index)
+    # print(simu_bulk_exp.index)
+    if np.all(simu_bulk_exp.index == cell_frac.index):
+        var = pd.DataFrame(index=simu_bulk_exp.columns, columns=[f'in_{gep_type}'])
+        var[f'in_{gep_type}'] = 1
+        adata = AnnData(X=simu_bulk_exp.values.astype('float32'), obs=cell_frac, uns=uns,
+                        var=var, dtype=np.dtype('float32'))
+        adata.write_h5ad(filename=Path(result_file_path), compression='gzip')
+    else:
+        raise KeyError('simu_bulk_exp and cell_frac file should have same sample order')
+
+
+def read_data_from_h5ad(h5ad_file_path: str) -> dict:
+    """
+    Read simulated bulk gene expression profiles (GEPs) from .h5ad file
+
+    :param h5ad_file_path: the file path of simulated bulk GEPs file (.h5ad)
+
+    :return: a dict contains bulk GEPs (bulk_exp) and cell fractions (cell_frac) used to generate this dataset
+    """
+    raw_input = read_h5ad(h5ad_file_path)
+    cell_fraction = raw_input.obs.round(3)
+    if type(raw_input.X) == csr_matrix:
+        x_data = raw_input.X.A.astype(np.float32)  # convert sparse matrix to dense matrix
+    else:
+        x_data = raw_input.X.astype(np.float32)  # samples x genes (eg: 6000 x 18863)
+    bulk_exp = pd.DataFrame(data=x_data, index=raw_input.obs.index, columns=raw_input.var.index).round(3)
+    return {'bulk_exp': bulk_exp, 'cell_frac': cell_fraction}
+
+
+def ciber_exp(bulk_exp_fp, index_sample=True, log_transformed=True, result_fp=None):
+    """
+    generate expression file format of CIBERSORT, gene by sample, non-log space, tab-delimited format
+    :param bulk_exp_fp: .csv file, log2(CPM + 1)
+    :param index_sample: sample by gene if True, or gene by sample if False
+    :param log_transformed: input dataset is log transformed if True
+    :param result_fp:
+    :return: gene by sample, non-log space values (CPM/TPM) and tab-delimited
+    """
+    bulk_exp = pd.read_csv(bulk_exp_fp, index_col=0)
+    if index_sample:
+        bulk_exp = bulk_exp.T
+    if log_transformed:
+        bulk_exp = log_exp2cpm(bulk_exp)
+    if result_fp is not None:
+        bulk_exp.round(2).to_csv(result_fp, sep='\t')
+
+
+def log_exp2cpm(exp_df: Union[pd.DataFrame, np.array], log_base=2, correct=1) -> Union[pd.DataFrame, np.array]:
+    """
+    Convert log2(CPM + 1) to non-log space values (CPM / TPM)
+
+    :param exp_df: samples by genes
+
+    :param log_base: the base of log transform
+
+    :param correct: plus 1 for avoiding log transform 0
+
+    :return: counts per million (CPM) or transcript per million (TPM)
+    """
+    exp = np.power(log_base, exp_df) - correct
+    # exp = exp.astype(np.float64)
+    cpm = exp / np.vstack(exp.sum(axis=1)) * 1e6
+    # cpm = cpm.astype(np.float32)
+    return cpm
+
+
+def non_log2log_cpm(input_file_path: Union[str, pd.DataFrame], result_file_path: str = None,
+                    transpose: bool = True, correct: int = 1):
+    """
+    Convert non-log expression data to log2(CPM + 1) or log2(TPM + 1)
+
+    :param input_file_path: non-log space expression file
+
+    :param result_file_path: file path, samples by genes
+
+    :param transpose: if input file is samples by genes, set to False, otherwise set to True
+
+    :param correct: plus 1 for avoiding log transform 0
+
+    :return: log2(CPM + 1) or save result to file
+    """
+
+    bulk_exp = pd.DataFrame()
+    if type(input_file_path) is str:
+        sep = get_sep(input_file_path)
+        bulk_exp = pd.read_csv(input_file_path, index_col=0, sep=sep)
+    elif type(input_file_path) is pd.DataFrame:
+        bulk_exp = input_file_path
+    if transpose:
+        bulk_exp = bulk_exp.T  # transpose to samples by genes
+    bulk_exp = non_log2cpm(bulk_exp)  # CPM/TPM
+    bulk_exp = np.log2(bulk_exp + correct)
+    if result_file_path is not None:
+        bulk_exp.round(3).to_csv(result_file_path)
+    else:
+        return bulk_exp.round(3)
+
+
+def non_log2cpm(exp_df, sum_exp=1e6) -> pd.DataFrame:
+    """
+    Normalize gene expression to CPM / TPM for non-log space
+
+    :param exp_df: gene expression profile in non-log space, sample by gene
+
+    :param sum_exp: sum of gene expression for each sample, default is 1e6
+
+    :return: counts per million (CPM) or transcript per million (TPM)
+    """
+    return exp_df / np.vstack(exp_df.sum(axis=1)) * sum_exp
+
+
+def get_corr(df_col1, df_col2, return_p_value=False) -> Union[float, tuple]:
+    """
+    calculate the correlation between two columns of dataframe
+    :param df_col1: series, column1
+    :param df_col2: series, column2
+    :param return_p_value: if return p-value
+    :return:
+    """
+    # correlation = np.corrcoef(df_col1, df_col2)
+    corr, p_value = stats.pearsonr(df_col1, df_col2)
+    if return_p_value:
+        return corr, p_value
+    else:
+        return corr
+    # return correlation[0, 1]
+
+
+def get_sep(file_path, comment: str = None):
+    """
+    check the separater (`\t` or `,`) in this file
+    :param file_path:
+    :param comment: if remove comment lines start with ''
+    :return:
+    """
+    sep = '\t'
+    with open(file_path, 'r') as f_handle:
+        # first_line = ''
+        while True:
+            first_line = f_handle.readline()
+            if comment is not None:
+                if first_line.startswith(comment):
+                    continue
+                else:
+                    break
+            break
+        if ',' in first_line:
+            sep = ','
+    return sep
+
+
+def read_marker_gene(marker_gene_file_path: str, include_t_cell: bool = False,
+                     include_cd8_nk_marker: bool = False, use_cancer_cell: bool = False,
+                     add_top_corr_gene: bool = False, corr_mean: bool = False) -> dict:
+    """
+    read marker genes for each cell type
+    :param marker_gene_file_path: file path of selected marker genes for each cell type
+    :param include_t_cell: if include the marker genes of T Cells for both CD4 and CD8 T
+    :param include_cd8_nk_marker: if remain "CD8 T / NK" marker genes
+    :param use_cancer_cell: if use "Cancer Cells" to replace "Epithelial Cells"
+    :param add_top_corr_gene: add top correlated genes from the corr between cell fraction and gene expression value
+    :param corr_mean: only two genes for CD4 T Cells and two genes for B Cells, others are same as core_marker
+    :return: a dict of cell type to marker genes, {'': []}
+    """
+    cell_type2marker = {}
+    marker_gene = pd.read_csv(marker_gene_file_path)
+    if 'corr_mean' in marker_gene.columns and corr_mean:
+        marker_gene = marker_gene.loc[marker_gene['corr_mean'] == 1, :].copy()
+    if 'core_marker' in marker_gene.columns:
+        if add_top_corr_gene:
+            marker_gene = marker_gene.loc[marker_gene['core_marker'].isin([1, 2]), :].copy()
+        else:
+            marker_gene = marker_gene.loc[marker_gene['core_marker'] == 1, :].copy()
+        if not include_cd8_nk_marker:
+            marker_gene = marker_gene.loc[marker_gene['cell_type'] != 'CD8 T / NK', :].copy()
+    cell_types = sorted(marker_gene['cell_type'].unique())
+    for ct in cell_types:
+        if include_t_cell:
+            cell_type2marker[ct] = list(marker_gene.loc[marker_gene['cell_type'] == ct, 'marker_gene'].unique())
+        else:
+            if ct != 'T Cells':
+                cell_type2marker[ct] = list(marker_gene.loc[marker_gene['cell_type'] == ct, 'marker_gene'].unique())
+    if include_cd8_nk_marker and cell_type2marker.get('CD8 T / NK', ''):
+        cell_type2marker['NK'] += cell_type2marker['CD8 T / NK']
+        cell_type2marker['CD8 T'] += cell_type2marker['CD8 T / NK']
+    if use_cancer_cell and 'Epithelial Cells' in cell_type2marker:
+        cell_type2marker['Cancer Cells'] = cell_type2marker['Epithelial Cells']
+        del cell_type2marker['Epithelial Cells']
+    return cell_type2marker
+
+
+def cal_exp_by_gene_list(exp_df, gene_list, min_exp_value=0, method='mean'):
+    """
+    calculate mean expression (or max) of a gene list (for single cell type)
+    :param exp_df: sample by gene, usually in CPM / TPM
+    :param gene_list: a list of genes which all are included in exp_df
+    :param min_exp_value: min mean expression of the gene list
+    :param method: mean or max
+    :return: mean or max expression value of marker genes for each sample
+    """
+    for gene in gene_list:
+        if gene not in exp_df.columns:
+            raise KeyError(f'Gene {gene} not include in exp_df')
+    current_exp = exp_df.loc[:, gene_list].copy()
+    if method == 'mean':
+        current_value = current_exp.mean(axis=1)
+    elif method == 'max':
+        current_value = current_exp.max(axis=1)
+    else:
+        raise KeyError('Only "mean" or "max" allowed')
+    current_value[current_value < min_exp_value] = min_exp_value
+    if exp_df.shape[0] == 1:
+        return round(float(current_value), 3)  # float
+    return current_value.round(3)  # pd.Series
+
+
+def save_key_params(all_vars: dict, save_to_file_path=None):
+    if save_to_file_path is None:
+        k_params_path = os.path.join(all_vars['result_dir'], 'key_parames.txt')
+    else:
+        k_params_path = save_to_file_path
+    if not os.path.exists(k_params_path):
+        key_paths = ['result_dir', 'merged_sc_dataset_file_path', 'simu_bulk_exp_dir', 'generated_sc_dataset_dir',
+                     'test_set_dir', 'tcga_data_dir', 'cancer_purity_file_path', 'marker_gene_file_path',
+                     'pre_trained_model_dir', 'pred_cell_frac_tcga_dir']
+        model_names = ['DeSide']
+        log_file_path = all_vars.get('log_file_path', '')
+        hyper_params = all_vars['deside_parameters']
+        other_params = ['all_cell_types', 'dataset2parameters', 'cd4_high_in_cd8', 'n_base',
+                        'total_cell_number', 'removed_cell_types', 'merge_t_cell', 'filter_simulated_bulk_cell',
+                        'remove_cancer_cell_when_training', 'one_minus_alpha', 'remove_cancer_cell']
+        key_paths_dict = {k: all_vars[k] for k in key_paths if k in all_vars}
+        other_params_dict = {k: all_vars[k] for k in other_params if k in all_vars}
+
+        all_key_params = {'model_names': model_names, 'key_paths_dict': key_paths_dict, 'hyper_params': hyper_params,
+                          'other_params': other_params_dict, 'key_params_path': k_params_path,
+                          'log_file_path': log_file_path}
+        with open(k_params_path, 'w', encoding='utf-8') as f:
+            json.dump(all_key_params, f, ensure_ascii=False, indent=4)
+
+
+def print_msg(p_str, log_file_path=None):
+    print()
+    current_info = f'---->>> {p_str} <<<----'
+    current_time = time.ctime()
+    print(current_info)
+    print(current_time)
+    if log_file_path is not None:
+        with open(log_file_path, 'a') as f_handle:
+            f_handle.write(current_info + '\n')
+            f_handle.write(current_time + '\n')
+            f_handle.write('\n')
+
+
+def read_xy(a: Union[str, pd.DataFrame], xy='cell_frac') -> pd.DataFrame:
+    """
+    read cell fraction or bulk expression
+    :param a: a file path or a DataFrame
+    :param xy: cell_frac or bulk_exp, only for .h5ad file
+    """
+    if (type(a) == str) and ('.h5ad' in a):
+        raw_data = read_data_from_h5ad(a)
+        exp = raw_data[xy]
+    else:
+        exp = read_df(a)
+    return exp
+
+
+def cal_corr_gene_exp_with_cell_frac(gene_exp: pd.DataFrame, cell_frac: pd.DataFrame,
+                                     result_file_path=None, filtered_by_corr: float = None,
+                                     filter_by_num: int = None):
+    """
+    calculate correlation between gene expression values and cell fractions for each cell type
+    :param gene_exp: non-log space, tpm/cpm, samples by genes
+    :param cell_frac: samples by cell types
+    :param result_file_path:
+    :param filtered_by_corr: threshold of correlation, only keep genes with higher corr than this value
+    :param filter_by_num: the max number of genes to keep for each cell type
+    :return: correlation, genes by cell types, filtered or all gene list
+    """
+    if not os.path.exists(result_file_path):
+        _, n_cell_type = cell_frac.shape
+        _, n_gene = gene_exp.shape
+        print(f'The shape of cell_frac: {cell_frac.shape}')
+        print(f'The shape of gene_exp: {gene_exp.shape}')
+        corr = np.corrcoef(cell_frac.values, gene_exp.values, rowvar=False)
+        corr_df = pd.DataFrame(data=corr[:n_cell_type, n_cell_type:].T,
+                               columns=cell_frac.columns, index=gene_exp.columns)
+    else:
+        print(f'Previous correlation file will be used: {result_file_path}')
+        corr_df = pd.read_csv(result_file_path, index_col=0)
+    if (filtered_by_corr is not None) and (filter_by_num is not None):
+        for cell_type in corr_df.columns:
+            if corr_df.loc[corr_df[cell_type] >= filtered_by_corr, cell_type].shape[0] > filter_by_num:
+                corr_df2 = corr_df.sort_values(by=[cell_type], ascending=False)
+                # set to 0 if there are too many high corr genes for the cell fraction of this cell type
+                corr_df.loc[corr_df.index.isin(corr_df2.iloc[filter_by_num:, :].index), cell_type] = 0
+        corr_df[f'n_at_least_one'] = np.sum(corr_df >= filtered_by_corr, axis=1)
+    elif filtered_by_corr is not None:
+        corr_df[f'n_at_least_one'] = np.sum(corr_df >= filtered_by_corr, axis=1)
+    elif filter_by_num is not None:
+        for cell_type in corr_df.columns:
+            corr_df2 = corr_df.sort_values(by=[cell_type], ascending=False)
+            # set to 0 if there are too many genes than filter_by_num of this cell type
+            corr_df.loc[corr_df.index.isin(corr_df2.iloc[filter_by_num:, :].index), cell_type] = 0
+        corr_df[f'n_at_least_one'] = np.sum(corr_df > 0, axis=1)
+    if (filtered_by_corr is not None) or (filter_by_num is not None):
+        corr_df_filtered = corr_df.loc[corr_df[f'n_at_least_one'] >= 1,
+                                       [i for i in corr_df.columns if i != 'n_at_least_one']].copy()
+        corr_df_filtered.to_csv(result_file_path, float_format='%g')
+        return corr_df_filtered
+    else:
+        corr_df.to_csv(result_file_path, float_format='%g')
+        return corr_df
+
+
+def read_df(df_file: Union[str, pd.DataFrame, np.ndarray]) -> Union[pd.DataFrame, np.ndarray]:
+    """
+    check the type of df_file
+    - if df_file is a file path, read this file
+    - if df_file is a DataFrame, return directly
+    """
+    if type(df_file) == str:  # the file path of current file
+        sep = get_sep(df_file)  # separated by '\t' or ','
+        df = pd.read_csv(df_file, index_col=0, sep=sep)
+    elif type(df_file) == pd.DataFrame:
+        return df_file  # return DataFrame directly
+    elif type(df_file) == np.ndarray:
+        return df_file  # return np.ndarray directly
+    else:
+        raise TypeError(
+            f'Only file path or pd.DataFrame was supported by df_file, {type(df_file)} is not supported.')
+    return df
+
+
+def aggregate_marker_gene_exp(exp_df: pd.DataFrame, marker_genes: dict = None,
+                              agg_methods: dict = None, return_ratio: bool = False,
+                              show_marker_gene: bool = True):
+    """
+    aggregate marker genes by the corresponding method in agg_methods (mean or max)
+    :param exp_df: a DataFrame of gene expression profiles, TPM, samples by genes
+    :param marker_genes:
+    :param agg_methods: aggregate multiple marker genes of a cell type by `mean` or `max`
+    :param return_ratio: return the ratio of aggregated marker gene exp for each cell type if True
+    :param show_marker_gene: whether printing marker genes or not
+    """
+    if marker_genes is None:
+        marker_genes = default_core_marker_genes.copy()
+    if agg_methods is None:
+        agg_methods = {}
+    for k, _ in marker_genes.items():
+        if k not in agg_methods:
+            agg_methods[k] = 'mean'
+
+    cell_type2marker_exp = {}
+    for ct, marker in marker_genes.items():
+        method = agg_methods[ct]
+        current_tpm = exp_df.loc[:, exp_df.columns.isin(marker)].copy()  # sample by gene
+        current_valid_marker = current_tpm.columns.to_list()
+        if len(current_valid_marker) > 0:
+            current_marker_str = ', '.join(current_valid_marker)
+            if show_marker_gene:
+                print(f'   Using {len(current_valid_marker)} marker genes for cell type {ct}: {current_marker_str}')
+            # cell_type2mean_exp[ct + '_marker_mean'] = current_tpm.mean(axis=0)
+            cell_type2marker_exp[ct + f'_marker_{method}'] = cal_exp_by_gene_list(exp_df=exp_df, method=method,
+                                                                                  gene_list=current_valid_marker,
+                                                                                  min_exp_value=1)
+        else:
+            Warning(f'No any marker genes in bulk cell TPM for cell type {ct}, '
+                    f'this cell type will be ignored in later analysis.')
+    marker_exp = pd.DataFrame.from_dict(cell_type2marker_exp, orient='columns')
+    if return_ratio:
+        return marker_exp / marker_exp.sum(axis=1).values.reshape(-1, 1)
+    else:
+        return marker_exp.round(3)
+
+
+def cal_marker_ratio(bulk_exp_file_path: str, marker_genes: dict, marker_ratio_file_path: str,
+                     agg_methods: dict = None, log_transformed: bool = True):
+    """
+    calculate marker ratio of each sample by gene expression values at large scale
+    :param bulk_exp_file_path: log2cpm1p or TPM/CPM
+    :param marker_genes:
+    :param log_transformed: whether log2cpm1p or TPM/CPM
+    :param marker_ratio_file_path: result file path
+    :param agg_methods: aggregate multiple marker genes of a cell type by `mean` or `max`
+    """
+    if not os.path.exists(marker_ratio_file_path):
+        # cell_frac = pd.read_csv(cell_frac_file_path, index_col=0)
+        cell_types = list(marker_genes.keys())  # cell types in current dataset
+        # only keep cell types in current dataset
+        marker_genes = {k: v for k, v in marker_genes.items() if k in cell_types}
+        # marker_ratio_dict = {}
+        # col_names = None
+
+        with open(marker_ratio_file_path, 'w') as write_file_handle:
+            csv_writer = csv.writer(write_file_handle)
+            csv_writer.writerow(['sample_id'] + list(marker_genes.keys()))
+        with pd.read_csv(bulk_exp_file_path, chunksize=1000, index_col=0) as f_handle:
+            for chunk in f_handle:
+                if 'cancer_type' in chunk.columns:
+                    chunk = chunk.drop(columns=['cancer_type'])
+                if log_transformed:
+                    current_exp = log_exp2cpm(chunk)  # convert log2cpm1p to CPM / TPM
+                else:
+                    current_exp = chunk
+                current_marker_ratio = aggregate_marker_gene_exp(exp_df=current_exp, marker_genes=marker_genes,
+                                                                 agg_methods=agg_methods, return_ratio=True)
+                current_marker_ratio.to_csv(marker_ratio_file_path, mode='a', header=False, float_format='%g')
+    else:
+        print(f'   Previous result has existed: {marker_ratio_file_path}')
+
+
+def get_cell_num(cell_type_frac, total_num=500):
+    """
+    calculate the number of cells to choose for each cell type based on the total number of cells
+    and fraction of each cell type
+    :param cell_type_frac: dataFrame
+        the fraction of each cell type, sum to 1 for each row, samples by cell types
+    :param total_num: the total number of cells contributing to one simulated RNA-seq sample
+    :return:
+    """
+    assert type(cell_type_frac) is pd.DataFrame
+    cell_num = cell_type_frac * total_num
+    if total_num == 1:  # assign 1 for all cell types for matrix multiplication
+        cell_num = cell_type_frac * 0 + 1
+    elif total_num == 0:
+        cell_num = np.ceil(cell_type_frac)  # assign 1 for the cell types with non-zero cell fractions
+    return cell_num.round(0).astype(int)
+
+
+def do_pca_analysis(exp_df, n_components=5, pca_result_fp=None, save_model: bool = False):
+    """
+    PCA analysis
+    :param exp_df:
+    :param n_components:
+    :param pca_result_fp:
+    :param save_model:
+    :return: fitted PCA model
+    """
+    if os.path.exists(pca_result_fp):
+        print(f'Loading PCA result from file: {pca_result_fp}')
+        pca = load(pca_result_fp)
+    else:
+        pca = PCA(n_components=n_components)
+        pca.fit(exp_df)
+        if save_model:
+            dump(pca, pca_result_fp)
+    return pca
+
+
+def do_umap_analysis(exp_df, n_components=5, n_neighbors=15, min_dist=0.1,
+                     umap_model_result_fp=None, save_model: bool = False):
+    """
+    t-SNE analysis
+    :param exp_df:
+    :param n_components:
+    :param n_neighbors:
+    :param min_dist:
+    :param umap_model_result_fp:
+    :param save_model:
+    :return:
+    """
+    if os.path.exists(umap_model_result_fp):
+        print(f'Loading UMAP result from file: {umap_model_result_fp}')
+        umap_model = load(umap_model_result_fp)
+    else:
+        umap_model = umap.UMAP(n_neighbors=n_neighbors, min_dist=min_dist, n_components=n_components)
+        umap_model.fit(exp_df)
+        if save_model:
+            dump(umap_model, umap_model_result_fp)
+    return umap_model
+
+
+def get_ccc(x, y):
+    # Concordance Correlation Coefficient(CCC), https://en.wikipedia.org/wiki/Concordance_correlation_coefficient
+    vx, cov_xy, cov_xy, vy = np.cov(x, y, bias=True).flatten()
+    mx, my = x.mean(), y.mean()
+    return 2*cov_xy / (vx + vy + (mx-my)**2)
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `DeSide-1.0.1/deside/utility/read_file.py` & `DeSide-1.0.2/deside/utility/read_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,332 +1,372 @@
-import os
-import sys
-import numpy as np
-import pandas as pd
-import anndata as an
-from tqdm import tqdm
-from typing import Union
-from scipy.sparse import csr_matrix
-from sklearn import preprocessing as pp
-from .pub_func import (log_exp2cpm, read_df, non_log2log_cpm, non_log2cpm,
-                       get_inx2cell_type, sorted_cell_types, log2_transform)
-
-
-class ReadH5AD(object):
-    """
-    read .h5ad file, usually the values are log2 transformed
-    """
-    def __init__(self, file_path: str, show_info: bool = False):
-        """
-        :param file_path: the file path of .h5ad file, samples by genes, log2cpm1p format
-        """
-        self.dataset = an.read_h5ad(file_path)
-        if show_info:
-            print(self.dataset)
-
-    def get_df(self, result_file_path: str = None, convert_to_tpm: bool = False,
-               scaling_by_sample: bool = False) -> pd.DataFrame:
-        """
-        convert to DataFrame, samples by genes, log space (log2cpm1p)
-        :param result_file_path:
-        :param convert_to_tpm: whether to convert log2cpm1p to TPM
-        :param scaling_by_sample: whether to scale the expression values of each sample to [0, 1] by 'min_max'
-        """
-        if type(self.dataset.X) == csr_matrix:
-            x_data = self.dataset.X.A.astype(np.float32)  # convert sparse matrix to dense matrix
-        else:
-            x_data = self.dataset.X.astype(np.float32)
-
-        if convert_to_tpm:
-            x_data = log_exp2cpm(x_data)
-        if scaling_by_sample:
-            scaler = pp.MinMaxScaler(feature_range=(0, 1), copy=True)
-            x_data = scaler.fit_transform(x_data.T).T
-
-        df = pd.DataFrame(data=x_data, index=self.dataset.obs.index,
-                          columns=self.dataset.var.index).round(3)
-        if result_file_path is not None:
-            df.to_csv(result_file_path, float_format='%.3f')
-        return df
-
-    def get_cell_fraction(self) -> Union[None, pd.DataFrame]:
-        if self.dataset.obs.shape[1] > 0:
-            return self.dataset.obs.round(3)
-        else:
-            print('   There is no cell fraction in this .h5ad file')
-            return None
-
-    def get_h5ad(self):
-        return self.dataset
-
-
-class ReadExp(object):
-    """
-    read gene expression file, and convert to specific format (TPM / CPM, log2cpm1p)
-    - TPM: transcript per million
-    - CPM: UMI reads per million (3' end sc-RNA seq), same as TPM in the full-length RNA-seq of bulk cells
-    - log_space: log2(CPM + 1), or log2(TPM + 1)
-    - non_log: non log space, could be normalized to TPM
-    Data from full-length protocols may benefit from normalization methods that take into account gene length
-    (e.g. Patelet al, 2014; Kowalczyket al,2015; Soneson & Robinson, 2018),
-    while 3' enrichment data do not.
-    A  commonly  used  normalization  method  for  full-length scRNA-seq data is TPM normalization (Liet al, 2009),
-    which comes from bulk RNA-seq analysis. (Luecken, M. D. & Theis, F. J., Mol. Syst. Biol. 15, e8746 (2019))
-    """
-    def __init__(self, exp_file, exp_type='TPM', transpose: bool = False):
-        """
-        :param exp_file: file path or DataFrame, samples by genes
-        :param exp_type: TPM / CPM, log_space, non_log
-        :param transpose: transpose if exp_file formed as genes (index) by samples (columns)
-        """
-        assert exp_type in ['TPM', 'CPM', 'log_space', 'non_log']
-        self.file_type = exp_type
-        self.exp = read_df(exp_file)
-        if transpose:
-            self.exp = self.exp.T
-        self.scaled_by_sample = False
-
-    def to_tpm(self):
-        if self.file_type == 'non_log':
-            self.exp = non_log2cpm(self.exp)
-        elif self.file_type == 'TPM' or self.file_type == 'CPM':
-            pass
-        elif self.file_type == 'log_space':
-            self.exp = log_exp2cpm(self.exp)
-        self.file_type = 'TPM'
-
-    def to_log2cpm1p(self):
-        if self.file_type != 'log_space':
-            self.exp = non_log2log_cpm(self.exp, transpose=False)
-        else:
-            print('   This file has already log2 transformed.')
-        self.file_type = 'log_space'
-
-    def get_file_type(self):
-        return self.file_type
-
-    def get_exp(self):
-        return self.exp.round(3)
-
-    def save(self, file_path, sep=',', transpose: bool = False):
-        if transpose:
-            self.exp = self.exp.T.copy()
-        self.exp.to_csv(file_path, sep=sep, float_format='%.3f')
-
-    def do_scaling(self):
-        """
-        Scaling by sample to [0, 1], same as Scaden
-        """
-        if not self.scaled_by_sample:
-            scaler = pp.MinMaxScaler(feature_range=(0, 1), copy=True)
-            x_scaled = scaler.fit_transform(self.exp.T).T  # scaling by column (sample), so T is needed here
-            self.scaled_by_sample = True
-            self.exp = pd.DataFrame(data=x_scaled, index=self.exp.index,
-                                    columns=self.exp.columns).round(3)
-        # return self.exp
-
-    def do_scaling_by_constant(self, divide_by=20):
-        """
-        Scaling by dividing a constant in log space, so all expression values are in [0, 1)
-        """
-        if self.file_type != 'log_space':
-            raise ValueError('   This file is not in log space')
-        if np.any(self.exp.values > 1.0):
-            self.exp = self.exp / divide_by
-
-    def align_with_gene_list(self, gene_list: list = None, fill_not_exist=False):
-        common_genes = [i for i in gene_list if i in self.exp.columns]
-        not_exist_in_exp = [i for i in gene_list if i not in common_genes]
-        removed_genes = [i for i in self.exp.columns if i not in common_genes]
-        print(f'{len(common_genes)} common genes will be used, {len(removed_genes)} genes will be removed.')
-        self.exp = self.exp.loc[:, common_genes].copy()
-        if fill_not_exist and (len(not_exist_in_exp) != 0):
-            print(f'{len(not_exist_in_exp)} genes are not in current dataset, 0 will be filled')
-            _not_exist_exp = pd.DataFrame(np.zeros((self.exp.shape[0], len(not_exist_in_exp))), index=self.exp.index,
-                                          columns=not_exist_in_exp)
-            self.exp = pd.concat([self.exp, _not_exist_exp], axis=1)
-            self.exp = self.exp.loc[:, gene_list].copy()
-        if self.file_type == 'log_space':  # scaling to TPM after alignment
-            self.to_tpm()
-            self.to_log2cpm1p()
-        else:
-            self.file_type = 'non_log'
-            self.to_tpm()
-
-
-class TrainingDatasetLoader(object):
-    def __init__(self, pos_data_path, neg_data_path):
-
-        print("Opening {} and {}".format(pos_data_path, neg_data_path))
-        sys.stdout.flush()
-
-        self.cache_pos = ReadH5AD(pos_data_path)
-        self.cache_neg = ReadH5AD(neg_data_path)
-
-        print("Loading data into memory...")
-        sys.stdout.flush()
-        self.gep_pos = self.cache_pos.get_df()  # log space, samples by genes
-        self.cell_prop_pos = self.cache_pos.get_cell_fraction()  # samples by cell types
-        self.gep_neg = self.cache_neg.get_df()
-        self.cell_prop_neg = self.cache_neg.get_cell_fraction()
-
-        # self.images = self.cache['images'][:]
-        # self.labels = self.cache['labels'][:].astype(np.float32)
-        # self.image_dims = self.images.shape
-        # n_train_samples = self.cell_prop_pos.shape[0] + self.cell_prop_neg.shape[0]
-
-        # self.train_inds = np.random.permutation(np.arange(n_train_samples))
-
-        self.pos_train_inds = np.random.permutation(np.arange(self.cell_prop_pos.shape[0]))
-        self.neg_train_inds = np.random.permutation(np.arange(self.cell_prop_neg.shape[0]))
-
-    def get_train_size(self):
-        return self.cell_prop_pos.shape[0] + self.cell_prop_neg.shape[0]
-
-    def get_n_genes(self):
-        # the number of genes in each GEP
-        return self.gep_pos.shape[1]
-
-    def get_n_cell_types(self):
-        return self.cell_prop_pos.shape[1]
-
-    # def get_train_steps_per_epoch(self, batch_size, factor=10):
-    #     return self.get_train_size()//factor//batch_size
-
-    def get_batch(self, n, only_faces=False, p_pos=None, p_neg=None):
-        if only_faces:
-            selected_inds = np.random.choice(self.pos_train_inds, size=n, replace=False, p=p_pos)
-            train_gep = self.gep_pos.iloc[selected_inds, :].copy()
-            train_cell_prop = self.cell_prop_pos.iloc[selected_inds, :].copy()
-        else:
-            # selected_pos_inds = tfp.distributions.Multinomial(total_count=n//2, logits=self.pos_train_inds, )
-            selected_pos_inds = np.random.choice(self.pos_train_inds, size=n//2, replace=False, p=p_pos)
-            selected_neg_inds = np.random.choice(self.neg_train_inds, size=n//2, replace=False, p=p_neg)
-            t_gep1 = self.gep_pos.iloc[selected_pos_inds, :].copy()
-            t_cell_prop1 = self.cell_prop_pos.iloc[selected_pos_inds, :].copy()
-            t_gep2 = self.gep_neg.iloc[selected_neg_inds, :].copy()
-            t_cell_prop2 = self.cell_prop_neg.iloc[selected_neg_inds, :].copy()
-            train_gep = pd.concat([t_gep1, t_gep2])
-            train_cell_prop = pd.concat([t_cell_prop1, t_cell_prop2])
-
-        return train_gep.values, train_cell_prop.values
-
-    # def get_n_most_prob_faces(self, prob, n):
-    #     idx = np.argsort(prob)[::-1]
-    #     most_prob_inds = self.pos_train_inds[idx[:10*n:10]]
-    #     return (self.images[most_prob_inds,...]/255.).astype(np.float32)
-
-    def get_all_pos(self) -> np.ndarray:
-        return self.gep_pos.values
-
-
-def read_single_cell_type_dataset(sct_dataset_file_path: str, latent_z_nn_info_file: Union[str, pd.DataFrame] = None):
-    """
-    positive samples of SCT (single cell type), generated by SingleCellTypeGEPGenerator
-    :param sct_dataset_file_path: the file path of GEPs for single cell type (SCT), positive samples
-    :param latent_z_nn_info_file: neighbor information of latent z for all samples, used for QC
-    """
-    sct_dataset_obj = ReadH5AD(sct_dataset_file_path)
-    sct_dataset_df = sct_dataset_obj.get_df(convert_to_tpm=True)
-    inx2cell_type = get_inx2cell_type()
-    if (latent_z_nn_info_file is not None) and os.path.exists(latent_z_nn_info_file):
-        latent_z_nn_info = read_df(latent_z_nn_info_file)
-        latent_z_nn_info = \
-            latent_z_nn_info.loc[
-                (latent_z_nn_info['class'] != -1) &  # only positive samples
-                (latent_z_nn_info['n_neighbor_class'] == 1) &  # all neighbors belong to the same cell type
-                (latent_z_nn_info['class'] == latent_z_nn_info['pred_class']),  # predicted class is same as true class
-                ['class']].copy()
-        latent_z_nn_info['cell_type'] = latent_z_nn_info['class'].map(lambda x: inx2cell_type[x])
-        sct_dataset_obs = latent_z_nn_info.copy()
-    else:
-        sct_dataset_obs = sct_dataset_obj.get_cell_fraction()
-        sct_dataset_obs['class'] = sct_dataset_obs.values.argmax(axis=1)
-        sct_dataset_obs['cell_type'] = sct_dataset_obs['class'].map(lambda x: inx2cell_type[x])
-    return sct_dataset_obs, sct_dataset_df
-
-
-def read_sct_dataset(sct_files: list, scaling_by_constant=False):
-    """
-    combine all sct dataset together
-    :param sct_files: a list of file paths for all used SCT datasets, .h5ad format
-    :param scaling_by_constant:
-    :return:
-    """
-    sct_exp_list, sct_info_list = [], []
-    for file_path in sct_files:
-        sct_obj = ReadH5AD(file_path)
-        sct_df = sct_obj.get_df().astype(np.float32)
-        sct_cell_frac = sct_obj.get_cell_fraction()
-        if scaling_by_constant:
-            sct_obj = ReadExp(sct_df, exp_type='log_space')
-            sct_obj.do_scaling_by_constant()
-            sct_df = sct_obj.get_exp()
-        sct_exp_list.append(sct_df)
-        sct_info_list.append(sct_cell_frac)
-    sct_exp = pd.concat(sct_exp_list, axis=0)
-    sct_info = pd.concat(sct_info_list, axis=0)
-    sample2inx_sct_ds = {sample_id: i for i, sample_id in enumerate(sct_info.index.to_list())}
-    assert len(sample2inx_sct_ds) == sct_exp.shape[0], 'Duplicated sample ids are not allowed.'
-    return sct_exp, sample2inx_sct_ds
-
-
-def read_ds_two_parts(dataset2info: dict, dataset_name: str, sample2inx_sct_ds: dict, scaling_by_constant=False):
-    """
-
-    :param dataset2info:
-    :param dataset_name:
-    :param sample2inx_sct_ds: mapping sample id to index in SCT dataset (used in simulating bulk GEPs)
-    :param scaling_by_constant:
-    :return:
-    """
-    x_list, y_list = [], []
-    col_name_sc_id = [f'{_}_sc_inx' for _ in sorted_cell_types]
-    for k, v in dataset2info.items():
-        path_to_exp_data = v['h5ad_file_path']
-        dataset_type = v['dataset_type']
-        x_obj = ReadH5AD(path_to_exp_data)
-        cell_prop = x_obj.get_cell_fraction()
-        x_df = x_obj.get_df().astype(np.float32)
-        if dataset_type == 'sct':
-            cell_prop[col_name_sc_id] = 0
-            for r_id, _ in tqdm(cell_prop.iterrows()):
-                cell_prop.loc[r_id, col_name_sc_id] = sample2inx_sct_ds[r_id]
-        else:
-            path_to_sc_id = os.path.join(v['file_dir'], v['sampled_sc_id_file'])
-            sc_ids = pd.read_csv(path_to_sc_id, index_col=[0, 1])
-            r_id2sc_inx = {}
-            for r_id, row in tqdm(cell_prop.iterrows()):
-                q_inx = list(zip([r_id] * len(sorted_cell_types), sorted_cell_types))
-                selected_sc_id = sc_ids.loc[q_inx, 'selected_cell_id'].to_list()
-                r_id2sc_inx[r_id] = [sample2inx_sct_ds[_] for _ in selected_sc_id]
-            r_id2sc_inx_df = pd.DataFrame.from_dict(r_id2sc_inx, orient='index', columns=col_name_sc_id)
-            cell_prop = cell_prop.merge(r_id2sc_inx_df, left_index=True, right_index=True)
-            # cell_prop.loc[r_id, col_name_sc_id] =
-        if scaling_by_constant:
-            x_obj = ReadExp(x_df, exp_type='log_space')
-            x_obj.do_scaling_by_constant()
-            x_df = x_obj.get_exp()
-        x_list.append(x_df.copy())
-        y_list.append(cell_prop.copy())
-    x = pd.concat(x_list)
-    y = pd.concat(y_list)
-
-    print(f'   There are {x.shape[0]} samples in {dataset_name}...')
-    return x, y
-
-
-def align_with_gene_list(dataset_file: Union[pd.DataFrame, str], gene_list, gene_exp_type) -> pd.DataFrame:
-    """
-
-    :param dataset_file: file path or DataFrame, samples by genes
-    :param gene_list:
-    :param gene_exp_type: TPM / CPM, log_space, non_log
-    :return: log2tpm1p
-    """
-    dataset = ReadExp(dataset_file, exp_type=gene_exp_type).get_exp()
-    gene_not_in_ds = [i for i in gene_list if i not in dataset.columns]
-    dataset[gene_not_in_ds] = 0  # set expression values to 0 if a gene not exists
-    dataset = dataset.loc[:, gene_list].copy()  # remove genes not contain in gene_list
-    dataset = log_exp2cpm(dataset)
-    dataset = log2_transform(dataset)
-    return dataset
+import os
+import sys
+import numpy as np
+import pandas as pd
+import anndata as an
+from tqdm import tqdm
+from typing import Union
+from scipy.sparse import csr_matrix
+from sklearn import preprocessing as pp
+from .pub_func import (log_exp2cpm, read_df, non_log2log_cpm, non_log2cpm,
+                       get_inx2cell_type, sorted_cell_types, log2_transform)
+
+
+class ReadH5AD(object):
+    """
+    Read .h5ad file, usually the values are log2 transformed
+
+    :param file_path: the file path of .h5ad file, samples by genes, log2cpm1p format
+    :param show_info: whether to show the information of the dataset after reading
+    """
+    def __init__(self, file_path: str, show_info: bool = False):
+        """
+        """
+        self.dataset = an.read_h5ad(file_path)
+        if show_info:
+            print(self.dataset)
+
+    def get_df(self, result_file_path: str = None, convert_to_tpm: bool = False,
+               scaling_by_sample: bool = False) -> pd.DataFrame:
+        """
+        Convert to DataFrame, samples by genes, log space (log2cpm1p)
+
+        :param result_file_path:
+        :param convert_to_tpm: whether to convert log2cpm1p to TPM
+        :param scaling_by_sample: whether to scale the expression values of each sample to [0, 1] by 'min_max'
+        """
+        if type(self.dataset.X) == csr_matrix:
+            x_data = self.dataset.X.A.astype(np.float32)  # convert sparse matrix to dense matrix
+        else:
+            x_data = self.dataset.X.astype(np.float32)
+
+        if convert_to_tpm:
+            x_data = log_exp2cpm(x_data)
+        if scaling_by_sample:
+            scaler = pp.MinMaxScaler(feature_range=(0, 1), copy=True)
+            x_data = scaler.fit_transform(x_data.T).T
+
+        df = pd.DataFrame(data=x_data, index=self.dataset.obs.index,
+                          columns=self.dataset.var.index).round(3)
+        if result_file_path is not None:
+            df.to_csv(result_file_path, float_format='%.3f')
+        return df
+
+    def get_cell_fraction(self) -> Union[None, pd.DataFrame]:
+        """
+        Get cell fraction, cells by cell types
+        """
+        if self.dataset.obs.shape[1] > 0:
+            return self.dataset.obs.round(3)
+        else:
+            print('   There is no cell fraction in this .h5ad file')
+            return None
+
+    def get_h5ad(self):
+        """
+        Get the .h5ad file
+        """
+        return self.dataset
+
+
+class ReadExp(object):
+    """
+    Read gene expression file, and convert to specific format (TPM / CPM, log2cpm1p)
+
+    - TPM: transcript per million
+
+    - CPM: UMI reads per million (3' end sc-RNA seq), same as TPM in the full-length RNA-seq of bulk cells
+
+    - log_space: log2(CPM + 1), or log2(TPM + 1)
+
+    - non_log: non log space, could be normalized to TPM
+
+    - Data from full-length protocols may benefit from normalization methods that take into account gene length
+      (e.g. Patelet al, 2014; Kowalczyket al,2015; Soneson & Robinson, 2018), while 3' enrichment data do not.
+
+    - A commonly used normalization method for full-length scRNA-seq data is TPM normalization (Liet al, 2009),
+      which comes from bulk RNA-seq analysis. (Luecken, M. D. & Theis, F. J., Mol. Syst. Biol. 15, e8746 (2019))
+
+    :param exp_file: file path or DataFrame, samples by genes
+    :param exp_type: TPM / CPM, log_space, non_log
+    :param transpose: transpose if exp_file formed as genes (index) by samples (columns)
+    """
+    def __init__(self, exp_file, exp_type='TPM', transpose: bool = False):
+        """
+        """
+        assert exp_type in ['TPM', 'CPM', 'log_space', 'non_log']
+        self.file_type = exp_type
+        self.exp = read_df(exp_file)
+        if transpose:
+            self.exp = self.exp.T
+        self.scaled_by_sample = False
+
+    def to_tpm(self):
+        """
+        Convert to TPM
+        """
+        if self.file_type == 'non_log':
+            self.exp = non_log2cpm(self.exp)
+        elif self.file_type == 'TPM' or self.file_type == 'CPM':
+            pass
+        elif self.file_type == 'log_space':
+            self.exp = log_exp2cpm(self.exp)
+        self.file_type = 'TPM'
+
+    def to_log2cpm1p(self):
+        """
+        Convert to log2(TPM + 1)
+        """
+        if self.file_type != 'log_space':
+            self.exp = non_log2log_cpm(self.exp, transpose=False)
+        else:
+            print('   This file has already log2 transformed.')
+        self.file_type = 'log_space'
+
+    def get_file_type(self) -> str:
+        """
+        Get the file type
+        """
+        return self.file_type
+
+    def get_exp(self) -> pd.DataFrame:
+        """
+        Get the expression matrix
+        """
+        return self.exp.round(3)
+
+    def save(self, file_path, sep=',', transpose: bool = False):
+        """
+        Save the expression matrix to file
+
+        :param file_path: file path
+        :param sep: separator, default is ','
+        :param transpose: transpose index and columns
+        """
+        if transpose:
+            self.exp = self.exp.T.copy()
+        self.exp.to_csv(file_path, sep=sep, float_format='%.3f')
+
+    def do_scaling(self):
+        """
+        Scaling GEPs by sample to [0, 1], same as Scaden
+        """
+        if not self.scaled_by_sample:
+            scaler = pp.MinMaxScaler(feature_range=(0, 1), copy=True)
+            x_scaled = scaler.fit_transform(self.exp.T).T  # scaling by column (sample), so T is needed here
+            self.scaled_by_sample = True
+            self.exp = pd.DataFrame(data=x_scaled, index=self.exp.index,
+                                    columns=self.exp.columns).round(3)
+        # return self.exp
+
+    def do_scaling_by_constant(self, divide_by=20):
+        """
+        Scaling GEPs by dividing a constant in log space, so all expression values are in [0, 1)
+        """
+        if self.file_type != 'log_space':
+            raise ValueError('   This file is not in log space')
+        if np.any(self.exp.values > 1.0):
+            self.exp = self.exp / divide_by
+
+    def align_with_gene_list(self, gene_list: list = None, fill_not_exist=False):
+        """
+        Align the expression matrix with a gene list
+
+        :param gene_list: gene list
+        :param fill_not_exist: fill 0 if gene not exist in the expression matrix when True
+        """
+        common_genes = [i for i in gene_list if i in self.exp.columns]
+        not_exist_in_exp = [i for i in gene_list if i not in common_genes]
+        removed_genes = [i for i in self.exp.columns if i not in common_genes]
+        print(f'{len(common_genes)} common genes will be used, {len(removed_genes)} genes will be removed.')
+        self.exp = self.exp.loc[:, common_genes].copy()
+        if fill_not_exist and (len(not_exist_in_exp) != 0):
+            print(f'{len(not_exist_in_exp)} genes are not in current dataset, 0 will be filled')
+            _not_exist_exp = pd.DataFrame(np.zeros((self.exp.shape[0], len(not_exist_in_exp))), index=self.exp.index,
+                                          columns=not_exist_in_exp)
+            self.exp = pd.concat([self.exp, _not_exist_exp], axis=1)
+            self.exp = self.exp.loc[:, gene_list].copy()
+        if self.file_type == 'log_space':  # scaling to TPM after alignment
+            self.to_tpm()
+            self.to_log2cpm1p()
+        else:
+            self.file_type = 'non_log'
+            self.to_tpm()
+
+
+class TrainingDatasetLoader(object):
+    def __init__(self, pos_data_path, neg_data_path):
+
+        print("Opening {} and {}".format(pos_data_path, neg_data_path))
+        sys.stdout.flush()
+
+        self.cache_pos = ReadH5AD(pos_data_path)
+        self.cache_neg = ReadH5AD(neg_data_path)
+
+        print("Loading data into memory...")
+        sys.stdout.flush()
+        self.gep_pos = self.cache_pos.get_df()  # log space, samples by genes
+        self.cell_prop_pos = self.cache_pos.get_cell_fraction()  # samples by cell types
+        self.gep_neg = self.cache_neg.get_df()
+        self.cell_prop_neg = self.cache_neg.get_cell_fraction()
+
+        # self.images = self.cache['images'][:]
+        # self.labels = self.cache['labels'][:].astype(np.float32)
+        # self.image_dims = self.images.shape
+        # n_train_samples = self.cell_prop_pos.shape[0] + self.cell_prop_neg.shape[0]
+
+        # self.train_inds = np.random.permutation(np.arange(n_train_samples))
+
+        self.pos_train_inds = np.random.permutation(np.arange(self.cell_prop_pos.shape[0]))
+        self.neg_train_inds = np.random.permutation(np.arange(self.cell_prop_neg.shape[0]))
+
+    def get_train_size(self):
+        return self.cell_prop_pos.shape[0] + self.cell_prop_neg.shape[0]
+
+    def get_n_genes(self):
+        # the number of genes in each GEP
+        return self.gep_pos.shape[1]
+
+    def get_n_cell_types(self):
+        return self.cell_prop_pos.shape[1]
+
+    # def get_train_steps_per_epoch(self, batch_size, factor=10):
+    #     return self.get_train_size()//factor//batch_size
+
+    def get_batch(self, n, only_faces=False, p_pos=None, p_neg=None):
+        if only_faces:
+            selected_inds = np.random.choice(self.pos_train_inds, size=n, replace=False, p=p_pos)
+            train_gep = self.gep_pos.iloc[selected_inds, :].copy()
+            train_cell_prop = self.cell_prop_pos.iloc[selected_inds, :].copy()
+        else:
+            # selected_pos_inds = tfp.distributions.Multinomial(total_count=n//2, logits=self.pos_train_inds, )
+            selected_pos_inds = np.random.choice(self.pos_train_inds, size=n//2, replace=False, p=p_pos)
+            selected_neg_inds = np.random.choice(self.neg_train_inds, size=n//2, replace=False, p=p_neg)
+            t_gep1 = self.gep_pos.iloc[selected_pos_inds, :].copy()
+            t_cell_prop1 = self.cell_prop_pos.iloc[selected_pos_inds, :].copy()
+            t_gep2 = self.gep_neg.iloc[selected_neg_inds, :].copy()
+            t_cell_prop2 = self.cell_prop_neg.iloc[selected_neg_inds, :].copy()
+            train_gep = pd.concat([t_gep1, t_gep2])
+            train_cell_prop = pd.concat([t_cell_prop1, t_cell_prop2])
+
+        return train_gep.values, train_cell_prop.values
+
+    # def get_n_most_prob_faces(self, prob, n):
+    #     idx = np.argsort(prob)[::-1]
+    #     most_prob_inds = self.pos_train_inds[idx[:10*n:10]]
+    #     return (self.images[most_prob_inds,...]/255.).astype(np.float32)
+
+    def get_all_pos(self) -> np.ndarray:
+        return self.gep_pos.values
+
+
+def read_single_cell_type_dataset(sct_dataset_file_path: str, latent_z_nn_info_file: Union[str, pd.DataFrame] = None):
+    """
+    positive samples of SCT (single cell type), generated by SingleCellTypeGEPGenerator
+    :param sct_dataset_file_path: the file path of GEPs for single cell type (SCT), positive samples
+    :param latent_z_nn_info_file: neighbor information of latent z for all samples, used for QC
+    """
+    sct_dataset_obj = ReadH5AD(sct_dataset_file_path)
+    sct_dataset_df = sct_dataset_obj.get_df(convert_to_tpm=True)
+    inx2cell_type = get_inx2cell_type()
+    if (latent_z_nn_info_file is not None) and os.path.exists(latent_z_nn_info_file):
+        latent_z_nn_info = read_df(latent_z_nn_info_file)
+        latent_z_nn_info = \
+            latent_z_nn_info.loc[
+                (latent_z_nn_info['class'] != -1) &  # only positive samples
+                (latent_z_nn_info['n_neighbor_class'] == 1) &  # all neighbors belong to the same cell type
+                (latent_z_nn_info['class'] == latent_z_nn_info['pred_class']),  # predicted class is same as true class
+                ['class']].copy()
+        latent_z_nn_info['cell_type'] = latent_z_nn_info['class'].map(lambda x: inx2cell_type[x])
+        sct_dataset_obs = latent_z_nn_info.copy()
+    else:
+        sct_dataset_obs = sct_dataset_obj.get_cell_fraction()
+        sct_dataset_obs['class'] = sct_dataset_obs.values.argmax(axis=1)
+        sct_dataset_obs['cell_type'] = sct_dataset_obs['class'].map(lambda x: inx2cell_type[x])
+    return sct_dataset_obs, sct_dataset_df
+
+
+def read_sct_dataset(sct_files: list, scaling_by_constant=False):
+    """
+    combine all sct dataset together
+    :param sct_files: a list of file paths for all used SCT datasets, .h5ad format
+    :param scaling_by_constant:
+    :return:
+    """
+    sct_exp_list, sct_info_list = [], []
+    for file_path in sct_files:
+        sct_obj = ReadH5AD(file_path)
+        sct_df = sct_obj.get_df().astype(np.float32)
+        sct_cell_frac = sct_obj.get_cell_fraction()
+        if scaling_by_constant:
+            sct_obj = ReadExp(sct_df, exp_type='log_space')
+            sct_obj.do_scaling_by_constant()
+            sct_df = sct_obj.get_exp()
+        sct_exp_list.append(sct_df)
+        sct_info_list.append(sct_cell_frac)
+    sct_exp = pd.concat(sct_exp_list, axis=0)
+    sct_info = pd.concat(sct_info_list, axis=0)
+    sample2inx_sct_ds = {sample_id: i for i, sample_id in enumerate(sct_info.index.to_list())}
+    assert len(sample2inx_sct_ds) == sct_exp.shape[0], 'Duplicated sample ids are not allowed.'
+    return sct_exp, sample2inx_sct_ds
+
+
+def read_ds_two_parts(dataset2info: dict, dataset_name: str, sample2inx_sct_ds: dict, scaling_by_constant=False):
+    """
+
+    :param dataset2info:
+    :param dataset_name:
+    :param sample2inx_sct_ds: mapping sample id to index in SCT dataset (used in simulating bulk GEPs)
+    :param scaling_by_constant:
+    :return:
+    """
+    x_list, y_list = [], []
+    col_name_sc_id = [f'{_}_sc_inx' for _ in sorted_cell_types]
+    for k, v in dataset2info.items():
+        path_to_exp_data = v['h5ad_file_path']
+        dataset_type = v['dataset_type']
+        x_obj = ReadH5AD(path_to_exp_data)
+        cell_prop = x_obj.get_cell_fraction()
+        x_df = x_obj.get_df().astype(np.float32)
+        if dataset_type == 'sct':
+            cell_prop[col_name_sc_id] = 0
+            for r_id, _ in tqdm(cell_prop.iterrows()):
+                cell_prop.loc[r_id, col_name_sc_id] = sample2inx_sct_ds[r_id]
+        else:
+            path_to_sc_id = os.path.join(v['file_dir'], v['sampled_sc_id_file'])
+            sc_ids = pd.read_csv(path_to_sc_id, index_col=[0, 1])
+            r_id2sc_inx = {}
+            for r_id, row in tqdm(cell_prop.iterrows()):
+                q_inx = list(zip([r_id] * len(sorted_cell_types), sorted_cell_types))
+                selected_sc_id = sc_ids.loc[q_inx, 'selected_cell_id'].to_list()
+                r_id2sc_inx[r_id] = [sample2inx_sct_ds[_] for _ in selected_sc_id]
+            r_id2sc_inx_df = pd.DataFrame.from_dict(r_id2sc_inx, orient='index', columns=col_name_sc_id)
+            cell_prop = cell_prop.merge(r_id2sc_inx_df, left_index=True, right_index=True)
+            # cell_prop.loc[r_id, col_name_sc_id] =
+        if scaling_by_constant:
+            x_obj = ReadExp(x_df, exp_type='log_space')
+            x_obj.do_scaling_by_constant()
+            x_df = x_obj.get_exp()
+        x_list.append(x_df.copy())
+        y_list.append(cell_prop.copy())
+    x = pd.concat(x_list)
+    y = pd.concat(y_list)
+
+    print(f'   There are {x.shape[0]} samples in {dataset_name}...')
+    return x, y
+
+
+def align_with_gene_list(dataset_file: Union[pd.DataFrame, str], gene_list, gene_exp_type) -> pd.DataFrame:
+    """
+
+    :param dataset_file: file path or DataFrame, samples by genes
+    :param gene_list:
+    :param gene_exp_type: TPM / CPM, log_space, non_log
+    :return: log2tpm1p
+    """
+    dataset = ReadExp(dataset_file, exp_type=gene_exp_type).get_exp()
+    gene_not_in_ds = [i for i in gene_list if i not in dataset.columns]
+    dataset[gene_not_in_ds] = 0  # set expression values to 0 if a gene not exists
+    dataset = dataset.loc[:, gene_list].copy()  # remove genes not contain in gene_list
+    dataset = log_exp2cpm(dataset)
+    dataset = log2_transform(dataset)
+    return dataset
```

### Comparing `DeSide-1.0.1/deside/workflow/workflow.py` & `DeSide-1.0.2/deside/workflow/workflow.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-import os
-import numpy as np
-import pandas as pd
-import warnings
-from ..decon_cf import DeSide
-from ..utility import check_dir, print_msg, set_fig_style
-from ..utility.read_file import ReadH5AD
-from ..utility.compare import mean_exp_of_marker_gene, read_and_merge_result, cal_gene_signature_score
-from ..plot import (compare_exp_and_cell_fraction, plot_predicted_result,
-                    compare_cell_fraction_across_cancer_type, ScatterPlot, compare_y_y_pred_plot)
-warnings.simplefilter(action='ignore', category=FutureWarning)
-warnings.simplefilter(action='ignore', category=UserWarning)
-
-
-def tcga_evaluation(marker_gene_file_path, total_result_dir, pred_cell_frac_tcga_dir,
-                    cell_types, tcga_data_dir, outlier_file_path=None, pre_trained_model_dir=None,
-                    model_name: str = None, signature_score_method: str = 'mean_exp', cancer_types: list = None,
-                    update_figures=False):
-    """
-
-    :param marker_gene_file_path:
-    :param total_result_dir:
-    :param pred_cell_frac_tcga_dir:
-    :param cell_types:
-    :param tcga_data_dir:
-    :param outlier_file_path:
-    :param pre_trained_model_dir: the directory of pre-trained model
-    :param model_name: model name
-    :param signature_score_method:
-        mean_exp (the mean or max expression of corresponding marker genes for each cell type) or
-        gene_signature_score (Combes et al., 2022, Cell 185, 184-203)
-    :param cancer_types: a list of cancer types
-    :param update_figures: update figures or not
-    :return:
-    """
-    # marker_gene_file_path = marker_gene_file_path
-    # pred_cell_frac_dir = pred_cell_frac_tcga_dir
-    # result_dir = total_result_dir
-    if cancer_types is None:
-        cancer_types = ['ACC', 'BLCA', 'BRCA', 'GBM', 'HNSC', 'LGG', 'LIHC', 'LUAD', 'PAAD', 'PRAD',
-                        'CESC', 'COAD', 'KICH', 'KIRC', 'KIRP', 'LUSC', 'READ', 'THCA', 'UCEC']
-    # for model in model_name:
-    merged_signature_score_and_cell_frac_file_path = \
-        os.path.join(pred_cell_frac_tcga_dir, f'merged_all_signature_score_and_cell_fraction_by_{model_name}.csv')
-    pred_cell_frac_dir_current_model = os.path.join(pred_cell_frac_tcga_dir, model_name)
-    check_dir(pred_cell_frac_dir_current_model)
-    all_pred_cell_frac_file_path = os.path.join(pred_cell_frac_dir_current_model,
-                                                f'all_predicted_cell_fraction_by_{model_name}.csv')
-    signature_score_result_dir = os.path.join(pred_cell_frac_dir_current_model, 'signature_score')
-    check_dir(signature_score_result_dir)
-    all_signature_score_file_path = os.path.join(signature_score_result_dir, 'all_cancer_type_signature_score.csv')
-    # cell_types = cell_types
-    if 'DeSide' in model_name:
-        if os.path.exists(os.path.join(pre_trained_model_dir, model_name, model_name, 'genes.txt')):
-            gene_list_in_model_fp = os.path.join(pre_trained_model_dir, model_name, model_name, 'genes.txt')
-        else:
-            gene_list_in_model_fp = os.path.join(pre_trained_model_dir, 'genes.txt')
-    else:  # Scaden
-        gene_list_in_model_fp = os.path.join(pre_trained_model_dir, model_name, 'm256', 'genes.txt')
-    gene_list_in_model = list(pd.read_csv(gene_list_in_model_fp, index_col=0, sep='\t')['0'])
-    bulk_tpm = pd.read_csv(os.path.join(tcga_data_dir, 'merged_tpm.csv'), index_col=0)
-    sample2cancer_type = pd.read_csv(os.path.join(tcga_data_dir, 'tcga_sample_id2cancer_type.csv'), index_col=0)
-
-    if not os.path.exists(all_signature_score_file_path):
-        signature_scores = []
-        for cancer_type in cancer_types:
-            print('----------------------------------------------------')
-            print(f'Deal with cancer type: {cancer_type}...')
-            # tpm_file_path = os.path.join(tcga_data_dir, cancer_type, f'{cancer_type}_TPM.csv')
-            current_sample_ids = sample2cancer_type.loc[sample2cancer_type['cancer_type'] == cancer_type, :].copy()
-            tpm_file = bulk_tpm.loc[bulk_tpm.index.isin(current_sample_ids.index.to_list()), :].copy().T
-            result_file_path = os.path.join(signature_score_result_dir, f'{cancer_type}_signature_score.csv')
-            if signature_score_method == 'mean_exp':
-                current_signature_score = \
-                    mean_exp_of_marker_gene(marker_gene_file_path=marker_gene_file_path,
-                                            bulk_tpm_file_path=tpm_file, cell_types=cell_types,
-                                            result_file_path=result_file_path, cancer_type=cancer_type,
-                                            gene_list_in_model=gene_list_in_model)
-            else:  # gene_signature_score
-                current_signature_score = cal_gene_signature_score(marker_gene_file_path=marker_gene_file_path,
-                                                                   bulk_tpm_file_path=tpm_file,
-                                                                   cell_types=cell_types,
-                                                                   result_file_path=result_file_path,
-                                                                   cancer_type=cancer_type)
-            signature_scores.append(current_signature_score)
-        # merge all mean expression (gene signature score) of marker genes together
-        all_signature_score = pd.concat(signature_scores)
-        if all_signature_score.shape[0] > 0:
-            all_signature_score.to_csv(all_signature_score_file_path, float_format='%.3f')
-    else:
-        print(f'   Using the previous result of signature score of marker genes from: '
-              f'{all_signature_score_file_path}')
-        all_signature_score = pd.read_csv(all_signature_score_file_path, index_col=0)
-
-    # combine all predicted cell fraction for each cancer type together
-    if not os.path.exists(all_pred_cell_frac_file_path):
-        print(f'   Merge all predicted result by {model_name}...')
-        # if 'DeSide' in model:
-        #     _cell_types = cell_types + ['1-others']
-        # else:
-        #     _cell_types = cell_types
-        _cell_type_name_mapping = dict(zip(cell_types, cell_types))
-        read_and_merge_result(raw_result_dir=pred_cell_frac_dir_current_model,
-                              cell_type_name_mapping=_cell_type_name_mapping,
-                              algo=model_name, result_file_path=all_pred_cell_frac_file_path)
-    else:
-        print(f'   Using the previous result of merged cell fractions from: {all_pred_cell_frac_file_path}.')
-    all_pred_cell_fractions_df = pd.read_csv(all_pred_cell_frac_file_path, index_col='sample_id')
-
-    # merge two parts together
-    if not os.path.exists(merged_signature_score_and_cell_frac_file_path):
-        if 'cancer_type' in all_signature_score.columns:
-            all_signature_score.drop(columns=['cancer_type'], inplace=True)
-        merged_df = all_signature_score.merge(all_pred_cell_fractions_df, left_index=True, right_index=True)
-        merged_df.to_csv(merged_signature_score_and_cell_frac_file_path)
-
-    # comparing mean expression of marker genes and the predicted cell fraction of corresponding cell type
-    result_dir_new = os.path.join(total_result_dir, f'corr_signature_score_and_pred_cell_fraction', model_name)
-    # outlier samples in correlation for each cancer type, selected manually
-    # outlier_file_path = 'outlier_samples.txt'
-    outlier_file_path = outlier_file_path
-
-    cell_types_clustering = [i for i in cell_types if i != 'Cancer Cells']
-    compare_exp_and_cell_fraction(merged_file_path=merged_signature_score_and_cell_frac_file_path,
-                                  clustering_ct=cell_types_clustering, font_scale=1.5,
-                                  cell_types=cell_types, outlier_file_path=outlier_file_path,
-                                  result_dir=result_dir_new, update_figures=update_figures,
-                                  signature_score_method=signature_score_method)
-
-    print('Plot predicted cell proportion across all cancer types...')
-    cell_types2max = {'B Cells': 0.1, 'CD4 T': 0.1, 'DC': 0.1, 'CD8 T': 0.1}
-    across_all_dir = os.path.join(total_result_dir, 'across_all_cancer_type', model_name)
-    for cell_type in cell_types:
-        cell_type2max = cell_types2max.get(cell_type, 0.0)
-        compare_cell_fraction_across_cancer_type(merged_cell_fraction=all_pred_cell_fractions_df,
-                                                 result_dir=across_all_dir,
-                                                 outlier_file_path=outlier_file_path,
-                                                 ylabel=f'Predicted cell prop. of {cell_type} by {model_name}',
-                                                 cell_type=cell_type, cell_type2max=cell_type2max)
-
-
-def run_step3(evaluation_dataset2path, log_file_path, result_dir, model_dir,
-              all_cell_types, one_minus_alpha=False):
-    # Step3, evaluation on test set
-    print_msg('Step3: Predicting cell fractions of test set and evaluation...',
-              log_file_path=log_file_path)
-
-    for dataset_name, file_path in evaluation_dataset2path.items():
-        # if 'Test_set' in dataset_name:
-        print(f'   Evaluating on dataset {dataset_name}...')
-        predicted_result_dir = os.path.join(result_dir, dataset_name)
-        check_dir(predicted_result_dir)
-        predicted_cell_frac_file_path = os.path.join(predicted_result_dir,
-                                                     f'{dataset_name}_pred_cell_frac.csv')
-
-        generated_bulk_gep_fp = file_path
-        if dataset_name == 'Pre_Test_set':
-            generated_bulk_gep_fp = './datasets/simulated_bulk_cell_dataset/test_set_nbase3_7ds/' \
-                                    'simu_bulk_exp_Test_set2_log2cpm1p.h5ad'
-        generated_cell_frac = ReadH5AD(generated_bulk_gep_fp).get_cell_fraction()
-
-        if not os.path.exists(predicted_cell_frac_file_path):
-            deside_model = DeSide(model_dir=model_dir)
-            deside_model.predict(input_file=generated_bulk_gep_fp,
-                                 output_file_path=predicted_cell_frac_file_path,
-                                 exp_type='log_space', scaling_by_sample=False,
-                                 scaling_by_constant=True, one_minus_alpha=one_minus_alpha)
-        print('   > Comparing cell frac between y_true and y_pred...')
-        for cell_type in generated_cell_frac.columns.to_list():
-            s_plot = ScatterPlot(x=predicted_cell_frac_file_path,
-                                 y=generated_cell_frac,
-                                 postfix=f'pred_y_y_{cell_type}')
-            s_plot.plot(show_columns={'x': cell_type, 'y': cell_type}, fig_size=(8, 8),
-                        result_file_dir=predicted_result_dir, show_mae=True,
-                        show_rmse=True, show_diag=True,
-                        show_corr=True,
-                        x_label='y_pred by DeSide', y_label=f'y_true of {dataset_name}',
-                        show_reg_line=False)
-        # plot all cell types in one figure
-        compare_y_y_pred_plot(y_true=generated_cell_frac,
-                              y_pred=predicted_cell_frac_file_path,
-                              show_columns=all_cell_types, result_file_dir=predicted_result_dir,
-                              model_name=f'DeSide', show_metrics=True,
-                              y_label=f'y_pred')
-
-
-def run_step4(tcga_data_dir, cancer_types, log_file_path, model_dir, marker_gene_file_path,
-              result_dir, pred_cell_frac_tcga_dir, cancer_purity_file_path, all_cell_types,
-              model_names, signature_score_method, one_minus_alpha=False,
-              update_figures=False, outlier_file_path=None):
-    # TCGA
-    print_msg("Step 4: Predict cell fraction of TCGA...", log_file_path=log_file_path)
-    # model_name = 'DeSide'
-    for model_name in model_names:
-        bulk_tpm = pd.read_csv(os.path.join(tcga_data_dir, 'merged_tpm.csv'), index_col=0)
-        sample2cancer_type = pd.read_csv(os.path.join(tcga_data_dir, 'tcga_sample_id2cancer_type.csv'), index_col=0)
-        for cancer_type in cancer_types:
-            current_sample_ids = sample2cancer_type.loc[sample2cancer_type['cancer_type'] == cancer_type, :].copy()
-            current_bulk_tpm = bulk_tpm.loc[bulk_tpm.index.isin(current_sample_ids.index.to_list()), :].copy()
-            print(f'current_bulk_tpm: {current_bulk_tpm.shape}')
-            current_result_dir = os.path.join(pred_cell_frac_tcga_dir, model_name, cancer_type)
-            check_dir(current_result_dir)
-            y_pred_file_path = os.path.join(current_result_dir, 'y_predicted_result.csv')
-            if not os.path.exists(y_pred_file_path):
-                print(f'Predicting cell fractions of {cancer_type} samples by model {model_name}...')
-                deside_model = DeSide(model_dir=model_dir)
-                deside_model.predict(input_file=current_bulk_tpm, output_file_path=y_pred_file_path,
-                                     exp_type='TPM', scaling_by_constant=True,
-                                     scaling_by_sample=False, one_minus_alpha=one_minus_alpha)
-            else:
-                print(f'   Previous result existed: {y_pred_file_path}')
-            print(f'   Plot and compare predicted result...')
-            # y_pred_file_path = os.path.join(current_result_dir, 'y_predicted_result.csv')
-            plot_predicted_result(cell_frac_result_fp=y_pred_file_path, bulk_exp_fp=current_bulk_tpm.T,
-                                  cancer_type=cancer_type, model_name=model_name, result_dir=current_result_dir,
-                                  cancer_purity_fp=cancer_purity_file_path, update_figures=update_figures)
-
-        tcga_evaluation(marker_gene_file_path=marker_gene_file_path, total_result_dir=result_dir,
-                        pred_cell_frac_tcga_dir=pred_cell_frac_tcga_dir,
-                        cell_types=all_cell_types, tcga_data_dir=tcga_data_dir,
-                        pre_trained_model_dir=model_dir, model_name=model_name,
-                        signature_score_method=signature_score_method, cancer_types=cancer_types,
-                        update_figures=update_figures, outlier_file_path=outlier_file_path)
-
-        # calculate the distribution of predicted cell proportions in TCGA
-        # model_name = 'DeSide'
-        all_pred_cell_frac_file_path = os.path.join(pred_cell_frac_tcga_dir, model_name,
-                                                    f'all_predicted_cell_fraction_by_{model_name}.csv')
-        pred_cell_frac = pd.read_csv(all_pred_cell_frac_file_path, index_col=0)
-        pred_cell_frac = pred_cell_frac.loc[:, all_cell_types].copy()
-        cell_type2cell_prop_dis = {}
-        bins = np.linspace(0, 1, 11)
-        pred_cell_prop_dis_file_path = os.path.join(pred_cell_frac_tcga_dir, model_name,
-                                                    'pred_cell_frac_distribution.csv')
-        if not os.path.exists(pred_cell_prop_dis_file_path):
-            for ct in all_cell_types:
-                current_cp = pred_cell_frac[ct].values
-                hist, bin_edges = np.histogram(current_cp, bins=bins)
-                cell_type2cell_prop_dis[ct] = hist / len(current_cp)
-            cell_type2cell_prop_dis_df = pd.DataFrame.from_dict(cell_type2cell_prop_dis, orient='index')
-            cell_type2cell_prop_dis_df.to_csv(pred_cell_prop_dis_file_path, float_format='%g')
+import os
+import numpy as np
+import pandas as pd
+import warnings
+from ..decon_cf import DeSide
+from ..utility import check_dir, print_msg, set_fig_style
+from ..utility.read_file import ReadH5AD
+from ..utility.compare import mean_exp_of_marker_gene, read_and_merge_result, cal_gene_signature_score
+from ..plot import (compare_exp_and_cell_fraction, plot_predicted_result,
+                    compare_cell_fraction_across_cancer_type, ScatterPlot, compare_y_y_pred_plot)
+warnings.simplefilter(action='ignore', category=FutureWarning)
+warnings.simplefilter(action='ignore', category=UserWarning)
+
+
+def tcga_evaluation(marker_gene_file_path, total_result_dir, pred_cell_frac_tcga_dir,
+                    cell_types, tcga_data_dir, outlier_file_path=None, pre_trained_model_dir=None,
+                    model_name: str = None, signature_score_method: str = 'mean_exp', cancer_types: list = None,
+                    update_figures=False):
+    """
+
+    :param marker_gene_file_path:
+    :param total_result_dir:
+    :param pred_cell_frac_tcga_dir:
+    :param cell_types:
+    :param tcga_data_dir:
+    :param outlier_file_path:
+    :param pre_trained_model_dir: the directory of pre-trained model
+    :param model_name: model name
+    :param signature_score_method:
+        mean_exp (the mean or max expression of corresponding marker genes for each cell type) or
+        gene_signature_score (Combes et al., 2022, Cell 185, 184-203)
+    :param cancer_types: a list of cancer types
+    :param update_figures: update figures or not
+    :return:
+    """
+    # marker_gene_file_path = marker_gene_file_path
+    # pred_cell_frac_dir = pred_cell_frac_tcga_dir
+    # result_dir = total_result_dir
+    if cancer_types is None:
+        cancer_types = ['ACC', 'BLCA', 'BRCA', 'GBM', 'HNSC', 'LGG', 'LIHC', 'LUAD', 'PAAD', 'PRAD',
+                        'CESC', 'COAD', 'KICH', 'KIRC', 'KIRP', 'LUSC', 'READ', 'THCA', 'UCEC']
+    # for model in model_name:
+    merged_signature_score_and_cell_frac_file_path = \
+        os.path.join(pred_cell_frac_tcga_dir, f'merged_all_signature_score_and_cell_fraction_by_{model_name}.csv')
+    pred_cell_frac_dir_current_model = os.path.join(pred_cell_frac_tcga_dir, model_name)
+    check_dir(pred_cell_frac_dir_current_model)
+    all_pred_cell_frac_file_path = os.path.join(pred_cell_frac_dir_current_model,
+                                                f'all_predicted_cell_fraction_by_{model_name}.csv')
+    signature_score_result_dir = os.path.join(pred_cell_frac_dir_current_model, 'signature_score')
+    check_dir(signature_score_result_dir)
+    all_signature_score_file_path = os.path.join(signature_score_result_dir, 'all_cancer_type_signature_score.csv')
+    # cell_types = cell_types
+    if 'DeSide' in model_name:
+        if os.path.exists(os.path.join(pre_trained_model_dir, model_name, model_name, 'genes.txt')):
+            gene_list_in_model_fp = os.path.join(pre_trained_model_dir, model_name, model_name, 'genes.txt')
+        else:
+            gene_list_in_model_fp = os.path.join(pre_trained_model_dir, 'genes.txt')
+    else:  # Scaden
+        gene_list_in_model_fp = os.path.join(pre_trained_model_dir, model_name, 'm256', 'genes.txt')
+    gene_list_in_model = list(pd.read_csv(gene_list_in_model_fp, index_col=0, sep='\t')['0'])
+    bulk_tpm = pd.read_csv(os.path.join(tcga_data_dir, 'merged_tpm.csv'), index_col=0)
+    sample2cancer_type = pd.read_csv(os.path.join(tcga_data_dir, 'tcga_sample_id2cancer_type.csv'), index_col=0)
+
+    if not os.path.exists(all_signature_score_file_path):
+        signature_scores = []
+        for cancer_type in cancer_types:
+            print('----------------------------------------------------')
+            print(f'Deal with cancer type: {cancer_type}...')
+            # tpm_file_path = os.path.join(tcga_data_dir, cancer_type, f'{cancer_type}_TPM.csv')
+            current_sample_ids = sample2cancer_type.loc[sample2cancer_type['cancer_type'] == cancer_type, :].copy()
+            tpm_file = bulk_tpm.loc[bulk_tpm.index.isin(current_sample_ids.index.to_list()), :].copy().T
+            result_file_path = os.path.join(signature_score_result_dir, f'{cancer_type}_signature_score.csv')
+            if signature_score_method == 'mean_exp':
+                current_signature_score = \
+                    mean_exp_of_marker_gene(marker_gene_file_path=marker_gene_file_path,
+                                            bulk_tpm_file_path=tpm_file, cell_types=cell_types,
+                                            result_file_path=result_file_path, cancer_type=cancer_type,
+                                            gene_list_in_model=gene_list_in_model)
+            else:  # gene_signature_score
+                current_signature_score = cal_gene_signature_score(marker_gene_file_path=marker_gene_file_path,
+                                                                   bulk_tpm_file_path=tpm_file,
+                                                                   cell_types=cell_types,
+                                                                   result_file_path=result_file_path,
+                                                                   cancer_type=cancer_type)
+            signature_scores.append(current_signature_score)
+        # merge all mean expression (gene signature score) of marker genes together
+        all_signature_score = pd.concat(signature_scores)
+        if all_signature_score.shape[0] > 0:
+            all_signature_score.to_csv(all_signature_score_file_path, float_format='%.3f')
+    else:
+        print(f'   Using the previous result of signature score of marker genes from: '
+              f'{all_signature_score_file_path}')
+        all_signature_score = pd.read_csv(all_signature_score_file_path, index_col=0)
+
+    # combine all predicted cell fraction for each cancer type together
+    if not os.path.exists(all_pred_cell_frac_file_path):
+        print(f'   Merge all predicted result by {model_name}...')
+        # if 'DeSide' in model:
+        #     _cell_types = cell_types + ['1-others']
+        # else:
+        #     _cell_types = cell_types
+        _cell_type_name_mapping = dict(zip(cell_types, cell_types))
+        read_and_merge_result(raw_result_dir=pred_cell_frac_dir_current_model,
+                              cell_type_name_mapping=_cell_type_name_mapping,
+                              algo=model_name, result_file_path=all_pred_cell_frac_file_path)
+    else:
+        print(f'   Using the previous result of merged cell fractions from: {all_pred_cell_frac_file_path}.')
+    all_pred_cell_fractions_df = pd.read_csv(all_pred_cell_frac_file_path, index_col='sample_id')
+
+    # merge two parts together
+    if not os.path.exists(merged_signature_score_and_cell_frac_file_path):
+        if 'cancer_type' in all_signature_score.columns:
+            all_signature_score.drop(columns=['cancer_type'], inplace=True)
+        merged_df = all_signature_score.merge(all_pred_cell_fractions_df, left_index=True, right_index=True)
+        merged_df.to_csv(merged_signature_score_and_cell_frac_file_path)
+
+    # comparing mean expression of marker genes and the predicted cell fraction of corresponding cell type
+    result_dir_new = os.path.join(total_result_dir, f'corr_signature_score_and_pred_cell_fraction', model_name)
+    # outlier samples in correlation for each cancer type, selected manually
+    # outlier_file_path = 'outlier_samples.txt'
+    outlier_file_path = outlier_file_path
+
+    cell_types_clustering = [i for i in cell_types if i != 'Cancer Cells']
+    compare_exp_and_cell_fraction(merged_file_path=merged_signature_score_and_cell_frac_file_path,
+                                  clustering_ct=cell_types_clustering, font_scale=1.5,
+                                  cell_types=cell_types, outlier_file_path=outlier_file_path,
+                                  result_dir=result_dir_new, update_figures=update_figures,
+                                  signature_score_method=signature_score_method)
+
+    print('Plot predicted cell proportion across all cancer types...')
+    cell_types2max = {'B Cells': 0.1, 'CD4 T': 0.1, 'DC': 0.1, 'CD8 T': 0.1}
+    across_all_dir = os.path.join(total_result_dir, 'across_all_cancer_type', model_name)
+    for cell_type in cell_types:
+        cell_type2max = cell_types2max.get(cell_type, 0.0)
+        compare_cell_fraction_across_cancer_type(merged_cell_fraction=all_pred_cell_fractions_df,
+                                                 result_dir=across_all_dir,
+                                                 outlier_file_path=outlier_file_path,
+                                                 ylabel=f'Predicted cell prop. of {cell_type} by {model_name}',
+                                                 cell_type=cell_type, cell_type2max=cell_type2max)
+
+
+def run_step3(evaluation_dataset2path, log_file_path, result_dir, model_dir,
+              all_cell_types, one_minus_alpha=False):
+    # Step3, evaluation on test set
+    print_msg('Step3: Predicting cell fractions of test set and evaluation...',
+              log_file_path=log_file_path)
+
+    for dataset_name, file_path in evaluation_dataset2path.items():
+        # if 'Test_set' in dataset_name:
+        print(f'   Evaluating on dataset {dataset_name}...')
+        predicted_result_dir = os.path.join(result_dir, dataset_name)
+        check_dir(predicted_result_dir)
+        predicted_cell_frac_file_path = os.path.join(predicted_result_dir,
+                                                     f'{dataset_name}_pred_cell_frac.csv')
+
+        generated_bulk_gep_fp = file_path
+        if dataset_name == 'Pre_Test_set':
+            generated_bulk_gep_fp = './datasets/simulated_bulk_cell_dataset/test_set_nbase3_7ds/' \
+                                    'simu_bulk_exp_Test_set2_log2cpm1p.h5ad'
+        generated_cell_frac = ReadH5AD(generated_bulk_gep_fp).get_cell_fraction()
+
+        if not os.path.exists(predicted_cell_frac_file_path):
+            deside_model = DeSide(model_dir=model_dir)
+            deside_model.predict(input_file=generated_bulk_gep_fp,
+                                 output_file_path=predicted_cell_frac_file_path,
+                                 exp_type='log_space', scaling_by_sample=False,
+                                 scaling_by_constant=True, one_minus_alpha=one_minus_alpha)
+        print('   > Comparing cell frac between y_true and y_pred...')
+        for cell_type in generated_cell_frac.columns.to_list():
+            s_plot = ScatterPlot(x=predicted_cell_frac_file_path,
+                                 y=generated_cell_frac,
+                                 postfix=f'pred_y_y_{cell_type}')
+            s_plot.plot(show_columns={'x': cell_type, 'y': cell_type}, fig_size=(8, 8),
+                        result_file_dir=predicted_result_dir, show_mae=True,
+                        show_rmse=True, show_diag=True,
+                        show_corr=True,
+                        x_label='y_pred by DeSide', y_label=f'y_true of {dataset_name}',
+                        show_reg_line=False)
+        # plot all cell types in one figure
+        compare_y_y_pred_plot(y_true=generated_cell_frac,
+                              y_pred=predicted_cell_frac_file_path,
+                              show_columns=all_cell_types, result_file_dir=predicted_result_dir,
+                              model_name=f'DeSide', show_metrics=True,
+                              y_label=f'y_pred')
+
+
+def run_step4(tcga_data_dir, cancer_types, log_file_path, model_dir, marker_gene_file_path,
+              result_dir, pred_cell_frac_tcga_dir, cancer_purity_file_path, all_cell_types,
+              model_names, signature_score_method, one_minus_alpha=False,
+              update_figures=False, outlier_file_path=None):
+    # TCGA
+    print_msg("Step 4: Predict cell fraction of TCGA...", log_file_path=log_file_path)
+    # model_name = 'DeSide'
+    for model_name in model_names:
+        bulk_tpm = pd.read_csv(os.path.join(tcga_data_dir, 'merged_tpm.csv'), index_col=0)
+        sample2cancer_type = pd.read_csv(os.path.join(tcga_data_dir, 'tcga_sample_id2cancer_type.csv'), index_col=0)
+        for cancer_type in cancer_types:
+            current_sample_ids = sample2cancer_type.loc[sample2cancer_type['cancer_type'] == cancer_type, :].copy()
+            current_bulk_tpm = bulk_tpm.loc[bulk_tpm.index.isin(current_sample_ids.index.to_list()), :].copy()
+            print(f'current_bulk_tpm: {current_bulk_tpm.shape}')
+            current_result_dir = os.path.join(pred_cell_frac_tcga_dir, model_name, cancer_type)
+            check_dir(current_result_dir)
+            y_pred_file_path = os.path.join(current_result_dir, 'y_predicted_result.csv')
+            if not os.path.exists(y_pred_file_path):
+                print(f'Predicting cell fractions of {cancer_type} samples by model {model_name}...')
+                deside_model = DeSide(model_dir=model_dir)
+                deside_model.predict(input_file=current_bulk_tpm, output_file_path=y_pred_file_path,
+                                     exp_type='TPM', scaling_by_constant=True,
+                                     scaling_by_sample=False, one_minus_alpha=one_minus_alpha)
+            else:
+                print(f'   Previous result existed: {y_pred_file_path}')
+            print(f'   Plot and compare predicted result...')
+            # y_pred_file_path = os.path.join(current_result_dir, 'y_predicted_result.csv')
+            plot_predicted_result(cell_frac_result_fp=y_pred_file_path, bulk_exp_fp=current_bulk_tpm.T,
+                                  cancer_type=cancer_type, model_name=model_name, result_dir=current_result_dir,
+                                  cancer_purity_fp=cancer_purity_file_path, update_figures=update_figures)
+
+        tcga_evaluation(marker_gene_file_path=marker_gene_file_path, total_result_dir=result_dir,
+                        pred_cell_frac_tcga_dir=pred_cell_frac_tcga_dir,
+                        cell_types=all_cell_types, tcga_data_dir=tcga_data_dir,
+                        pre_trained_model_dir=model_dir, model_name=model_name,
+                        signature_score_method=signature_score_method, cancer_types=cancer_types,
+                        update_figures=update_figures, outlier_file_path=outlier_file_path)
+
+        # calculate the distribution of predicted cell proportions in TCGA
+        # model_name = 'DeSide'
+        all_pred_cell_frac_file_path = os.path.join(pred_cell_frac_tcga_dir, model_name,
+                                                    f'all_predicted_cell_fraction_by_{model_name}.csv')
+        pred_cell_frac = pd.read_csv(all_pred_cell_frac_file_path, index_col=0)
+        pred_cell_frac = pred_cell_frac.loc[:, all_cell_types].copy()
+        cell_type2cell_prop_dis = {}
+        bins = np.linspace(0, 1, 11)
+        pred_cell_prop_dis_file_path = os.path.join(pred_cell_frac_tcga_dir, model_name,
+                                                    'pred_cell_frac_distribution.csv')
+        if not os.path.exists(pred_cell_prop_dis_file_path):
+            for ct in all_cell_types:
+                current_cp = pred_cell_frac[ct].values
+                hist, bin_edges = np.histogram(current_cp, bins=bins)
+                cell_type2cell_prop_dis[ct] = hist / len(current_cp)
+            cell_type2cell_prop_dis_df = pd.DataFrame.from_dict(cell_type2cell_prop_dis, orient='index')
+            cell_type2cell_prop_dis_df.to_csv(pred_cell_prop_dis_file_path, float_format='%g')
```

### Comparing `DeSide-1.0.1/docs/.DS_Store` & `DeSide-1.0.2/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `DeSide-1.0.1/docs/Makefile` & `DeSide-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `DeSide-1.0.1/docs/changelog.md` & `DeSide-1.0.2/docs/changelog.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-Change Log
-==========
-
-## v0.2
-1 Oct 2020, first release.
-
-## v0.9.2
-12 May 2021, build workflow and create documentation
-
-## v0.9.3
-18 May 2021, bug fix, deal with more tumor types
-
-## v0.9.4
-11 Jun 2021, bug fix, update `Scanpy` to v1.7.2, deal with the correlation between predicted cell fractions of each cell type and mean gene expression of corresponding marker genes
-
-## v0.9.5
-2 Jul 2021, typo fix, update `Scanpy` to v1.8.0 & update `seaborn` to v0.11.1
-
-## v0.9.6
-7 Jul 2021, typo fix, check if `Cancer Cells` existed and update `bbknn` to v1.5.1
-
-## v0.9.6.1
-16 Jul 2021, set `total_cell_number` to 100 and `n_base` to 3 when simulating bulk cell data for better keeping cell type diversity
-
-## v0.9.7
-13 Sep 2021
-- Filtering single cell data of CD4 T and CD8 T cells by the ratio of marker genes
-- Updating marker gene list and re-annotating sub-clustering based on dot-plot figure of each single cell dataset
-
-## v0.9.8
-19 Nov 2021
-- Building the whole workflow in one file
-- Recording main parameters and running logs
-
-## v0.9.9
-21 Jan 2022
-- Using marker gene ratios to compare the similarity of GEPs between simulated bulk cell dataset and TCGA dataset
-- New method to filter simulated bulk cell GEPs depends on the nearest neighbors of each sample in TCGA dataset
-- Filtering genes by the correlation between gene expression values and cell fraction of each cell type
-- Removing genes depends on the loading matrix of PCA analysis by combining both simulated dataset and TCGA dataset
-
-## v0.9.9.1
-3 Mar 2022
-- update for evaluation
+Change Log
+==========
+The record of all notable changes to this project will be documented in this file.
+***
+
+## v0.2
+1 Oct 2020, first release.
+
+## v0.9.2
+12 May 2021, build workflow and create documentation
+
+## v0.9.3
+18 May 2021, bug fix, deal with more tumor types
+
+## v0.9.4
+11 Jun 2021, bug fix, update `Scanpy` to v1.7.2, deal with the correlation between predicted cell fractions of each cell type and mean gene expression of corresponding marker genes
+
+## v0.9.5
+2 Jul 2021, typo fix, update `Scanpy` to v1.8.0 & update `seaborn` to v0.11.1
+
+## v0.9.6
+7 Jul 2021, typo fix, check if `Cancer Cells` existed and update `bbknn` to v1.5.1
+
+## v0.9.6.1
+16 Jul 2021, set `total_cell_number` to 100 and `n_base` to 3 when simulating bulk cell data for better keeping cell type diversity
+
+## v0.9.7
+13 Sep 2021
+- Filtering single cell data of CD4 T and CD8 T cells by the ratio of marker genes
+- Updating marker gene list and re-annotating sub-clustering based on dot-plot figure of each single cell dataset
+
+## v0.9.8
+19 Nov 2021
+- Building the whole workflow in one file
+- Recording main parameters and running logs
+
+## v1.0.2 (bioRxiv)
+2 Jun 2023
+- Update documentation
```

### Comparing `DeSide-1.0.1/docs/conf.py` & `DeSide-1.0.2/docs/conf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,97 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# This file only contains a selection of the most common options. For a full
-# list see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-# -- Path setup --------------------------------------------------------------
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-#
-import os
-import sys
-sys.path.insert(0, os.path.abspath(r'..'))
-
-
-# -- Project information -----------------------------------------------------
-
-project = 'DeSide'
-copyright = '2021, iSynBio'
-author = 'Xin Xiong'
-
-# The full version, including alpha/beta/rc tags
-release = '0.9.1'
-
-
-# -- General configuration ---------------------------------------------------
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
-# ones.
-extensions = [
-    "myst_parser",
-    'sphinx.ext.autodoc',
-    # 'sphinx.ext.doctest',
-    # 'sphinx.ext.coverage',
-    # 'sphinx.ext.napoleon',
-    'sphinx.ext.mathjax',
-    # 'sphinx.ext.autosummary',
-    # 'sphinx.ext.intersphinx',
-    # 'matplotlib.sphinxext.plot_directive',
-    # 'gallery_generator',
-    # 'numpydoc',
-    # 'sphinx_issues',
-]
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-
-# -- Options for HTML output -------------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-# https://sphinx-book-theme.readthedocs.io/en/latest/, sphinx-book-theme-0.0.42
-html_theme = 'sphinx_book_theme'
-html_logo = "_static/logo.png"
-html_title = "DEep-learning and SIngle-cell based DEconvolution"
-html_copy_source = True
-# html_sourcelink_suffix = ""
-html_favicon = "_static/logo.png"
-# html_last_updated_fmt = ""
-
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-# ref to https://github.com/mwaskom/seaborn/blob/master/doc/conf.py
-html_theme_options = {
-    "theme_dev_mode": True,
-    "path_to_docs": "docs",
-    "repository_url": "https://github.com/OnlyBelter/DeSide",
-    "use_edit_page_button": True,
-    "use_issues_button": True,
-    "use_repository_button": True,
-    "use_download_button": True,
-}
-
-# Add type of source files
-source_suffix = ['.rst', '.md']
-
-fontawesome_included = True
+# Configuration file for the Sphinx documentation builder.
+#
+# This file only contains a selection of the most common options. For a full
+# list see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# -- Path setup --------------------------------------------------------------
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+#
+import os
+import sys
+# import sphinx_book_theme
+sys.path.insert(0, os.path.abspath(r'..'))
+
+
+# -- Project information -----------------------------------------------------
+
+project = 'DeSide'
+copyright = '2023, iSynBio & HKBU'
+author = 'Xin Xiong & Yerong Liu'
+
+# The full version, including alpha/beta/rc tags
+release = '1.0.2'
+
+
+# -- General configuration ---------------------------------------------------
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
+# ones.
+extensions = [
+    "myst_parser",
+    'sphinx.ext.autodoc',
+    'sphinx.ext.viewcode',
+    # 'sphinx.ext.doctest',
+    # 'sphinx.ext.coverage',
+    # 'sphinx.ext.napoleon',
+    'sphinx.ext.mathjax',
+    # 'sphinx.ext.autosummary',
+    # 'sphinx.ext.intersphinx',
+    # 'matplotlib.sphinxext.plot_directive',
+    # 'gallery_generator',
+    # 'numpydoc',
+    # 'sphinx_issues',
+]
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This pattern also affects html_static_path and html_extra_path.
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+
+# -- Options for HTML output -------------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+# https://sphinx-book-theme.readthedocs.io/en/latest/, sphinx-book-theme-0.0.42
+html_theme = 'furo'
+html_logo = "_static/logo.png"
+html_title = "DeSide"
+html_copy_source = True
+# html_sourcelink_suffix = ""
+html_favicon = "_static/logo.png"
+# html_last_updated_fmt = ""
+highlight_language = "python"
+
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ['_static']
+
+# ref to https://github.com/mwaskom/seaborn/blob/master/doc/conf.py
+html_theme_options = {
+    "source_directory": "docs/",
+    "source_repository": "https://github.com/OnlyBelter/DeSide",
+    # "source_edit_link": True,
+    # "use_issues_button": True,
+    # "use_repository_button": True,
+    # "use_download_button": True,
+}
+
+# custom css
+html_css_files = [
+    '_static/custom.css',
+]
+
+# Add type of source files
+source_suffix = ['.rst', '.md']
+
+fontawesome_included = True
```

### Comparing `DeSide-1.0.1/docs/make.bat` & `DeSide-1.0.2/docs/make.bat`

 * *Files identical despite different names*

