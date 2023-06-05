# Comparing `tmp/vsdeinterlace-0.5.0.tar.gz` & `tmp/vsdeinterlace-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdeinterlace-0.5.0.tar", last modified: Thu May  4 22:00:07 2023, max compression
+gzip compressed data, was "vsdeinterlace-0.5.1.tar", last modified: Mon Jun  5 14:35:02 2023, max compression
```

## Comparing `vsdeinterlace-0.5.0.tar` & `vsdeinterlace-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:07.764684 vsdeinterlace-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-04 22:00:07.764684 vsdeinterlace-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-04 22:00:07.764684 vsdeinterlace-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:07.760684 vsdeinterlace-0.5.0/vsdeinterlace/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/vsdeinterlace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/vsdeinterlace/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/vsdeinterlace/blending.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/vsdeinterlace/combing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/vsdeinterlace/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/vsdeinterlace/ivtc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/vsdeinterlace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-04 21:59:33.000000 vsdeinterlace-0.5.0/vsdeinterlace/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:07.764684 vsdeinterlace-0.5.0/vsdeinterlace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-04 22:00:07.000000 vsdeinterlace-0.5.0/vsdeinterlace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-04 22:00:07.000000 vsdeinterlace-0.5.0/vsdeinterlace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:00:07.000000 vsdeinterlace-0.5.0/vsdeinterlace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 22:00:07.000000 vsdeinterlace-0.5.0/vsdeinterlace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 22:00:07.000000 vsdeinterlace-0.5.0/vsdeinterlace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:35:02.633328 vsdeinterlace-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-05 14:35:02.633328 vsdeinterlace-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-05 14:35:02.633328 vsdeinterlace-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:35:02.629328 vsdeinterlace-0.5.1/vsdeinterlace/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/vsdeinterlace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/vsdeinterlace/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/vsdeinterlace/blending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/vsdeinterlace/combing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/vsdeinterlace/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/vsdeinterlace/ivtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/vsdeinterlace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-05 14:34:35.000000 vsdeinterlace-0.5.1/vsdeinterlace/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:35:02.633328 vsdeinterlace-0.5.1/vsdeinterlace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-05 14:35:02.000000 vsdeinterlace-0.5.1/vsdeinterlace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-05 14:35:02.000000 vsdeinterlace-0.5.1/vsdeinterlace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:35:02.000000 vsdeinterlace-0.5.1/vsdeinterlace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 14:35:02.000000 vsdeinterlace-0.5.1/vsdeinterlace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 14:35:02.000000 vsdeinterlace-0.5.1/vsdeinterlace.egg-info/top_level.txt
```

### Comparing `vsdeinterlace-0.5.0/LICENSE` & `vsdeinterlace-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdeinterlace-0.5.0/PKG-INFO` & `vsdeinterlace-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdeinterlace
-Version: 0.5.0
+Version: 0.5.1
 Summary: VapourSynth deinterlacing and interlaced/telecined content helper functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-deinterlace
 Project-URL: Documentation, https://vsdeinterlace.encode.moe/en/latest/
```

### Comparing `vsdeinterlace-0.5.0/setup.cfg` & `vsdeinterlace-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsdeinterlace-0.5.0/setup.py` & `vsdeinterlace-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `vsdeinterlace-0.5.0/vsdeinterlace/blending.py` & `vsdeinterlace-0.5.1/vsdeinterlace/blending.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     """
 
     if isinstance(bobbed, tuple):
         bob0, bob1 = bobbed
     else:
         bob0, bob1 = bobbed.std.SelectEvery(2, 0), bobbed.std.SelectEvery(2, 1)
 
-    ab0, bc0, c0 = shift_clip_multi(bob0, (0, 1, 2))
+    ab0, bc0, c0 = shift_clip_multi(bob0, (0, 2))
     bc1, ab1, a1 = shift_clip_multi(bob1)
 
     deblended = norm_expr([a1, ab1, ab0, bc1, bc0, c0], ('b', 'y x - z + b c - a + + 2 /'))
 
     if fieldmatched:
         return deblending_helper(fieldmatched, deblended)
```

### Comparing `vsdeinterlace-0.5.0/vsdeinterlace/combing.py` & `vsdeinterlace-0.5.1/vsdeinterlace/combing.py`

 * *Files identical despite different names*

### Comparing `vsdeinterlace-0.5.0/vsdeinterlace/funcs.py` & `vsdeinterlace-0.5.1/vsdeinterlace/funcs.py`

 * *Files identical despite different names*

### Comparing `vsdeinterlace-0.5.0/vsdeinterlace/ivtc.py` & `vsdeinterlace-0.5.1/vsdeinterlace/ivtc.py`

 * *Files identical despite different names*

### Comparing `vsdeinterlace-0.5.0/vsdeinterlace/utils.py` & `vsdeinterlace-0.5.1/vsdeinterlace/utils.py`

 * *Files identical despite different names*

### Comparing `vsdeinterlace-0.5.0/vsdeinterlace.egg-info/PKG-INFO` & `vsdeinterlace-0.5.1/vsdeinterlace.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdeinterlace
-Version: 0.5.0
+Version: 0.5.1
 Summary: VapourSynth deinterlacing and interlaced/telecined content helper functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-deinterlace
 Project-URL: Documentation, https://vsdeinterlace.encode.moe/en/latest/
```

