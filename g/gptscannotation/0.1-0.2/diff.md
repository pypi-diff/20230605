# Comparing `tmp/gptscannotation-0.1.tar.gz` & `tmp/gptscannotation-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptscannotation-0.1.tar", last modified: Mon Jun  5 01:05:24 2023, max compression
+gzip compressed data, was "gptscannotation-0.2.tar", last modified: Mon Jun  5 01:09:17 2023, max compression
```

## Comparing `gptscannotation-0.1.tar` & `gptscannotation-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 01:05:24.830439 gptscannotation-0.1/
--rw-rw-rw-   0        0        0      216 2023-06-05 01:05:24.829441 gptscannotation-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4988 2023-06-05 01:04:08.000000 gptscannotation-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 01:05:24.822461 gptscannotation-0.1/gptscannotation/
--rw-rw-rw-   0        0        0       40 2023-06-04 22:00:41.000000 gptscannotation-0.1/gptscannotation/__init__.py
--rw-rw-rw-   0        0        0    11758 2023-06-05 00:43:09.000000 gptscannotation-0.1/gptscannotation/chat_workflow.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:05:24.828445 gptscannotation-0.1/gptscannotation.egg-info/
--rw-rw-rw-   0        0        0      216 2023-06-05 01:05:24.000000 gptscannotation-0.1/gptscannotation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-05 01:05:24.000000 gptscannotation-0.1/gptscannotation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 01:05:24.000000 gptscannotation-0.1/gptscannotation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-05 01:05:24.000000 gptscannotation-0.1/gptscannotation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 01:05:24.000000 gptscannotation-0.1/gptscannotation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 01:05:24.830439 gptscannotation-0.1/setup.cfg
--rw-rw-rw-   0        0        0      384 2023-06-05 01:04:56.000000 gptscannotation-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:09:17.341070 gptscannotation-0.2/
+-rw-rw-rw-   0        0        0      216 2023-06-05 01:09:17.340073 gptscannotation-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4988 2023-06-05 01:04:08.000000 gptscannotation-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 01:09:17.334089 gptscannotation-0.2/gptscannotation/
+-rw-rw-rw-   0        0        0       40 2023-06-04 22:00:41.000000 gptscannotation-0.2/gptscannotation/__init__.py
+-rw-rw-rw-   0        0        0    11759 2023-06-05 01:07:49.000000 gptscannotation-0.2/gptscannotation/chat_workflow.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:09:17.339075 gptscannotation-0.2/gptscannotation.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-06-05 01:09:17.000000 gptscannotation-0.2/gptscannotation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-05 01:09:17.000000 gptscannotation-0.2/gptscannotation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:09:17.000000 gptscannotation-0.2/gptscannotation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-05 01:09:17.000000 gptscannotation-0.2/gptscannotation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 01:09:17.000000 gptscannotation-0.2/gptscannotation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 01:09:17.341070 gptscannotation-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      384 2023-06-05 01:09:03.000000 gptscannotation-0.2/setup.py
```

### Comparing `gptscannotation-0.1/README.md` & `gptscannotation-0.2/README.md`

 * *Files identical despite different names*

### Comparing `gptscannotation-0.1/gptscannotation/chat_workflow.py` & `gptscannotation-0.2/gptscannotation/chat_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from skimage.filters import threshold_ots
+from skimage.filters import threshold_otsu
 import openai
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import time
 
 def extra_genes_inquiry(adata, genes, cluster_ids, log_counts_layer, use_raw):
```

