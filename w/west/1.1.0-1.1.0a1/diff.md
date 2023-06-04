# Comparing `tmp/west-1.1.0.tar.gz` & `tmp/west-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "west-1.1.0.tar", last modified: Sun Jun  4 23:49:05 2023, max compression
+gzip compressed data, was "west-1.1.0a1.tar", last modified: Fri Jun  2 19:53:16 2023, max compression
```

## Comparing `west-1.1.0.tar` & `west-1.1.0a1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-04 23:49:05.674162 west-1.1.0/
--rw-r--r--   0 mbolivar   (501) staff       (20)    11357 2021-03-11 03:24:30.000000 west-1.1.0/LICENSE
--rw-r--r--   0 mbolivar   (501) staff       (20)      105 2023-05-01 21:45:22.000000 west-1.1.0/MANIFEST.in
--rw-r--r--   0 mbolivar   (501) staff       (20)     4509 2023-06-04 23:49:05.674040 west-1.1.0/PKG-INFO
--rw-r--r--   0 mbolivar   (501) staff       (20)     3958 2023-06-04 23:48:38.000000 west-1.1.0/README.rst
--rw-r--r--   0 mbolivar   (501) staff       (20)       38 2023-06-04 23:49:05.674193 west-1.1.0/setup.cfg
--rw-r--r--   0 mbolivar   (501) staff       (20)     1567 2023-05-01 21:45:22.000000 west-1.1.0/setup.py
-drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-04 23:49:05.668753 west-1.1.0/src/
-drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-04 23:49:05.671326 west-1.1.0/src/west/
--rw-r--r--   0 mbolivar   (501) staff       (20)      204 2021-03-11 03:24:30.000000 west-1.1.0/src/west/__init__.py
--rw-r--r--   0 mbolivar   (501) staff       (20)       39 2021-03-11 03:24:30.000000 west-1.1.0/src/west/__main__.py
-drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-04 23:49:05.672752 west-1.1.0/src/west/app/
--rw-r--r--   0 mbolivar   (501) staff       (20)       63 2021-03-11 03:24:30.000000 west-1.1.0/src/west/app/__init__.py
--rw-r--r--   0 mbolivar   (501) staff       (20)     7271 2023-05-01 21:45:22.000000 west-1.1.0/src/west/app/config.py
--rwxr-xr-x   0 mbolivar   (501) staff       (20)    46302 2023-06-04 23:48:38.000000 west-1.1.0/src/west/app/main.py
--rw-r--r--   0 mbolivar   (501) staff       (20)    76773 2023-06-04 23:48:38.000000 west-1.1.0/src/west/app/project.py
--rw-r--r--   0 mbolivar   (501) staff       (20)    24619 2023-05-01 21:45:22.000000 west-1.1.0/src/west/commands.py
--rw-r--r--   0 mbolivar   (501) staff       (20)    24014 2023-06-04 23:48:38.000000 west-1.1.0/src/west/configuration.py
--rw-r--r--   0 mbolivar   (501) staff       (20)     6501 2023-06-04 23:47:36.000000 west-1.1.0/src/west/log.py
--rw-r--r--   0 mbolivar   (501) staff       (20)     4797 2023-06-01 23:49:07.000000 west-1.1.0/src/west/manifest-schema.yml
--rw-r--r--   0 mbolivar   (501) staff       (20)   108818 2023-06-04 23:48:38.000000 west-1.1.0/src/west/manifest.py
--rw-r--r--   0 mbolivar   (501) staff       (20)        0 2023-05-01 21:45:22.000000 west-1.1.0/src/west/py.typed
--rw-r--r--   0 mbolivar   (501) staff       (20)     2926 2022-04-04 18:01:00.000000 west-1.1.0/src/west/util.py
--rw-r--r--   0 mbolivar   (501) staff       (20)      615 2023-06-04 23:48:38.000000 west-1.1.0/src/west/version.py
--rw-r--r--   0 mbolivar   (501) staff       (20)     1001 2021-03-11 03:24:30.000000 west-1.1.0/src/west/west-commands-schema.yml
-drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-04 23:49:05.672168 west-1.1.0/src/west.egg-info/
--rw-r--r--   0 mbolivar   (501) staff       (20)     4509 2023-06-04 23:49:05.000000 west-1.1.0/src/west.egg-info/PKG-INFO
--rw-r--r--   0 mbolivar   (501) staff       (20)      728 2023-06-04 23:49:05.000000 west-1.1.0/src/west.egg-info/SOURCES.txt
--rw-r--r--   0 mbolivar   (501) staff       (20)        1 2023-06-04 23:49:05.000000 west-1.1.0/src/west.egg-info/dependency_links.txt
--rw-r--r--   0 mbolivar   (501) staff       (20)       44 2023-06-04 23:49:05.000000 west-1.1.0/src/west.egg-info/entry_points.txt
--rw-r--r--   0 mbolivar   (501) staff       (20)        1 2023-06-04 23:49:05.000000 west-1.1.0/src/west.egg-info/not-zip-safe
--rw-r--r--   0 mbolivar   (501) staff       (20)       52 2023-06-04 23:49:05.000000 west-1.1.0/src/west.egg-info/requires.txt
--rw-r--r--   0 mbolivar   (501) staff       (20)        5 2023-06-04 23:49:05.000000 west-1.1.0/src/west.egg-info/top_level.txt
-drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-04 23:49:05.673829 west-1.1.0/tests/
--rw-r--r--   0 mbolivar   (501) staff       (20)      566 2023-05-01 21:45:22.000000 west-1.1.0/tests/test_commands.py
--rw-r--r--   0 mbolivar   (501) staff       (20)    19522 2023-06-04 23:48:38.000000 west-1.1.0/tests/test_config.py
--rw-r--r--   0 mbolivar   (501) staff       (20)     1658 2022-04-04 18:01:00.000000 west-1.1.0/tests/test_help.py
--rw-r--r--   0 mbolivar   (501) staff       (20)      795 2021-03-11 03:46:31.000000 west-1.1.0/tests/test_main.py
--rw-r--r--   0 mbolivar   (501) staff       (20)   101805 2023-06-04 23:48:38.000000 west-1.1.0/tests/test_manifest.py
--rw-r--r--   0 mbolivar   (501) staff       (20)    86895 2023-06-04 23:48:38.000000 west-1.1.0/tests/test_project.py
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.285008 west-1.1.0a1/
+-rw-r--r--   0 mbolivar   (501) staff       (20)    11357 2021-03-11 03:24:30.000000 west-1.1.0a1/LICENSE
+-rw-r--r--   0 mbolivar   (501) staff       (20)      105 2023-05-01 21:45:22.000000 west-1.1.0a1/MANIFEST.in
+-rw-r--r--   0 mbolivar   (501) staff       (20)     4511 2023-06-02 19:53:16.284880 west-1.1.0a1/PKG-INFO
+-rw-r--r--   0 mbolivar   (501) staff       (20)     3958 2023-05-01 21:45:22.000000 west-1.1.0a1/README.rst
+-rw-r--r--   0 mbolivar   (501) staff       (20)       38 2023-06-02 19:53:16.285047 west-1.1.0a1/setup.cfg
+-rw-r--r--   0 mbolivar   (501) staff       (20)     1567 2023-05-01 21:45:22.000000 west-1.1.0a1/setup.py
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.277415 west-1.1.0a1/src/
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.280625 west-1.1.0a1/src/west/
+-rw-r--r--   0 mbolivar   (501) staff       (20)      204 2021-03-11 03:24:30.000000 west-1.1.0a1/src/west/__init__.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)       39 2021-03-11 03:24:30.000000 west-1.1.0a1/src/west/__main__.py
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.281948 west-1.1.0a1/src/west/app/
+-rw-r--r--   0 mbolivar   (501) staff       (20)       63 2021-03-11 03:24:30.000000 west-1.1.0a1/src/west/app/__init__.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     7271 2023-05-01 21:45:22.000000 west-1.1.0a1/src/west/app/config.py
+-rwxr-xr-x   0 mbolivar   (501) staff       (20)    46302 2023-06-02 19:40:31.000000 west-1.1.0a1/src/west/app/main.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    76773 2023-06-02 19:40:31.000000 west-1.1.0a1/src/west/app/project.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    24619 2023-05-01 21:45:22.000000 west-1.1.0a1/src/west/commands.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    24014 2023-05-16 19:06:45.000000 west-1.1.0a1/src/west/configuration.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     6501 2023-05-01 21:45:22.000000 west-1.1.0a1/src/west/log.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     4797 2023-06-01 23:49:07.000000 west-1.1.0a1/src/west/manifest-schema.yml
+-rw-r--r--   0 mbolivar   (501) staff       (20)   108818 2023-06-02 19:40:31.000000 west-1.1.0a1/src/west/manifest.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)        0 2023-05-01 21:45:22.000000 west-1.1.0a1/src/west/py.typed
+-rw-r--r--   0 mbolivar   (501) staff       (20)     2926 2022-04-04 18:01:00.000000 west-1.1.0a1/src/west/util.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)      617 2023-06-02 19:50:05.000000 west-1.1.0a1/src/west/version.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     1001 2021-03-11 03:24:30.000000 west-1.1.0a1/src/west/west-commands-schema.yml
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.281465 west-1.1.0a1/src/west.egg-info/
+-rw-r--r--   0 mbolivar   (501) staff       (20)     4511 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/PKG-INFO
+-rw-r--r--   0 mbolivar   (501) staff       (20)      728 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/SOURCES.txt
+-rw-r--r--   0 mbolivar   (501) staff       (20)        1 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/dependency_links.txt
+-rw-r--r--   0 mbolivar   (501) staff       (20)       44 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/entry_points.txt
+-rw-r--r--   0 mbolivar   (501) staff       (20)        1 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/not-zip-safe
+-rw-r--r--   0 mbolivar   (501) staff       (20)       52 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/requires.txt
+-rw-r--r--   0 mbolivar   (501) staff       (20)        5 2023-06-02 19:53:16.000000 west-1.1.0a1/src/west.egg-info/top_level.txt
+drwxr-xr-x   0 mbolivar   (501) staff       (20)        0 2023-06-02 19:53:16.284229 west-1.1.0a1/tests/
+-rw-r--r--   0 mbolivar   (501) staff       (20)      566 2023-05-01 21:45:22.000000 west-1.1.0a1/tests/test_commands.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    19522 2023-05-16 19:06:45.000000 west-1.1.0a1/tests/test_config.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)     1658 2022-04-04 18:01:00.000000 west-1.1.0a1/tests/test_help.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)      795 2021-03-11 03:46:31.000000 west-1.1.0a1/tests/test_main.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)   101805 2023-06-02 19:40:31.000000 west-1.1.0a1/tests/test_manifest.py
+-rw-r--r--   0 mbolivar   (501) staff       (20)    86895 2023-05-16 19:06:45.000000 west-1.1.0a1/tests/test_project.py
```

### Comparing `west-1.1.0/LICENSE` & `west-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `west-1.1.0/PKG-INFO` & `west-1.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: west
-Version: 1.1.0
+Version: 1.1.0a1
 Summary: Zephyr RTOS Project meta-tool
 Home-page: https://github.com/zephyrproject-rtos/west
 Author: Zephyr Project
 Author-email: devel@lists.zephyrproject.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `west-1.1.0/README.rst` & `west-1.1.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `west-1.1.0/setup.py` & `west-1.1.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/app/config.py` & `west-1.1.0a1/src/west/app/config.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/app/main.py` & `west-1.1.0a1/src/west/app/main.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/app/project.py` & `west-1.1.0a1/src/west/app/project.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/commands.py` & `west-1.1.0a1/src/west/commands.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/configuration.py` & `west-1.1.0a1/src/west/configuration.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/log.py` & `west-1.1.0a1/src/west/log.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/manifest-schema.yml` & `west-1.1.0a1/src/west/manifest-schema.yml`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/manifest.py` & `west-1.1.0a1/src/west/manifest.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/util.py` & `west-1.1.0a1/src/west/util.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west/version.py` & `west-1.1.0a1/src/west/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2019, Nordic Semiconductor ASA
 #
 # Don't put anything else in here!
 #
 # This is the Python 3 version of option 3 in:
 # https://packaging.python.org/guides/single-sourcing-package-version/#single-sourcing-the-version
 
-__version__ = '1.1.0'
+__version__ = '1.1.0a1'
 #
 # MAINTAINERS:
 #
 # Make sure to update west.manifest.SCHEMA_VERSION if there have been
 # manifest schema version changes since the last release.
 #
 # Note that this is the "logical" west manifest schema, and that the
```

### Comparing `west-1.1.0/src/west/west-commands-schema.yml` & `west-1.1.0a1/src/west/west-commands-schema.yml`

 * *Files identical despite different names*

### Comparing `west-1.1.0/src/west.egg-info/PKG-INFO` & `west-1.1.0a1/src/west.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: west
-Version: 1.1.0
+Version: 1.1.0a1
 Summary: Zephyr RTOS Project meta-tool
 Home-page: https://github.com/zephyrproject-rtos/west
 Author: Zephyr Project
 Author-email: devel@lists.zephyrproject.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `west-1.1.0/src/west.egg-info/SOURCES.txt` & `west-1.1.0a1/src/west.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `west-1.1.0/tests/test_commands.py` & `west-1.1.0a1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/tests/test_config.py` & `west-1.1.0a1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/tests/test_help.py` & `west-1.1.0a1/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/tests/test_main.py` & `west-1.1.0a1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/tests/test_manifest.py` & `west-1.1.0a1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `west-1.1.0/tests/test_project.py` & `west-1.1.0a1/tests/test_project.py`

 * *Files identical despite different names*

