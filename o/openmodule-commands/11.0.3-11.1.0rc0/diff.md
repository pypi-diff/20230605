# Comparing `tmp/openmodule_commands-11.0.3.tar.gz` & `tmp/openmodule_commands-11.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-11.0.3.tar", last modified: Fri May  5 16:34:09 2023, max compression
+gzip compressed data, was "openmodule_commands-11.1.0rc0.tar", last modified: Mon Jun  5 10:52:16 2023, max compression
```

## Comparing `openmodule_commands-11.0.3.tar` & `openmodule_commands-11.1.0rc0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:34:09.916428 openmodule_commands-11.0.3/
--rw-r--r--   0 root         (0) root         (0)      302 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     6535 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      618 2023-05-05 16:34:09.916428 openmodule_commands-11.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-05-05 16:33:53.000000 openmodule_commands-11.0.3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:34:09.916428 openmodule_commands-11.0.3/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-05-05 16:34:09.916428 openmodule_commands-11.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-05-05 16:33:53.000000 openmodule_commands-11.0.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-05-05 16:33:53.000000 openmodule_commands-11.0.3/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:16.024458 openmodule_commands-11.1.0rc0/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     6525 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-05 10:52:16.024458 openmodule_commands-11.1.0rc0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-05 10:52:03.000000 openmodule_commands-11.1.0rc0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:16.024458 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-05 10:52:15.000000 openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-05 10:52:16.025458 openmodule_commands-11.1.0rc0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-05 10:52:03.000000 openmodule_commands-11.1.0rc0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-05 10:52:03.000000 openmodule_commands-11.1.0rc0/translate.py
```

### Comparing `openmodule_commands-11.0.3/ChangeLog` & `openmodule_commands-11.1.0rc0/ChangeLog`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 CHANGES
 =======
 
+v11.1.0.rc0
+-----------
+
+* fixed testcase
+* small changes in csv export and databox upload adding more testcases docs
+* move files instead of copy
+* readme
+* util for databox upload
+* removing language dependency
+* removing ="asdf" for strings
+* added decimal separator support for english
+* some testcases for csv exporter, incorrect default value + static missing [skip ci]
+* fixed comment
+* added csv\_export library (no testcases)
+* removed mock rpcs from schema
+
 v11.0.3
 -------
 
 * Fixed typo, added compute\_id as label to all metrics, convert all label values to string
 * touch to get rid of skip ci on my commit
 * docs update [skip ci]
 * main test function deprecated and documentation for main tests added
@@ -142,32 +158,7 @@
 
 * # OpenModule \* rpc client resource filter only applies if resource in message \* all zmq messages now use utc timestamps
 
 v6.1.6
 ------
 
 * 6.1.6
-
-v6.1.5
-------
-
-* bug fix test cases
-* rpc-client refactor + kv\_redis
-* rpc-client
-* added default zmq.LINGER for context to be more compatible with OMv1 socket creation
-* wait for rpc assertion
-
-v6.1.4
-------
-
-* Resource Filter in RPC Server + removed urljoin from ApiMocker
-
-v6.1.3
-------
-
-* fixes a unicode issue
-
-v6.1.2
-------
-
-* count message uses lazy settings resource, import cleanup
-* fixes a timezone issue where the timezone of the local system would change results
```

### Comparing `openmodule_commands-11.0.3/PKG-INFO` & `openmodule_commands-11.1.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 11.0.3
+Version: 11.1.0rc0
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.0.3/__init__.py` & `openmodule_commands-11.1.0rc0/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.0.3/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-11.1.0rc0/openmodule_commands.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 11.0.3
+Version: 11.1.0rc0
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.0.3/setup.cfg` & `openmodule_commands-11.1.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.0.3/setup.py` & `openmodule_commands-11.1.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.0.3/translate.py` & `openmodule_commands-11.1.0rc0/translate.py`

 * *Files identical despite different names*

