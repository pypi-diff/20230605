# Comparing `tmp/smper-3.3.tar.gz` & `tmp/smper-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smper-3.3.tar", last modified: Mon Jun  5 11:56:42 2023, max compression
+gzip compressed data, was "smper-4.0.tar", last modified: Mon Jun  5 11:58:37 2023, max compression
```

## Comparing `smper-3.3.tar` & `smper-4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:56:42.529217 smper-3.3/
--rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-05 11:56:42.529028 smper-3.3/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smper-3.3/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-05 11:56:42.529287 smper-3.3/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      420 2023-06-05 11:56:39.000000 smper-3.3/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:56:42.527069 smper-3.3/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:56:42.527895 smper-3.3/src/smper/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smper-3.3/src/smper/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     5971 2023-06-05 11:55:29.000000 smper-3.3/src/smper/smper.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:56:42.528805 smper-3.3/src/smper.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-05 11:56:42.000000 smper-3.3/src/smper.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      223 2023-06-05 11:56:42.000000 smper-3.3/src/smper.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-05 11:56:42.000000 smper-3.3/src/smper.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-01-22 20:56:54.000000 smper-3.3/src/smper.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        6 2023-06-05 11:56:42.000000 smper-3.3/src/smper.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:58:37.168976 smper-4.0/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-05 11:58:37.168792 smper-4.0/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smper-4.0/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-05 11:58:37.169034 smper-4.0/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      420 2023-06-05 11:58:28.000000 smper-4.0/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:58:37.166898 smper-4.0/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:58:37.167791 smper-4.0/src/smper/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smper-4.0/src/smper/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     5971 2023-06-05 11:55:29.000000 smper-4.0/src/smper/smper.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:58:37.168592 smper-4.0/src/smper.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-05 11:58:37.000000 smper-4.0/src/smper.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      223 2023-06-05 11:58:37.000000 smper-4.0/src/smper.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-05 11:58:37.000000 smper-4.0/src/smper.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-01-22 20:56:54.000000 smper-4.0/src/smper.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        6 2023-06-05 11:58:37.000000 smper-4.0/src/smper.egg-info/top_level.txt
```

### Comparing `smper-3.3/src/smper/smper.py` & `smper-4.0/src/smper/smper.py`

 * *Files identical despite different names*

