# Comparing `tmp/monotonic-nn-0.2.0rc1.tar.gz` & `tmp/monotonic-nn-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic-nn-0.2.0rc1.tar", last modified: Mon Jun  5 12:17:15 2023, max compression
+gzip compressed data, was "monotonic-nn-0.2.0rc2.tar", last modified: Mon Jun  5 12:24:00 2023, max compression
```

## Comparing `monotonic-nn-0.2.0rc1.tar` & `monotonic-nn-0.2.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/
--rw-r--r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc1/LICENSE
--rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc1/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    10560 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     9547 2023-06-05 12:16:54.000000 monotonic-nn-0.2.0rc1/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/airt/
--rw-rw-r--   0 davor     (1000) davor     (1000)       25 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/airt/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    31430 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     9926 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/airt/keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/keras/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14087 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/keras/experiments.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/airt/keras/layers/
--rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/keras/layers/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    10560 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 07:37:05.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      224 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/top_level.txt
--rw-r--r--   0 davor     (1000) davor     (1000)      919 2023-06-05 12:11:04.000000 monotonic-nn-0.2.0rc1/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/setup.cfg
--rw-r--r--   0 davor     (1000) davor     (1000)     3093 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc1/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.047675 monotonic-nn-0.2.0rc2/
+-rw-r--r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc2/LICENSE
+-rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc2/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10562 2023-06-05 12:24:00.047675 monotonic-nn-0.2.0rc2/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9549 2023-06-05 12:23:32.000000 monotonic-nn-0.2.0rc2/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.043675 monotonic-nn-0.2.0rc2/airt/
+-rw-rw-r--   0 davor     (1000) davor     (1000)       25 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.043675 monotonic-nn-0.2.0rc2/airt/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/_components/helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    31430 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9926 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/_modidx.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.043675 monotonic-nn-0.2.0rc2/airt/keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/keras/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14087 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/keras/experiments.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.043675 monotonic-nn-0.2.0rc2/airt/keras/layers/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/keras/layers/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.047675 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10562 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-05 12:24:00.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/SOURCES.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/dependency_links.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/entry_points.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 07:37:05.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/not-zip-safe
+-rw-rw-r--   0 davor     (1000) davor     (1000)      224 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/requires.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/top_level.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)      919 2023-06-05 12:23:53.000000 monotonic-nn-0.2.0rc2/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-05 12:24:00.047675 monotonic-nn-0.2.0rc2/setup.cfg
+-rw-r--r--   0 davor     (1000) davor     (1000)     3093 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc2/setup.py
```

### Comparing `monotonic-nn-0.2.0rc1/LICENSE` & `monotonic-nn-0.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc1/PKG-INFO` & `monotonic-nn-0.2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
@@ -151,15 +151,17 @@
 - set 1 for increasingly monotonic parameter,
 
 - set -1 for decreasingly monotonic parameter, and
 
 - set 0 otherwise.
 
 In our case, the `monotonicity_indicator` is `[1, 0, -1]` because $y$
-is: - monotonically increasing w.r.t. $x_1$
+is: 
+
+- monotonically increasing w.r.t. $x_1$
 $\left(\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and
 
 - monotonically decreasing w.r.t. $x_3$
   $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq 0\right)$.
 
 ``` python
 from tensorflow.keras import Sequential
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc1 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc2 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://mono-dense-keras.airt.ai/ Keywords: tensorflow keras
 monotone "monotonic neural networks" "dense layer" Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
```

### Comparing `monotonic-nn-0.2.0rc1/README.md` & `monotonic-nn-0.2.0rc2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,17 @@
 - set 1 for increasingly monotonic parameter,
 
 - set -1 for decreasingly monotonic parameter, and
 
 - set 0 otherwise.
 
 In our case, the `monotonicity_indicator` is `[1, 0, -1]` because $y$
-is: - monotonically increasing w.r.t. $x_1$
+is: 
+
+- monotonically increasing w.r.t. $x_1$
 $\left(\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and
 
 - monotonically decreasing w.r.t. $x_3$
   $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq 0\right)$.
 
 ``` python
 from tensorflow.keras import Sequential
```

### Comparing `monotonic-nn-0.2.0rc1/airt/_components/mono_dense_layer.py` & `monotonic-nn-0.2.0rc2/airt/_components/mono_dense_layer.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc1/airt/_modidx.py` & `monotonic-nn-0.2.0rc2/airt/_modidx.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc1/airt/keras/experiments.py` & `monotonic-nn-0.2.0rc2/airt/keras/experiments.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/PKG-INFO` & `monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
@@ -151,15 +151,17 @@
 - set 1 for increasingly monotonic parameter,
 
 - set -1 for decreasingly monotonic parameter, and
 
 - set 0 otherwise.
 
 In our case, the `monotonicity_indicator` is `[1, 0, -1]` because $y$
-is: - monotonically increasing w.r.t. $x_1$
+is: 
+
+- monotonically increasing w.r.t. $x_1$
 $\left(\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and
 
 - monotonically decreasing w.r.t. $x_3$
   $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq 0\right)$.
 
 ``` python
 from tensorflow.keras import Sequential
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc1 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc2 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://mono-dense-keras.airt.ai/ Keywords: tensorflow keras
 monotone "monotonic neural networks" "dense layer" Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
```

### Comparing `monotonic-nn-0.2.0rc1/settings.ini` & `monotonic-nn-0.2.0rc2/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = monotonic-nn
 lib_name = %(repo)s
-version = 0.2.0rc1
+version = 0.2.0rc2
 min_python = 3.8
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = airt
 nbs_path = nbs
```

### Comparing `monotonic-nn-0.2.0rc1/setup.py` & `monotonic-nn-0.2.0rc2/setup.py`

 * *Files identical despite different names*

