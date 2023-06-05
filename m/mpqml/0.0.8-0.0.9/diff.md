# Comparing `tmp/mpqml-0.0.8.tar.gz` & `tmp/mpqml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpqml-0.0.8.tar", last modified: Tue Mar 14 07:46:59 2023, max compression
+gzip compressed data, was "mpqml-0.0.9.tar", last modified: Mon Jun  5 02:43:25 2023, max compression
```

## Comparing `mpqml-0.0.8.tar` & `mpqml-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 07:46:59.743577 mpqml-0.0.8/
--rw-rw-rw-   0        0        0      229 2023-03-14 07:46:59.743192 mpqml-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-14 07:46:59.733515 mpqml-0.0.8/mpqml/
--rw-rw-rw-   0        0        0   202240 2023-03-14 07:45:21.000000 mpqml-0.0.8/mpqml/My_machine_learning.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0     5041 2023-02-10 05:40:49.000000 mpqml-0.0.8/mpqml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 07:46:59.742181 mpqml-0.0.8/mpqml.egg-info/
--rw-rw-rw-   0        0        0      229 2023-03-14 07:46:59.000000 mpqml-0.0.8/mpqml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-03-14 07:46:59.000000 mpqml-0.0.8/mpqml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 07:46:59.000000 mpqml-0.0.8/mpqml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-14 07:46:59.000000 mpqml-0.0.8/mpqml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 07:46:59.743577 mpqml-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      433 2023-03-14 07:43:09.000000 mpqml-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:43:25.833892 mpqml-0.0.9/
+-rw-rw-rw-   0        0        0      229 2023-06-05 02:43:25.832881 mpqml-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 02:43:25.828357 mpqml-0.0.9/mpqml/
+-rw-rw-rw-   0        0        0   202240 2023-03-14 07:45:21.000000 mpqml-0.0.9/mpqml/My_machine_learning.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0     5041 2023-02-10 05:40:49.000000 mpqml-0.0.9/mpqml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:43:25.832881 mpqml-0.0.9/mpqml.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-06-05 02:43:25.000000 mpqml-0.0.9/mpqml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-06-05 02:43:25.000000 mpqml-0.0.9/mpqml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 02:43:25.000000 mpqml-0.0.9/mpqml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-05 02:43:25.000000 mpqml-0.0.9/mpqml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 02:43:25.000000 mpqml-0.0.9/mpqml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 02:43:25.833892 mpqml-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      481 2023-06-05 02:42:36.000000 mpqml-0.0.9/setup.py
```

### Comparing `mpqml-0.0.8/mpqml/__init__.py` & `mpqml-0.0.9/mpqml/__init__.py`

 * *Files identical despite different names*

