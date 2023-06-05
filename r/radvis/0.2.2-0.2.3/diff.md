# Comparing `tmp/radvis-0.2.2.tar.gz` & `tmp/radvis-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radvis-0.2.2.tar", last modified: Mon May 29 05:35:51 2023, max compression
+gzip compressed data, was "radvis-0.2.3.tar", last modified: Mon Jun  5 03:40:46 2023, max compression
```

## Comparing `radvis-0.2.2.tar` & `radvis-0.2.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.154143 radvis-0.2.2/
--rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4225 2023-05-29 05:35:51.153149 radvis-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3922 2023-05-29 03:06:20.000000 radvis-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.113148 radvis-0.2.2/radvis/
--rw-rw-rw-   0        0        0      357 2023-05-29 05:35:20.000000 radvis-0.2.2/radvis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.133148 radvis-0.2.2/radvis/image/
--rw-rw-rw-   0        0        0       78 2023-05-29 02:23:29.000000 radvis-0.2.2/radvis/image/__init__.py
--rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.2.2/radvis/image/load.py
--rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.2.2/radvis/image/rad_dicom_image.py
--rw-rw-rw-   0        0        0     3673 2023-05-29 02:54:49.000000 radvis-0.2.2/radvis/image/rad_image.py
--rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.2.2/radvis/image/rad_nifti_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.136150 radvis-0.2.2/radvis/mesh/
--rw-rw-rw-   0        0        0      130 2023-05-29 03:00:11.000000 radvis-0.2.2/radvis/mesh/__init__.py
--rw-rw-rw-   0        0        0     1618 2023-05-29 03:00:19.000000 radvis-0.2.2/radvis/mesh/compute_mesh.py
--rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.2.2/radvis/mesh/rad_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.139142 radvis-0.2.2/radvis/processing/
--rw-rw-rw-   0        0        0      171 2023-05-29 03:20:54.000000 radvis-0.2.2/radvis/processing/__init__.py
--rw-rw-rw-   0        0        0     3165 2023-05-29 03:04:44.000000 radvis-0.2.2/radvis/processing/image.py
--rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.2.2/radvis/processing/registration.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.142142 radvis-0.2.2/radvis/visualize/
--rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.2.2/radvis/visualize/__init__.py
--rw-rw-rw-   0        0        0     8860 2023-05-29 00:55:04.000000 radvis-0.2.2/radvis/visualize/rad_slicer.py
--rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.2.2/radvis/visualize/rad_slicer_group.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.127147 radvis-0.2.2/radvis.egg-info/
--rw-rw-rw-   0        0        0     4225 2023-05-29 05:35:50.000000 radvis-0.2.2/radvis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      874 2023-05-29 05:35:51.000000 radvis-0.2.2/radvis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 05:35:50.000000 radvis-0.2.2/radvis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-29 05:35:50.000000 radvis-0.2.2/radvis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-29 05:35:50.000000 radvis-0.2.2/radvis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 05:35:51.154143 radvis-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-05-29 05:35:41.000000 radvis-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.143141 radvis-0.2.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.2.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.145143 radvis-0.2.2/tests/mocks/
--rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.2.2/tests/mocks/__init__.py
--rw-rw-rw-   0        0        0      455 2023-05-29 02:42:01.000000 radvis-0.2.2/tests/mocks/mock_rad_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.148142 radvis-0.2.2/tests/test_mesh/
--rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.2.2/tests/test_mesh/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.2.2/tests/test_mesh/test_compute_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.150148 radvis-0.2.2/tests/test_processing/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:40:16.000000 radvis-0.2.2/tests/test_processing/__init__.py
--rw-rw-rw-   0        0        0     1645 2023-05-29 02:59:47.000000 radvis-0.2.2/tests/test_processing/test_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:35:51.152143 radvis-0.2.2/tests/test_visualize/
--rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.2.2/tests/test_visualize/__init__.py
--rw-rw-rw-   0        0        0      837 2023-05-29 02:59:35.000000 radvis-0.2.2/tests/test_visualize/test_rad_slicer.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.318421 radvis-0.2.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3768 2023-06-05 03:40:46.317422 radvis-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3467 2023-06-05 03:40:01.000000 radvis-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.278073 radvis-0.2.3/radvis/
+-rw-rw-rw-   0        0        0      357 2023-05-29 05:35:20.000000 radvis-0.2.3/radvis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.300665 radvis-0.2.3/radvis/image/
+-rw-rw-rw-   0        0        0       78 2023-05-29 02:23:29.000000 radvis-0.2.3/radvis/image/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.2.3/radvis/image/load.py
+-rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.2.3/radvis/image/rad_dicom_image.py
+-rw-rw-rw-   0        0        0     3673 2023-05-29 02:54:49.000000 radvis-0.2.3/radvis/image/rad_image.py
+-rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.2.3/radvis/image/rad_nifti_image.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.302661 radvis-0.2.3/radvis/mesh/
+-rw-rw-rw-   0        0        0      130 2023-05-29 03:00:11.000000 radvis-0.2.3/radvis/mesh/__init__.py
+-rw-rw-rw-   0        0        0     1618 2023-05-29 03:00:19.000000 radvis-0.2.3/radvis/mesh/compute_mesh.py
+-rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.2.3/radvis/mesh/rad_mesh.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.306172 radvis-0.2.3/radvis/processing/
+-rw-rw-rw-   0        0        0      171 2023-05-29 03:20:54.000000 radvis-0.2.3/radvis/processing/__init__.py
+-rw-rw-rw-   0        0        0     3165 2023-05-29 03:04:44.000000 radvis-0.2.3/radvis/processing/image.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.2.3/radvis/processing/registration.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.309176 radvis-0.2.3/radvis/visualize/
+-rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.2.3/radvis/visualize/__init__.py
+-rw-rw-rw-   0        0        0     9409 2023-06-05 03:35:02.000000 radvis-0.2.3/radvis/visualize/rad_slicer.py
+-rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.2.3/radvis/visualize/rad_slicer_group.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.295655 radvis-0.2.3/radvis.egg-info/
+-rw-rw-rw-   0        0        0     3768 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      874 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 03:40:46.318421 radvis-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-06-05 03:29:31.000000 radvis-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.310176 radvis-0.2.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.2.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.311238 radvis-0.2.3/tests/mocks/
+-rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.2.3/tests/mocks/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-05-29 02:42:01.000000 radvis-0.2.3/tests/mocks/mock_rad_image.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.313245 radvis-0.2.3/tests/test_mesh/
+-rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.2.3/tests/test_mesh/__init__.py
+-rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.2.3/tests/test_mesh/test_compute_mesh.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.315245 radvis-0.2.3/tests/test_processing/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:40:16.000000 radvis-0.2.3/tests/test_processing/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-05-29 02:59:47.000000 radvis-0.2.3/tests/test_processing/test_image.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.316421 radvis-0.2.3/tests/test_visualize/
+-rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.2.3/tests/test_visualize/__init__.py
+-rw-rw-rw-   0        0        0      837 2023-05-29 02:59:35.000000 radvis-0.2.3/tests/test_visualize/test_rad_slicer.py
```

### Comparing `radvis-0.2.2/LICENSE` & `radvis-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/PKG-INFO` & `radvis-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.2.2
+Version: 0.2.3
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -71,37 +71,38 @@
 image = rv.load_image(IMAGE_PATH)
 mask = rv.load_image(IMAGE_MASK_PATH)
 
 slicer = rv.RadSlicer(image, AXIS, width=3)
 slicer.add_mask(mask, color="red", alpha=0.3)
 
 slicer.display()
-# slicer.save_animation(f"images/axis_{AXIS}_brain_seg.gif", fps=30)
+slicer.save_animation(f"images/axis_{AXIS}_brain_seg.gif", fps=30)
+slicer.save_frame(f"images/axis_{AXIS}_brain_seg.png", index=180, dpi=300)
 ```
 
 <p float="left">
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_1_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PZ2WT3CJ26PONDN2YZC7T46Q" width="49%" /> 
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_2_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PDVRWL2CW2OCTUV3CZC7T5BQ" width="49%" />
 </p>
 
 ## Processing Module
 
 The processing module of RadVis offers a set of functions to perform preprocessing tasks
 
 ### Clipping
-The `percentile_clipping` function allows you to clip the pixel intensities of an image at specified lower and upper percentiles. This can be helpful in enhancing the contrast of the image.
+The `percentile_clipping` function clips pixel intensities above and below percentile ranges
 
 ### Noise Reduction
-The `noise_reduction` function can be used to reduce the amount of noise in your images, which is particularly useful for medical images where noise can often interfere with the analysis.
+The `noise_reduction` function reduces the amount of noise in the image
 
 ### Normalization
-The `normalization` function is used to normalize the pixel intensities of the image to a specified range. This is useful for preparing your images for machine learning models, which often perform better when the input data is normalized.
+The `normalization` function normalizes the pixel intensities of the image to a specified range.
 
 ### Padding
-The `add_padding` function can be used to add padding to your images, which can be useful when you need to make all your images the same size for subsequent analysis or to apply a neural network that requires input images to be of a certain size.
+The `add_padding` function adds padding evenly to match a target shape
 
 Example usage of processing functions:
 
 ```python
 import radvis as rv
 import numpy as np
```

### Comparing `radvis-0.2.2/README.md` & `radvis-0.2.3/radvis.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: radvis
+Version: 0.2.3
+Summary: A visualization tool for medical images
+Home-page: https://github.com/medlee-code/RadVis
+Author: Matthew lee
+Author-email: matthewlee@medlee.io
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # RadVis
 RadVis (Radiology Visualization) is a visualization tool for medical images.
 
 Currently implemented features:
 - Load both DICOM and NIFTI images
 - Can display 2D slices of the 3D images
 - Ability to add a mask to the image
@@ -60,37 +71,38 @@
 image = rv.load_image(IMAGE_PATH)
 mask = rv.load_image(IMAGE_MASK_PATH)
 
 slicer = rv.RadSlicer(image, AXIS, width=3)
 slicer.add_mask(mask, color="red", alpha=0.3)
 
 slicer.display()
-# slicer.save_animation(f"images/axis_{AXIS}_brain_seg.gif", fps=30)
+slicer.save_animation(f"images/axis_{AXIS}_brain_seg.gif", fps=30)
+slicer.save_frame(f"images/axis_{AXIS}_brain_seg.png", index=180, dpi=300)
 ```
 
 <p float="left">
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_1_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PZ2WT3CJ26PONDN2YZC7T46Q" width="49%" /> 
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_2_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PDVRWL2CW2OCTUV3CZC7T5BQ" width="49%" />
 </p>
 
 ## Processing Module
 
 The processing module of RadVis offers a set of functions to perform preprocessing tasks
 
 ### Clipping
-The `percentile_clipping` function allows you to clip the pixel intensities of an image at specified lower and upper percentiles. This can be helpful in enhancing the contrast of the image.
+The `percentile_clipping` function clips pixel intensities above and below percentile ranges
 
 ### Noise Reduction
-The `noise_reduction` function can be used to reduce the amount of noise in your images, which is particularly useful for medical images where noise can often interfere with the analysis.
+The `noise_reduction` function reduces the amount of noise in the image
 
 ### Normalization
-The `normalization` function is used to normalize the pixel intensities of the image to a specified range. This is useful for preparing your images for machine learning models, which often perform better when the input data is normalized.
+The `normalization` function normalizes the pixel intensities of the image to a specified range.
 
 ### Padding
-The `add_padding` function can be used to add padding to your images, which can be useful when you need to make all your images the same size for subsequent analysis or to apply a neural network that requires input images to be of a certain size.
+The `add_padding` function adds padding evenly to match a target shape
 
 Example usage of processing functions:
 
 ```python
 import radvis as rv
 import numpy as np
 
@@ -102,8 +114,8 @@
 filtered_image = rv.processing.noise_reduction(clipped_image, filter_size=1)
 normalized_image = rv.processing.normalization(filtered_image, min_val=0, max_val=255)
 padded_image = rv.processing.add_padding(normalized_image, target_shape=(128, 128, 128))
 
 # Displaying processed image
 slicer = rv.RadSlicer(padded_image, axis=0)
 slicer.display()
-```
+```
```

### Comparing `radvis-0.2.2/radvis/image/load.py` & `radvis-0.2.3/radvis/image/load.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/radvis/image/rad_dicom_image.py` & `radvis-0.2.3/radvis/image/rad_dicom_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/radvis/image/rad_image.py` & `radvis-0.2.3/radvis/image/rad_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/radvis/image/rad_nifti_image.py` & `radvis-0.2.3/radvis/image/rad_nifti_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/radvis/mesh/compute_mesh.py` & `radvis-0.2.3/radvis/mesh/compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/radvis/mesh/rad_mesh.py` & `radvis-0.2.3/radvis/mesh/rad_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/radvis/processing/image.py` & `radvis-0.2.3/radvis/processing/image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/radvis/visualize/rad_slicer.py` & `radvis-0.2.3/radvis/visualize/rad_slicer.py`

 * *Files 13% similar despite different names*

```diff
@@ -214,23 +214,39 @@
         Save an animation of all slices to a GIF file.
 
         :param filepath: The path to save the animation to
         :param fps: The frames per second for the animation, defaults to 10
         """
         # Ensure display has been called at least once
         if self._ax is None:
-            self.display()
+            self.display(show_plot=False)
 
         # Create the animation
         anim = FuncAnimation(self.fig, self._update_image, frames=self.radimage.shape[self.axis], interval=1000//fps)
 
         try:
             anim.save(filepath, writer=PillowWriter(fps=fps))
         except Exception as e:
             print(f"Could not save the animation due to the following error: {e}")
+
+    def save_frame(self, filepath: str, index: int = 0, dpi: int = 72) -> None:
+        """
+        Save a single frame of the RadSlicer plot to a PNG file.
+
+        :param filepath: The path to save the frame to
+        :param index: The slice index to save, defaults to 0
+        """
+        # Ensure display has been called at least once
+        if self._ax is None:
+            self.display(show_plot=False)
+
+        # Save the frame
+        self._update_image(index)
+
+        self.fig.savefig(filepath, dpi=dpi)
             
     def copy(self):
         """
         Create a copy of the RadSlicer object.
         """
         return copy.deepcopy(self)
```

### Comparing `radvis-0.2.2/radvis/visualize/rad_slicer_group.py` & `radvis-0.2.3/radvis/visualize/rad_slicer_group.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/radvis.egg-info/SOURCES.txt` & `radvis-0.2.3/radvis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/setup.py` & `radvis-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='radvis',
-    version='0.2.2',
+    version='0.2.3',
     url='https://github.com/medlee-code/RadVis',
     author='Matthew lee',
     author_email='matthewlee@medlee.io',
     description='A visualization tool for medical images',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `radvis-0.2.2/tests/test_mesh/test_compute_mesh.py` & `radvis-0.2.3/tests/test_mesh/test_compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/tests/test_processing/test_image.py` & `radvis-0.2.3/tests/test_processing/test_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.2/tests/test_visualize/test_rad_slicer.py` & `radvis-0.2.3/tests/test_visualize/test_rad_slicer.py`

 * *Files identical despite different names*

