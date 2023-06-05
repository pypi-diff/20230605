# Comparing `tmp/getModelSpec-1.0.1.tar.gz` & `tmp/getModelSpec-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getModelSpec-1.0.1.tar", last modified: Mon Jun  5 00:42:14 2023, max compression
+gzip compressed data, was "dist\getModelSpec-1.0.2.tar", last modified: Mon Jun  5 00:50:37 2023, max compression
```

## Comparing `getModelSpec-1.0.1.tar` & `getModelSpec-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/
--rw-rw-rw-   0        0        0      125 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getModelSpec-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/
--rw-rw-rw-   0        0        0      125 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/getModelSpec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      412 2023-06-05 00:40:28.000000 getModelSpec-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/src/
--rw-rw-rw-   0        0        0       36 2023-06-04 03:54:37.000000 getModelSpec-1.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     6360 2023-06-05 00:22:24.000000 getModelSpec-1.0.1/src/sony.py
-drwxrwxrwx   0        0        0        0 2023-06-05 00:42:14.000000 getModelSpec-1.0.1/tools/
--rw-rw-rw-   0        0        0      169 2023-06-04 09:34:54.000000 getModelSpec-1.0.1/tools/__init__.py
--rw-rw-rw-   0        0        0      926 2023-06-04 16:42:08.000000 getModelSpec-1.0.1/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/
+-rw-rw-rw-   0        0        0      125 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getModelSpec-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/getModelSpec.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/getModelSpec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/getModelSpec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/getModelSpec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/getModelSpec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/getModelSpec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/getModelSpec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      412 2023-06-05 00:50:23.000000 getModelSpec-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/src/
+-rw-rw-rw-   0        0        0       36 2023-06-04 03:54:37.000000 getModelSpec-1.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     6340 2023-06-05 00:49:00.000000 getModelSpec-1.0.2/src/sony.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:50:37.000000 getModelSpec-1.0.2/tools/
+-rw-rw-rw-   0        0        0       45 2023-06-05 00:49:00.000000 getModelSpec-1.0.2/tools/__init__.py
+-rw-rw-rw-   0        0        0      912 2023-06-05 00:49:00.000000 getModelSpec-1.0.2/tools/webdriver.py
```

### Comparing `getModelSpec-1.0.1/src/sony.py` & `getModelSpec-1.0.2/src/sony.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import time
 import re
 import pandas as pd
-import numpy as np
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 
 from tools.webdriver import WebDriver
```

### Comparing `getModelSpec-1.0.1/tools/webdriver.py` & `getModelSpec-1.0.2/tools/webdriver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import sys
 from selenium import webdriver
 
-
 class WebDriver:
     def __init__(self):
 
         pass
 
     @staticmethod
     def get_crome():
```

