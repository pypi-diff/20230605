# Comparing `tmp/segmenteverygrain-0.0.2.tar.gz` & `tmp/segmenteverygrain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmenteverygrain-0.0.2.tar", last modified: Sat Jun  3 00:23:16 2023, max compression
+gzip compressed data, was "segmenteverygrain-0.0.3.tar", last modified: Mon Jun  5 01:12:51 2023, max compression
```

## Comparing `segmenteverygrain-0.0.2.tar` & `segmenteverygrain-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-03 00:23:16.407230 segmenteverygrain-0.0.2/
--rw-r--r--   0 zoltan     (502) staff       (20)    11350 2023-05-24 19:25:16.000000 segmenteverygrain-0.0.2/LICENSE.txt
--rw-r--r--   0 zoltan     (502) staff       (20)     4022 2023-06-03 00:23:16.407104 segmenteverygrain-0.0.2/PKG-INFO
--rw-r--r--   0 zoltan     (502) staff       (20)     3270 2023-05-29 21:10:25.000000 segmenteverygrain-0.0.2/README.md
--rw-r--r--   0 zoltan     (502) staff       (20)      664 2023-06-03 00:22:58.000000 segmenteverygrain-0.0.2/pyproject.toml
-drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-03 00:23:16.405835 segmenteverygrain-0.0.2/segmenteverygrain/
--rw-r--r--   0 zoltan     (502) staff       (20)       59 2023-05-25 16:54:43.000000 segmenteverygrain-0.0.2/segmenteverygrain/__init__.py
--rw-r--r--   0 zoltan     (502) staff       (20)    31747 2023-06-03 00:06:35.000000 segmenteverygrain-0.0.2/segmenteverygrain/segmenteverygrain.py
-drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-03 00:23:16.406921 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/
--rw-r--r--   0 zoltan     (502) staff       (20)     4022 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/PKG-INFO
--rw-r--r--   0 zoltan     (502) staff       (20)      318 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/SOURCES.txt
--rw-r--r--   0 zoltan     (502) staff       (20)        1 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/dependency_links.txt
--rw-r--r--   0 zoltan     (502) staff       (20)      116 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/requires.txt
--rw-r--r--   0 zoltan     (502) staff       (20)       18 2023-06-03 00:23:16.000000 segmenteverygrain-0.0.2/segmenteverygrain.egg-info/top_level.txt
--rw-r--r--   0 zoltan     (502) staff       (20)       38 2023-06-03 00:23:16.407269 segmenteverygrain-0.0.2/setup.cfg
--rw-r--r--   0 zoltan     (502) staff       (20)      961 2023-06-03 00:22:55.000000 segmenteverygrain-0.0.2/setup.py
+drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-05 01:12:51.605831 segmenteverygrain-0.0.3/
+-rw-r--r--   0 zoltan     (502) staff       (20)    11350 2023-05-24 19:25:16.000000 segmenteverygrain-0.0.3/LICENSE.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)     4020 2023-06-05 01:12:51.605684 segmenteverygrain-0.0.3/PKG-INFO
+-rw-r--r--   0 zoltan     (502) staff       (20)     3268 2023-06-05 01:05:16.000000 segmenteverygrain-0.0.3/README.md
+-rw-r--r--   0 zoltan     (502) staff       (20)      664 2023-06-05 01:12:13.000000 segmenteverygrain-0.0.3/pyproject.toml
+drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-05 01:12:51.598718 segmenteverygrain-0.0.3/segmenteverygrain/
+-rw-r--r--   0 zoltan     (502) staff       (20)       59 2023-05-25 16:54:43.000000 segmenteverygrain-0.0.3/segmenteverygrain/__init__.py
+-rw-r--r--   0 zoltan     (502) staff       (20)    31539 2023-06-05 00:55:34.000000 segmenteverygrain-0.0.3/segmenteverygrain/segmenteverygrain.py
+drwxr-xr-x   0 zoltan     (502) staff       (20)        0 2023-06-05 01:12:51.605422 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/
+-rw-r--r--   0 zoltan     (502) staff       (20)     4020 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/PKG-INFO
+-rw-r--r--   0 zoltan     (502) staff       (20)      318 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/SOURCES.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)        1 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/dependency_links.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)      116 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/requires.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)       18 2023-06-05 01:12:51.000000 segmenteverygrain-0.0.3/segmenteverygrain.egg-info/top_level.txt
+-rw-r--r--   0 zoltan     (502) staff       (20)       38 2023-06-05 01:12:51.605887 segmenteverygrain-0.0.3/setup.cfg
+-rw-r--r--   0 zoltan     (502) staff       (20)      961 2023-06-05 01:12:17.000000 segmenteverygrain-0.0.3/setup.py
```

### Comparing `segmenteverygrain-0.0.2/LICENSE.txt` & `segmenteverygrain-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `segmenteverygrain-0.0.2/PKG-INFO` & `segmenteverygrain-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: segmenteverygrain
-Version: 0.0.2
+Version: 0.0.3
 Summary: A SAM-based model for segmenting grains in images of grains
 Home-page: https://github.com/zsylvester/segmenteverygrain
 Author: Zoltan Sylvester
 Author-email: Zoltan Sylvester <zoltan.sylvester@beg.utexas.edu>
 Project-URL: Homepage, https://github.com/zsylvester/segmenteverygrain
 Project-URL: Bug Tracker, https://github.com/zsylvester/segmenteverygrain/issues
 Keywords: sedimentology,geomorphology,grain size,segment anything model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Segment Every Grain
+# segmenteverygrain
 
-<img src="https://github.com/zsylvester/segmenteverygrain/blob/main/gravel_example_mask.jpg" width="600">
+<img src="https://github.com/zsylvester/segmenteverygrain/blob/main/gravel_example_mask.png" width="600">
 
 ## Description
 
 'segmenteverygrain' is a Python package that aims to detect grains (or grain-like objects) in images. The goal is to develop an ML model that does a reasonably good job at detecting most of the grains in a photo, so that it will be useful for determining grain size and grain shape, a common task in geomorphology and sedimentary geology. 'segmenteverygrain' relies on the [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything), developed by Meta, for getting high-quality outlines of the grains. However, SAM requires prompts for every object detected and, when used in 'everything' mode, it tends to be slow and results in many overlapping masks and non-grain (background) objects. To deal with these issues, 'segmenteverygrain' relies on a Unet-style, patch-based convolutional neural network to create a first-pass segmentation which is then used as a set of prompts for the SAM-based segmentation. Some of the grains will be missed with this approach, but the segmentations that are created tend to be of high quality. 
 
 'segmenteverygrain' also includes a set of functions that make it possible to clean up the segmentation results: delete and merge objects by clicking on them, and adding grains that were not segmented automatically. The QC-d masks can be saved and added to a dataset of grain images (see the 'images' folder). These images then can be used to improve the Unet model. Many of the images used in the dataset are from the [sedinet](https://github.com/DigitalGrainSize/SediNet) project.
```

### Comparing `segmenteverygrain-0.0.2/README.md` & `segmenteverygrain-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Segment Every Grain
+# segmenteverygrain
 
-<img src="https://github.com/zsylvester/segmenteverygrain/blob/main/gravel_example_mask.jpg" width="600">
+<img src="https://github.com/zsylvester/segmenteverygrain/blob/main/gravel_example_mask.png" width="600">
 
 ## Description
 
 'segmenteverygrain' is a Python package that aims to detect grains (or grain-like objects) in images. The goal is to develop an ML model that does a reasonably good job at detecting most of the grains in a photo, so that it will be useful for determining grain size and grain shape, a common task in geomorphology and sedimentary geology. 'segmenteverygrain' relies on the [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything), developed by Meta, for getting high-quality outlines of the grains. However, SAM requires prompts for every object detected and, when used in 'everything' mode, it tends to be slow and results in many overlapping masks and non-grain (background) objects. To deal with these issues, 'segmenteverygrain' relies on a Unet-style, patch-based convolutional neural network to create a first-pass segmentation which is then used as a set of prompts for the SAM-based segmentation. Some of the grains will be missed with this approach, but the segmentations that are created tend to be of high quality. 
 
 'segmenteverygrain' also includes a set of functions that make it possible to clean up the segmentation results: delete and merge objects by clicking on them, and adding grains that were not segmented automatically. The QC-d masks can be saved and added to a dataset of grain images (see the 'images' folder). These images then can be used to improve the Unet model. Many of the images used in the dataset are from the [sedinet](https://github.com/DigitalGrainSize/SediNet) project.
```

### Comparing `segmenteverygrain-0.0.2/pyproject.toml` & `segmenteverygrain-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "segmenteverygrain"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Zoltan Sylvester", email="zoltan.sylvester@beg.utexas.edu" },
 ]
 description = "A SAM-based model for segmenting grains in images of grains"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `segmenteverygrain-0.0.2/segmenteverygrain/segmenteverygrain.py` & `segmenteverygrain-0.0.3/segmenteverygrain/segmenteverygrain.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import cv2
 import networkx as nx
 import rasterio
 from rasterio.features import rasterize
 
 from skimage import measure, morphology
 from skimage.measure import regionprops, regionprops_table
-from skimage.morphology import label, binary_dilation, binary_erosion, reconstruction
+from skimage.morphology import label, binary_erosion, binary_dilation, binary_opening, reconstruction
 from skimage.segmentation import watershed
 from skimage.io import imread, imshow, concatenate_images
 from skimage.transform import resize
 from skimage.feature import peak_local_max
 
 from shapely.geometry import Polygon, MultiPolygon, LineString, Point
 from shapely.affinity import scale
@@ -189,15 +189,15 @@
     db_labels = dbscan.labels_
     coords_ws = coords[np.where(db_labels == -1)[0]]
     for i in np.unique(db_labels):
         xy = np.mean(coords[np.where(db_labels == i)[0]], axis=0)
         coords_ws = np.vstack((coords_ws, xy))
     coords_ws = coords_ws.astype('int32')
     background_probs = big_im_pred[:,:,0][coords_ws[:,1], coords_ws[:,0]]
-    inds = np.where(background_probs < 0.05)[0]
+    inds = np.where(background_probs < 0.3)[0] # get rid of prompts that are likely to be background
     coords_ws = coords_ws[inds, :]
 
     all_coords = np.vstack((coords_ws, coords_simple))
     return labels_simple, grains, all_coords
 
 def one_point_prompt(x, y, ax, image, predictor):
     input_point = np.array([[x, y]])
@@ -220,32 +220,24 @@
         mask[temp_labels != largest_label] = 0
     else:
         mask = masks[ind]
     contours = measure.find_contours(mask, 0.5)
     sx = contours[0][:,1]
     sy = contours[0][:,0]
     r, c = np.shape(mask)
-    if mask[0,0]: # if the mask contains the upper left corner of the image
-        sx = np.hstack((-0.5, sx, -0.5))
-        sy = np.hstack((-0.5, sy, -0.5))
-    if mask[0,-1]: # if the mask contains the upper right corner of the image
-        sx = np.hstack((c-0.5, sx, c-0.5))
-        sy = np.hstack((-0.5, sy, -0.5))
-    if mask[-1,0]: # if the mask contains the lower left corner of the image
-        sx = np.hstack((-0.5, sx, -0.5))
-        sy = np.hstack((r-0.5, sy, r-0.5))
-    if mask[-1,-1]: # if the mask contains the lower right corner of the image
-        sx = np.hstack((c-0.5, sx, c-0.5))
-        sy = np.hstack((r-0.5, sy, r-0.5))
-    if np.any(mask[0, :]) and np.any(mask[:, -1]) and not mask[0, -1] \
-        or np.any(mask[0, :]) and np.any(mask[:, 0]) and not mask[0, 0] \
-        or np.any(mask[-1, :]) and np.any(mask[:, 0]) and not mask[-1, 0] \
-        or np.any(mask[-1, :]) and np.any(mask[:, -1]) and not mask[-1, -1]:
-        sx = np.hstack((contours[0][:,1], contours[1][:,1]))
-        sy = np.hstack((contours[0][:,0], contours[1][:,0]))
+    if np.any(mask[0, :]) or np.any(mask[-1, :]) or np.any(mask[:, 0]) or np.any(mask[0, -1]):
+        mask = np.pad(mask, 1, mode='constant')
+        contours = measure.find_contours(mask, 0.5)
+        sx = contours[0][:,1]
+        sy = contours[0][:,0]
+        if np.any(mask[1, :]):
+            sy = sy-1
+        if np.any(mask[:,1]):
+            sx = sx-1
+        mask = mask[1:-1, 1:-1]
     color = np.concatenate([np.random.random(3), np.array([0.6])], axis=0)
     ax.fill(sx, sy, facecolor=color, edgecolor='k', alpha=0.5)
     return sx, sy, mask
 
 def multi_point_prompt(x, y, ax, image, predictor):
     input_point = np.array([[x, y]])
     input_label = np.array([1])
@@ -257,33 +249,24 @@
     ind = np.argmax(scores)
     if np.sum(masks[ind])/(image.shape[0]*image.shape[1]) > 0.1:
         scores = np.delete(scores, ind)
         ind = np.argmax(scores)
     contours = measure.find_contours(masks[ind], 0.5)
     sx = contours[0][:,1]
     sy = contours[0][:,0]
-    r, c = np.shape(masks[ind])
-    if masks[ind][0,0]: # if the mask contains the upper left corner of the image
-        sx = np.hstack((-0.5, sx, -0.5))
-        sy = np.hstack((-0.5, sy, -0.5))
-    if masks[ind][0,-1]: # if the mask contains the upper right corner of the image
-        sx = np.hstack((c-0.5, sx, c-0.5))
-        sy = np.hstack((-0.5, sy, -0.5))
-    if masks[ind][-1,0]: # if the mask contains the lower left corner of the image
-        sx = np.hstack((-0.5, sx, -0.5))
-        sy = np.hstack((r-0.5, sy, r-0.5))
-    if masks[ind][-1,-1]: # if the mask contains the lower right corner of the image
-        sx = np.hstack((c-0.5, sx, c-0.5))
-        sy = np.hstack((r-0.5, sy, r-0.5))
-    if np.any(mask[0, :]) and np.any(mask[:, -1]) and not mask[0, -1] \
-        or np.any(mask[0, :]) and np.any(mask[:, 0]) and not mask[0, 0] \
-        or np.any(mask[-1, :]) and np.any(mask[:, 0]) and not mask[-1, 0] \
-        or np.any(mask[-1, :]) and np.any(mask[:, -1]) and not mask[-1, -1]:
-        sx = np.hstack((contours[0][:,1], contours[1][:,1]))
-        sy = np.hstack((contours[0][:,0], contours[1][:,0]))
+    if np.any(mask[0, :]) or np.any(mask[-1, :]) or np.any(mask[:, 0]) or np.any(mask[0, -1]):
+        mask = np.pad(mask, 1, mode='constant')
+        contours = measure.find_contours(mask, 0.5)
+        sx = contours[0][:,1]
+        sy = contours[0][:,0]
+        if np.any(mask[1, :]):
+            sy = sy-1
+        if np.any(mask[:,1]):
+            sx = sx-1
+        mask = mask[1:-1, 1:-1]
     color = np.concatenate([np.random.random(3), np.array([0.6])], axis=0)
     ax.fill(sx, sy, facecolor=color, edgecolor='k', alpha=0.5)
     return sx, sy, masks[ind]
 
 def two_point_prompt(x1, y1, x2, y2, ax, image, predictor):
     input_point = np.array([[x1, y1], [x2, y2]])
     input_label = np.array([1, 0])
@@ -459,29 +442,56 @@
     for j in trange(len(comps)): # second deal with the overlapping objects, one connected component at a time
         polygons = [] # polygons in the connected component
         for i in comps[j]:
             polygons.append(all_grains[i])
         most_similar_polygon = pick_most_similar_polygon(polygons)
         if most_similar_polygon.area > min_area:
             new_grains.append(most_similar_polygon)
-        poly_union = unary_union(polygons)
-        remaining_polys = poly_union.difference(most_similar_polygon) # subtract the most similar polygon from the union of all polygons
-        poly_areas = []
-        if type(remaining_polys) == MultiPolygon:
-            for geom in remaining_polys.geoms:
-                poly_areas.append(geom.area)
-            inds = np.where(np.array(poly_areas) > min_area)[0]
-            for ind in inds:
-                new_grains.append(remaining_polys.geoms[ind])
-        if type(remaining_polys) == Polygon:
-            if remaining_polys.area > min_area:
-                new_grains.append(remaining_polys)
     all_grains = new_grains # replace original list of polygons
     # create labeled image:
     labels = np.zeros(big_im.shape[:-1])
+    for i in trange(len(all_grains)):
+        mask = rasterize(
+            shapes=[all_grains[i]],
+            out_shape=big_im.shape[:-1],
+            fill=0,
+            out=None,
+            transform=rasterio.Affine(1.0, 0.0, 0.0,
+               0.0, 1.0, 0.0),
+            all_touched=False,
+            default_value=1,
+            dtype=None,
+        )
+        labels[(mask==1) & (labels==0)] = i+1
+    remaining_grains_im = big_im_pred[:,:,1].copy()
+    remaining_grains_im[labels > 0] = 0
+    remaining_grains_im[remaining_grains_im>0.8] = 1
+    remaining_grains_im[remaining_grains_im<1] = 0
+    remaining_grains_im = binary_erosion(remaining_grains_im, footprint=np.ones((9, 9)))
+    remaining_grains_im = binary_dilation(remaining_grains_im, footprint=np.ones((12, 12)))
+    labels_remaining_grains, n_elems = measure.label(remaining_grains_im, return_num = True, connectivity=1)
+    for i in range(1, n_elems):
+        if np.sum(mask) > min_area:
+            mask = np.zeros(np.shape(labels_remaining_grains))
+            mask[labels_remaining_grains == i] = 1
+            contours = measure.find_contours(mask, 0.5)
+            sx = contours[0][:,1]
+            sy = contours[0][:,0]
+            if np.any(mask[0, :]) or np.any(mask[-1, :]) or np.any(mask[:, 0]) or np.any(mask[0, -1]):
+                mask = np.pad(mask, 1, mode='constant')
+                contours = measure.find_contours(mask, 0.5)
+                sx = contours[0][:,1]
+                sy = contours[0][:,0]
+                if np.any(mask[1, :]):
+                    sy = sy-1
+                if np.any(mask[:,1]):
+                    sx = sx-1
+                mask = mask[1:-1, 1:-1]
+            all_grains.append(Polygon(np.vstack((sx, sy)).T))
+    labels = np.zeros(big_im.shape[:-1])
     mask_all = np.zeros(big_im.shape[:-1])
     for i in trange(len(all_grains)):
         mask = rasterize(
             shapes=[all_grains[i]],
             out_shape=big_im.shape[:-1],
             fill=0,
             out=None,
```

### Comparing `segmenteverygrain-0.0.2/segmenteverygrain.egg-info/PKG-INFO` & `segmenteverygrain-0.0.3/segmenteverygrain.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: segmenteverygrain
-Version: 0.0.2
+Version: 0.0.3
 Summary: A SAM-based model for segmenting grains in images of grains
 Home-page: https://github.com/zsylvester/segmenteverygrain
 Author: Zoltan Sylvester
 Author-email: Zoltan Sylvester <zoltan.sylvester@beg.utexas.edu>
 Project-URL: Homepage, https://github.com/zsylvester/segmenteverygrain
 Project-URL: Bug Tracker, https://github.com/zsylvester/segmenteverygrain/issues
 Keywords: sedimentology,geomorphology,grain size,segment anything model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Segment Every Grain
+# segmenteverygrain
 
-<img src="https://github.com/zsylvester/segmenteverygrain/blob/main/gravel_example_mask.jpg" width="600">
+<img src="https://github.com/zsylvester/segmenteverygrain/blob/main/gravel_example_mask.png" width="600">
 
 ## Description
 
 'segmenteverygrain' is a Python package that aims to detect grains (or grain-like objects) in images. The goal is to develop an ML model that does a reasonably good job at detecting most of the grains in a photo, so that it will be useful for determining grain size and grain shape, a common task in geomorphology and sedimentary geology. 'segmenteverygrain' relies on the [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything), developed by Meta, for getting high-quality outlines of the grains. However, SAM requires prompts for every object detected and, when used in 'everything' mode, it tends to be slow and results in many overlapping masks and non-grain (background) objects. To deal with these issues, 'segmenteverygrain' relies on a Unet-style, patch-based convolutional neural network to create a first-pass segmentation which is then used as a set of prompts for the SAM-based segmentation. Some of the grains will be missed with this approach, but the segmentations that are created tend to be of high quality. 
 
 'segmenteverygrain' also includes a set of functions that make it possible to clean up the segmentation results: delete and merge objects by clicking on them, and adding grains that were not segmented automatically. The QC-d masks can be saved and added to a dataset of grain images (see the 'images' folder). These images then can be used to improve the Unet model. Many of the images used in the dataset are from the [sedinet](https://github.com/DigitalGrainSize/SediNet) project.
```

### Comparing `segmenteverygrain-0.0.2/setup.py` & `segmenteverygrain-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """\
 
 """
 
 setuptools.setup(
     name="segmenteverygrain",
-    version="0.0.2",
+    version="0.0.3",
     author="Zoltan Sylvester",
     author_email="zoltan.sylvester@beg.utexas.edu",
     description="a SAM-based model for segmenting grains in images of grains",
     keywords = 'sedimentology, geomorphology, grain size, segment anything model',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zsylvester/segmenteverygrain",
```

