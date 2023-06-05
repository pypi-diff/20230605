# Comparing `tmp/leosatpy-0.1.0.tar.gz` & `tmp/leosatpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leosatpy-0.1.0.tar", last modified: Sun Jun  4 23:42:46 2023, max compression
+gzip compressed data, was "leosatpy-0.1.1.tar", last modified: Mon Jun  5 01:48:24 2023, max compression
```

## Comparing `leosatpy-0.1.0.tar` & `leosatpy-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-04 23:42:46.444665 leosatpy-0.1.0/
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    35149 2022-08-24 02:26:29.000000 leosatpy-0.1.0/LICENSE
--rw-r--r--   0 cadam     (1000) cadam     (1000)    14778 2023-06-04 23:42:46.443665 leosatpy-0.1.0/PKG-INFO
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    13919 2023-06-04 18:42:12.000000 leosatpy-0.1.0/README.rst
-drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-04 23:42:46.401664 leosatpy-0.1.0/leosatpy/
--rw-r--r--   0 cadam     (1000) cadam     (1000)        0 2023-06-02 19:27:22.000000 leosatpy-0.1.0/leosatpy/__init__.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    99209 2023-06-04 04:25:17.000000 leosatpy-0.1.0/leosatpy/analyseSatObs.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    64014 2023-06-04 04:25:17.000000 leosatpy-0.1.0/leosatpy/calibrateSatObs.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)     4101 2023-06-02 00:45:41.000000 leosatpy-0.1.0/leosatpy/leosatpy_config.ini
--rw-r--r--   0 cadam     (1000) cadam     (1000)    96052 2023-06-04 05:15:44.000000 leosatpy-0.1.0/leosatpy/reduceSatObs.py
-drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-04 23:42:46.442664 leosatpy-0.1.0/leosatpy/utils/
--rw-r--r--   0 cadam     (1000) cadam     (1000)        0 2023-06-02 03:30:59.000000 leosatpy-0.1.0/leosatpy/utils/__init__.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    20810 2023-06-04 05:15:44.000000 leosatpy-0.1.0/leosatpy/utils/arguments.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    16314 2023-06-04 05:15:44.000000 leosatpy-0.1.0/leosatpy/utils/base_conf.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    22529 2023-06-04 04:13:22.000000 leosatpy-0.1.0/leosatpy/utils/dataset.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    11394 2023-06-04 05:15:44.000000 leosatpy-0.1.0/leosatpy/utils/photometry.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    33834 2023-06-04 05:15:44.000000 leosatpy-0.1.0/leosatpy/utils/satellites.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    78259 2023-06-02 05:07:49.000000 leosatpy-0.1.0/leosatpy/utils/sources.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    26135 2023-06-04 05:15:44.000000 leosatpy-0.1.0/leosatpy/utils/tables.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    24200 2023-06-04 05:15:44.000000 leosatpy-0.1.0/leosatpy/utils/telescope_conf.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    31224 2023-06-04 05:15:44.000000 leosatpy-0.1.0/leosatpy/utils/transformations.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)       81 2023-06-02 20:25:53.000000 leosatpy-0.1.0/leosatpy/utils/version.py
-drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-04 23:42:46.418664 leosatpy-0.1.0/leosatpy.egg-info/
--rw-r--r--   0 cadam     (1000) cadam     (1000)    14778 2023-06-04 23:42:46.000000 leosatpy-0.1.0/leosatpy.egg-info/PKG-INFO
--rw-r--r--   0 cadam     (1000) cadam     (1000)      724 2023-06-04 23:42:46.000000 leosatpy-0.1.0/leosatpy.egg-info/SOURCES.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)        1 2023-06-04 23:42:46.000000 leosatpy-0.1.0/leosatpy.egg-info/dependency_links.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)      152 2023-06-04 23:42:46.000000 leosatpy-0.1.0/leosatpy.egg-info/entry_points.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)        1 2023-06-02 19:16:57.000000 leosatpy-0.1.0/leosatpy.egg-info/not-zip-safe
--rw-r--r--   0 cadam     (1000) cadam     (1000)      365 2023-06-04 23:42:46.000000 leosatpy-0.1.0/leosatpy.egg-info/requires.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)        9 2023-06-04 23:42:46.000000 leosatpy-0.1.0/leosatpy.egg-info/top_level.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)       86 2023-06-02 16:48:25.000000 leosatpy-0.1.0/pyproject.toml
--rw-r--r--   0 cadam     (1000) cadam     (1000)      364 2023-05-29 13:43:59.000000 leosatpy-0.1.0/requirements.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)       38 2023-06-04 23:42:46.444665 leosatpy-0.1.0/setup.cfg
--rw-r--r--   0 cadam     (1000) cadam     (1000)     2012 2023-06-02 20:38:58.000000 leosatpy-0.1.0/setup.py
+drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-05 01:48:24.083762 leosatpy-0.1.1/
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    35149 2022-08-24 02:26:29.000000 leosatpy-0.1.1/LICENSE
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    15293 2023-06-05 01:48:24.082762 leosatpy-0.1.1/PKG-INFO
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    14434 2023-06-05 01:41:34.000000 leosatpy-0.1.1/README.rst
+drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-05 01:48:24.080762 leosatpy-0.1.1/leosatpy/
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        0 2023-06-02 19:27:22.000000 leosatpy-0.1.1/leosatpy/__init__.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    99209 2023-06-04 04:25:17.000000 leosatpy-0.1.1/leosatpy/analyseSatObs.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    64014 2023-06-04 04:25:17.000000 leosatpy-0.1.1/leosatpy/calibrateSatObs.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)     4101 2023-06-02 00:45:41.000000 leosatpy-0.1.1/leosatpy/leosatpy_config.ini
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    96052 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/reduceSatObs.py
+drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-05 01:48:24.082762 leosatpy-0.1.1/leosatpy/utils/
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        0 2023-06-02 03:30:59.000000 leosatpy-0.1.1/leosatpy/utils/__init__.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    20810 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/arguments.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    16314 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/base_conf.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    22529 2023-06-04 04:13:22.000000 leosatpy-0.1.1/leosatpy/utils/dataset.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    11394 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/photometry.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    33834 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/satellites.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    78259 2023-06-02 05:07:49.000000 leosatpy-0.1.1/leosatpy/utils/sources.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    26135 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/tables.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    24200 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/telescope_conf.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    31224 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/transformations.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)       81 2023-06-05 01:42:11.000000 leosatpy-0.1.1/leosatpy/utils/version.py
+drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-05 01:48:24.081762 leosatpy-0.1.1/leosatpy.egg-info/
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    15293 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/PKG-INFO
+-rw-r--r--   0 cadam     (1000) cadam     (1000)      724 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/SOURCES.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        1 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/dependency_links.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)      152 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/entry_points.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        1 2023-06-02 19:16:57.000000 leosatpy-0.1.1/leosatpy.egg-info/not-zip-safe
+-rw-r--r--   0 cadam     (1000) cadam     (1000)      365 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/requires.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        9 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/top_level.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)       86 2023-06-02 16:48:25.000000 leosatpy-0.1.1/pyproject.toml
+-rw-r--r--   0 cadam     (1000) cadam     (1000)      364 2023-05-29 13:43:59.000000 leosatpy-0.1.1/requirements.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)       38 2023-06-05 01:48:24.083762 leosatpy-0.1.1/setup.cfg
+-rw-r--r--   0 cadam     (1000) cadam     (1000)     2012 2023-06-02 20:38:58.000000 leosatpy-0.1.1/setup.py
```

### Comparing `leosatpy-0.1.0/LICENSE` & `leosatpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/PKG-INFO` & `leosatpy-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leosatpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: LEOSatpy is a highly-automated end-to-end pipeline for the reduction, calibration, and analysis of Low Earth Orbit Satellite observations from various telescopes.
 Home-page: http://leosatpy.readthedocs.io/
 Download-URL: https://github.com/CLEOsat-group/leosatpy/archive/master.zip
 Author: Christian Adam
 Author-email: christian.adam84@gmail.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
@@ -51,27 +51,39 @@
     :alt: GitHub Repo stars
     :target: https://github.com/CLEOsat-group/leosatpy
 
 .. |watch| image:: https://img.shields.io/github/watchers/CLEOsat-Group/leosatpy?style=social
     :alt: GitHub watchers
     :target: https://github.com/CLEOsat-group/leosatpy
 
+.. |pypi| image:: https://img.shields.io/pypi/v/leosatpy
+    :alt: PyPI
+    :target: https://pypi.org/project/leosatpy/
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/leosatpy
+    :alt: PyPI - Python Version
+    :target: https://pypi.org/project/leosatpy/
+
+.. |last-commit| image:: https://img.shields.io/github/last-commit/CLEOsat-Group/leosatpy
+    :alt: GitHub last commit
+    :target: https://github.com/CLEOsat-group/leosatpy
+
 .. |license| image:: https://img.shields.io/github/license/CLEOsat-Group/leosatpy
     :alt: GitHub
     :target: https://github.com/CLEOsat-group/leosatpy/blob/master/LICENSE
 
 ..
     |stars| |watch|
 
 LEOSatpy
 ========
 
 .. badges
 
-|license|
+|pypi| |python| |last-commit| |license|
 
 **LEOSatpy** (Low Earth Orbit satellite python) is an end-to-end pipeline to process and analyse
 satellite trail observations from various telescopes.
 
 The pipeline is written in Python 3 and provides the following functionalities:
 
 ===========================  ==========================================================================
@@ -127,15 +139,15 @@
     $ conda activate leosatpy_env
 
 
 Installation
 ^^^^^^^^^^^^
 
 
-LEOSatpy is available on PyPI, and can be installed using pip:
+LEOSatpy is available on `PyPI <https://pypi.org/project/leosatpy/>`_, and can be installed using pip:
 
 .. code:: bash
 
     $ (leosatpy_env) pip install leosatpy
 
 Alternatively, the latest release of LEOSatpy is also available from the `GitHub repository <https://github.com/CLEOsat-group/leosatpy>`_.
```

### Comparing `leosatpy-0.1.0/README.rst` & `leosatpy-0.1.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -32,27 +32,39 @@
     :alt: GitHub Repo stars
     :target: https://github.com/CLEOsat-group/leosatpy
 
 .. |watch| image:: https://img.shields.io/github/watchers/CLEOsat-Group/leosatpy?style=social
     :alt: GitHub watchers
     :target: https://github.com/CLEOsat-group/leosatpy
 
+.. |pypi| image:: https://img.shields.io/pypi/v/leosatpy
+    :alt: PyPI
+    :target: https://pypi.org/project/leosatpy/
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/leosatpy
+    :alt: PyPI - Python Version
+    :target: https://pypi.org/project/leosatpy/
+
+.. |last-commit| image:: https://img.shields.io/github/last-commit/CLEOsat-Group/leosatpy
+    :alt: GitHub last commit
+    :target: https://github.com/CLEOsat-group/leosatpy
+
 .. |license| image:: https://img.shields.io/github/license/CLEOsat-Group/leosatpy
     :alt: GitHub
     :target: https://github.com/CLEOsat-group/leosatpy/blob/master/LICENSE
 
 ..
     |stars| |watch|
 
 LEOSatpy
 ========
 
 .. badges
 
-|license|
+|pypi| |python| |last-commit| |license|
 
 **LEOSatpy** (Low Earth Orbit satellite python) is an end-to-end pipeline to process and analyse
 satellite trail observations from various telescopes.
 
 The pipeline is written in Python 3 and provides the following functionalities:
 
 ===========================  ==========================================================================
@@ -108,15 +120,15 @@
     $ conda activate leosatpy_env
 
 
 Installation
 ^^^^^^^^^^^^
 
 
-LEOSatpy is available on PyPI, and can be installed using pip:
+LEOSatpy is available on `PyPI <https://pypi.org/project/leosatpy/>`_, and can be installed using pip:
 
 .. code:: bash
 
     $ (leosatpy_env) pip install leosatpy
 
 Alternatively, the latest release of LEOSatpy is also available from the `GitHub repository <https://github.com/CLEOsat-group/leosatpy>`_.
```

### Comparing `leosatpy-0.1.0/leosatpy/analyseSatObs.py` & `leosatpy-0.1.1/leosatpy/analyseSatObs.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/calibrateSatObs.py` & `leosatpy-0.1.1/leosatpy/calibrateSatObs.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/leosatpy_config.ini` & `leosatpy-0.1.1/leosatpy/leosatpy_config.ini`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/reduceSatObs.py` & `leosatpy-0.1.1/leosatpy/reduceSatObs.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/utils/arguments.py` & `leosatpy-0.1.1/leosatpy/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/utils/base_conf.py` & `leosatpy-0.1.1/leosatpy/utils/base_conf.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/utils/dataset.py` & `leosatpy-0.1.1/leosatpy/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/utils/photometry.py` & `leosatpy-0.1.1/leosatpy/utils/photometry.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/utils/satellites.py` & `leosatpy-0.1.1/leosatpy/utils/satellites.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/utils/sources.py` & `leosatpy-0.1.1/leosatpy/utils/sources.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/utils/tables.py` & `leosatpy-0.1.1/leosatpy/utils/tables.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/utils/telescope_conf.py` & `leosatpy-0.1.1/leosatpy/utils/telescope_conf.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy/utils/transformations.py` & `leosatpy-0.1.1/leosatpy/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/leosatpy.egg-info/PKG-INFO` & `leosatpy-0.1.1/leosatpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leosatpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: LEOSatpy is a highly-automated end-to-end pipeline for the reduction, calibration, and analysis of Low Earth Orbit Satellite observations from various telescopes.
 Home-page: http://leosatpy.readthedocs.io/
 Download-URL: https://github.com/CLEOsat-group/leosatpy/archive/master.zip
 Author: Christian Adam
 Author-email: christian.adam84@gmail.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
@@ -51,27 +51,39 @@
     :alt: GitHub Repo stars
     :target: https://github.com/CLEOsat-group/leosatpy
 
 .. |watch| image:: https://img.shields.io/github/watchers/CLEOsat-Group/leosatpy?style=social
     :alt: GitHub watchers
     :target: https://github.com/CLEOsat-group/leosatpy
 
+.. |pypi| image:: https://img.shields.io/pypi/v/leosatpy
+    :alt: PyPI
+    :target: https://pypi.org/project/leosatpy/
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/leosatpy
+    :alt: PyPI - Python Version
+    :target: https://pypi.org/project/leosatpy/
+
+.. |last-commit| image:: https://img.shields.io/github/last-commit/CLEOsat-Group/leosatpy
+    :alt: GitHub last commit
+    :target: https://github.com/CLEOsat-group/leosatpy
+
 .. |license| image:: https://img.shields.io/github/license/CLEOsat-Group/leosatpy
     :alt: GitHub
     :target: https://github.com/CLEOsat-group/leosatpy/blob/master/LICENSE
 
 ..
     |stars| |watch|
 
 LEOSatpy
 ========
 
 .. badges
 
-|license|
+|pypi| |python| |last-commit| |license|
 
 **LEOSatpy** (Low Earth Orbit satellite python) is an end-to-end pipeline to process and analyse
 satellite trail observations from various telescopes.
 
 The pipeline is written in Python 3 and provides the following functionalities:
 
 ===========================  ==========================================================================
@@ -127,15 +139,15 @@
     $ conda activate leosatpy_env
 
 
 Installation
 ^^^^^^^^^^^^
 
 
-LEOSatpy is available on PyPI, and can be installed using pip:
+LEOSatpy is available on `PyPI <https://pypi.org/project/leosatpy/>`_, and can be installed using pip:
 
 .. code:: bash
 
     $ (leosatpy_env) pip install leosatpy
 
 Alternatively, the latest release of LEOSatpy is also available from the `GitHub repository <https://github.com/CLEOsat-group/leosatpy>`_.
```

### Comparing `leosatpy-0.1.0/leosatpy.egg-info/SOURCES.txt` & `leosatpy-0.1.1/leosatpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.0/setup.py` & `leosatpy-0.1.1/setup.py`

 * *Files identical despite different names*

