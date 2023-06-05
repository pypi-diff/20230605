# Comparing `tmp/dm_pix-0.4.0.tar.gz` & `tmp/dm_pix-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm_pix-0.4.0.tar", last modified: Fri Feb 17 14:05:02 2023, max compression
+gzip compressed data, was "dm_pix-0.4.1.tar", last modified: Mon Jun  5 10:35:53 2023, max compression
```

## Comparing `dm_pix-0.4.0.tar` & `dm_pix-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:05:02.910309 dm_pix-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-17 14:04:53.000000 dm_pix-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-17 14:04:53.000000 dm_pix-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-02-17 14:05:02.910309 dm_pix-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-02-17 14:04:53.000000 dm_pix-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:05:02.906309 dm_pix-0.4.0/dm_pix/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:05:02.906309 dm_pix-0.4.0/dm_pix/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    26742 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/augment_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/color_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/color_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/depth_and_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/depth_and_space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/interpolation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/patch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/_src/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 14:04:53.000000 dm_pix-0.4.0/dm_pix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:05:02.906309 dm_pix-0.4.0/dm_pix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-02-17 14:05:02.000000 dm_pix-0.4.0/dm_pix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-17 14:05:02.000000 dm_pix-0.4.0/dm_pix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 14:05:02.000000 dm_pix-0.4.0/dm_pix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 14:05:02.000000 dm_pix-0.4.0/dm_pix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-17 14:05:02.000000 dm_pix-0.4.0/dm_pix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-17 14:05:02.000000 dm_pix-0.4.0/dm_pix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:05:02.906309 dm_pix-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-02-17 14:04:53.000000 dm_pix-0.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:05:02.910309 dm_pix-0.4.0/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-02-17 14:04:53.000000 dm_pix-0.4.0/docs/ext/coverage_check.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-17 14:04:53.000000 dm_pix-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-17 14:04:53.000000 dm_pix-0.4.0/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-17 14:04:53.000000 dm_pix-0.4.0/requirements_examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-17 14:04:53.000000 dm_pix-0.4.0/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 14:05:02.910309 dm_pix-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-02-17 14:04:53.000000 dm_pix-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:35:53.652793 dm_pix-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-05 10:35:42.000000 dm_pix-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 10:35:42.000000 dm_pix-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-06-05 10:35:53.652793 dm_pix-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-05 10:35:42.000000 dm_pix-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:35:53.648793 dm_pix-0.4.1/dm_pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:35:53.652793 dm_pix-0.4.1/dm_pix/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/augment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/color_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/color_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/depth_and_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/depth_and_space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/interpolation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/patch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/_src/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:35:42.000000 dm_pix-0.4.1/dm_pix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:35:53.648793 dm_pix-0.4.1/dm_pix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-06-05 10:35:53.000000 dm_pix-0.4.1/dm_pix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-05 10:35:53.000000 dm_pix-0.4.1/dm_pix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:35:53.000000 dm_pix-0.4.1/dm_pix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:35:53.000000 dm_pix-0.4.1/dm_pix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-05 10:35:53.000000 dm_pix-0.4.1/dm_pix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 10:35:53.000000 dm_pix-0.4.1/dm_pix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:35:53.652793 dm_pix-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-05 10:35:42.000000 dm_pix-0.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:35:53.652793 dm_pix-0.4.1/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-05 10:35:42.000000 dm_pix-0.4.1/docs/ext/coverage_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 10:35:42.000000 dm_pix-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-05 10:35:42.000000 dm_pix-0.4.1/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 10:35:42.000000 dm_pix-0.4.1/requirements_examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 10:35:42.000000 dm_pix-0.4.1/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:35:53.652793 dm_pix-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-05 10:35:42.000000 dm_pix-0.4.1/setup.py
```

### Comparing `dm_pix-0.4.0/LICENSE` & `dm_pix-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/PKG-INFO` & `dm_pix-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm_pix
-Version: 0.4.0
+Version: 0.4.1
 Summary: PIX is an image processing library in JAX, for JAX.
 Home-page: https://github.com/deepmind/dm_pix
 Author: DeepMind
 Author-email: pix-dev@google.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dm_pix-0.4.0/README.md` & `dm_pix-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/__init__.py` & `dm_pix-0.4.1/dm_pix/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 from dm_pix._src import augment
 from dm_pix._src import color_conversion
 from dm_pix._src import depth_and_space
 from dm_pix._src import interpolation
 from dm_pix._src import metrics
 from dm_pix._src import patch
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 # Augmentations.
 adjust_brightness = augment.adjust_brightness
 adjust_contrast = augment.adjust_contrast
 adjust_gamma = augment.adjust_gamma
 adjust_hue = augment.adjust_hue
 adjust_saturation = augment.adjust_saturation
 affine_transform = augment.affine_transform
+center_crop = augment.center_crop
 elastic_deformation = augment.elastic_deformation
 flip_left_right = augment.flip_left_right
 flip_up_down = augment.flip_up_down
 gaussian_blur = augment.gaussian_blur
+pad_to_size = augment.pad_to_size
 random_brightness = augment.random_brightness
 random_contrast = augment.random_contrast
 random_crop = augment.random_crop
 random_flip_left_right = augment.random_flip_left_right
 random_flip_up_down = augment.random_flip_up_down
 random_gamma = augment.random_gamma
 random_hue = augment.random_hue
 random_saturation = augment.random_saturation
+resize_with_crop_or_pad = augment.resize_with_crop_or_pad
 rotate = augment.rotate
 rot90 = augment.rot90
 solarize = augment.solarize
 
 # Color conversions.
 hsl_to_rgb = color_conversion.hsl_to_rgb
 hsv_to_rgb = color_conversion.hsv_to_rgb
@@ -77,35 +80,38 @@
 __all__ = (
     "adjust_brightness",
     "adjust_contrast",
     "adjust_gamma",
     "adjust_hue",
     "adjust_saturation",
     "affine_transform",
+    "center_crop",
     "depth_to_space",
     "elastic_deformation",
     "extract_patches",
     "flat_nd_linear_interpolate",
     "flat_nd_linear_interpolate_constant",
     "flip_left_right",
     "flip_up_down",
     "gaussian_blur",
     "hsl_to_rgb",
     "hsv_to_rgb",
     "mae",
     "mse",
+    "pad_to_size",
     "psnr",
     "random_brightness",
     "random_contrast",
     "random_crop",
     "random_flip_left_right",
     "random_flip_up_down",
     "random_gamma",
     "random_hue",
     "random_saturation",
+    "resize_with_crop_or_pad",
     "rotate",
     "rgb_to_hsl",
     "rgb_to_hsv",
     "rgb_to_grayscale",
     "rmse",
     "rot90",
     "simse",
```

### Comparing `dm_pix-0.4.0/dm_pix/_src/__init__.py` & `dm_pix-0.4.1/dm_pix/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/api_test.py` & `dm_pix-0.4.1/dm_pix/_src/api_test.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/augment.py` & `dm_pix-0.4.1/dm_pix/_src/augment.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 All functions expect float-encoded images, with values in [0, 1].
 Do not clip their outputs to this range to allow chaining without losing
 information. The outside-of-bounds behavior is (as much as possible) similar to
 that of TensorFlow.
 """
 
 import functools
-from typing import Callable, Sequence, Tuple, Union
+from typing import Any, Callable, Optional, Sequence, Tuple, Union
 
 import chex
 from dm_pix._src import color_conversion
 from dm_pix._src import interpolation
 import jax
 import jax.numpy as jnp
 
@@ -235,14 +235,166 @@
 
   if channel_axis != -1:  # Set channel axis back to original index.
     transformed_image = jnp.moveaxis(
         transformed_image, source=-1, destination=channel_axis)
   return transformed_image
 
 
+def center_crop(
+    image: chex.Array,
+    height: chex.Numeric,
+    width: chex.Numeric,
+    *,
+    channel_axis: int = -1,
+) -> chex.Array:
+  """Crops an image to the given size keeping the same center of the original.
+
+  Target height/width given can be greater than the current size of the image
+  which results in being a no-op for that dimension.
+
+  In case of odd size along any dimension the bottom/right side gets the extra
+  pixel.
+
+  Args:
+    image: a JAX array representing an image. Assumes that the image is either
+      ...HWC or ...CHW.
+    height: target height to crop the image to.
+    width: target width to crop the image to.
+    channel_axis: the index of the channel axis.
+
+  Returns:
+    The cropped image(s).
+  """
+  chex.assert_rank(image, {3, 4})
+  batch, current_height, current_width, channel = _get_dimension_values(
+      image=image, channel_axis=channel_axis
+  )
+  center_h, center_w = current_height // 2, current_width // 2
+
+  left = max(center_w - (width // 2), 0)
+  right = min(left + width, current_width)
+  top = max(center_h - (height // 2), 0)
+  bottom = min(top + height, current_height)
+
+  if _channels_last(image, channel_axis):
+    start_indices = (top, left, 0)
+    limit_indices = (bottom, right, channel)
+  else:
+    start_indices = (0, top, left)
+    limit_indices = (channel, bottom, right)
+
+  if batch is not None:  # In case batch of images is given.
+    start_indices = (0, *start_indices)
+    limit_indices = (batch, *limit_indices)
+
+  return jax.lax.slice(
+      image, start_indices=start_indices, limit_indices=limit_indices
+  )
+
+
+def pad_to_size(
+    image: chex.Array,
+    target_height: int,
+    target_width: int,
+    *,
+    mode: str = "constant",
+    pad_kwargs: Optional[Any] = None,
+    channel_axis: int = -1,
+) -> chex.Array:
+  """Pads an image to the given size keeping the original image centered.
+
+  For different padding methods and kwargs please see:
+  https://jax.readthedocs.io/en/latest/_autosummary/jax.numpy.pad.html
+
+  In case of odd size difference along any dimension the bottom/right side gets
+  the extra padding pixel.
+
+  Target size can be smaller than original size which results in a no-op for
+  such dimension.
+
+  Args:
+    image: a JAX array representing an image. Assumes that the image is either
+      ...HWC or ...CHW.
+    target_height: target height to pad the image to.
+    target_width: target width to pad the image to.
+    mode: Mode for padding the images, see jax.numpy.pad for details. Default is
+      `constant`.
+    pad_kwargs: Keyword arguments to pass jax.numpy.pad, see documentation for
+      options.
+    channel_axis: the index of the channel axis.
+
+  Returns:
+    The padded image(s).
+  """
+  chex.assert_rank(image, {3, 4})
+  batch, height, width, _ = _get_dimension_values(
+      image=image, channel_axis=channel_axis
+  )
+  delta_width = max(target_width - width, 0)
+  delta_height = max(target_height - height, 0)
+  if delta_width == 0 and delta_height == 0:
+    return image
+
+  left = delta_width // 2
+  right = max(target_width - (left + width), 0)
+  top = delta_height // 2
+  bottom = max(target_height - (top + height), 0)
+
+  pad_width = ((top, bottom), (left, right), (0, 0))
+  if batch:
+    pad_width = ((0, 0), *pad_width)
+
+  return jnp.pad(image, pad_width=pad_width, mode=mode, **pad_kwargs or {})
+
+
+def resize_with_crop_or_pad(
+    image: chex.Array,
+    target_height: chex.Numeric,
+    target_width: chex.Numeric,
+    *,
+    pad_mode: str = "constant",
+    pad_kwargs: Optional[Any] = None,
+    channel_axis: int = -1,
+) -> chex.Array:
+  """Crops and/or pads an image to a target width and height.
+
+  Equivalent in functionality to tf.image.resize_with_crop_or_pad but allows for
+  different padding methods as well beyond zero padding.
+
+  Args:
+    image: a JAX array representing an image. Assumes that the image is either
+      ...HWC or ...CHW.
+    target_height: target height to crop or pad the image to.
+    target_width: target width to crop or pad the image to.
+    pad_mode: mode for padding the images, see jax.numpy.pad for details.
+      Default is `constant`.
+    pad_kwargs: keyword arguments to pass jax.numpy.pad, see documentation for
+      options.
+    channel_axis: the index of the channel axis.
+
+  Returns:
+    The image(s) resized by crop or pad to the desired target size.
+  """
+  chex.assert_rank(image, {3, 4})
+  image = center_crop(
+      image,
+      height=target_height,
+      width=target_width,
+      channel_axis=channel_axis,
+  )
+  return pad_to_size(
+      image,
+      target_height=target_height,
+      target_width=target_width,
+      channel_axis=channel_axis,
+      mode=pad_mode,
+      pad_kwargs=pad_kwargs,
+  )
+
+
 def flip_left_right(
     image: chex.Array,
     *,
     channel_axis: int = -1,
 ) -> chex.Array:
   """Flips an image along the horizontal axis.
 
@@ -791,7 +943,40 @@
   elif mode == "constant" and order == 1:
     interpolate_function = functools.partial(
         interpolation.flat_nd_linear_interpolate_constant, cval=cval)
   else:
     interpolate_function = functools.partial(
         jax.scipy.ndimage.map_coordinates, mode=mode, order=order, cval=cval)
   return interpolate_function
+
+
+def _get_dimension_values(
+    image: chex.Array,
+    channel_axis: int,
+) -> Tuple[Optional[int], int, int, int]:
+  """Gets shape values in BHWC order.
+
+  If single image is given B is None.
+
+  Small utility to get dimension values regardless of channel axis and single
+  image or batch of images are passed.
+
+  Args:
+    image: a JAX array representing an image. Assumes that the image is either
+      ...HWC or ...CHW.
+    channel_axis: channel_axis: the index of the channel axis.
+
+  Returns:
+    A tuple with the values of each dimension in order BHWC.
+  """
+  chex.assert_rank(image, {3, 4})
+  if image.ndim == 4:
+    if _channels_last(image=image, channel_axis=channel_axis):
+      batch, height, width, channel = image.shape
+    else:
+      batch, channel, height, width = image.shape
+  else:
+    if _channels_last(image=image, channel_axis=channel_axis):
+      batch, (height, width, channel) = None, image.shape
+    else:
+      batch, (channel, height, width) = None, image.shape
+  return batch, height, width, channel
```

### Comparing `dm_pix-0.4.0/dm_pix/_src/augment_test.py` & `dm_pix-0.4.1/dm_pix/_src/augment_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -351,19 +351,89 @@
     # Sigma has to be constant for jit since kernel_size is derived from it.
     self._test_fn_with_random_arg(
         images_list,
         jax_fn=elastic_deformation,
         reference_fn=None,
         alpha=(40, 80))
 
+  @parameterized.product(
+      images_list=(_RAND_FLOATS_IN_RANGE, _RAND_FLOATS_OUT_OF_RANGE),
+      height=(131, 111, 1, 88),
+      width=(111, 105, 1, 40),
+  )
+  def test_center_crop(self, images_list, height, width):
+    center_crop = functools.partial(
+        augment.center_crop,
+        height=height,
+        width=width,
+    )
+    # Using layer as reference as other tf utility functions are not exactly
+    # this same center crop:
+    # - tf.image.crop_and_resize
+    # - tf.image.central_crop
+    reference = tf.keras.layers.CenterCrop(
+        height=height,
+        width=width,
+    )
+    self._test_fn(images_list, jax_fn=center_crop, reference_fn=reference)
+
+  @parameterized.product(
+      images_list=(_RAND_FLOATS_IN_RANGE, _RAND_FLOATS_OUT_OF_RANGE),
+      target_height=(156, 131, 200, 251),
+      target_width=(156, 111, 200, 251),
+  )
+  def test_pad_to_size(self, images_list, target_height, target_width):
+    pad_fn = functools.partial(
+        augment.pad_to_size,
+        target_height=target_height,
+        target_width=target_width,
+        mode="constant",
+        pad_kwargs={"constant_values": 0},
+    )
+    # We have to rely on `resize_with_crop_or_pad` as there are no pad to size
+    # equivalents.
+    reference_fn = functools.partial(
+        tf.image.resize_with_crop_or_pad,
+        target_height=target_height,
+        target_width=target_width,
+    )
+
+    self._test_fn(images_list, jax_fn=pad_fn, reference_fn=reference_fn)
+
+  @parameterized.product(
+      images_list=(_RAND_FLOATS_IN_RANGE, _RAND_FLOATS_OUT_OF_RANGE),
+      target_height=(156, 138, 200, 251),
+      target_width=(156, 138, 200, 251),
+  )
+  def test_resize_with_crop_or_pad(
+      self, images_list, target_height, target_width
+  ):
+    resize_crop_or_pad = functools.partial(
+        augment.resize_with_crop_or_pad,
+        target_height=target_height,
+        target_width=target_width,
+        pad_mode="constant",
+        pad_kwargs={"constant_values": 0},
+    )
+    reference_fn = functools.partial(
+        tf.image.resize_with_crop_or_pad,
+        target_height=target_height,
+        target_width=target_width,
+    )
+
+    self._test_fn(
+        images_list, jax_fn=resize_crop_or_pad, reference_fn=reference_fn
+    )
+
 
 class TestMatchReference(_ImageAugmentationTest):
 
-  def _test_fn_with_random_arg(self, images_list, jax_fn, reference_fn,
-                               **kw_range):
+  def _test_fn_with_random_arg(
+      self, images_list, jax_fn, reference_fn, **kw_range
+  ):
     if reference_fn is None:
       return
     assert len(kw_range) == 1
     kw_name, (random_min, random_max) = list(kw_range.items())[0]
     for image_rgb in images_list:
       argument = np.random.uniform(random_min, random_max, size=())
       adjusted_jax = jax_fn(image_rgb, **{kw_name: argument})
@@ -434,10 +504,62 @@
     jax_fn_jitted = jax.jit(jax_fn)
     for image_rgb in images_list:
       adjusted_jax = jax_fn(image_rgb)
       adjusted_jit = jax_fn_jitted(image_rgb)
       self.assertAllCloseTolerant(adjusted_jax, adjusted_jit)
 
 
+class TestCustom(parameterized.TestCase):
+  """Tests custom logic that is not covered by reference functions."""
+
+  @parameterized.product(
+      images_list=(_RAND_FLOATS_IN_RANGE, _RAND_FLOATS_OUT_OF_RANGE),
+      height=(250, 200),
+      width=(250, 200),
+      expected_height=(131, 131),
+      expected_width=(111, 111),
+  )
+  def test_center_crop_size_bigger_than_original(
+      self,
+      images_list,
+      height,
+      width,
+      expected_height,
+      expected_width,
+  ):
+    output = augment.center_crop(
+        image=jnp.array(images_list),
+        height=height,
+        width=width,
+    )
+
+    self.assertEqual(output.shape[1], expected_height)
+    self.assertEqual(output.shape[2], expected_width)
+
+  @parameterized.product(
+      images_list=(_RAND_FLOATS_IN_RANGE, _RAND_FLOATS_OUT_OF_RANGE),
+      target_height=(55, 84),
+      target_width=(55, 84),
+      expected_height=(131, 131),
+      expected_width=(111, 111),
+  )
+  def test_pad_to_size_when_target_size_smaller_than_original(
+      self,
+      images_list,
+      target_height,
+      target_width,
+      expected_height,
+      expected_width,
+  ):
+    output = augment.pad_to_size(
+        image=jnp.array(images_list),
+        target_height=target_height,
+        target_width=target_width,
+    )
+
+    self.assertEqual(output.shape[1], expected_height)
+    self.assertEqual(output.shape[2], expected_width)
+
+
 if __name__ == "__main__":
   jax.config.update("jax_default_matmul_precision", "float32")
   absltest.main()
```

### Comparing `dm_pix-0.4.0/dm_pix/_src/color_conversion.py` & `dm_pix-0.4.1/dm_pix/_src/color_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
   Args:
     image_rgb: an RGB image, with float values in range [0, 1]. Behavior outside
       of these bounds is not guaranteed.
     channel_axis: the channel axis. image_rgb should have 3 layers along this
       axis.
 
   Returns:
-    An HSV image, with float values in range [0, 1], stacked along channel_axis.
+    An HSL image, with float values in range [0, 1], stacked along channel_axis.
   """
   red, green, blue = split_channels(image_rgb, channel_axis)
 
   c_max = jnp.maximum(red, jnp.maximum(green, blue))
   c_min = jnp.minimum(red, jnp.minimum(green, blue))
   c_sum = c_max + c_min
   c_diff = c_max - c_min
```

### Comparing `dm_pix-0.4.0/dm_pix/_src/color_conversion_test.py` & `dm_pix-0.4.1/dm_pix/_src/color_conversion_test.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/depth_and_space.py` & `dm_pix-0.4.1/dm_pix/_src/depth_and_space.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/depth_and_space_test.py` & `dm_pix-0.4.1/dm_pix/_src/depth_and_space_test.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/interpolation.py` & `dm_pix-0.4.1/dm_pix/_src/interpolation.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/interpolation_test.py` & `dm_pix-0.4.1/dm_pix/_src/interpolation_test.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/metrics.py` & `dm_pix-0.4.1/dm_pix/_src/metrics.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/metrics_test.py` & `dm_pix-0.4.1/dm_pix/_src/metrics_test.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/patch.py` & `dm_pix-0.4.1/dm_pix/_src/patch.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/patch_test.py` & `dm_pix-0.4.1/dm_pix/_src/patch_test.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix/_src/test_utils.py` & `dm_pix-0.4.1/dm_pix/_src/test_utils.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/dm_pix.egg-info/PKG-INFO` & `dm_pix-0.4.1/dm_pix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-pix
-Version: 0.4.0
+Version: 0.4.1
 Summary: PIX is an image processing library in JAX, for JAX.
 Home-page: https://github.com/deepmind/dm_pix
 Author: DeepMind
 Author-email: pix-dev@google.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dm_pix-0.4.0/dm_pix.egg-info/SOURCES.txt` & `dm_pix-0.4.1/dm_pix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/docs/conf.py` & `dm_pix-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/docs/ext/coverage_check.py` & `dm_pix-0.4.1/docs/ext/coverage_check.py`

 * *Files identical despite different names*

### Comparing `dm_pix-0.4.0/setup.py` & `dm_pix-0.4.1/setup.py`

 * *Files identical despite different names*

