# Comparing `tmp/mlplatformutils-0.8.tar.gz` & `tmp/mlplatformutils-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.8.tar", last modified: Sun Jun  4 23:16:14 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.8.1.tar", last modified: Mon Jun  5 01:15:38 2023, max compression
```

## Comparing `mlplatformutils-0.8.tar` & `mlplatformutils-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 23:16:14.336393 mlplatformutils-0.8/
--rw-rw-rw-   0        0        0      293 2023-06-04 23:16:14.337389 mlplatformutils-0.8/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-04 23:16:14.342389 mlplatformutils-0.8/setup.cfg
--rw-rw-rw-   0        0        0      457 2023-06-04 23:15:33.000000 mlplatformutils-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 23:16:14.212829 mlplatformutils-0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 23:16:14.234861 mlplatformutils-0.8/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 23:16:14.332404 mlplatformutils-0.8/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.8/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.8/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.8/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       19 2023-06-04 23:15:23.000000 mlplatformutils-0.8/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-04 23:16:14.285383 mlplatformutils-0.8/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0      293 2023-06-04 23:16:13.000000 mlplatformutils-0.8/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-04 23:16:14.000000 mlplatformutils-0.8/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 23:16:13.000000 mlplatformutils-0.8/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-04 23:16:13.000000 mlplatformutils-0.8/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-04 23:16:13.000000 mlplatformutils-0.8/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.141885 mlplatformutils-0.8.1/
+-rw-rw-rw-   0        0        0     2938 2023-06-05 01:15:38.142886 mlplatformutils-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.1/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-05 01:15:38.156886 mlplatformutils-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-05 01:15:25.000000 mlplatformutils-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.012061 mlplatformutils-0.8.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.032568 mlplatformutils-0.8.1/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.1/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.137886 mlplatformutils-0.8.1/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-05 01:04:22.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.094344 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     2938 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.8/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.8.1/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.8.1/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.8.1/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.8.1/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.8.1/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.8.1/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

