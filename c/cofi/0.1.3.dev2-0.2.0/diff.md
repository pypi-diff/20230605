# Comparing `tmp/cofi-0.1.3.dev2.tar.gz` & `tmp/cofi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cofi-0.1.3.dev2.tar", last modified: Wed Apr  5 13:30:58 2023, max compression
+gzip compressed data, was "cofi-0.2.0.tar", last modified: Mon Jun  5 06:30:40 2023, max compression
```

## Comparing `cofi-0.1.3.dev2.tar` & `cofi-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:30:58.980601 cofi-0.1.3.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-05 13:30:58.980601 cofi-0.1.3.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 13:30:58.980601 cofi-0.1.3.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:30:58.972601 cofi-0.1.3.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:30:58.976601 cofi-0.1.3.dev2/src/cofi/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70845 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/_base_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/_inversion_options.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 13:30:58.000000 cofi-0.1.3.dev2/src/cofi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:30:58.976601 cofi-0.1.3.dev2/src/cofi/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/tools/_base_inference_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/tools/_cofi_simple_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/tools/_emcee.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/tools/_pytorch_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/tools/_scipy_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/tools/_scipy_opt_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/tools/_scipy_opt_min.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:30:58.976601 cofi-0.1.3.dev2/src/cofi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/utils/_regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/src/cofi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:30:58.976601 cofi-0.1.3.dev2/src/cofi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-05 13:30:58.000000 cofi-0.1.3.dev2/src/cofi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-05 13:30:58.000000 cofi-0.1.3.dev2/src/cofi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 13:30:58.000000 cofi-0.1.3.dev2/src/cofi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-05 13:30:58.000000 cofi-0.1.3.dev2/src/cofi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-05 13:30:58.000000 cofi-0.1.3.dev2/src/cofi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:30:58.980601 cofi-0.1.3.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/tests/test_base_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/tests/test_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/tests/test_inversion_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-05 13:30:44.000000 cofi-0.1.3.dev2/tests/test_inversion_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.125372 cofi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-05 06:30:22.000000 cofi-0.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-05 06:30:40.125372 cofi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-05 06:30:22.000000 cofi-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-05 06:30:23.000000 cofi-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:30:40.125372 cofi-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.117371 cofi-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.121371 cofi-0.2.0/src/cofi/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67472 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/_base_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/_inversion_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.121371 cofi-0.2.0/src/cofi/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_base_inference_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_cofi_simple_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_emcee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_pytorch_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_scipy_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_scipy_opt_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/tools/_scipy_opt_min.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.121371 cofi-0.2.0/src/cofi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/utils/_reg_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/utils/_reg_lp_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/utils/_reg_model_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 06:30:23.000000 cofi-0.2.0/src/cofi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.121371 cofi-0.2.0/src/cofi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 06:30:40.000000 cofi-0.2.0/src/cofi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:30:40.125372 cofi-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_base_problem_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_base_problem_for_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_base_problem_for_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_base_problem_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_inversion_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-05 06:30:23.000000 cofi-0.2.0/tests/test_inversion_result.py
```

### Comparing `cofi-0.1.3.dev2/LICENCE` & `cofi-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/PKG-INFO` & `cofi-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofi
-Version: 0.1.3.dev2
+Version: 0.2.0
 Summary: Common Framework for Inference
 Author: InLab, CoFI development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -20,31 +20,32 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
 
 # <img src="https://raw.githubusercontent.com/inlab-geo/cofi/main/docs/source/_static/latte_art_cropped.png" width="5%" style="vertical-align:bottom"/> CoFI (Common Framework for Inference)
 
-
 [![PyPI version](https://img.shields.io/pypi/v/cofi?logo=pypi&style=flat-square&color=cae9ff&labelColor=f8f9fa)](https://pypi.org/project/cofi/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/cofi.svg?logo=condaforge&style=flat-square&color=cce3de&labelColor=f8f9fa&logoColor=344e41)](https://anaconda.org/conda-forge/cofi)
 [![Documentation Status](https://img.shields.io/readthedocs/cofi?logo=readthedocs&style=flat-square&color=fed9b7&labelColor=f8f9fa&logoColor=eaac8b)](https://cofi.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://img.shields.io/codecov/c/github/inlab-geo/cofi?logo=pytest&style=flat-square&token=T8R9VKM4D7&color=ffcad4&labelColor=f8f9fa&logoColor=ff99c8)](https://codecov.io/gh/inlab-geo/cofi)
 [![Slack](https://img.shields.io/badge/Slack-InLab_community-4A154B?logo=slack&style=flat-square&color=cdb4db&labelColor=f8f9fa&logoColor=9c89b8)](https://join.slack.com/t/inlab-community/shared_invite/zt-1ejny069z-v5ZyvP2tDjBR42OAu~TkHg)
 <!-- [![Wheels](https://img.shields.io/pypi/wheel/cofi)](https://pypi.org/project/cofi/) -->
 
+> Related repositories by [InLab](https://inlab.edu.au/community/):
+> - [CoFI Examples](https://github.com/inlab-geo/cofi-examples)
+> - [Espresso](https://github.com/inlab-geo/espresso)
 
 ## Introduction
 
 CoFI (Common Framework for Inference) is an open source initiative for interfacing between generic inference algorithms and specific geoscience problems.
 
 With a mission to bridge the gap between the domain expertise and the inference expertise, CoFI provides an interface across a wide range of inference algorithms from different sources, underpinned by a rich set of domain relevant [examples](https://cofi.readthedocs.io/en/latest/examples/generated/index.html).
 
-> This project and [documentation](https://cofi.readthedocs.io/en/latest/) are under initial development stage. Please feel free to contact us for feedback or issues!
-
+Read [the documentation](https://cofi.readthedocs.io/en/latest/), and let us know your feedback or any issues!
 
 ## Installation
 
 From PyPI:
 
 ```console
 $ pip install cofi
```

### Comparing `cofi-0.1.3.dev2/README.md` & `cofi-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 
 
 # <img src="https://raw.githubusercontent.com/inlab-geo/cofi/main/docs/source/_static/latte_art_cropped.png" width="5%" style="vertical-align:bottom"/> CoFI (Common Framework for Inference)
 
-
 [![PyPI version](https://img.shields.io/pypi/v/cofi?logo=pypi&style=flat-square&color=cae9ff&labelColor=f8f9fa)](https://pypi.org/project/cofi/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/cofi.svg?logo=condaforge&style=flat-square&color=cce3de&labelColor=f8f9fa&logoColor=344e41)](https://anaconda.org/conda-forge/cofi)
 [![Documentation Status](https://img.shields.io/readthedocs/cofi?logo=readthedocs&style=flat-square&color=fed9b7&labelColor=f8f9fa&logoColor=eaac8b)](https://cofi.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://img.shields.io/codecov/c/github/inlab-geo/cofi?logo=pytest&style=flat-square&token=T8R9VKM4D7&color=ffcad4&labelColor=f8f9fa&logoColor=ff99c8)](https://codecov.io/gh/inlab-geo/cofi)
 [![Slack](https://img.shields.io/badge/Slack-InLab_community-4A154B?logo=slack&style=flat-square&color=cdb4db&labelColor=f8f9fa&logoColor=9c89b8)](https://join.slack.com/t/inlab-community/shared_invite/zt-1ejny069z-v5ZyvP2tDjBR42OAu~TkHg)
 <!-- [![Wheels](https://img.shields.io/pypi/wheel/cofi)](https://pypi.org/project/cofi/) -->
 
+> Related repositories by [InLab](https://inlab.edu.au/community/):
+> - [CoFI Examples](https://github.com/inlab-geo/cofi-examples)
+> - [Espresso](https://github.com/inlab-geo/espresso)
 
 ## Introduction
 
 CoFI (Common Framework for Inference) is an open source initiative for interfacing between generic inference algorithms and specific geoscience problems.
 
 With a mission to bridge the gap between the domain expertise and the inference expertise, CoFI provides an interface across a wide range of inference algorithms from different sources, underpinned by a rich set of domain relevant [examples](https://cofi.readthedocs.io/en/latest/examples/generated/index.html).
 
-> This project and [documentation](https://cofi.readthedocs.io/en/latest/) are under initial development stage. Please feel free to contact us for feedback or issues!
-
+Read [the documentation](https://cofi.readthedocs.io/en/latest/), and let us know your feedback or any issues!
 
 ## Installation
 
 From PyPI:
 
 ```console
 $ pip install cofi
```

### Comparing `cofi-0.1.3.dev2/pyproject.toml` & `cofi-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/__init__.py` & `cofi-0.2.0/src/cofi/__init__.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/_base_problem.py` & `cofi-0.2.0/src/cofi/_base_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from numbers import Number
 from typing import Callable, Union, Tuple, Sequence
 import functools
 import json
 
 import numpy as np
 
+from .utils import BaseRegularization
 from ._exceptions import (
     DimensionMismatchError,
     InvalidOptionError,
     InvocationError,
     NotDefinedError,
 )
 
@@ -193,15 +194,14 @@
         BaseProblem.hessian_times_vector
         BaseProblem.residual
         BaseProblem.jacobian
         BaseProblem.jacobian_times_vector
         BaseProblem.data_misfit
         BaseProblem.regularization
         BaseProblem.regularization_matrix
-        BaseProblem.regularization_factor
         BaseProblem.forward
         BaseProblem.name
         BaseProblem.data
         BaseProblem.data_covariance
         BaseProblem.data_covariance_inv
         BaseProblem.model_covariance
         BaseProblem.model_covariance_inv
@@ -226,15 +226,14 @@
         "hessian_times_vector",
         "residual",
         "jacobian",
         "jacobian_times_vector",
         "data_misfit",
         "regularization",
         "regularization_matrix",
-        "regularization_factor",
         "forward",
         "data",
         "data_covariance",
         "data_covariance_inv",
         "initial_model",
         "model_shape",
         "blobs_dtype",
@@ -964,16 +963,15 @@
             self.data_misfit = _FunctionWrapper(
                 "data_misfit", data_misfit, args, kwargs
             )
         self._update_autogen("data_misfit")
 
     def set_regularization(
         self,
-        regularization: Union[str, Callable[[np.ndarray], Number]],
-        regularization_factor: Number = 1,
+        regularization: Union[Callable[[np.ndarray], Number], BaseRegularization],
         regularization_matrix: Union[
             np.ndarray, Callable[[np.ndarray], np.ndarray]
         ] = None,
         args: list = None,
         kwargs: dict = None,
     ):
         r"""Sets the function to compute the regularization
@@ -985,19 +983,14 @@
         { ``None``, ``"fro"``, ``"nuc"``, ``numpy.inf``, ``-numpy.inf`` } :math:`\cup\;\mathbb{R}^*`
 
         Parameters
         ----------
         regularization : str or (function - np.ndarray -> Number)
             either a string from pre-built functions above, or a regularization function that
             matches :meth:`regularization` in signature.
-        regularization_factor : Number, optional
-            the regularization factor (lamda) that adjusts the ratio of the regularization
-            term over the data misfit, by default 1. If ``regularization`` and ``data_misfit``
-            are set but ``objective`` isn't, then we will generate ``objective`` function as
-            following: :math:`\text{objective}(model)=\text{data_misfit}(model)+\text{factor}\times\text{regularization}(model)`
         regularization_matrix : np.ndarray or (function - np.ndarray -> np.ndarray)
             a matrix of shape ``(model_size, model_size)``, or a function that takes in
             a model and calculates the (weighting) matrix.
 
             - If this is None,
               :math:`\text{regularization}(model)=\lambda\times\text{regularization}(model)`
             - If this is set to be a matrix (np.ndarray, or other array like types),
@@ -1006,108 +999,57 @@
               :math:`\text{regularization}(model)=\lambda\times\text{regularization}(\text{regularization_matrix}(model)\cdot model)`
 
         args : list, optional
             extra list of positional arguments for regularization function
         kwargs : dict, optional
             extra dict of keyword arguments for regularization function
 
-        Raises
-        ------
-        InvalidOptionError
-            when you've passed in a string not in our supported regularization list
-
         Examples
         --------
 
         We demonstrate with a few examples on a ``BaseProblem`` instance.
 
         >>> from cofi import BaseProblem
         >>> inv_problem = BaseProblem()
 
-        1. Example with an L1 norm
-
-        >>> inv_problem.set_regularization(1)
-        >>> inv_problem.regularization([1,1])
-        2
-
-        2. Example with an inf norm
-
-        >>> inv_problem.set_regularization("inf")
-        >>> inv_problem.regularization([1,1])
-        1
-
-        3. Example with a custom regularization function
+        1. Example with a custom regularization function
 
         >>> inv_problem.set_regularization(lambda x: sum(x))
         >>> inv_problem.regularization([1,1])
         2
 
-        4. Example with an L2 norm and regularization factor of 0.5 (by default 1)
+        2. Example with a custom regularization + a regularization matrix
 
-        >>> inv_problem.set_regularization(2, 0.5)
+        >>> inv_problem.set_regularization(lambda x: np.sum(x**2), np.eye(3))
         >>> inv_problem.regularization([1,1])
-        0.7071067811865476
-
-        5. Example with a regularization matrix
-
-        >>> inv_problem.set_regularization(2, 0.5, np.array([[2,0], [0,1]]))
-        >>> inv_problem.regularization([1,1])
-        1.118033988749895
+        2
         """
-        # preprocess regularization_matrix
-        if np.ndim(regularization_matrix) != 0:
+        # preprocess regularization_matrix if there is one
+        _reg_matrix = None
+        if regularization_matrix is not None:
+            _reg_matrix = regularization_matrix
+        elif isinstance(regularization, BaseRegularization) and hasattr(
+            regularization, "matrix"
+        ):
+            _reg_matrix = regularization.matrix
+        # wrap regularization_matrix as a function
+        if _reg_matrix is not None and np.ndim(_reg_matrix) != 0:
             self.regularization_matrix = _FunctionWrapper(
-                "regularization_matrix", _matrix_to_func, args=[regularization_matrix]
+                "regularization_matrix", _matrix_to_func, args=[_reg_matrix]
             )
-        elif callable(regularization_matrix):
+        elif _reg_matrix is not None and callable(_reg_matrix):
             self.regularization_matrix = _FunctionWrapper(
-                "regularization_matrix", regularization_matrix
+                "regularization_matrix", _reg_matrix
             )
         else:
             self.regularization_matrix = None
-        # preprocess regularization function without lambda
-        if isinstance(regularization, (Number, str)) or not regularization:
-            order = regularization
-            if (
-                isinstance(order, str)
-                and order not in ["fro", "nuc", "inf", "-inf"]
-                or isinstance(order, Number)
-                and order < 0
-            ):
-                raise InvalidOptionError(
-                    name="regularization order",
-                    invalid_option=order,
-                    valid_options=(
-                        "[None, 'fro', 'nuc', numpy.inf, -numpy.inf] or any positive"
-                        " number"
-                    ),
-                )
-            elif isinstance(order, str) and order in ["inf", "-inf"]:
-                order = float(order)
-            _reg = _FunctionWrapper(
-                "regularization_none_lamda", np.linalg.norm, args=[order]
-            )
-        else:
-            _reg = _FunctionWrapper(
-                "regularization_none_lamda", regularization, args, kwargs
-            )
-        # wrapper function that calculates: lambda * raw regularization value
-        self._regularization_factor = regularization_factor
-        if self.regularization_matrix is None:
-            self.regularization = _FunctionWrapper(
-                "regularization",
-                _regularization_with_lamda,
-                args=[_reg, regularization_factor],
-            )
-        else:
-            self.regularization = _FunctionWrapper(
-                "regularization",
-                _regularization_with_lamda_n_matrix,
-                args=[_reg, regularization_factor, self.regularization_matrix],
-            )
+        # process regularization function
+        self.regularization = _FunctionWrapper(
+            "regularization", regularization, args, kwargs
+        )
         # update some autogenerated functions (as usual)
         self._update_autogen("regularization")
 
     def set_forward(
         self,
         forward: Callable[[np.ndarray], Union[np.ndarray, Number]],
         args: list = None,
@@ -1441,32 +1383,14 @@
             :meth:`set_log_posterior_with_blobs`)
         """
         if hasattr(self, "_blobs_dtype") and self._blobs_dtype is not None:
             return self._blobs_dtype
         raise NotDefinedError(needs="blobs name and type")
 
     @property
-    def regularization_factor(self) -> Number:
-        r"""regularization factor (lambda) that adjusts weights of the regularization
-        term
-
-        Raises
-        ------
-        NotDefinedError
-            when this property has not been defined (by
-            :meth:`set_regularization`
-        """
-        if (
-            hasattr(self, "_regularization_factor")
-            and self._regularization_factor is not None
-        ):
-            return self._regularization_factor
-        raise NotDefinedError(needs="regularization_factor (lamda)")
-
-    @property
     def bounds(self):
         r"""TODO: document me!
 
         Raises
         ------
         NotDefinedError
             when this property has not been defined (by
@@ -1594,19 +1518,14 @@
 
     @property
     def blobs_dtype_defined(self) -> bool:
         r"""indicates whether :meth:`blobs_dtype` has been defined"""
         return self._check_property_defined("blobs_dtype")
 
     @property
-    def regularization_factor_defined(self) -> bool:
-        r"""indicates whether :meth:`regularization_factor` has been defined"""
-        return self._check_property_defined("regularization_factor")
-
-    @property
     def bounds_defined(self) -> bool:
         r"""indicates whether :meth:`bounds` has been defined"""
         return self._check_property_defined("bounds")
 
     @property
     def constraints_defined(self) -> bool:
         r"""indicates whether :meth:`constraints` has been defined"""
@@ -1714,20 +1633,20 @@
 
     def _data_misfit_squared_error(self, model: np.ndarray) -> Number:
         try:
             res = self.residual(model)
             if self.data_covariance_inv_defined:
                 if _is_diag(self.data_covariance_inv):
                     weighted_res = np.diag(self.data_covariance_inv) * res
-                    return np.sum(np.square(weighted_res))
+                    return res @ weighted_res
                 else:
                     return res.T @ self.data_covariance_inv @ res
             elif self.data_covariance_defined and _is_diag(self.data_covariance):
                 weighted_res = res / np.diag(self.data_covariance)
-                return np.sum(np.square(weighted_res))
+                return res @ weighted_res
             else:
                 return np.sum(np.square(res))
         except Exception as exception:
             raise InvocationError(func_name="data misfit", autogen=True) from exception
 
     def summary(self):
         r"""Helper method that prints a summary of current ``BaseProblem`` object to
@@ -1891,22 +1810,14 @@
     except Exception as exception:
         raise InvocationError(
             func_name="jacobian_times_vector from given jacobian function",
             autogen=True,
         ) from exception
 
 
-def _regularization_with_lamda(model, reg_func, lamda):
-    return lamda * reg_func(model)
-
-
-def _regularization_with_lamda_n_matrix(model, reg_func, lamda, reg_matrix_func):
-    return lamda * reg_func(reg_matrix_func(model) @ model)
-
-
 def _matrix_to_func(_, matrix):
     return matrix
 
 
 def _is_diag(matrix):
     diag_elem = np.diag(matrix).copy()
     np.fill_diagonal(matrix, 0)
```

### Comparing `cofi-0.1.3.dev2/src/cofi/_exceptions.py` & `cofi-0.2.0/src/cofi/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/_inversion.py` & `cofi-0.2.0/src/cofi/_inversion.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/_inversion_options.py` & `cofi-0.2.0/src/cofi/_inversion_options.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/tools/__init__.py` & `cofi-0.2.0/src/cofi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/tools/_base_inference_tool.py` & `cofi-0.2.0/src/cofi/tools/_base_inference_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,16 @@
 
     def wrap_error_handler(func):
         def wrapped_func(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except Exception as e:
                 raise CofiError(
-                    f"error ocurred {when} ({context}). Check exception details "
-                    "from message above.",
+                    (
+                        f"error ocurred {when} ({context}). Check exception details "
+                        "from message above."
+                    ),
                 ) from e
 
         return wrapped_func
 
     return wrap_error_handler
```

### Comparing `cofi-0.1.3.dev2/src/cofi/tools/_cofi_simple_newton.py` & `cofi-0.2.0/src/cofi/tools/_cofi_simple_newton.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/tools/_emcee.py` & `cofi-0.2.0/src/cofi/tools/_emcee.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/tools/_pytorch_optim.py` & `cofi-0.2.0/src/cofi/tools/_pytorch_optim.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/tools/_scipy_lstsq.py` & `cofi-0.2.0/src/cofi/tools/_scipy_lstsq.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,29 +115,28 @@
         # check whether to take regularization into account
         self._params["with_tikhonov"] = (
             self._params["with_tikhonov_if_possible"]
             and inv_problem.regularization_defined
         )
         # get lamda and L matrix if needed
         if self._params["with_tikhonov"]:
-            self._lamda = inv_problem.regularization_factor
             if inv_problem.regularization_matrix_defined:
                 try:
                     _L = inv_problem.regularization_matrix(dummy_model)
                 except Exception as exception:
                     raise ValueError(
                         "regularization matrix function isn't set properly for least "
                         "squares solver, this should return a matrix unrelated to "
                         "model vector"
                     ) from exception
                 self._LtL = _L.T @ _L
                 self._components_used.append("regularization_matrix")
             else:
                 self._LtL = np.identity(self._G.shape[1])
-            self._a += self._lamda * self._LtL
+            self._a += self._LtL
 
     def __call__(self) -> dict:
         res_p, residual, rank, singular_vals = self._call_lstsq()
         res = {
             "success": True,
             "model": res_p,
             "sum_of_squared_residuals": residual,
```

### Comparing `cofi-0.1.3.dev2/src/cofi/tools/_scipy_opt_lstsq.py` & `cofi-0.2.0/src/cofi/tools/_scipy_opt_lstsq.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/src/cofi/tools/_scipy_opt_min.py` & `cofi-0.2.0/src/cofi/tools/_scipy_opt_min.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 from . import BaseInferenceTool, error_handler
 
 
 # Official documentation for scipy.optimize.minimize
 # https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html
 
-# 'jac' is only for:
+# 'jac' will be used when choosing the following methods:
 # CG, BFGS, Newton-CG, L-BFGS-B, TNC, SLSQP, dogleg, trust-ncg, trust-krylov, trust-exact
 # and trust-constr
 
-# 'hess' is only for:
+# 'hess' will be used when choosing the following methods:
 # Newton-CG, dogleg, trust-ncg, trust-krylov, trust-exact and trust-constr
 
-# 'hessp' is only for:
+# 'hessp' will be used when choosing the following methods:
 # Newton-CG, trust-ncg, trust-krylov, trust-constr
 
-# 'bounds' is only for:
+# 'bounds' will be used when choosing the following methods:
 # Nelder-Mead, L-BFGS-B, TNC, SLSQP, Powell, and trust-constr
 
-# 'constraints' is only for:
+# 'constraints' will be used when choosing the following methods:
 # COBYLA, SLSQP and trust-constr
 
 # other arguments include: tol, options, callback
 
 
 class ScipyOptMin(BaseInferenceTool):
     documentation_links = [
```

### Comparing `cofi-0.1.3.dev2/src/cofi.egg-info/PKG-INFO` & `cofi-0.2.0/src/cofi.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofi
-Version: 0.1.3.dev2
+Version: 0.2.0
 Summary: Common Framework for Inference
 Author: InLab, CoFI development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -20,31 +20,32 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
 
 # <img src="https://raw.githubusercontent.com/inlab-geo/cofi/main/docs/source/_static/latte_art_cropped.png" width="5%" style="vertical-align:bottom"/> CoFI (Common Framework for Inference)
 
-
 [![PyPI version](https://img.shields.io/pypi/v/cofi?logo=pypi&style=flat-square&color=cae9ff&labelColor=f8f9fa)](https://pypi.org/project/cofi/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/cofi.svg?logo=condaforge&style=flat-square&color=cce3de&labelColor=f8f9fa&logoColor=344e41)](https://anaconda.org/conda-forge/cofi)
 [![Documentation Status](https://img.shields.io/readthedocs/cofi?logo=readthedocs&style=flat-square&color=fed9b7&labelColor=f8f9fa&logoColor=eaac8b)](https://cofi.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://img.shields.io/codecov/c/github/inlab-geo/cofi?logo=pytest&style=flat-square&token=T8R9VKM4D7&color=ffcad4&labelColor=f8f9fa&logoColor=ff99c8)](https://codecov.io/gh/inlab-geo/cofi)
 [![Slack](https://img.shields.io/badge/Slack-InLab_community-4A154B?logo=slack&style=flat-square&color=cdb4db&labelColor=f8f9fa&logoColor=9c89b8)](https://join.slack.com/t/inlab-community/shared_invite/zt-1ejny069z-v5ZyvP2tDjBR42OAu~TkHg)
 <!-- [![Wheels](https://img.shields.io/pypi/wheel/cofi)](https://pypi.org/project/cofi/) -->
 
+> Related repositories by [InLab](https://inlab.edu.au/community/):
+> - [CoFI Examples](https://github.com/inlab-geo/cofi-examples)
+> - [Espresso](https://github.com/inlab-geo/espresso)
 
 ## Introduction
 
 CoFI (Common Framework for Inference) is an open source initiative for interfacing between generic inference algorithms and specific geoscience problems.
 
 With a mission to bridge the gap between the domain expertise and the inference expertise, CoFI provides an interface across a wide range of inference algorithms from different sources, underpinned by a rich set of domain relevant [examples](https://cofi.readthedocs.io/en/latest/examples/generated/index.html).
 
-> This project and [documentation](https://cofi.readthedocs.io/en/latest/) are under initial development stage. Please feel free to contact us for feedback or issues!
-
+Read [the documentation](https://cofi.readthedocs.io/en/latest/), and let us know your feedback or any issues!
 
 ## Installation
 
 From PyPI:
 
 ```console
 $ pip install cofi
```

### Comparing `cofi-0.1.3.dev2/src/cofi.egg-info/SOURCES.txt` & `cofi-0.2.0/src/cofi.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -18,13 +18,18 @@
 src/cofi/tools/_cofi_simple_newton.py
 src/cofi/tools/_emcee.py
 src/cofi/tools/_pytorch_optim.py
 src/cofi/tools/_scipy_lstsq.py
 src/cofi/tools/_scipy_opt_lstsq.py
 src/cofi/tools/_scipy_opt_min.py
 src/cofi/utils/__init__.py
-src/cofi/utils/_regularization.py
-tests/test_base_problem.py
+src/cofi/utils/_reg_base.py
+src/cofi/utils/_reg_lp_norm.py
+src/cofi/utils/_reg_model_cov.py
+tests/test_base_problem_basics.py
+tests/test_base_problem_for_optimization.py
+tests/test_base_problem_for_sampling.py
+tests/test_base_problem_misc.py
 tests/test_deprecation.py
 tests/test_inversion.py
 tests/test_inversion_options.py
 tests/test_inversion_result.py
```

### Comparing `cofi-0.1.3.dev2/tests/test_inversion.py` & `cofi-0.2.0/tests/test_inversion.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/tests/test_inversion_options.py` & `cofi-0.2.0/tests/test_inversion_options.py`

 * *Files identical despite different names*

### Comparing `cofi-0.1.3.dev2/tests/test_inversion_result.py` & `cofi-0.2.0/tests/test_inversion_result.py`

 * *Files identical despite different names*

