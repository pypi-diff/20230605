# Comparing `tmp/jefferson-0.4.4.tar.gz` & `tmp/jefferson-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jefferson-0.4.4.tar", max compression
+gzip compressed data, was "jefferson-0.4.5.tar", max compression
```

## Comparing `jefferson-0.4.4.tar` & `jefferson-0.4.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1083 2023-05-22 19:56:39.859706 jefferson-0.4.4/LICENSE
--rwxr-xr-x   0        0        0      965 2023-05-22 19:56:39.863706 jefferson-0.4.4/README.md
--rw-r--r--   0        0        0        0 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/__init__.py
--rw-r--r--   0        0        0     1792 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/cli.py
--rw-r--r--   0        0        0        0 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/compression/__init__.py
--rw-r--r--   0        0        0      395 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/compression/jffs2_lzma.py
--rw-r--r--   0        0        0      829 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/compression/rtime.py
--rw-r--r--   0        0        0        0 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/core/__init__.py
--rw-r--r--   0        0        0    16776 2023-05-22 19:56:39.863706 jefferson-0.4.4/jefferson/jffs2.py
--rw-r--r--   0        0        0      825 2023-05-22 19:56:39.863706 jefferson-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 jefferson-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-05 12:42:15.142762 jefferson-0.4.5/LICENSE
+-rwxr-xr-x   0        0        0      965 2023-06-05 12:42:15.142762 jefferson-0.4.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 12:42:15.142762 jefferson-0.4.5/jefferson/__init__.py
+-rw-r--r--   0        0        0     1792 2023-06-05 12:42:15.142762 jefferson-0.4.5/jefferson/cli.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:42:15.142762 jefferson-0.4.5/jefferson/compression/__init__.py
+-rw-r--r--   0        0        0      395 2023-06-05 12:42:15.142762 jefferson-0.4.5/jefferson/compression/jffs2_lzma.py
+-rw-r--r--   0        0        0      829 2023-06-05 12:42:15.142762 jefferson-0.4.5/jefferson/compression/rtime.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:42:15.142762 jefferson-0.4.5/jefferson/core/__init__.py
+-rw-r--r--   0        0        0    16765 2023-06-05 12:42:15.142762 jefferson-0.4.5/jefferson/jffs2.py
+-rw-r--r--   0        0        0      825 2023-06-05 12:42:15.142762 jefferson-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 jefferson-0.4.5/PKG-INFO
```

### Comparing `jefferson-0.4.4/LICENSE` & `jefferson-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.4/README.md` & `jefferson-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.4/jefferson/cli.py` & `jefferson-0.4.5/jefferson/cli.py`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.4/jefferson/compression/rtime.py` & `jefferson-0.4.5/jefferson/compression/rtime.py`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.4/jefferson/jffs2.py` & `jefferson-0.4.5/jefferson/jffs2.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import stat
 import struct
 import sys
 import zlib
 from pathlib import Path
 
 import cstruct
-from lzallright.lzallright import LZOCompressor as lzo
+from lzallright import LZOCompressor as lzo
 
 import jefferson.compression.jffs2_lzma as jffs2_lzma
 import jefferson.compression.rtime as rtime
 
 
 def PAD(x):
     return ((x) + 3) & ~3
```

### Comparing `jefferson-0.4.4/pyproject.toml` & `jefferson-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jefferson"
-version = "0.4.4"
+version = "0.4.5"
 description = "JFFS2 filesystem extraction tool."
 authors = ["ONEKEY <support@onekey.com>", "Stefan Viehböck <support@onekey.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "jefferson" },
 ]
```

### Comparing `jefferson-0.4.4/PKG-INFO` & `jefferson-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jefferson
-Version: 0.4.4
+Version: 0.4.5
 Summary: JFFS2 filesystem extraction tool.
 License: MIT
 Author: ONEKEY
 Author-email: support@onekey.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

