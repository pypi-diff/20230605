# Comparing `tmp/LinSATNet-0.0.3.tar.gz` & `tmp/LinSATNet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LinSATNet-0.0.3.tar", last modified: Mon Jun  5 10:14:25 2023, max compression
+gzip compressed data, was "LinSATNet-0.0.4.tar", last modified: Mon Jun  5 10:17:59 2023, max compression
```

## Comparing `LinSATNet-0.0.3.tar` & `LinSATNet-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:14:25.960266 LinSATNet-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 10:14:16.000000 LinSATNet-0.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:14:25.960266 LinSATNet-0.0.3/LinSATNet/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 10:14:16.000000 LinSATNet-0.0.3/LinSATNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-05 10:14:16.000000 LinSATNet-0.0.3/LinSATNet/linsat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:14:25.960266 LinSATNet-0.0.3/LinSATNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-05 10:14:25.000000 LinSATNet-0.0.3/LinSATNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 10:14:25.000000 LinSATNet-0.0.3/LinSATNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:14:25.000000 LinSATNet-0.0.3/LinSATNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 10:14:25.000000 LinSATNet-0.0.3/LinSATNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 10:14:25.000000 LinSATNet-0.0.3/LinSATNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-05 10:14:25.960266 LinSATNet-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-06-05 10:14:16.000000 LinSATNet-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:14:25.960266 LinSATNet-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-05 10:14:17.000000 LinSATNet-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 10:17:50.000000 LinSATNet-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/LinSATNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 10:17:50.000000 LinSATNet-0.0.4/LinSATNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-05 10:17:50.000000 LinSATNet-0.0.4/LinSATNet/linsat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/LinSATNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 10:17:59.000000 LinSATNet-0.0.4/LinSATNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18800 2023-06-05 10:17:50.000000 LinSATNet-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:17:59.943541 LinSATNet-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-05 10:17:51.000000 LinSATNet-0.0.4/setup.py
```

### Comparing `LinSATNet-0.0.3/LICENSE` & `LinSATNet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `LinSATNet-0.0.3/LinSATNet/linsat.py` & `LinSATNet-0.0.4/LinSATNet/linsat.py`

 * *Files identical despite different names*

### Comparing `LinSATNet-0.0.3/LinSATNet.egg-info/PKG-INFO` & `LinSATNet-0.0.4/LinSATNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.3
+Version: 0.0.4
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -55,15 +55,15 @@
 ```
 
 In this example, we try to enforce doubly-stochastic constraint to a 3x3 matrix.
 The doubly-stochastic constraint means that all rows and columns of the matrix
 should sum to 1.
 
 The 3x3 matrix is flattened into a vector, and the following positive
-linear constraints are considered (for $`\mathbf{E}\mathbf{x}=\mathbf{f}`$):
+linear constraints are considered (for $\mathbf{E}\mathbf{x}=\mathbf{f}$):
 ```python
 E = torch.tensor(
     [[1, 1, 1, 0, 0, 0, 0, 0, 0],
      [0, 0, 0, 1, 1, 1, 0, 0, 0],
      [0, 0, 0, 0, 0, 0, 1, 1, 1],
      [1, 0, 0, 1, 0, 0, 1, 0, 0],
      [0, 1, 0, 0, 1, 0, 0, 1, 0],
@@ -151,15 +151,15 @@
 * ``max_iter``: (``default=100``) max number of iterations
 * ``dummy_val``: (``default=0``) the value of dummy variables appended to the input vector
 
 **return:** PyTorch tensor of size ($n_v$) or ($b \times n_v$), the projected variables
 
 Notations:
 * $b$ means the batch size.
-* $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $`n_c`$s)
+* $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $n_c$)
 * $n_v$ means the number of variables
 
 ### Some practical notes
 
 1. You must ensure that your input constraints have a non-empty feasible space.
 Otherwise, ``linsat_layer`` will not converge.
 2. You may tune the value of ``tau`` for your specific tasks. Monitor the output
```

### Comparing `LinSATNet-0.0.3/PKG-INFO` & `LinSATNet-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.3
+Version: 0.0.4
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -55,15 +55,15 @@
 ```
 
 In this example, we try to enforce doubly-stochastic constraint to a 3x3 matrix.
 The doubly-stochastic constraint means that all rows and columns of the matrix
 should sum to 1.
 
 The 3x3 matrix is flattened into a vector, and the following positive
-linear constraints are considered (for $`\mathbf{E}\mathbf{x}=\mathbf{f}`$):
+linear constraints are considered (for $\mathbf{E}\mathbf{x}=\mathbf{f}$):
 ```python
 E = torch.tensor(
     [[1, 1, 1, 0, 0, 0, 0, 0, 0],
      [0, 0, 0, 1, 1, 1, 0, 0, 0],
      [0, 0, 0, 0, 0, 0, 1, 1, 1],
      [1, 0, 0, 1, 0, 0, 1, 0, 0],
      [0, 1, 0, 0, 1, 0, 0, 1, 0],
@@ -151,15 +151,15 @@
 * ``max_iter``: (``default=100``) max number of iterations
 * ``dummy_val``: (``default=0``) the value of dummy variables appended to the input vector
 
 **return:** PyTorch tensor of size ($n_v$) or ($b \times n_v$), the projected variables
 
 Notations:
 * $b$ means the batch size.
-* $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $`n_c`$s)
+* $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $n_c$)
 * $n_v$ means the number of variables
 
 ### Some practical notes
 
 1. You must ensure that your input constraints have a non-empty feasible space.
 Otherwise, ``linsat_layer`` will not converge.
 2. You may tune the value of ``tau`` for your specific tasks. Monitor the output
```

### Comparing `LinSATNet-0.0.3/README.md` & `LinSATNet-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ```
 
 In this example, we try to enforce doubly-stochastic constraint to a 3x3 matrix.
 The doubly-stochastic constraint means that all rows and columns of the matrix
 should sum to 1.
 
 The 3x3 matrix is flattened into a vector, and the following positive
-linear constraints are considered (for $`\mathbf{E}\mathbf{x}=\mathbf{f}`$):
+linear constraints are considered (for $\mathbf{E}\mathbf{x}=\mathbf{f}$):
 ```python
 E = torch.tensor(
     [[1, 1, 1, 0, 0, 0, 0, 0, 0],
      [0, 0, 0, 1, 1, 1, 0, 0, 0],
      [0, 0, 0, 0, 0, 0, 1, 1, 1],
      [1, 0, 0, 1, 0, 0, 1, 0, 0],
      [0, 1, 0, 0, 1, 0, 0, 1, 0],
@@ -153,15 +153,15 @@
 * ``max_iter``: (``default=100``) max number of iterations
 * ``dummy_val``: (``default=0``) the value of dummy variables appended to the input vector
 
 **return:** PyTorch tensor of size ($n_v$) or ($b \times n_v$), the projected variables
 
 Notations:
 * $b$ means the batch size.
-* $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $`n_c`$s)
+* $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $n_c$)
 * $n_v$ means the number of variables
 
 ### Some practical notes
 
 1. You must ensure that your input constraints have a non-empty feasible space.
 Otherwise, ``linsat_layer`` will not converge.
 2. You may tune the value of ``tau`` for your specific tasks. Monitor the output
```

### Comparing `LinSATNet-0.0.3/setup.py` & `LinSATNet-0.0.4/setup.py`

 * *Files identical despite different names*

