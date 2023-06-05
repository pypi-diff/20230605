# Comparing `tmp/boundaryscheme-1.0.tar.gz` & `tmp/boundaryscheme-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/boundaryscheme-1.0.tar", last modified: Mon Jun  5 13:29:48 2023, max compression
+gzip compressed data, was "dist/boundaryscheme-2.1.tar", last modified: Mon Jun  5 13:40:12 2023, max compression
```

## Comparing `boundaryscheme-1.0.tar` & `boundaryscheme-2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:29:48.000000 boundaryscheme-1.0/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1891 2023-06-05 13:29:48.000000 boundaryscheme-1.0/PKG-INFO
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:29:48.000000 boundaryscheme-1.0/tests/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 07:50:58.000000 boundaryscheme-1.0/tests/__init__.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       61 2023-06-05 07:51:32.000000 boundaryscheme-1.0/tests/test_import.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:29:48.000000 boundaryscheme-1.0/boundaryscheme.egg-info/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1891 2023-06-05 13:29:48.000000 boundaryscheme-1.0/boundaryscheme.egg-info/PKG-INFO
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      522 2023-06-05 13:29:48.000000 boundaryscheme-1.0/boundaryscheme.egg-info/SOURCES.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       29 2023-06-05 13:29:48.000000 boundaryscheme-1.0/boundaryscheme.egg-info/requires.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       30 2023-06-05 13:29:48.000000 boundaryscheme-1.0/boundaryscheme.egg-info/top_level.txt
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        1 2023-06-05 13:29:48.000000 boundaryscheme-1.0/boundaryscheme.egg-info/dependency_links.txt
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     1247 2023-05-31 13:02:22.000000 boundaryscheme-1.0/README.md
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      940 2023-06-05 13:29:30.000000 boundaryscheme-1.0/setup.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:29:48.000000 boundaryscheme-1.0/examples/
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-05-16 09:26:00.000000 boundaryscheme-1.0/examples/__init__.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1995 2023-06-04 15:20:10.000000 boundaryscheme-1.0/examples/draw_detKLcurve.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1401 2023-05-31 17:06:49.000000 boundaryscheme-1.0/examples/draw_nbrzerosdetKL.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      925 2023-05-31 17:06:37.000000 boundaryscheme-1.0/examples/draw_symbol.py
-drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:29:48.000000 boundaryscheme-1.0/boundaryscheme/
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     6390 2023-06-04 15:21:00.000000 boundaryscheme-1.0/boundaryscheme/boundaries.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      137 2023-05-16 09:27:39.000000 boundaryscheme-1.0/boundaryscheme/__init__.py
--rwxrwxrwx   0 pierrelebarbenchon   (501) staff       (20)    10942 2023-06-05 07:45:15.000000 boundaryscheme-1.0/boundaryscheme/utils.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)    20955 2023-06-05 07:40:10.000000 boundaryscheme-1.0/boundaryscheme/schemes.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2605 2023-01-16 09:04:43.000000 boundaryscheme-1.0/boundaryscheme/complex_winding_number.py
--rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)    23173 2023-06-04 15:21:40.000000 boundaryscheme-1.0/boundaryscheme/pyplot.py
--rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       38 2023-06-05 13:29:48.000000 boundaryscheme-1.0/setup.cfg
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1833 2023-06-05 13:40:12.000000 boundaryscheme-2.1/PKG-INFO
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/tests/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 07:50:58.000000 boundaryscheme-2.1/tests/__init__.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       61 2023-06-05 07:51:32.000000 boundaryscheme-2.1/tests/test_import.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1833 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/PKG-INFO
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      522 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/SOURCES.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       29 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/requires.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       30 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/top_level.txt
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        1 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme.egg-info/dependency_links.txt
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     1221 2023-06-05 13:37:51.000000 boundaryscheme-2.1/README.md
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      940 2023-06-05 13:29:30.000000 boundaryscheme-2.1/setup.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/examples/
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)        0 2023-05-16 09:26:00.000000 boundaryscheme-2.1/examples/__init__.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1995 2023-06-04 15:20:10.000000 boundaryscheme-2.1/examples/draw_detKLcurve.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     1401 2023-05-31 17:06:49.000000 boundaryscheme-2.1/examples/draw_nbrzerosdetKL.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      925 2023-05-31 17:06:37.000000 boundaryscheme-2.1/examples/draw_symbol.py
+drwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)        0 2023-06-05 13:40:12.000000 boundaryscheme-2.1/boundaryscheme/
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)     6390 2023-06-04 15:21:00.000000 boundaryscheme-2.1/boundaryscheme/boundaries.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)      137 2023-06-05 13:39:33.000000 boundaryscheme-2.1/boundaryscheme/__init__.py
+-rwxrwxrwx   0 pierrelebarbenchon   (501) staff       (20)    10942 2023-06-05 07:45:15.000000 boundaryscheme-2.1/boundaryscheme/utils.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)    20955 2023-06-05 07:40:10.000000 boundaryscheme-2.1/boundaryscheme/schemes.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)     2605 2023-01-16 09:04:43.000000 boundaryscheme-2.1/boundaryscheme/complex_winding_number.py
+-rwxr-xr-x   0 pierrelebarbenchon   (501) staff       (20)    23173 2023-06-04 15:21:40.000000 boundaryscheme-2.1/boundaryscheme/pyplot.py
+-rw-r--r--   0 pierrelebarbenchon   (501) staff       (20)       38 2023-06-05 13:40:12.000000 boundaryscheme-2.1/setup.cfg
```

### Comparing `boundaryscheme-1.0/PKG-INFO` & `boundaryscheme-2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: boundaryscheme
-Version: 1.0
+Version: 2.1
 Summary: This library implements Kreiss-Lopatinskii determinant for numerical scheme with boundary
 Home-page: UNKNOWN
 Author: Pierre Le Barbenchon
 License: UNKNOWN
 Description: This is the architecture for the package "boundaryscheme" 
         
         
         # boundaryscheme
         Package Python to use numerical scheme with boundaries which is described in the PhD manuscript 
         > P. Le Barbenchon, Étude théorique et numérique de la stabilité GKS pour des schémas d'ordre élevé en présence de bords, PhD, 2023.
         
+        # Documentations du package
+        
+        https://plebarbenchon.github.io/boundaryscheme
+        
         # Installation
         ```bash
         git clone https://github.com/PLeBarbenchon/boundaryscheme.git
         cd boundaryscheme
         pip3 install -r requirements.txt
         pip3 install -e .
         python3 examples/draw_detKLcurve.py
@@ -31,22 +35,14 @@
         
         bsplt.detKLcurve(BeamWarming, SILW(2,3),lambdacursor = True)
         plt.show()
         ```
         
         ![mygif](https://github.com/PLeBarbenchon/boundaryscheme/assets/92107096/2ca0d414-77a6-410e-a582-a3950699dcf0)
         
-        # Plot a Kreiss--Lopatinskii determinant curve
-        
-        à écrire
-        
-        # Create a scheme
-        
-        In schemes.py, create 
-        
         # Citing
         
         The code is citable via Zenodo. Please cite as:
         
         P. Le Barbenchon, boundaryscheme: package Python for numerical schemes with boundaries. 2023. [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7773742.svg)](https://doi.org/10.5281/zenodo.7773742)
```

### Comparing `boundaryscheme-1.0/boundaryscheme.egg-info/PKG-INFO` & `boundaryscheme-2.1/boundaryscheme.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: boundaryscheme
-Version: 1.0
+Version: 2.1
 Summary: This library implements Kreiss-Lopatinskii determinant for numerical scheme with boundary
 Home-page: UNKNOWN
 Author: Pierre Le Barbenchon
 License: UNKNOWN
 Description: This is the architecture for the package "boundaryscheme" 
         
         
         # boundaryscheme
         Package Python to use numerical scheme with boundaries which is described in the PhD manuscript 
         > P. Le Barbenchon, Étude théorique et numérique de la stabilité GKS pour des schémas d'ordre élevé en présence de bords, PhD, 2023.
         
+        # Documentations du package
+        
+        https://plebarbenchon.github.io/boundaryscheme
+        
         # Installation
         ```bash
         git clone https://github.com/PLeBarbenchon/boundaryscheme.git
         cd boundaryscheme
         pip3 install -r requirements.txt
         pip3 install -e .
         python3 examples/draw_detKLcurve.py
@@ -31,22 +35,14 @@
         
         bsplt.detKLcurve(BeamWarming, SILW(2,3),lambdacursor = True)
         plt.show()
         ```
         
         ![mygif](https://github.com/PLeBarbenchon/boundaryscheme/assets/92107096/2ca0d414-77a6-410e-a582-a3950699dcf0)
         
-        # Plot a Kreiss--Lopatinskii determinant curve
-        
-        à écrire
-        
-        # Create a scheme
-        
-        In schemes.py, create 
-        
         # Citing
         
         The code is citable via Zenodo. Please cite as:
         
         P. Le Barbenchon, boundaryscheme: package Python for numerical schemes with boundaries. 2023. [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7773742.svg)](https://doi.org/10.5281/zenodo.7773742)
```

### Comparing `boundaryscheme-1.0/boundaryscheme.egg-info/SOURCES.txt` & `boundaryscheme-2.1/boundaryscheme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boundaryscheme-1.0/README.md` & `boundaryscheme-2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 This is the architecture for the package "boundaryscheme" 
 
 
 # boundaryscheme
 Package Python to use numerical scheme with boundaries which is described in the PhD manuscript 
 > P. Le Barbenchon, Étude théorique et numérique de la stabilité GKS pour des schémas d'ordre élevé en présence de bords, PhD, 2023.
 
+# Documentations du package
+
+https://plebarbenchon.github.io/boundaryscheme
+
 # Installation
 ```bash
 git clone https://github.com/PLeBarbenchon/boundaryscheme.git
 cd boundaryscheme
 pip3 install -r requirements.txt
 pip3 install -e .
 python3 examples/draw_detKLcurve.py
@@ -24,21 +28,13 @@
 
 bsplt.detKLcurve(BeamWarming, SILW(2,3),lambdacursor = True)
 plt.show()
 ```
 
 ![mygif](https://github.com/PLeBarbenchon/boundaryscheme/assets/92107096/2ca0d414-77a6-410e-a582-a3950699dcf0)
 
-# Plot a Kreiss--Lopatinskii determinant curve
-
-à écrire
-
-# Create a scheme
-
-In schemes.py, create 
-
 # Citing
 
 The code is citable via Zenodo. Please cite as:
 
 P. Le Barbenchon, boundaryscheme: package Python for numerical schemes with boundaries. 2023. [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7773742.svg)](https://doi.org/10.5281/zenodo.7773742)
```

### Comparing `boundaryscheme-1.0/setup.py` & `boundaryscheme-2.1/setup.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-1.0/examples/draw_detKLcurve.py` & `boundaryscheme-2.1/examples/draw_detKLcurve.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-1.0/examples/draw_nbrzerosdetKL.py` & `boundaryscheme-2.1/examples/draw_nbrzerosdetKL.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-1.0/examples/draw_symbol.py` & `boundaryscheme-2.1/examples/draw_symbol.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-1.0/boundaryscheme/boundaries.py` & `boundaryscheme-2.1/boundaryscheme/boundaries.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-1.0/boundaryscheme/utils.py` & `boundaryscheme-2.1/boundaryscheme/utils.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-1.0/boundaryscheme/schemes.py` & `boundaryscheme-2.1/boundaryscheme/schemes.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-1.0/boundaryscheme/complex_winding_number.py` & `boundaryscheme-2.1/boundaryscheme/complex_winding_number.py`

 * *Files identical despite different names*

### Comparing `boundaryscheme-1.0/boundaryscheme/pyplot.py` & `boundaryscheme-2.1/boundaryscheme/pyplot.py`

 * *Files identical despite different names*

