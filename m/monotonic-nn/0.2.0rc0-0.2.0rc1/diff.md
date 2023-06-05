# Comparing `tmp/monotonic-nn-0.2.0rc0.tar.gz` & `tmp/monotonic-nn-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic-nn-0.2.0rc0.tar", last modified: Mon Jun  5 12:09:23 2023, max compression
+gzip compressed data, was "monotonic-nn-0.2.0rc1.tar", last modified: Mon Jun  5 12:17:15 2023, max compression
```

## Comparing `monotonic-nn-0.2.0rc0.tar` & `monotonic-nn-0.2.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:09:23.130118 monotonic-nn-0.2.0rc0/
--rw-r--r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc0/LICENSE
--rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc0/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    10436 2023-06-05 12:09:23.130118 monotonic-nn-0.2.0rc0/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     9423 2023-06-05 12:06:42.000000 monotonic-nn-0.2.0rc0/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:09:23.130118 monotonic-nn-0.2.0rc0/airt/
--rw-rw-r--   0 davor     (1000) davor     (1000)       25 2023-06-05 12:09:06.000000 monotonic-nn-0.2.0rc0/airt/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:09:23.130118 monotonic-nn-0.2.0rc0/airt/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:09:06.000000 monotonic-nn-0.2.0rc0/airt/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-05 12:09:05.000000 monotonic-nn-0.2.0rc0/airt/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    31430 2023-06-05 12:09:06.000000 monotonic-nn-0.2.0rc0/airt/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     9926 2023-06-05 12:09:06.000000 monotonic-nn-0.2.0rc0/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:09:23.130118 monotonic-nn-0.2.0rc0/airt/keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:09:06.000000 monotonic-nn-0.2.0rc0/airt/keras/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14087 2023-06-05 12:09:05.000000 monotonic-nn-0.2.0rc0/airt/keras/experiments.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:09:23.130118 monotonic-nn-0.2.0rc0/airt/keras/layers/
--rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-05 12:09:06.000000 monotonic-nn-0.2.0rc0/airt/keras/layers/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:09:23.130118 monotonic-nn-0.2.0rc0/monotonic_nn.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    10436 2023-06-05 12:09:23.000000 monotonic-nn-0.2.0rc0/monotonic_nn.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-05 12:09:23.000000 monotonic-nn-0.2.0rc0/monotonic_nn.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 12:09:23.000000 monotonic-nn-0.2.0rc0/monotonic_nn.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-05 12:09:23.000000 monotonic-nn-0.2.0rc0/monotonic_nn.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 07:37:05.000000 monotonic-nn-0.2.0rc0/monotonic_nn.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      224 2023-06-05 12:09:23.000000 monotonic-nn-0.2.0rc0/monotonic_nn.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-05 12:09:23.000000 monotonic-nn-0.2.0rc0/monotonic_nn.egg-info/top_level.txt
--rw-r--r--   0 davor     (1000) davor     (1000)      919 2023-06-05 12:07:11.000000 monotonic-nn-0.2.0rc0/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-05 12:09:23.130118 monotonic-nn-0.2.0rc0/setup.cfg
--rw-r--r--   0 davor     (1000) davor     (1000)     3093 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc0/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/
+-rw-r--r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc1/LICENSE
+-rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc1/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10560 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9547 2023-06-05 12:16:54.000000 monotonic-nn-0.2.0rc1/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/airt/
+-rw-rw-r--   0 davor     (1000) davor     (1000)       25 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/airt/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/_components/helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    31430 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9926 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/_modidx.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/airt/keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/keras/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14087 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/keras/experiments.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/airt/keras/layers/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-05 12:17:06.000000 monotonic-nn-0.2.0rc1/airt/keras/layers/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10560 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/SOURCES.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/dependency_links.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/entry_points.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 07:37:05.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/not-zip-safe
+-rw-rw-r--   0 davor     (1000) davor     (1000)      224 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/requires.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-05 12:17:15.000000 monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/top_level.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)      919 2023-06-05 12:11:04.000000 monotonic-nn-0.2.0rc1/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-05 12:17:15.299773 monotonic-nn-0.2.0rc1/setup.cfg
+-rw-r--r--   0 davor     (1000) davor     (1000)     3093 2023-06-05 07:35:04.000000 monotonic-nn-0.2.0rc1/setup.py
```

### Comparing `monotonic-nn-0.2.0rc0/LICENSE` & `monotonic-nn-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc0/PKG-INFO` & `monotonic-nn-0.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Free for non-commercial use
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-Tutorial
+Constrained Monotonic Neural Networks
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This Python library implements Monotonic Dense Layer as described in
 Davor Runje, Sharath M. Shankaranarayana, “Constrained Monotonic Neural
 Networks” \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
@@ -40,15 +40,15 @@
   author={Davor Runje and Sharath M. Shankaranarayana},
   booktitle={Proceedings of the 40th {International Conference on Machine Learning}},
   year={2023}
 }
 ```
 
 This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 (Constrained Monotonic Fully Connected Layer). Below is the figure from
 the paper for reference.
 
 In the code, the variable `monotonicity_indicator` corresponds to **t**
 in the figure and parameters `is_convex`, `is_concave` and
 `activation_weights` are used to calculate the activation selector **s**
 as follows:
@@ -62,15 +62,15 @@
   and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)`
   and `units = 10`, then
 
 $$
 (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2)
 $$
 
-![mono-dense-layer-diagram](https://github.com/airtai/mono-dense-keras/raw/main/nbs/images/mono-dense-layer-diagram.png)
+![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/images/mono-dense-layer-diagram.png)
 
 ## Running in Google Colab
 
 You can start this interactive tutorial in Google Colab by clicking the
 button below:
 
 <a href="https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb" target=”_blank”>
@@ -134,18 +134,18 @@
       <td id="T_37b51_row4_col2" class="data row4 col2" >0.467509</td>
       <td id="T_37b51_row4_col3" class="data row4 col3" >0.780875</td>
     </tr>
   </tbody>
 </table>
 
 Now, we’ll use the
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 layer instead of `Dense` layer to build a simple monotonic network. By
 default, the
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 layer assumes the output of the layer is monotonically increasing with
 all inputs. This assumtion is always true for all layers except possibly
 the first one. For the first layer, we use `monotonicity_indicator` to
 specify which input parameters are monotonic and to specify are they
 increasingly or decreasingly monotonic:
 
 - set 1 for increasingly monotonic parameter,
```

#### html2text {}

```diff
@@ -1,59 +1,62 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc0 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc1 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://mono-dense-keras.airt.ai/ Keywords: tensorflow keras
 monotone "monotonic neural networks" "dense layer" Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: Free for non-commercial use Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE Tutorial ================  This Python library implements
-Monotonic Dense Layer as described in Davor Runje, Sharath M. Shankaranarayana,
-âConstrained Monotonic Neural Networksâ \[[PDF](https://arxiv.org/pdf/
-2205.11775.pdf)\]. If you use this library, please cite: ``` title="bibtex"
-@inproceedings{runje2023, title={Constrained Monotonic Neural Networks},
-author={Davor Runje and Sharath M. Shankaranarayana}, booktitle={Proceedings of
-the 40th {International Conference on Machine Learning}}, year={2023} } ```
-This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
-(Constrained Monotonic Fully Connected Layer). Below is the figure from the
-paper for reference. In the code, the variable `monotonicity_indicator`
-corresponds to **t** in the figure and parameters `is_convex`, `is_concave` and
-`activation_weights` are used to calculate the activation selector **s** as
-follows: - if `is_convex` or `is_concave` is **True**, then the activation
-selector **s** will be (`units`, 0, 0) and (0, `units`, 0), respecively. - if
-both `is_convex` or `is_concave` is **False**, then the `activation_weights`
-represent ratios between $\breve{s}$, $\hat{s}$ and $\tilde{s}$, respecively.
-E.g. if `activation_weights = (2, 2, 1)` and `units = 10`, then $$ (\breve{s},
-\hat{s}, \tilde{s}) = (4, 4, 2) $$ ![mono-dense-layer-diagram](https://
-github.com/airtai/mono-dense-keras/raw/main/nbs/images/mono-dense-layer-
-diagram.png) ## Running in Google Colab You can start this interactive tutorial
-in Google Colab by clicking the button below: [Open_in_Colab] ## Install ``` sh
-pip install monotonic-nn ``` ## How to use In this example, weâll assume we
-have a simple dataset with three inputs values $x_1$, $x_2$ and $x_3$ sampled
-from the normal distribution, while the output value $y$ is calculated
-according to the following formula before adding Gaussian noise to it: $y =
-x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
+License-File: LICENSE Constrained Monotonic Neural Networks ================
+This Python library implements Monotonic Dense Layer as described in Davor
+Runje, Sharath M. Shankaranarayana, âConstrained Monotonic Neural Networksâ
+\[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\]. If you use this library,
+please cite: ``` title="bibtex" @inproceedings{runje2023, title={Constrained
+Monotonic Neural Networks}, author={Davor Runje and Sharath M.
+Shankaranarayana}, booktitle={Proceedings of the 40th {International Conference
+on Machine Learning}}, year={2023} } ``` This package contains an
+implementation of our Monotonic Dense Layer [`MonoDense`](https://
+monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
+#airt.keras.layers.MonoDense) (Constrained Monotonic Fully Connected Layer).
+Below is the figure from the paper for reference. In the code, the variable
+`monotonicity_indicator` corresponds to **t** in the figure and parameters
+`is_convex`, `is_concave` and `activation_weights` are used to calculate the
+activation selector **s** as follows: - if `is_convex` or `is_concave` is
+**True**, then the activation selector **s** will be (`units`, 0, 0) and (0,
+`units`, 0), respecively. - if both `is_convex` or `is_concave` is **False**,
+then the `activation_weights` represent ratios between $\breve{s}$, $\hat{s}$
+and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)` and
+`units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$ ![mono-
+dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/
+images/mono-dense-layer-diagram.png) ## Running in Google Colab You can start
+this interactive tutorial in Google Colab by clicking the button below: [Open
+in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In this
+example, weâll assume we have a simple dataset with three inputs values
+$x_1$, $x_2$ and $x_3$ sampled from the normal distribution, while the output
+value $y$ is calculated according to the following formula before adding
+Gaussian noise to it: $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-
+x_3}$
 x0        x1        x2        y
 0.304717  -1.039984 0.750451  0.234541
 0.940565  -1.951035 -1.302180 4.199094
 0.127840  -0.316243 -0.016801 0.834086
 -0.853044 0.879398  0.777792  -0.093359
 0.066031  1.127241  0.467509  0.780875
-Now, weâll use the [`MonoDense`](api/airt/keras/layers/MonoDense/
-#airt.keras.layers.MonoDense) layer instead of `Dense` layer to build a simple
-monotonic network. By default, the [`MonoDense`](api/airt/keras/layers/
-MonoDense/#airt.keras.layers.MonoDense) layer assumes the output of the layer
-is monotonically increasing with all inputs. This assumtion is always true for
-all layers except possibly the first one. For the first layer, we use
+Now, weâll use the [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/
+keras/layers/MonoDense/#airt.keras.layers.MonoDense) layer instead of `Dense`
+layer to build a simple monotonic network. By default, the [`MonoDense`](https:
+//monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
+#airt.keras.layers.MonoDense) layer assumes the output of the layer is
+monotonically increasing with all inputs. This assumtion is always true for all
+layers except possibly the first one. For the first layer, we use
 `monotonicity_indicator` to specify which input parameters are monotonic and to
 specify are they increasingly or decreasingly monotonic: - set 1 for
 increasingly monotonic parameter, - set -1 for decreasingly monotonic
 parameter, and - set 0 otherwise. In our case, the `monotonicity_indicator` is
 `[1, 0, -1]` because $y$ is: - monotonically increasing w.r.t. $x_1$ $\left
 (\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and - monotonically
 decreasing w.r.t. $x_3$ $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq
```

### Comparing `monotonic-nn-0.2.0rc0/README.md` & `monotonic-nn-0.2.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Tutorial
+Constrained Monotonic Neural Networks
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This Python library implements Monotonic Dense Layer as described in
 Davor Runje, Sharath M. Shankaranarayana, “Constrained Monotonic Neural
 Networks” \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
@@ -15,15 +15,15 @@
   author={Davor Runje and Sharath M. Shankaranarayana},
   booktitle={Proceedings of the 40th {International Conference on Machine Learning}},
   year={2023}
 }
 ```
 
 This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 (Constrained Monotonic Fully Connected Layer). Below is the figure from
 the paper for reference.
 
 In the code, the variable `monotonicity_indicator` corresponds to **t**
 in the figure and parameters `is_convex`, `is_concave` and
 `activation_weights` are used to calculate the activation selector **s**
 as follows:
@@ -37,15 +37,15 @@
   and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)`
   and `units = 10`, then
 
 $$
 (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2)
 $$
 
-![mono-dense-layer-diagram](https://github.com/airtai/mono-dense-keras/raw/main/nbs/images/mono-dense-layer-diagram.png)
+![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/images/mono-dense-layer-diagram.png)
 
 ## Running in Google Colab
 
 You can start this interactive tutorial in Google Colab by clicking the
 button below:
 
 <a href="https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb" target=”_blank”>
@@ -109,18 +109,18 @@
       <td id="T_37b51_row4_col2" class="data row4 col2" >0.467509</td>
       <td id="T_37b51_row4_col3" class="data row4 col3" >0.780875</td>
     </tr>
   </tbody>
 </table>
 
 Now, we’ll use the
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 layer instead of `Dense` layer to build a simple monotonic network. By
 default, the
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 layer assumes the output of the layer is monotonically increasing with
 all inputs. This assumtion is always true for all layers except possibly
 the first one. For the first layer, we use `monotonicity_indicator` to
 specify which input parameters are monotonic and to specify are they
 increasingly or decreasingly monotonic:
 
 - set 1 for increasingly monotonic parameter,
```

#### html2text {}

```diff
@@ -1,46 +1,48 @@
-Tutorial ================  This Python library implements Monotonic Dense Layer
-as described in Davor Runje, Sharath M. Shankaranarayana, âConstrained
-Monotonic Neural Networksâ \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
-If you use this library, please cite: ``` title="bibtex" @inproceedings
-{runje2023, title={Constrained Monotonic Neural Networks}, author={Davor Runje
-and Sharath M. Shankaranarayana}, booktitle={Proceedings of the 40th
-{International Conference on Machine Learning}}, year={2023} } ``` This package
-contains an implementation of our Monotonic Dense Layer [`MonoDense`](api/airt/
-keras/layers/MonoDense/#airt.keras.layers.MonoDense) (Constrained Monotonic
-Fully Connected Layer). Below is the figure from the paper for reference. In
-the code, the variable `monotonicity_indicator` corresponds to **t** in the
-figure and parameters `is_convex`, `is_concave` and `activation_weights` are
-used to calculate the activation selector **s** as follows: - if `is_convex` or
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
 `is_concave` is **True**, then the activation selector **s** will be (`units`,
 0, 0) and (0, `units`, 0), respecively. - if both `is_convex` or `is_concave`
 is **False**, then the `activation_weights` represent ratios between $\breve
 {s}$, $\hat{s}$ and $\tilde{s}$, respecively. E.g. if `activation_weights = (2,
 2, 1)` and `units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$
-![mono-dense-layer-diagram](https://github.com/airtai/mono-dense-keras/raw/
-main/nbs/images/mono-dense-layer-diagram.png) ## Running in Google Colab You
-can start this interactive tutorial in Google Colab by clicking the button
-below: [Open_in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to
-use In this example, weâll assume we have a simple dataset with three inputs
-values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution, while the
-output value $y$ is calculated according to the following formula before adding
+![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/
+nbs/images/mono-dense-layer-diagram.png) ## Running in Google Colab You can
+start this interactive tutorial in Google Colab by clicking the button below:
+[Open_in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In
+this example, weâll assume we have a simple dataset with three inputs values
+$x_1$, $x_2$ and $x_3$ sampled from the normal distribution, while the output
+value $y$ is calculated according to the following formula before adding
 Gaussian noise to it: $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-
 x_3}$
 x0        x1        x2        y
 0.304717  -1.039984 0.750451  0.234541
 0.940565  -1.951035 -1.302180 4.199094
 0.127840  -0.316243 -0.016801 0.834086
 -0.853044 0.879398  0.777792  -0.093359
 0.066031  1.127241  0.467509  0.780875
-Now, weâll use the [`MonoDense`](api/airt/keras/layers/MonoDense/
-#airt.keras.layers.MonoDense) layer instead of `Dense` layer to build a simple
-monotonic network. By default, the [`MonoDense`](api/airt/keras/layers/
-MonoDense/#airt.keras.layers.MonoDense) layer assumes the output of the layer
-is monotonically increasing with all inputs. This assumtion is always true for
-all layers except possibly the first one. For the first layer, we use
+Now, weâll use the [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/
+keras/layers/MonoDense/#airt.keras.layers.MonoDense) layer instead of `Dense`
+layer to build a simple monotonic network. By default, the [`MonoDense`](https:
+//monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
+#airt.keras.layers.MonoDense) layer assumes the output of the layer is
+monotonically increasing with all inputs. This assumtion is always true for all
+layers except possibly the first one. For the first layer, we use
 `monotonicity_indicator` to specify which input parameters are monotonic and to
 specify are they increasingly or decreasingly monotonic: - set 1 for
 increasingly monotonic parameter, - set -1 for decreasingly monotonic
 parameter, and - set 0 otherwise. In our case, the `monotonicity_indicator` is
 `[1, 0, -1]` because $y$ is: - monotonically increasing w.r.t. $x_1$ $\left
 (\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and - monotonically
 decreasing w.r.t. $x_3$ $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq
```

### Comparing `monotonic-nn-0.2.0rc0/airt/_components/mono_dense_layer.py` & `monotonic-nn-0.2.0rc1/airt/_components/mono_dense_layer.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc0/airt/_modidx.py` & `monotonic-nn-0.2.0rc1/airt/_modidx.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc0/airt/keras/experiments.py` & `monotonic-nn-0.2.0rc1/airt/keras/experiments.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.2.0rc0/monotonic_nn.egg-info/PKG-INFO` & `monotonic-nn-0.2.0rc1/monotonic_nn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Free for non-commercial use
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-Tutorial
+Constrained Monotonic Neural Networks
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This Python library implements Monotonic Dense Layer as described in
 Davor Runje, Sharath M. Shankaranarayana, “Constrained Monotonic Neural
 Networks” \[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\].
@@ -40,15 +40,15 @@
   author={Davor Runje and Sharath M. Shankaranarayana},
   booktitle={Proceedings of the 40th {International Conference on Machine Learning}},
   year={2023}
 }
 ```
 
 This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 (Constrained Monotonic Fully Connected Layer). Below is the figure from
 the paper for reference.
 
 In the code, the variable `monotonicity_indicator` corresponds to **t**
 in the figure and parameters `is_convex`, `is_concave` and
 `activation_weights` are used to calculate the activation selector **s**
 as follows:
@@ -62,15 +62,15 @@
   and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)`
   and `units = 10`, then
 
 $$
 (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2)
 $$
 
-![mono-dense-layer-diagram](https://github.com/airtai/mono-dense-keras/raw/main/nbs/images/mono-dense-layer-diagram.png)
+![mono-dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/images/mono-dense-layer-diagram.png)
 
 ## Running in Google Colab
 
 You can start this interactive tutorial in Google Colab by clicking the
 button below:
 
 <a href="https://colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb" target=”_blank”>
@@ -134,18 +134,18 @@
       <td id="T_37b51_row4_col2" class="data row4 col2" >0.467509</td>
       <td id="T_37b51_row4_col3" class="data row4 col3" >0.780875</td>
     </tr>
   </tbody>
 </table>
 
 Now, we’ll use the
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 layer instead of `Dense` layer to build a simple monotonic network. By
 default, the
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
+[`MonoDense`](https://monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
 layer assumes the output of the layer is monotonically increasing with
 all inputs. This assumtion is always true for all layers except possibly
 the first one. For the first layer, we use `monotonicity_indicator` to
 specify which input parameters are monotonic and to specify are they
 increasingly or decreasingly monotonic:
 
 - set 1 for increasingly monotonic parameter,
```

#### html2text {}

```diff
@@ -1,59 +1,62 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc0 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.2.0rc1 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://mono-dense-keras.airt.ai/ Keywords: tensorflow keras
 monotone "monotonic neural networks" "dense layer" Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: Free for non-commercial use Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE Tutorial ================  This Python library implements
-Monotonic Dense Layer as described in Davor Runje, Sharath M. Shankaranarayana,
-âConstrained Monotonic Neural Networksâ \[[PDF](https://arxiv.org/pdf/
-2205.11775.pdf)\]. If you use this library, please cite: ``` title="bibtex"
-@inproceedings{runje2023, title={Constrained Monotonic Neural Networks},
-author={Davor Runje and Sharath M. Shankaranarayana}, booktitle={Proceedings of
-the 40th {International Conference on Machine Learning}}, year={2023} } ```
-This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](api/airt/keras/layers/MonoDense/#airt.keras.layers.MonoDense)
-(Constrained Monotonic Fully Connected Layer). Below is the figure from the
-paper for reference. In the code, the variable `monotonicity_indicator`
-corresponds to **t** in the figure and parameters `is_convex`, `is_concave` and
-`activation_weights` are used to calculate the activation selector **s** as
-follows: - if `is_convex` or `is_concave` is **True**, then the activation
-selector **s** will be (`units`, 0, 0) and (0, `units`, 0), respecively. - if
-both `is_convex` or `is_concave` is **False**, then the `activation_weights`
-represent ratios between $\breve{s}$, $\hat{s}$ and $\tilde{s}$, respecively.
-E.g. if `activation_weights = (2, 2, 1)` and `units = 10`, then $$ (\breve{s},
-\hat{s}, \tilde{s}) = (4, 4, 2) $$ ![mono-dense-layer-diagram](https://
-github.com/airtai/mono-dense-keras/raw/main/nbs/images/mono-dense-layer-
-diagram.png) ## Running in Google Colab You can start this interactive tutorial
-in Google Colab by clicking the button below: [Open_in_Colab] ## Install ``` sh
-pip install monotonic-nn ``` ## How to use In this example, weâll assume we
-have a simple dataset with three inputs values $x_1$, $x_2$ and $x_3$ sampled
-from the normal distribution, while the output value $y$ is calculated
-according to the following formula before adding Gaussian noise to it: $y =
-x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
+License-File: LICENSE Constrained Monotonic Neural Networks ================
+This Python library implements Monotonic Dense Layer as described in Davor
+Runje, Sharath M. Shankaranarayana, âConstrained Monotonic Neural Networksâ
+\[[PDF](https://arxiv.org/pdf/2205.11775.pdf)\]. If you use this library,
+please cite: ``` title="bibtex" @inproceedings{runje2023, title={Constrained
+Monotonic Neural Networks}, author={Davor Runje and Sharath M.
+Shankaranarayana}, booktitle={Proceedings of the 40th {International Conference
+on Machine Learning}}, year={2023} } ``` This package contains an
+implementation of our Monotonic Dense Layer [`MonoDense`](https://
+monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
+#airt.keras.layers.MonoDense) (Constrained Monotonic Fully Connected Layer).
+Below is the figure from the paper for reference. In the code, the variable
+`monotonicity_indicator` corresponds to **t** in the figure and parameters
+`is_convex`, `is_concave` and `activation_weights` are used to calculate the
+activation selector **s** as follows: - if `is_convex` or `is_concave` is
+**True**, then the activation selector **s** will be (`units`, 0, 0) and (0,
+`units`, 0), respecively. - if both `is_convex` or `is_concave` is **False**,
+then the `activation_weights` represent ratios between $\breve{s}$, $\hat{s}$
+and $\tilde{s}$, respecively. E.g. if `activation_weights = (2, 2, 1)` and
+`units = 10`, then $$ (\breve{s}, \hat{s}, \tilde{s}) = (4, 4, 2) $$ ![mono-
+dense-layer-diagram](https://github.com/airtai/monotonic-nn/raw/main/nbs/
+images/mono-dense-layer-diagram.png) ## Running in Google Colab You can start
+this interactive tutorial in Google Colab by clicking the button below: [Open
+in_Colab] ## Install ``` sh pip install monotonic-nn ``` ## How to use In this
+example, weâll assume we have a simple dataset with three inputs values
+$x_1$, $x_2$ and $x_3$ sampled from the normal distribution, while the output
+value $y$ is calculated according to the following formula before adding
+Gaussian noise to it: $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-
+x_3}$
 x0        x1        x2        y
 0.304717  -1.039984 0.750451  0.234541
 0.940565  -1.951035 -1.302180 4.199094
 0.127840  -0.316243 -0.016801 0.834086
 -0.853044 0.879398  0.777792  -0.093359
 0.066031  1.127241  0.467509  0.780875
-Now, weâll use the [`MonoDense`](api/airt/keras/layers/MonoDense/
-#airt.keras.layers.MonoDense) layer instead of `Dense` layer to build a simple
-monotonic network. By default, the [`MonoDense`](api/airt/keras/layers/
-MonoDense/#airt.keras.layers.MonoDense) layer assumes the output of the layer
-is monotonically increasing with all inputs. This assumtion is always true for
-all layers except possibly the first one. For the first layer, we use
+Now, weâll use the [`MonoDense`](https://monotonic.airt.ai/latest/api/airt/
+keras/layers/MonoDense/#airt.keras.layers.MonoDense) layer instead of `Dense`
+layer to build a simple monotonic network. By default, the [`MonoDense`](https:
+//monotonic.airt.ai/latest/api/airt/keras/layers/MonoDense/
+#airt.keras.layers.MonoDense) layer assumes the output of the layer is
+monotonically increasing with all inputs. This assumtion is always true for all
+layers except possibly the first one. For the first layer, we use
 `monotonicity_indicator` to specify which input parameters are monotonic and to
 specify are they increasingly or decreasingly monotonic: - set 1 for
 increasingly monotonic parameter, - set -1 for decreasingly monotonic
 parameter, and - set 0 otherwise. In our case, the `monotonicity_indicator` is
 `[1, 0, -1]` because $y$ is: - monotonically increasing w.r.t. $x_1$ $\left
 (\frac{\partial y}{x_1} = 3 {x_1}^2 \geq 0\right)$, and - monotonically
 decreasing w.r.t. $x_3$ $\left(\frac{\partial y}{x_3} = - e^{-x_2} \leq
```

### Comparing `monotonic-nn-0.2.0rc0/settings.ini` & `monotonic-nn-0.2.0rc1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = monotonic-nn
 lib_name = %(repo)s
-version = 0.2.0rc0
+version = 0.2.0rc1
 min_python = 3.8
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = airt
 nbs_path = nbs
```

### Comparing `monotonic-nn-0.2.0rc0/setup.py` & `monotonic-nn-0.2.0rc1/setup.py`

 * *Files identical despite different names*

