# Comparing `tmp/cvxreg-0.0.5.tar.gz` & `tmp/cvxreg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxreg-0.0.5.tar", last modified: Sat Jun  3 20:58:30 2023, max compression
+gzip compressed data, was "cvxreg-0.0.6.tar", last modified: Mon Jun  5 17:27:08 2023, max compression
```

## Comparing `cvxreg-0.0.5.tar` & `cvxreg-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.744887 cvxreg-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 20:58:20.000000 cvxreg-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-03 20:58:30.744887 cvxreg-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-03 20:58:20.000000 cvxreg-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.740887 cvxreg-0.0.5/cvxreg/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.744887 cvxreg-0.0.5/cvxreg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/models/_penalized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.744887 cvxreg-0.0.5/cvxreg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/utils/extmath.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-03 20:58:20.000000 cvxreg-0.0.5/cvxreg/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:58:30.744887 cvxreg-0.0.5/cvxreg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 20:58:30.000000 cvxreg-0.0.5/cvxreg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 20:58:30.744887 cvxreg-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-03 20:58:20.000000 cvxreg-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-05 17:26:58.000000 cvxreg-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-05 17:27:08.175946 cvxreg-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-05 17:26:58.000000 cvxreg-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/cvxreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/cvxreg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/models/_penalized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/cvxreg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/_param_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/extmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/cvxreg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:27:08.175946 cvxreg-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 17:26:58.000000 cvxreg-0.0.6/setup.py
```

### Comparing `cvxreg-0.0.5/LICENSE` & `cvxreg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.5/PKG-INFO` & `cvxreg-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/ConvexRegression
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
@@ -12,17 +12,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
+[![PyPI version](https://img.shields.io/pypi/v/cvxreg.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
-**pycreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+**cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
 * interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
```

### Comparing `cvxreg-0.0.5/README.md` & `cvxreg-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
+[![PyPI version](https://img.shields.io/pypi/v/cvxreg.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
-**pycreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+**cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
 * interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
```

### Comparing `cvxreg-0.0.5/cvxreg/models/_base.py` & `cvxreg-0.0.6/cvxreg/models/_penalized.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,99 @@
-# import dependencies
-from abc import ABCMeta, abstractmethod
+from numbers import Real
+
 import numpy as np
 import pandas as pd
 from pystoned import CNLS
+from pyomo.environ import Objective, minimize
 
-from ..base import BaseEstimator
+from ._base import CRModel
 from ..constant import Convex, Concave, OPT_DEFAULT, OPT_LOCAL
 from ..utils import tools
-from ..utils.extmath import yhat
+from ..utils._param_check import Interval, StrOptions
 
-class CRModel(BaseEstimator, metaclass=ABCMeta):
-    """
-    Base class for CR models
-    """
-    @abstractmethod
-    def fit(self):
-        """Fit model."""
 
-    def _decision_function(self, x):
-        tools.assert_optimized(self.optimization_status)
-        
-        x = self._validate_data(x)
-        y_hat = yhat(self.intercept_, self.coef_, x, fun=self.shape)
-        return y_hat
-    
-    def predict(self, x):
-        """
-        Predict the output variable
-
-        Args:
-            x (float): input variables.
-
-        Returns:
-            float: predicted output variable
-        """
-        return self._decision_function(x)
-    
-
-class CR(CRModel, CNLS.CNLS):
+class PCR(CRModel, CNLS.CNLS):
     """
-    Convex Regression (CR) model
+    Penalized Convex Regression (PCR) model
     """
 
-    def __init__(self, x, y, shape=Convex, positive=False, fit_intercept=True):
-        """CNLS model
+    _parameter_constraints: dict = {
+        "c": [Interval(Real, 0, None)],
+        "shape": [StrOptions({Convex, Concave})],
+        'fit_intercept': ['boolean'],
+        'positive': ['boolean']
+    }
+
+    def __init__(self, c=1.0, shape=Convex, positive=False, fit_intercept=True):
+        """PCR model
 
         Args:
             y (float): output variable. 
             x (float): input variables.
             fun (String, optional): FUN_CVX (convex funtion) or FUN_CCV (concave funtion). Defaults to FUN_CVX.
             positive (bool, optional): True if the coefficients are positive. Defaults to False.
             fit_intercept (bool, optional): True if the model should include an intercept. Defaults to True.
         """
         
+        self.c = c
         self.shape = shape
         self.fit_intercept = fit_intercept
         self.positive = positive
 
+    def fit(self, x, y, email=OPT_LOCAL, solver=OPT_DEFAULT):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        self._validate_params()
+        x, y = self._validate_data(x, y)
+
         if self.shape == Convex:
             fun_var = CNLS.FUN_COST
         elif self.shape == Concave:
             fun_var = CNLS.FUN_PROD
-        CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=fun_var, rts=CNLS.RTS_CRS)
+        if self.fit_intercept:
+            intercept = CNLS.RTS_VRS
+        else:
+            intercept = CNLS.RTS_CRS
+        CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=fun_var, rts=intercept)
 
-        if self.positive is True:
+        # new objective function
+        self.__model__.objective.deactivate()
+        self.__model__.new_objective = Objective(rule=self.__new_objective_rule(),
+                                                     sense=minimize,
+                                                     doc='objective function')
+
+        if self.positive:
             self.__model__.beta.setlb(0.0)
         else:
             self.__model__.beta.setlb(None)
 
-
-    def fit(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
         # TODO(error/warning handling): Check problem status after optimization
         self.problem_status, self.optimization_status = tools.optimize_model(
             self.__model__, email, solver)
         
         tools.assert_optimized(self.optimization_status)
-        tools.assert_various_return_to_scale(self.fit_intercept)
 
         alpha = list(self.__model__.alpha[:].value)
 
         beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
                                                           list(self.__model__.beta[:, :].value))])
         beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
         beta = beta.pivot(index='Name', columns='Key', values='Value')
     
         if self.fit_intercept:
-            self.intercept_ = np.array(alpha)
+            self.intercept_ = alpha
             self.coef_ = beta.to_numpy()
         else:
             self.intercept_ = 0.0
             self.coef_ = beta.to_numpy()
-
         return self
+    
+    def __new_objective_rule(self):
+        """return new objective function"""
+        def objective_rule(model):
+            return sum(model.epsilon[i] ** 2 for i in model.I) \
+                + self.c * sum(model.beta[i, j] ** 2 for i in model.I for j in model.J)
+        return objective_rule
```

### Comparing `cvxreg-0.0.5/cvxreg/utils/check.py` & `cvxreg-0.0.6/cvxreg/utils/check.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.5/cvxreg/utils/extmath.py` & `cvxreg-0.0.6/cvxreg/utils/extmath.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     refers to equation (4.1) in journal article:
     "Representation theorem for convex nonparametric least squares. Timo Kuosmanen (2008)"
     input:
     alpha and beta are regression coefficients; x_test is the input of test sample.
     output:
     return the estimated y_hat.
     '''
-
     # check the dimension of input
     if beta.shape[1] != x_test.shape[1]:
         raise ValueError('beta and x_test should have the same number of dimensions.')
     else:
         # compute yhat for each testing observation
         yhat = np.zeros((len(x_test),))
         for i in range(len(x_test)):
```

### Comparing `cvxreg-0.0.5/cvxreg.egg-info/PKG-INFO` & `cvxreg-0.0.6/cvxreg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/ConvexRegression
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
@@ -12,17 +12,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
+[![PyPI version](https://img.shields.io/pypi/v/cvxreg.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
-**pycreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+**cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
 * interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
```

### Comparing `cvxreg-0.0.5/setup.py` & `cvxreg-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='cvxreg',
-    version='0.0.5',
+    version='0.0.6',
     description='A Python Package for Convex Regression',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Zhiqiang Liao',
     author_email='zhiqiang.liao@aalto.fi',
```

