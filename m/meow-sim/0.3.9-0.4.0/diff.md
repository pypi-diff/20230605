# Comparing `tmp/meow-sim-0.3.9.tar.gz` & `tmp/meow-sim-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.3.9.tar", last modified: Mon Jun  5 05:31:47 2023, max compression
+gzip compressed data, was "meow-sim-0.4.0.tar", last modified: Mon Jun  5 20:36:19 2023, max compression
```

## Comparing `meow-sim-0.3.9.tar` & `meow-sim-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.170044 meow-sim-0.3.9/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 05:31:43.000000 meow-sim-0.3.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 05:31:47.170044 meow-sim-0.3.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 05:31:43.000000 meow-sim-0.3.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.166044 meow-sim-0.3.9/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.166044 meow-sim-0.3.9/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8007 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.166044 meow-sim-0.3.9/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5317 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.170044 meow-sim-0.3.9/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10178 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10785 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3564 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12030 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     5682 2023-06-05 05:31:43.000000 meow-sim-0.3.9/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.170044 meow-sim-0.3.9/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 05:31:47.000000 meow-sim-0.3.9/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 05:31:43.000000 meow-sim-0.3.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 05:31:47.170044 meow-sim-0.3.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:31:47.170044 meow-sim-0.3.9/tests/
--rw-r--r--   0 root         (0) root         (0)     4009 2023-06-05 05:31:43.000000 meow-sim-0.3.9/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-06-05 05:31:43.000000 meow-sim-0.3.9/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 05:31:43.000000 meow-sim-0.3.9/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 20:36:15.000000 meow-sim-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 20:36:19.863043 meow-sim-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 20:36:15.000000 meow-sim-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.859043 meow-sim-0.4.0/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12184 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     5962 2023-06-05 20:36:15.000000 meow-sim-0.4.0/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 20:36:19.000000 meow-sim-0.4.0/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 20:36:15.000000 meow-sim-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 20:36:19.863043 meow-sim-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:36:19.863043 meow-sim-0.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-05 20:36:15.000000 meow-sim-0.4.0/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-05 20:36:15.000000 meow-sim-0.4.0/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 20:36:15.000000 meow-sim-0.4.0/tests/test_nbs.py
```

### Comparing `meow-sim-0.3.9/LICENSE` & `meow-sim-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.9/PKG-INFO` & `meow-sim-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.9
+Version: 0.4.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.9/README.md` & `meow-sim-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.9/meow/__init__.py` & `meow-sim-0.4.0/meow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.3.9"
+__version__ = "0.4.0"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.3.9/meow/assets/silicon.csv` & `meow-sim-0.4.0/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.9/meow/assets/silicon_oxide.csv` & `meow-sim-0.4.0/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.9/meow/base_model.py` & `meow-sim-0.4.0/meow/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     except Exception:
         shape = Any
 
     return shape, dtype
 
 
 def _try_parse_shape_int(value):
-    from typing import _LiteralGenericAlias  # type: ignore
+    from typing import _LiteralGenericAlias  # fmt: skip # type: ignore
 
     if isinstance(value, _LiteralGenericAlias):
         (value,) = value.__args__
     try:
         return int(value)
     except Exception:
         return 1
```

### Comparing `meow-sim-0.3.9/meow/cache.py` & `meow-sim-0.4.0/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.9/meow/cell.py` & `meow-sim-0.4.0/meow/cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         return 0.5 * (self.z_min + self.z_max)
 
     @property
     def length(self):
         return np.abs(self.z_max - self.z_min)
 
     def _visualize(self, c="z", axs=None):
-        import matplotlib.pyplot as plt
-        from matplotlib.colors import ListedColormap, to_rgba
+        import matplotlib.pyplot as plt  # fmt: skip
+        from matplotlib.colors import ListedColormap, to_rgba  # fmt: skip
 
         colors = [(0, 0, 0, 0)] + [
             to_rgba(m.meta.get("color", (0, 0, 0, 0))) for m in self.materials
         ]
         cmap = ListedColormap(colors=colors)  # type: ignore
         if axs is None:
             _, axs = plt.subplots(1, len(c), figsize=(3 * len(c), 3))
```

### Comparing `meow-sim-0.3.9/meow/cross_section.py` & `meow-sim-0.4.0/meow/cross_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ A CrossSection """
+
 from typing import Any, Dict
 
 import numpy as np
 from pydantic import Field
 
 from .base_model import BaseModel
 from .cell import Cell
@@ -59,15 +60,15 @@
         return self.cell.mesh
 
     @property
     def structures(self):
         return self.cell.structures
 
     def _visualize(self, c="z", axs=None):
-        import matplotlib.pyplot as plt
+        import matplotlib.pyplot as plt  # fmt: skip
 
         if axs is None:
             _, axs = plt.subplots(1, len(c), figsize=(3 * len(c), 3))
         c_list = list(c)
         if any(c not in "xyz" for c in c_list):
             raise ValueError(f"Invalid component. Got: {c}. Should be 'x', 'y' or 'z'.")
         axs = np.array(axs, dtype=object).ravel()
```

### Comparing `meow-sim-0.3.9/meow/eme/__init__.py` & `meow-sim-0.4.0/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.9/meow/eme/common.py` & `meow-sim-0.4.0/meow/eme/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """ SAX backend for EME (default backend) """
+
 from typing import Any, Dict, List
 
 import numpy as np
 
-from ..mode import Mode, inner_product as inner_product_normal, inner_product_conj
+from ..mode import Mode
+from ..mode import inner_product as inner_product_normal
+from ..mode import inner_product_conj
 
 DEFAULT_CONJUGATE_TRANSPOSE = True
 DEFAULT_ENFORCE_RECIPROCITY = False
 DEFAULT_ENFORCE_LOSSY_UNITARITY = False
 
 
 def compute_interface_s_matrix(
```

### Comparing `meow-sim-0.3.9/meow/eme/sax.py` & `meow-sim-0.4.0/meow/eme/sax.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """ SAX backend for EME (default backend) """
-from functools import partial
+
 from typing import List
 
 import numpy as np
 import sax
 from sax.backends import circuit_backends
-from sax.circuit import _make_singlemode_or_multimode
-from sax.netlist import Netlist
 from sax.utils import get_ports
 
 from ..base_model import _array
 from ..mode import Mode
-from .common import compute_interface_s_matrices, compute_propagation_s_matrices
 from .common import (
-    select_ports as select_ports,
     DEFAULT_CONJUGATE_TRANSPOSE,
-    DEFAULT_ENFORCE_RECIPROCITY,
     DEFAULT_ENFORCE_LOSSY_UNITARITY,
+    DEFAULT_ENFORCE_RECIPROCITY,
+    compute_interface_s_matrices,
+    compute_propagation_s_matrices,
 )
 
 try:
     import klujax
+
+
 except ImportError:
     klujax = None
 
 
 def _get_netlist(propagations, interfaces):
     """get the netlist of a stack of `Modes`"""
```

### Comparing `meow-sim-0.3.9/meow/environment.py` & `meow-sim-0.4.0/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.9/meow/fde/lumerical.py` & `meow-sim-0.4.0/meow/fde/lumerical.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,64 @@
 """ FDE Lumerical Backend """
 
-from typing import Optional
-
 import numpy as np
 from pydantic.types import PositiveInt
 
 from ..cross_section import CrossSection
+from ..environment import Environment
 from ..mode import Mode, normalize_energy, zero_phase
+from ..structures import Structure
 
 _global = {"sim": None}
 
 
-def _assert_default_mesh_setting(condition, param_name):
-    if condition:
-        raise NotImplementedError(
-            f"Setting mesh.{param_name} is currently not supported in the Lumerical Backend. "
-            "Please open an issue of submit a PR on GitHub to fix this: ",
-            "https://github.com/flaport/meow",
-        )
-
-
-def set_sim(
-    sim: "lumapi.MODE",  # type: ignore
-):
-    _global["sim"] = sim
-
-
 def get_sim(**kwargs):
     sim = kwargs.get("sim", None)
     if sim is not None:
         return sim
     sim = _global["sim"]
     if sim is None:
         raise ValueError(
             "Could not start Lumerical simulation. "
             "Please either pass the `lumapi.MODE` simulation object as an argument to `compute_modes_lumerical` or "
             "use `set_sim(sim)` to globally set the lumapi.MODE simulation object."
         )
     return sim
 
 
-def create_lumerical_geometries(sim, structures, env, unit):
+def create_lumerical_geometries(
+    sim, structures: list[Structure], env: Environment, unit: float
+):
     sim = get_sim(sim=sim)
     sim.switchtolayout()
     sim.deleteall()
     for s in structures:
         s._lumadd(sim, env, unit, "yzx")
 
 
 # @validate_arguments
 def compute_modes_lumerical(
     cs: CrossSection,
     num_modes: PositiveInt = 10,
-    sim: Optional["lumapi.MODE"] = None,  # type: ignore
+    sim=None,
     unit: float = 1e-6,
 ):
     """compute ``Modes` for a given ``FdeSpec` (Lumerical backend)
 
     Args:
         sim: the lumerical simulation object
         spec: The FDE simulation specification
         unit: Conversion factor between MEOW unit (probably um) and Lumerical unit (probably m).
     """
-    from lumapi import LumApiError, MODE  # fmt: skip # type: ignore
+    from lumapi import LumApiError  # fmt: skip # type: ignore
 
     sim = get_sim(sim=sim)
-    _assert_default_mesh_setting(cs.cell.mesh.angle_phi != 0, "angle_phi")
-    _assert_default_mesh_setting(cs.cell.mesh.angle_theta != 0, "angle_theta")
-    _assert_default_mesh_setting(cs.cell.mesh.bend_radius < 1e10, "bend_radius")
+    _assert_default_mesh_setting(cs.cell.mesh.angle_phi == 0, "angle_phi")
+    _assert_default_mesh_setting(cs.cell.mesh.angle_theta == 0, "angle_theta")
+    _assert_default_mesh_setting(cs.cell.mesh.bend_radius is None, "bend_radius")
 
     assert sim is not None
     create_lumerical_geometries(sim, cs.cell.structures, cs.env, unit)
     sim.select("FDE")
     sim.delete()
     pml_settings = {}
     num_pml_y, num_pml_z = 0, 0
@@ -131,7 +118,20 @@
         except LumApiError:
             break
         mode = normalize_energy(mode)
         mode = zero_phase(mode)
         modes.append(mode)
 
     return sorted(modes, key=lambda m: np.real(m.neff), reverse=True)
+
+
+def _assert_default_mesh_setting(condition, param_name):
+    if not condition:
+        raise NotImplementedError(
+            f"Setting mesh.{param_name} is currently not supported in the Lumerical Backend. "
+            "Please open an issue of submit a PR on GitHub to fix this: ",
+            "https://github.com/flaport/meow",
+        )
+
+
+def set_sim(sim):
+    _global["sim"] = sim
```

### Comparing `meow-sim-0.3.9/meow/fde/tidy3d.py` & `meow-sim-0.4.0/meow/fde/tidy3d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 """ FDE Tidy3d backend (default backend for MEOW) """
 
 from types import SimpleNamespace
-from typing import Optional
+from typing import Literal
 
 import numpy as np
+import tidy3d
+from packaging import version
 from pydantic import validate_arguments
 from pydantic.types import PositiveFloat, PositiveInt
 from scipy.constants import c
 from tidy3d.plugins.mode.solver import compute_modes as _compute_modes
-import tidy3d
+
 from ..cross_section import CrossSection
 from ..mode import Mode, Modes, normalize_energy, zero_phase
 
 
-from packaging import version
-
-
 @validate_arguments
 def compute_modes_tidy3d(
     cs: CrossSection,
     num_modes: PositiveInt = 10,
-    target_neff: Optional[PositiveFloat] = None,
+    target_neff: PositiveFloat | None = None,
+    precision: Literal["single", "double"] = "single",
 ) -> Modes:
     """compute ``Modes`` for a given ``FdeSpec`` (Tidy3D backend)
 
     Args:
         cs: The ``CrossSection`` to calculate the modes for
         num_modes: Number of modes returned by mode solver.
         target_neff: Guess for initial effective index of the mode.
     """
 
     if num_modes < 1:
         raise ValueError("You need to request at least 1 mode.")
 
-    bend_radius = None if cs.cell.mesh.bend_radius > 1e10 else cs.cell.mesh.bend_radius
-    bend_axis = None if bend_radius is None else cs.cell.mesh.bend_axis
     od = np.zeros_like(cs.nx)  # off diagonal entry
     new_tidy3d = version.parse(tidy3d.__version__) >= version.parse("2.2.0")
     ((Ex, Ey, Ez), (Hx, Hy, Hz)), neffs = (
         x.squeeze()
         for x in _compute_modes(
             eps_cross=[cs.nx**2, od, od, od, cs.ny**2, od, od, od, cs.nz**2]
             if new_tidy3d
             else [cs.nx**2, cs.ny**2, cs.nz**2],
             coords=[cs.mesh.x, cs.mesh.y],
             freq=c / (cs.env.wl * 1e-6),
             mode_spec=SimpleNamespace(
                 num_modes=num_modes,
                 angle_theta=cs.cell.mesh.angle_theta,
                 angle_phi=cs.cell.mesh.angle_phi,
-                bend_radius=bend_radius,
-                bend_axis=bend_axis,
-                target_neff=target_neff or cs.nx.max(),
+                bend_radius=cs.cell.mesh.bend_radius,
+                bend_axis=cs.cell.mesh.bend_axis,
+                target_neff=target_neff,
                 num_pml=cs.cell.mesh.num_pml,
                 sort_by="largest_neff",
                 filter_pol=None,
-                precision="double",
+                precision=precision,
             ),
         )
     )
 
     if num_modes == 1:
         modes = [
             Mode(
```

### Comparing `meow-sim-0.3.9/meow/gds_structures.py` & `meow-sim-0.4.0/meow/gds_structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """ GDS Extrusions """
-# TODO: Maybe it makes more sense to use native GDSFactory tooling for this
 
 from typing import Dict, List, Tuple
 
 import numpy as np
 import shapely.geometry as sg
 from pydantic import Field
 
 from .base_model import BaseModel
 from .geometries import Prism
 from .materials import Material
 from .structures import Structure
 
+# TODO: Maybe it makes more sense to use native GDSFactory tooling for this
+
 
 class GdsExtrusionRule(BaseModel):
     """a `GdsExtrusionRule` describes a single extrusion rule.
     Multiple of such rules can later be associated with a gds layer tuple."""
 
     material: Material = Field(description="the material of the extrusion")
     h_min: float = Field(description="the extrusion starting height")
@@ -29,15 +30,15 @@
     )
 
     def __call__(self, poly) -> Structure:
         if self.buffer > 0:
             try:
                 poly = np.asarray(sg.Polygon(poly).buffer(self.buffer).boundary.coords)
             except NotImplementedError:
-                import gdspy
+                import gdspy  # fmt: skip
 
                 polygonset = gdspy.offset(gdspy.Polygon(poly), 0.25)
                 assert polygonset is not None
                 poly = polygonset.polygons[0]
         return Structure(
             material=self.material,
             geometry=Prism(
```

### Comparing `meow-sim-0.3.9/meow/geometries.py` & `meow-sim-0.4.0/meow/geometries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Geometries """
 
+import warnings
 from secrets import token_hex
 from typing import Dict, List, Literal, Tuple, Union, cast
 
 import numpy as np
 import shapely.geometry as sg
 from pydantic import Field, validator
 
@@ -30,16 +31,16 @@
         if value not in GEOMETRIES:
             raise ValueError(
                 f"Invalid Geometry type. Got: {value!r}. Valid types: {GEOMETRIES}."
             )
         return value
 
     def _visualize(self, scale=None):
-        from trimesh.scene import Scene
-        from trimesh.transformations import rotation_matrix
+        from trimesh.scene import Scene  # fmt: skip
+        from trimesh.transformations import rotation_matrix  # fmt: skip
 
         scene = Scene()
         scene.add_geometry(self._trimesh(scale=scale))
         scene.apply_transform(rotation_matrix(-np.pi / 6, (0, 1, 0)))
         return scene.show()
 
     def _mask2d_single(self, X, Y, z):
@@ -99,16 +100,16 @@
             material=material_name,
             override_mesh_order_from_material_database=True,
             mesh_order=mesh_order,
             **kwargs,
         )
 
     def _trimesh(self, color=None, scale=None):
-        from trimesh import Trimesh
-        from trimesh.creation import extrude_polygon
+        from trimesh import Trimesh  # fmt: skip
+        from trimesh.creation import extrude_polygon  # fmt: skip
 
         sx, sy, sz = scale or (1, 1, 1)
         poly = sg.Polygon(
             [
                 (self.x_min * sx, self.y_min * sy),
                 (self.x_min * sx, self.y_max * sy),
                 (self.x_max * sx, self.y_max * sy),
@@ -146,15 +147,19 @@
     def _mask2d_single(self, X, Y, z):
         poly = sg.Polygon(self.poly)
         if self.axis == "x":
             # x, y, z -> y, z, x
             y_min, _ = self.poly.min(0)
             y_max, _ = self.poly.max(0)
             line = sg.LineString([(y_min, z), (y_max, z)])
-            intersections = poly.intersection(line)
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    "ignore", category=RuntimeWarning, module="shapely"
+                )
+                intersections = poly.intersection(line)
 
             if not isinstance(intersections, sg.MultiLineString):
                 intersection_array = np.asarray(intersections.coords)
                 if not intersection_array.shape[0]:
                     return np.zeros_like(Y, dtype=bool)
                 intersections = sg.MultiLineString([intersections])
 
@@ -169,15 +174,19 @@
                 return (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
 
         elif self.axis == "y":
             # x, y, z -> z, x, y
             _, x_min = self.poly.min(0)
             _, x_max = self.poly.max(0)
             line = sg.LineString([(z, x_min), (z, x_max)])
-            intersections = poly.intersection(line)
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    "ignore", category=RuntimeWarning, module="shapely"
+                )
+                intersections = poly.intersection(line)
 
             if not isinstance(intersections, sg.MultiLineString):
                 intersection_array = np.asarray(intersections.coords)
                 if not intersection_array.shape[0]:
                     return np.zeros_like(Y, dtype=bool)
                 intersections = sg.MultiLineString([intersections])
 
@@ -233,15 +242,15 @@
 
         if xyz in ["yzx", "zxy"]:
             raise NotImplementedError(
                 "Only prisms extruded perpendicular to the 'chip surface' are currently supported in Lumerical."
             )
 
     def _trimesh(self, color=None, scale=None):
-        from trimesh.creation import extrude_polygon
+        from trimesh.creation import extrude_polygon  # fmt: skip
 
         poly = sg.Polygon(self.poly)
         prism = extrude_polygon(poly, self.h_max - self.h_min)
         prism = prism.apply_translation((0, 0, self.h_min))
         if self.axis == "x":
             prism.vertices = np.roll(prism.vertices, shift=1, axis=1)  # type: ignore
         if self.axis == "y":
@@ -250,15 +259,15 @@
             sx, sy, sz = scale
             prism.vertices *= np.array([[sx, sy, sz]])  # type: ignore
         if color is not None:
             prism.visual.face_colors = _to_rgba(color)  # type: ignore
         return prism
 
     def _center(self):
-        import shapely.geometry as sg
+        import shapely.geometry as sg  # fmt: skip
 
         a, b = np.array(sg.Polygon(self.poly).centroid.xy).ravel()
         c = 0.5 * (self.h_min + self.h_max)
         x, y, z = {
             "x": (c, a, b),
             "y": (b, c, a),
             "z": (a, b, c),
@@ -270,12 +279,11 @@
             "x": (1, 0, 0),
             "y": (0, 1, 0),
             "z": (0, 0, 1),
         }[self.axis]
 
 
 def _to_rgba(c):
-    from matplotlib.colors import to_rgba as _to_rgba_mpl
-
+    from matplotlib.colors import to_rgba as _to_rgba_mpl  # fmt: skip
     r, g, b, a = _to_rgba_mpl(c)
     a = min(max(a, 0.1), 0.9)
     return float(r), float(g), float(b), float(a)
```

### Comparing `meow-sim-0.3.9/meow/integrate.py` & `meow-sim-0.4.0/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.9/meow/materials.py` & `meow-sim-0.4.0/meow/materials.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         ni = result.take(pos["targets"]["ni"], axs["targets"])
         n = nr + 1j * ni
         # FIXME: ideally we should just be able to return `n` here...
         # return n
         return np.squeeze(np.real(n))  # TODO: allow complex multi-dimensional n
 
     def _lumadd(self, sim, env, unit):
-        from matplotlib.cm import get_cmap
+        from matplotlib.cm import get_cmap  # fmt: skip
 
         n = self(env)
         wl = np.asarray(env.wl * unit, dtype=complex).ravel()
         eps = np.asarray(n, dtype=complex).ravel() ** 2
         data = np.stack([c / wl, eps], 1)  # permittivity, not index
 
         if not sim.materialexists(self.name):
```

### Comparing `meow-sim-0.3.9/meow/mesh.py` & `meow-sim-0.4.0/meow/mesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,24 +26,24 @@
         default=0.0,
         description="Azimuth angle of the propagation axis in the plane orthogonal to the mesh.",
     )
     angle_theta: float = Field(
         default=0.0,
         description="Polar angle of the propagation axis from the injection axis.",
     )
-    bend_radius: float = Field(
-        default=np.inf,
+    bend_radius: float | None = Field(
+        default=None,
         description=(
             "A curvature radius for simulation of waveguide bends. "
             "Tidy3D: Can be negative, in which case the mode plane center has a smaller value than "
             "the curvature center along the tangential axis perpendicular to the bend axis."
         ),
     )
-    bend_axis: Literal[0, 1] = Field(
-        default=1,
+    bend_axis: Literal[0, 1] | None = Field(
+        default=None,
         description=(
             "Index into the two tangential axes defining the normal to the plane in which the bend lies. "
             "This must be provided if ``bend_radius`` is not ``None``. For example, for a ring in the "
             "global xy-plane, and a mode plane in either the xz or the yz plane, the ``bend_axis`` is "
             "always 1 (the global z axis)."
         ),
     )
```

### Comparing `meow-sim-0.3.9/meow/mode.py` & `meow-sim-0.4.0/meow/mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ An EigenMode """
 
 import pickle
+import warnings
 from itertools import product
 from typing import Any, List, Tuple
 
 import numpy as np
 from pydantic import Field, PrivateAttr
 from scipy.constants import epsilon_0 as eps0
 from scipy.constants import mu_0 as mu0
@@ -116,16 +117,16 @@
         fields=None,
         ax=None,
         n_cmap=None,
         mode_cmap=None,
         num_levels=8,
         operation=lambda x: np.abs(x) ** 2,
     ):
-        import matplotlib.pyplot as plt
-        from matplotlib import colors
+        import matplotlib.pyplot as plt  # fmt: skip
+        from matplotlib import colors  # fmt: skip
 
         if fields is None or len(fields) == 0:
             fields = ["Ex"]
 
         if len(fields) > 1:
             if ax is None:
                 _, ax = plt.subplots(len(fields), 1, figsize=(5, len(fields) * 3))
@@ -163,15 +164,17 @@
                 name="c_cmap", colors=["#ffffff", "#c1d9ed"]
             )
         if mode_cmap is None:
             mode_cmap = "inferno"
         X = getattr(self.mesh, f"X{c}")
         Y = getattr(self.mesh, f"Y{c}")
         mode = operation(getattr(self, field))
-        plt.contour(X, Y, mode, cmap=mode_cmap, levels=np.linspace(mode.min(), mode.max(), num_levels))  # fmt: skip
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=UserWarning)
+            plt.contour(X, Y, mode, cmap=mode_cmap, levels=np.linspace(mode.min(), mode.max(), num_levels))  # fmt: skip
         plt.colorbar(label="mode")
 
         n = np.real(getattr(self.cs, f"n{c}"))
         plt.pcolormesh(X, Y, n, cmap=n_cmap)
         plt.colorbar(label="n")
         plt.xlabel(x)
         plt.ylabel(y)
```

### Comparing `meow-sim-0.3.9/meow/structures.py` & `meow-sim-0.4.0/meow/structures.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
     def _visualize(self, scale=None):
         return self._trimesh(scale=scale).show()
 
 
 def visualize_structures(structures, scale=None):
     """easily visualize a collection (list) of `Structure` objects"""
-    from trimesh.scene import Scene
-    from trimesh.transformations import rotation_matrix
+    from trimesh.scene import Scene  # fmt: skip
+    from trimesh.transformations import rotation_matrix  # fmt: skip
 
     scene = Scene(
         geometry=[s._trimesh(scale=scale) for s in sort_structures(structures)]
     )
     scene.apply_transform(rotation_matrix(np.pi - np.pi / 6, (0, 1, 0)))
     return scene.show()
```

### Comparing `meow-sim-0.3.9/meow/visualize.py` & `meow-sim-0.4.0/meow/visualize.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """ Visualizations for common meow-datatypes """
 
+import warnings
 from typing import Any
 
 import numpy as np
 
 try:
     import matplotlib.pyplot as plt
+
+
 except ImportError:
     plt = None
 
 try:
-    import gdsfactory as gf
+    import gdsfactory as gf  # fmt: skip
 except ImportError:
     gf = None
 
 try:
-    from jaxlib.xla_extension import DeviceArray  # type: ignore
+    from jaxlib.xla_extension import DeviceArray  # fmt: skip # type: ignore
 except ImportError:
     DeviceArray = None
 
 
 def _visualize_s_matrix(S, fmt=".3f", title=None, show=True):
-    import matplotlib.pyplot as plt
+    import matplotlib.pyplot as plt  # fmt: skip
 
     Z = np.abs(S)
     y, x = np.arange(Z.shape[0])[::-1], np.arange(Z.shape[1])
     Y, X = np.meshgrid(y, x)
 
     plt.figure(figsize=(2 * x.shape[0] / 3, 2 * y.shape[0] / 3))
     plt.pcolormesh(X, Y, Z[::-1].T, cmap="Greys", vmin=0.0, vmax=2.0 * Z.max())
@@ -55,15 +58,15 @@
         plt.title(title)
 
     if show:
         plt.show()
 
 
 def _visualize_s_pm_matrix(Spm, fmt=".3f", title=None, show=True):
-    import matplotlib.pyplot as plt
+    import matplotlib.pyplot as plt  # fmt: skip
 
     S, pm = Spm
     _visualize_s_matrix(S, fmt=fmt, title=title, show=False)
     num_left = len([p for p in pm if "left" in p])
     Z = np.abs(S)
     y, x = np.arange(Z.shape[0])[::-1], np.arange(Z.shape[1])
 
@@ -71,15 +74,15 @@
     plt.axhline(x[num_left] - 0.5, color="red")
 
     if show:
         plt.show()
 
 
 def _visualize_gdsfactory(comp):
-    import gdsfactory as gf
+    import gdsfactory as gf  # fmt: skip
 
     gf.plot(comp)  # type: ignore
 
 
 def _is_s_matrix(obj: Any):
     return (
         (
@@ -97,17 +100,17 @@
         x, y = obj
         return True
     except Exception:
         return False
 
 
 def _visualize_modes(modes):
-    from mpl_toolkits.axes_grid1 import make_axes_locatable
-    import matplotlib.pyplot as plt
-    from matplotlib.colors import LinearSegmentedColormap
+    import matplotlib.pyplot as plt  # fmt: skip
+    from matplotlib.colors import LinearSegmentedColormap  # fmt: skip
+    from mpl_toolkits.axes_grid1 import make_axes_locatable  # fmt: skip
 
     num_modes = len(modes)
     cs = modes[0].cs
     X, Y, n = cs.mesh.Xz, cs.mesh.Yz, cs.nz
     x_min, x_max = cs.mesh.x.min(), cs.mesh.x.max()
     y_min, y_max = cs.mesh.y.min(), cs.mesh.y.max()
     delta_x = x_max - x_min
@@ -141,15 +144,17 @@
                 f"M{i}: {field}: n={m.neff.real:.2f}+{m.neff.imag:.1e}j, {100*m.te_fraction:.1f}%TE",
                 fontsize=9,
             )
             plt.pcolormesh(X, Y, n, cmap=n_cmap)
             value[value < 1e-2] = np.nan
             # value[0, 0] = 0.0
             # value[-1, -1] = mx[field]
-            plt.contour(X, Y, value, cmap="inferno")
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore", category=UserWarning)
+                plt.contour(X, Y, value, cmap="inferno")
             divider = make_axes_locatable(ax[i, j])
             cax = divider.append_axes("right", size="5%", pad=0.05)
             plt.colorbar(cax=cax)
     fig.subplots_adjust(hspace=0, wspace=2 / (2 * W))
 
 
 def visualize(obj: Any, **kwargs: Any):
@@ -159,17 +164,17 @@
         obj: the meow object to visualize
         **kwargs: extra configuration to visualize the object
 
     Note:
         Most meow objects have a `._visualize` method.
         Check out its help to see which kwargs are accepted.
     """
-    from .mode import Mode
-    from .base_model import BaseModel
-    from .structures import Structure, visualize_structures
+    from .base_model import BaseModel  # fmt: skip
+    from .mode import Mode  # fmt: skip
+    from .structures import Structure, visualize_structures  # fmt: skip
 
     # if isinstance(obj, Mode):
     #    return _visualize_mode(obj)
     if isinstance(obj, list) and all(isinstance(o, Mode) for o in obj):
         return _visualize_modes(obj)
     elif isinstance(obj, BaseModel):
         return obj._visualize(**kwargs)
```

### Comparing `meow-sim-0.3.9/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.4.0/meow_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.9
+Version: 0.4.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.3.9/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.4.0/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.9/pyproject.toml` & `meow-sim-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.3.9"
+version = "0.4.0"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.3.9/tests/test_deserialization.py` & `meow-sim-0.4.0/tests/test_deserialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from functools import lru_cache, wraps
-from typing import List
-
 import numpy as np
-from pydantic import Field, parse_raw_as
+from pydantic import Field
 
 import meow as mw
 
 
 class SimpleMode(mw.BaseModel):
     neff: complex = Field(description="the effective index of the mode")
     cs: mw.CrossSection = Field(
```

### Comparing `meow-sim-0.3.9/tests/test_mode_operators.py` & `meow-sim-0.4.0/tests/test_mode_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from meow import Mode
 
-
 MODE_DATA = {
     "neff": {"real": 3.526228477887, "imag": -0.03995016558},
     "Ex": [1, 1],
     "Ey": [2, 2],
     "Ez": [3, 3],
     "Hx": [1, 1],
     "Hy": [2, 2],
@@ -123,10 +122,10 @@
 
 
 def test_divide_scalar():
     assert (mode1 / 2).Ex[0, 0] == 1 / 2
 
 
 if __name__ == "__main__":
-    import pytest
+    import pytest  # fmt: skip
 
     pytest.main([__file__])
```

### Comparing `meow-sim-0.3.9/tests/test_nbs.py` & `meow-sim-0.4.0/tests/test_nbs.py`

 * *Files identical despite different names*

