# Comparing `tmp/rmlab-0.4.3.tar.gz` & `tmp/rmlab-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmlab-0.4.3.tar", last modified: Sun Jun  4 15:55:21 2023, max compression
+gzip compressed data, was "rmlab-0.4.4.tar", last modified: Mon Jun  5 14:30:25 2023, max compression
```

## Comparing `rmlab-0.4.3.tar` & `rmlab-0.4.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.027712 rmlab-0.4.3/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-04 15:55:06.000000 rmlab-0.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1990 2023-06-04 15:55:21.027712 rmlab-0.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-06-04 15:55:06.000000 rmlab-0.4.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-04 15:55:06.000000 rmlab-0.4.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-04 15:55:21.027712 rmlab-0.4.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.015712 rmlab-0.4.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.018712 rmlab-0.4.3/src/rmlab/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.020712 rmlab-0.4.3/src/rmlab/_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9590 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    14244 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_api/fetch.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_api/observability.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_api/remove.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_api/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)    10142 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_api/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.021712 rmlab-0.4.3/src/rmlab/_data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4993 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_data/conversions.py
--rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_data/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1937 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_data/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.021712 rmlab-0.4.3/src/rmlab/_util/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.021712 rmlab-0.4.3/src/rmlab/api/
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.022712 rmlab-0.4.3/src/rmlab/api/fetch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/fetch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11464 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/fetch/core.py
--rw-rw-rw-   0 root         (0) root         (0)     8419 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/fetch/flight_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4924 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/fetch/parametric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.022712 rmlab-0.4.3/src/rmlab/api/observability/
--rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/observability/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.023712 rmlab-0.4.3/src/rmlab/api/operations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4951 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/operations/optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     2962 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/operations/simulation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.023712 rmlab-0.4.3/src/rmlab/api/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/persistence/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/remove.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.023712 rmlab-0.4.3/src/rmlab/api/upload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13213 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/upload/core.py
--rw-rw-rw-   0 root         (0) root         (0)     5265 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/upload/flight_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.024712 rmlab-0.4.3/src/rmlab/api/upload/parametric/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/upload/parametric/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2992 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/upload/parametric/customers.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/upload/parametric/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     4391 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/api/upload/parametric/pricing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.025712 rmlab-0.4.3/src/rmlab/data/
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6828 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/flight.py
--rw-rw-rw-   0 root         (0) root         (0)    10309 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/items.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.026712 rmlab-0.4.3/src/rmlab/data/parametric/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/parametric/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/parametric/_customers_base.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/parametric/_pricing_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8670 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/parametric/customers_choice.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/parametric/customers_request.py
--rw-rw-rw-   0 root         (0) root         (0)     7923 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/parametric/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/parametric/pricing_behavior.py
--rw-rw-rw-   0 root         (0) root         (0)    10949 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/parametric/pricing_optimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     3922 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/parametric/pricing_range.py
--rw-rw-rw-   0 root         (0) root         (0)     4379 2023-06-04 15:55:06.000000 rmlab-0.4.3/src/rmlab/data/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 15:55:21.019712 rmlab-0.4.3/src/rmlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1990 2023-06-04 15:55:21.000000 rmlab-0.4.3/src/rmlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1713 2023-06-04 15:55:21.000000 rmlab-0.4.3/src/rmlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 15:55:21.000000 rmlab-0.4.3/src/rmlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 15:55:21.000000 rmlab-0.4.3/src/rmlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-04 15:55:21.000000 rmlab-0.4.3/src/rmlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.720768 rmlab-0.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-05 14:30:11.000000 rmlab-0.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-06-05 14:30:25.720768 rmlab-0.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-06-05 14:30:11.000000 rmlab-0.4.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-05 14:30:11.000000 rmlab-0.4.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-05 14:30:25.721768 rmlab-0.4.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.706768 rmlab-0.4.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.709768 rmlab-0.4.4/src/rmlab/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.712768 rmlab-0.4.4/src/rmlab/_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9590 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14244 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_api/fetch.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_api/observability.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_api/remove.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_api/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10142 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_api/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.713768 rmlab-0.4.4/src/rmlab/_data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4993 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_data/conversions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_data/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_data/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.713768 rmlab-0.4.4/src/rmlab/_util/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.713768 rmlab-0.4.4/src/rmlab/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.714769 rmlab-0.4.4/src/rmlab/api/fetch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/fetch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11464 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/fetch/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     8419 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/fetch/flight_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4924 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/fetch/parametric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.715768 rmlab-0.4.4/src/rmlab/api/observability/
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/observability/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.715768 rmlab-0.4.4/src/rmlab/api/operations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4951 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/operations/optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2962 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/operations/simulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.715768 rmlab-0.4.4/src/rmlab/api/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/persistence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/remove.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.716768 rmlab-0.4.4/src/rmlab/api/upload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13213 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/upload/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     5265 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/upload/flight_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.717768 rmlab-0.4.4/src/rmlab/api/upload/parametric/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/upload/parametric/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/upload/parametric/customers.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/upload/parametric/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4391 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/api/upload/parametric/pricing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.718768 rmlab-0.4.4/src/rmlab/data/
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/flight.py
+-rw-rw-rw-   0 root         (0) root         (0)    10309 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.720768 rmlab-0.4.4/src/rmlab/data/parametric/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/parametric/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/parametric/_customers_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/parametric/_pricing_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/parametric/customers_choice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/parametric/customers_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     7923 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/parametric/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/parametric/pricing_behavior.py
+-rw-rw-rw-   0 root         (0) root         (0)    10949 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/parametric/pricing_optimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/parametric/pricing_range.py
+-rw-rw-rw-   0 root         (0) root         (0)     4379 2023-06-05 14:30:11.000000 rmlab-0.4.4/src/rmlab/data/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:30:25.710769 rmlab-0.4.4/src/rmlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-06-05 14:30:25.000000 rmlab-0.4.4/src/rmlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-06-05 14:30:25.000000 rmlab-0.4.4/src/rmlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 14:30:25.000000 rmlab-0.4.4/src/rmlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 14:30:25.000000 rmlab-0.4.4/src/rmlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-05 14:30:25.000000 rmlab-0.4.4/src/rmlab.egg-info/top_level.txt
```

### Comparing `rmlab-0.4.3/LICENSE` & `rmlab-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/PKG-INFO` & `rmlab-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmlab
-Version: 0.4.3
+Version: 0.4.4
 Summary: RMLab python client
 Home-page: https://rmlab.ai
 Author: Anton Rey
 Author-email: aanton.rv@gmail.com
 Project-URL: Bug Tracker, https://rmlab.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rmlab-0.4.3/README.md` & `rmlab-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/setup.cfg` & `rmlab-0.4.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rmlab
-version = 0.4.3
+version = 0.4.4
 author = Anton Rey
 author_email = aanton.rv@gmail.com
 description = RMLab python client
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://rmlab.ai
 project_urls =
```

### Comparing `rmlab-0.4.3/src/rmlab/__init__.py` & `rmlab-0.4.4/src/rmlab/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/_api/base.py` & `rmlab-0.4.4/src/rmlab/_api/base.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/_api/fetch.py` & `rmlab-0.4.4/src/rmlab/_api/fetch.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/_api/remove.py` & `rmlab-0.4.4/src/rmlab/_api/remove.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/_api/simulation.py` & `rmlab-0.4.4/src/rmlab/_api/simulation.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/_api/upload.py` & `rmlab-0.4.4/src/rmlab/_api/upload.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/_data/conversions.py` & `rmlab-0.4.4/src/rmlab/_data/conversions.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/_data/enums.py` & `rmlab-0.4.4/src/rmlab/_data/enums.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/_data/types.py` & `rmlab-0.4.4/src/rmlab/_data/types.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/_util/__init__.py` & `rmlab-0.4.4/src/rmlab/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/__init__.py` & `rmlab-0.4.4/src/rmlab/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/fetch/core.py` & `rmlab-0.4.4/src/rmlab/api/fetch/core.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/fetch/flight_data.py` & `rmlab-0.4.4/src/rmlab/api/fetch/flight_data.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/fetch/parametric.py` & `rmlab-0.4.4/src/rmlab/api/fetch/parametric.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/observability/__init__.py` & `rmlab-0.4.4/src/rmlab/api/observability/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/operations/optimization.py` & `rmlab-0.4.4/src/rmlab/api/operations/optimization.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/operations/simulation.py` & `rmlab-0.4.4/src/rmlab/api/operations/simulation.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/persistence/__init__.py` & `rmlab-0.4.4/src/rmlab/api/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/remove.py` & `rmlab-0.4.4/src/rmlab/api/remove.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/upload/core.py` & `rmlab-0.4.4/src/rmlab/api/upload/core.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/upload/flight_data.py` & `rmlab-0.4.4/src/rmlab/api/upload/flight_data.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/upload/parametric/customers.py` & `rmlab-0.4.4/src/rmlab/api/upload/parametric/customers.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/upload/parametric/filters.py` & `rmlab-0.4.4/src/rmlab/api/upload/parametric/filters.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/api/upload/parametric/pricing.py` & `rmlab-0.4.4/src/rmlab/api/upload/parametric/pricing.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/__init__.py` & `rmlab-0.4.4/src/rmlab/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/flight.py` & `rmlab-0.4.4/src/rmlab/data/flight.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/items.py` & `rmlab-0.4.4/src/rmlab/data/items.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/parametric/customers_choice.py` & `rmlab-0.4.4/src/rmlab/data/parametric/customers_choice.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/parametric/customers_request.py` & `rmlab-0.4.4/src/rmlab/data/parametric/customers_request.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/parametric/filter.py` & `rmlab-0.4.4/src/rmlab/data/parametric/filter.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/parametric/pricing_behavior.py` & `rmlab-0.4.4/src/rmlab/data/parametric/pricing_behavior.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/parametric/pricing_optimizer.py` & `rmlab-0.4.4/src/rmlab/data/parametric/pricing_optimizer.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/parametric/pricing_range.py` & `rmlab-0.4.4/src/rmlab/data/parametric/pricing_range.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab/data/scenario.py` & `rmlab-0.4.4/src/rmlab/data/scenario.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.3/src/rmlab.egg-info/PKG-INFO` & `rmlab-0.4.4/src/rmlab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmlab
-Version: 0.4.3
+Version: 0.4.4
 Summary: RMLab python client
 Home-page: https://rmlab.ai
 Author: Anton Rey
 Author-email: aanton.rv@gmail.com
 Project-URL: Bug Tracker, https://rmlab.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rmlab-0.4.3/src/rmlab.egg-info/SOURCES.txt` & `rmlab-0.4.4/src/rmlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

