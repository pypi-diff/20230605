# Comparing `tmp/xia_compiler_python-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_python-0.1.2-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 160365 bytes, number of entries: 7
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-03 19:08 xia_compiler_python/__init__.py
--rw-r--r--  2.0 unx   410112 b- defN 23-Jun-03 19:10 xia_compiler_python/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-03 19:10 xia_compiler_python-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      674 b- defN 23-Jun-03 19:10 xia_compiler_python-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-03 19:10 xia_compiler_python-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-03 19:10 xia_compiler_python-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      641 b- defN 23-Jun-03 19:10 xia_compiler_python-0.1.1.dist-info/RECORD
-7 files, 411813 bytes uncompressed, 159209 bytes compressed:  61.3%
+Zip file size: 134806 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-05 10:02 xia_compiler_python/__init__.py
+-rw-r--r--  2.0 unx   356920 b- defN 23-Jun-05 10:02 xia_compiler_python/compiler.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 10:02 xia_compiler_python-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      637 b- defN 23-Jun-05 10:02 xia_compiler_python-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 10:02 xia_compiler_python-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 10:02 xia_compiler_python-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      645 b- defN 23-Jun-05 10:02 xia_compiler_python-0.1.2.dist-info/RECORD
+7 files, 358597 bytes uncompressed, 133644 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_python/__init__.py
 Comment: 
 
-Filename: xia_compiler_python/compiler.cp39-win_amd64.pyd
+Filename: xia_compiler_python/compiler.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_compiler_python-0.1.1.dist-info/LICENSE.txt
+Filename: xia_compiler_python-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.1.dist-info/METADATA
+Filename: xia_compiler_python-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_python-0.1.1.dist-info/WHEEL
+Filename: xia_compiler_python-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_python-0.1.1.dist-info/top_level.txt
+Filename: xia_compiler_python-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.1.dist-info/RECORD
+Filename: xia_compiler_python-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_python/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_python.compiler import PythonCompiler
 
 
 __all__ = [
     "PythonCompiler"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

