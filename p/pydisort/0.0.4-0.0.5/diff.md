# Comparing `tmp/pydisort-0.0.4.tar.gz` & `tmp/pydisort-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisort-0.0.4.tar", last modified: Sun Jun  4 16:28:07 2023, max compression
+gzip compressed data, was "pydisort-0.0.5.tar", last modified: Mon Jun  5 05:08:55 2023, max compression
```

## Comparing `pydisort-0.0.4.tar` & `pydisort-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 16:28:07.991413 pydisort-0.0.4/
--rw-r--r--   0 zyhu       (502) staff       (20)       52 2023-06-04 16:28:07.990613 pydisort-0.0.4/PKG-INFO
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 16:28:07.982846 pydisort-0.0.4/pydisort/
--rw-r--r--   0 zyhu       (502) staff       (20)       24 2023-06-04 01:28:16.000000 pydisort-0.0.4/pydisort/__init__.py
--rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 16:24:51.000000 pydisort-0.0.4/pydisort/pydisort.cpython-310-darwin.so
--rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 00:45:04.000000 pydisort-0.0.4/pydisort/pydisort.cpython-311-darwin.so
--rw-r--r--   0 zyhu       (502) staff       (20)   656160 2023-06-04 04:41:55.000000 pydisort-0.0.4/pydisort/pydisort.cpython-36m-x86_64-linux-gnu.so
--rw-r--r--   0 zyhu       (502) staff       (20)   547920 2023-06-04 14:55:32.000000 pydisort-0.0.4/pydisort/pydisort.cpython-38-darwin.so
--rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 16:19:20.000000 pydisort-0.0.4/pydisort/pydisort.cpython-39-darwin.so
--rwxr-xr-x   0 zyhu       (502) staff       (20)   652096 2023-06-04 01:53:08.000000 pydisort-0.0.4/pydisort/pydisort.cpython-39-x86_64-linux-gnu.so
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 16:28:07.989755 pydisort-0.0.4/pydisort.egg-info/
--rw-r--r--   0 zyhu       (502) staff       (20)       52 2023-06-04 16:28:07.000000 pydisort-0.0.4/pydisort.egg-info/PKG-INFO
--rw-r--r--   0 zyhu       (502) staff       (20)      414 2023-06-04 16:28:07.000000 pydisort-0.0.4/pydisort.egg-info/SOURCES.txt
--rw-r--r--   0 zyhu       (502) staff       (20)        1 2023-06-04 16:28:07.000000 pydisort-0.0.4/pydisort.egg-info/dependency_links.txt
--rw-r--r--   0 zyhu       (502) staff       (20)        9 2023-06-04 16:28:07.000000 pydisort-0.0.4/pydisort.egg-info/top_level.txt
--rw-r--r--   0 zyhu       (502) staff       (20)       38 2023-06-04 16:28:07.992008 pydisort-0.0.4/setup.cfg
--rw-r--r--   0 zyhu       (502) staff       (20)      193 2023-06-04 16:27:37.000000 pydisort-0.0.4/setup.py
+drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-05 05:08:55.695918 pydisort-0.0.5/
+-rw-r--r--   0 zyhu       (502) staff       (20)       52 2023-06-05 05:08:55.695347 pydisort-0.0.5/PKG-INFO
+drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-05 05:08:55.688144 pydisort-0.0.5/pydisort/
+-rw-r--r--   0 zyhu       (502) staff       (20)       24 2023-06-04 19:26:25.000000 pydisort-0.0.5/pydisort/__init__.py
+-rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 19:26:25.000000 pydisort-0.0.5/pydisort/pydisort.cpython-310-darwin.so
+-rw-r--r--   0 zyhu       (502) staff       (20)   713704 2023-06-05 02:54:40.000000 pydisort-0.0.5/pydisort/pydisort.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 19:26:25.000000 pydisort-0.0.5/pydisort/pydisort.cpython-311-darwin.so
+-rw-r--r--   0 zyhu       (502) staff       (20)   709608 2023-06-05 04:55:44.000000 pydisort-0.0.5/pydisort/pydisort.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0 zyhu       (502) staff       (20)   656160 2023-06-04 19:26:25.000000 pydisort-0.0.5/pydisort/pydisort.cpython-36m-x86_64-linux-gnu.so
+-rw-r--r--   0 zyhu       (502) staff       (20)   697288 2023-06-05 05:03:09.000000 pydisort-0.0.5/pydisort/pydisort.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0 zyhu       (502) staff       (20)   547920 2023-06-04 19:26:25.000000 pydisort-0.0.5/pydisort/pydisort.cpython-38-darwin.so
+-rw-r--r--   0 zyhu       (502) staff       (20)   701384 2023-06-05 04:47:08.000000 pydisort-0.0.5/pydisort/pydisort.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 19:26:25.000000 pydisort-0.0.5/pydisort/pydisort.cpython-39-darwin.so
+-rwxr-xr-x   0 zyhu       (502) staff       (20)   652096 2023-06-04 19:26:25.000000 pydisort-0.0.5/pydisort/pydisort.cpython-39-x86_64-linux-gnu.so
+drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-05 05:08:55.694524 pydisort-0.0.5/pydisort.egg-info/
+-rw-r--r--   0 zyhu       (502) staff       (20)       52 2023-06-05 05:08:55.000000 pydisort-0.0.5/pydisort.egg-info/PKG-INFO
+-rw-r--r--   0 zyhu       (502) staff       (20)      613 2023-06-05 05:08:55.000000 pydisort-0.0.5/pydisort.egg-info/SOURCES.txt
+-rw-r--r--   0 zyhu       (502) staff       (20)        1 2023-06-05 05:08:55.000000 pydisort-0.0.5/pydisort.egg-info/dependency_links.txt
+-rw-r--r--   0 zyhu       (502) staff       (20)        9 2023-06-05 05:08:55.000000 pydisort-0.0.5/pydisort.egg-info/top_level.txt
+-rw-r--r--   0 zyhu       (502) staff       (20)       38 2023-06-05 05:08:55.696096 pydisort-0.0.5/setup.cfg
+-rw-r--r--   0 zyhu       (502) staff       (20)      193 2023-06-05 05:05:54.000000 pydisort-0.0.5/setup.py
```

### Comparing `pydisort-0.0.4/pydisort/pydisort.cpython-310-darwin.so` & `pydisort-0.0.5/pydisort/pydisort.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `pydisort-0.0.4/pydisort/pydisort.cpython-311-darwin.so` & `pydisort-0.0.5/pydisort/pydisort.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `pydisort-0.0.4/pydisort/pydisort.cpython-36m-x86_64-linux-gnu.so` & `pydisort-0.0.5/pydisort/pydisort.cpython-36m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pydisort-0.0.4/pydisort/pydisort.cpython-38-darwin.so` & `pydisort-0.0.5/pydisort/pydisort.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `pydisort-0.0.4/pydisort/pydisort.cpython-39-darwin.so` & `pydisort-0.0.5/pydisort/pydisort.cpython-39-darwin.so`

 * *Files identical despite different names*

### Comparing `pydisort-0.0.4/pydisort/pydisort.cpython-39-x86_64-linux-gnu.so` & `pydisort-0.0.5/pydisort/pydisort.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

