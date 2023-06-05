# Comparing `tmp/hcai-nova-server-nightly-0.1.8.dev202306050652.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.9.dev202306050655.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.8.dev202306050652.tar", last modified: Mon Jun  5 06:52:25 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.9.dev202306050655.tar", last modified: Mon Jun  5 06:55:18 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652.tar` & `hcai-nova-server-nightly-0.1.9.dev202306050655.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:25.131107 hcai-nova-server-nightly-0.1.8.dev202306050652/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-05 06:52:10.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 06:52:25.131107 hcai-nova-server-nightly-0.1.8.dev202306050652/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-05 06:52:10.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:25.131107 hcai-nova-server-nightly-0.1.8.dev202306050652/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 06:52:25.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-05 06:52:25.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 06:52:25.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-05 06:52:25.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/hcai_nova_server_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-05 06:52:25.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-05 06:52:25.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:25.131107 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:25.131107 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9818 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7072 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:25.131107 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:25.131107 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-05 06:52:25.131107 hcai-nova-server-nightly-0.1.8.dev202306050652/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-05 06:52:11.000000 hcai-nova-server-nightly-0.1.8.dev202306050652/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.288236 hcai-nova-server-nightly-0.1.9.dev202306050655/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 06:55:18.288236 hcai-nova-server-nightly-0.1.9.dev202306050655/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.284236 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-05 06:55:18.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.284236 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.284236 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9818 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7072 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.284236 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:18.288236 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-05 06:55:18.288236 hcai-nova-server-nightly-0.1.9.dev202306050655/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-05 06:55:00.000000 hcai-nova-server-nightly-0.1.9.dev202306050655/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/PKG-INFO` & `hcai-nova-server-nightly-0.1.9.dev202306050655/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.8.dev202306050652
+Version: 0.1.9.dev202306050655
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.8.dev202306050652
+Version: 0.1.9.dev202306050655
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.9.dev202306050655/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/app.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/app.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306050652/setup.py` & `hcai-nova-server-nightly-0.1.9.dev202306050655/setup.py`

 * *Files identical despite different names*

