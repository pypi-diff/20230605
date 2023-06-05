# Comparing `tmp/element-lab-0.2.0.tar.gz` & `tmp/element-lab-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-lab-0.2.0.tar", last modified: Thu Mar  9 23:53:47 2023, max compression
+gzip compressed data, was "element-lab-0.3.0.tar", last modified: Mon Jun  5 17:06:37 2023, max compression
```

## Comparing `element-lab-0.2.0.tar` & `element-lab-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 23:53:47.682294 element-lab-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-09 23:53:45.000000 element-lab-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-09 23:53:47.682294 element-lab-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-09 23:53:45.000000 element-lab-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 23:53:47.678295 element-lab-0.2.0/element_lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 23:53:45.000000 element-lab-0.2.0/element_lab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 23:53:47.678295 element-lab-0.2.0/element_lab/export/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-09 23:53:45.000000 element-lab-0.2.0/element_lab/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-03-09 23:53:45.000000 element-lab-0.2.0/element_lab/export/nwb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-03-09 23:53:45.000000 element-lab-0.2.0/element_lab/lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-03-09 23:53:45.000000 element-lab-0.2.0/element_lab/project.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-09 23:53:45.000000 element-lab-0.2.0/element_lab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 23:53:47.678295 element-lab-0.2.0/element_lab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-09 23:53:47.000000 element-lab-0.2.0/element_lab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-09 23:53:47.000000 element-lab-0.2.0/element_lab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 23:53:47.000000 element-lab-0.2.0/element_lab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-09 23:53:47.000000 element-lab-0.2.0/element_lab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 23:53:47.000000 element-lab-0.2.0/element_lab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 23:53:47.682294 element-lab-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-09 23:53:45.000000 element-lab-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:37.326969 element-lab-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-05 17:06:33.000000 element-lab-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-05 17:06:37.326969 element-lab-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-05 17:06:33.000000 element-lab-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:37.326969 element-lab-0.3.0/element_lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:33.000000 element-lab-0.3.0/element_lab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:37.326969 element-lab-0.3.0/element_lab/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-05 17:06:33.000000 element-lab-0.3.0/element_lab/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-05 17:06:33.000000 element-lab-0.3.0/element_lab/export/nwb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-06-05 17:06:33.000000 element-lab-0.3.0/element_lab/lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-05 17:06:33.000000 element-lab-0.3.0/element_lab/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 17:06:33.000000 element-lab-0.3.0/element_lab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:37.326969 element-lab-0.3.0/element_lab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-05 17:06:37.000000 element-lab-0.3.0/element_lab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-05 17:06:37.000000 element-lab-0.3.0/element_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:06:37.000000 element-lab-0.3.0/element_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 17:06:37.000000 element-lab-0.3.0/element_lab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 17:06:37.000000 element-lab-0.3.0/element_lab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:06:37.326969 element-lab-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-05 17:06:33.000000 element-lab-0.3.0/setup.py
```

### Comparing `element-lab-0.2.0/LICENSE` & `element-lab-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `element-lab-0.2.0/PKG-INFO` & `element-lab-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-lab
-Version: 0.2.0
+Version: 0.3.0
 Summary: DataJoint Elements for Lab Management
 Home-page: https://github.com/datajoint/element-lab
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience lab management datajoint
 Platform: UNKNOWN
```

### Comparing `element-lab-0.2.0/element_lab/export/nwb.py` & `element-lab-0.3.0/element_lab/export/nwb.py`

 * *Files identical despite different names*

### Comparing `element-lab-0.2.0/element_lab/lab.py` & `element-lab-0.3.0/element_lab/lab.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,7 +268,25 @@
     definition = """
     source                : varchar(32)  # abbreviated source name
     ---
     source_name           : varchar(255)
     contact_details=''    : varchar(255)
     source_description='' : varchar(255)
     """
+
+
+@schema
+class Device(dj.Lookup):
+    """Devices within the lab.
+
+    Attributes:
+        device ( varchar(32) ): Device short name.
+        modality ( varchar(64) ): Modality for which this device is used.
+        description ( varchar(256) ): Optional. Description of the device.
+    """
+
+    definition = """
+    device             : varchar(32)
+    ---
+    modality           : varchar(64)
+    description=''     : varchar(256)
+    """
```

### Comparing `element-lab-0.2.0/element_lab/project.py` & `element-lab-0.3.0/element_lab/project.py`

 * *Files identical despite different names*

### Comparing `element-lab-0.2.0/element_lab.egg-info/PKG-INFO` & `element-lab-0.3.0/element_lab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-lab
-Version: 0.2.0
+Version: 0.3.0
 Summary: DataJoint Elements for Lab Management
 Home-page: https://github.com/datajoint/element-lab
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience lab management datajoint
 Platform: UNKNOWN
```

### Comparing `element-lab-0.2.0/setup.py` & `element-lab-0.3.0/setup.py`

 * *Files identical despite different names*

