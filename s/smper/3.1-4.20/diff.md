# Comparing `tmp/smper-3.1.tar.gz` & `tmp/smper-4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smper-3.1.tar", last modified: Fri Jun  2 21:03:18 2023, max compression
+gzip compressed data, was "smper-4.20.tar", last modified: Mon Jun  5 12:03:57 2023, max compression
```

## Comparing `smper-3.1.tar` & `smper-4.20.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-02 21:03:18.808371 smper-3.1/
--rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-02 21:03:18.808179 smper-3.1/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smper-3.1/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-02 21:03:18.808434 smper-3.1/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      420 2023-06-02 21:03:15.000000 smper-3.1/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-02 21:03:18.806156 smper-3.1/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-02 21:03:18.806889 smper-3.1/src/smper/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smper-3.1/src/smper/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     8705 2023-06-02 21:02:03.000000 smper-3.1/src/smper/smper.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-02 21:03:18.807937 smper-3.1/src/smper.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-02 21:03:18.000000 smper-3.1/src/smper.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      223 2023-06-02 21:03:18.000000 smper-3.1/src/smper.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-02 21:03:18.000000 smper-3.1/src/smper.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-01-22 20:56:54.000000 smper-3.1/src/smper.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        6 2023-06-02 21:03:18.000000 smper-3.1/src/smper.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 12:03:57.708604 smper-4.20/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-05 12:03:57.708351 smper-4.20/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smper-4.20/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-05 12:03:57.708672 smper-4.20/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-05 12:03:54.000000 smper-4.20/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 12:03:57.706550 smper-4.20/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 12:03:57.707219 smper-4.20/src/smper/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smper-4.20/src/smper/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     6067 2023-06-05 12:03:47.000000 smper-4.20/src/smper/smper.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 12:03:57.708105 smper-4.20/src/smper.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-05 12:03:57.000000 smper-4.20/src/smper.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      223 2023-06-05 12:03:57.000000 smper-4.20/src/smper.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-05 12:03:57.000000 smper-4.20/src/smper.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-01-22 20:56:54.000000 smper-4.20/src/smper.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        6 2023-06-05 12:03:57.000000 smper-4.20/src/smper.egg-info/top_level.txt
```

