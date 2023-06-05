# Comparing `tmp/monotonic-nn-0.3.0.tar.gz` & `tmp/monotonic-nn-0.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic-nn-0.3.0.tar", last modified: Mon Jun  5 12:42:47 2023, max compression
+gzip compressed data, was "monotonic-nn-0.3.0rc0.tar", last modified: Mon Jun  5 12:35:27 2023, max compression
```

## Comparing `monotonic-nn-0.3.0.tar` & `monotonic-nn-0.3.0rc0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:42:47.143541 monotonic-nn-0.3.0/
--rw-r--r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 07:35:04.000000 monotonic-nn-0.3.0/LICENSE
--rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-06-05 07:35:04.000000 monotonic-nn-0.3.0/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    10657 2023-06-05 12:42:47.143541 monotonic-nn-0.3.0/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     9516 2023-06-05 12:24:54.000000 monotonic-nn-0.3.0/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:42:47.143541 monotonic-nn-0.3.0/airt/
--rw-rw-r--   0 davor     (1000) davor     (1000)       22 2023-06-05 12:42:23.000000 monotonic-nn-0.3.0/airt/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:42:47.143541 monotonic-nn-0.3.0/airt/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:42:23.000000 monotonic-nn-0.3.0/airt/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-05 12:42:23.000000 monotonic-nn-0.3.0/airt/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    31430 2023-06-05 12:42:23.000000 monotonic-nn-0.3.0/airt/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     9926 2023-06-05 12:42:23.000000 monotonic-nn-0.3.0/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:42:47.143541 monotonic-nn-0.3.0/airt/keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:42:23.000000 monotonic-nn-0.3.0/airt/keras/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14087 2023-06-05 12:42:23.000000 monotonic-nn-0.3.0/airt/keras/experiments.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:42:47.143541 monotonic-nn-0.3.0/airt/keras/layers/
--rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-05 12:42:23.000000 monotonic-nn-0.3.0/airt/keras/layers/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:42:47.143541 monotonic-nn-0.3.0/monotonic_nn.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    10657 2023-06-05 12:42:47.000000 monotonic-nn-0.3.0/monotonic_nn.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-05 12:42:47.000000 monotonic-nn-0.3.0/monotonic_nn.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 12:42:47.000000 monotonic-nn-0.3.0/monotonic_nn.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-05 12:42:47.000000 monotonic-nn-0.3.0/monotonic_nn.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 07:37:05.000000 monotonic-nn-0.3.0/monotonic_nn.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-05 12:42:47.000000 monotonic-nn-0.3.0/monotonic_nn.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-05 12:42:47.000000 monotonic-nn-0.3.0/monotonic_nn.egg-info/top_level.txt
--rw-r--r--   0 davor     (1000) davor     (1000)      916 2023-06-05 12:42:17.000000 monotonic-nn-0.3.0/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-05 12:42:47.143541 monotonic-nn-0.3.0/setup.cfg
--rw-r--r--   0 davor     (1000) davor     (1000)     3157 2023-06-05 12:32:50.000000 monotonic-nn-0.3.0/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/
+-rw-r--r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 07:35:04.000000 monotonic-nn-0.3.0rc0/LICENSE
+-rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-06-05 07:35:04.000000 monotonic-nn-0.3.0rc0/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10660 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9516 2023-06-05 12:24:54.000000 monotonic-nn-0.3.0rc0/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/airt/
+-rw-rw-r--   0 davor     (1000) davor     (1000)       22 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/airt/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-05 12:25:52.000000 monotonic-nn-0.3.0rc0/airt/_components/helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    31430 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9926 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/_modidx.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/airt/keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/keras/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14087 2023-06-05 12:25:52.000000 monotonic-nn-0.3.0rc0/airt/keras/experiments.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/airt/keras/layers/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-05 12:25:53.000000 monotonic-nn-0.3.0rc0/airt/keras/layers/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10660 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/SOURCES.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/dependency_links.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/entry_points.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 07:37:05.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/not-zip-safe
+-rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/requires.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-05 12:35:27.000000 monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/top_level.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)      919 2023-06-05 12:34:58.000000 monotonic-nn-0.3.0rc0/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-05 12:35:27.573294 monotonic-nn-0.3.0rc0/setup.cfg
+-rw-r--r--   0 davor     (1000) davor     (1000)     3157 2023-06-05 12:32:50.000000 monotonic-nn-0.3.0rc0/setup.py
```

### Comparing `monotonic-nn-0.3.0/LICENSE` & `monotonic-nn-0.3.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.0/PKG-INFO` & `monotonic-nn-0.3.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.3.0
+Version: 0.3.0rc0
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.0 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.0rc0 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
 colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
```

### Comparing `monotonic-nn-0.3.0/README.md` & `monotonic-nn-0.3.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.0/airt/_components/mono_dense_layer.py` & `monotonic-nn-0.3.0rc0/airt/_components/mono_dense_layer.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.0/airt/_modidx.py` & `monotonic-nn-0.3.0rc0/airt/_modidx.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.0/airt/keras/experiments.py` & `monotonic-nn-0.3.0rc0/airt/keras/experiments.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.0/monotonic_nn.egg-info/PKG-INFO` & `monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.3.0
+Version: 0.3.0rc0
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.0 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.0rc0 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
 colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
```

### Comparing `monotonic-nn-0.3.0/settings.ini` & `monotonic-nn-0.3.0rc0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = monotonic-nn
 lib_name = %(repo)s
-version = 0.3.0
+version = 0.3.0rc0
 min_python = 3.8
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = airt
 nbs_path = nbs
```

### Comparing `monotonic-nn-0.3.0/setup.py` & `monotonic-nn-0.3.0rc0/setup.py`

 * *Files identical despite different names*

