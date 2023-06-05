# Comparing `tmp/openmodule_commands-11.1.0rc0.tar.gz` & `tmp/openmodule_commands-11.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-11.1.0rc0.tar", last modified: Mon Jun  5 10:52:16 2023, max compression
+gzip compressed data, was "openmodule_commands-11.1.0rc1.tar", last modified: Mon Jun  5 11:17:12 2023, max compression
```

## Comparing `openmodule_commands-11.1.0rc0.tar` & `openmodule_commands-11.1.0rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:16.024458 openmodule_commands-11.1.0rc0/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     6525 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-05 10:52:16.024458 openmodule_commands-11.1.0rc0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-05 10:52:03.000000 openmodule_commands-11.1.0rc0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:16.024458 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-05 10:52:16.025458 openmodule_commands-11.1.0rc0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-05 10:52:03.000000 openmodule_commands-11.1.0rc0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-05 10:52:03.000000 openmodule_commands-11.1.0rc0/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:17:12.332812 openmodule_commands-11.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-05 11:17:12.000000 openmodule_commands-11.1.0rc1/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     6462 2023-06-05 11:17:12.000000 openmodule_commands-11.1.0rc1/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-05 11:17:12.332812 openmodule_commands-11.1.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-05 11:17:00.000000 openmodule_commands-11.1.0rc1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:17:12.331812 openmodule_commands-11.1.0rc1/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-05 11:17:12.000000 openmodule_commands-11.1.0rc1/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-05 11:17:12.000000 openmodule_commands-11.1.0rc1/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 11:17:12.000000 openmodule_commands-11.1.0rc1/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-06-05 11:17:12.000000 openmodule_commands-11.1.0rc1/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 11:17:12.000000 openmodule_commands-11.1.0rc1/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-05 11:17:12.000000 openmodule_commands-11.1.0rc1/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-05 11:17:12.000000 openmodule_commands-11.1.0rc1/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-05 11:17:12.332812 openmodule_commands-11.1.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-05 11:17:00.000000 openmodule_commands-11.1.0rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-05 11:17:00.000000 openmodule_commands-11.1.0rc1/translate.py
```

### Comparing `openmodule_commands-11.1.0rc0/ChangeLog` & `openmodule_commands-11.1.0rc1/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v11.1.0.rc1
+-----------
+
+* databox upload now can have dst as folder (endswith "/")
+
 v11.1.0.rc0
 -----------
 
 * fixed testcase
 * small changes in csv export and databox upload adding more testcases docs
 * move files instead of copy
 * readme
@@ -152,13 +157,7 @@
 * reduced warnings in the testcases
 * GUID type and rpc server changes to better support all pydantic models, in this case Union Types. DEVICE-891
 * fixes an issue in rpc server logging, and adds more debug log output
 
 v7.0.0
 ------
 
-* # OpenModule \* rpc client resource filter only applies if resource in message \* all zmq messages now use utc timestamps
-
-v6.1.6
-------
-
-* 6.1.6
```

### Comparing `openmodule_commands-11.1.0rc0/PKG-INFO` & `openmodule_commands-11.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 11.1.0rc0
+Version: 11.1.0rc1
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.0rc0/__init__.py` & `openmodule_commands-11.1.0rc1/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-11.1.0rc1/openmodule_commands.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 11.1.0rc0
+Version: 11.1.0rc1
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.0rc0/setup.cfg` & `openmodule_commands-11.1.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc0/setup.py` & `openmodule_commands-11.1.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc0/translate.py` & `openmodule_commands-11.1.0rc1/translate.py`

 * *Files identical despite different names*

