# Comparing `tmp/meow-sim-0.4.0.tar.gz` & `tmp/meow-sim-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.4.0.tar", last modified: Mon Jun  5 20:36:19 2023, max compression
+gzip compressed data, was "meow-sim-0.4.1.tar", last modified: Mon Jun  5 20:45:35 2023, max compression
```

## Comparing `meow-sim-0.4.0.tar` & `meow-sim-0.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 20:36:15.000000 meow-sim-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 20:36:19.863043 meow-sim-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 20:36:15.000000 meow-sim-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.859043 meow-sim-0.4.0/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5354 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12184 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     5962 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 20:36:15.000000 meow-sim-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 20:36:19.863043 meow-sim-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-05 20:36:15.000000 meow-sim-0.4.0/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-05 20:36:15.000000 meow-sim-0.4.0/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 20:36:15.000000 meow-sim-0.4.0/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 20:45:31.000000 meow-sim-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 20:45:35.636978 meow-sim-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 20:45:31.000000 meow-sim-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12184 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     5962 2023-06-05 20:45:31.000000 meow-sim-0.4.1/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 20:45:35.000000 meow-sim-0.4.1/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 20:45:31.000000 meow-sim-0.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 20:45:35.636978 meow-sim-0.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:45:35.636978 meow-sim-0.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-05 20:45:31.000000 meow-sim-0.4.1/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-05 20:45:31.000000 meow-sim-0.4.1/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 20:45:31.000000 meow-sim-0.4.1/tests/test_nbs.py
```

### Comparing `meow-sim-0.4.0/LICENSE` & `meow-sim-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/PKG-INFO` & `meow-sim-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.4.0
+Version: 0.4.1
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.4.0/README.md` & `meow-sim-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/__init__.py` & `meow-sim-0.4.1/meow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.4.0/meow/assets/silicon.csv` & `meow-sim-0.4.1/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/assets/silicon_oxide.csv` & `meow-sim-0.4.1/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/base_model.py` & `meow-sim-0.4.1/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/cache.py` & `meow-sim-0.4.1/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/cell.py` & `meow-sim-0.4.1/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/cross_section.py` & `meow-sim-0.4.1/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/eme/__init__.py` & `meow-sim-0.4.1/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/eme/common.py` & `meow-sim-0.4.1/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/eme/sax.py` & `meow-sim-0.4.1/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/environment.py` & `meow-sim-0.4.1/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/fde/lumerical.py` & `meow-sim-0.4.1/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/fde/tidy3d.py` & `meow-sim-0.4.1/meow/fde/tidy3d.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 @validate_arguments
 def compute_modes_tidy3d(
     cs: CrossSection,
     num_modes: PositiveInt = 10,
     target_neff: PositiveFloat | None = None,
-    precision: Literal["single", "double"] = "single",
+    precision: Literal["single", "double"] = "double",
 ) -> Modes:
     """compute ``Modes`` for a given ``FdeSpec`` (Tidy3D backend)
 
     Args:
         cs: The ``CrossSection`` to calculate the modes for
         num_modes: Number of modes returned by mode solver.
         target_neff: Guess for initial effective index of the mode.
```

### Comparing `meow-sim-0.4.0/meow/gds_structures.py` & `meow-sim-0.4.1/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/geometries.py` & `meow-sim-0.4.1/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/integrate.py` & `meow-sim-0.4.1/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/materials.py` & `meow-sim-0.4.1/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/mesh.py` & `meow-sim-0.4.1/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/mode.py` & `meow-sim-0.4.1/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/structures.py` & `meow-sim-0.4.1/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow/visualize.py` & `meow-sim-0.4.1/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.4.1/meow_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.4.0
+Version: 0.4.1
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.4.0/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.4.1/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/pyproject.toml` & `meow-sim-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.4.0/tests/test_deserialization.py` & `meow-sim-0.4.1/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/tests/test_mode_operators.py` & `meow-sim-0.4.1/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.0/tests/test_nbs.py` & `meow-sim-0.4.1/tests/test_nbs.py`

 * *Files identical despite different names*

