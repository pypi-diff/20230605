# Comparing `tmp/jykj-0.0.2.tar.gz` & `tmp/jykj-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jykj-0.0.2.tar", last modified: Fri May 19 02:29:14 2023, max compression
+gzip compressed data, was "jykj-0.0.3.tar", last modified: Mon Jun  5 03:23:09 2023, max compression
```

## Comparing `jykj-0.0.2.tar` & `jykj-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 02:29:14.267795 jykj-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      348 2023-05-19 02:29:14.266798 jykj-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-19 02:29:14.241796 jykj-0.0.2/jykj/
--rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.2/jykj/__init__.py
--rw-rw-rw-   0        0        0    11061 2023-05-19 02:20:55.000000 jykj-0.0.2/jykj/business_model.py
-drwxrwxrwx   0        0        0        0 2023-05-19 02:29:14.265812 jykj-0.0.2/jykj.egg-info/
--rw-rw-rw-   0        0        0      348 2023-05-19 02:29:14.000000 jykj-0.0.2/jykj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-19 02:29:14.000000 jykj-0.0.2/jykj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 02:29:14.000000 jykj-0.0.2/jykj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-19 02:29:14.000000 jykj-0.0.2/jykj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-19 02:29:14.000000 jykj-0.0.2/jykj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 02:29:14.267795 jykj-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      548 2023-05-19 02:29:02.000000 jykj-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:23:09.520947 jykj-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-05-04 06:17:54.000000 jykj-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      348 2023-06-05 03:23:09.519945 jykj-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 03:23:09.509531 jykj-0.0.3/jykj/
+-rw-rw-rw-   0        0        0        0 2023-05-15 03:16:59.000000 jykj-0.0.3/jykj/__init__.py
+-rw-rw-rw-   0        0        0    22779 2023-06-05 03:20:47.000000 jykj-0.0.3/jykj/business_model.py
+drwxrwxrwx   0        0        0        0 2023-06-05 03:23:09.518945 jykj-0.0.3/jykj.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-06-05 03:23:09.000000 jykj-0.0.3/jykj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-06-05 03:23:09.000000 jykj-0.0.3/jykj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 03:23:09.000000 jykj-0.0.3/jykj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 03:23:09.000000 jykj-0.0.3/jykj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-05 03:23:09.000000 jykj-0.0.3/jykj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 03:23:09.520947 jykj-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      548 2023-06-05 03:21:23.000000 jykj-0.0.3/setup.py
```

### Comparing `jykj-0.0.2/LICENSE` & `jykj-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jykj-0.0.2/setup.py` & `jykj-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jykj",
-    version="0.0.2",
+    version="0.0.3",
     author="jykj",
     author_email="renshuai@jylink.com",
     description="",
     long_description="",
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

