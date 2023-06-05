# Comparing `tmp/napari-svg-0.1.7.tar.gz` & `tmp/napari-svg-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-svg-0.1.7.tar", last modified: Thu May 25 21:21:54 2023, max compression
+gzip compressed data, was "napari-svg-0.1.8.tar", last modified: Mon Jun  5 13:01:17 2023, max compression
```

## Comparing `napari-svg-0.1.7.tar` & `napari-svg-0.1.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.695243 napari-svg-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-25 21:21:43.000000 napari-svg-0.1.7/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.683243 napari-svg-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.687243 napari-svg-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-25 21:21:43.000000 napari-svg-0.1.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-25 21:21:43.000000 napari-svg-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-25 21:21:43.000000 napari-svg-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 21:21:43.000000 napari-svg-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-25 21:21:54.695243 napari-svg-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-25 21:21:43.000000 napari-svg-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.687243 napari-svg-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 21:21:43.000000 napari-svg-0.1.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-25 21:21:43.000000 napari-svg-0.1.7/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.691243 napari-svg-0.1.7/napari_svg/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/_shape_to_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.691243 napari-svg-0.1.7/napari_svg/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/_tests/test_get_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/_tests/test_write_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/hook_implementations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/layer_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-25 21:21:43.000000 napari-svg-0.1.7/napari_svg/xml_to_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.691243 napari-svg-0.1.7/napari_svg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 21:21:54.000000 napari-svg-0.1.7/napari_svg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:21:54.695243 napari-svg-0.1.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 21:21:43.000000 napari-svg-0.1.7/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 21:21:43.000000 napari-svg-0.1.7/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 21:21:43.000000 napari-svg-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 21:21:54.695243 napari-svg-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-25 21:21:43.000000 napari-svg-0.1.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-25 21:21:43.000000 napari-svg-0.1.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.290155 napari-svg-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-05 13:01:07.000000 napari-svg-0.1.8/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.286155 napari-svg-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.286155 napari-svg-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-05 13:01:07.000000 napari-svg-0.1.8/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 13:01:07.000000 napari-svg-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-05 13:01:07.000000 napari-svg-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-05 13:01:07.000000 napari-svg-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-05 13:01:17.290155 napari-svg-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-05 13:01:07.000000 napari-svg-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.286155 napari-svg-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 13:01:07.000000 napari-svg-0.1.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 13:01:07.000000 napari-svg-0.1.8/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.286155 napari-svg-0.1.8/napari_svg/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/_shape_to_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.290155 napari-svg-0.1.8/napari_svg/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/_tests/test_get_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/_tests/test_write_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/hook_implementations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/layer_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/xml_to_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.290155 napari-svg-0.1.8/napari_svg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.290155 napari-svg-0.1.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 13:01:07.000000 napari-svg-0.1.8/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:01:07.000000 napari-svg-0.1.8/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 13:01:07.000000 napari-svg-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-05 13:01:17.290155 napari-svg-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-05 13:01:07.000000 napari-svg-0.1.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-05 13:01:07.000000 napari-svg-0.1.8/tox.ini
```

### Comparing `napari-svg-0.1.7/.cruft.json` & `napari-svg-0.1.8/.cruft.json`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/.github/workflows/test_and_deploy.yml` & `napari-svg-0.1.8/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/.gitignore` & `napari-svg-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/LICENSE` & `napari-svg-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/PKG-INFO` & `napari-svg-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-svg
-Version: 0.1.7
+Version: 0.1.8
 Summary: A plugin for reading and writing svg files with napari
 Home-page: https://github.com/napari/napari-svg
 Download-URL: https://github.com/napari/napari-svg
 Author: Nicholas Sofroniew
 Author-email: sofroniewn@gmail.com
 License: BSD-3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `napari-svg-0.1.7/README.md` & `napari-svg-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/napari_svg/_shape_to_xml.py` & `napari-svg-0.1.8/napari_svg/_shape_to_xml.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/napari_svg/_tests/test_get_writer.py` & `napari-svg-0.1.8/napari_svg/_tests/test_get_writer.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/napari_svg/_tests/test_write_layer.py` & `napari-svg-0.1.8/napari_svg/_tests/test_write_layer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import numpy as np
 import pytest
 from napari.layers import Image, Points, Labels, Shapes, Vectors
+from napari.utils.colormaps.colormap_utils import ensure_colormap
 from napari_svg import (
     napari_write_image,
     napari_write_labels,
     napari_write_points,
     napari_write_shapes,
     napari_write_vectors,
 )
 
 
 @pytest.fixture(params=['image', 'labels', 'points', 'shapes', 'shapes-rectangles', 'vectors'])
 def layer_writer_and_data(request):
     meta_required = False
-    
     if request.param == 'image':
         data = np.random.rand(20, 20)
         layer = Image(data)
         writer = napari_write_image
     elif request.param == 'labels':
         data = np.random.randint(10, size=(20, 20))
         layer = Labels(data)
@@ -117,7 +117,25 @@
 
     # Check no data is writen
     return_path = writer(path, layer_data[0], layer_data[1])
     assert return_path is None
 
     # Check file still does not exist
     assert not os.path.isfile(path)
+
+
+@pytest.mark.parametrize('colormap', ('viridis', ensure_colormap('viridis').dict()))
+def test_write_image_colormaps(tmpdir, layer_writer_and_data, colormap):
+    writer, layer_data, _ = layer_writer_and_data
+    layer_data[1]['colormap'] = colormap
+
+    path = os.path.join(tmpdir, 'layer_file.svg')
+
+    # Check file does not exist
+    assert not os.path.isfile(path)
+
+    # Write data
+    return_path = writer(path, layer_data[0], layer_data[1])
+    assert return_path == path
+
+    # Check file now exists
+    assert os.path.isfile(path)
```

### Comparing `napari-svg-0.1.7/napari_svg/hook_implementations.py` & `napari-svg-0.1.8/napari_svg/hook_implementations.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/napari_svg/layer_to_xml.py` & `napari-svg-0.1.8/napari_svg/layer_to_xml.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from xml.etree.ElementTree import Element
 from base64 import b64encode
 import numpy as np
 from copy import copy
 from imageio import imwrite
-from vispy.color import get_colormap
+from napari.utils.colormaps.colormap_utils import ensure_colormap
+
+
 from ._shape_to_xml import (
     ellipse_to_xml,
     line_to_xml,
     path_to_xml,
     polygon_to_xml,
     rectangle_to_xml,
 )
@@ -60,36 +62,30 @@
         rgb = False
 
     if 'contrast_limits' in meta:
         contrast_limits = meta['contrast_limits']
     else:
         contrast_limits = [0, 1]
 
-    if 'colormap' in meta:
-        colormap_name = meta['colormap']
-
-        # convert 'gray' colormap name to 'grays' for vispy compatibility
-        # see: https://github.com/napari/napari-svg/pull/12
-        if colormap_name == 'gray':
-            colormap_name = 'grays'
-    else:
-        colormap_name = 'grays'
+    colormap = meta.get('colormap', 'gray')
 
     if 'opacity' in meta:
         opacity = meta['opacity']
     else:
         opacity = 1
 
     # Check if data is multiscale, and if so take only last layer
     if multiscale:
         data = data[-1]
 
+    data = np.squeeze(data)
+
     # Check if more than 2 dimensional and if so error.
     if data.ndim - int(rgb) > 2:
-        raise ValueError('Image must be 2 dimensional to save as svg')
+        raise ValueError(f'Image must be 2 dimensional, not {data.ndim - int(rgb)} to save as svg')
     else:
         image = data
 
     # Find extrema of data
     extrema = np.array([[0, 0], [image.shape[0], image.shape[1]]])
 
     if rgb:
@@ -100,35 +96,32 @@
             image, contrast_limits[0], contrast_limits[1]
         )
         image = image - contrast_limits[0]
         color_range = contrast_limits[1] - contrast_limits[0]
         if color_range != 0:
             image = image / color_range
 
-        # get colormap
-        # TODO: Currently we only support vispy colormaps, need to
-        # add support for all napari colormaps, matters for Labels too.
-        cmap = get_colormap(colormap_name)
-            
-        # apply colormap to data
-        mapped_image = cmap[image.ravel()]
-        mapped_image = mapped_image.RGBA.reshape(image.shape + (4,))
+        cmap = ensure_colormap(colormap)
+
+        # to keep backward compatibility with napari <0.4.18
+        # because of a bug in `vmap.map`, we need to ravel, map, then reshape
+        mapped_image = (cmap.map(image.ravel()).reshape(image.shape + (4,)) * 255).astype(np.uint8)
 
     image_str = imwrite('<bytes>', mapped_image, format='png')
     image_str = "data:image/png;base64," + str(b64encode(image_str))[2:-1]
     props = {'xlink:href': image_str}
 
     width = str(image.shape[1])
     height = str(image.shape[0])
 
     xml = Element(
         'image', width=width, height=height, opacity=str(opacity), **props
     )
     xml_list = [xml]
-    
+
     return xml_list, extrema
 
 
 def points_to_xml(data, meta):
     """Generates a xml data for points.
 
     Only two dimensional points data is supported. Z ordering of the points
@@ -151,14 +144,15 @@
         Extrema of data, specified as a minumum then maximum of the (x, y)
         coordinates.
     """
     # Extract metadata parameters
     if 'size' in meta:
         size = meta['size']
         if size.ndim == 2:
+            # backward compatibility for napari<v0.4.18 with anisotropic sizes
             size = np.mean(size, axis=1)
     else:
         size = np.ones(data.shape[0])
 
     if 'face_color' in meta:
         face_color = meta['face_color']
     else:
```

### Comparing `napari-svg-0.1.7/napari_svg/xml_to_svg.py` & `napari-svg-0.1.8/napari_svg/xml_to_svg.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/napari_svg.egg-info/PKG-INFO` & `napari-svg-0.1.8/napari_svg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-svg
-Version: 0.1.7
+Version: 0.1.8
 Summary: A plugin for reading and writing svg files with napari
 Home-page: https://github.com/napari/napari-svg
 Download-URL: https://github.com/napari/napari-svg
 Author: Nicholas Sofroniew
 Author-email: sofroniewn@gmail.com
 License: BSD-3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `napari-svg-0.1.7/napari_svg.egg-info/SOURCES.txt` & `napari-svg-0.1.8/napari_svg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.7/setup.cfg` & `napari-svg-0.1.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 zip_safe = False
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	imageio>=2.5.0
 	numpy>=1.16.0
 	napari-plugin-engine>=0.1.4
-	vispy >= 0.6.4
+	vispy>=0.6.4
 
 [options.extras_require]
 testing = 
 	pytest
 	pytest-cov
 	napari >= 0.4
 	pyqt5
```

### Comparing `napari-svg-0.1.7/tox.ini` & `napari-svg-0.1.8/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # For more information about tox, see https://tox.readthedocs.io/en/latest/
 [tox]
-envlist = py{37,38,39}-{linux,macos,windows}
+envlist = py{37,38,39,310}-{linux,macos,windows}
 
 [gh-actions]
 python =
     3.7: py37
     3.8: py38
     3.9: py39
+    3.10: py310
     
 [gh-actions:env]
 PLATFORM =
     ubuntu-latest: linux
     macos-latest: macos
     windows-latest: windows
```

