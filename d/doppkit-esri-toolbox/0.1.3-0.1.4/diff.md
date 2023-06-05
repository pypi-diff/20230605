# Comparing `tmp/doppkit-esri-toolbox-0.1.3.tar.gz` & `tmp/doppkit-esri-toolbox-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-esri-toolbox-0.1.3.tar", last modified: Thu May 25 21:11:33 2023, max compression
+gzip compressed data, was "doppkit-esri-toolbox-0.1.4.tar", last modified: Mon Jun  5 16:54:13 2023, max compression
```

## Comparing `doppkit-esri-toolbox-0.1.3.tar` & `doppkit-esri-toolbox-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.373572 doppkit-esri-toolbox-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 21:11:33.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.373572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/arcpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.373572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/help/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/help/gp/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/help/gp/Fetch_Export_grid access.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:33.377572 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.Fetch_Export.pyt.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-25 21:11:16.000000 doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:54:13.059681 doppkit-esri-toolbox-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 16:53:59.000000 doppkit-esri-toolbox-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-06-05 16:54:13.059681 doppkit-esri-toolbox-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-05 16:53:59.000000 doppkit-esri-toolbox-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-05 16:53:59.000000 doppkit-esri-toolbox-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:54:13.059681 doppkit-esri-toolbox-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:54:13.051681 doppkit-esri-toolbox-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:54:13.055681 doppkit-esri-toolbox-0.1.4/src/doppkit_esri_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-06-05 16:54:13.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_esri_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-05 16:54:13.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_esri_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:54:13.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_esri_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:54:13.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_esri_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 16:54:13.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_esri_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:54:13.055681 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 16:53:59.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:54:13.055681 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:54:13.055681 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/arcpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-05 16:53:59.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:54:13.051681 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/help/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:54:13.055681 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/help/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-05 16:53:59.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/help/gp/Fetch_Export_grid access.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:54:13.059681 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/toolboxes/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-05 16:53:59.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.Fetch_Export.pyt.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-05 16:53:59.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-05 16:53:59.000000 doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt.xml
```

### Comparing `doppkit-esri-toolbox-0.1.3/LICENSE` & `doppkit-esri-toolbox-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.3/PKG-INFO` & `doppkit-esri-toolbox-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit-esri-toolbox
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-esri-toolbox-0.1.3/README.md` & `doppkit-esri-toolbox-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.3/pyproject.toml` & `doppkit-esri-toolbox-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/PKG-INFO` & `doppkit-esri-toolbox-0.1.4/src/doppkit_esri_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit-esri-toolbox
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-esri-toolbox-0.1.3/src/doppkit_esri_toolbox.egg-info/SOURCES.txt` & `doppkit-esri-toolbox-0.1.4/src/doppkit_esri_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py` & `doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/help/gp/Fetch_Export_grid access.xml` & `doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/help/gp/Fetch_Export_grid access.xml`

 * *Files identical despite different names*

### Comparing `doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt` & `doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from doppkit.sync import sync
 import asyncio
 
 from typing import NamedTuple
 
 
 class SyncParameters(NamedTuple):
+    grid_server: arcpy.Parameter
     token: arcpy.Parameter
     aoi_pk: arcpy.Parameter
     directory: arcpy.Parameter
     add_to_map: arcpy.Parameter
 
 
 class Toolbox:
@@ -34,14 +35,24 @@
         """Define the tool (tool name is the name of the class)."""
         self.label = "GRiD Sync"
         self.description = ""
         self.canRunInBackground = False
 
     def getParameterInfo(self):
         """Define parameter definitions"""
+        grid_server = arcpy.Parameter(
+            displayName="GRiD Server",
+            name="grid_server",
+            datatype="GPString",
+            parameterType="Required",
+            direction="Input",
+        )
+        # specify the default server
+        grid_server.value = "https://grid.nga.mil/grid"
+
         grid_access_token = arcpy.Parameter(
             displayName="GRiD Access Token",
             name="grid_access_token",
             datatype="GPStringHidden",  # not actually encrypted!!
             parameterType="Required",
             direction="Input",
         )
@@ -63,15 +74,15 @@
             displayName="Add Files to Map?",
             name="add_to_map",
             datatype="GPBoolean",
             parameterType="Required",
             direction="Input",
         )
         add_to_map.value = True
-        return [grid_access_token, aoi_name, dl_directory, add_to_map]
+        return [grid_server, grid_access_token, aoi_name, dl_directory, add_to_map]
 
     def updateParameters(self, parameters):
         """Modify the values and properties of parameters before internal
         validation is performed.  This method is called whenever a parameter
         has been changed."""
         return
 
@@ -84,15 +95,15 @@
         """The source code of the tool."""
 
         named_parameters = SyncParameters(
             *parameters
         )
 
         token = named_parameters.token.valueAsText
-        url = "https://grid.nga.mil/grid"
+        url = named_parameters.grid_server.valueAsText
         log_level = "DEBUG"
 
         # no event loop in ESRI toolboxes?
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
 
         app = Application(token, url, log_level, 20)
```

### Comparing `doppkit-esri-toolbox-0.1.3/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt.xml` & `doppkit-esri-toolbox-0.1.4/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt.xml`

 * *Files identical despite different names*

