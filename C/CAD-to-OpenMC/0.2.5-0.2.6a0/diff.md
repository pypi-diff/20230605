# Comparing `tmp/CAD_to_OpenMC-0.2.5.tar.gz` & `tmp/CAD_to_OpenMC-0.2.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CAD_to_OpenMC-0.2.5.tar", last modified: Tue Apr  4 09:37:02 2023, max compression
+gzip compressed data, was "CAD_to_OpenMC-0.2.6a0.tar", last modified: Mon Jun  5 15:58:24 2023, max compression
```

## Comparing `CAD_to_OpenMC-0.2.5.tar` & `CAD_to_OpenMC-0.2.6a0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-04-04 09:37:02.925749 CAD_to_OpenMC-0.2.5/
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1071 2022-04-21 08:49:34.000000 CAD_to_OpenMC-0.2.5/LICENSE
--rw-r--r--   0 erkn      (1000) erkn      (1000)     8588 2023-04-04 09:37:02.925749 CAD_to_OpenMC-0.2.5/PKG-INFO
--rw-r--r--   0 erkn      (1000) erkn      (1000)     7993 2023-03-28 11:26:13.000000 CAD_to_OpenMC-0.2.5/README.md
--rw-r--r--   0 erkn      (1000) erkn      (1000)      901 2023-04-04 09:36:13.000000 CAD_to_OpenMC-0.2.5/pyproject.toml
--rw-r--r--   0 erkn      (1000) erkn      (1000)       38 2023-04-04 09:37:02.925749 CAD_to_OpenMC-0.2.5/setup.cfg
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-04-04 09:37:02.812416 CAD_to_OpenMC-0.2.5/src/
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-04-04 09:37:02.889082 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/
--rw-r--r--   0 erkn      (1000) erkn      (1000)      610 2023-03-24 12:54:20.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/__init__.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)    26695 2023-03-28 11:28:50.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/assembly.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      404 2023-03-27 16:57:21.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/assemblymesher.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      203 2023-03-28 11:28:50.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/assemblymesher_base.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     5941 2023-03-28 11:28:50.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/assemblymesher_cq.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     6496 2023-03-28 11:28:50.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/assemblymesher_gmsh.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     3307 2023-03-27 17:00:11.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/meshutils.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      329 2022-08-23 06:16:29.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/object_factory.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     4131 2023-03-27 17:00:08.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/stl_utils.py
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-04-04 09:37:02.899082 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC.egg-info/
--rw-r--r--   0 erkn      (1000) erkn      (1000)     8588 2023-04-04 09:37:02.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC.egg-info/PKG-INFO
--rw-r--r--   0 erkn      (1000) erkn      (1000)      629 2023-04-04 09:37:02.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC.egg-info/SOURCES.txt
--rw-r--r--   0 erkn      (1000) erkn      (1000)        1 2023-04-04 09:37:02.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC.egg-info/dependency_links.txt
--rw-r--r--   0 erkn      (1000) erkn      (1000)      110 2023-04-04 09:37:02.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC.egg-info/requires.txt
--rw-r--r--   0 erkn      (1000) erkn      (1000)       14 2023-04-04 09:37:02.000000 CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC.egg-info/top_level.txt
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-04-04 09:37:02.922416 CAD_to_OpenMC-0.2.5/tests/
--rw-r--r--   0 erkn      (1000) erkn      (1000)      884 2023-03-28 08:41:37.000000 CAD_to_OpenMC-0.2.5/tests/testRun.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      674 2023-03-28 08:41:56.000000 CAD_to_OpenMC-0.2.5/tests/test_cqstl.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)      485 2023-03-24 12:54:20.000000 CAD_to_OpenMC-0.2.5/tests/test_gmsh.py
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1045 2023-01-25 15:31:23.000000 CAD_to_OpenMC-0.2.5/tests/test_wOpenMC.py
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-06-05 15:58:24.486061 CAD_to_OpenMC-0.2.6a0/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1071 2022-04-21 08:49:34.000000 CAD_to_OpenMC-0.2.6a0/LICENSE
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     8668 2023-06-05 15:58:24.486061 CAD_to_OpenMC-0.2.6a0/PKG-INFO
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     7993 2023-04-20 15:34:44.000000 CAD_to_OpenMC-0.2.6a0/README.md
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      945 2023-06-05 15:38:06.000000 CAD_to_OpenMC-0.2.6a0/pyproject.toml
+-rw-r--r--   0 erkn      (1000) erkn      (1000)       38 2023-06-05 15:58:24.486061 CAD_to_OpenMC-0.2.6a0/setup.cfg
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-06-05 15:58:24.482728 CAD_to_OpenMC-0.2.6a0/src/
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-06-05 15:58:24.482728 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      610 2023-04-17 16:03:40.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/__init__.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)    26695 2023-06-05 15:30:24.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/assembly.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      404 2023-06-05 15:30:24.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/assemblymesher.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      203 2023-04-20 15:35:11.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/assemblymesher_base.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     5941 2023-06-05 15:30:24.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/assemblymesher_cq.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     6496 2023-04-20 15:35:11.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/assemblymesher_gmsh.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     3307 2023-04-17 16:03:40.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/meshutils.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      329 2022-08-23 06:16:29.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/object_factory.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     4131 2023-04-17 16:03:40.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/stl_utils.py
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-06-05 15:58:24.486061 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC.egg-info/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     8668 2023-06-05 15:58:24.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC.egg-info/PKG-INFO
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      650 2023-06-05 15:58:24.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC.egg-info/SOURCES.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)        1 2023-06-05 15:58:24.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC.egg-info/dependency_links.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)       84 2023-06-05 15:58:24.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC.egg-info/requires.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)       14 2023-06-05 15:58:24.000000 CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC.egg-info/top_level.txt
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-06-05 15:58:24.486061 CAD_to_OpenMC-0.2.6a0/tests/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      884 2023-04-26 10:19:25.000000 CAD_to_OpenMC-0.2.6a0/tests/testRun.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      674 2023-06-05 15:30:24.000000 CAD_to_OpenMC-0.2.6a0/tests/test_cqstl.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      785 2023-04-26 10:10:54.000000 CAD_to_OpenMC-0.2.6a0/tests/test_cqstl2.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      485 2023-06-05 15:30:24.000000 CAD_to_OpenMC-0.2.6a0/tests/test_gmsh.py
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1045 2023-01-25 15:31:23.000000 CAD_to_OpenMC-0.2.6a0/tests/test_wOpenMC.py
```

### Comparing `CAD_to_OpenMC-0.2.5/LICENSE` & `CAD_to_OpenMC-0.2.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/PKG-INFO` & `CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
-Name: CAD_to_OpenMC
-Version: 0.2.5
+Name: CAD-to-OpenMC
+Version: 0.2.6a0
 Summary: Package to automagically convert step-gometries to h5m descriptions for neutronics by OpenMC
 Author-email: Erik B Knudsen <erik.knudsen@copenhagenatomics.com>
 Project-URL: Homepage, https://github.com/openmsr/CAD_to_OpenMC
 Project-URL: Bug Tracker, https://github.com/openmsr/CAD_to_OpenMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python application](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)
 
 # CAD_to_OpenMC
```

### Comparing `CAD_to_OpenMC-0.2.5/README.md` & `CAD_to_OpenMC-0.2.6a0/README.md`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/pyproject.toml` & `CAD_to_OpenMC-0.2.6a0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [project]
 name="CAD_to_OpenMC"
-version="0.2.5"
+version="0.2.6a0"
 authors = [
   { name="Erik B Knudsen", email="erik.knudsen@copenhagenatomics.com" },
 ]
 description = "Package to automagically convert step-gometries to h5m descriptions for neutronics by OpenMC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Development Status :: 4 - Beta",
+    "Environment :: Console",
 ]
 dependencies=[
         'gmsh',
-        'pyparsing==2.4',
-        'cadquery==2.2.0b2',
-        'cadquery-ocp==7.6.3a0',
+        'pyparsing',
+        'cadquery>=2',
+        'cadquery-ocp>=7',
         'numpy',
         'OCP',
         'meshio',
         'trimesh',
         'networkx',
-        'Cython==0.29.32'
+        'Cython'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/openmsr/CAD_to_OpenMC"
 "Bug Tracker" = "https://github.com/openmsr/CAD_to_OpenMC/issues"
 
 [build-system]
```

### Comparing `CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/__init__.py` & `CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/__init__.py`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/assembly.py` & `CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/assembly.py`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/assemblymesher_cq.py` & `CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/assemblymesher_cq.py`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/assemblymesher_gmsh.py` & `CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/assemblymesher_gmsh.py`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/meshutils.py` & `CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/meshutils.py`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC/stl_utils.py` & `CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC/stl_utils.py`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC.egg-info/PKG-INFO` & `CAD_to_OpenMC-0.2.6a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
-Name: CAD-to-OpenMC
-Version: 0.2.5
+Name: CAD_to_OpenMC
+Version: 0.2.6a0
 Summary: Package to automagically convert step-gometries to h5m descriptions for neutronics by OpenMC
 Author-email: Erik B Knudsen <erik.knudsen@copenhagenatomics.com>
 Project-URL: Homepage, https://github.com/openmsr/CAD_to_OpenMC
 Project-URL: Bug Tracker, https://github.com/openmsr/CAD_to_OpenMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python application](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml/badge.svg)](https://github.com/openmsr/CAD_to_OpenMC/actions/workflows/python-app.yml)
 
 # CAD_to_OpenMC
```

### Comparing `CAD_to_OpenMC-0.2.5/src/CAD_to_OpenMC.egg-info/SOURCES.txt` & `CAD_to_OpenMC-0.2.6a0/src/CAD_to_OpenMC.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 src/CAD_to_OpenMC.egg-info/PKG-INFO
 src/CAD_to_OpenMC.egg-info/SOURCES.txt
 src/CAD_to_OpenMC.egg-info/dependency_links.txt
 src/CAD_to_OpenMC.egg-info/requires.txt
 src/CAD_to_OpenMC.egg-info/top_level.txt
 tests/testRun.py
 tests/test_cqstl.py
+tests/test_cqstl2.py
 tests/test_gmsh.py
 tests/test_wOpenMC.py
```

### Comparing `CAD_to_OpenMC-0.2.5/tests/testRun.py` & `CAD_to_OpenMC-0.2.6a0/tests/testRun.py`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/tests/test_cqstl.py` & `CAD_to_OpenMC-0.2.6a0/tests/test_cqstl.py`

 * *Files identical despite different names*

### Comparing `CAD_to_OpenMC-0.2.5/tests/test_wOpenMC.py` & `CAD_to_OpenMC-0.2.6a0/tests/test_wOpenMC.py`

 * *Files identical despite different names*

