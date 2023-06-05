# Comparing `tmp/KS_Constants-1.2.8.tar.gz` & `tmp/KS_Constants-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KS_Constants-1.2.8.tar", last modified: Sat Oct  8 21:42:03 2022, max compression
+gzip compressed data, was "KS_Constants-1.2.9.tar", last modified: Sat Oct  8 22:31:19 2022, max compression
```

## Comparing `KS_Constants-1.2.8.tar` & `KS_Constants-1.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-10-08 21:42:03.074691 KS_Constants-1.2.8/
-drwxrwxrwx   0        0        0        0 2022-10-08 21:42:03.060691 KS_Constants-1.2.8/KS_Constants.egg-info/
--rw-rw-rw-   0        0        0      248 2022-10-08 21:42:02.000000 KS_Constants-1.2.8/KS_Constants.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2022-10-08 21:42:03.000000 KS_Constants-1.2.8/KS_Constants.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-08 21:42:02.000000 KS_Constants-1.2.8/KS_Constants.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-10-08 21:42:02.000000 KS_Constants-1.2.8/KS_Constants.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      248 2022-10-08 21:42:03.072689 KS_Constants-1.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-08 21:42:03.070689 KS_Constants-1.2.8/ks_constants/
--rw-rw-rw-   0        0        0        0 2022-10-08 03:11:24.000000 KS_Constants-1.2.8/ks_constants/__init__.py
--rw-rw-rw-   0        0        0      246 2022-10-08 00:23:50.000000 KS_Constants-1.2.8/ks_constants/devs.py
--rw-rw-rw-   0        0        0       87 2022-10-08 03:40:05.000000 KS_Constants-1.2.8/ks_constants/locale.py
--rw-rw-rw-   0        0        0      838 2022-10-08 15:40:59.000000 KS_Constants-1.2.8/ks_constants/map_switch.py
--rw-rw-rw-   0        0        0     4594 2022-10-08 21:41:02.000000 KS_Constants-1.2.8/ks_constants/maps.py
--rw-rw-rw-   0        0        0      661 2022-10-08 03:41:36.000000 KS_Constants-1.2.8/ks_constants/regions.py
--rw-rw-rw-   0        0        0     7661 2022-10-08 21:30:54.000000 KS_Constants-1.2.8/ks_constants/roles.py
--rw-rw-rw-   0        0        0       42 2022-10-08 21:42:03.075687 KS_Constants-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      293 2022-10-08 21:41:28.000000 KS_Constants-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-08 21:42:03.071687 KS_Constants-1.2.8/tests/
--rw-rw-rw-   0        0        0        0 2022-10-08 00:23:50.000000 KS_Constants-1.2.8/tests/__init__.py
--rw-rw-rw-   0        0        0     1490 2022-10-08 21:41:21.000000 KS_Constants-1.2.8/tests/basic_tests.py
+drwxrwxrwx   0        0        0        0 2022-10-08 22:31:19.948292 KS_Constants-1.2.9/
+drwxrwxrwx   0        0        0        0 2022-10-08 22:31:19.939293 KS_Constants-1.2.9/KS_Constants.egg-info/
+-rw-rw-rw-   0        0        0      248 2022-10-08 22:31:19.000000 KS_Constants-1.2.9/KS_Constants.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2022-10-08 22:31:19.000000 KS_Constants-1.2.9/KS_Constants.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-08 22:31:19.000000 KS_Constants-1.2.9/KS_Constants.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2022-10-08 22:31:19.000000 KS_Constants-1.2.9/KS_Constants.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      248 2022-10-08 22:31:19.948292 KS_Constants-1.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-08 22:31:19.945293 KS_Constants-1.2.9/ks_constants/
+-rw-rw-rw-   0        0        0        0 2022-10-08 03:11:24.000000 KS_Constants-1.2.9/ks_constants/__init__.py
+-rw-rw-rw-   0        0        0      246 2022-10-08 00:23:50.000000 KS_Constants-1.2.9/ks_constants/devs.py
+-rw-rw-rw-   0        0        0       87 2022-10-08 03:40:05.000000 KS_Constants-1.2.9/ks_constants/locale.py
+-rw-rw-rw-   0        0        0      838 2022-10-08 15:40:59.000000 KS_Constants-1.2.9/ks_constants/map_switch.py
+-rw-rw-rw-   0        0        0     4594 2022-10-08 21:41:02.000000 KS_Constants-1.2.9/ks_constants/maps.py
+-rw-rw-rw-   0        0        0      661 2022-10-08 03:41:36.000000 KS_Constants-1.2.9/ks_constants/regions.py
+-rw-rw-rw-   0        0        0     7673 2022-10-08 22:07:36.000000 KS_Constants-1.2.9/ks_constants/roles.py
+-rw-rw-rw-   0        0        0       42 2022-10-08 22:31:19.949292 KS_Constants-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      293 2022-10-08 22:31:06.000000 KS_Constants-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-08 22:31:19.947293 KS_Constants-1.2.9/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-08 00:23:50.000000 KS_Constants-1.2.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     1490 2022-10-08 21:41:21.000000 KS_Constants-1.2.9/tests/basic_tests.py
```

### Comparing `KS_Constants-1.2.8/ks_constants/map_switch.py` & `KS_Constants-1.2.9/ks_constants/map_switch.py`

 * *Files identical despite different names*

### Comparing `KS_Constants-1.2.8/ks_constants/maps.py` & `KS_Constants-1.2.9/ks_constants/maps.py`

 * *Files identical despite different names*

### Comparing `KS_Constants-1.2.8/ks_constants/regions.py` & `KS_Constants-1.2.9/ks_constants/regions.py`

 * *Files identical despite different names*

### Comparing `KS_Constants-1.2.8/ks_constants/roles.py` & `KS_Constants-1.2.9/ks_constants/roles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from enum import Enum
+from enum import Enum, IntEnum
 from ks_constants.devs import Developer
 from ks_constants.locale import Language
 
 
-class Team(Enum):
+class Team(IntEnum):
     Survivor = 0
     Kerrigan = 1
 
 
 class RoleType(Enum):
     Builder = (0, Team.Survivor)
     Support = (1, Team.Survivor)
```

### Comparing `KS_Constants-1.2.8/tests/basic_tests.py` & `KS_Constants-1.2.9/tests/basic_tests.py`

 * *Files identical despite different names*

