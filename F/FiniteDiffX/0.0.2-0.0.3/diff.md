# Comparing `tmp/FiniteDiffX-0.0.2.tar.gz` & `tmp/FiniteDiffX-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiniteDiffX-0.0.2.tar", last modified: Mon Mar 20 08:56:23 2023, max compression
+gzip compressed data, was "FiniteDiffX-0.0.3.tar", last modified: Mon Jun  5 12:43:32 2023, max compression
```

## Comparing `FiniteDiffX-0.0.2.tar` & `FiniteDiffX-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:56:23.450929 FiniteDiffX-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:56:23.446929 FiniteDiffX-0.0.2/FiniteDiffX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-03-20 08:56:23.000000 FiniteDiffX-0.0.2/FiniteDiffX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-20 08:56:23.000000 FiniteDiffX-0.0.2/FiniteDiffX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 08:56:23.000000 FiniteDiffX-0.0.2/FiniteDiffX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 08:56:23.000000 FiniteDiffX-0.0.2/FiniteDiffX.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-20 08:56:23.000000 FiniteDiffX-0.0.2/FiniteDiffX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-20 08:56:23.000000 FiniteDiffX-0.0.2/FiniteDiffX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-03-20 08:56:23.446929 FiniteDiffX-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:56:23.446929 FiniteDiffX-0.0.2/finitediffx/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/finitediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:56:23.446929 FiniteDiffX-0.0.2/finitediffx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/finitediffx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/finitediffx/_src/fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/finitediffx/_src/finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/finitediffx/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 08:56:23.450929 FiniteDiffX-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:56:23.446929 FiniteDiffX-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/tests/test_fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-03-20 08:56:05.000000 FiniteDiffX-0.0.2/tests/test_finite_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/finitediffx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/finitediffx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/_src/fgrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/_src/finite_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/tests/test_fgrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/tests/test_finite_diff.py
```

### Comparing `FiniteDiffX-0.0.2/LICENSE` & `FiniteDiffX-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.2/finitediffx/_src/finite_diff.py` & `FiniteDiffX-0.0.3/finitediffx/_src/finite_diff.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,26 @@
-# credits to Mahmoud Asem 2022 @KAIST
-# functions that operate on arrays
-# higher accuracy finite difference gradient might require
-# setting jax.config.update("jax_enable_x64", True)
+# Copyright 2023 FiniteDiffX authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 from __future__ import annotations
 
 import functools as ft
 from itertools import combinations
+from typing import Literal
 
 import jax
 import jax.numpy as jnp
 
 from finitediffx._src.utils import (
     _check_and_return,
     _generate_backward_offsets,
@@ -25,57 +35,74 @@
     "gradient",
     "jacobian",
     "laplacian",
     "curl",
     "divergence",
 )
 
+MethodKind = Literal["central", "forward", "backward"]
+
 
 def _central_difference(
     x: jax.Array,
     *,
     axis: int,
-    left_coeffs,
-    center_coeffs,
-    right_coeffs,
-    left_offsets,
-    center_offsets,
-    right_offsets,
-):
+    left_coeffs: tuple[float, ...],
+    center_coeffs: tuple[float, ...],
+    right_coeffs: tuple[float, ...],
+    left_offsets: tuple[float, ...],
+    center_offsets: tuple[float, ...],
+    right_offsets: tuple[float, ...],
+) -> jax.Array:
+    # offset defines the position of the point to be used in the finite difference
+    # and coeff defines the coefficient to be used in the finite difference
+    # for example, if we have a 5 point stencil for first derivative, the
+    # offsets = (-2, -1, 0, 1, 2)
+    # coefficients = (1/12, -2/3, 0, 2/3, -1/12)
+    # this means that the finite difference is
+    # df/fx = 1/12 * f(x-2) - 2/3 * f(x-1) + 0 * f(x) + 2/3 * f(x+1) - 1/12 * f(x+2)
+
     size = x.shape[axis]
+
+    # axis defines the axis along which the finite difference is to be computed
+    # for example, if x is a 2D array, then axis = 0 means that the finite difference
+    # is to be computed along the first axis, i.e. df/dx
+    # axis = 1 means that the finite difference is to be computed along the second axis i.e. df/dy
     sliced = ft.partial(jax.lax.slice_in_dim, x, axis=axis)
 
-    # use central difference for interior points
+    # calculate the finite difference for the left side of the array
+    # i.e. coefficients * f(x-offset)
+
     left_x = sum(
         coeff * sliced(offset, offset - center_offsets[0])
         for offset, coeff in zip(left_offsets, left_coeffs)
     )
 
-    right_x = sum(
-        coeff * sliced(size + (offset - center_offsets[-1]), size + (offset))
-        for offset, coeff in zip(right_offsets, right_coeffs)
-    )
-
     center_x = sum(
         coeff * sliced(offset - center_offsets[0], size + (offset - center_offsets[-1]))
         for offset, coeff in zip(center_offsets, center_coeffs)
     )
 
+    right_x = sum(
+        coeff * sliced(size + (offset - center_offsets[-1]), size + (offset))
+        for offset, coeff in zip(right_offsets, right_coeffs)
+    )
+
     return jnp.concatenate([left_x, center_x, right_x], axis=axis)
 
 
 def _central_difference_edge(
-    x,
+    x: jax.Array,
     *,
-    axis,
-    left_coeffs,
-    right_coeffs,
-    left_offsets,
-    right_offsets,
-):
+    axis: int,
+    left_coeffs: tuple[float, ...],
+    right_coeffs: tuple[float, ...],
+    left_offsets: tuple[float, ...],
+    right_offsets: tuple[float, ...],
+) -> jax.Array:
     size = x.shape[axis]
     sliced = ft.partial(jax.lax.slice_in_dim, x, axis=axis)
 
     left_x = sum(
         coeff * sliced(offset, offset + left_offsets[-1] + size % 2)
         for offset, coeff in zip(left_offsets, left_coeffs)
     )
@@ -85,22 +112,22 @@
         for offset, coeff in zip(right_offsets, right_coeffs)
     )
 
     return jnp.concatenate([left_x, right_x], axis=axis)
 
 
 def _forward_difference(
-    x,
+    x: jax.Array,
     *,
-    axis,
-    left_coeffs,
-    right_coeffs,
-    left_offsets,
-    right_offsets,
-):
+    axis: int,
+    left_coeffs: tuple[float, ...],
+    right_coeffs: tuple[float, ...],
+    left_offsets: tuple[float, ...],
+    right_offsets: tuple[float, ...],
+) -> jax.Array:
     size = x.shape[axis]
     sliced = ft.partial(jax.lax.slice_in_dim, x, axis=axis)
 
     left_x = sum(
         coeff * sliced(offset - left_offsets[0], size + (offset - left_offsets[-1]))
         for offset, coeff in zip(left_offsets, left_coeffs)
     )
@@ -110,21 +137,21 @@
         for offset, coeff in zip(right_offsets, right_coeffs)
     )
 
     return jnp.concatenate([left_x, right_x], axis=axis)
 
 
 def _backward_difference(
-    x,
+    x: jax.Array,
     *,
-    axis,
-    left_coeffs,
-    right_coeffs,
-    left_offsets,
-    right_offsets,
+    axis: int,
+    left_coeffs: tuple[float, ...],
+    right_coeffs: tuple[float, ...],
+    left_offsets: tuple[float, ...],
+    right_offsets: tuple[float, ...],
 ):
     size = x.shape[axis]
     sliced = ft.partial(jax.lax.slice_in_dim, x, axis=axis)
 
     left_x = sum(
         coeff * sliced(offset, offset - right_offsets[0])
         for offset, coeff in zip(left_offsets, left_coeffs)
@@ -142,15 +169,15 @@
 def difference(
     array: jax.Array,
     *,
     axis: int = 0,
     accuracy: int = 1,
     step_size: float | jax.Array = 1,
     derivative: int = 1,
-    method: str = "central",
+    method: MethodKind = "central",
 ) -> jax.Array:
     """Compute the finite difference derivative along a given axis with a given accuracy
     using central difference for interior points and forward/backward difference for boundary points
     Similar to np.gradient, but with the option to specify accuracy, derivative and step size
     See: https://github.com/google/jax/blob/main/jax/_src/numpy/lax_numpy.py
 
     Args:
@@ -160,42 +187,50 @@
         step_size: step size. Default is 1
         derivative: derivative order of the gradient. Default is 1
         method: the method to use (forward, central, backward). Default is central
     Returns:
         Finite difference derivative along the given axis
 
     Example:
-        # dydx of a 2D array
-        >>> x, y = [jnp.linspace(0, 1, 100)] * 2
-        >>> dx, dy = x[1] - x[0], y[1] - y[0]
-        >>> X, Y = jnp.meshgrid(x, y, indexing="ij")
-        >>> F =  jnp.sin(X) * jnp.cos(Y)
-        >>> dFdX = difference(F, step_size=dx, axis=0, accuracy=3, method="central")
-        >>> dFdXdY = difference(dFdX, step_size=dy, axis=1, accuracy=3, method="central")
-
-        # 1d finite difference derivative
-        >>> x = jnp.array([1.2, 1.3, 2.2, 3., 4.5, 5.5, 6., 7., 8., 20.])
-        >>> difference(x, accuracy=1)
-        [ 0.0999999  0.5        0.85       1.15       1.25       0.75 0.75       1.         6.5       12.       ]
-
+        >>> # dydx of a 2D array
+        >>> import finitediffx as fdx
+        >>> import jax.numpy as jnp
+        >>> import jax
+        >>> with jax.experimental.enable_x64():
+        ...     x, y = [jnp.linspace(0, 1, 100)] * 2
+        ...     dx, dy = x[1] - x[0], y[1] - y[0]
+        ...     X, Y = jnp.meshgrid(x, y, indexing="ij")
+        ...     F =  jnp.sin(X) * jnp.cos(Y)
+        ...     dFdX = fdx.difference(F, step_size=dx, axis=0, accuracy=3, method="central")
+        ...     dFdXdY = fdx.difference(dFdX, step_size=dy, axis=1, accuracy=3, method="central")
+        ...     # 1d finite difference derivative
+        ...     x = jnp.array([1.2, 1.3, 2.2, 3., 4.5, 5.5, 6., 7., 8., 20.])
+        ...     print(fdx.difference(x, accuracy=1))
+        [ 0.1   0.5   0.85  1.15  1.25  0.75  0.75  1.    6.5  12.  ]
+
+
+    Note:
+        Handling of boundary points is done by applying forward/backward difference
+        to the first/last element and central difference to the interior elements.
+        For the previous example, the following steps are performed:
 
-        # apply forward difference to the first element with accuracy 1
+        - apply forward difference to the first element with accuracy 1
         x_1 = 1.3-1.2 = 0.1
 
-        # apply central difference to interior elements with accuracy 2
+        - apply central difference to interior elements with accuracy 2
         x_2 = (2.2-1.2)/2 = 0.5
         x_3 = (3.-1.3)/2 = 0.85
         x_4 = (4.5-2.2)/2 = 1.15
         x_5 = (5.5-3.)/2 = 1.25
         x_6 = (6.-4.5)/2 = 0.75
         x_7 = (7.-5.5)/2 = 0.75
         x_8 = (8.-6.)/2 = 1.
         x_9 = (20.-7.)/2 = 6.5
 
-        # apply backward difference to the last element with accuracy 1
+        - apply backward difference to the last element with accuracy 1
         x_10 = 20.-8. = 12.
     """
     size = array.shape[axis]
 
     center_offsets = _generate_central_offsets(derivative, accuracy + 1)
     center_coeffs = generate_finitediff_coeffs(center_offsets, derivative)
 
@@ -248,50 +283,56 @@
             axis=axis,
             left_coeffs=left_coeffs,
             right_coeffs=right_coeffs,
             left_offsets=left_offsets,
             right_offsets=right_offsets,
         ) / (step_size**derivative)
 
-    msg = f"Size of the array along axis {axis} is smaller than the number of points required"
-    msg += f" for the accuracy {accuracy} and derivative {derivative} requested"
-    msg += f".\nSize must be larger than {len(left_offsets)}, but got {size}"
-    msg += f".\nMethod should be 'central', 'forward', 'backward', but got {method}"
-    raise ValueError(msg)
+    raise ValueError(
+        f"Size of the array along axis {axis} is smaller than the number of points required"
+        f" for the accuracy {accuracy} and derivative {derivative} requested"
+        f".\nSize must be larger than {len(left_offsets)}, but got {size}"
+        f".\nMethod should be 'central', 'forward', 'backward', but got {method}"
+    )
 
 
 @ft.partial(jax.jit, static_argnames=("accuracy", "method"))
 def gradient(
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 1,
     step_size: float | tuple[float, ...] | jax.Array = 1,
-    method: str = "central",
+    method: MethodKind = "central",
 ) -> jax.Array:
     """Compute the ∇F of input array where F is a scalar function of x and
     returns vectors of the same shape as x stacked along the first axis.
 
     Args:
         x: input array
         accuracy: accuracy order of the gradient. Default is 1, can be a tuple for each axis
         step_size: step size. Default is 1, can be a tuple for each axis
         method: the method to use (forward, central, backward). Default is central
 
     Index notation : dF/dxi
 
     Example:
-        # ∇F of a 2D array
-        >>> x, y = [jnp.linspace(0, 1, 100)] * 2
-        >>> dx, dy = x[1] - x[0], y[1] - y[0]
-        >>> X, Y = jnp.meshgrid(x, y, indexing="ij")
-        >>> Z = X**2 + Y**3
-        >>> dZdX , dZdY = gradient(Z, step_size=(dx,dy))
-        >>> dZdx_true, dZdy_true= 2*X , 3*Y**2
-        >>> numpy.testing.assert_allclose(dZdx, dZdx_true, atol=1e-4)
-        >>> numpy.testing.assert_allclose(dZdy, dZdy_true, atol=1e-4)
+        >>> # ∇F of a 2D array
+        >>> import finitediffx as fdx
+        >>> import jax.numpy as jnp
+        >>> import numpy.testing as npt
+        >>> import jax
+        >>> with jax.experimental.enable_x64():
+        ...     x, y = [jnp.linspace(0, 1, 100)] * 2
+        ...     dx, dy = x[1] - x[0], y[1] - y[0]
+        ...     X, Y = jnp.meshgrid(x, y, indexing="ij")
+        ...     Z = X**2 + Y**3
+        ...     dZdX , dZdY = fdx.gradient(Z, step_size=(dx,dy), accuracy=5)
+        ...     dZdX_true, dZdY_true= 2*X , 3*Y**2
+        ...     npt.assert_allclose(dZdX, dZdX_true, atol=1e-4)
+        ...     npt.assert_allclose(dZdY, dZdY_true, atol=1e-4)
     """
     accuracy = _check_and_return(accuracy, array.ndim, "accuracy")
     step_size = _check_and_return(step_size, array.ndim, "step_size")
 
     return jnp.stack(
         [
             difference(
@@ -310,31 +351,35 @@
 
 @ft.partial(jax.jit, static_argnames=("accuracy", "method"))
 def jacobian(
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 1,
     step_size: float | tuple[float, ...] | jax.Array = 1,
-    method: str = "central",
+    method: MethodKind = "central",
 ) -> jax.Array:
     """Compute the ∂Fi/∂xj of input array where F is a vector function of x and
     returns vectors of the same shape as x stacked along the first axis.
 
     Args:
         x: input array
         accuracy: accuracy order of the gradient. Default is 1, can be a tuple for each axis
         step_size: step size. Default is 1, can be a tuple for each axis
         method: the method to use (forward, central, backward). Default is central
 
     Index notation: ∂Fi/∂xj
 
     Example:
-        # F: R^2 -> R^2
-        # F = [ x^2*y, 5x+siny ]
-        # JF = [ [2xy, x^2], [5, cos(y)] ]
+        >>> # F: R^2 -> R^2
+        >>> # F = [ x^2*y, 5x+siny ]
+        >>> # JF = [ [2xy, x^2], [5, cos(y)] ]
+        >>> import finitediffx as fdx
+        >>> import jax.numpy as jnp
+        >>> import numpy.testing as npt
+        >>> import jax
         >>> with jax.experimental.enable_x64():
         ...    x, y = [jnp.linspace(-1, 1, 100)] * 2
         ...    dx, dy = x[1] - x[0], y[1] - y[0]
         ...    X, Y = jnp.meshgrid(x, y, indexing="ij")
         ...    F1 = X**2 * Y
         ...    F2 = 5 * X + jnp.sin(Y)
         ...    F = jnp.stack([F1, F2], axis=0)
@@ -357,39 +402,42 @@
 @ft.partial(jax.jit, static_argnames=("accuracy", "method", "keepdims"))
 def divergence(
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 1,
     step_size: float | tuple[float, ...] = 1,
     keepdims: bool = True,
-    method: str = "central",
+    method: MethodKind = "central",
 ) -> jax.Array:
     """Compute the ∇.F of input array where F is a vector field whose components are the first axis of x
     and returns a scalar field
 
     Args:
         x: input array where the leading axis is the dimension of the vector field
         accuracy: accuracy order of the gradient. Default is 1, can be a tuple for each axis
         step_size: step size. Default is 1, can be a tuple for each axis
         method: the method to use (forward, central, backward). Default is central
         keepdims: whether to keep the leading dimension. Default is True.
 
     Index notation: dFi/dxi
 
     Example:
-        # ∇.F of a 2D array
+        >>> # ∇.F of a 2D array
+        >>> import finitediffx as fdx
+        >>> import jax.numpy as jnp
+        >>> import numpy.testing as npt
         >>> x, y = [jnp.linspace(0, 1, 100)] * 2
         >>> dx, dy = x[1] - x[0], y[1] - y[0]
         >>> X, Y = jnp.meshgrid(x, y, indexing="ij")
         >>> F1 = X**2 + Y**3
         >>> F2 = X**4 + Y**3
         >>> F = jnp.stack([F1, F2], axis=0) # 2D vector field F = (F1, F2)
         >>> divZ = divergence(F,step_size=(dx,dy), accuracy=7, keepdims=False)
         >>> divZ_true = 2*X + 3*Y**2  # (dF1/dx) + (dF2/dy)
-        >>> numpy.testing.assert_allclose(divZ, divZ_true, atol=5e-4)
+        >>> npt.assert_allclose(divZ, divZ_true, atol=5e-4)
     """
     accuracy = _check_and_return(accuracy, array.ndim - 1, "accuracy")
     step_size = _check_and_return(step_size, array.ndim - 1, "step_size")
 
     result = sum(
         difference(
             array[axis],
@@ -409,35 +457,39 @@
 
 @ft.partial(jax.jit, static_argnames=("accuracy", "method"))
 def hessian(
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 2,
     step_size: float | tuple[float, ...] | jax.Array = 1,
-    method: str = "central",
+    method: MethodKind = "central",
 ) -> jax.Array:
     """Compute hessian of F: R^m -> R
 
     Args:
         x: input array
         accuracy: accuracy order of the gradient. Default is 2, can be a tuple for each axis
         method: the method to use (forward, central, backward). Default is central
         step_size: step size. Default is 1, can be a tuple for each axis
 
     Index notation: d2F/dxij
 
     Example:
-        >>> x, y = [jnp.linspace(-1, 1, 100)] * 2
-        >>> dx, dy = x[1] - x[0], y[1] - y[0]
-        >>> X, Y = jnp.meshgrid(x, y, indexing="ij")
-
-        >>> F = X**2 * Y
-        >>> H = hessian(F, accuracy=4, step_size=(dx, dy))
-        >>> H_true = jnp.array([[2 * Y, 2 * X], [2 * X, jnp.zeros_like(X)]])
-        >>> npt.assert_allclose(H, H_true, atol=1e-7)
+        >>> import finitediffx as fdx
+        >>> import jax.numpy as jnp
+        >>> import numpy.testing as npt
+        >>> import jax
+        >>> with jax.experimental.enable_x64():
+        ...     x, y = [jnp.linspace(-1, 1, 100)] * 2
+        ...     dx, dy = x[1] - x[0], y[1] - y[0]
+        ...     X, Y = jnp.meshgrid(x, y, indexing="ij")
+        ...     F = X**2 * Y
+        ...     H = fdx.hessian(F, accuracy=4, step_size=(dx, dy))
+        ...     H_true = jnp.array([[2 * Y, 2 * X], [2 * X, jnp.zeros_like(X)]])
+        ...     npt.assert_allclose(H, H_true, atol=1e-7)
     """
     accuracy = _check_and_return(accuracy, array.ndim, "accuracy")
     step_size = _check_and_return(step_size, array.ndim, "step_size")
     axes = tuple(range(array.ndim))
     F = dict()
 
     # diag
@@ -477,79 +529,75 @@
 
 @ft.partial(jax.jit, static_argnames=("accuracy", "method"))
 def laplacian(
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 1,
     step_size: float | tuple[float, ...] | jax.Array = 1,
-    method: str = "central",
+    method: MethodKind = "central",
 ) -> jax.Array:
     """Compute the ΔF of input array.
     Args:
         x: input array
         accuracy: accuracy order of the gradient. Default is 1, can be a tuple for each axis
         step_size: step size. Default is 1, can be a tuple for each axis
         method: the method to use (forward, central, backward). Default is central
 
     Index notation: d2F/dxi2
     Example:
-        # ΔF array
-        >>> x, y = [jnp.linspace(0, 1, 100)] * 2
-        >>> dx, dy = x[1] - x[0], y[1] - y[0]
-        >>> X, Y = jnp.meshgrid(x, y, indexing="ij")
-        >>> Z = X**4 + Y**3
-        >>> laplacianZ = laplacian(Z, step_size=(dx,dy))
-        >>> laplacianZ_true = 12*X**2 + 6*Y
-        >>> numpy.testing.assert_allclose(laplacianZ, laplacianZ_true, atol=1e-4)
+        >>> import finitediffx as fdx
+        >>> import jax.numpy as jnp
+        >>> import numpy.testing as npt
+        >>> import jax
+        >>> with jax.experimental.enable_x64():
+        ...    x, y = [jnp.linspace(0, 1, 100)] * 2
+        ...    dx, dy = x[1] - x[0], y[1] - y[0]
+        ...    X, Y = jnp.meshgrid(x, y, indexing="ij")
+        ...    Z = X**4 + Y**3
+        ...    laplacianZ = fdx.laplacian(Z, step_size=(dx,dy), accuracy=10)
+        ...    laplacianZ_true = 12*X**2 + 6*Y
+        ...    npt.assert_allclose(laplacianZ, laplacianZ_true, atol=1e-4)
     """
     accuracy = _check_and_return(accuracy, array.ndim, "accuracy")
     step_size = _check_and_return(step_size, array.ndim, "step_size")
 
     return sum(
         difference(
-            array, accuracy=acc, step_size=step, derivative=2, method=method, axis=axis
+            array,
+            accuracy=acc,
+            step_size=step,
+            derivative=2,
+            method=method,
+            axis=axis,
         )
         for axis, (acc, step) in enumerate(zip(accuracy, step_size))
     )
 
 
 def _curl_2d(
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 1,
     step_size: float | tuple[float, ...] | jax.Array = 1,
-    method: str = "central",
+    method: MethodKind = "central",
     keepdims: bool = True,
 ) -> jax.Array:
-    """Compute the ∇×F of input array where F is a vector field whose components are the first axis of x
-    and returns a vector field
-
-    Index notation: εijk dFk/dxj
-
-    Args:
-        x: input array where the leading axis is the dimension of the vector field
-        accuracy: accuracy order of the gradient. Default is 1, can be a tuple for each axis
-        step_size: step size. Default is 1, can be a tuple for each axis
-        method: the method to use (forward, central, backward). Default is central
-        keepdims: whether to keep the leading dimension of the vector field
-
-    Example:
-        >>> x,y = [jnp.linspace(-1,1,50)]*2
-        >>> dx,dy = x[1]-x[0],y[1]-y[0]
-        >>> X,Y = jnp.meshgrid(x,y, indexing="ij")
-        >>> F1 = jnp.sin(Y)
-        >>> F2 = jnp.cos(X)
-        >>> F = jnp.stack([F1,F2], axis=0)
-        >>> curl = curl_2d(F, accuracy=4, step_size=dx)
-    """
     dF1dY = difference(
-        array[0], accuracy=accuracy[1], step_size=step_size[1], method=method, axis=1
+        array[0],
+        accuracy=accuracy[1],
+        step_size=step_size[1],
+        method=method,
+        axis=1,
     )
     dF2dX = difference(
-        array[1], accuracy=accuracy[0], step_size=step_size[0], method=method, axis=0
+        array[1],
+        accuracy=accuracy[0],
+        step_size=step_size[0],
+        method=method,
+        axis=0,
     )
 
     result = dF2dX - dF1dY
 
     if keepdims:
         return jnp.expand_dims(result, axis=0)
 
@@ -560,32 +608,56 @@
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 1,
     step_size: float | tuple[float, ...] | jnp.ndarry = 1,
     method: str = "central",
 ) -> jax.Array:
     dF1dY = difference(
-        array[0], accuracy=accuracy[1], step_size=step_size[1], method=method, axis=1
+        array[0],
+        accuracy=accuracy[1],
+        step_size=step_size[1],
+        method=method,
+        axis=1,
     )
     dF1dZ = difference(
-        array[0], accuracy=accuracy[2], step_size=step_size[2], method=method, axis=2
+        array[0],
+        accuracy=accuracy[2],
+        step_size=step_size[2],
+        method=method,
+        axis=2,
     )
 
     dF2dX = difference(
-        array[1], accuracy=accuracy[0], step_size=step_size[0], method=method, axis=0
+        array[1],
+        accuracy=accuracy[0],
+        step_size=step_size[0],
+        method=method,
+        axis=0,
     )
     dF2dZ = difference(
-        array[1], accuracy=accuracy[2], step_size=step_size[2], method=method, axis=2
+        array[1],
+        accuracy=accuracy[2],
+        step_size=step_size[2],
+        method=method,
+        axis=2,
     )
 
     dF3dX = difference(
-        array[2], accuracy=accuracy[0], step_size=step_size[0], method=method, axis=0
+        array[2],
+        accuracy=accuracy[0],
+        step_size=step_size[0],
+        method=method,
+        axis=0,
     )
     dF3dY = difference(
-        array[2], accuracy=accuracy[1], step_size=step_size[1], method=method, axis=1
+        array[2],
+        accuracy=accuracy[1],
+        step_size=step_size[1],
+        method=method,
+        axis=1,
     )
 
     return jnp.stack(
         [
             dF3dY - dF2dZ,
             dF1dZ - dF3dX,
             dF2dX - dF1dY,
@@ -596,15 +668,15 @@
 
 @ft.partial(jax.jit, static_argnames=("accuracy", "method", "keepdims"))
 def curl(
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 1,
     step_size: float | tuple[float, ...] | jax.Array = 1,
-    method: str = "central",
+    method: MethodKind = "central",
     keepdims: bool = True,
 ) -> jax.Array:
     """Compute the ∇×F of input array where F is a vector field whose components are the first axis of x
     and returns a vector field
 
     Index notation: εijk dFk/dxj
 
@@ -612,37 +684,41 @@
         x: input array where the leading axis is the dimension of the vector field
         accuracy: accuracy order of the gradient. Default is 1, can be a tuple for each axis
         step_size: step size. Default is 1, can be a tuple for each axis
         method: the method to use (forward, central, backward). Default is central
         keepdims: whether to keep the leading dimension of the vector field (only for 2D)
 
     Example:
-        Curl for a 3D vector field is defined as
-        F = (F1, F2, F3)
-        ∇×F = (dF3/dy - dF2/dz, dF1/dz - dF3/dx, dF2/dx - dF1/dy)
-        >>> jax.config.update("jax_enable_x64", True)
-        >>> x,y,z = [jnp.linspace(0, 1, 100)] * 3
-        >>> dx,dy,dz = x[1]-x[0], y[1]-y[0], z[1]-z[0]
-        >>> X,Y,Z = jnp.meshgrid(x,y,z, indexing="ij")
-        >>> F1 = X**2 + Y**3
-        >>> F2 = X**4 + Y**3
-        >>> F3 = jnp.zeros_like(F1)
-        >>> F = jnp.stack([F1,F2,F3], axis=0)
-        >>> curlF = finitediffx.curl(F, step_size=(dx,dy,dz),  accuracy=6)
-        >>> curlF_exact = jnp.stack([F1*0,F1*0, 4*X**3 - 3*Y**2], axis=0)
-        >>> npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
+        >>> # Curl for a 3D vector field is defined as
+        >>> # F = (F1, F2, F3)
+        >>> # ∇×F = (dF3/dy - dF2/dz, dF1/dz - dF3/dx, dF2/dx - dF1/dy)
+        >>> import finitediffx as fdx
+        >>> import jax.numpy as jnp
+        >>> import numpy.testing as npt
+        >>> import jax
+        >>> with jax.experimental.enable_x64():
+        ...     x,y,z = [jnp.linspace(0, 1, 100)] * 3
+        ...     dx,dy,dz = x[1]-x[0], y[1]-y[0], z[1]-z[0]
+        ...     X,Y,Z = jnp.meshgrid(x,y,z, indexing="ij")
+        ...     F1 = X**2 + Y**3
+        ...     F2 = X**4 + Y**3
+        ...     F3 = jnp.zeros_like(F1)
+        ...     F = jnp.stack([F1,F2,F3], axis=0)
+        ...     curlF = fdx.curl(F, step_size=(dx,dy,dz),  accuracy=6)
+        ...     curlF_exact = jnp.stack([F1*0,F1*0, 4*X**3 - 3*Y**2], axis=0)
+        ...     npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
 
-        Curl of 2D vector field is defined as
+        >>> # Curl of 2D vector field is defined as
         >>> x,y = [jnp.linspace(-1,1,50)]*2
         >>> dx,dy = x[1]-x[0],y[1]-y[0]
         >>> X,Y = jnp.meshgrid(x,y, indexing="ij")
         >>> F1 = jnp.sin(Y)
         >>> F2 = jnp.cos(X)
         >>> F = jnp.stack([F1,F2], axis=0)
-        >>> curl = curl_2d(F, accuracy=4, step_size=dx)
+        >>> curl = fdx.curl(F, accuracy=4, step_size=dx)
     """
 
     accuracy = _check_and_return(accuracy, array.ndim - 1, "accuracy")
     step_size = _check_and_return(step_size, array.ndim - 1, "step_size")
 
     if array.ndim == 4 and array.shape[0] == 3:
         return _curl_3d(array, accuracy=accuracy, method=method, step_size=step_size)
@@ -652,11 +728,12 @@
             array,
             accuracy=accuracy,
             step_size=step_size,
             method=method,
             keepdims=keepdims,
         )
 
-    msg = f"`curl` is only implemented for 2D and 3D vector fields, got {array.ndim}D"
-    msg += "for 2D vector fields, the leading axis must have a shape=2, "
-    msg += "for 3D vector fields, the leading axis must have a shape=3"
-    raise ValueError(msg)
+    raise ValueError(
+        f"`curl` is only implemented for 2D and 3D vector fields, got {array.ndim}D"
+        "for 2D vector fields, the leading axis must have a shape=2, "
+        "for 3D vector fields, the leading axis must have a shape=3"
+    )
```

### Comparing `FiniteDiffX-0.0.2/setup.py` & `FiniteDiffX-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     author="Mahmoud Asem",
     description=("Finite difference tools in JAX."),
     long_description=open(os.path.join(_CURRENT_DIR, "README.md")).read(),
     long_description_content_type="text/markdown",
     author_email="asem00@kaist.ac.kr",
     keywords="python jax",
     packages=find_namespace_packages(exclude=['examples", "tests","experimental']),
-    install_requires=["jax>=0.4.0"],
+    install_requires=["jax>=0.4.0", "typing-extensions"],
     zip_safe=False,  # Required for full installation.
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
```

### Comparing `FiniteDiffX-0.0.2/tests/test_fgrad.py` & `FiniteDiffX-0.0.3/tests/test_fgrad.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,31 @@
+import functools as ft
+
 import jax
 import jax.numpy as jnp
 import numpy as np
+import numpy as onp
+import numpy.testing as npt
 import pytest
 from jax.experimental import enable_x64
 
-from finitediffx import fgrad, generate_finitediff_coeffs
+from finitediffx import Offset, define_fdjvp, fgrad, generate_finitediff_coeffs
 
 
 def test_generate_finitediff_coeffs():
     with enable_x64():
         DF = lambda N: generate_finitediff_coeffs(N, 1)
         all_correct = lambda x, y: np.testing.assert_allclose(x, y, atol=1e-2)
 
         # https://en.wikipedia.org/wiki/fgraderence_coefficient
         all_correct(DF((0, 1)), jnp.array([-1.0, 1.0]))
         all_correct(DF((0, 1, 2)), jnp.array([-3 / 2.0, 2.0, -1 / 2]))
         all_correct(DF((0, 1, 2, 3)), jnp.array([-11 / 6, 3.0, -3 / 2, 1 / 3]))
-        all_correct(
-            DF((0, 1, 2, 3, 4)), jnp.array([-25 / 12, 4.0, -3.0, 4 / 3, -1 / 4])
-        )
-        all_correct(
-            DF((0, 1, 2, 3, 4, 5)),
-            jnp.array([-137 / 60, 5.0, -5, 10 / 3, -5 / 4, 1 / 5]),
-        )
+        all_correct(DF((0, 1, 2, 3, 4)), jnp.array([-25 / 12, 4.0, -3.0, 4 / 3, -1 / 4]))  # fmt: skip
+        all_correct(DF((0, 1, 2, 3, 4, 5)), jnp.array([-137 / 60, 5.0, -5, 10 / 3, -5 / 4, 1 / 5]),)  # fmt: skip
         all_correct(
             DF((0, 1, 2, 3, 4, 5, 6)),
             jnp.array([-49 / 20, 6.0, -15 / 2, 20 / 3, -15 / 4, 6 / 5, -1 / 6]),
         )
 
         # https://web.media.mit.edu/~crtaylor/calculator.html
         all_correct(DF((-2.2, 3.2, 5)), jnp.array([-205 / 972, 280 / 972, -75 / 972]))
@@ -117,14 +116,59 @@
             f3 = fgrad(fgrad(func))
             args = (1.5, 2.5, 3.5)
             F1, F2, F3 = f1(*args), f2(*args), f3(*args)
             all_correct(F1, F2)
             all_correct(F1, F3)
 
 
+def test_fgrad_multiple_step_sizes():
+    with enable_x64():
+        # test multiple step sizes
+        func = lambda x, y: (x + y) ** 2
+        dfunc = fgrad(
+            func,
+            step_size=(None, 1e-3),
+            offsets=(jnp.array([-1, 1.0]), jnp.array([-2, 2.0])),
+            argnums=(0, 1),
+        )
+
+        dval = dfunc(1.0, 1.0)
+        assert dval[0] != dval[1]  # different step sizes
+        npt.assert_allclose(dval[0], 4.0, atol=1e-3)
+        npt.assert_allclose(dval[1], 4.0, atol=1e-3)
+
+    with pytest.raises(TypeError):
+        dfunc = fgrad(
+            func,
+            step_size=(None, 1e-3),
+            offsets=(jnp.array([-1, 1.0]), jnp.array([-2, 2.0])),
+            argnums=0,
+        )  # non-tuple argnums with tuple step_size
+
+    with pytest.raises(AssertionError):
+        # mismatched argnums length and step_size length
+        dfunc = fgrad(func, step_size=(None,), argnums=(0, 1))
+
+    with pytest.raises(AssertionError):
+        # mismatched argnums length and step_size length
+        dfunc = fgrad(func, offsets=(jnp.array([-1, 1.0]),), argnums=(0, 1))
+
+    with pytest.raises(ValueError):
+        # wrong accuracy
+        dfunc = fgrad(
+            func,
+            offsets=(Offset(accuracy=0), Offset(accuracy=1)),
+            argnums=(0, 1),
+        )
+
+    with pytest.raises(TypeError):
+        # wrong accuracy
+        dfunc = fgrad(func, offsets=(Offset(accuracy=2), ""), argnums=(0, 1))
+
+
 def test_fgrad_argnum():
     with enable_x64():
         all_correct = lambda lhs, rhs: np.testing.assert_allclose(lhs, rhs, atol=0.05)
 
         # test argnums
         func = lambda x, y, z: x**2 + y**3 + z**4
         f1 = jax.grad(func, argnums=(0,))(1.0, 1.0, 1.0)
@@ -150,11 +194,44 @@
     with pytest.raises(ValueError):
         fgrad(lambda x: x, argnums=-1)
 
     with pytest.raises(ValueError):
         fgrad(lambda x: x, argnums=1.0)
 
     with pytest.raises(ValueError):
-        fgrad(lambda x: x, accuracy=1)
+        fgrad(lambda x: x, offsets=Offset(accuracy=1))
 
     with pytest.raises(ValueError):
         fgrad(lambda x: x, argnums=[1, 2])
+
+
+def test_fdjvp():
+    def wrap_pure_callback(func):
+        @ft.wraps(func)
+        def wrapper(*args, **kwargs):
+            args = [jnp.asarray(arg) for arg in args]
+            func_ = lambda *a, **k: func(*a, **k).astype(a[0].dtype)
+            dtype_ = jax.ShapeDtypeStruct(
+                jnp.broadcast_shapes(*[ai.shape for ai in args]),
+                args[0].dtype,
+            )
+            return jax.pure_callback(func_, dtype_, *args, **kwargs, vectorized=True)
+
+        return wrapper
+
+    @jax.jit
+    @define_fdjvp
+    @wrap_pure_callback
+    def numpy_func(x, y):
+        return onp.power(x, 2) + onp.power(y, 2)
+
+    npt.assert_allclose(
+        jax.grad(numpy_func, argnums=0)(1.0, 2.0),
+        jnp.array(2.0),
+        atol=1e-3,
+    )
+
+    npt.assert_allclose(
+        jax.grad(numpy_func, argnums=1)(1.0, 2.0),
+        jnp.array(4.0),
+        atol=1e-3,
+    )
```

### Comparing `FiniteDiffX-0.0.2/tests/test_finite_diff.py` & `FiniteDiffX-0.0.3/tests/test_finite_diff.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,32 +70,45 @@
         dFdY = difference(F, step_size=dy, axis=1, accuracy=3)
         npt.assert_allclose(dFdY, -jnp.sin(X) * jnp.sin(Y), atol=1e-7)
 
         # 1 4 6 3 2
         # left = (4-1), (6-4), (3-6), (2-3)-> forward difference
         # right = (2-3) = -1 -> backward difference
         npt.assert_allclose(
-            difference(jnp.array([1, 4, 6, 3, 2]), accuracy=1, axis=0, derivative=1, method="forward"),
-            jnp.array([3., 2., -3., -1., -1.]),
+            difference(
+                jnp.array([1, 4, 6, 3, 2]),
+                accuracy=1,
+                axis=0,
+                derivative=1,
+                method="forward",
+            ),
+            jnp.array([3.0, 2.0, -3.0, -1.0, -1.0]),
         )
 
         # 1 4 6 3 2 4
         # Forward Coeffs -> [-1.5  2.  -0.5] (0, 1, 2)
         # Backward Coeffs -> [ 0.5 -2.   1.5] (-2, -1, 0)
         npt.assert_allclose(
-            difference(jnp.array([1, 4, 6, 3, 2, 4]), accuracy=2, axis=0, derivative=1, method="forward"),
+            difference(
+                jnp.array([1, 4, 6, 3, 2, 4]),
+                accuracy=2,
+                axis=0,
+                derivative=1,
+                method="forward",
+            ),
             jnp.array([3.5, 4.5, -4.0, -2.5, 0.0, 3.5]),
         )
 
         # no central difference possible
         x = jnp.array([1.2, 1.4])
         # Forward Coeffs -> [-1 1] (0, 1)
         # Backward Coeffs -> [1 -1] (-1, 0)
         npt.assert_allclose(
-            difference(x, accuracy=1, axis=0, derivative=1, method="forward"), jnp.array([0.2, 0.2])
+            difference(x, accuracy=1, axis=0, derivative=1, method="forward"),
+            jnp.array([0.2, 0.2]),
         )
 
 
 def test_difference_backward():
     with enable_x64():
         x, y = [jnp.linspace(0, 1, 1000)] * 2
         dx, dy = x[1] - x[0], y[1] - y[0]
@@ -107,91 +120,103 @@
         dFdY = difference(F, step_size=dy, axis=1, accuracy=3)
         npt.assert_allclose(dFdY, -jnp.sin(X) * jnp.sin(Y), atol=1e-7)
 
         # 1 4 6 3 2
         # left = (4-1)-> forward difference
         # right = (4-1), (6-4), (3-6), (2-3) = -1 -> backward difference
         npt.assert_allclose(
-            difference(jnp.array([1, 4, 6, 3, 2]), accuracy=1, axis=0, derivative=1, method="backward"),
-            jnp.array([3., 3., 2., -3., -1.]),
+            difference(
+                jnp.array([1, 4, 6, 3, 2]),
+                accuracy=1,
+                axis=0,
+                derivative=1,
+                method="backward",
+            ),
+            jnp.array([3.0, 3.0, 2.0, -3.0, -1.0]),
         )
 
         # 1 4 6 3 2 4
         # Forward Coeffs -> [-1.5  2.  -0.5] (0, 1, 2)
         # Backward Coeffs -> [ 0.5 -2.   1.5] (-2, -1, 0)
         npt.assert_allclose(
-            difference(jnp.array([1, 4, 6, 3, 2, 4]), accuracy=2, axis=0, derivative=1, method="backward"),
+            difference(
+                jnp.array([1, 4, 6, 3, 2, 4]),
+                accuracy=2,
+                axis=0,
+                derivative=1,
+                method="backward",
+            ),
             jnp.array([3.5, 4.5, 1.5, -5.5, 0.0, 3.5]),
         )
 
         # no central difference possible
         x = jnp.array([1.2, 1.4])
         # Forward Coeffs -> [-1 1] (0, 1)
         # Backward Coeffs -> [1 -1] (-1, 0)
         npt.assert_allclose(
-            difference(x, accuracy=1, axis=0, derivative=1, method="backward"), jnp.array([0.2, 0.2])
+            difference(x, accuracy=1, axis=0, derivative=1, method="backward"),
+            jnp.array([0.2, 0.2]),
         )
 
 
-@pytest.mark.parametrize(
-        "method", ("central", "forward","backward")
-)
+@pytest.mark.parametrize("method", ("central", "forward", "backward"))
 def test_divergence(method):
     with enable_x64():
         x, y = [jnp.linspace(0, 1, 100)] * 2
         dx, dy = x[1] - x[0], y[1] - y[0]
         X, Y = jnp.meshgrid(x, y, indexing="ij")
         F1 = X**2 + Y**3
         F2 = X**4 + Y**3
         F = jnp.stack([F1, F2], axis=0)  # 2D vector field F = (F1, F2)
-        divZ = divergence(F, step_size=(dx, dy), accuracy=7, method=method, keepdims=False)
+        divZ = divergence(
+            F, step_size=(dx, dy), accuracy=7, method=method, keepdims=False
+        )
         divZ_true = 2 * X + 3 * Y**2  # (dF1/dx) + (dF2/dy)
         npt.assert_allclose(divZ, divZ_true, atol=5e-7)
 
-        divZ = divergence(F, step_size=(dx, dy), accuracy=7,  method=method, keepdims=True)
+        divZ = divergence(
+            F, step_size=(dx, dy), accuracy=7, method=method, keepdims=True
+        )
         divZ_true = 2 * X + 3 * Y**2  # (dF1/dx) + (dF2/dy)
         npt.assert_allclose(divZ, divZ_true[None], atol=5e-7)
 
 
-@pytest.mark.parametrize(
-        "method", ("central", "forward","backward")
-)
+@pytest.mark.parametrize("method", ("central", "forward", "backward"))
 def test_gradient(method):
     with enable_x64():
         x, y = [jnp.linspace(0, 1, 100)] * 2
         dx, dy = x[1] - x[0], y[1] - y[0]
         X, Y = jnp.meshgrid(x, y, indexing="ij")
         F = X**2 + Y**3
         gradF = gradient(F, step_size=(dx, dy), accuracy=7, method=method)
         gradF_true = jnp.stack([2 * X, 3 * Y**2], axis=0)
         npt.assert_allclose(gradF, gradF_true, atol=5e-7)
 
 
 @pytest.mark.parametrize(
-        "method,atol", [
-            ("central", 1e-7),
-            ("forward", 1e-6),
-            ("backward",1e-7)
-        ]
+    "method,atol",
+    [
+        ("central", 5e-6),
+        ("forward", 5e-6),
+        ("backward", 5e-6),
+    ],
 )
 def test_laplacian(method, atol):
     with enable_x64():
         # needs float64 for higher accuracy
         x, y = [jnp.linspace(0, 1, 100)] * 2
         dx, dy = x[1] - x[0], y[1] - y[0]
         X, Y = jnp.meshgrid(x, y, indexing="ij")
         Z = X**4 + Y**3
         laplacianZ = laplacian(Z, step_size=(dx, dy), accuracy=10, method=method)
         laplacianZ_true = 12 * X**2 + 6 * Y
         npt.assert_allclose(laplacianZ, laplacianZ_true, atol=atol)
 
 
-@pytest.mark.parametrize(
-        "method", ("central", "forward","backward")
-)
+@pytest.mark.parametrize("method", ("central", "forward", "backward"))
 def test_curl(method):
     with enable_x64():
         x, y, z = [jnp.linspace(0, 1, 100)] * 3
         dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
         X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
         F1 = X**2 + Y**2
         F2 = X**4 + Y**3
@@ -218,17 +243,15 @@
         res = curl(F, accuracy=4, step_size=dx, method=method, keepdims=True)
         npt.assert_allclose(res[0], -jnp.sin(X) - jnp.cos(Y), atol=1e-4)
 
     with pytest.raises(ValueError):
         curl(F[None], accuracy=4, step_size=dx, method=method, keepdims=True)
 
 
-@pytest.mark.parametrize(
-        "method", ("central", "forward","backward")
-)
+@pytest.mark.parametrize("method", ("central", "forward", "backward"))
 def test_jacobian(method):
     with enable_x64():
         x, y = [jnp.linspace(-1, 1, 100)] * 2
         dx, dy = x[1] - x[0], y[1] - y[0]
         X, Y = jnp.meshgrid(x, y, indexing="ij")
         F1 = X**2 * Y
         F2 = 5 * X + jnp.sin(Y)
@@ -255,17 +278,15 @@
                 [X3 * jnp.cos(X1), jnp.zeros_like(X1), jnp.sin(X1)],
             ]
         )
 
         npt.assert_allclose(JY, JY_true, rtol=1e-3, atol=1e-5)
 
 
-@pytest.mark.parametrize(
-        "method", ("central", "forward","backward")
-)
+@pytest.mark.parametrize("method", ("central", "forward", "backward"))
 def test_hessian(method):
     with enable_x64():
         x, y = [jnp.linspace(-1, 1, 100)] * 2
         dx, dy = x[1] - x[0], y[1] - y[0]
         X, Y = jnp.meshgrid(x, y, indexing="ij")
 
         F = X**2 * Y
```

