# Comparing `tmp/polygons-0.3.0-cp39-none-win_amd64.whl.zip` & `tmp/polygons-0.3.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,7 @@
-Zip file size: 168800 bytes, number of entries: 4
--rw-r--r--  4.6 unx     4534 b- defN 21-Apr-09 11:45 polygons-0.3.0.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 21-Apr-09 11:45 polygons-0.3.0.dist-info/WHEEL
--rwxr-xr-x  4.6 unx   402944 b- defN 21-Apr-09 11:45 polygons.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      295 b- defN 21-Apr-09 11:45 polygons-0.3.0.dist-info/RECORD
-4 files, 407868 bytes uncompressed, 168226 bytes compressed:  58.8%
+Zip file size: 193926 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     4459 b- defN 23-Jun-05 17:56 polygons-0.3.2.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jun-05 17:56 polygons-0.3.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx      115 b- defN 23-Jun-05 17:56 polygons/__init__.py
+-rwxr-xr-x  4.6 unx   471552 b- defN 23-Jun-05 17:56 polygons/polygons.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      380 b- defN 23-Jun-05 17:56 polygons-0.3.2.dist-info/RECORD
+5 files, 476600 bytes uncompressed, 193224 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
-Filename: polygons-0.3.0.dist-info/METADATA
+Filename: polygons-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: polygons-0.3.0.dist-info/WHEEL
+Filename: polygons-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: polygons.cp39-win_amd64.pyd
+Filename: polygons/__init__.py
 Comment: 
 
-Filename: polygons-0.3.0.dist-info/RECORD
+Filename: polygons/polygons.cp39-win_amd64.pyd
 Comment: 
 
-Zip file comment: zip-rs
+Filename: polygons-0.3.2.dist-info/RECORD
+Comment: 
+
+Zip file comment:
```

## Comparing `polygons-0.3.0.dist-info/METADATA` & `polygons-0.3.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: polygons
-Version: 0.3.0
-Classifiers: Programming Language :: Python
+Version: 0.3.2
 Summary: Fast points-in-polygon test and distances to polygons.
 Home-Page: https://github.com/bast/polygons
 Author: Radovan Bast <bast@users.noreply.github.com>
-Author-Email: Radovan Bast <bast@users.noreply.github.com>
+Author-email: Radovan Bast <bast@users.noreply.github.com>
 License: GPL-3.0-only
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 [![test status](https://github.com/bast/polygons/workflows/Test/badge.svg)](https://github.com/bast/polygons/actions)
 [![license badge](https://img.shields.io/badge/license-%20GPL-blue.svg)](LICENSE)
 [![link to Crates](https://img.shields.io/crates/v/polygons.svg)](https://crates.io/crates/polygons)
 [![link to PyPI](https://badge.fury.io/py/polygons.svg)](https://badge.fury.io/py/polygons)
 [![link to Zenodo/DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3825616.svg)](https://doi.org/10.5281/zenodo.3825616)
@@ -35,15 +33,15 @@
 
 ```
 $ pip install polygons
 ```
 
 ## Supported versions
 
-- Python: 3.6, 3.7, 3.8, 3.9
+- Python: 3.8 - 3.10
 - Operating systems: Linux, macOS, and Windows
 
 
 ## Capabilities
 
 - Check whether points are inside or outside polygons
 - Nearest distances to edges
```

