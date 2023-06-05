# Comparing `tmp/spherediff-1.2.0.tar.gz` & `tmp/spherediff-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/kormos/spherediff/dist/.tmp-yjpk4dce/spherediff-1.2.0.tar", last modified: Tue May 30 02:21:09 2023, max compression
+gzip compressed data, was "/home/kormos/spherediff/dist/.tmp-lzfndteu/spherediff-1.2.1.tar", last modified: Mon Jun  5 07:31:21 2023, max compression
```

## Comparing `spherediff-1.2.0.tar` & `spherediff-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-30 02:21:09.692022 spherediff-1.2.0/
--rw-r--r--   0 kormos    (1000) kormos    (1000)     1068 2023-05-22 22:12:37.000000 spherediff-1.2.0/LICENSE.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)     4973 2023-05-30 02:21:09.692022 spherediff-1.2.0/PKG-INFO
--rw-r--r--   0 kormos    (1000) kormos    (1000)     4477 2023-05-30 00:39:12.000000 spherediff-1.2.0/README.md
--rw-r--r--   0 kormos    (1000) kormos    (1000)      766 2023-05-30 00:39:23.000000 spherediff-1.2.0/pyproject.toml
--rw-r--r--   0 kormos    (1000) kormos    (1000)       38 2023-05-30 02:21:09.692022 spherediff-1.2.0/setup.cfg
--rw-r--r--   0 kormos    (1000) kormos    (1000)       50 2023-05-22 21:59:35.000000 spherediff-1.2.0/setup.py
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-30 02:21:09.692022 spherediff-1.2.0/src/
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-30 02:21:09.692022 spherediff-1.2.0/src/spherediff/
--rw-r--r--   0 kormos    (1000) kormos    (1000)        0 2023-05-08 23:09:07.000000 spherediff-1.2.0/src/spherediff/__init__.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     8087 2023-05-29 03:14:23.000000 spherediff-1.2.0/src/spherediff/coeffs.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)    11140 2023-05-30 02:11:22.000000 spherediff-1.2.0/src/spherediff/kernel.py
--rwxr-xr-x   0 kormos    (1000) kormos    (1000)     4459 2023-05-29 03:14:23.000000 spherediff-1.2.0/src/spherediff/poly.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2332 2023-05-30 02:13:29.000000 spherediff-1.2.0/src/spherediff/sample.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     1176 2023-05-29 19:35:49.000000 spherediff-1.2.0/src/spherediff/score.py
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-30 02:21:09.692022 spherediff-1.2.0/src/spherediff.egg-info/
--rw-r--r--   0 kormos    (1000) kormos    (1000)     4973 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/PKG-INFO
--rw-r--r--   0 kormos    (1000) kormos    (1000)      383 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/SOURCES.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)        1 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/dependency_links.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)       75 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/requires.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)       11 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/top_level.txt
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-05 07:31:21.774713 spherediff-1.2.1/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     1068 2023-05-22 22:12:37.000000 spherediff-1.2.1/LICENSE.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     5856 2023-06-05 07:31:21.774713 spherediff-1.2.1/PKG-INFO
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     5360 2023-06-05 07:24:48.000000 spherediff-1.2.1/README.md
+-rw-r--r--   0 kormos    (1000) kormos    (1000)      766 2023-06-05 07:03:08.000000 spherediff-1.2.1/pyproject.toml
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       38 2023-06-05 07:31:21.774713 spherediff-1.2.1/setup.cfg
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       50 2023-05-22 21:59:35.000000 spherediff-1.2.1/setup.py
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-05 07:31:21.764713 spherediff-1.2.1/src/
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-05 07:31:21.774713 spherediff-1.2.1/src/spherediff/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)        0 2023-05-08 23:09:07.000000 spherediff-1.2.1/src/spherediff/__init__.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     8087 2023-05-29 03:14:23.000000 spherediff-1.2.1/src/spherediff/coeffs.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)    11140 2023-05-30 02:11:22.000000 spherediff-1.2.1/src/spherediff/kernel.py
+-rwxr-xr-x   0 kormos    (1000) kormos    (1000)     4459 2023-05-29 03:14:23.000000 spherediff-1.2.1/src/spherediff/poly.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     2332 2023-06-05 07:12:18.000000 spherediff-1.2.1/src/spherediff/sample.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     1423 2023-06-05 07:12:07.000000 spherediff-1.2.1/src/spherediff/score.py
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-05 07:31:21.774713 spherediff-1.2.1/src/spherediff.egg-info/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     5856 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/PKG-INFO
+-rw-r--r--   0 kormos    (1000) kormos    (1000)      383 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/SOURCES.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)        1 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/dependency_links.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       75 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/requires.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       11 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/top_level.txt
```

### Comparing `spherediff-1.2.0/LICENSE.txt` & `spherediff-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spherediff-1.2.0/PKG-INFO` & `spherediff-1.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: spherediff
-Version: 1.2.0
-Summary: Sample from the diffusion kernel on any n-sphere
-Author-email: Rian Kormos <Rian.Kormos@ucsf.edu>
-Project-URL: Homepage, https://github.com/rckormos/SphereDiff
-Keywords: diffusion,hypersphere,sampling
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # SphereDiff
 
 ## Purpose
 
 The purpose of this package is to sample from the isotropic diffusion kernel 
 on the surface of an n-dimensional unit sphere, where n is an arbitrary 
 natural number dimension greater than or equal to 3.
@@ -88,22 +74,25 @@
 of the logarithm of the probability density. This may be done using the 
 `score_spherical_kernel` function, which may be imported as follows:
 
 ```
 from spherediff.score import score_spherical_kernel
 ```
 
-This function takes four arguments. The first is n, the dimension of the 
-space in which the n-sphere is embedded. The second is a numpy array of 
-shape (N, n) consisting of the n-dimensional unit vectors at which to 
-evaluate the score function. The third is a numpy array of shape (N, n) 
-consisting of the n-dimensional unit vectors at which to center the 
-distributions of which the corresponding score functions will be evaluated. 
-The fourth is a numpy array of shape (N,) consisting of the scalar variance 
-parameters of each distribution.
+This function takes four arguments and one additional, optional argument. 
+The first is n, the dimension of the space in which the n-sphere is embedded. 
+The second is a numpy array of shape (N, n) consisting of the n-dimensional 
+unit vectors at which to evaluate the score function. The third is a numpy 
+array of shape (N, n) consisting of the n-dimensional unit vectors at which 
+to center the distributions of which the corresponding score functions will 
+be evaluated. The fourth is a numpy array of shape (N,) consisting of the 
+scalar variance parameters of each distribution. The fifth is a boolean 
+flag that determines whether the distributions of interest are supported 
+on the full surface of the n-sphere (if False) or on the hemisphere with 
+reflecting boundary conditions for the diffusion kernel.
 
 Example output from `score_spherical_kernel` is:
 
 ```
 >>> import numpy as np
 >>> from spherediff.sample import sample_spherical_kernel
 >>> from spherediff.score import score_spherical_kernel
@@ -121,13 +110,26 @@
 >>> x
 array([[ 0.30027556, -0.53104481,  0.79235472],
        [ 0.91657116, -0.39288942,  0.07439905],
        [ 0.81325411,  0.41495422, -0.40795926],
        [ 0.39907791, -0.44171124, -0.80350981],
        [ 0.16422958, -0.76019121, -0.62860001]])
 >>> score_spherical_kernel(3, x, means, vars)
-array([[ 0.45383257, -1.4484151 , -0.34370955],
-       [ 2.57268711,  3.50638512, -2.19627206],
-       [ 0.33420178,  5.16225326, -0.64669865],
-       [ 2.62797084,  2.20685896, -1.97070763],
-       [-3.68698876, -0.78777185, -3.71349795]])
+array([[ 3.40175815,  3.11417869,  0.79800571],
+       [ 1.12626049,  2.20918798, -2.20878198],
+       [ 0.65201631,  0.12437106,  1.42627781],
+       [ 2.65653386, -1.32241858,  2.04638588],
+       [-0.69053884,  0.17827374, -0.39600546]])
+>>> x = sample_spherical_kernel(3, means, vars, hemisphere=True)
+>>> x
+array([[ 0.92723597,  0.02336567,  0.37374791],
+       [ 0.99421791, -0.03878944, -0.10013055],
+       [ 0.15771025,  0.6492883 , -0.74401087],
+       [ 0.2418101 , -0.41127436, -0.87885225],
+       [-0.11192408, -0.71437847, -0.69075061]])
+>>> score_spherical_kernel(3, x, means, vars, hemisphere=True)
+array([[-1.74036155, -1.77246139,  4.42849462],
+       [-0.0852985 , -1.00528069, -0.45751298],
+       [ 2.51709283,  0.09916178,  0.62009298],
+       [ 4.08775888, -1.8186883 ,  1.97580568],
+       [ 1.8912707 , -0.37819329,  0.08468239]])
 ```
```

### Comparing `spherediff-1.2.0/pyproject.toml` & `spherediff-1.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spherediff"
-version = "1.2.0"
+version = "1.2.1"
 description = "Sample from the diffusion kernel on any n-sphere"
 readme = "README.md"
 authors = [{name = "Rian Kormos", email = "Rian.Kormos@ucsf.edu"}]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License", 
     "Programming Language :: Python",
```

### Comparing `spherediff-1.2.0/src/spherediff/coeffs.py` & `spherediff-1.2.1/src/spherediff/coeffs.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.2.0/src/spherediff/kernel.py` & `spherediff-1.2.1/src/spherediff/kernel.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.2.0/src/spherediff/poly.py` & `spherediff-1.2.1/src/spherediff/poly.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.2.0/src/spherediff/sample.py` & `spherediff-1.2.1/src/spherediff/sample.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.2.0/src/spherediff/score.py` & `spherediff-1.2.1/src/spherediff/score.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from .kernel import *
 
-def score_spherical_kernel(n, x, mean, var):
+def score_spherical_kernel(n, x, mean, var, hemisphere=False):
     """Compute the score function from the diffusion kernel on the n-D sphere.
 
     Parameters
     ----------
     n : int
         The dimensionality of the space in which the spherical surface is 
         embedded.
     x : np.array [N x n]
         The n-dimensional unit vectors at which to compute the score.
     mean : np.array [N x n]
         The n-dimensional unit vectors to be used as the means of the 
         distributions according to which to compute the score.
     var : np.array [N] 
         Scalar variances of the distributions for each vector.
+    hemisphere : bool
+        If True, sample on the n-hemisphere instead of the n-sphere.
 
     Returns
     -------
     score : np.array [N x n]
         The score function evaluated at each point x.
     """
     assert x.shape[0] == mean.shape[0] and x.shape[1] == mean.shape[1]
@@ -26,8 +28,12 @@
     assert len(mean[0]) == n
     N = len(var)
     projections = (x * mean).sum(axis=1, keepdims=True)
     phi = np.arccos(projections)
     rejections = mean - projections * x
     rejections /= -np.linalg.norm(rejections, axis=1, keepdims=True)
     ker, ker_deriv = raw_kernel(n, var, phi)
+    if hemisphere:
+        ker_rev, ker_deriv_rev = kernel(n, var, np.pi - phi)
+        ker += ker_rev
+        ker_deriv += ker_deriv_rev
     return rejections * ker_deriv / ker
```

### Comparing `spherediff-1.2.0/src/spherediff.egg-info/PKG-INFO` & `spherediff-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherediff
-Version: 1.2.0
+Version: 1.2.1
 Summary: Sample from the diffusion kernel on any n-sphere
 Author-email: Rian Kormos <Rian.Kormos@ucsf.edu>
 Project-URL: Homepage, https://github.com/rckormos/SphereDiff
 Keywords: diffusion,hypersphere,sampling
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -88,22 +88,25 @@
 of the logarithm of the probability density. This may be done using the 
 `score_spherical_kernel` function, which may be imported as follows:
 
 ```
 from spherediff.score import score_spherical_kernel
 ```
 
-This function takes four arguments. The first is n, the dimension of the 
-space in which the n-sphere is embedded. The second is a numpy array of 
-shape (N, n) consisting of the n-dimensional unit vectors at which to 
-evaluate the score function. The third is a numpy array of shape (N, n) 
-consisting of the n-dimensional unit vectors at which to center the 
-distributions of which the corresponding score functions will be evaluated. 
-The fourth is a numpy array of shape (N,) consisting of the scalar variance 
-parameters of each distribution.
+This function takes four arguments and one additional, optional argument. 
+The first is n, the dimension of the space in which the n-sphere is embedded. 
+The second is a numpy array of shape (N, n) consisting of the n-dimensional 
+unit vectors at which to evaluate the score function. The third is a numpy 
+array of shape (N, n) consisting of the n-dimensional unit vectors at which 
+to center the distributions of which the corresponding score functions will 
+be evaluated. The fourth is a numpy array of shape (N,) consisting of the 
+scalar variance parameters of each distribution. The fifth is a boolean 
+flag that determines whether the distributions of interest are supported 
+on the full surface of the n-sphere (if False) or on the hemisphere with 
+reflecting boundary conditions for the diffusion kernel.
 
 Example output from `score_spherical_kernel` is:
 
 ```
 >>> import numpy as np
 >>> from spherediff.sample import sample_spherical_kernel
 >>> from spherediff.score import score_spherical_kernel
@@ -121,13 +124,26 @@
 >>> x
 array([[ 0.30027556, -0.53104481,  0.79235472],
        [ 0.91657116, -0.39288942,  0.07439905],
        [ 0.81325411,  0.41495422, -0.40795926],
        [ 0.39907791, -0.44171124, -0.80350981],
        [ 0.16422958, -0.76019121, -0.62860001]])
 >>> score_spherical_kernel(3, x, means, vars)
-array([[ 0.45383257, -1.4484151 , -0.34370955],
-       [ 2.57268711,  3.50638512, -2.19627206],
-       [ 0.33420178,  5.16225326, -0.64669865],
-       [ 2.62797084,  2.20685896, -1.97070763],
-       [-3.68698876, -0.78777185, -3.71349795]])
+array([[ 3.40175815,  3.11417869,  0.79800571],
+       [ 1.12626049,  2.20918798, -2.20878198],
+       [ 0.65201631,  0.12437106,  1.42627781],
+       [ 2.65653386, -1.32241858,  2.04638588],
+       [-0.69053884,  0.17827374, -0.39600546]])
+>>> x = sample_spherical_kernel(3, means, vars, hemisphere=True)
+>>> x
+array([[ 0.92723597,  0.02336567,  0.37374791],
+       [ 0.99421791, -0.03878944, -0.10013055],
+       [ 0.15771025,  0.6492883 , -0.74401087],
+       [ 0.2418101 , -0.41127436, -0.87885225],
+       [-0.11192408, -0.71437847, -0.69075061]])
+>>> score_spherical_kernel(3, x, means, vars, hemisphere=True)
+array([[-1.74036155, -1.77246139,  4.42849462],
+       [-0.0852985 , -1.00528069, -0.45751298],
+       [ 2.51709283,  0.09916178,  0.62009298],
+       [ 4.08775888, -1.8186883 ,  1.97580568],
+       [ 1.8912707 , -0.37819329,  0.08468239]])
 ```
```

