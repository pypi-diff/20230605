# Comparing `tmp/fafbseg-1.8.0.tar.gz` & `tmp/fafbseg-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fafbseg-1.8.0.tar", last modified: Tue Feb 15 08:46:24 2022, max compression
+gzip compressed data, was "dist/fafbseg-1.9.0.tar", last modified: Mon Mar 28 18:19:20 2022, max compression
```

## Comparing `fafbseg-1.8.0.tar` & `fafbseg-1.9.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (116)    35149 2022-02-15 08:46:15.000000 fafbseg-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       81 2022-02-15 08:46:15.000000 fafbseg-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2022-02-15 08:46:24.000000 fafbseg-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      589 2022-02-15 08:46:15.000000 fafbseg-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg/
--rw-r--r--   0 runner    (1001) docker     (116)      831 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       53 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg/data/
--rw-r--r--   0 runner    (1001) docker     (116)      361 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/data/README.md
--rw-r--r--   0 runner    (1001) docker     (116)  6763875 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/data/global_area_ids.npy.zip
--rw-r--r--   0 runner    (1001) docker     (116)     1109 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/data/volume_name_dict.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg/flywire/
--rw-r--r--   0 runner    (1001) docker     (116)      937 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18703 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/_synapses_spine.py
--rw-r--r--   0 runner    (1001) docker     (116)    16513 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/annotations.py
--rw-r--r--   0 runner    (1001) docker     (116)    24305 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/l2.py
--rw-r--r--   0 runner    (1001) docker     (116)     4988 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/merge.py
--rw-r--r--   0 runner    (1001) docker     (116)     8173 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/meshes.py
--rw-r--r--   0 runner    (1001) docker     (116)    17468 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (116)    40801 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (116)    14620 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/skeletonize.py
--rw-r--r--   0 runner    (1001) docker     (116)    29756 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/synapses.py
--rw-r--r--   0 runner    (1001) docker     (116)     9553 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/flywire/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg/google/
--rw-r--r--   0 runner    (1001) docker     (116)      807 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10785 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/google/meshes.py
--rw-r--r--   0 runner    (1001) docker     (116)    29918 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/google/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (116)     4684 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/google/synapses.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg/move/
--rw-r--r--   0 runner    (1001) docker     (116)      748 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/move/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8240 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/move/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (116)    23835 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/move/merge.py
--rw-r--r--   0 runner    (1001) docker     (116)    15944 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/move/merge_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg/spine/
--rw-r--r--   0 runner    (1001) docker     (116)      785 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/spine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    26221 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/spine/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg/synapses/
--rw-r--r--   0 runner    (1001) docker     (116)      816 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/synapses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    25192 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/synapses/offline.py
--rw-r--r--   0 runner    (1001) docker     (116)    18825 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/synapses/online.py
--rw-r--r--   0 runner    (1001) docker     (116)     7442 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/synapses/transmitters.py
--rw-r--r--   0 runner    (1001) docker     (116)    12862 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/synapses/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2764 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg/xform/
--rw-r--r--   0 runner    (1001) docker     (116)      756 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/xform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13899 2022-02-15 08:46:15.000000 fafbseg-1.8.0/fafbseg/xform/xform.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1144 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      206 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2022-02-15 08:46:24.000000 fafbseg-1.8.0/fafbseg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-02-15 08:46:24.000000 fafbseg-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1505 2022-02-15 08:46:15.000000 fafbseg-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)    35149 2022-03-28 18:19:13.000000 fafbseg-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2022-03-28 18:19:13.000000 fafbseg-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     1394 2022-03-28 18:19:20.000000 fafbseg-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      591 2022-03-28 18:19:13.000000 fafbseg-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg/
+-rw-r--r--   0 runner    (1001) docker     (116)      831 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg/data/
+-rw-r--r--   0 runner    (1001) docker     (116)      361 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)  6763875 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/data/global_area_ids.npy.zip
+-rw-r--r--   0 runner    (1001) docker     (116)     1109 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/data/volume_name_dict.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg/flywire/
+-rw-r--r--   0 runner    (1001) docker     (116)      937 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18703 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/_synapses_spine.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19460 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24511 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/l2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5073 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/merge.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8178 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17478 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (116)    51863 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14865 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/skeletonize.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29754 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/synapses.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10093 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/flywire/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg/google/
+-rw-r--r--   0 runner    (1001) docker     (116)      807 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10785 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/google/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29912 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/google/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4685 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/google/synapses.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg/move/
+-rw-r--r--   0 runner    (1001) docker     (116)      748 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/move/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8240 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/move/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23835 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/move/merge.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15944 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/move/merge_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg/spine/
+-rw-r--r--   0 runner    (1001) docker     (116)      785 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/spine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26263 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/spine/base.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg/synapses/
+-rw-r--r--   0 runner    (1001) docker     (116)      816 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/synapses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25192 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/synapses/offline.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18825 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/synapses/online.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7442 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/synapses/transmitters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12862 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/synapses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3389 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg/xform/
+-rw-r--r--   0 runner    (1001) docker     (116)      756 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/xform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13899 2022-03-28 18:19:13.000000 fafbseg-1.9.0/fafbseg/xform/xform.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1394 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1144 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      206 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2022-03-28 18:19:20.000000 fafbseg-1.9.0/fafbseg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-03-28 18:19:20.000000 fafbseg-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1505 2022-03-28 18:19:13.000000 fafbseg-1.9.0/setup.py
```

### Comparing `fafbseg-1.8.0/LICENSE` & `fafbseg-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/PKG-INFO` & `fafbseg-1.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fafbseg
-Version: 1.8.0
+Version: 1.9.0
 Summary: Tools to work with auto-segmented FAFB data
 Home-page: https://github.com/flyconnectome/fafbseg-py
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Keywords: FAFB neuron segmentation flywire Google synapses
 Platform: UNKNOWN
@@ -32,11 +32,11 @@
 
 ```bash
 pip3 install fafbseg
 ```
 
 Install from Github
 ```bash
-pip3 install git+git://github.com/flyconnectome/fafbseg-py.git
+pip3 install git+https://github.com/flyconnectome/fafbseg-py.git
 ```
```

### Comparing `fafbseg-1.8.0/README.md` & `fafbseg-1.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 
 ```bash
 pip3 install fafbseg
 ```
 
 Install from Github
 ```bash
-pip3 install git+git://github.com/flyconnectome/fafbseg-py.git
+pip3 install git+https://github.com/flyconnectome/fafbseg-py.git
 ```
```

### Comparing `fafbseg-1.8.0/fafbseg/__init__.py` & `fafbseg-1.9.0/fafbseg/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/data/global_area_ids.npy.zip` & `fafbseg-1.9.0/fafbseg/data/global_area_ids.npy.zip`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/data/volume_name_dict.json` & `fafbseg-1.9.0/fafbseg/data/volume_name_dict.json`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/flywire/__init__.py` & `fafbseg-1.9.0/fafbseg/flywire/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/flywire/_synapses_spine.py` & `fafbseg-1.9.0/fafbseg/flywire/_synapses_spine.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/flywire/annotations.py` & `fafbseg-1.9.0/fafbseg/flywire/annotations.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,27 +13,110 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
 """Functions to fetch and set annotations in FlyWire using the annotation
 framework and the materialization engine."""
 
 import navis
+import requests
 
 import datetime as dt
 import numpy as np
 import pandas as pd
 
+from ..utils import make_iterable
 from .utils import get_cave_client, retry
-from .segmentation import locs_to_segments
+from .segmentation import locs_to_segments, supervoxels_to_roots, is_latest_root
 
 
 __all__ = ['get_somas', 'get_materialization_versions',
            'create_annotation_table', 'get_annotation_tables',
            'get_annotation_table_info', 'get_annotations',
-           'delete_annotations', 'upload_annotations']
+           'delete_annotations', 'upload_annotations',
+           'is_proofread']
+
+
+PR_TABLE = None
+PR_META = None
+
+
+def is_proofread(x, cache=True):
+    """Test if neuron has been set to `proofread`.
+
+    Under the hood, this uses a cached version of the proofreading table which
+    is updated everytime this function gets called.
+
+    Parameters
+    ----------
+    x  :            int | list of int
+                    Root IDs to check.
+    cache :         bool
+                    Use and update a locally cached version of the proofreading
+                    table. Setting this to ``False`` will force fetching the
+                    full table which is considerably slower.
+
+    Returns
+    -------
+    proofread :     np.ndarray
+                    Boolean array.
+
+    """
+    global PR_TABLE, PR_META
+
+    if not isinstance(x, (np.ndarray, set, list, pd.Series)):
+        x = [x]
+
+    # Force into array and convert to integer
+    x = np.asarray(x).astype(np.int64)
+
+    # Check if any of the roots are outdated -> can't check those
+    il = is_latest_root(x)
+    if any(~il):
+        raise ValueError(f' Root ID(s) outdated: {x[~il]}')
+
+    # Get available materialization versions
+    client = get_cave_client('production')
+    mat_versions = client.materialize.get_versions()
+
+    # Check if the cached version is outdated
+    if cache and PR_META:
+        if max(mat_versions) > PR_META['mat_version']:
+            PR_TABLE = None
+            PR_META = None
+
+    # If nothing cached catch the table from scratch
+    if isinstance(PR_TABLE, type(None)) or not cache:
+        # This ought to automatically use the most recent materialization version
+        PR_META = dict(timestamp=dt.datetime.utcnow(),
+                       mat_version=max(mat_versions))
+        PR_TABLE = client.materialize.live_query(table='proofreading_status_public_v1',
+                                                 timestamp=PR_META['timestamp'])
+        # Only keep relevant rows and columns
+        PR_TABLE = PR_TABLE.loc[PR_TABLE.valid == 't', ['pt_supervoxel_id', 'pt_root_id']]
+    else:
+        # Update root IDs
+        now = dt.datetime.utcnow()
+        # get_delta_roots currently acts up if there are no new roots
+        # (i.e. if this gets called in quick succession)
+        try:
+            old_roots, _ = client.chunkedgraph.get_delta_roots(PR_META['timestamp'], now)
+        except requests.exceptions.HTTPError as e:
+            if "need at least one array" in str(e):
+                old_roots = []
+            else:
+                raise
+        except BaseException:
+            raise
+
+        to_update = PR_TABLE.pt_root_id.isin(old_roots)
+        if any(to_update):
+            PR_TABLE.loc[to_update, 'pt_root_id'] = supervoxels_to_roots(PR_TABLE.loc[to_update, 'pt_supervoxel_id'].values)
+        PR_META['timestamp'] = now
+
+    return np.isin(x, PR_TABLE.pt_root_id.values)
 
 
 def get_materialization_versions(dataset='production'):
     """Fetch info on the available materializations."""
     # Get/Initialize the CAVE client
     client = get_cave_client(dataset)
 
@@ -163,17 +246,17 @@
     client = get_cave_client(dataset)
 
     return client.annotation.get_table_metadata(table_name)
 
 
 def get_annotations(table_name: str,
                     materialization='live',
-                    split_positions=False,
+                    split_positions: bool = False,
                     drop_invalid: bool = True,
-                    dataset='production',
+                    dataset: str = 'production',
                     **filters):
     """Get annotations from given table.
 
     Parameters
     ----------
     table_name :        str
                         Name of the table.
@@ -380,17 +463,17 @@
     """
     if isinstance(x, navis.BaseNeuron):
         x = navis.NeuronList(x)
 
     filter_in_dict = None
     if not isinstance(x, type(None)):
         if isinstance(x, navis.NeuronList):
-            root_ids = x.id.astype(int)
+            root_ids = x.id.astype(np.int64)
         else:
-            root_ids = navis.utils.make_iterable(x).astype(int)
+            root_ids = make_iterable(x, force_type=np.int64)
         filter_in_dict = {'pt_root_id': root_ids}
 
     nuc = get_annotations('nuclei_v1',
                           materialization=materialization,
                           split_positions=split_positions,
                           dataset=dataset,
                           filter_in_dict=filter_in_dict)
```

### Comparing `fafbseg-1.8.0/fafbseg/flywire/l2.py` & `fafbseg-1.9.0/fafbseg/flywire/l2.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     0  720575940614131061        286               2  2364.39616  132.467837     60.271   [305456, 311184, ...
 
     """
     if navis.utils.is_iterable(root_ids):
         root_ids = np.unique(root_ids)
         info = []
         with ThreadPoolExecutor(max_workers=max_threads) as pool:
-            func = retry(partial(l2_info, dataset=dataset))
+            func = partial(l2_info, dataset=dataset)
             futures = pool.map(func, root_ids)
             info = [f for f in navis.config.tqdm(futures,
                                                  desc='Fetching L2 info',
                                                  total=len(root_ids),
                                                  disable=not progress or len(root_ids) == 1,
                                                  leave=False)]
         return pd.concat(info, axis=0)
@@ -86,24 +86,25 @@
     # Get/Initialize the CAVE client
     client = get_cave_client(dataset)
 
     get_l2_ids = partial(retry(client.chunkedgraph.get_leaves), stop_layer=2)
     l2_ids = get_l2_ids(root_ids)
 
     attributes = ['area_nm2', 'size_nm3', 'max_dt_nm', 'rep_coord_nm']
-    info = client.l2cache.get_l2data(l2_ids.tolist(), attributes=attributes)
+    get_l2data = retry(client.l2cache.get_l2data)
+    info = get_l2data(l2_ids.tolist(), attributes=attributes)
     n_miss = len([v for v in info.values() if not v])
 
     row = [root_ids, len(l2_ids), n_miss]
     info_df = pd.DataFrame([row],
                            columns=['root_id', 'l2_chunks', 'chunks_missing'])
 
     # Collect L2 attributes
     for at in attributes:
-        if at in ('rep_coord_nm'):
+        if at in ('rep_coord_nm', ):
             continue
 
         summed = sum([v.get(at, 0) for v in info.values()])
         if at.endswith('3'):
             summed /= 1000**3
         elif at.endswith('2'):
             summed /= 1000**2
@@ -318,15 +319,16 @@
     ch_dims = np.squeeze(ch_dims)
 
     xyz = swc[['x', 'y', 'z']].values
     swc[['x', 'y', 'z']] = chunks_to_nm(xyz, vol) + ch_dims / 2
 
     if refine:
         # Get the L2 representative coordinates
-        l2_info = client.l2cache.get_l2data(l2_ids.tolist(), attributes=['rep_coord_nm'])
+        get_l2data = retry(client.l2cache.get_l2data)
+        l2_info = get_l2data(l2_ids.tolist(), attributes=['rep_coord_nm'])
         # Missing L2 chunks will be {'id': {}}
         new_co = {l2dict[int(k)]: v['rep_coord_nm'] for k, v in l2_info.items() if v}
 
         # Map refined coordinates onto the SWC
         has_new = swc.node_id.isin(new_co)
 
         # Only apply if we actually have new coordinates - otherwise there
@@ -360,15 +362,16 @@
     return tn
 
 
 def l2_dotprops(root_ids, min_size=None, omit_failures=None, progress=True,
                 max_threads=10, dataset='production', **kwargs):
     """Generate dotprops from L2 chunks.
 
-    L2 chunks not present in the L2 cache are silently ignored.
+    L2 chunks not present in the L2 cache or without a `pca` attribute
+    (happens for very small chunks) are silently ignored.
 
     Parameters
     ----------
     root_ids  :         int | list of ints
                         Root ID(s) of the FlyWire neuron(s) you want to
                         dotprops for.
     min_size :          int, optional
@@ -450,23 +453,24 @@
         attributes.append('size_nm3')
 
     l2_info = {}
     with navis.config.tqdm(desc='Fetching L2 vectors',
                            disable=not progress,
                            total=len(l2_ids_all),
                            leave=False) as pbar:
-        func = retry(client.l2cache.get_l2data)
+        get_l2data = retry(client.l2cache.get_l2data)
         for chunk_ix in np.arange(0, len(l2_ids_all), chunk_size):
             chunk = l2_ids_all[chunk_ix: chunk_ix + chunk_size]
-            l2_info.update(func(chunk.tolist(), attributes=attributes))
+            l2_info.update(get_l2data(chunk.tolist(), attributes=attributes))
             pbar.update(len(chunk))
 
     # L2 chunks without info will show as empty dictionaries
     # Let's drop them to make our life easier (speeds up indexing too)
-    l2_info = {k: v for k, v in l2_info.items() if v}
+    # Note that small L2 chunks won't have a `pca`
+    l2_info = {k: v for k, v in l2_info.items() if 'pca' in v}
 
     # Generate dotprops
     dps = []
     for root, ids in navis.config.tqdm(zip(root_ids, l2_ids),
                                        desc='Creating dotprops',
                                        total=len(root_ids),
                                        disable=not progress or len(root_ids) <= 1,
```

### Comparing `fafbseg-1.8.0/fafbseg/flywire/merge.py` & `fafbseg-1.9.0/fafbseg/flywire/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,12 +124,15 @@
 
     # Xform to FAFB
     n_fafb = xform.flywire_to_fafb14(n_fw, on_fail='raise', coordinates='nm', inplace=False)
     mesh_fafb = xform.flywire_to_fafb14(tm.Trimesh(mesh.vertices, mesh.faces),
                                         on_fail='raise', coordinates='nm', inplace=False)
 
     # Heal neuron
-    n_fafb = navis.heal_fragmented_neuron(n_fafb)
+    try:
+        n_fafb = navis.heal_skeleton(n_fafb)
+    except AttributeError:
+        n_fafb = navis.heal_fragmented_neuron(n_fafb)
 
     # Merge neuron
     return merge_into_catmaid(n_fafb, target_instance=target_instance, tag=tag,
                               mesh=mesh_fafb, **kwargs)
```

### Comparing `fafbseg-1.8.0/fafbseg/flywire/meshes.py` & `fafbseg-1.9.0/fafbseg/flywire/meshes.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     >>> m = flywire.get_mesh_neuron(720575940614131061)
     >>> m.plot3d()  # doctest: +SKIP
 
     """
     vol = parse_volume(dataset)
 
     if navis.utils.is_iterable(id):
-        id = np.asarray(id).astype(int)
+        id = np.asarray(id).astype(np.int64)
         if 0 in id:
             raise ValueError('Root ID 0 among the queried IDs')
 
         if not threads or threads == 1:
             return navis.NeuronList([get_mesh_neuron(n, dataset=dataset,
                                                      with_synapses=with_synapses)
                                      for n in navis.config.tqdm(id,
```

### Comparing `fafbseg-1.8.0/fafbseg/flywire/neuroglancer.py` & `fafbseg-1.9.0/fafbseg/flywire/neuroglancer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import matplotlib.colors as mcl
 import numpy as np
 import pandas as pd
 
 from urllib.parse import urlparse, parse_qs, quote
 
 from . import utils
+from ..utils import make_iterable
 
 __all__ = ['decode_url', 'encode_url']
 
 NGL_URL = 'https://ngl.flywire.ai'
 MINIMAL_SCENE = {'layers': [{'source': 'precomputed://gs://microns-seunglab/drosophila_v0/alignment/image_rechunked',
                              'type': 'image',
                              'blend': 'default',
@@ -139,23 +140,23 @@
             scene['layers'][-1]['name'] = 'sandbox-segmentation-FOR PRACTICE ONLY'
     else:
         seg_layer_ix = seg_layer_ix[0]
 
     # If provided, add segments
     if not isinstance(segments, type(None)):
         # Force to list and make strings
-        segments = navis.utils.make_iterable(segments, force_type=str).tolist()
+        segments = make_iterable(segments, force_type=str).tolist()
 
         # Add to, not replace already selected segments
         present = scene['layers'][seg_layer_ix].get('segments', [])
         scene['layers'][seg_layer_ix]['segments'] = present + segments
 
     if not isinstance(invis_segs, type(None)):
         # Force to list and make strings
-        invis_segs = navis.utils.make_iterable(invis_segs, force_type=str).tolist()
+        invis_segs = make_iterable(invis_segs, force_type=str).tolist()
 
         # Add to, not replace already selected segments
         present = scene['layers'][seg_layer_ix].get('hiddenSegments', [])
         scene['layers'][seg_layer_ix]['hiddenSegments'] = present + invis_segs
 
     # All present segments
     seg_layer = scene['layers'][seg_layer_ix]
```

### Comparing `fafbseg-1.8.0/fafbseg/flywire/segmentation.py` & `fafbseg-1.9.0/fafbseg/flywire/segmentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,36 +15,144 @@
 
 import pymaid
 import navis
 import requests
 import textwrap
 import time
 
+import cloudvolume as cv
 import datetime as dt
 import numpy as np
 import pandas as pd
+import networkx as nx
 
 from concurrent import futures
 from diskcache import Cache
 from requests_futures.sessions import FuturesSession
 from scipy import ndimage
 from tqdm.auto import trange, tqdm
 
 from .. import spine
 from .. import xform
 
+from ..utils import make_iterable
 from .utils import (parse_volume, FLYWIRE_DATASETS, get_chunkedgraph_secret,
-                    retry, get_cave_client)
+                    retry, get_cave_client, parse_bounds)
 
 
 __all__ = ['fetch_edit_history', 'fetch_leaderboard', 'locs_to_segments',
            'locs_to_supervoxels', 'skid_to_id', 'update_ids',
            'roots_to_supervoxels', 'supervoxels_to_roots',
            'neuron_to_segments', 'is_latest_root', 'is_valid_root',
-           'is_valid_supervoxel']
+           'is_valid_supervoxel', 'get_voxels', 'get_lineage_graph']
+
+
+def get_lineage_graph(x, size=False, user=False, synapses=False,
+                      proofreading_status=False, progress=True,
+                      dataset='production'):
+    """Get lineage graph for given neuron.
+
+    This piggy-backs on the CAVEclient but importantly we remap users and
+    operation IDs such that each node's labels refer to the operation that
+    created them.
+
+    Parameters
+    ----------
+    x :         int
+                A single root ID.
+    size :      bool
+                If True, will add `size` and `survivals` node attributes. The
+                former indicates the number of supervoxels, the latter how many
+                of these supervoxels made it into `x`.
+    synapses :  bool
+                If True, will add `pre|post|synapses` node attributes which
+                indicate how many of the synapses in `x` came from this fragment.
+                Note that this doesn't tell you e.g. how many false-positive
+                synapses were removed via a split. This works only if the root
+                ID is up-to-date.
+    user :      bool
+                If True, will add user `user` node attribute.
+    proofreading_status : bool
+                If True, will add a `proofread_by` node attribute indicating if
+                a user has set a given root ID to proofread.
+
+    Returns
+    -------
+    networkx.DiGraph
+
+    """
+    x = int(x)
+
+    client = get_cave_client(dataset=dataset)
+    G = client.chunkedgraph.get_lineage_graph(x, as_nx_graph=True)
+
+    # Remap operation ID
+    op_remapped = {}
+    for n in G:
+        pred = list(G.predecessors(n))
+        if pred:
+            op_remapped[n] = G.nodes[pred[0]]['operation_id']
+
+    # Remove existing operation IDs
+    for n in G.nodes:
+        G.nodes[n].pop('operation_id', None)
+    # Apply new IDs
+    nx.set_node_attributes(G, op_remapped, name='operation_id')
+
+    if user:
+        op_ids = nx.get_node_attributes(G, "operation_id")
+        details = client.chunkedgraph.get_operation_details(list(op_ids.values()))
+        users = {n: details[str(o)]['user'] for n, o in op_ids.items()}
+        nx.set_node_attributes(G, users, name='user')
+
+    if size:
+        sv = roots_to_supervoxels(list(G.nodes), dataset=dataset, progress=progress)
+        sizes = {n: len(sv[n]) for n in G.nodes}
+        nx.set_node_attributes(G, sizes, name='size')
+
+        survivors = {n: int(np.isin(sv[n], sv[x]).sum()) for n in G.nodes}
+        nx.set_node_attributes(G, survivors, name='survivors')
+    else:
+        sv = None
+
+    if synapses:
+        pre = client.materialize.live_query(
+                        table=client.materialize.synapse_table,
+                        filter_equal_dict=dict(pre_pt_root_id=x),
+                        timestamp=dt.datetime.now(),
+                        select_columns=['pre_pt_supervoxel_id',
+                                        'post_pt_supervoxel_id']
+                                        )
+        post = client.materialize.live_query(
+                        table=client.materialize.synapse_table,
+                        filter_equal_dict=dict(post_pt_root_id=x),
+                        timestamp=dt.datetime.now(),
+                        select_columns=['pre_pt_supervoxel_id',
+                                        'post_pt_supervoxel_id']
+                                        )
+        if isinstance(sv, type(None)):
+            sv = roots_to_supervoxels(list(G.nodes), dataset=dataset, progress=progress)
+
+        n_pre = {n: int(pre.pre_pt_supervoxel_id.isin(sv[n]).sum()) for n in G.nodes}
+        n_post = {n: int(post.post_pt_supervoxel_id.isin(sv[n]).sum()) for n in G.nodes}
+        n_syn = {n: n_pre[n] + n_post[n] for n in G.nodes}
+        nx.set_node_attributes(G, n_pre, name='presynapses')
+        nx.set_node_attributes(G, n_post, name='postsynapses')
+        nx.set_node_attributes(G, n_post, name='synapses')
+
+    if proofreading_status:
+        from .annotations import get_annotations
+        nodes = np.array(list(G.nodes)).astype(np.int64)
+        pr = get_annotations('proofreading_status_public_v1',
+                             filter_in_dict=dict(valid_id=nodes))
+        if len(pr):
+            user = pr.groupby('valid_id').user_id.apply(list).to_dict()
+            nx.set_node_attributes(G, {n: user[n] for n in pr.valid_id}, name='proofread_by')
+
+    return G
 
 
 def fetch_leaderboard(days=7, by_day=False, progress=True, max_threads=4):
     """Fetch leader board (# of edits).
 
     Parameters
     ----------
@@ -220,15 +328,15 @@
     >>> flywire.roots_to_supervoxels(720575940619164912)[720575940619164912]
     array([78180637324085660, 78180706043394027, 78180706043400870, ...,
            78743587210799793, 78743587210799781, 78743587210818108],
           dtype=uint64)
 
     """
     # Make sure we are working with an array of integers
-    x = navis.utils.make_iterable(x).astype(int, copy=False)
+    x = make_iterable(x, force_type=np.int64)
 
     if len(x) <= 1:
         progress = False
 
     # Get the volume
     vol = parse_volume(dataset)
 
@@ -248,15 +356,15 @@
                 with sv_cache.transact():
                     svoxels.update({i: sv_cache[i] for i in x[is_cached]})
 
     # Get the supervoxels for the roots that are still missing
     # We need to convert keys to integer array because otherwise there is a
     # mismatch in types (int vs np.int?) which causes all root IDs to be in miss
     # -> I think that's because of the way disk cache works
-    miss = x[~np.isin(x, np.array(list(svoxels.keys())).astype(int))]
+    miss = x[~np.isin(x, np.array(list(svoxels.keys()), dtype=np.int64))]
     get_leaves = retry(vol.get_leaves)
     svoxels.update({i: get_leaves(i,
                                   bbox=vol.meta.bounds(0),
                                   mip=0) for i in navis.config.tqdm(miss,
                                                                     desc='Querying',
                                                                     disable=not progress,
                                                                     leave=False)})
@@ -266,29 +374,31 @@
         with sv_cache.transact():
             for i in miss:
                 sv_cache[i] = svoxels[i]
 
     return svoxels
 
 
-def supervoxels_to_roots(x, timestamp=None, batch_size=10_000,
+def supervoxels_to_roots(x, timestamp=None, batch_size=10_000, stop_layer=10,
                          retry=True, progress=True, dataset='production'):
     """Get root(s) for given supervoxel(s).
 
     Parameters
     ----------
     x :             int | list of int
                     Supervoxel ID(s) to find the root(s) for.
     timestamp :     int | str | datetime
                     Get roots at given date (and time). Int must be unix
                     timestamp. String must be ISO 8601 - e.g. '2021-11-15'.
                     If timestamp is given, will ignore `use_cache`.
     batch_size :    int
                     Max number of supervoxel IDs per query. Reduce batch size if
                     you experience time outs.
+    stop_layer :    int
+                    Set e.g. to ``2`` to get L2 IDs instead of root IDs.
     retry :         bool
                     Whether to retry if a batched query fails.
     dataset :       str | CloudVolume
                     Against which dataset to query::
                         - "production" (current production dataset, fly_v31)
                         - "sandbox" (i.e. fly_v26)
     progress :      bool
@@ -302,21 +412,19 @@
     Examples
     --------
     >>> from fafbseg import flywire
     >>> flywire.supervoxels_to_roots(78321855915861142)
 
     """
     # Make sure we are working with an array of integers
-    x = navis.utils.make_iterable(x)
+    x = make_iterable(x, force_type=np.int64)
 
     # Check if IDs are valid (zeros are fine because we filter for them later on)
     is_valid_supervoxel(x[(x != 0) & (x != '0')], raise_exc=True)
 
-    x = x.astype(np.int64, copy=False)
-
     # Parse the volume
     vol = parse_volume(dataset)
 
     # Prepare results array
     roots = np.zeros(x.shape, dtype=np.int64)
 
     if isinstance(timestamp, np.datetime64):
@@ -331,20 +439,22 @@
             # This batch
             batch = x[i:i+batch_size]
 
             # get_roots() doesn't like to be asked for zeros - causes server error
             not_zero = batch != 0
             try:
                 roots[i:i+batch_size][not_zero] = vol.get_roots(batch[not_zero],
+                                                                stop_layer=stop_layer,
                                                                 timestamp=timestamp)
             except BaseException:
                 if not retry:
                     raise
                 time.sleep(1)
                 roots[i:i+batch_size][not_zero] = vol.get_roots(batch[not_zero],
+                                                                stop_layer=stop_layer,
                                                                 timestamp=timestamp)
 
             pbar.update(len(batch))
 
     return roots
 
 
@@ -392,15 +502,15 @@
                              ', fw.y, fw.z] or [x, y, z] columns.')
 
         # Make sure we are working with numbers
         if not np.issubdtype(locs.dtype, np.number):
             locs = locs.astype(np.float64)
 
     return spine.transform.get_segids(locs, segmentation='flywire_190410',
-                                      coordinates=coordinates, mip=-1)
+                                      coordinates=coordinates, mip=mip)
 
 
 def neuron_to_segments(x, short=False, dataset='production', coordinates='voxel'):
     """Get root IDs overlapping with a given neuron.
 
     Parameters
     ----------
@@ -647,15 +757,15 @@
     >>> from fafbseg import flywire
     >>> flywire.is_latest_root(720575940621039145)
     array([True])
 
     """
     dataset = FLYWIRE_DATASETS.get(dataset, dataset)
 
-    id = navis.utils.make_iterable(id).astype(str)
+    id = make_iterable(id, force_type=str)
 
     # The server doesn't like being asked for zeros
     not_zero = id != '0'
 
     # Check if all other IDs are valid
     is_valid_root(id[not_zero], raise_exc=True)
 
@@ -776,15 +886,15 @@
                 raise ValueError(f'Number of supervoxels ({len(supervoxels)}) does '
                                  f'not match number of root IDs ({len(id)})')
             elif any(pd.isnull(supervoxels)):
                 raise ValueError('`supervoxels` must not contain `None`')
             elif any(pd.isnull(id)):
                 raise ValueError('`id` must not contain `None`')
 
-            id = np.array(id).astype(int)
+            id = np.array(id).astype(np.int64)
 
             res = pd.DataFrame()
             res['old_id'] = id
             res['new_id'] = id
             res.loc[~is_latest, 'new_id'] = supervoxels_to_roots(supervoxels[~is_latest],
                                                                  dataset=dataset)
             res['conf'] = 1
@@ -1151,7 +1261,184 @@
     except:
         is_valid = False
 
     if raise_exc and not is_valid:
         raise ValueError(f'{x} is not a valid supervoxel ID')
 
     return is_valid
+
+
+def get_voxels(x, mip=0, sv_map=False, bounds=None, thin=False, progress=True,
+               use_mirror=True, dataset='production'):
+    """Fetch voxels making a up given root ID.
+
+    Parameters
+    ----------
+    x :             int
+                    A single root ID.
+    mip :           int
+                    Scale at which to fetch voxels. Mip 0, for example, is
+                    16 x 16 x 40nm.
+    sv_map :        bool
+                    If True, additionally return a map with the L2 ID for each
+                    voxel.
+    bounds :        (3, 2) or (2, 3) array, optional
+                    Bounding box to return voxels in. Expected to be in 4, 4, 40
+                    voxel space.
+    thin :          bool
+                    If True, will remove voxels at the interface of adjacent
+                    supervoxels that are not supposed to be connected according
+                    to the L2 graph. This is rather expensive but can help in
+                    situations where a neuron self-touches.
+    use_mirror :    bool
+                    If True (default), will use an mirror of the base
+                    segmentation for supervoxel look-up. Possibly slightly
+                    slower than the production data set but doesn't incur
+                    egress charges for Princeton.
+    progress :      bool
+                    Whether to show a progress bar or not.
+
+    Returns
+    -------
+    voxels :        (N, 3) np.ndarray
+                    In voxel space according to `mip`.
+    sv_map :        (N, ) np.ndarray
+                    Supervoxel ID for each voxel. Only if `sv_map=True`.
+
+    """
+    # IDEA:
+    # 1. Find surface voxels for each L2 chunk
+    # 2. Get L2 graph and determine which L2 chunks are supposed to be connected
+    # 3. Remove surface voxel between adjacent but not connected L2 chunks
+
+    from .l2 import chunks_to_nm
+
+    # This is a mirror for base segmentation
+    vol = parse_volume(dataset)
+    client = get_cave_client()
+
+    if use_mirror:
+        sv_vol = cv.CloudVolume('precomputed://https://seungdata.princeton.edu/'
+                                'sseung-archive/fafbv14-ws/'
+                                'ws_190410_FAFB_v02_ws_size_threshold_200',
+                                 use_https=True, progress=False, fill_missing=True)
+    else:
+        sv_vol = vol
+
+    is_valid_root(x, raise_exc=True)
+
+    # Get L2 chunks making up this neuron
+    l2_ids = client.chunkedgraph.get_leaves(x, stop_layer=2)
+
+    # Get supervoxels for this neuron
+    sv = roots_to_supervoxels(x, dataset=dataset)[x]
+
+    # Turn l2_ids into chunk indices
+    l2_ix = [np.array(vol.mesh.meta.meta.decode_chunk_position(l)) for l in l2_ids]
+    l2_ix = np.unique(l2_ix, axis=0)
+
+    # Convert to nm
+    l2_nm = np.asarray(chunks_to_nm(l2_ix, vol=vol))
+
+    # Convert to voxel space
+    l2_vxl = l2_nm // vol.meta.scales[mip]["resolution"]
+
+    # Apply bounds
+    bounds = parse_bounds(bounds)
+    if not isinstance(bounds, type(None)):
+        base_to_mip = np.array(vol.meta.scales[mip]["resolution"]) / [4, 4, 40]
+        bounds = bounds // base_to_mip.reshape(-1, 1)
+        l2_vxl = l2_vxl[np.all(l2_vxl >= bounds[:, 0], axis=1)]
+        l2_vxl = l2_vxl[np.all(l2_vxl <= bounds[:, 1], axis=1)]
+
+    voxels = []
+    svids = []
+    ch_size = np.array(vol.mesh.meta.meta.graph_chunk_size)
+    ch_size = ch_size // (vol.mip_resolution(mip) / vol.mip_resolution(0))
+    old_mip = sv_vol.mip
+    try:
+        sv_vol.mip = mip
+        for ch in tqdm(l2_vxl,
+                       disable=not progress,
+                       leave=False,
+                       desc='Loading'):
+            ct = sv_vol[ch[0]:ch[0] + ch_size[0],
+                        ch[1]:ch[1] + ch_size[1],
+                        ch[2]:ch[2] + ch_size[2]][:, :, :, 0]
+            is_root = np.isin(ct, sv)
+            this_vxl = np.dstack(np.where(is_root))[0]
+            this_vxl = this_vxl + ch
+            voxels.append(this_vxl)
+
+            if sv_map or thin:
+                svids.append(ct[is_root])
+    except BaseException:
+        raise
+    finally:
+        sv_vol.mip = old_mip
+
+    # uint 16 should be sufficient because even at mip 0 the volume has
+    # shape (54100, 28160, 7046) -> doesn't exceed 65_535
+    voxels = np.vstack(voxels).astype('uint16')
+    if len(svids):
+        svids = np.concatenate(svids)
+
+    if thin:
+        from .l2 import l2_graph
+
+        try:
+            from pykdtree.kdtree import KDTree
+        except ImportError:
+            from scipy.spatial import cKDTree as KDTree
+
+        # Get the l2 ID for each supervoxel
+        l2_ids = vol.get_roots(svids, stop_layer=2)
+        l2_dict = dict(zip(svids, l2_ids))
+
+        # Get the l2 graph
+        G = l2_graph(x)
+
+        # Create KD tree for all voxels
+        tree = KDTree(voxels)
+
+        # Create a mask for invalidated voxels
+        invalid = np.zeros(len(voxels), dtype=bool)
+
+        # Now go over each supervoxel
+        for sv in tqdm(np.unique(svids),
+                       disable= not progress,
+                       desc='Thinning',
+                       leave=False):
+            # Get the voxels for this supervoxel
+            is_this_sv = svids == sv
+
+            # If supervoxel has no voxels just continue
+            if not np.any(is_this_sv):
+                continue
+
+            # Get all supervoxels that could be connected to this supervoxel
+            is_this_l2 = l2_ids == l2_dict[sv]
+            is_connected_l2 = np.isin(l2_ids, list(G.neighbors(l2_dict[sv])))
+
+            # The mask needs to exclude anything that:
+            # Isn't this supervoxel OR is supposed to be connected OR
+            # has already been invalidated in a prior run
+            mask = is_this_l2 | is_connected_l2 | invalid
+
+            # Find "other" voxels that touch voxels for this supervoxel
+            dist, ix = tree.query(voxels[is_this_sv],
+                                  mask=mask,
+                                  distance_upper_bound=1.75)
+            is_touching = dist < np.inf
+
+            if not np.any(is_touching):
+                continue
+
+            invalid[np.where(is_this_sv)[0][is_touching]] = True
+
+        voxels = voxels[~invalid]
+        svids = svids[~invalid]
+
+    if not sv_map:
+        return voxels
+    else:
+        return voxels, svids
```

### Comparing `fafbseg-1.8.0/fafbseg/flywire/skeletonize.py` & `fafbseg-1.9.0/fafbseg/flywire/skeletonize.py`

 * *Files 3% similar despite different names*

```diff
@@ -341,44 +341,50 @@
         sg = nx.ego_graph(G, center, distance='weight', radius=radius)
         nodes = set(sg.nodes)
         patches.append(nodes)
         not_seen -= nodes
 
 
 def skeletonize_neuron_parallel(ids, n_cores=os.cpu_count() // 2, **kwargs):
-    """Skeletonization on parallel cores [WIP].
+    """Skeletonization on parallel cores.
 
     Parameters
     ----------
     ids :       iterable
                 Root IDs of neurons you want to skeletonize.
     n_cores :   int
                 Number of cores to use. Don't go too crazy on this as the
                 downloading of meshes becomes a bottle neck if you try to do
                 too many at the same time. Keep your internet speed in
-                mind.
+                mind. For reference: with 100Mbps internet, I can comfortably
+                run on 8 cores with some room to spare.
     **kwargs
                 Keyword arguments are passed on to `skeletonize_neuron`.
 
     Returns
     -------
     navis.NeuronList
 
+    See Also
+    --------
+    :func:`fafbseg.flywire.skeletonize_neuron`
+                The function called for individual neurons.
+
     """
     if n_cores < 2 or n_cores > os.cpu_count():
         raise ValueError('`n_cores` must be between 2 and max number of cores.')
 
     sig = inspect.signature(skeletonize_neuron)
     for k in kwargs:
         if k not in sig.parameters:
             raise ValueError('unexpected keyword argument for '
                              f'`skeletonize_neuron`: {k}')
 
     # Make sure IDs are all integers
-    ids = np.asarray(ids).astype(int)
+    ids = np.asarray(ids).astype(np.int64)
 
     # Prepare the calls and parameters
     kwargs['progress'] = False
     funcs = [skeletonize_neuron] * len(ids)
     parsed_kwargs = [kwargs] * len(ids)
     combinations = list(zip(funcs, [[i] for i in ids], parsed_kwargs))
```

### Comparing `fafbseg-1.8.0/fafbseg/flywire/synapses.py` & `fafbseg-1.9.0/fafbseg/flywire/synapses.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from functools import partial
 from pathlib import Path
 from tqdm.auto import trange
 
 from .segmentation import is_latest_root
 from .utils import parse_root_ids, get_cave_client, retry, get_synapse_areas
 
+from ..utils import make_iterable
 from ..synapses.utils import catmaid_table
 from ..synapses.transmitters import collapse_nt_predictions
 
 __all__ = ['fetch_synapses', 'fetch_connectivity', 'predict_transmitter',
            'fetch_adjacency', 'synapse_counts']
 
 
@@ -181,15 +182,15 @@
     syn = fetch_synapses(x, pre=True, post=False, attach=False, min_score=None,
                          transmitters=True, live_query=live_query,
                          neuropils=neuropils is not None,
                          batch_size=batch_size,
                          dataset=dataset, **kwargs)
 
     if not isinstance(neuropils, type(None)):
-        neuropils = navis.utils.make_iterable(neuropils)
+        neuropils = make_iterable(neuropils)
         filter_in = [n for n in neuropils if not n.startswith('~')]
         filter_out = [n[1:] for n in neuropils if n.startswith('~')]
 
         if filter_in:
             syn = syn[syn.neuropil.isin(filter_in)]
         if filter_out:
             syn = syn[~syn.neuropil.isin(filter_out)]
@@ -485,15 +486,15 @@
     syn = pd.concat(syn, axis=0, ignore_index=True)
 
     # Depending on how queries were batched, we need to drop duplicate synapses
     syn.drop_duplicates('id', inplace=True)
 
     # Subset to the desired neuropils
     if not isinstance(neuropils, type(None)):
-        neuropils = navis.utils.make_iterable(neuropils)
+        neuropils = make_iterable(neuropils)
 
         if len(neuropils):
             filter_in = [n for n in neuropils if not n.startswith('~')]
             filter_out = [n[1:] for n in neuropils if n.startswith('~')]
 
             syn['neuropil'] = get_synapse_areas(syn['id'].values)
             syn['neuropil'] = syn.neuropil.astype('category')
@@ -634,15 +635,15 @@
             syn.append(func(filter_in_dict=dict(pre_pt_root_id=batch)))
 
     # Combine results from batches
     syn = pd.concat(syn, axis=0, ignore_index=True)
 
     # Subset to the desired neuropils
     if not isinstance(neuropils, type(None)):
-        neuropils = navis.utils.make_iterable(neuropils)
+        neuropils = make_iterable(neuropils)
 
         if len(neuropils):
             filter_in = [n for n in neuropils if not n.startswith('~')]
             filter_out = [n[1:] for n in neuropils if n.startswith('~')]
 
             syn['neuropil'] = get_synapse_areas(syn['id'].values)
             syn['neuropil'] = syn.neuropil.astype('category')
```

### Comparing `fafbseg-1.8.0/fafbseg/flywire/utils.py` & `fafbseg-1.9.0/fafbseg/flywire/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -211,19 +211,19 @@
     if isinstance(x, navis.BaseNeuron):
         ids = [x.id]
     elif isinstance(x, navis.NeuronList):
         ids = x.id
     elif isinstance(x, (int, np.int)):
         ids = [x]
     else:
-        ids = navis.utils.make_iterable(x)
+        ids = utils.make_iterable(x, dtype=np.int64)
 
     # Make sure we are working with proper numerical IDs
     try:
-        return np.asarray(ids).astype(int)
+        return np.asarray(ids, dtype=np.int64)
     except ValueError:
         raise ValueError(f'Unable to convert given root IDs to integer: {ids}')
     except BaseException:
         raise
 
 
 def parse_volume(vol, **kwargs):
@@ -293,8 +293,34 @@
             except requests.HTTPError:
                 if i >= retries:
                     raise
             except BaseException:
                 raise
             time.sleep(cooldown * i)
     return wrapper
-    return wrapper
+
+
+def parse_bounds(x):
+    """Parse bounds.
+
+    Parameters
+    ----------
+    x :     (3, 2) array | (2, 3) array | None
+
+    Returns
+    -------
+    bounds :    (3, 2) np.array
+
+    """
+    if isinstance(x, type(None)):
+        return x
+
+    x = np.asarray(x)
+
+    if not x.ndim == 2 or x.shape not in [(3, 2), (2, 3)]:
+        raise ValueError('Must provide bounding box as (3, 2) or (2, 3) array, '
+                         f'got {x.shape}')
+
+    if x.shape == (2, 3):
+        x = x.T
+
+    return np.vstack((x.min(axis=1), x.max(axis=1))).T
```

### Comparing `fafbseg-1.8.0/fafbseg/google/__init__.py` & `fafbseg-1.9.0/fafbseg/google/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/google/meshes.py` & `fafbseg-1.9.0/fafbseg/google/meshes.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/google/segmentation.py` & `fafbseg-1.9.0/fafbseg/google/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                         Will be ``None`` if no skeleton found.
 
     """
     assert isinstance(autoseg_instance, pymaid.CatmaidInstance)
 
     assert isinstance(seg_ids, (list, np.ndarray, set, tuple, pd.Index, int, str))
 
-    seg_ids = navis.utils.make_iterable(seg_ids)
+    seg_ids = utils.make_iterable(seg_ids)
 
     # Prepare map seg ID -> skeleton ID
     seg2skid = {int(i): None for i in seg_ids}
 
     # First find neurons by name
     # Do NOT change the order of "names"!
     names = [name_pattern.format(id=i) for i in seg_ids]
```

### Comparing `fafbseg-1.8.0/fafbseg/google/synapses.py` & `fafbseg-1.9.0/fafbseg/google/synapses.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import navis
 
 import numpy as np
 
 from .segmentation import neuron_to_segments
 
 from ..synapses.utils import catmaid_table
-from .. import spine
+from .. import spine, utils
 
 __all__ = ['fetch_synapses', 'fetch_connectivity']
 
 
 def fetch_synapses(x, attach=True, dataset='production', progress=True):
     """Fetch Buhmann et al. (2019) synapses for given neuron(s).
 
@@ -98,15 +98,15 @@
         ids = {}
         for n in overlaps.columns:
             this = overlaps[overlaps[n] > 0][n]
             ids.update(dict(zip(this.index.values, [n] * this.shape[0])))
     elif isinstance(x, (int, np.int)):
         ids = {x: x}
     else:
-        ids = {n: n for n in navis.utils.make_iterable(x)}
+        ids = {n: n for n in utils.make_iterable(x)}
 
     # Query the synapses
     syn = spine.synapses.get_connectivity(list(ids.keys()),
                                           segmentation=segmentation)
 
     # Next we need to run some clean-up:
     # 1. Drop below threshold connections
```

### Comparing `fafbseg-1.8.0/fafbseg/move/__init__.py` & `fafbseg-1.9.0/fafbseg/move/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/move/interfaces.py` & `fafbseg-1.9.0/fafbseg/move/interfaces.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/move/merge.py` & `fafbseg-1.9.0/fafbseg/move/merge.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/move/merge_utils.py` & `fafbseg-1.9.0/fafbseg/move/merge_utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/spine/__init__.py` & `fafbseg-1.9.0/fafbseg/spine/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/spine/base.py` & `fafbseg-1.9.0/fafbseg/spine/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 import numpy as np
 import pandas as pd
 import trimesh as tm
 
 from abc import ABC
 from io import StringIO, BytesIO
 
+from ..utils import make_iterable
+
 use_pbars = True
 
 
 class OnDemandDict(dict):
     """Initialized with a just a URL.
 
     Will fetch data from given URL on first request.
@@ -147,15 +149,15 @@
                         If `as_array=False`: dictionary mapping ID to
                         centroid `{L2_ID: [x, y, z], ..}`.
 
         """
         url = self.makeurl('mesh/l2_centroid/flywire_fafb_production/')
 
         # Make sure we have an array of integers
-        ids = navis.utils.make_iterable(ids).astype(int)
+        ids = make_iterable(ids, force_type=np.int64)
 
         with navis.config.tqdm(total=len(ids), desc='Fetching centroids',
                                leave=False, disable=not progress) as pbar:
 
             # First we will get everything that's cached in a single big query
             post = {
                       "token": token,
@@ -454,15 +456,15 @@
             # Make sure we are working with numbers
             # -> if dtype is "object" we will get errors from np.round
             if not np.issubdtype(vxl.dtype, np.number):
                 vxl = vxl.astype(np.float64)
 
             # Convert to voxels
             vxl_size = self.info[dataset]['voxel_size']
-            vxl = np.round(vxl / vxl_size).astype(int)
+            vxl = np.round(vxl / vxl_size).astype(np.int64)
 
         return vxl
 
     def get_offsets(self, x, transform, coordinates='nm', mip=-1, limit_request=10e9,
                     on_fail='warn'):
         """Transform coordinates.
 
@@ -699,15 +701,15 @@
     if x.ndim != 2 or x.shape[1] != 3:
         raise TypeError('Expected (N, 3) array, got {}'.format(x.shape))
 
     # We need to convert to voxel coordinates
     # Note that we are rounding here to get to voxels.
     # This will have the most impact on the Z section.
     if coordinates not in ['vxl', 'voxel', 'voxels']:
-        x = np.round(x / [4, 4, 40]).astype(int)
+        x = np.round(x / [4, 4, 40]).astype(np.int64)
 
     # Generate URL
     url = f'{TRANSFORM_SERVICE_URL}/{query}/dataset/{dataset}/s/{mip}/values_binary/format/array_float_Nx3'
 
     # Make sure we don't exceed the maximum size for each request
     stack = []
     limit_request = int(limit_request)
```

### Comparing `fafbseg-1.8.0/fafbseg/synapses/__init__.py` & `fafbseg-1.9.0/fafbseg/synapses/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/synapses/offline.py` & `fafbseg-1.9.0/fafbseg/synapses/offline.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/synapses/online.py` & `fafbseg-1.9.0/fafbseg/synapses/online.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/synapses/transmitters.py` & `fafbseg-1.9.0/fafbseg/synapses/transmitters.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/synapses/utils.py` & `fafbseg-1.9.0/fafbseg/synapses/utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/utils.py` & `fafbseg-1.9.0/fafbseg/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,21 @@
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 """Collection of utility functions."""
 
 import requests
+import six
+
+import numpy as np
 
 from functools import wraps
 from urllib.parse import urlparse, urlencode
+from collections.abc import Iterable
 
 use_pbars = True
 
 
 def never_cache(function):
     """Decorate to prevent caching of server responses."""
     @wraps(function)
@@ -86,7 +90,32 @@
         arg_str = str(arg)
         joiner = '' if url.endswith('/') else '/'
         relative = arg_str[1:] if arg_str.startswith('/') else arg_str
         url = requests.compat.urljoin(url + joiner, relative)
     if GET:
         url += '?{}'.format(urlencode(GET))
     return url
+
+
+def make_iterable(x, force_type = None) -> np.ndarray:
+    """Force input into a numpy array.
+
+    For dicts, keys will be turned into array.
+
+    Examples
+    --------
+    >>> from navis.utils import make_iterable
+    >>> make_iterable(1)
+    array([1])
+    >>> make_iterable([1])
+    array([1])
+    >>> make_iterable({'a': 1})
+    array(['a'], dtype='<U1')
+
+    """
+    if not isinstance(x, Iterable) or isinstance(x, six.string_types):
+        x = [x]
+
+    if isinstance(x, (dict, set)):
+        x = list(x)
+
+    return np.asarray(x, dtype=force_type)
```

### Comparing `fafbseg-1.8.0/fafbseg/xform/__init__.py` & `fafbseg-1.9.0/fafbseg/xform/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg/xform/xform.py` & `fafbseg-1.9.0/fafbseg/xform/xform.py`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/fafbseg.egg-info/PKG-INFO` & `fafbseg-1.9.0/fafbseg.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fafbseg
-Version: 1.8.0
+Version: 1.9.0
 Summary: Tools to work with auto-segmented FAFB data
 Home-page: https://github.com/flyconnectome/fafbseg-py
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Keywords: FAFB neuron segmentation flywire Google synapses
 Platform: UNKNOWN
@@ -32,11 +32,11 @@
 
 ```bash
 pip3 install fafbseg
 ```
 
 Install from Github
 ```bash
-pip3 install git+git://github.com/flyconnectome/fafbseg-py.git
+pip3 install git+https://github.com/flyconnectome/fafbseg-py.git
 ```
```

### Comparing `fafbseg-1.8.0/fafbseg.egg-info/SOURCES.txt` & `fafbseg-1.9.0/fafbseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fafbseg-1.8.0/setup.py` & `fafbseg-1.9.0/setup.py`

 * *Files identical despite different names*

