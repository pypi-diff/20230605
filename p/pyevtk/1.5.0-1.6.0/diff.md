# Comparing `tmp/pyevtk-1.5.0.tar.gz` & `tmp/pyevtk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevtk-1.5.0.tar", last modified: Fri Apr  8 09:12:52 2022, max compression
+gzip compressed data, was "pyevtk-1.6.0.tar", last modified: Mon Jun  5 15:25:14 2023, max compression
```

## Comparing `pyevtk-1.5.0.tar` & `pyevtk-1.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:12:52.641723 pyevtk-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-04-08 09:12:40.000000 pyevtk-1.5.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-04-08 09:12:40.000000 pyevtk-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-04-08 09:12:40.000000 pyevtk-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5358 2022-04-08 09:12:52.641723 pyevtk-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4780 2022-04-08 09:12:40.000000 pyevtk-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:12:52.641723 pyevtk-1.5.0/evtk/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-04-08 09:12:40.000000 pyevtk-1.5.0/evtk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:12:52.641723 pyevtk-1.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2608 2022-04-08 09:12:40.000000 pyevtk-1.5.0/examples/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-04-08 09:12:40.000000 pyevtk-1.5.0/examples/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-04-08 09:12:40.000000 pyevtk-1.5.0/examples/lines.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-04-08 09:12:40.000000 pyevtk-1.5.0/examples/lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-04-08 09:12:40.000000 pyevtk-1.5.0/examples/points.py
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-04-08 09:12:40.000000 pyevtk-1.5.0/examples/poly_lines.py
--rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-04-08 09:12:40.000000 pyevtk-1.5.0/examples/rectilinear.py
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-04-08 09:12:40.000000 pyevtk-1.5.0/examples/structured.py
--rw-r--r--   0 runner    (1001) docker     (121)     3838 2022-04-08 09:12:40.000000 pyevtk-1.5.0/examples/unstructured.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:12:52.641723 pyevtk-1.5.0/pyevtk/
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-04-08 09:12:40.000000 pyevtk-1.5.0/pyevtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-04-08 09:12:52.641723 pyevtk-1.5.0/pyevtk/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5277 2022-04-08 09:12:40.000000 pyevtk-1.5.0/pyevtk/evtk.py
--rw-r--r--   0 runner    (1001) docker     (121)    28899 2022-04-08 09:12:40.000000 pyevtk-1.5.0/pyevtk/hl.py
--rw-r--r--   0 runner    (1001) docker     (121)    27536 2022-04-08 09:12:40.000000 pyevtk-1.5.0/pyevtk/vtk.py
--rw-r--r--   0 runner    (1001) docker     (121)     4677 2022-04-08 09:12:40.000000 pyevtk-1.5.0/pyevtk/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:12:52.641723 pyevtk-1.5.0/pyevtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5358 2022-04-08 09:12:52.000000 pyevtk-1.5.0/pyevtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-04-08 09:12:52.000000 pyevtk-1.5.0/pyevtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-08 09:12:52.000000 pyevtk-1.5.0/pyevtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-08 09:12:52.000000 pyevtk-1.5.0/pyevtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-08 09:12:52.000000 pyevtk-1.5.0/pyevtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-04-08 09:12:40.000000 pyevtk-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-04-08 09:12:52.641723 pyevtk-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-04-08 09:12:40.000000 pyevtk-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:12:52.641723 pyevtk-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-04-08 09:12:40.000000 pyevtk-1.5.0/tests/dummy.py
--rw-r--r--   0 runner    (1001) docker     (121)    70238 2022-04-08 09:12:40.000000 pyevtk-1.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:25:14.156230 pyevtk-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-05 15:25:01.000000 pyevtk-1.6.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-05 15:25:01.000000 pyevtk-1.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-05 15:25:01.000000 pyevtk-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-05 15:25:14.156230 pyevtk-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-05 15:25:01.000000 pyevtk-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:25:14.152230 pyevtk-1.6.0/evtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 15:25:01.000000 pyevtk-1.6.0/evtk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:25:14.152230 pyevtk-1.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-05 15:25:01.000000 pyevtk-1.6.0/examples/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 15:25:01.000000 pyevtk-1.6.0/examples/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-05 15:25:01.000000 pyevtk-1.6.0/examples/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-05 15:25:01.000000 pyevtk-1.6.0/examples/lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-05 15:25:01.000000 pyevtk-1.6.0/examples/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-05 15:25:01.000000 pyevtk-1.6.0/examples/poly_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-05 15:25:01.000000 pyevtk-1.6.0/examples/rectilinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-05 15:25:01.000000 pyevtk-1.6.0/examples/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-05 15:25:01.000000 pyevtk-1.6.0/examples/unstructured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:25:14.156230 pyevtk-1.6.0/pyevtk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-05 15:25:01.000000 pyevtk-1.6.0/pyevtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-05 15:25:14.156230 pyevtk-1.6.0/pyevtk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-05 15:25:01.000000 pyevtk-1.6.0/pyevtk/evtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29344 2023-06-05 15:25:01.000000 pyevtk-1.6.0/pyevtk/hl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-06-05 15:25:01.000000 pyevtk-1.6.0/pyevtk/vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-05 15:25:01.000000 pyevtk-1.6.0/pyevtk/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:25:14.156230 pyevtk-1.6.0/pyevtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-05 15:25:14.000000 pyevtk-1.6.0/pyevtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 15:25:14.000000 pyevtk-1.6.0/pyevtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:25:14.000000 pyevtk-1.6.0/pyevtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 15:25:14.000000 pyevtk-1.6.0/pyevtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 15:25:14.000000 pyevtk-1.6.0/pyevtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-05 15:25:01.000000 pyevtk-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 15:25:14.156230 pyevtk-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-05 15:25:01.000000 pyevtk-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:25:14.156230 pyevtk-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-05 15:25:01.000000 pyevtk-1.6.0/tests/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70238 2023-06-05 15:25:01.000000 pyevtk-1.6.0/versioneer.py
```

### Comparing `pyevtk-1.5.0/CHANGES.txt` & `pyevtk-1.6.0/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/LICENSE.txt` & `pyevtk-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/PKG-INFO` & `pyevtk-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyevtk
-Version: 1.5.0
+Version: 1.6.0
 Summary: Export data as binary VTK files
 Home-page: https://github.com/pyscience-projects/pyevtk
 Author: Paulo Herrera
 Author-email: pauloa.herrera@gmail.com
 Maintainer: Adamos Kyriakou
 Maintainer-email: somada141@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Coverage Status](https://codecov.io/gh/pyscience-projects/pyevtk/branch/master/graph/badge.svg)](https://codecov.io/gh/pyscience-projects/pyevtk)
 [![Build Status](https://github.com/pyscience-projects/pyevtk/workflows/Test%20Python/badge.svg)](https://github.com/pyscience-projects/pyevtk/actions?query=workflow%3A%22Test+Python%22)
 
 PREAMBLE:
@@ -125,9 +124,7 @@
 I will continue releasing this package as open source, so it is free to be used in any kind of project.
 I will also continue providing support for simple questions and making incremental improvements as time
 allows. However, I also  provide contract based support for commercial or research projects interested
 in this package or in topics related to data analysis and scientific programming with Python, Java, MATLAB/Octave, C/C++ or Fortran.
 For further details, please contact me to: paulo.herrera.eirl@gmail.com.
 
 **NOTE: PyEVTK moved to GitHub. The new official page is this one (https://github.com/paulo-herrera/PyEVTK)**
-
-
```

### Comparing `pyevtk-1.5.0/README.md` & `pyevtk-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/examples/group.py` & `pyevtk-1.6.0/examples/group.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/examples/image.py` & `pyevtk-1.6.0/examples/image.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/examples/lines.py` & `pyevtk-1.6.0/examples/lines.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/examples/lowlevel.py` & `pyevtk-1.6.0/examples/lowlevel.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/examples/points.py` & `pyevtk-1.6.0/examples/points.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/examples/poly_lines.py` & `pyevtk-1.6.0/examples/poly_lines.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/examples/rectilinear.py` & `pyevtk-1.6.0/examples/rectilinear.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/examples/structured.py` & `pyevtk-1.6.0/examples/structured.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/examples/unstructured.py` & `pyevtk-1.6.0/examples/unstructured.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/pyevtk/__init__.py` & `pyevtk-1.6.0/pyevtk/__init__.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/pyevtk/evtk.py` & `pyevtk-1.6.0/pyevtk/evtk.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/pyevtk/hl.py` & `pyevtk-1.6.0/pyevtk/hl.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,22 +198,31 @@
     if cellData is not None:
         keys = list(cellData.keys())
         data = cellData[keys[0]]
         if hasattr(data, "shape"):
             end = data.shape
         elif data[0].ndim == 3 and data[1].ndim == 3 and data[2].ndim == 3:
             end = data[0].shape
+        for i, s in enumerate(spacing):
+            if np.isclose(s, 0.0):
+                if end[i] == 1:
+                    end = end[:i] + (0,) + end[i + 1 :]
+                else:
+                    raise ValueError("imageToVTK: grid has lower dimension than data")
     elif pointData is not None:
         keys = list(pointData.keys())
         data = pointData[keys[0]]
         if hasattr(data, "shape"):
             end = data.shape
         elif data[0].ndim == 3 and data[1].ndim == 3 and data[2].ndim == 3:
             end = data[0].shape
         end = (end[0] - 1, end[1] - 1, end[2] - 1)
+        for i, s in enumerate(spacing):
+            if np.isclose(s, 0.0) and end[i] > 0:
+                raise ValueError("imageToVTK: grid has lower dimension than data")
 
     # Write data to file
     w = VtkFile(path, VtkImageData)
     w.openGrid(start=start, end=end, origin=origin, spacing=spacing)
     w.openPiece(start=start, end=end)
     _addDataToFile(w, cellData, pointData, fieldData)
     w.closePiece()
```

### Comparing `pyevtk-1.5.0/pyevtk/vtk.py` & `pyevtk-1.6.0/pyevtk/vtk.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from .xml import XmlWriter
 
 
 # ================================
 #            VTK Types
 # ================================
 
+
 #     FILE TYPES
 class VtkFileType:
     """
     Wrapper class for VTK file types.
 
     Parameters
     ----------
```

### Comparing `pyevtk-1.5.0/pyevtk/xml.py` & `pyevtk-1.6.0/pyevtk/xml.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/pyevtk.egg-info/PKG-INFO` & `pyevtk-1.6.0/pyevtk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyevtk
-Version: 1.5.0
+Version: 1.6.0
 Summary: Export data as binary VTK files
 Home-page: https://github.com/pyscience-projects/pyevtk
 Author: Paulo Herrera
 Author-email: pauloa.herrera@gmail.com
 Maintainer: Adamos Kyriakou
 Maintainer-email: somada141@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Coverage Status](https://codecov.io/gh/pyscience-projects/pyevtk/branch/master/graph/badge.svg)](https://codecov.io/gh/pyscience-projects/pyevtk)
 [![Build Status](https://github.com/pyscience-projects/pyevtk/workflows/Test%20Python/badge.svg)](https://github.com/pyscience-projects/pyevtk/actions?query=workflow%3A%22Test+Python%22)
 
 PREAMBLE:
@@ -125,9 +124,7 @@
 I will continue releasing this package as open source, so it is free to be used in any kind of project.
 I will also continue providing support for simple questions and making incremental improvements as time
 allows. However, I also  provide contract based support for commercial or research projects interested
 in this package or in topics related to data analysis and scientific programming with Python, Java, MATLAB/Octave, C/C++ or Fortran.
 For further details, please contact me to: paulo.herrera.eirl@gmail.com.
 
 **NOTE: PyEVTK moved to GitHub. The new official page is this one (https://github.com/paulo-herrera/PyEVTK)**
-
-
```

### Comparing `pyevtk-1.5.0/pyevtk.egg-info/SOURCES.txt` & `pyevtk-1.6.0/pyevtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/setup.cfg` & `pyevtk-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/setup.py` & `pyevtk-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,13 +53,14 @@
     package_dir={"pyevtk": "pyevtk"},
     package_data={"pyevtk": ["LICENSE.txt", "examples/*.py"]},
     install_requires=["numpy >= 1.8.0"],
     # necessary for 'python setup.py test'
     setup_requires=["pytest-runner"],
     tests_require=["pytest>=3.1", "pytest-cov", "twine", "check-manifest"],
     classifiers=[
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `pyevtk-1.5.0/tests/dummy.py` & `pyevtk-1.6.0/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `pyevtk-1.5.0/versioneer.py` & `pyevtk-1.6.0/versioneer.py`

 * *Files identical despite different names*

