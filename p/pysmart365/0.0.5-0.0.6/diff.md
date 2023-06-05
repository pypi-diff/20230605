# Comparing `tmp/pysmart365-0.0.5.tar.gz` & `tmp/pysmart365-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmart365-0.0.5.tar", last modified: Fri Jun  2 13:27:55 2023, max compression
+gzip compressed data, was "pysmart365-0.0.6.tar", last modified: Mon Jun  5 13:04:03 2023, max compression
```

## Comparing `pysmart365-0.0.5.tar` & `pysmart365-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 13:27:55.989868 pysmart365-0.0.5/
--rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      442 2023-06-02 13:27:55.989868 pysmart365-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-06-02 13:24:19.000000 pysmart365-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 13:27:55.970916 pysmart365-0.0.5/pysmart365/
--rw-rw-rw-   0        0        0     1028 2023-06-02 13:27:34.000000 pysmart365-0.0.5/pysmart365/MicroSoftware.py
--rw-rw-rw-   0        0        0     2218 2023-06-02 13:27:19.000000 pysmart365-0.0.5/pysmart365/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:27:55.988871 pysmart365-0.0.5/pysmart365.egg-info/
--rw-rw-rw-   0        0        0      442 2023-06-02 13:27:55.000000 pysmart365-0.0.5/pysmart365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-02 13:27:55.000000 pysmart365-0.0.5/pysmart365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 13:27:55.000000 pysmart365-0.0.5/pysmart365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-02 13:27:55.000000 pysmart365-0.0.5/pysmart365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 13:27:55.989868 pysmart365-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      504 2023-06-02 13:25:17.000000 pysmart365-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:04:03.214539 pysmart365-0.0.6/
+-rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      353 2023-06-05 13:04:03.213536 pysmart365-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-06-02 13:24:19.000000 pysmart365-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 13:04:03.203563 pysmart365-0.0.6/pysmart365/
+-rw-rw-rw-   0        0        0     1028 2023-06-02 13:27:34.000000 pysmart365-0.0.6/pysmart365/MicroSoftware.py
+-rw-rw-rw-   0        0        0     2218 2023-06-02 13:27:19.000000 pysmart365-0.0.6/pysmart365/__init__.py
+-rw-rw-rw-   0        0        0      296 2023-06-05 12:16:16.000000 pysmart365-0.0.6/pysmart365/modules.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:04:03.212538 pysmart365-0.0.6/pysmart365.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-05 13:04:03.000000 pysmart365-0.0.6/pysmart365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-05 13:04:03.000000 pysmart365-0.0.6/pysmart365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 13:04:03.000000 pysmart365-0.0.6/pysmart365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-05 13:04:03.000000 pysmart365-0.0.6/pysmart365.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 13:04:03.000000 pysmart365-0.0.6/pysmart365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 13:04:03.214539 pysmart365-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-06-05 13:03:50.000000 pysmart365-0.0.6/setup.py
```

### Comparing `pysmart365-0.0.5/LICENSE` & `pysmart365-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.5/README.md` & `pysmart365-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.5/pysmart365/MicroSoftware.py` & `pysmart365-0.0.6/pysmart365/MicroSoftware.py`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.5/pysmart365/__init__.py` & `pysmart365-0.0.6/pysmart365/__init__.py`

 * *Files identical despite different names*

