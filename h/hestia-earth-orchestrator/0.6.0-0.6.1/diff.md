# Comparing `tmp/hestia-earth-orchestrator-0.6.0.tar.gz` & `tmp/hestia-earth-orchestrator-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-orchestrator-0.6.0.tar", last modified: Thu Jun  1 14:20:19 2023, max compression
+gzip compressed data, was "hestia-earth-orchestrator-0.6.1.tar", last modified: Mon Jun  5 09:28:04 2023, max compression
```

## Comparing `hestia-earth-orchestrator-0.6.0.tar` & `hestia-earth-orchestrator-0.6.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.032527 hestia-earth-orchestrator-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2380 2023-06-01 14:20:19.031527 hestia-earth-orchestrator-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.023527 hestia-earth-orchestrator-0.6.0/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.024527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.024527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/config/
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.025527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/
--rw-rw-rw-   0 root         (0) root         (0)     3298 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.025527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/emissions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/emissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/emissions/deleted.py
--rw-rw-rw-   0 root         (0) root         (0)     4128 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/transformations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.025527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.026527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/
--rw-rw-rw-   0 root         (0) root         (0)     1416 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_append.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_default.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2659 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.027527 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2875 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/add_key_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/always.py
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.028527 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2380 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-01 14:20:18.000000 hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 14:20:19.032527 hestia-earth-orchestrator-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.022527 hestia-earth-orchestrator-0.6.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.029527 hestia-earth-orchestrator-0.6.0/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.029527 hestia-earth-orchestrator-0.6.0/tests/models/emissions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/models/emissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/models/emissions/test_deleted.py
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/models/test_transformations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.029527 hestia-earth-orchestrator-0.6.0/tests/strategies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.030527 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_append.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_default.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3207 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:20:19.031527 hestia-earth-orchestrator-0.6.0/tests/strategies/run/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/run/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3236 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/run/test_add_blank_node_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/run/test_add_key_if_missing.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-01 14:20:07.000000 hestia-earth-orchestrator-0.6.0/tests/strategies/run/test_always.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.801585 hestia-earth-orchestrator-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-06-05 09:28:04.801585 hestia-earth-orchestrator-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.793585 hestia-earth-orchestrator-0.6.1/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.794585 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.794585 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/config/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.795585 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.795585 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/models/emissions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/models/emissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/models/emissions/deleted.py
+-rw-rw-rw-   0 root         (0) root         (0)     4128 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/models/transformations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.795585 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.796585 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/merge_append.py
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/merge_default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/merge_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2659 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/merge_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.797585 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/run/
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/run/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/run/add_key_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/run/always.py
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.798585 hestia-earth-orchestrator-0.6.1/hestia_earth_orchestrator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-06-05 09:28:04.000000 hestia-earth-orchestrator-0.6.1/hestia_earth_orchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-05 09:28:04.000000 hestia-earth-orchestrator-0.6.1/hestia_earth_orchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 09:28:04.000000 hestia-earth-orchestrator-0.6.1/hestia_earth_orchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-05 09:28:04.000000 hestia-earth-orchestrator-0.6.1/hestia_earth_orchestrator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-05 09:28:04.000000 hestia-earth-orchestrator-0.6.1/hestia_earth_orchestrator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 09:28:04.801585 hestia-earth-orchestrator-0.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.792585 hestia-earth-orchestrator-0.6.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.798585 hestia-earth-orchestrator-0.6.1/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.799585 hestia-earth-orchestrator-0.6.1/tests/models/emissions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/models/emissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/models/emissions/test_deleted.py
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/models/test_transformations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.799585 hestia-earth-orchestrator-0.6.1/tests/strategies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.800585 hestia-earth-orchestrator-0.6.1/tests/strategies/merge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/merge/test_merge_append.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/merge/test_merge_default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/merge/test_merge_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3207 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/merge/test_merge_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:28:04.801585 hestia-earth-orchestrator-0.6.1/tests/strategies/run/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/run/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3236 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/run/test_add_blank_node_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/run/test_add_key_if_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-05 09:27:52.000000 hestia-earth-orchestrator-0.6.1/tests/strategies/run/test_always.py
```

### Comparing `hestia-earth-orchestrator-0.6.0/LICENSE` & `hestia-earth-orchestrator-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/PKG-INFO` & `hestia-earth-orchestrator-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-orchestrator
-Version: 0.6.0
+Version: 0.6.1
 Summary: Hestia's module to orchestrate the models.
 Home-page: https://gitlab.com/hestia-earth/hestia-engine-orchestrator
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-orchestrator-0.6.0/README.md` & `hestia-earth-orchestrator-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/__init__.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/log.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/__init__.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/emissions/deleted.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/models/emissions/deleted.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/models/transformations.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/models/transformations.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/__init__.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_append.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/merge_append.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_list.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/merge_list.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/merge/merge_node.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/merge/merge_node.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/strategies/run/add_blank_node_if_missing.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth/orchestrator/utils.py` & `hestia-earth-orchestrator-0.6.1/hestia_earth/orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/PKG-INFO` & `hestia-earth-orchestrator-0.6.1/hestia_earth_orchestrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-orchestrator
-Version: 0.6.0
+Version: 0.6.1
 Summary: Hestia's module to orchestrate the models.
 Home-page: https://gitlab.com/hestia-earth/hestia-engine-orchestrator
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-orchestrator-0.6.0/hestia_earth_orchestrator.egg-info/SOURCES.txt` & `hestia-earth-orchestrator-0.6.1/hestia_earth_orchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/setup.py` & `hestia-earth-orchestrator-0.6.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,19 +5,15 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
-
-def parse_require(path: pathlib.Path): return path.read_text().splitlines()
-
-
-REQUIRES = parse_require(HERE / "requirements.txt") + parse_require(HERE / "requirements-models.txt")
+REQUIRES = (HERE / "requirements.txt").read_text().splitlines()
 
 # This call to setup() does all the work
 setup(
     name='hestia-earth-orchestrator',
     version=VERSION,
     description="Hestia's module to orchestrate the models.",
     long_description=README,
```

### Comparing `hestia-earth-orchestrator-0.6.0/tests/models/emissions/test_deleted.py` & `hestia-earth-orchestrator-0.6.1/tests/models/emissions/test_deleted.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/tests/models/test_transformations.py` & `hestia-earth-orchestrator-0.6.1/tests/models/test_transformations.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_append.py` & `hestia-earth-orchestrator-0.6.1/tests/strategies/merge/test_merge_append.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_list.py` & `hestia-earth-orchestrator-0.6.1/tests/strategies/merge/test_merge_list.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/tests/strategies/merge/test_merge_node.py` & `hestia-earth-orchestrator-0.6.1/tests/strategies/merge/test_merge_node.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-orchestrator-0.6.0/tests/strategies/run/test_add_blank_node_if_missing.py` & `hestia-earth-orchestrator-0.6.1/tests/strategies/run/test_add_blank_node_if_missing.py`

 * *Files identical despite different names*

