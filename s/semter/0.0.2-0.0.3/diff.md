# Comparing `tmp/semter-0.0.2.tar.gz` & `tmp/semter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semter-0.0.2.tar", last modified: Mon Jun  5 16:20:54 2023, max compression
+gzip compressed data, was "semter-0.0.3.tar", last modified: Mon Jun  5 16:40:32 2023, max compression
```

## Comparing `semter-0.0.2.tar` & `semter-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:20:54.772022 semter-0.0.2/
--rw-rw-rw-   0        0        0     1065 2023-06-05 15:26:54.000000 semter-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-06-05 15:25:15.000000 semter-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      425 2023-06-05 16:20:54.772022 semter-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-06-05 15:22:16.000000 semter-0.0.2/README.rst
--rw-rw-rw-   0        0        0     5791 2023-06-05 15:31:40.000000 semter-0.0.2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:20:54.756418 semter-0.0.2/semter.egg-info/
--rw-rw-rw-   0        0        0      425 2023-06-05 16:20:54.000000 semter-0.0.2/semter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-06-05 16:20:54.000000 semter-0.0.2/semter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:20:54.000000 semter-0.0.2/semter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:20:54.000000 semter-0.0.2/semter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 16:20:54.772022 semter-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      539 2023-06-05 16:20:22.000000 semter-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:40:32.871827 semter-0.0.3/
+-rw-rw-rw-   0        0        0      129 2023-06-05 16:40:32.871827 semter-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 16:40:32.866844 semter-0.0.3/semter/
+-rw-rw-rw-   0        0        0       18 2023-06-05 16:09:14.000000 semter-0.0.3/semter/__init__.py
+-rw-rw-rw-   0        0        0     5773 2023-06-05 16:32:14.000000 semter-0.0.3/semter/tvz.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:40:32.870830 semter-0.0.3/semter.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-06-05 16:40:32.000000 semter-0.0.3/semter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-06-05 16:40:32.000000 semter-0.0.3/semter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:40:32.000000 semter-0.0.3/semter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 16:40:32.000000 semter-0.0.3/semter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-06-05 16:40:32.872823 semter-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-06-05 16:32:41.000000 semter-0.0.3/setup.py
```

### Comparing `semter-0.0.2/__init__.py` & `semter-0.0.3/semter/tvz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os.path
-
 
 class rv:
     def discrete(number):
         sklad = {1: "\
 import numpy as np\n\
 from scipy.stats import *\n\
 from tqdm import tqdm\n\
```

