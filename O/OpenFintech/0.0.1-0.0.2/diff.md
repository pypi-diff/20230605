# Comparing `tmp/OpenFintech-0.0.1.tar.gz` & `tmp/OpenFintech-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFintech-0.0.1.tar", last modified: Mon Jun  5 19:37:27 2023, max compression
+gzip compressed data, was "OpenFintech-0.0.2.tar", last modified: Mon Jun  5 19:46:23 2023, max compression
```

## Comparing `OpenFintech-0.0.1.tar` & `OpenFintech-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-05 19:37:27.155782 OpenFintech-0.0.1/
--rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.1/LICENSE
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-05 19:37:27.155067 OpenFintech-0.0.1/OpenFintech/
--rw-r--r--   0 harri      (501) staff       (20)        0 2023-06-05 19:21:39.000000 OpenFintech-0.0.1/OpenFintech/FinMongo.py
--rw-r--r--   0 harri      (501) staff       (20)        0 2023-06-05 19:20:23.000000 OpenFintech-0.0.1/OpenFintech/__init__.py
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-05 19:37:27.155520 OpenFintech-0.0.1/OpenFintech.egg-info/
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-05 19:37:27.000000 OpenFintech-0.0.1/OpenFintech.egg-info/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)      214 2023-06-05 19:37:27.000000 OpenFintech-0.0.1/OpenFintech.egg-info/SOURCES.txt
--rw-r--r--   0 harri      (501) staff       (20)        1 2023-06-05 19:37:27.000000 OpenFintech-0.0.1/OpenFintech.egg-info/dependency_links.txt
--rw-r--r--   0 harri      (501) staff       (20)       12 2023-06-05 19:37:27.000000 OpenFintech-0.0.1/OpenFintech.egg-info/top_level.txt
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-05 19:37:27.155673 OpenFintech-0.0.1/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)       14 2023-06-05 19:27:30.000000 OpenFintech-0.0.1/README.md
--rw-r--r--   0 harri      (501) staff       (20)       38 2023-06-05 19:37:27.155817 OpenFintech-0.0.1/setup.cfg
--rw-r--r--   0 harri      (501) staff       (20)      128 2023-06-05 19:36:38.000000 OpenFintech-0.0.1/setup.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-05 19:46:23.340360 OpenFintech-0.0.2/
+-rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.2/LICENSE
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-05 19:46:23.339532 OpenFintech-0.0.2/OpenFintech/
+-rw-r--r--   0 harri      (501) staff       (20)       91 2023-06-05 19:43:02.000000 OpenFintech-0.0.2/OpenFintech/FinMongo.py
+-rw-r--r--   0 harri      (501) staff       (20)       30 2023-06-05 19:43:01.000000 OpenFintech-0.0.2/OpenFintech/__init__.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-05 19:46:23.340104 OpenFintech-0.0.2/OpenFintech.egg-info/
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-05 19:46:23.000000 OpenFintech-0.0.2/OpenFintech.egg-info/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)      214 2023-06-05 19:46:23.000000 OpenFintech-0.0.2/OpenFintech.egg-info/SOURCES.txt
+-rw-r--r--   0 harri      (501) staff       (20)        1 2023-06-05 19:46:23.000000 OpenFintech-0.0.2/OpenFintech.egg-info/dependency_links.txt
+-rw-r--r--   0 harri      (501) staff       (20)       12 2023-06-05 19:46:23.000000 OpenFintech-0.0.2/OpenFintech.egg-info/top_level.txt
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-05 19:46:23.340261 OpenFintech-0.0.2/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)       14 2023-06-05 19:27:30.000000 OpenFintech-0.0.2/README.md
+-rw-r--r--   0 harri      (501) staff       (20)       38 2023-06-05 19:46:23.340392 OpenFintech-0.0.2/setup.cfg
+-rw-r--r--   0 harri      (501) staff       (20)      128 2023-06-05 19:45:12.000000 OpenFintech-0.0.2/setup.py
```

### Comparing `OpenFintech-0.0.1/LICENSE` & `OpenFintech-0.0.2/LICENSE`

 * *Files identical despite different names*

