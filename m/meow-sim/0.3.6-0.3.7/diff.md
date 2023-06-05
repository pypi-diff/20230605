# Comparing `tmp/meow-sim-0.3.6.tar.gz` & `tmp/meow-sim-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.3.6.tar", last modified: Mon Jun  5 01:43:49 2023, max compression
+gzip compressed data, was "meow-sim-0.3.7.tar", last modified: Mon Jun  5 01:43:47 2023, max compression
```

## Comparing `meow-sim-0.3.6.tar` & `meow-sim-0.3.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:49.187391 meow-sim-0.3.6/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 01:43:45.000000 meow-sim-0.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 01:43:49.187391 meow-sim-0.3.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 01:43:45.000000 meow-sim-0.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:49.183391 meow-sim-0.3.6/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:49.183391 meow-sim-0.3.6/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8007 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:49.183391 meow-sim-0.3.6/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5317 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:49.183391 meow-sim-0.3.6/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4631 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10197 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10785 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3564 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    11526 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     5666 2023-06-05 01:43:45.000000 meow-sim-0.3.6/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:49.187391 meow-sim-0.3.6/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 01:43:49.000000 meow-sim-0.3.6/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 01:43:49.000000 meow-sim-0.3.6/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 01:43:49.000000 meow-sim-0.3.6/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 01:43:49.000000 meow-sim-0.3.6/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 01:43:49.000000 meow-sim-0.3.6/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 01:43:45.000000 meow-sim-0.3.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 01:43:49.187391 meow-sim-0.3.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:49.187391 meow-sim-0.3.6/tests/
--rw-r--r--   0 root         (0) root         (0)     4009 2023-06-05 01:43:45.000000 meow-sim-0.3.6/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-06-05 01:43:45.000000 meow-sim-0.3.6/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 01:43:45.000000 meow-sim-0.3.6/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:47.746773 meow-sim-0.3.7/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 01:43:43.000000 meow-sim-0.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 01:43:47.746773 meow-sim-0.3.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 01:43:43.000000 meow-sim-0.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:47.746773 meow-sim-0.3.7/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:47.746773 meow-sim-0.3.7/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:47.746773 meow-sim-0.3.7/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5317 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:47.746773 meow-sim-0.3.7/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10197 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10785 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    11970 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     5666 2023-06-05 01:43:43.000000 meow-sim-0.3.7/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:47.746773 meow-sim-0.3.7/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 01:43:47.000000 meow-sim-0.3.7/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 01:43:47.000000 meow-sim-0.3.7/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 01:43:47.000000 meow-sim-0.3.7/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 01:43:47.000000 meow-sim-0.3.7/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 01:43:47.000000 meow-sim-0.3.7/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 01:43:43.000000 meow-sim-0.3.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 01:43:47.746773 meow-sim-0.3.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:43:47.746773 meow-sim-0.3.7/tests/
+-rw-r--r--   0 root         (0) root         (0)     4009 2023-06-05 01:43:43.000000 meow-sim-0.3.7/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-06-05 01:43:43.000000 meow-sim-0.3.7/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 01:43:43.000000 meow-sim-0.3.7/tests/test_nbs.py
```

### Comparing `meow-sim-0.3.6/LICENSE` & `meow-sim-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/PKG-INFO` & `meow-sim-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.6
+Version: 0.3.7
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.6/README.md` & `meow-sim-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/__init__.py` & `meow-sim-0.3.7/meow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.3.6/meow/assets/silicon.csv` & `meow-sim-0.3.7/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/assets/silicon_oxide.csv` & `meow-sim-0.3.7/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/base_model.py` & `meow-sim-0.3.7/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/cache.py` & `meow-sim-0.3.7/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/cell.py` & `meow-sim-0.3.7/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/cross_section.py` & `meow-sim-0.3.7/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/eme/__init__.py` & `meow-sim-0.3.7/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/eme/common.py` & `meow-sim-0.3.7/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/eme/sax.py` & `meow-sim-0.3.7/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/environment.py` & `meow-sim-0.3.7/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/fde/lumerical.py` & `meow-sim-0.3.7/meow/fde/lumerical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ FDE Lumerical Backend """
 
 from typing import Optional
 
 import numpy as np
 from pydantic import validate_arguments
 from pydantic.types import PositiveInt
-from lumapi import LumApiError, MODE
 
 from ..cross_section import CrossSection
 from ..mode import Mode, normalize_energy, zero_phase
 
 _global = {"sim": None}
 
 
@@ -60,14 +59,16 @@
     """compute ``Modes` for a given ``FdeSpec` (Lumerical backend)
 
     Args:
         sim: the lumerical simulation object
         spec: The FDE simulation specification
         unit: Conversion factor between MEOW unit (probably um) and Lumerical unit (probably m).
     """
+    from lumapi import LumApiError, MODE  # fmt: skip
+
     sim = get_sim(sim=sim)
     _assert_default_mesh_setting(cs.cell.mesh.angle_phi != 0, "angle_phi")
     _assert_default_mesh_setting(cs.cell.mesh.angle_theta != 0, "angle_theta")
     _assert_default_mesh_setting(cs.cell.mesh.bend_radius < 1e10, "bend_radius")
 
     assert sim is not None
     create_lumerical_geometries(sim, cs.cell.structures, cs.env, unit)
```

### Comparing `meow-sim-0.3.6/meow/fde/tidy3d.py` & `meow-sim-0.3.7/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/gds_structures.py` & `meow-sim-0.3.7/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/geometries.py` & `meow-sim-0.3.7/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/integrate.py` & `meow-sim-0.3.7/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/materials.py` & `meow-sim-0.3.7/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/mesh.py` & `meow-sim-0.3.7/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/mode.py` & `meow-sim-0.3.7/meow/mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,21 +246,36 @@
 
 
 Modes = List[Mode]
 
 
 def zero_phase(mode: Mode) -> Mode:
     """normalize (zero out) the phase of a `Mode`"""
-    return mode * np.exp(1j * np.random.rand() * 2 * np.pi)
-
-
-def _centroid_idxs(arr2d: np.ndarray) -> tuple[int, int]:
-    centroid_x = np.average(np.arange(arr2d.shape[1]), weights=arr2d.sum(axis=0))
-    centroid_y = np.average(np.arange(arr2d.shape[0]), weights=arr2d.sum(axis=1))
-    return round(float(centroid_x)), round(float(centroid_y))
+    e = np.abs(energy_density(mode))
+    m, n = np.array(np.where(e == e.max()))[:, 0]
+    phase = np.exp(-1j * np.angle(np.array(mode.Hx))[m][n])
+    new_mode = Mode(
+        neff=mode.neff,
+        cs=mode.cs,
+        Ex=mode.Ex * phase,
+        Ey=mode.Ey * phase,
+        Ez=mode.Ez * phase,
+        Hx=mode.Hx * phase,
+        Hy=mode.Hy * phase,
+        Hz=mode.Hz * phase,
+    )
+    if _sum_around(np.real(new_mode.Hx), m, n) < 0:
+        new_mode = invert_mode(new_mode)
+    return new_mode
+
+
+# def _centroid_idxs(arr2d: np.ndarray) -> tuple[int, int]:
+#    centroid_x = np.average(np.arange(arr2d.shape[1]), weights=arr2d.sum(axis=0))
+#    centroid_y = np.average(np.arange(arr2d.shape[0]), weights=arr2d.sum(axis=1))
+#    return round(float(centroid_x)), round(float(centroid_y))
 
 
 def _sum_around(field, m, n, r=2):
     total = 0
     idxs = range(-r, r + 1)
     idx_tups = product(idxs, idxs)
     M, N = field.shape
```

### Comparing `meow-sim-0.3.6/meow/structures.py` & `meow-sim-0.3.7/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow/visualize.py` & `meow-sim-0.3.7/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.3.7/meow_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.6
+Version: 0.3.7
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.6/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.3.7/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/pyproject.toml` & `meow-sim-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.3.6/tests/test_deserialization.py` & `meow-sim-0.3.7/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/tests/test_mode_operators.py` & `meow-sim-0.3.7/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.6/tests/test_nbs.py` & `meow-sim-0.3.7/tests/test_nbs.py`

 * *Files identical despite different names*

