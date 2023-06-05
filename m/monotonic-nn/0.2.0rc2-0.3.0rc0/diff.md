# Comparing `tmp/monotonic-nn-0.2.0rc2.tar.gz` & `tmp/monotonic-nn-0.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic-nn-0.2.0rc2.tar", last modified: Mon Jun  5 12:24:00 2023, max compression
+gzip compressed data, was "monotonic-nn-0.3.0rc0.tar", last modified: Mon Jun  5 12:35:27 2023, max compression
```

## Comparing `monotonic-nn-0.2.0rc2.tar` & `monotonic-nn-0.3.0rc0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.047675 monotonic-nn-0.2.0rc2/
--rw-r--r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc2/LICENSE
--rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc2/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    10562 2023-06-05 12:24:00.047675 monotonic-nn-0.2.0rc2/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     9549 2023-06-05 12:23:32.000000 monotonic-nn-0.2.0rc2/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.043675 monotonic-nn-0.2.0rc2/airt/
--rw-rw-r--   0 davor     (1000) davor     (1000)       25 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.043675 monotonic-nn-0.2.0rc2/airt/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    31430 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     9926 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.043675 monotonic-nn-0.2.0rc2/airt/keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/keras/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14087 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/keras/experiments.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.043675 monotonic-nn-0.2.0rc2/airt/keras/layers/
--rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc2/airt/keras/layers/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:24:00.047675 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    10562 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-05 12:24:00.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 07:37:05.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      224 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-05 12:23:59.000000 monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/top_level.txt
--rw-r--r--   0 davor     (1000) davor     (1000)      919 2023-06-05 12:23:53.000000 monotonic-nn-0.2.0rc2/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-05 12:24:00.047675 monotonic-nn-0.2.0rc2/setup.cfg
--rw-r--r--   0 davor     (1000) davor     (1000)     3093 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc2/setup.py
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

### Comparing `monotonic-nn-0.2.0rc2/LICENSE` & `monotonic-nn-0.3.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc2/PKG-INFO` & `monotonic-nn-0.3.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.2.0rc2
+Version: 0.3.0rc0
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
-Project-URL: Documentation, https://mono-dense-keras.airt.ai/
+Project-URL: Documentation, https://monotonic.airt.ai/
+Project-URL: Tutorial, https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Free for non-commercial use
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: experiments
 License-File: LICENSE
 
 Constrained Monotonic Neural Networks
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
@@ -88,16 +90,14 @@
 In this example, we’ll assume we have a simple dataset with three inputs
 values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution,
 while the output value $y$ is calculated according to the following
 formula before adding Gaussian noise to it:
 
 $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 
-<style type="text/css">
-</style>
 <table id="T_37b51">
   <thead>
     <tr>
       <th id="T_37b51_level0_col0" class="col_heading level0 col0" >x0</th>
       <th id="T_37b51_level0_col1" class="col_heading level0 col1" >x1</th>
       <th id="T_37b51_level0_col2" class="col_heading level0 col2" >x2</th>
       <th id="T_37b51_level0_col3" class="col_heading level0 col3" >y</th>
```

#### html2text {}

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc2 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.0rc0 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
-Documentation, https://mono-dense-keras.airt.ai/ Keywords: tensorflow keras
-monotone "monotonic neural networks" "dense layer" Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: License :: Free for non-commercial use Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE Constrained Monotonic Neural Networks ================
-This Python library implements Monotonic Dense Layer as described in Davor
-Runje, Sharath M. Shankaranarayana, âConstrained Monotonic Neural Networksâ
-\[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\]. If you use this library,
-please cite: ``` title="bibtex" @inproceedings{runje2023, title={Constrained
-Monotonic Neural Networks}, author={Davor Runje and Sharath M.
-Shankaranarayana}, booktitle={Proceedings of the 40th {International Conference
-on Machine Learning}}, year={2023} } ``` This package contains an
-implementation of our Monotonic Dense Layer [`MonoDense`](https://
-monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
-#airt.keras.layers.MonoDense) (Constrained Monotonic Fully Connected Layer).
-Below is the figure from the paper for reference. In the code, the variable
-`monotonicity_indicator` corresponds to **t** in the figure and parameters
-`is_convex`, `is_concave` and `activation_weights` are used to calculate the
-activation selector **s** as follows: - if `is_convex` or `is_concave` is
-**True**, then the activation selector **s** will be (`units`, 0, 0) and (0,
-`units`, 0), respecively. - if both `is_convex` or `is_concave` is **False**,
-then the `activation_weights` represent ratios between $\breve{s}$, $\hat{s}$
-and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)` and
-`units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$ ![mono-
-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/
-images/mono-dense-layer-diagram.png) ## Running in Google Colab You can start
-this interactive tutorial in Google Colab by clicking the button below: [Open
-in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In this
-example, weâll assume we have a simple dataset with three inputs values
+Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
+colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
+Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: License :: Free for non-
+commercial use Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: experiments License-File: LICENSE
+Constrained Monotonic Neural Networks ================  This Python library
+implements Monotonic Dense Layer as described in Davor Runje, Sharath M.
+Shankaranarayana, âConstrained Monotonic Neural Networksâ \[[PDF](https://
+arxiv.org/pdf/2205.11775.pdf)\]. If you use this library, please cite: ```
+title="bibtex" @inproceedings{runje2023, title={Constrained Monotonic Neural
+Networks}, author={Davor Runje and Sharath M. Shankaranarayana}, booktitle=
+{Proceedings of the 40th {International Conference on Machine Learning}}, year=
+{2023} } ``` This package contains an implementation of our Monotonic Dense
+Layer [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/
+MonoDense/#airt.keras.layers.MonoDense) (Constrained Monotonic Fully Connected
+Layer). Below is the figure from the paper for reference. In the code, the
+variable `monotonicity_indicator` corresponds to **t** in the figure and
+parameters `is_convex`, `is_concave` and `activation_weights` are used to
+calculate the activation selector **s** as follows: - if `is_convex` or
+`is_concave` is **True**, then the activation selector **s** will be (`units`,
+0, 0) and (0, `units`, 0), respecively. - if both `is_convex` or `is_concave`
+is **False**, then the `activation_weights` represent ratios between $\breve
+{s}$, $\hat{s}$ and $\tilde{s}$, respecively. E.g. if `activation_weights = (2,
+2, 1)` and `units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$
+![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/
+nbs/images/mono-dense-layer-diagram.png) ## Running in Google Colab You can
+start this interactive tutorial in Google Colab by clicking the button below:
+[Open_in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In
+this example, weâll assume we have a simple dataset with three inputs values
 $x_1$, $x_2$ and $x_3$ sampled from the normal distribution, while the output
 value $y$ is calculated according to the following formula before adding
 Gaussian noise to it: $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-
 x_3}$
 x0        x1        x2        y
 0.304717  -1.039984 0.750451  0.234541
 0.940565  -1.951035 -1.302180 4.199094
```

### Comparing `monotonic-nn-0.2.0rc2/README.md` & `monotonic-nn-0.3.0rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,14 @@
 In this example, we’ll assume we have a simple dataset with three inputs
 values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution,
 while the output value $y$ is calculated according to the following
 formula before adding Gaussian noise to it:
 
 $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 
-<style type="text/css">
-</style>
 <table id="T_37b51">
   <thead>
     <tr>
       <th id="T_37b51_level0_col0" class="col_heading level0 col0" >x0</th>
       <th id="T_37b51_level0_col1" class="col_heading level0 col1" >x1</th>
       <th id="T_37b51_level0_col2" class="col_heading level0 col2" >x2</th>
       <th id="T_37b51_level0_col3" class="col_heading level0 col3" >y</th>
```

### Comparing `monotonic-nn-0.2.0rc2/airt/_components/mono_dense_layer.py` & `monotonic-nn-0.3.0rc0/airt/_components/mono_dense_layer.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc2/airt/_modidx.py` & `monotonic-nn-0.3.0rc0/airt/_modidx.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc2/airt/keras/experiments.py` & `monotonic-nn-0.3.0rc0/airt/keras/experiments.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc2/monotonic_nn.egg-info/PKG-INFO` & `monotonic-nn-0.3.0rc0/monotonic_nn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.2.0rc2
+Version: 0.3.0rc0
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
-Project-URL: Documentation, https://mono-dense-keras.airt.ai/
+Project-URL: Documentation, https://monotonic.airt.ai/
+Project-URL: Tutorial, https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Free for non-commercial use
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: experiments
 License-File: LICENSE
 
 Constrained Monotonic Neural Networks
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
@@ -88,16 +90,14 @@
 In this example, we’ll assume we have a simple dataset with three inputs
 values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution,
 while the output value $y$ is calculated according to the following
 formula before adding Gaussian noise to it:
 
 $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 
-<style type="text/css">
-</style>
 <table id="T_37b51">
   <thead>
     <tr>
       <th id="T_37b51_level0_col0" class="col_heading level0 col0" >x0</th>
       <th id="T_37b51_level0_col1" class="col_heading level0 col1" >x1</th>
       <th id="T_37b51_level0_col2" class="col_heading level0 col2" >x2</th>
       <th id="T_37b51_level0_col3" class="col_heading level0 col3" >y</th>
```

#### html2text {}

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc2 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.0rc0 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
-Documentation, https://mono-dense-keras.airt.ai/ Keywords: tensorflow keras
-monotone "monotonic neural networks" "dense layer" Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: License :: Free for non-commercial use Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE Constrained Monotonic Neural Networks ================
-This Python library implements Monotonic Dense Layer as described in Davor
-Runje, Sharath M. Shankaranarayana, âConstrained Monotonic Neural Networksâ
-\[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\]. If you use this library,
-please cite: ``` title="bibtex" @inproceedings{runje2023, title={Constrained
-Monotonic Neural Networks}, author={Davor Runje and Sharath M.
-Shankaranarayana}, booktitle={Proceedings of the 40th {International Conference
-on Machine Learning}}, year={2023} } ``` This package contains an
-implementation of our Monotonic Dense Layer [`MonoDense`](https://
-monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
-#airt.keras.layers.MonoDense) (Constrained Monotonic Fully Connected Layer).
-Below is the figure from the paper for reference. In the code, the variable
-`monotonicity_indicator` corresponds to **t** in the figure and parameters
-`is_convex`, `is_concave` and `activation_weights` are used to calculate the
-activation selector **s** as follows: - if `is_convex` or `is_concave` is
-**True**, then the activation selector **s** will be (`units`, 0, 0) and (0,
-`units`, 0), respecively. - if both `is_convex` or `is_concave` is **False**,
-then the `activation_weights` represent ratios between $\breve{s}$, $\hat{s}$
-and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)` and
-`units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$ ![mono-
-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/
-images/mono-dense-layer-diagram.png) ## Running in Google Colab You can start
-this interactive tutorial in Google Colab by clicking the button below: [Open
-in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In this
-example, weâll assume we have a simple dataset with three inputs values
+Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
+colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
+Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: License :: Free for non-
+commercial use Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: experiments License-File: LICENSE
+Constrained Monotonic Neural Networks ================  This Python library
+implements Monotonic Dense Layer as described in Davor Runje, Sharath M.
+Shankaranarayana, âConstrained Monotonic Neural Networksâ \[[PDF](https://
+arxiv.org/pdf/2205.11775.pdf)\]. If you use this library, please cite: ```
+title="bibtex" @inproceedings{runje2023, title={Constrained Monotonic Neural
+Networks}, author={Davor Runje and Sharath M. Shankaranarayana}, booktitle=
+{Proceedings of the 40th {International Conference on Machine Learning}}, year=
+{2023} } ``` This package contains an implementation of our Monotonic Dense
+Layer [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/
+MonoDense/#airt.keras.layers.MonoDense) (Constrained Monotonic Fully Connected
+Layer). Below is the figure from the paper for reference. In the code, the
+variable `monotonicity_indicator` corresponds to **t** in the figure and
+parameters `is_convex`, `is_concave` and `activation_weights` are used to
+calculate the activation selector **s** as follows: - if `is_convex` or
+`is_concave` is **True**, then the activation selector **s** will be (`units`,
+0, 0) and (0, `units`, 0), respecively. - if both `is_convex` or `is_concave`
+is **False**, then the `activation_weights` represent ratios between $\breve
+{s}$, $\hat{s}$ and $\tilde{s}$, respecively. E.g. if `activation_weights = (2,
+2, 1)` and `units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$
+![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/
+nbs/images/mono-dense-layer-diagram.png) ## Running in Google Colab You can
+start this interactive tutorial in Google Colab by clicking the button below:
+[Open_in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In
+this example, weâll assume we have a simple dataset with three inputs values
 $x_1$, $x_2$ and $x_3$ sampled from the normal distribution, while the output
 value $y$ is calculated according to the following formula before adding
 Gaussian noise to it: $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-
 x_3}$
 x0        x1        x2        y
 0.304717  -1.039984 0.750451  0.234541
 0.940565  -1.951035 -1.302180 4.199094
```

### Comparing `monotonic-nn-0.2.0rc2/settings.ini` & `monotonic-nn-0.3.0rc0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = monotonic-nn
 lib_name = %(repo)s
-version = 0.2.0rc2
+version = 0.3.0rc0
 min_python = 3.8
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = airt
 nbs_path = nbs
```

### Comparing `monotonic-nn-0.2.0rc2/setup.py` & `monotonic-nn-0.3.0rc0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,17 +25,20 @@
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
 py_versions = '3.6 3.7 3.8 3.9 3.10 3.11'.split()
 
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 
 requirements = ["tensorflow>=2.10.0"]
-    
+
+experiments_requirements = [
+    "keras-tuner[bayesian]==1.3.5"
+]
+
 dev_requirements = [
-    "keras-tuner[bayesian]==1.3.5",
     "nbdev_mkdocs==0.5.1",
     "pytest==7.3.1",
     "pandas>=1.3.5",
     "nbqa==1.7.0",
     "black==23.3.0",
     "isort==5.12.0",
     "matplotlib==3.7.1",
@@ -45,16 +48,16 @@
     "semgrep==1.23.0",
     "tqdm",
 ]
 
 project_urls = {
    'Bug Tracker': cfg['git_url'] + '/issues',
    'CI': cfg['git_url'] + '/actions',
-   'Documentation': 'https://mono-dense-keras.airt.ai/',
-#    'Tutorial': 'https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb'
+   'Documentation': 'https://monotonic.airt.ai/',
+   'Tutorial': 'https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb'
 }
 
 setuptools.setup(
     name = cfg['lib_name'],
     license = lic[0],
     classifiers = [
         'Development Status :: ' + statuses[int(cfg['status'])],
@@ -62,15 +65,15 @@
         'Natural Language :: ' + cfg['language'].title(),
     ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
     url = cfg['git_url'],
     project_urls=project_urls,
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
-    extras_require={ 'dev': dev_requirements },
+    extras_require={ 'dev': dev_requirements + experiments_requirements, "experiments": experiments_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
     entry_points = {
         'console_scripts': cfg.get('console_scripts','').split(),
```

