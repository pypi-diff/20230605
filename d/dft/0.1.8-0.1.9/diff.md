# Comparing `tmp/dft-0.1.8-py3-none-any.whl.zip` & `tmp/dft-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 3765 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-17 10:52 dft/__init__.py
--rw-r--r--  2.0 unx     2635 b- defN 22-Jun-17 10:52 dft/df_plot.py
--rwxr-xr-x  2.0 unx       60 b- defN 22-Jun-17 10:52 dft-0.1.8.data/scripts/dft
--rw-r--r--  2.0 unx       57 b- defN 22-Jun-17 10:52 execution_handler/__init__.py
--rw-r--r--  2.0 unx      137 b- defN 22-Jun-17 10:52 execution_handler/base_execution_handler.py
--rw-r--r--  2.0 unx     1074 b- defN 22-Jun-17 10:52 dft-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      826 b- defN 22-Jun-17 10:52 dft-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jun-17 10:52 dft-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 22-Jun-17 10:52 dft-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      769 b- defN 22-Jun-17 10:52 dft-0.1.8.dist-info/RECORD
-10 files, 5672 bytes uncompressed, 2451 bytes compressed:  56.8%
+Zip file size: 4027 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       78 b- defN 22-Jun-17 11:09 dft/__init__.py
+-rw-r--r--  2.0 unx       57 b- defN 22-Jun-17 11:09 dft/execution_handler/__init__.py
+-rw-r--r--  2.0 unx      137 b- defN 22-Jun-17 11:09 dft/execution_handler/base_execution_handler.py
+-rw-r--r--  2.0 unx       22 b- defN 22-Jun-17 11:09 dft/plotting/__init__.py
+-rw-r--r--  2.0 unx     2635 b- defN 22-Jun-17 11:09 dft/plotting/df_plot.py
+-rwxr-xr-x  2.0 unx       60 b- defN 22-Jun-17 11:09 dft-0.1.9.data/scripts/dft
+-rw-r--r--  2.0 unx     1074 b- defN 22-Jun-17 11:09 dft-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      826 b- defN 22-Jun-17 11:09 dft-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jun-17 11:09 dft-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 22-Jun-17 11:09 dft-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      865 b- defN 22-Jun-17 11:09 dft-0.1.9.dist-info/RECORD
+11 files, 5850 bytes uncompressed, 2555 bytes compressed:  56.3%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: dft/__init__.py
 Comment: 
 
-Filename: dft/df_plot.py
+Filename: dft/execution_handler/__init__.py
 Comment: 
 
-Filename: dft-0.1.8.data/scripts/dft
+Filename: dft/execution_handler/base_execution_handler.py
 Comment: 
 
-Filename: execution_handler/__init__.py
+Filename: dft/plotting/__init__.py
 Comment: 
 
-Filename: execution_handler/base_execution_handler.py
+Filename: dft/plotting/df_plot.py
 Comment: 
 
-Filename: dft-0.1.8.dist-info/LICENSE
+Filename: dft-0.1.9.data/scripts/dft
 Comment: 
 
-Filename: dft-0.1.8.dist-info/METADATA
+Filename: dft-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: dft-0.1.8.dist-info/WHEEL
+Filename: dft-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: dft-0.1.8.dist-info/top_level.txt
+Filename: dft-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: dft-0.1.8.dist-info/RECORD
+Filename: dft-0.1.9.dist-info/top_level.txt
+Comment: 
+
+Filename: dft-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dft/__init__.py

```diff
@@ -0,0 +1,5 @@
+00000000: 6672 6f6d 202e 706c 6f74 7469 6e67 2069  from .plotting i
+00000010: 6d70 6f72 7420 2a0a 6672 6f6d 202e 6578  mport *.from .ex
+00000020: 6563 7574 696f 6e5f 6861 6e64 6c65 7220  ecution_handler 
+00000030: 696d 706f 7274 2062 6173 655f 6578 6563  import base_exec
+00000040: 7574 696f 6e5f 6861 6e64 6c65 720a       ution_handler.
```

## Comparing `dft/df_plot.py` & `dft/plotting/df_plot.py`

 * *Files identical despite different names*

## Comparing `dft-0.1.8.dist-info/LICENSE` & `dft-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dft-0.1.8.dist-info/METADATA` & `dft-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dft
-Version: 0.1.8
+Version: 0.1.9
 Summary: DF Package
 Home-page: https://github.com/TBD
 Author: Data Facade
 Author-email: info@data-facade.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

