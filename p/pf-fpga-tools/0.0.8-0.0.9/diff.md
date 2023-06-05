# Comparing `tmp/pf_fpga_tools-0.0.8.tar.gz` & `tmp/pf_fpga_tools-0.0.9.tar.gz`

## Comparing `pf_fpga_tools-0.0.8.tar` & `pf_fpga_tools-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/.flake8
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/Exceptions.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/__init__.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/utils.py
--rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfBuildCore/__main__.py
--rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfBuildCore/pfBuildCore.py
--rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfCloneCoreTemplate/__main__.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
--rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfConvertImage/__main__.py
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfConvertImage/pfConvertImage.py
--rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfInstallCore/__main__.py
--rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfInstallCore/pfInstallCore.py
--rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfQuartusEdit/__main__.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py
--rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfReverseBitstream/__main__.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/LICENSE
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/README.md
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/.flake8
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/Exceptions.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/__init__.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/utils.py
+-rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfBuildCore/__main__.py
+-rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfBuildCore/pfBuildCore.py
+-rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfCloneCoreTemplate/__main__.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
+-rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfConvertImage/__main__.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfConvertImage/pfConvertImage.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfInstallCore/__main__.py
+-rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfInstallCore/pfInstallCore.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfQuartusEdit/__main__.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py
+-rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfReverseBitstream/__main__.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/README.md
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.9/PKG-INFO
```

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/utils.py` & `pf_fpga_tools-0.0.9/pfFPGATools/utils.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfBuildCore/__main__.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfBuildCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfBuildCore/pfBuildCore.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfBuildCore/pfBuildCore.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfCloneCoreTemplate/__main__.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfCloneCoreTemplate/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfConvertImage/__main__.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfConvertImage/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfConvertImage/pfConvertImage.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfConvertImage/pfConvertImage.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfInstallCore/__main__.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfInstallCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfInstallCore/pfInstallCore.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfInstallCore/pfInstallCore.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfQuartusEdit/__main__.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfQuartusEdit/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfReverseBitstream/__main__.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfReverseBitstream/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py` & `pf_fpga_tools-0.0.9/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/LICENSE` & `pf_fpga_tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/README.md` & `pf_fpga_tools-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfFPGATools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-fpga-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-fpga-tools.svg)](https://pypi.org/project/pf-fpga-tools)
 
 A set of tools for building and installing [**openFPGA**](https://www.analogue.co/developer) cores for the [**Analog Pocket**](https://www.analogue.co/pocket).
 
 Copyright (c) 2023-present Didier Malenfant.
 
-#### This project is obsolete and has been replaced by the more generic [pf-tools](https://pypi.org/project/pf-tools/).
+#### This project is obsolete and has been replaced by the more generic [pf-dev-tools](https://pypi.org/project/pf-dev-tools/).
 
 -----
 
 ### Installation
 
 **pfFPGATools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
```

### Comparing `pf_fpga_tools-0.0.8/pyproject.toml` & `pf_fpga_tools-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.8/PKG-INFO` & `pf_fpga_tools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pf-fpga-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of tools for openFPGA projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
 Project-URL: Documentation, https://github.com/DidierMalenfant/pfFPGATools#readme
 Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfFPGATools/issues
 Project-URL: Source Code, https://github.com/DidierMalenfant/pfFPGATools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
@@ -24,15 +24,15 @@
 
 [![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfFPGATools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-fpga-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-fpga-tools.svg)](https://pypi.org/project/pf-fpga-tools)
 
 A set of tools for building and installing [**openFPGA**](https://www.analogue.co/developer) cores for the [**Analog Pocket**](https://www.analogue.co/pocket).
 
 Copyright (c) 2023-present Didier Malenfant.
 
-#### This project is obsolete and has been replaced by the more generic [pf-tools](https://pypi.org/project/pf-tools/).
+#### This project is obsolete and has been replaced by the more generic [pf-dev-tools](https://pypi.org/project/pf-dev-tools/).
 
 -----
 
 ### Installation
 
 **pfFPGATools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
```

