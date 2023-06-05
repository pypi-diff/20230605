# Comparing `tmp/meow-sim-0.3.5.tar.gz` & `tmp/meow-sim-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.3.5.tar", last modified: Thu Jun  1 00:57:41 2023, max compression
+gzip compressed data, was "meow-sim-0.3.8.tar", last modified: Mon Jun  5 01:53:52 2023, max compression
```

## Comparing `meow-sim-0.3.5.tar` & `meow-sim-0.3.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.199327 meow-sim-0.3.5/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-01 00:57:36.000000 meow-sim-0.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3178 2023-06-01 00:57:41.199327 meow-sim-0.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-01 00:57:36.000000 meow-sim-0.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.191327 meow-sim-0.3.5/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.191327 meow-sim-0.3.5/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8007 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.191327 meow-sim-0.3.5/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3667 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.195327 meow-sim-0.3.5/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3440 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10197 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10785 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3564 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    11409 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-06-01 00:57:36.000000 meow-sim-0.3.5/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.199327 meow-sim-0.3.5/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3178 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      395 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-01 00:57:41.000000 meow-sim-0.3.5/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1890 2023-06-01 00:57:36.000000 meow-sim-0.3.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 00:57:41.199327 meow-sim-0.3.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 00:57:41.199327 meow-sim-0.3.5/tests/
--rw-r--r--   0 root         (0) root         (0)     4009 2023-06-01 00:57:36.000000 meow-sim-0.3.5/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-06-01 00:57:36.000000 meow-sim-0.3.5/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-01 00:57:36.000000 meow-sim-0.3.5/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.454864 meow-sim-0.3.8/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-05 01:53:48.000000 meow-sim-0.3.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 01:53:52.454864 meow-sim-0.3.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 01:53:48.000000 meow-sim-0.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.450864 meow-sim-0.3.8/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.450864 meow-sim-0.3.8/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.450864 meow-sim-0.3.8/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5317 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.450864 meow-sim-0.3.8/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10178 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10785 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-06-05 01:53:48.000000 meow-sim-0.3.8/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.454864 meow-sim-0.3.8/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 01:53:52.000000 meow-sim-0.3.8/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-05 01:53:48.000000 meow-sim-0.3.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 01:53:52.454864 meow-sim-0.3.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:53:52.454864 meow-sim-0.3.8/tests/
+-rw-r--r--   0 root         (0) root         (0)     4009 2023-06-05 01:53:48.000000 meow-sim-0.3.8/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-06-05 01:53:48.000000 meow-sim-0.3.8/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-05 01:53:48.000000 meow-sim-0.3.8/tests/test_nbs.py
```

### Comparing `meow-sim-0.3.5/LICENSE` & `meow-sim-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/PKG-INFO` & `meow-sim-0.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.5
+Version: 0.3.8
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `meow-sim-0.3.5/README.md` & `meow-sim-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/__init__.py` & `meow-sim-0.3.8/meow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.3.5"
+__version__ = "0.3.8"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.3.5/meow/assets/silicon.csv` & `meow-sim-0.3.8/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/assets/silicon_oxide.csv` & `meow-sim-0.3.8/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/base_model.py` & `meow-sim-0.3.8/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/cache.py` & `meow-sim-0.3.8/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/cell.py` & `meow-sim-0.3.8/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/cross_section.py` & `meow-sim-0.3.8/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/eme/__init__.py` & `meow-sim-0.3.8/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/eme/common.py` & `meow-sim-0.3.8/meow/eme/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 """ SAX backend for EME (default backend) """
 from typing import Any, Dict, List
 
 import numpy as np
 
-from ..mode import Mode, inner_product
+from ..mode import Mode, inner_product as inner_product_normal, inner_product_conj
+
+DEFAULT_CONJUGATE_TRANSPOSE = True
+DEFAULT_ENFORCE_RECIPROCITY = False
+DEFAULT_ENFORCE_LOSSY_UNITARITY = False
 
 
 def compute_interface_s_matrix(
     modes1: List[Mode],
     modes2: List[Mode],
-    enforce_reciprocity: bool = True,
-    enforce_lossy_unitarity: bool = False,
+    conjugate_transpose: bool = DEFAULT_CONJUGATE_TRANSPOSE,
+    enforce_reciprocity: bool = DEFAULT_ENFORCE_RECIPROCITY,
+    enforce_lossy_unitarity: bool = DEFAULT_ENFORCE_LOSSY_UNITARITY,
 ):
     """get the S-matrix of the interface between two `CrossSection`s"""
     # overlap matrices
+    inner_product = inner_product_conj if conjugate_transpose else inner_product_normal
+    transp = (lambda x: x.T.conj()) if conjugate_transpose else (lambda x: x.T)
     NL, NR = len(modes1), len(modes2)
     O_LL = np.array([inner_product(modes1[m], modes1[m]) for m in range(NL)])
     O_RR = np.array([inner_product(modes2[n], modes2[n]) for n in range(NR)])
-    O_LR = np.array(
-        [[inner_product(modes1[m], modes2[n]) for n in range(NR)] for m in range(NL)]
-    )
-    O_RL = np.array(
-        [[inner_product(modes2[m], modes1[n]) for n in range(NL)] for m in range(NR)]
-    )
+    O_LR = np.array([[inner_product(modes1[m], modes2[n]) for n in range(NR)] for m in range(NL)])  # fmt: skip
+    O_RL = np.array([[inner_product(modes2[m], modes1[n]) for n in range(NL)] for m in range(NR)])  # fmt: skip
 
-    # extra phase correction.
+    # extra phase correction (disabled?).
 
     # ignoring the phase seems to corresponds best with lumerical.
-    O_LL = np.abs(O_LL)
-    O_RR = np.abs(O_RR)
+    # O_LL = np.abs(O_LL)
+    # O_RR = np.abs(O_RR)
 
     # alternative phase correction (probably worth testing this out)
     # O_LL = O_LL*np.exp(-1j*np.angle(O_LL))
     # O_RR = O_RR*np.exp(-1j*np.angle(O_RR))
 
     # yet another alternative phase correction (probably worth testing this out too)
-    # O_LR = O_LR@np.diag(np.exp(-1j*np.angle(np.diag(O_LR))))
-    # O_RL = O_RL@np.diag(np.exp(-1j*np.angle(np.diag(O_RL))))
+    # O_LR = O_LR*np.diag(np.exp(-1j*np.angle(np.diag(O_LR))))
+    # O_RL = O_RL*np.diag(np.exp(-1j*np.angle(np.diag(O_RL))))
 
     # transmission L->R
-    LHS = O_LR + O_RL.T
+    LHS = O_LR + transp(O_RL)
     RHS = np.diag(2 * O_LL)
     T_LR, _, _, _ = np.linalg.lstsq(LHS, RHS, rcond=None)
-    U, t, V = np.linalg.svd(T_LR, full_matrices=False)
 
     # HACK: we don't expect gain --> invert singular values that lead to gain
     # see: https://github.com/BYUCamachoLab/emepy/issues/12
+    U, t, V = np.linalg.svd(T_LR, full_matrices=False)
     t = np.where(t > 1, 1 / t, t)
-
     T_LR = U @ np.diag(t) @ V
 
     # transmission R->L
-    LHS = O_RL + O_LR.T
+    LHS = O_RL + transp(O_LR)
     RHS = np.diag(2 * O_RR)
     T_RL, _, _, _ = np.linalg.lstsq(LHS, RHS, rcond=None)
-    U, t, V = np.linalg.svd(T_RL, full_matrices=False)
 
     # HACK: we don't expect gain --> invert singular values that lead to gain
+    U, t, V = np.linalg.svd(T_RL, full_matrices=False)
     t = np.where(t > 1, 1 / t, t)
-
     T_RL = U @ np.diag(t) @ V
 
     # reflection
-    R_LR = np.diag(1 / (2 * O_LL)) @ (O_RL.T - O_LR) @ T_LR  # type: ignore
-    R_RL = np.diag(1 / (2 * O_RR)) @ (O_LR.T - O_RL) @ T_RL  # type: ignore
+    R_LR = np.diag(1 / (2 * O_LL)) @ (transp(O_RL) - O_LR) @ T_LR  # type: ignore
+    R_RL = np.diag(1 / (2 * O_RR)) @ (transp(O_LR) - O_RL) @ T_RL  # type: ignore
 
     # s-matrix
     S = np.concatenate(
         [
             np.concatenate([R_LR, T_RL], 1),
             np.concatenate([T_LR, R_RL], 1),
         ],
@@ -89,22 +90,24 @@
     port_map = {p: i for i, p in enumerate(in_ports + out_ports)}
 
     return S, port_map
 
 
 def compute_interface_s_matrices(
     modes: List[List[Mode]],
-    enforce_reciprocity: bool = True,
-    enforce_lossy_unitarity: bool = False,
+    conjugate_transpose: bool = DEFAULT_CONJUGATE_TRANSPOSE,
+    enforce_reciprocity: bool = DEFAULT_ENFORCE_RECIPROCITY,
+    enforce_lossy_unitarity: bool = DEFAULT_ENFORCE_LOSSY_UNITARITY,
 ):
     """get all the S-matrices of all the interfaces in a collection of `CrossSections`"""
     return {
         f"i_{i}_{i + 1}": compute_interface_s_matrix(
             modes1=modes1,
             modes2=modes2,
+            conjugate_transpose=conjugate_transpose,
             enforce_reciprocity=enforce_reciprocity,
             enforce_lossy_unitarity=enforce_lossy_unitarity,
         )
         for i, (modes1, modes2) in enumerate(zip(modes[:-1], modes[1:]))
     }
```

### Comparing `meow-sim-0.3.5/meow/eme/sax.py` & `meow-sim-0.3.8/meow/eme/sax.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 from sax.circuit import _make_singlemode_or_multimode
 from sax.netlist import Netlist
 from sax.utils import get_ports
 
 from ..base_model import _array
 from ..mode import Mode
 from .common import compute_interface_s_matrices, compute_propagation_s_matrices
-from .common import select_ports as select_ports
+from .common import (
+    select_ports as select_ports,
+    DEFAULT_CONJUGATE_TRANSPOSE,
+    DEFAULT_ENFORCE_RECIPROCITY,
+    DEFAULT_ENFORCE_LOSSY_UNITARITY,
+)
 
 try:
     import klujax
 except ImportError:
     klujax = None
 
 
@@ -71,17 +76,18 @@
             f"Invalid SAX Backend. Got: {sax_backend!r}. Should be 'default' or 'klu'."
         )
     return sax_backend
 
 
 def compute_s_matrix_sax(
     modes: List[List[Mode]],
-    sax_backend=None,
-    enforce_reciprocity=True,
-    enforce_lossy_unitarity=False,
+    sax_backend: str | None = None,
+    conjugate_transpose: bool = DEFAULT_CONJUGATE_TRANSPOSE,
+    enforce_reciprocity: bool = DEFAULT_ENFORCE_RECIPROCITY,
+    enforce_lossy_unitarity: bool = DEFAULT_ENFORCE_LOSSY_UNITARITY,
     **kwargs,
 ):
     """Calculate the S-matrix for given sets of modes, each set belonging to a `Cell`
 
     Args:
         modes: Each collection of modes for each of the `Cell` objects
         backend: which SAX backend to use to calculate the final S-matrix.
@@ -92,14 +98,15 @@
     )
     _compute_interface_s_matrices = kwargs.pop(
         "compute_interface_s_matrices", compute_interface_s_matrices
     )
     propagations = _compute_propagation_s_matrices(modes)
     interfaces = _compute_interface_s_matrices(
         modes,
+        conjugate_transpose=conjugate_transpose,
         enforce_reciprocity=enforce_reciprocity,
         enforce_lossy_unitarity=enforce_lossy_unitarity,
         **kwargs,
     )
 
     # TODO: fix SAX Multimode to reduce this ad-hoc SAX-hacking.
     net = _get_netlist(propagations, interfaces)
```

### Comparing `meow-sim-0.3.5/meow/environment.py` & `meow-sim-0.3.8/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/fde/lumerical.py` & `meow-sim-0.3.8/meow/fde/lumerical.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ FDE Lumerical Backend """
 
 from typing import Optional
 
 import numpy as np
-from pydantic import validate_arguments
 from pydantic.types import PositiveInt
 
 from ..cross_section import CrossSection
 from ..mode import Mode, normalize_energy, zero_phase
 
 _global = {"sim": None}
 
@@ -23,83 +22,116 @@
 
 def set_sim(
     sim: "lumapi.MODE",  # type: ignore
 ):
     _global["sim"] = sim
 
 
-def get_sim():
+def get_sim(**kwargs):
+    sim = kwargs.get("sim", None)
+    if sim is not None:
+        return sim
     sim = _global["sim"]
     if sim is None:
         raise ValueError(
             "Could not start Lumerical simulation. "
             "Please either pass the `lumapi.MODE` simulation object as an argument to `compute_modes_lumerical` or "
             "use `set_sim(sim)` to globally set the lumapi.MODE simulation object."
         )
     return sim
 
 
+def create_lumerical_geometries(sim, structures, env, unit):
+    sim = get_sim(sim=sim)
+    sim.switchtolayout()
+    sim.deleteall()
+    for s in structures:
+        s._lumadd(sim, env, unit, "yzx")
+
+
 # @validate_arguments
 def compute_modes_lumerical(
     cs: CrossSection,
     num_modes: PositiveInt = 10,
     sim: Optional["lumapi.MODE"] = None,  # type: ignore
     unit: float = 1e-6,
 ):
     """compute ``Modes` for a given ``FdeSpec` (Lumerical backend)
 
     Args:
         sim: the lumerical simulation object
         spec: The FDE simulation specification
         unit: Conversion factor between MEOW unit (probably um) and Lumerical unit (probably m).
     """
+    from lumapi import LumApiError, MODE  # fmt: skip # type: ignore
+
+    sim = get_sim(sim=sim)
     _assert_default_mesh_setting(cs.cell.mesh.angle_phi != 0, "angle_phi")
     _assert_default_mesh_setting(cs.cell.mesh.angle_theta != 0, "angle_theta")
     _assert_default_mesh_setting(cs.cell.mesh.bend_radius < 1e10, "bend_radius")
 
-    if sim is None:
-        sim = get_sim()
-
     assert sim is not None
-
-    sim.switchtolayout()
-    sim.deleteall()
-    for s in cs.structures:
-        s._lumadd(sim, cs.env, unit, "yzx")
-
+    create_lumerical_geometries(sim, cs.cell.structures, cs.env, unit)
     sim.select("FDE")
     sim.delete()
+    pml_settings = {}
+    num_pml_y, num_pml_z = 0, 0
+    if cs.cell.mesh.num_pml[0] > 0:
+        pml_settings.update(
+            {
+                "y_min_bc": "PML",
+                "y_max_bc": "PML",
+            }
+        )
+        num_pml_y = 22  # TODO: allow adjusting these values
+    if cs.cell.mesh.num_pml[1] > 0:
+        pml_settings.update(
+            {
+                "z_min_bc": "PML",
+                "z_max_bc": "PML",
+            }
+        )
+        num_pml_z = 22  # TODO: allow adjusting these values
     sim.addfde(
         background_index=1.0,
         solver_type="2D X normal",
         x=float(cs.cell.z * unit),
         y_min=float(cs.mesh.x.min() * unit),
         y_max=float(cs.mesh.x.max() * unit),
         z_min=float(cs.mesh.y.min() * unit),
         z_max=float(cs.mesh.y.max() * unit),
-        define_z_mesh_by="number of mesh cells",
         define_y_mesh_by="number of mesh cells",
+        define_z_mesh_by="number of mesh cells",
         mesh_cells_y=cs.mesh.x_.shape[0],
         mesh_cells_z=cs.mesh.y_.shape[0],
+        **pml_settings,
     )
+    # set mesh size again, because PML messes with it:
+    if cs.cell.mesh.num_pml[0] > 0:
+        sim.setnamed("FDE", "mesh cells y", cs.mesh.x_.shape[0] - num_pml_y)
+    if cs.cell.mesh.num_pml[1] > 0:
+        sim.setnamed("FDE", "mesh cells z", cs.mesh.y_.shape[0] - num_pml_z)
     sim.setanalysis("number of trial modes", int(num_modes))
     sim.setanalysis("search", "near n")
     sim.setanalysis("use max index", True)
     sim.setanalysis("wavelength", float(cs.env.wl * unit))
     sim.findmodes()
     modes = []
     for j in range(1, num_modes + 1):
-        mode = Mode(
-            neff=sim.getdata(f"mode{j}", "neff").ravel().item(),
-            cs=cs,
-            Ez=sim.getdata(f"mode{j}", "Ex").squeeze()[:-1, :-1],
-            Ex=sim.getdata(f"mode{j}", "Ey").squeeze()[:-1, :-1],
-            Ey=sim.getdata(f"mode{j}", "Ez").squeeze()[:-1, :-1],
-            Hz=sim.getdata(f"mode{j}", "Hx").squeeze()[:-1, :-1],
-            Hx=sim.getdata(f"mode{j}", "Hy").squeeze()[:-1, :-1],
-            Hy=sim.getdata(f"mode{j}", "Hz").squeeze()[:-1, :-1],
-        )
+        try:
+            mode = Mode(
+                neff=sim.getdata(f"mode{j}", "neff").ravel().item(),
+                cs=cs,
+                Ez=sim.getdata(f"mode{j}", "Ex").squeeze()[:-1, :-1],
+                Ex=sim.getdata(f"mode{j}", "Ey").squeeze()[:-1, :-1],
+                Ey=sim.getdata(f"mode{j}", "Ez").squeeze()[:-1, :-1],
+                Hz=sim.getdata(f"mode{j}", "Hx").squeeze()[:-1, :-1],
+                Hx=sim.getdata(f"mode{j}", "Hy").squeeze()[:-1, :-1],
+                Hy=sim.getdata(f"mode{j}", "Hz").squeeze()[:-1, :-1],
+            )
+        except LumApiError:
+            break
         mode = normalize_energy(mode)
         mode = zero_phase(mode)
         modes.append(mode)
 
     return sorted(modes, key=lambda m: np.real(m.neff), reverse=True)
```

### Comparing `meow-sim-0.3.5/meow/fde/tidy3d.py` & `meow-sim-0.3.8/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/gds_structures.py` & `meow-sim-0.3.8/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/geometries.py` & `meow-sim-0.3.8/meow/geometries.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     def _mask2d_single(self, X, Y, z):
         poly = sg.Polygon(self.poly)
         if self.axis == "x":
             # x, y, z -> y, z, x
             y_min, _ = self.poly.min(0)
             y_max, _ = self.poly.max(0)
             line = sg.LineString([(y_min, z), (y_max, z)])
-            intersections = np.asarray(poly.intersection(line).coords)
+            intersections = poly.intersection(line)
 
             if not isinstance(intersections, sg.MultiLineString):
                 intersection_array = np.asarray(intersections.coords)
                 if not intersection_array.shape[0]:
                     return np.zeros_like(Y, dtype=bool)
                 intersections = sg.MultiLineString([intersections])
```

### Comparing `meow-sim-0.3.5/meow/integrate.py` & `meow-sim-0.3.8/meow/integrate.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,12 +21,12 @@
         lambda x: extent[1][0],
         lambda x: extent[1][1],
         epsabs=1,
         epsrel=0.001,
     )[0]
 
 
-def integrate_2d(x, y, data):
+def integrate_2d(x, y, data) -> float:
     """much simpler integration over the full grid"""
     int1 = simpson(data, y)
     int2 = simpson(int1, x)
-    return int2
+    return float(int2)
```

### Comparing `meow-sim-0.3.5/meow/materials.py` & `meow-sim-0.3.8/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/mesh.py` & `meow-sim-0.3.8/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow/mode.py` & `meow-sim-0.3.8/meow/mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ An EigenMode """
 
 import pickle
 from itertools import product
 from typing import Any, List, Tuple
-import numbers
 
 import numpy as np
 from pydantic import Field, PrivateAttr
 from scipy.constants import epsilon_0 as eps0
 from scipy.constants import mu_0 as mu0
 from scipy.linalg import norm
 
@@ -45,18 +44,18 @@
     _Px: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = PrivateAttr()
     _Py: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = PrivateAttr()
     _Pz: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = PrivateAttr()
     _A: np.float_ = PrivateAttr()
 
     def __init__(self, **data: Any):
         super().__init__(**data)
-        self._Px = None
-        self._Py = None
-        self._Pz = None
-        self._A = None
+        self._Px = None  # type: ignore
+        self._Py = None  # type: ignore
+        self._Pz = None  # type: ignore
+        self._A = None  # type: ignore
 
     @property
     def te_fraction(self):
         """the TE polarization fraction of the mode."""
         return te_fraction(self)
 
     def _calc_poynting(self):
@@ -68,15 +67,15 @@
 
     def _calc_area(self):
         vecE = np.stack([self.Ex, self.Ey, self.Ez], axis=-1)
         E_sq = norm(vecE, axis=-1, ord=2)
         E_qu = E_sq**2
         x = self.cs.mesh.x_
         y = self.cs.mesh.y_
-        self._A = integrate_2d(x, y, E_sq) ** 2 / integrate_2d(x, y, E_qu)
+        self._A = np.float_(integrate_2d(x, y, E_sq) ** 2 / integrate_2d(x, y, E_qu))
 
     @property
     def Px(self):
         if self._Px is None:
             self._calc_poynting()
         return self._Px
 
@@ -208,15 +207,15 @@
             Hx=self.Hx + other.Hx,
             Hy=self.Hy + other.Hy,
             Hz=self.Hz + other.Hz,
         )
         return new_mode
 
     def __mul__(self, other):
-        if not isinstance(other, numbers.Number):
+        if not isinstance(other, (float, complex)):
             raise TypeError(
                 f"unsupported operand type(s) for *: 'Mode' and '{type(other).__name__}'"
             )
         new_mode = Mode(
             neff=self.neff,
             cs=self.cs,
             Ex=self.Ex * other,
@@ -227,15 +226,15 @@
             Hz=self.Hz * other,
         )
         return new_mode
 
     __rmul__ = __mul__
 
     def __truediv__(self, other):
-        if not isinstance(other, numbers.Number):
+        if not isinstance(other, (float, complex)):
             raise TypeError(
                 f"unsupported operand type(s) for /: 'Mode' and '{type(other).__name__}'"
             )
         return self * (1 / other)
 
     def __sub__(self, other):
         if not isinstance(other, Mode):
@@ -264,22 +263,28 @@
         Hz=mode.Hz * phase,
     )
     if _sum_around(np.real(new_mode.Hx), m, n) < 0:
         new_mode = invert_mode(new_mode)
     return new_mode
 
 
+# def _centroid_idxs(arr2d: np.ndarray) -> tuple[int, int]:
+#    centroid_x = np.average(np.arange(arr2d.shape[1]), weights=arr2d.sum(axis=0))
+#    centroid_y = np.average(np.arange(arr2d.shape[0]), weights=arr2d.sum(axis=1))
+#    return round(float(centroid_x)), round(float(centroid_y))
+
+
 def _sum_around(field, m, n, r=2):
     total = 0
     idxs = range(-r, r + 1)
     idx_tups = product(idxs, idxs)
     M, N = field.shape
     for i, j in idx_tups:
         m_ = min(m + i, M - 1) if i >= 0 else max(m + i, 0)
-        n_ = min(n + j, N - 1) if i >= 0 else max(n + j, 0)
+        n_ = min(n + j, N - 1) if j >= 0 else max(n + j, 0)
         total = total + field[m_, n_]
     return total
 
 
 def invert_mode(mode: Mode) -> Mode:
     """invert a `Mode`"""
     return Mode(
@@ -293,16 +298,23 @@
         Hz=-mode.Hz,
     )
 
 
 def inner_product(mode1: Mode, mode2: Mode) -> float:
     """the inner product of a `Mode` with another `Mode` is uniquely defined."""
     mesh = mode1.mesh
+    cross = mode1.Ex * mode2.Hy - mode1.Ey * mode2.Hx
+    return np.trapz(np.trapz(cross, mesh.y_), mesh.x_)
+
+
+def inner_product_conj(mode1: Mode, mode2: Mode) -> float:
+    """the inner product of a `Mode` with another `Mode` is uniquely defined."""
+    mesh = mode1.mesh
     cross = mode1.Ex * mode2.Hy.conj() - mode1.Ey * mode2.Hx.conj()
-    return 0.25 * np.trapz(np.trapz(cross, mesh.y_), mesh.x_)
+    return np.trapz(np.trapz(cross, mesh.y_), mesh.x_)
 
 
 def normalize_product(mode: Mode) -> Mode:
     """normalize a `Mode` according to the `inner_product` with itself"""
     factor = np.sqrt(inner_product(mode, mode))
     return Mode(
         neff=mode.neff,
```

### Comparing `meow-sim-0.3.5/meow/structures.py` & `meow-sim-0.3.8/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.3.8/meow_sim.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.3.5
+Version: 0.3.8
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `meow-sim-0.3.5/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.3.8/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/pyproject.toml` & `meow-sim-0.3.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.3.5"
+version = "0.3.8"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
@@ -23,16 +23,14 @@
 license = { text = "Apache Software License" }
 readme = "README.md"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 dependencies = [
@@ -40,25 +38,25 @@
   "numpy>=1.24",
   "pydantic",
   "sax>=0.8.4",
   "scipy",
   "shapely",
   "tidy3d>=2.1",
   "trimesh[easy]",
-  "packaging", 
+  "packaging",
 ]
 
 [project.optional-dependencies]
 min = ["meow-sim"]
 vis = ["matplotlib", "trimesh[easy]"]
 jax = ["jax", "jaxlib"]
 klu = ["klujax>0.1.2"]
 ipy = ["ipykernel", "ipywidgets", "ipympl", "nbstripout", "tqdm"]
 gds = ["gdsfactory>6.27.0", "klayout>0.28.2"]
-dev = ["bump2version", "nbstripout", "pre-commit", "black", "sphinx", "autodoc-pydantic", "myst-nb>0.17.1"]
+dev = ["bump2version", "nbstripout", "pre-commit", "black", "sphinx", "autodoc-pydantic", "myst-nb>0.17.1", "jupyter-book"]
 full = ["meow-sim[vis,klu,jax,ipy,gds]"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["meow*"]
 exclude = []
 namespaces = true
```

### Comparing `meow-sim-0.3.5/tests/test_deserialization.py` & `meow-sim-0.3.8/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/tests/test_mode_operators.py` & `meow-sim-0.3.8/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.3.5/tests/test_nbs.py` & `meow-sim-0.3.8/tests/test_nbs.py`

 * *Files identical despite different names*

