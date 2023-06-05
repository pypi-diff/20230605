# Comparing `tmp/autoeap-0.3.1.3.tar.gz` & `tmp/autoeap-0.3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autoeap-0.3.1.3.tar", last modified: Mon Feb 13 13:16:26 2023, max compression
+gzip compressed data, was "dist/autoeap-0.3.1.4.tar", last modified: Mon Jun  5 10:18:57 2023, max compression
```

## Comparing `autoeap-0.3.1.3.tar` & `autoeap-0.3.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/
--rw-r--r--   0 batty      (501) staff       (20)     2046 2020-11-26 15:30:23.000000 autoeap-0.3.1.3/.gitignore
--rw-r--r--   0 batty      (501) staff       (20)     1080 2020-11-26 15:26:27.000000 autoeap-0.3.1.3/LICENCE
--rw-r--r--   0 batty      (501) staff       (20)    15890 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/PKG-INFO
--rw-r--r--   0 batty      (501) staff       (20)    13398 2022-09-23 10:54:15.000000 autoeap-0.3.1.3/README.md
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/autoeap.egg-info/
--rw-r--r--   0 batty      (501) staff       (20)    15890 2023-02-13 13:16:17.000000 autoeap-0.3.1.3/autoeap.egg-info/PKG-INFO
--rw-r--r--   0 batty      (501) staff       (20)      852 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/autoeap.egg-info/SOURCES.txt
--rw-r--r--   0 batty      (501) staff       (20)        1 2023-02-13 13:16:17.000000 autoeap-0.3.1.3/autoeap.egg-info/dependency_links.txt
--rw-r--r--   0 batty      (501) staff       (20)       62 2023-02-13 13:16:17.000000 autoeap-0.3.1.3/autoeap.egg-info/entry_points.txt
--rw-r--r--   0 batty      (501) staff       (20)      187 2023-02-13 13:16:17.000000 autoeap-0.3.1.3/autoeap.egg-info/requires.txt
--rw-r--r--   0 batty      (501) staff       (20)       12 2023-02-13 13:16:17.000000 autoeap-0.3.1.3/autoeap.egg-info/top_level.txt
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/docs/
--rw-r--r--   0 batty      (501) staff       (20)    23035 2021-10-08 13:32:53.000000 autoeap-0.3.1.3/docs/autoeap_logo.png
--rw-r--r--   0 batty      (501) staff       (20)  1174747 2021-12-15 15:52:33.000000 autoeap-0.3.1.3/docs/autoeap_workflow.ipynb
--rw-r--r--   0 batty      (501) staff       (20)    98448 2021-10-08 13:32:53.000000 autoeap-0.3.1.3/docs/ktwo212466080-c17_k2sc.jpg
--rw-r--r--   0 batty      (501) staff       (20)    96918 2021-10-08 13:32:53.000000 autoeap-0.3.1.3/docs/ktwo212466080-c17_raw.jpg
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/examples/
--rw-r--r--   0 batty      (501) staff       (20)   217630 2021-12-14 17:25:46.000000 autoeap-0.3.1.3/examples/apply_k2sc.ipynb
--rw-r--r--   0 batty      (501) staff       (20)  5002560 2021-09-29 14:36:35.000000 autoeap-0.3.1.3/examples/ktwo212466080-c17_lpd-targ.fits
--rw-r--r--   0 batty      (501) staff       (20)    81259 2021-12-14 17:10:03.000000 autoeap-0.3.1.3/examples/shortest_introduction.ipynb
--rw-r--r--   0 batty      (501) staff       (20)   131011 2021-12-14 17:20:18.000000 autoeap-0.3.1.3/examples/trend_correction.ipynb
--rw-r--r--   0 batty      (501) staff       (20)   759397 2021-12-14 17:22:19.000000 autoeap-0.3.1.3/examples/usage_of_detrender.ipynb
--rw-r--r--   0 batty      (501) staff       (20)      147 2023-02-13 13:15:05.000000 autoeap-0.3.1.3/pyproject.toml
--rw-r--r--   0 batty      (501) staff       (20)      187 2023-02-13 13:11:09.000000 autoeap-0.3.1.3/requirements.txt
--rw-r--r--   0 batty      (501) staff       (20)       38 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/setup.cfg
--rw-r--r--   0 batty      (501) staff       (20)     1774 2022-01-18 17:27:57.000000 autoeap-0.3.1.3/setup.py
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/src/
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/src/PDM/
--rw-r--r--   0 batty      (501) staff       (20)   249676 2021-12-14 14:25:41.000000 autoeap-0.3.1.3/src/PDM/PDM_pyc.c
--rw-r--r--   0 batty      (501) staff       (20)     3313 2021-10-08 13:32:53.000000 autoeap-0.3.1.3/src/PDM/PDM_pyc.pyx
--rw-r--r--   0 batty      (501) staff       (20)     6145 2022-03-04 14:09:44.000000 autoeap-0.3.1.3/src/PDM/pdm.c
--rwxr-xr-x   0 batty      (501) staff       (20)      207 2021-02-28 19:38:35.000000 autoeap-0.3.1.3/src/__init__.py
--rw-r--r--   0 batty      (501) staff       (20)     2882 2021-11-07 16:12:45.000000 autoeap-0.3.1.3/src/aperture_to_fits.py
--rwxr-xr-x   0 batty      (501) staff       (20)    82291 2022-05-17 14:27:09.000000 autoeap-0.3.1.3/src/autoeapcore.py
--rw-r--r--   0 batty      (501) staff       (20)     8497 2021-10-08 13:39:51.000000 autoeap-0.3.1.3/src/detrender.py
--rw-r--r--   0 batty      (501) staff       (20)    17277 2021-10-08 13:32:53.000000 autoeap-0.3.1.3/src/k2sc_stable.py
--rwxr-xr-x   0 batty      (501) staff       (20)    61649 2020-11-23 21:12:27.000000 autoeap-0.3.1.3/src/photutils_stable.py
--rw-r--r--   0 batty      (501) staff       (20)       24 2023-02-13 13:15:42.000000 autoeap-0.3.1.3/src/version.py
-drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-02-13 13:16:26.000000 autoeap-0.3.1.3/tests/
--rw-r--r--   0 batty      (501) staff       (20)   140920 2021-12-14 17:00:19.000000 autoeap-0.3.1.3/tests/EPIC220198696_c8_autoEAP.lc
--rw-r--r--   0 batty      (501) staff       (20)    93650 2021-12-14 17:03:00.000000 autoeap-0.3.1.3/tests/EPIC220198696_c8_autoEAP.lc_corr
--rw-r--r--   0 batty      (501) staff       (20)      535 2021-10-08 13:32:53.000000 autoeap-0.3.1.3/tests/test_detrender.py
--rw-r--r--   0 batty      (501) staff       (20)      524 2021-10-08 13:32:53.000000 autoeap-0.3.1.3/tests/test_raw_lightcurve.py
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/
+-rw-r--r--   0 batty      (501) staff       (20)     2046 2020-11-26 15:30:23.000000 autoeap-0.3.1.4/.gitignore
+-rw-r--r--   0 batty      (501) staff       (20)     1080 2020-11-26 15:26:27.000000 autoeap-0.3.1.4/LICENCE
+-rw-r--r--   0 batty      (501) staff       (20)    15890 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/PKG-INFO
+-rw-r--r--   0 batty      (501) staff       (20)    13398 2022-09-23 10:54:15.000000 autoeap-0.3.1.4/README.md
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/autoeap.egg-info/
+-rw-r--r--   0 batty      (501) staff       (20)    15890 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/autoeap.egg-info/PKG-INFO
+-rw-r--r--   0 batty      (501) staff       (20)      852 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/autoeap.egg-info/SOURCES.txt
+-rw-r--r--   0 batty      (501) staff       (20)        1 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/autoeap.egg-info/dependency_links.txt
+-rw-r--r--   0 batty      (501) staff       (20)       62 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/autoeap.egg-info/entry_points.txt
+-rw-r--r--   0 batty      (501) staff       (20)      187 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/autoeap.egg-info/requires.txt
+-rw-r--r--   0 batty      (501) staff       (20)       12 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/autoeap.egg-info/top_level.txt
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/docs/
+-rw-r--r--   0 batty      (501) staff       (20)    23035 2021-10-08 13:32:53.000000 autoeap-0.3.1.4/docs/autoeap_logo.png
+-rw-r--r--   0 batty      (501) staff       (20)  1174747 2021-12-15 15:52:33.000000 autoeap-0.3.1.4/docs/autoeap_workflow.ipynb
+-rw-r--r--   0 batty      (501) staff       (20)    98448 2021-10-08 13:32:53.000000 autoeap-0.3.1.4/docs/ktwo212466080-c17_k2sc.jpg
+-rw-r--r--   0 batty      (501) staff       (20)    96918 2021-10-08 13:32:53.000000 autoeap-0.3.1.4/docs/ktwo212466080-c17_raw.jpg
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/examples/
+-rw-r--r--   0 batty      (501) staff       (20)   217630 2021-12-14 17:25:46.000000 autoeap-0.3.1.4/examples/apply_k2sc.ipynb
+-rw-r--r--   0 batty      (501) staff       (20)  5002560 2021-09-29 14:36:35.000000 autoeap-0.3.1.4/examples/ktwo212466080-c17_lpd-targ.fits
+-rw-r--r--   0 batty      (501) staff       (20)    81259 2021-12-14 17:10:03.000000 autoeap-0.3.1.4/examples/shortest_introduction.ipynb
+-rw-r--r--   0 batty      (501) staff       (20)   131011 2021-12-14 17:20:18.000000 autoeap-0.3.1.4/examples/trend_correction.ipynb
+-rw-r--r--   0 batty      (501) staff       (20)   759397 2021-12-14 17:22:19.000000 autoeap-0.3.1.4/examples/usage_of_detrender.ipynb
+-rw-r--r--   0 batty      (501) staff       (20)      147 2023-02-13 13:15:05.000000 autoeap-0.3.1.4/pyproject.toml
+-rw-r--r--   0 batty      (501) staff       (20)      187 2023-02-13 13:11:09.000000 autoeap-0.3.1.4/requirements.txt
+-rw-r--r--   0 batty      (501) staff       (20)       38 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/setup.cfg
+-rw-r--r--   0 batty      (501) staff       (20)     1774 2022-01-18 17:27:57.000000 autoeap-0.3.1.4/setup.py
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/src/
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/src/PDM/
+-rw-r--r--   0 batty      (501) staff       (20)   257562 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/src/PDM/PDM_pyc.c
+-rw-r--r--   0 batty      (501) staff       (20)     3313 2021-10-08 13:32:53.000000 autoeap-0.3.1.4/src/PDM/PDM_pyc.pyx
+-rw-r--r--   0 batty      (501) staff       (20)     6145 2022-03-04 14:09:44.000000 autoeap-0.3.1.4/src/PDM/pdm.c
+-rwxr-xr-x   0 batty      (501) staff       (20)      207 2021-02-28 19:38:35.000000 autoeap-0.3.1.4/src/__init__.py
+-rw-r--r--   0 batty      (501) staff       (20)     2882 2021-11-07 16:12:45.000000 autoeap-0.3.1.4/src/aperture_to_fits.py
+-rwxr-xr-x   0 batty      (501) staff       (20)    82291 2022-05-17 14:27:09.000000 autoeap-0.3.1.4/src/autoeapcore.py
+-rw-r--r--   0 batty      (501) staff       (20)     8943 2023-06-05 10:09:51.000000 autoeap-0.3.1.4/src/detrender.py
+-rw-r--r--   0 batty      (501) staff       (20)    17277 2021-10-08 13:32:53.000000 autoeap-0.3.1.4/src/k2sc_stable.py
+-rwxr-xr-x   0 batty      (501) staff       (20)    61649 2020-11-23 21:12:27.000000 autoeap-0.3.1.4/src/photutils_stable.py
+-rw-r--r--   0 batty      (501) staff       (20)       24 2023-06-05 10:10:21.000000 autoeap-0.3.1.4/src/version.py
+drwxr-xr-x   0 batty      (501) staff       (20)        0 2023-06-05 10:18:57.000000 autoeap-0.3.1.4/tests/
+-rw-r--r--   0 batty      (501) staff       (20)   140920 2021-12-14 17:00:19.000000 autoeap-0.3.1.4/tests/EPIC220198696_c8_autoEAP.lc
+-rw-r--r--   0 batty      (501) staff       (20)    93650 2021-12-14 17:03:00.000000 autoeap-0.3.1.4/tests/EPIC220198696_c8_autoEAP.lc_corr
+-rw-r--r--   0 batty      (501) staff       (20)      535 2021-10-08 13:32:53.000000 autoeap-0.3.1.4/tests/test_detrender.py
+-rw-r--r--   0 batty      (501) staff       (20)      524 2021-10-08 13:32:53.000000 autoeap-0.3.1.4/tests/test_raw_lightcurve.py
```

### Comparing `autoeap-0.3.1.3/.gitignore` & `autoeap-0.3.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/LICENCE` & `autoeap-0.3.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/PKG-INFO` & `autoeap-0.3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoeap
-Version: 0.3.1.3
+Version: 0.3.1.4
 Summary: Automated version of Extended Aperture Photometry developed for high amplitude K2 variable stars.
 Home-page: https://github.com/konkolyseismolab/autoeap/
 Author: Attila Bodi & Pal Szabo
 Author-email: bodi.attila@csfk.org
 License: UNKNOWN
 Description: <div align="center">
         <img src="https://raw.githubusercontent.com/konkolyseismolab/autoeap/master/docs/autoeap_logo.png" width="50%">
```

### Comparing `autoeap-0.3.1.3/README.md` & `autoeap-0.3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/autoeap.egg-info/PKG-INFO` & `autoeap-0.3.1.4/autoeap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoeap
-Version: 0.3.1.3
+Version: 0.3.1.4
 Summary: Automated version of Extended Aperture Photometry developed for high amplitude K2 variable stars.
 Home-page: https://github.com/konkolyseismolab/autoeap/
 Author: Attila Bodi & Pal Szabo
 Author-email: bodi.attila@csfk.org
 License: UNKNOWN
 Description: <div align="center">
         <img src="https://raw.githubusercontent.com/konkolyseismolab/autoeap/master/docs/autoeap_logo.png" width="50%">
```

### Comparing `autoeap-0.3.1.3/autoeap.egg-info/SOURCES.txt` & `autoeap-0.3.1.4/autoeap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/docs/autoeap_logo.png` & `autoeap-0.3.1.4/docs/autoeap_logo.png`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/docs/autoeap_workflow.ipynb` & `autoeap-0.3.1.4/docs/autoeap_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/docs/ktwo212466080-c17_k2sc.jpg` & `autoeap-0.3.1.4/docs/ktwo212466080-c17_k2sc.jpg`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/docs/ktwo212466080-c17_raw.jpg` & `autoeap-0.3.1.4/docs/ktwo212466080-c17_raw.jpg`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/examples/apply_k2sc.ipynb` & `autoeap-0.3.1.4/examples/apply_k2sc.ipynb`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/examples/ktwo212466080-c17_lpd-targ.fits` & `autoeap-0.3.1.4/examples/ktwo212466080-c17_lpd-targ.fits`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/examples/shortest_introduction.ipynb` & `autoeap-0.3.1.4/examples/shortest_introduction.ipynb`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/examples/trend_correction.ipynb` & `autoeap-0.3.1.4/examples/trend_correction.ipynb`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/examples/usage_of_detrender.ipynb` & `autoeap-0.3.1.4/examples/usage_of_detrender.ipynb`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/setup.py` & `autoeap-0.3.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/src/PDM/PDM_pyc.c` & `autoeap-0.3.1.4/src/PDM/PDM_pyc.c`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
             "/Users/batty/opt/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/batty/opt/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/batty/opt/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/batty/opt/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarraytypes.h",
             "/Users/batty/opt/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "/Users/batty/opt/miniconda3/lib/python3.7/site-packages/numpy/core/include",
             "/opt/local/include"
         ],
         "libraries": [
@@ -633,14 +636,17 @@
 
 #define __PYX_HAVE__PDM
 #define __PYX_HAVE_API__PDM
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
@@ -908,195 +914,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":689
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":690
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":691
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":692
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":696
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":697
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":698
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":699
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":703
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":704
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":713
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":714
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":715
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":717
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":718
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":719
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":721
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":722
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":724
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":725
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":726
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1123,42 +1129,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":728
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":729
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":730
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":732
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1628,14 +1634,24 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'PDM' */
 __PYX_EXTERN_C DL_IMPORT(void) pdm_binned_step(double *, double *, double *, double *, double *, int const , int const , float const , int const ); /*proto*/
 __PYX_EXTERN_C DL_IMPORT(void) pdm_binned_linterp(double *, double *, double *, double *, double *, int const , int const , float const , int const ); /*proto*/
 __PYX_EXTERN_C DL_IMPORT(void) pdm_binless_tophat(double *, double *, double *, double *, double *, int const , int const , float const , int const ); /*proto*/
 __PYX_EXTERN_C DL_IMPORT(void) pdm_binless_gauss(double *, double *, double *, double *, double *, int const , int const , float const , int const ); /*proto*/
@@ -1665,15 +1681,14 @@
 static const char __pyx_k_ndata[] = "ndata";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_power[] = "power";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_nfreqs[] = "nfreqs";
 static const char __pyx_k_KeyError[] = "KeyError";
-static const char __pyx_k_floating[] = "floating";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_binned_step[] = "binned_step";
 static const char __pyx_k_binless_gauss[] = "binless_gauss";
 static const char __pyx_k_binless_tophat[] = "binless_tophat";
 static const char __pyx_k_binned_linterp[] = "binned_linterp";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_src_PDM_PDM_pyc_pyx[] = "src/PDM/PDM_pyc.pyx";
@@ -1687,15 +1702,14 @@
 static PyObject *__pyx_n_u_binless_gauss;
 static PyObject *__pyx_n_u_binless_tophat;
 static PyObject *__pyx_n_u_binned_linterp;
 static PyObject *__pyx_n_u_binned_step;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_dphi;
 static PyObject *__pyx_n_s_dtype;
-static PyObject *__pyx_n_s_floating;
 static PyObject *__pyx_n_s_freqs;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_kind;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_nbins;
 static PyObject *__pyx_n_s_ndata;
@@ -1889,23 +1903,22 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyArrayObject *__pyx_t_7 = NULL;
+  PyArrayObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
   int __pyx_t_8;
-  int __pyx_t_9;
+  Py_ssize_t __pyx_t_9;
   Py_ssize_t __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
-  Py_ssize_t __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PDM", 0);
   __pyx_pybuffer_power.pybuffer.buf = NULL;
   __pyx_pybuffer_power.refcount = 0;
   __pyx_pybuffernd_power.data = NULL;
@@ -1990,104 +2003,98 @@
   __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 82, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)__pyx_ptype_5numpy_floating)) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_floating); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 82, __pyx_L1_error)
-  __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_power.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_power.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_power = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_power.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 82, __pyx_L1_error)
     } else {__pyx_pybuffernd_power.diminfo[0].strides = __pyx_pybuffernd_power.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_power.diminfo[0].shape = __pyx_pybuffernd_power.rcbuffer->pybuffer.shape[0];
     }
   }
-  __pyx_t_7 = 0;
-  __pyx_v_power = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
+  __pyx_v_power = ((PyArrayObject *)__pyx_t_5);
+  __pyx_t_5 = 0;
 
   /* "src/PDM/PDM_pyc.pyx":85
  * 
  *     # --- Call C funtion ---
  *     if kind == 'binned_step':             # <<<<<<<<<<<<<<
  *         pdm_binned_step(
  *                 &t[0],
  */
-  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_kind, __pyx_n_u_binned_step, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 85, __pyx_L1_error)
-  __pyx_t_9 = (__pyx_t_8 != 0);
-  if (__pyx_t_9) {
+  __pyx_t_7 = (__Pyx_PyUnicode_Equals(__pyx_v_kind, __pyx_n_u_binned_step, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_8 = (__pyx_t_7 != 0);
+  if (__pyx_t_8) {
 
     /* "src/PDM/PDM_pyc.pyx":87
  *     if kind == 'binned_step':
  *         pdm_binned_step(
  *                 &t[0],             # <<<<<<<<<<<<<<
  *                 &y[0],
  *                 &w[0],
  */
-    __pyx_t_10 = 0;
+    __pyx_t_9 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":88
  *         pdm_binned_step(
  *                 &t[0],
  *                 &y[0],             # <<<<<<<<<<<<<<
  *                 &w[0],
  *                 &freqs[0],
  */
-    __pyx_t_11 = 0;
+    __pyx_t_10 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":89
  *                 &t[0],
  *                 &y[0],
  *                 &w[0],             # <<<<<<<<<<<<<<
  *                 &freqs[0],
  *                 &power[0],
  */
-    __pyx_t_12 = 0;
+    __pyx_t_11 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":90
  *                 &y[0],
  *                 &w[0],
  *                 &freqs[0],             # <<<<<<<<<<<<<<
  *                 &power[0],
  *                 ndata,
  */
-    __pyx_t_13 = 0;
+    __pyx_t_12 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":91
  *                 &w[0],
  *                 &freqs[0],
  *                 &power[0],             # <<<<<<<<<<<<<<
  *                 ndata,
  *                 nfreqs,
  */
-    __pyx_t_14 = 0;
+    __pyx_t_13 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":86
  *     # --- Call C funtion ---
  *     if kind == 'binned_step':
  *         pdm_binned_step(             # <<<<<<<<<<<<<<
  *                 &t[0],
  *                 &y[0],
  */
-    pdm_binned_step((&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_t.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_t.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_y.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_y.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_w.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_w.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_freqs.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_freqs.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_power.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_power.diminfo[0].strides))), __pyx_v_ndata, __pyx_v_nfreqs, __pyx_v_dphi, __pyx_v_nbins);
+    pdm_binned_step((&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_t.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_t.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_y.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_y.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_w.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_w.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_freqs.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_freqs.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_power.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_power.diminfo[0].strides))), __pyx_v_ndata, __pyx_v_nfreqs, __pyx_v_dphi, __pyx_v_nbins);
 
     /* "src/PDM/PDM_pyc.pyx":85
  * 
  *     # --- Call C funtion ---
  *     if kind == 'binned_step':             # <<<<<<<<<<<<<<
  *         pdm_binned_step(
  *                 &t[0],
@@ -2098,71 +2105,71 @@
   /* "src/PDM/PDM_pyc.pyx":96
  *                 dphi,
  *                 nbins)
  *     elif kind == 'binned_linterp':             # <<<<<<<<<<<<<<
  *         pdm_binned_linterp(
  *                 &t[0],
  */
-  __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_kind, __pyx_n_u_binned_linterp, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
-  __pyx_t_8 = (__pyx_t_9 != 0);
-  if (__pyx_t_8) {
+  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_kind, __pyx_n_u_binned_linterp, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_7 = (__pyx_t_8 != 0);
+  if (__pyx_t_7) {
 
     /* "src/PDM/PDM_pyc.pyx":98
  *     elif kind == 'binned_linterp':
  *         pdm_binned_linterp(
  *                 &t[0],             # <<<<<<<<<<<<<<
  *                 &y[0],
  *                 &w[0],
  */
-    __pyx_t_14 = 0;
+    __pyx_t_13 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":99
  *         pdm_binned_linterp(
  *                 &t[0],
  *                 &y[0],             # <<<<<<<<<<<<<<
  *                 &w[0],
  *                 &freqs[0],
  */
-    __pyx_t_13 = 0;
+    __pyx_t_12 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":100
  *                 &t[0],
  *                 &y[0],
  *                 &w[0],             # <<<<<<<<<<<<<<
  *                 &freqs[0],
  *                 &power[0],
  */
-    __pyx_t_12 = 0;
+    __pyx_t_11 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":101
  *                 &y[0],
  *                 &w[0],
  *                 &freqs[0],             # <<<<<<<<<<<<<<
  *                 &power[0],
  *                 ndata,
  */
-    __pyx_t_11 = 0;
+    __pyx_t_10 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":102
  *                 &w[0],
  *                 &freqs[0],
  *                 &power[0],             # <<<<<<<<<<<<<<
  *                 ndata,
  *                 nfreqs,
  */
-    __pyx_t_10 = 0;
+    __pyx_t_9 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":97
  *                 nbins)
  *     elif kind == 'binned_linterp':
  *         pdm_binned_linterp(             # <<<<<<<<<<<<<<
  *                 &t[0],
  *                 &y[0],
  */
-    pdm_binned_linterp((&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_t.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_t.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_y.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_y.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_w.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_w.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_freqs.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_freqs.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_power.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_power.diminfo[0].strides))), __pyx_v_ndata, __pyx_v_nfreqs, __pyx_v_dphi, __pyx_v_nbins);
+    pdm_binned_linterp((&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_t.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_t.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_y.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_y.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_w.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_w.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_freqs.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_freqs.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_power.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_power.diminfo[0].strides))), __pyx_v_ndata, __pyx_v_nfreqs, __pyx_v_dphi, __pyx_v_nbins);
 
     /* "src/PDM/PDM_pyc.pyx":96
  *                 dphi,
  *                 nbins)
  *     elif kind == 'binned_linterp':             # <<<<<<<<<<<<<<
  *         pdm_binned_linterp(
  *                 &t[0],
@@ -2173,71 +2180,71 @@
   /* "src/PDM/PDM_pyc.pyx":107
  *                 dphi,
  *                 nbins)
  *     elif kind == 'binless_tophat':             # <<<<<<<<<<<<<<
  *         pdm_binless_tophat(
  *                 &t[0],
  */
-  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_kind, __pyx_n_u_binless_tophat, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __pyx_t_9 = (__pyx_t_8 != 0);
-  if (__pyx_t_9) {
+  __pyx_t_7 = (__Pyx_PyUnicode_Equals(__pyx_v_kind, __pyx_n_u_binless_tophat, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_8 = (__pyx_t_7 != 0);
+  if (__pyx_t_8) {
 
     /* "src/PDM/PDM_pyc.pyx":109
  *     elif kind == 'binless_tophat':
  *         pdm_binless_tophat(
  *                 &t[0],             # <<<<<<<<<<<<<<
  *                 &y[0],
  *                 &w[0],
  */
-    __pyx_t_10 = 0;
+    __pyx_t_9 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":110
  *         pdm_binless_tophat(
  *                 &t[0],
  *                 &y[0],             # <<<<<<<<<<<<<<
  *                 &w[0],
  *                 &freqs[0],
  */
-    __pyx_t_11 = 0;
+    __pyx_t_10 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":111
  *                 &t[0],
  *                 &y[0],
  *                 &w[0],             # <<<<<<<<<<<<<<
  *                 &freqs[0],
  *                 &power[0],
  */
-    __pyx_t_12 = 0;
+    __pyx_t_11 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":112
  *                 &y[0],
  *                 &w[0],
  *                 &freqs[0],             # <<<<<<<<<<<<<<
  *                 &power[0],
  *                 ndata,
  */
-    __pyx_t_13 = 0;
+    __pyx_t_12 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":113
  *                 &w[0],
  *                 &freqs[0],
  *                 &power[0],             # <<<<<<<<<<<<<<
  *                 ndata,
  *                 nfreqs,
  */
-    __pyx_t_14 = 0;
+    __pyx_t_13 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":108
  *                 nbins)
  *     elif kind == 'binless_tophat':
  *         pdm_binless_tophat(             # <<<<<<<<<<<<<<
  *                 &t[0],
  *                 &y[0],
  */
-    pdm_binless_tophat((&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_t.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_t.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_y.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_y.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_w.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_w.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_freqs.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_freqs.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_power.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_power.diminfo[0].strides))), __pyx_v_ndata, __pyx_v_nfreqs, __pyx_v_dphi, __pyx_v_nbins);
+    pdm_binless_tophat((&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_t.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_t.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_y.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_y.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_w.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_w.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_freqs.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_freqs.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_power.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_power.diminfo[0].strides))), __pyx_v_ndata, __pyx_v_nfreqs, __pyx_v_dphi, __pyx_v_nbins);
 
     /* "src/PDM/PDM_pyc.pyx":107
  *                 dphi,
  *                 nbins)
  *     elif kind == 'binless_tophat':             # <<<<<<<<<<<<<<
  *         pdm_binless_tophat(
  *                 &t[0],
@@ -2248,71 +2255,71 @@
   /* "src/PDM/PDM_pyc.pyx":118
  *                 dphi,
  *                 nbins)
  *     elif kind == 'binless_gauss':             # <<<<<<<<<<<<<<
  *         pdm_binless_gauss(
  *                 &t[0],
  */
-  __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_v_kind, __pyx_n_u_binless_gauss, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
-  __pyx_t_8 = (__pyx_t_9 != 0);
-  if (likely(__pyx_t_8)) {
+  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_kind, __pyx_n_u_binless_gauss, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_7 = (__pyx_t_8 != 0);
+  if (likely(__pyx_t_7)) {
 
     /* "src/PDM/PDM_pyc.pyx":120
  *     elif kind == 'binless_gauss':
  *         pdm_binless_gauss(
  *                 &t[0],             # <<<<<<<<<<<<<<
  *                 &y[0],
  *                 &w[0],
  */
-    __pyx_t_14 = 0;
+    __pyx_t_13 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":121
  *         pdm_binless_gauss(
  *                 &t[0],
  *                 &y[0],             # <<<<<<<<<<<<<<
  *                 &w[0],
  *                 &freqs[0],
  */
-    __pyx_t_13 = 0;
+    __pyx_t_12 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":122
  *                 &t[0],
  *                 &y[0],
  *                 &w[0],             # <<<<<<<<<<<<<<
  *                 &freqs[0],
  *                 &power[0],
  */
-    __pyx_t_12 = 0;
+    __pyx_t_11 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":123
  *                 &y[0],
  *                 &w[0],
  *                 &freqs[0],             # <<<<<<<<<<<<<<
  *                 &power[0],
  *                 ndata,
  */
-    __pyx_t_11 = 0;
+    __pyx_t_10 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":124
  *                 &w[0],
  *                 &freqs[0],
  *                 &power[0],             # <<<<<<<<<<<<<<
  *                 ndata,
  *                 nfreqs,
  */
-    __pyx_t_10 = 0;
+    __pyx_t_9 = 0;
 
     /* "src/PDM/PDM_pyc.pyx":119
  *                 nbins)
  *     elif kind == 'binless_gauss':
  *         pdm_binless_gauss(             # <<<<<<<<<<<<<<
  *                 &t[0],
  *                 &y[0],
  */
-    pdm_binless_gauss((&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_t.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_t.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_y.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_y.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_w.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_w.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_freqs.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_freqs.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_power.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_power.diminfo[0].strides))), __pyx_v_ndata, __pyx_v_nfreqs, __pyx_v_dphi, __pyx_v_nbins);
+    pdm_binless_gauss((&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_t.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_t.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_y.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_y.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_w.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_w.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_freqs.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_freqs.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_float_t *, __pyx_pybuffernd_power.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_power.diminfo[0].strides))), __pyx_v_ndata, __pyx_v_nfreqs, __pyx_v_dphi, __pyx_v_nbins);
 
     /* "src/PDM/PDM_pyc.pyx":118
  *                 dphi,
  *                 nbins)
  *     elif kind == 'binless_gauss':             # <<<<<<<<<<<<<<
  *         pdm_binless_gauss(
  *                 &t[0],
@@ -2324,18 +2331,18 @@
  *                 nbins)
  *     else:
  *         raise KeyError('Function not available. Please use one of the followings: ' + \             # <<<<<<<<<<<<<<
  *                             'binless_tophat, binless_gauss, binned_linterp, binned_step')
  * 
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_KeyError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_Raise(__pyx_t_6, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_KeyError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_Raise(__pyx_t_5, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __PYX_ERR(0, 130, __pyx_L1_error)
   }
   __pyx_L3:;
 
   /* "src/PDM/PDM_pyc.pyx":133
  *                             'binless_tophat, binless_gauss, binned_linterp, binned_step')
  * 
@@ -2356,15 +2363,14 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_freqs.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_power.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_t.rcbuffer->pybuffer);
@@ -2383,15 +2389,15 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_power);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":734
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2400,29 +2406,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":734
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2433,15 +2439,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":737
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2450,29 +2456,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":737
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2483,15 +2489,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":740
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2500,29 +2506,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":740
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2533,15 +2539,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":743
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2550,29 +2556,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":743
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2583,15 +2589,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":746
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2600,29 +2606,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":746
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2633,212 +2639,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":749
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":753
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":749
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":868
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":869
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":870
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":868
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":872
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":873
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":874
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":875
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":874
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":876
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":872
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":880
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2854,15 +2860,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":881
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -2870,84 +2876,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":882
+      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":881
+      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":883
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":884
+      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 884, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":881
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":880
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2962,15 +2968,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":886
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2986,15 +2992,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":887
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3002,84 +3008,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":888
+      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":887
+      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":889
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":890
+      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 890, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":887
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":886
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3094,15 +3100,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":892
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3118,15 +3124,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":893
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3134,84 +3140,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":894
+      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":893
+      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":895
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":896
+      /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 896, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":893
+    /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":892
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3226,14 +3232,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
@@ -3283,15 +3463,14 @@
   {&__pyx_n_u_binless_gauss, __pyx_k_binless_gauss, sizeof(__pyx_k_binless_gauss), 0, 1, 0, 1},
   {&__pyx_n_u_binless_tophat, __pyx_k_binless_tophat, sizeof(__pyx_k_binless_tophat), 0, 1, 0, 1},
   {&__pyx_n_u_binned_linterp, __pyx_k_binned_linterp, sizeof(__pyx_k_binned_linterp), 0, 1, 0, 1},
   {&__pyx_n_u_binned_step, __pyx_k_binned_step, sizeof(__pyx_k_binned_step), 0, 1, 0, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_dphi, __pyx_k_dphi, sizeof(__pyx_k_dphi), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
-  {&__pyx_n_s_floating, __pyx_k_floating, sizeof(__pyx_k_floating), 0, 0, 1, 1},
   {&__pyx_n_s_freqs, __pyx_k_freqs, sizeof(__pyx_k_freqs), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_kind, __pyx_k_kind, sizeof(__pyx_k_kind), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_nbins, __pyx_k_nbins, sizeof(__pyx_k_nbins), 0, 0, 1, 1},
   {&__pyx_n_s_ndata, __pyx_k_ndata, sizeof(__pyx_k_ndata), 0, 0, 1, 1},
@@ -3308,15 +3487,15 @@
   {&__pyx_n_s_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 0, 1, 1},
   {&__pyx_n_s_y, __pyx_k_y, sizeof(__pyx_k_y), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 130, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -3329,33 +3508,33 @@
  *                             'binless_tophat, binless_gauss, binned_linterp, binned_step')
  * 
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Function_not_available_Please_us); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":884
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 884, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":890
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 890, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "src/PDM/PDM_pyc.pyx":56
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def PDM(    np.ndarray[np.double_t, ndim=1, mode="c"] t not None,             # <<<<<<<<<<<<<<
@@ -3435,26 +3614,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -3708,20 +3907,20 @@
  * # Version: 0.1  2021APR01
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":892
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../opt/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
  * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
```

### Comparing `autoeap-0.3.1.3/src/PDM/PDM_pyc.pyx` & `autoeap-0.3.1.4/src/PDM/PDM_pyc.pyx`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/src/PDM/pdm.c` & `autoeap-0.3.1.4/src/PDM/pdm.c`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/src/aperture_to_fits.py` & `autoeap-0.3.1.4/src/aperture_to_fits.py`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/src/autoeapcore.py` & `autoeap-0.3.1.4/src/autoeapcore.py`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/src/detrender.py` & `autoeap-0.3.1.4/src/detrender.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,28 +97,35 @@
         plt.plot(x,cos_trend,c='C1')
         plt.show()
         plt.close()
 
     return  goodpts
 
 
-def detrend_wrt_PDM(time,flux,fluxerr,polyorder='auto',sigma=10,show_plots=False,save_plots=False,filename=None,debug=False):
+def detrend_wrt_PDM(time,flux,fluxerr,polyorder='auto',sigma=10,period=None,show_plots=False,save_plots=False,filename=None,debug=False):
     """
     Deterending with a polynomial that is fitted w.r.t. phase dispersion minimization.
 
     Parameters
     ----------
     time : array-like
         Time values.
     flux : array-like
         Corresponding flux values.
     fluxerr : array-like
         Corresponding flux errors.
     polyorder : int , default : 9
         The order of the detrending polynomial.
+    sigma : float, default : 10
+        The number of standard deviations to use for sigma
+        clipping limit before spline correction.
+    period : float, optional
+        The period, which is used to phase fold
+        the light curve. If not given, the period
+        is derived using a Lomb-Scargle periodogram.
     show_plots: bool, default: False
         If `True` the plot will be displayed.
     save_plots: bool, default: False
         If `True` the plot will be saved to a subdirectory.
     filename : string
         If `save_plots` is `True`, the name of the output PNG file,
         without extension.
@@ -155,33 +162,36 @@
 
     # Keep only good points
     x = x[goodpts]
     y = y[goodpts]
     err = err[goodpts]
 
     # Get period
-    lsfreqs,lspow = LombScargle(x,y).autopower(nyquist_factor=1,samples_per_peak=50,minimum_frequency=0.05)
-    testf = lsfreqs[np.argmax(lspow)]
-
-    # If test period is larger than data length, remove linear
-    if testf <= 1/np.ptp(x):
-        y -= np.poly1d(np.polyfit(x,y,1))(x)
-
-        lsfreqs,lspow = LombScargle(x,y).autopower(normalization='psd',
-                                                nyquist_factor=1,
-                                                minimum_frequency=0.05,
-                                                samples_per_peak=50)
-
+    if period is None:
+        lsfreqs,lspow = LombScargle(x,y).autopower(nyquist_factor=1,samples_per_peak=50,minimum_frequency=0.05)
         testf = lsfreqs[np.argmax(lspow)]
 
-        # If period is still larger than data length
+        # If test period is larger than data length, remove linear
         if testf <= 1/np.ptp(x):
-            testf = 1/np.ptp(x)
+            y -= np.poly1d(np.polyfit(x,y,1))(x)
 
-    del lsfreqs,lspow
+            lsfreqs,lspow = LombScargle(x,y).autopower(normalization='psd',
+                                                    nyquist_factor=1,
+                                                    minimum_frequency=0.05,
+                                                    samples_per_peak=50)
+
+            testf = lsfreqs[np.argmax(lspow)]
+
+            # If period is still larger than data length
+            if testf <= 1/np.ptp(x):
+                testf = 1/np.ptp(x)
+
+        del lsfreqs,lspow
+    else:
+        testf = 1/period
 
     if debug:
         print('Best period is', round(1/testf,8),'days' )
 
         fig,ax = plt.subplots(1,2,figsize=(14,5))
         ax[1].plot( (x*testf)%1, y, '.', ms=2)
         ax[0].plot( x, y, '.', ms=2)
```

### Comparing `autoeap-0.3.1.3/src/k2sc_stable.py` & `autoeap-0.3.1.4/src/k2sc_stable.py`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/src/photutils_stable.py` & `autoeap-0.3.1.4/src/photutils_stable.py`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/tests/EPIC220198696_c8_autoEAP.lc` & `autoeap-0.3.1.4/tests/EPIC220198696_c8_autoEAP.lc`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/tests/EPIC220198696_c8_autoEAP.lc_corr` & `autoeap-0.3.1.4/tests/EPIC220198696_c8_autoEAP.lc_corr`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/tests/test_detrender.py` & `autoeap-0.3.1.4/tests/test_detrender.py`

 * *Files identical despite different names*

### Comparing `autoeap-0.3.1.3/tests/test_raw_lightcurve.py` & `autoeap-0.3.1.4/tests/test_raw_lightcurve.py`

 * *Files identical despite different names*

