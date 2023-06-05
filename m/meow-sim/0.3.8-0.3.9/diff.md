# Comparing `tmp/meow-sim-0.3.8.tar.gz` & `tmp/meow-sim-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.3.8.tar", last modified: Mon Jun  5 01:53:52 2023, max compression
+gzip compressed data, was "meow-sim-0.3.9.tar", last modified: Mon Jun  5 05:31:47 2023, max compression
```

## Comparing `meow-sim-0.3.8.tar` & `meow-sim-0.3.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.454864 meow-sim-0.3.8/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 01:53:48.000000 meow-sim-0.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 01:53:52.454864 meow-sim-0.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 01:53:48.000000 meow-sim-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.450864 meow-sim-0.3.8/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.450864 meow-sim-0.3.8/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8007 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.450864 meow-sim-0.3.8/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5317 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.450864 meow-sim-0.3.8/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10178 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10785 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3564 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12030 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     5682 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.454864 meow-sim-0.3.8/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 01:53:48.000000 meow-sim-0.3.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 01:53:52.454864 meow-sim-0.3.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.454864 meow-sim-0.3.8/tests/
--rw-r--r--   0 root         (0) root         (0)     4009 2023-06-05 01:53:48.000000 meow-sim-0.3.8/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-06-05 01:53:48.000000 meow-sim-0.3.8/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 01:53:48.000000 meow-sim-0.3.8/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.170044 meow-sim-0.3.9/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 05:31:43.000000 meow-sim-0.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 05:31:47.170044 meow-sim-0.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 05:31:43.000000 meow-sim-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.166044 meow-sim-0.3.9/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.166044 meow-sim-0.3.9/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.166044 meow-sim-0.3.9/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5317 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.170044 meow-sim-0.3.9/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10178 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10785 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.170044 meow-sim-0.3.9/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 05:31:43.000000 meow-sim-0.3.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 05:31:47.170044 meow-sim-0.3.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.170044 meow-sim-0.3.9/tests/
+-rw-r--r--   0 root         (0) root         (0)     4009 2023-06-05 05:31:43.000000 meow-sim-0.3.9/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-06-05 05:31:43.000000 meow-sim-0.3.9/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 05:31:43.000000 meow-sim-0.3.9/tests/test_nbs.py
```

### Comparing `meow-sim-0.3.8/LICENSE` & `meow-sim-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/PKG-INFO` & `meow-sim-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.8
+Version: 0.3.9
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.8/README.md` & `meow-sim-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/__init__.py` & `meow-sim-0.3.9/meow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.3.8/meow/assets/silicon.csv` & `meow-sim-0.3.9/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/assets/silicon_oxide.csv` & `meow-sim-0.3.9/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/base_model.py` & `meow-sim-0.3.9/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/cache.py` & `meow-sim-0.3.9/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/cell.py` & `meow-sim-0.3.9/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/cross_section.py` & `meow-sim-0.3.9/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/eme/__init__.py` & `meow-sim-0.3.9/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/eme/common.py` & `meow-sim-0.3.9/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/eme/sax.py` & `meow-sim-0.3.9/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/environment.py` & `meow-sim-0.3.9/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/fde/lumerical.py` & `meow-sim-0.3.9/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/fde/tidy3d.py` & `meow-sim-0.3.9/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/gds_structures.py` & `meow-sim-0.3.9/meow/gds_structures.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,22 @@
     )
     mesh_order: int = Field(
         default=5.0, description="the mesh order of the resulting `Structure`"
     )
 
     def __call__(self, poly) -> Structure:
         if self.buffer > 0:
-            poly = np.asarray(sg.Polygon(poly).buffer(self.buffer).boundary.coords)
+            try:
+                poly = np.asarray(sg.Polygon(poly).buffer(self.buffer).boundary.coords)
+            except NotImplementedError:
+                import gdspy
+
+                polygonset = gdspy.offset(gdspy.Polygon(poly), 0.25)
+                assert polygonset is not None
+                poly = polygonset.polygons[0]
         return Structure(
             material=self.material,
             geometry=Prism(
                 poly=poly,
                 h_min=self.h_min,
                 h_max=self.h_max,
                 axis="y",
```

### Comparing `meow-sim-0.3.8/meow/geometries.py` & `meow-sim-0.3.9/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/integrate.py` & `meow-sim-0.3.9/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/materials.py` & `meow-sim-0.3.9/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/mesh.py` & `meow-sim-0.3.9/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/mode.py` & `meow-sim-0.3.9/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/structures.py` & `meow-sim-0.3.9/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow/visualize.py` & `meow-sim-0.3.9/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.3.9/meow_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.8
+Version: 0.3.9
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.8/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.3.9/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/pyproject.toml` & `meow-sim-0.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.3.8"
+version = "0.3.9"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.3.8/tests/test_deserialization.py` & `meow-sim-0.3.9/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/tests/test_mode_operators.py` & `meow-sim-0.3.9/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.8/tests/test_nbs.py` & `meow-sim-0.3.9/tests/test_nbs.py`

 * *Files identical despite different names*

