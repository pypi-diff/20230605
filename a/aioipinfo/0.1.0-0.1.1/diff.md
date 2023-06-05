# Comparing `tmp/aioipinfo-0.1.0.tar.gz` & `tmp/aioipinfo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioipinfo-0.1.0.tar", last modified: Mon Jun  5 01:22:26 2023, max compression
+gzip compressed data, was "aioipinfo-0.1.1.tar", last modified: Mon Jun  5 01:33:24 2023, max compression
```

## Comparing `aioipinfo-0.1.0.tar` & `aioipinfo-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 01:22:26.983718 aioipinfo-0.1.0/
--rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-05 01:04:30.000000 aioipinfo-0.1.0/LICENSE
--rw-r--r--   0 gormo      (501) staff       (20)     1835 2023-06-05 01:22:26.983591 aioipinfo-0.1.0/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      281 2023-06-05 01:06:42.000000 aioipinfo-0.1.0/README.md
--rw-r--r--   0 gormo      (501) staff       (20)      530 2023-06-05 01:22:22.000000 aioipinfo-0.1.0/pyproject.toml
--rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-05 01:22:26.983754 aioipinfo-0.1.0/setup.cfg
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 01:22:26.982260 aioipinfo-0.1.0/src/
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 01:22:26.982925 aioipinfo-0.1.0/src/aioipinfo/
--rw-r--r--   0 gormo      (501) staff       (20)     4079 2023-06-05 01:22:22.000000 aioipinfo-0.1.0/src/aioipinfo/__init__.py
--rw-r--r--   0 gormo      (501) staff       (20)     1834 2023-06-05 01:11:57.000000 aioipinfo-0.1.0/src/aioipinfo/__main__.py
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 01:22:26.983422 aioipinfo-0.1.0/src/aioipinfo.egg-info/
--rw-r--r--   0 gormo      (501) staff       (20)     1835 2023-06-05 01:22:26.000000 aioipinfo-0.1.0/src/aioipinfo.egg-info/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      232 2023-06-05 01:22:26.000000 aioipinfo-0.1.0/src/aioipinfo.egg-info/SOURCES.txt
--rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-05 01:22:26.000000 aioipinfo-0.1.0/src/aioipinfo.egg-info/dependency_links.txt
--rw-r--r--   0 gormo      (501) staff       (20)       10 2023-06-05 01:22:26.000000 aioipinfo-0.1.0/src/aioipinfo.egg-info/top_level.txt
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 01:33:24.655497 aioipinfo-0.1.1/
+-rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-05 01:04:30.000000 aioipinfo-0.1.1/LICENSE
+-rw-r--r--   0 gormo      (501) staff       (20)     1833 2023-06-05 01:33:24.655371 aioipinfo-0.1.1/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      280 2023-06-05 01:31:41.000000 aioipinfo-0.1.1/README.md
+-rw-r--r--   0 gormo      (501) staff       (20)      529 2023-06-05 01:33:20.000000 aioipinfo-0.1.1/pyproject.toml
+-rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-05 01:33:24.655536 aioipinfo-0.1.1/setup.cfg
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 01:33:24.654033 aioipinfo-0.1.1/src/
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 01:33:24.654693 aioipinfo-0.1.1/src/aioipinfo/
+-rw-r--r--   0 gormo      (501) staff       (20)     4084 2023-06-05 01:33:20.000000 aioipinfo-0.1.1/src/aioipinfo/__init__.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1834 2023-06-05 01:11:57.000000 aioipinfo-0.1.1/src/aioipinfo/__main__.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 01:33:24.655210 aioipinfo-0.1.1/src/aioipinfo.egg-info/
+-rw-r--r--   0 gormo      (501) staff       (20)     1833 2023-06-05 01:33:24.000000 aioipinfo-0.1.1/src/aioipinfo.egg-info/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      232 2023-06-05 01:33:24.000000 aioipinfo-0.1.1/src/aioipinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-05 01:33:24.000000 aioipinfo-0.1.1/src/aioipinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       10 2023-06-05 01:33:24.000000 aioipinfo-0.1.1/src/aioipinfo.egg-info/top_level.txt
```

### Comparing `aioipinfo-0.1.0/LICENSE` & `aioipinfo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioipinfo-0.1.0/PKG-INFO` & `aioipinfo-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipinfo
-Version: 0.1.0
+Version: 0.1.1
 Summary: The aioipinfo Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,17 +21,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/gormaniac/aioipinfo
-Project-URL: Documentation, https://gormo.com/aioipinfo/
+Project-URL: Documentation, https://gormo.co/aioipinfo/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aioipinfo
 
 A simple, async [ipinfo.io](https://ipinfo.io) client.
 
-Exposes an `IPInfoClient` that implements one querying method, `ipinfo`, and includes a CLI client that can be run with `python3 -m aioipinfo`. See the [full docs](https://gormo.com/aioipinfo/) for more details.
+Exposes an `IPInfoClient` that implements one querying method, `ipinfo`, and includes a CLI client that can be run with `python3 -m aioipinfo`. See the [full docs](https://gormo.co/aioipinfo/) for more details.
```

### Comparing `aioipinfo-0.1.0/pyproject.toml` & `aioipinfo-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioipinfo"
-version = "0.1.0"
+version = "0.1.1"
 description = "The aioipinfo Python package"
 readme = "README.md"
 requires-python = ">=3.11"
 
 # Fill in dependencies here.
 dependencies = []
 
@@ -16,12 +16,12 @@
 name = "John Gorman"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/gormaniac/aioipinfo"
-Documentation = "https://gormo.com/aioipinfo/"
+Documentation = "https://gormo.co/aioipinfo/"
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
```

### Comparing `aioipinfo-0.1.0/src/aioipinfo/__init__.py` & `aioipinfo-0.1.1/src/aioipinfo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """IPInfo CLient."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 import dataclasses
 import ipaddress
 import json
 
 import aiohttp
 
@@ -54,19 +54,19 @@
     return lat.strip(), long.strip()
 
 
 @dataclasses.dataclass
 class IPInfoResponse:
     """The response object from an free ipinfo.io GeoLocation Data query.
 
-    See ipinfo.io docs_ for property info.
+    See ipinfo.io `docs`_ for property info.
 
     Exposes a `pprint` method that dumps the object to stdout.
 
-    _docs: https://ipinfo.io/developers/data-types#geolocation-data
+    .. _docs: https://ipinfo.io/developers/data-types#geolocation-data
     """
 
     ip: str
     hostname: str | None = None
     city: str | None = None
     region: str | None = None
     country: str | None = None
```

### Comparing `aioipinfo-0.1.0/src/aioipinfo/__main__.py` & `aioipinfo-0.1.1/src/aioipinfo/__main__.py`

 * *Files identical despite different names*

### Comparing `aioipinfo-0.1.0/src/aioipinfo.egg-info/PKG-INFO` & `aioipinfo-0.1.1/src/aioipinfo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipinfo
-Version: 0.1.0
+Version: 0.1.1
 Summary: The aioipinfo Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,17 +21,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/gormaniac/aioipinfo
-Project-URL: Documentation, https://gormo.com/aioipinfo/
+Project-URL: Documentation, https://gormo.co/aioipinfo/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aioipinfo
 
 A simple, async [ipinfo.io](https://ipinfo.io) client.
 
-Exposes an `IPInfoClient` that implements one querying method, `ipinfo`, and includes a CLI client that can be run with `python3 -m aioipinfo`. See the [full docs](https://gormo.com/aioipinfo/) for more details.
+Exposes an `IPInfoClient` that implements one querying method, `ipinfo`, and includes a CLI client that can be run with `python3 -m aioipinfo`. See the [full docs](https://gormo.co/aioipinfo/) for more details.
```

