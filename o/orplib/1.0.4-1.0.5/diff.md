# Comparing `tmp/orplib-1.0.4.tar.gz` & `tmp/orplib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orplib-1.0.4.tar", last modified: Thu May 11 21:09:09 2023, max compression
+gzip compressed data, was "orplib-1.0.5.tar", last modified: Mon Jun  5 21:27:00 2023, max compression
```

## Comparing `orplib-1.0.4.tar` & `orplib-1.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.195902 orplib-1.0.4/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       45 2023-05-11 21:06:43.000000 orplib-1.0.4/MANIFEST.in
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6973 2023-05-11 21:09:09.195902 orplib-1.0.4/PKG-INFO
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6543 2023-04-28 16:12:50.000000 orplib-1.0.4/README.md
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      101 2023-04-14 19:45:52.000000 orplib-1.0.4/pyproject.toml
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      821 2023-05-11 21:09:09.196902 orplib-1.0.4/setup.cfg
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.193902 orplib-1.0.4/src/
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.194902 orplib-1.0.4/src/orpl/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      341 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       89 2023-05-11 20:49:13.000000 orplib-1.0.4/src/orpl/__main__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    15209 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/baseline_removal.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    16694 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/bubblegif.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     8250 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/calibration.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     3772 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/cosmic_ray.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.194902 orplib-1.0.4/src/orpl/data/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/data/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    63150 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/data/synthetic_presets.json
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1019 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/datatypes.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6237 2023-05-11 20:11:54.000000 orplib-1.0.4/src/orpl/file_io.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.195902 orplib-1.0.4/src/orpl/gui/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/gui/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1100 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/gui/mplcanvas.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    28231 2023-05-11 20:49:15.000000 orplib-1.0.4/src/orpl/gui/orplGUI.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.195902 orplib-1.0.4/src/orpl/gui/uis/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/gui/uis/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    30696 2023-05-11 19:59:11.000000 orplib-1.0.4/src/orpl/gui/uis/ui_mainWindow.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1846 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/metrics.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     2135 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/normalization.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       92 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/pipelines.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     4566 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/plot.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7014 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/synthetic.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.195902 orplib-1.0.4/src/orplib.egg-info/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6973 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/PKG-INFO
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      705 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/SOURCES.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        1 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/dependency_links.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      161 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/requires.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        5 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/top_level.txt
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.443391 orplib-1.0.5/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       23 2023-05-11 21:09:19.000000 orplib-1.0.5/MANIFEST.in
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-06-05 21:27:00.443391 orplib-1.0.5/PKG-INFO
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6777 2023-05-11 21:32:45.000000 orplib-1.0.5/README.md
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      101 2023-04-14 19:45:52.000000 orplib-1.0.5/pyproject.toml
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      821 2023-06-05 21:27:00.443391 orplib-1.0.5/setup.cfg
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.440392 orplib-1.0.5/src/
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.442391 orplib-1.0.5/src/orpl/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      317 2023-05-12 18:34:44.000000 orplib-1.0.5/src/orpl/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       89 2023-06-05 21:20:32.000000 orplib-1.0.5/src/orpl/__main__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    15209 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/baseline_removal.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    16694 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/bubblegif.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     8250 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/calibration.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     3772 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/cosmic_ray.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.442391 orplib-1.0.5/src/orpl/data/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/data/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    63150 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/data/synthetic_presets.json
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1179 2023-06-05 21:21:11.000000 orplib-1.0.5/src/orpl/datatypes.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    10430 2023-06-05 21:21:53.000000 orplib-1.0.5/src/orpl/file_io.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.442391 orplib-1.0.5/src/orpl/gui/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/gui/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1100 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/gui/mplcanvas.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    28290 2023-05-17 15:11:57.000000 orplib-1.0.5/src/orpl/gui/orplGUI.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.442391 orplib-1.0.5/src/orpl/gui/uis/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/gui/uis/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    30696 2023-05-11 19:59:11.000000 orplib-1.0.5/src/orpl/gui/uis/ui_mainWindow.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1846 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/metrics.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     2135 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/normalization.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       92 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/pipelines.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     4566 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/plot.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7014 2023-04-14 19:45:52.000000 orplib-1.0.5/src/orpl/synthetic.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-05 21:27:00.443391 orplib-1.0.5/src/orplib.egg-info/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/PKG-INFO
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      705 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/SOURCES.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        1 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/dependency_links.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      161 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/requires.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        5 2023-06-05 21:27:00.000000 orplib-1.0.5/src/orplib.egg-info/top_level.txt
```

### Comparing `orplib-1.0.4/PKG-INFO` & `orplib-1.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: orplib
-Version: 1.0.4
-Summary: Open Raman Processing Library
-Home-page: https://github.com/mr-sheg/orpl
-Author: Guillaume Sheehy
-Author-email: guillaume.sheehy@polymtl.ca
-License: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # ORPL
 
 ORPL (read _orpel_) is the Open Raman Processing Library. It provides tools for the processing of Raman spectrum, including;
 
 1. System calibration (x-axis and system response)
 2. Cosmic Ray removal
 3. Baseline removal (autofluorescence)
@@ -33,14 +19,15 @@
     - [Windows Installation Guide](#windows-installation-guide)
     - [Already familiar with python and pip?](#already-familiar-with-python-and-pip)
     - [I'm new to python and this 'pip' thing?](#im-new-to-python-and-this-pip-thing)
     - [Updating ORPL to the latest version](#updating-orpl-to-the-latest-version)
       - [If you have admin rights](#if-you-have-admin-rights)
       - [If you do not have admin rights](#if-you-do-not-have-admin-rights)
     - [Building from source](#building-from-source)
+  - [Sample files](#sample-files)
   - [Baseline removal](#baseline-removal)
     - [BubbleFill](#bubblefill)
   - [How to cite this work](#how-to-cite-this-work)
     - [BibTex (.bib)](#bibtex-bib)
     - [EndNote (.enw)](#endnote-enw)
     - [Contributors](#contributors)
 
@@ -96,14 +83,18 @@
 
 and to update the build on pypi (this is a reminder for me, it won't do anything if you do this),
 
 ```
 python -m twine upload --repository pypi --skip-existing dist/*
 ```
 
+## Sample files
+
+You can download sample files to play around with ORPL - GUI or the library. They are located [here](https://github.com/mr-sheg/orpl/raw/main/sample%20data/ORPL%20sample%20data.zip)
+
 ## Baseline removal
 
 ### BubbleFill
 
 Bubblefill is a morphological processing algorithm designed for the removal of baselines in spectroscopic signal. It was created and optimized specifically to remove autofluorescence baselines in Raman spectra measured on biological samples.
 
 ![Bubblefill in action](documentation/bacon_100.gif)
```

### Comparing `orplib-1.0.4/README.md` & `orplib-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: orplib
+Version: 1.0.5
+Summary: Open Raman Processing Library
+Home-page: https://github.com/mr-sheg/orpl
+Author: Guillaume Sheehy
+Author-email: guillaume.sheehy@polymtl.ca
+License: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # ORPL
 
 ORPL (read _orpel_) is the Open Raman Processing Library. It provides tools for the processing of Raman spectrum, including;
 
 1. System calibration (x-axis and system response)
 2. Cosmic Ray removal
 3. Baseline removal (autofluorescence)
@@ -19,14 +33,15 @@
     - [Windows Installation Guide](#windows-installation-guide)
     - [Already familiar with python and pip?](#already-familiar-with-python-and-pip)
     - [I'm new to python and this 'pip' thing?](#im-new-to-python-and-this-pip-thing)
     - [Updating ORPL to the latest version](#updating-orpl-to-the-latest-version)
       - [If you have admin rights](#if-you-have-admin-rights)
       - [If you do not have admin rights](#if-you-do-not-have-admin-rights)
     - [Building from source](#building-from-source)
+  - [Sample files](#sample-files)
   - [Baseline removal](#baseline-removal)
     - [BubbleFill](#bubblefill)
   - [How to cite this work](#how-to-cite-this-work)
     - [BibTex (.bib)](#bibtex-bib)
     - [EndNote (.enw)](#endnote-enw)
     - [Contributors](#contributors)
 
@@ -82,14 +97,18 @@
 
 and to update the build on pypi (this is a reminder for me, it won't do anything if you do this),
 
 ```
 python -m twine upload --repository pypi --skip-existing dist/*
 ```
 
+## Sample files
+
+You can download sample files to play around with ORPL - GUI or the library. They are located [here](https://github.com/mr-sheg/orpl/raw/main/sample%20data/ORPL%20sample%20data.zip)
+
 ## Baseline removal
 
 ### BubbleFill
 
 Bubblefill is a morphological processing algorithm designed for the removal of baselines in spectroscopic signal. It was created and optimized specifically to remove autofluorescence baselines in Raman spectra measured on biological samples.
 
 ![Bubblefill in action](documentation/bacon_100.gif)
```

### Comparing `orplib-1.0.4/setup.cfg` & `orplib-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = orplib
-version = 1.0.4
+version = 1.0.5
 author = Guillaume Sheehy
 author_email = guillaume.sheehy@polymtl.ca
 description = Open Raman Processing Library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 url = https://github.com/mr-sheg/orpl
```

### Comparing `orplib-1.0.4/src/orpl/baseline_removal.py` & `orplib-1.0.5/src/orpl/baseline_removal.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/bubblegif.py` & `orplib-1.0.5/src/orpl/bubblegif.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/calibration.py` & `orplib-1.0.5/src/orpl/calibration.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/cosmic_ray.py` & `orplib-1.0.5/src/orpl/cosmic_ray.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/data/synthetic_presets.json` & `orplib-1.0.5/src/orpl/data/synthetic_presets.json`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/datatypes.py` & `orplib-1.0.5/src/orpl/datatypes.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,26 +2,34 @@
 from pathlib import Path
 from typing import Type
 
 from numpy import ndarray
 
 
 @dataclass(frozen=True)
-class Metadata:
+class Acquisition_info:
+    exposure_time: float  # [ms]
+    n_accumulations: int
+    laser_power: float
+    power_units: str
+
+
+@dataclass(frozen=True)
+class Rdf_metadata:
     # timestamp: int  # epoch [s]
     filepath: Type[Path]
     exposure_time: float  # [ms]
     source_power: float  # [mw]
     details: dict
     comment: str
 
 
 @dataclass(frozen=True)
 class Spectrum:
-    metadata: Metadata
+    metadata: Rdf_metadata
     accumulations: ndarray
     background: ndarray
     nbins: int = field(init=False)
     naccumulations: int = field(init=False)
     mean_spectrum: ndarray = field(init=False)
 
     def __post_init__(self):
```

### Comparing `orplib-1.0.4/src/orpl/gui/mplcanvas.py` & `orplib-1.0.5/src/orpl/gui/mplcanvas.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/gui/orplGUI.py` & `orplib-1.0.5/src/orpl/gui/orplGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import sys
 import traceback
+from importlib.metadata import version
 from pathlib import Path
 from time import strftime
 from typing import List, Tuple
 
 import numpy as np
 import pyperclip  # module to copy text to clipboard (ctrl + c | ctrl + v)
 import qtmodern.styles
@@ -16,24 +17,26 @@
     QFileDialog,
     QFileSystemModel,
     QMainWindow,
     QStyle,
 )
 from ruamel import yaml
 
-from orpl import ORPL_VERSION, file_io
+from orpl import file_io
 from orpl.baseline_removal import bubblefill, imodpoly, morph_br
 from orpl.calibration import autogenx, compute_irf
 from orpl.cosmic_ray import crfilter_multi, crfilter_single
 from orpl.datatypes import Spectrum
 from orpl.file_io import RDF
 from orpl.gui.mplcanvas import PlotWidget
 from orpl.gui.uis.ui_mainWindow import Ui_mainWindow
 from orpl.normalization import auc, maxband, minmax, snv
 
+ORPL_VERSION = version("orplib")
+
 # Set-up home directory for ORPL
 HOME_DIR = Path.home()
 ORPL_DIR = HOME_DIR / "orpl"
 if not ORPL_DIR.exists():
     ORPL_DIR.mkdir()
 LOG_DIR = ORPL_DIR / "logs"
 if not LOG_DIR.exists():
```

### Comparing `orplib-1.0.4/src/orpl/gui/uis/ui_mainWindow.py` & `orplib-1.0.5/src/orpl/gui/uis/ui_mainWindow.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/metrics.py` & `orplib-1.0.5/src/orpl/metrics.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/normalization.py` & `orplib-1.0.5/src/orpl/normalization.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/plot.py` & `orplib-1.0.5/src/orpl/plot.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orpl/synthetic.py` & `orplib-1.0.5/src/orpl/synthetic.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.4/src/orplib.egg-info/PKG-INFO` & `orplib-1.0.5/src/orplib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orplib
-Version: 1.0.4
+Version: 1.0.5
 Summary: Open Raman Processing Library
 Home-page: https://github.com/mr-sheg/orpl
 Author: Guillaume Sheehy
 Author-email: guillaume.sheehy@polymtl.ca
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,14 +33,15 @@
     - [Windows Installation Guide](#windows-installation-guide)
     - [Already familiar with python and pip?](#already-familiar-with-python-and-pip)
     - [I'm new to python and this 'pip' thing?](#im-new-to-python-and-this-pip-thing)
     - [Updating ORPL to the latest version](#updating-orpl-to-the-latest-version)
       - [If you have admin rights](#if-you-have-admin-rights)
       - [If you do not have admin rights](#if-you-do-not-have-admin-rights)
     - [Building from source](#building-from-source)
+  - [Sample files](#sample-files)
   - [Baseline removal](#baseline-removal)
     - [BubbleFill](#bubblefill)
   - [How to cite this work](#how-to-cite-this-work)
     - [BibTex (.bib)](#bibtex-bib)
     - [EndNote (.enw)](#endnote-enw)
     - [Contributors](#contributors)
 
@@ -96,14 +97,18 @@
 
 and to update the build on pypi (this is a reminder for me, it won't do anything if you do this),
 
 ```
 python -m twine upload --repository pypi --skip-existing dist/*
 ```
 
+## Sample files
+
+You can download sample files to play around with ORPL - GUI or the library. They are located [here](https://github.com/mr-sheg/orpl/raw/main/sample%20data/ORPL%20sample%20data.zip)
+
 ## Baseline removal
 
 ### BubbleFill
 
 Bubblefill is a morphological processing algorithm designed for the removal of baselines in spectroscopic signal. It was created and optimized specifically to remove autofluorescence baselines in Raman spectra measured on biological samples.
 
 ![Bubblefill in action](documentation/bacon_100.gif)
```

### Comparing `orplib-1.0.4/src/orplib.egg-info/SOURCES.txt` & `orplib-1.0.5/src/orplib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

