# Comparing `tmp/dfipy-0.1.2.tar.gz` & `tmp/dfipy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfipy-0.1.2.tar", max compression
+gzip compressed data, was "dfipy-0.1.3.tar", max compression
```

## Comparing `dfipy-0.1.2.tar` & `dfipy-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      557 2023-06-05 10:12:54.483500 dfipy-0.1.2/LICENCE
--rw-r--r--   0        0        0     1733 2023-06-05 10:12:54.483500 dfipy-0.1.2/README.md
--rw-r--r--   0        0        0      194 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/__init__.py
--rw-r--r--   0        0        0    16364 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/analysis.py
--rw-r--r--   0        0        0     4631 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/connection.py
--rw-r--r--   0        0        0    25259 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/getters.py
--rw-r--r--   0        0        0     1537 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/logging.py
--rw-r--r--   0        0        0    15871 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/show.py
--rw-r--r--   0        0        0     5566 2023-06-05 10:12:54.483500 dfipy-0.1.2/dfi/stream.py
--rw-r--r--   0        0        0     1994 2023-06-05 10:12:55.427519 dfipy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 dfipy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      557 2023-06-05 12:24:24.510120 dfipy-0.1.3/LICENCE
+-rw-r--r--   0        0        0     1741 2023-06-05 12:24:24.510120 dfipy-0.1.3/README.md
+-rw-r--r--   0        0        0      194 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/__init__.py
+-rw-r--r--   0        0        0    16364 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/analysis.py
+-rw-r--r--   0        0        0     4631 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/connection.py
+-rw-r--r--   0        0        0    25259 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/getters.py
+-rw-r--r--   0        0        0     1537 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/logging.py
+-rw-r--r--   0        0        0    15871 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/show.py
+-rw-r--r--   0        0        0     5566 2023-06-05 12:24:24.510120 dfipy-0.1.3/dfi/stream.py
+-rw-r--r--   0        0        0     1994 2023-06-05 12:24:25.394132 dfipy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 dfipy-0.1.3/PKG-INFO
```

### Comparing `dfipy-0.1.2/LICENCE` & `dfipy-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.2/README.md` & `dfipy-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <img src="docs/gs_logo.png" width="40%" align="right">
 
-[![Python versions](https://img.shields.io/pypi/pyversions/dfi.svg)](https://pypi.python.org/pypi/dfi/)
-[![PyPI version](https://badge.fury.io/py/dfi.svg)](https://badge.fury.io/py/dfi)
+[![Python versions](https://img.shields.io/pypi/pyversions/dfipy.svg)](https://pypi.python.org/pypi/dfipy/)
+[![PyPI version](https://badge.fury.io/py/dfipy.svg)](https://badge.fury.io/py/dfipy)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)
 
 # DFI API wrapper
 
 ## About
```

### Comparing `dfipy-0.1.2/dfi/analysis.py` & `dfipy-0.1.3/dfi/analysis.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.2/dfi/connection.py` & `dfipy-0.1.3/dfi/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class DFIConnect:
     """
     Class instantiating the connectors to the DFI API.
 
     Parameters
     ----------
     api_token: str,
-        token provided by generalsystem.com to access the running DFI enfironments.
+        token provided by generalsystem.com to access the running DFI environments.
     instance_name: str,
         DFI API engine instance.
     namespace: str,
         Name of the space where the DFI instance lives.
     query_timeout: int = 60,
         Time after an unresponsive query will be dropped.
     base_url : str =None
```

### Comparing `dfipy-0.1.2/dfi/getters.py` & `dfipy-0.1.3/dfi/getters.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.2/dfi/logging.py` & `dfipy-0.1.3/dfi/logging.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.2/dfi/show.py` & `dfipy-0.1.3/dfi/show.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.2/dfi/stream.py` & `dfipy-0.1.3/dfi/stream.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.2/pyproject.toml` & `dfipy-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ] # List of note tags to take in consideration, separated by a comma.
 
 [tool.poetry]
 name = "dfipy"
 # Package versions are derived from Git tags in CI and overridden during
 # building/publishing. See build/publish jobs in .gitlab-ci.yml.
 # Keep the following version at 0.0.0 as it is not used anyway.
-version = "0.1.2"
+version = "0.1.3"
 description = "DFI api python wrapper"
 authors = [
   "Maurizio Morriello <maurizio.morriello@excession.co>",
   "Sebastiano Ferraris <sebastiano.ferraris@excession.co>",
 ]
 readme = "README.md"
 include = ["LICENCE"]
```

### Comparing `dfipy-0.1.2/PKG-INFO` & `dfipy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfipy
-Version: 0.1.2
+Version: 0.1.3
 Summary: DFI api python wrapper
 Author: Maurizio Morriello
 Author-email: maurizio.morriello@excession.co
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,16 +22,16 @@
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Requires-Dist: sseclient-py (>=1.7.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <img src="docs/gs_logo.png" width="40%" align="right">
 
-[![Python versions](https://img.shields.io/pypi/pyversions/dfi.svg)](https://pypi.python.org/pypi/dfi/)
-[![PyPI version](https://badge.fury.io/py/dfi.svg)](https://badge.fury.io/py/dfi)
+[![Python versions](https://img.shields.io/pypi/pyversions/dfipy.svg)](https://pypi.python.org/pypi/dfipy/)
+[![PyPI version](https://badge.fury.io/py/dfipy.svg)](https://badge.fury.io/py/dfipy)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)
 
 # DFI API wrapper
 
 ## About
```

