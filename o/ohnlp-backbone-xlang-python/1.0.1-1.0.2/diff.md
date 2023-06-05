# Comparing `tmp/ohnlp-backbone-xlang-python-1.0.1.tar.gz` & `tmp/ohnlp-backbone-xlang-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.1.tar", last modified: Mon Jun  5 16:18:24 2023, max compression
+gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.2.tar", last modified: Mon Jun  5 16:20:24 2023, max compression
```

## Comparing `ohnlp-backbone-xlang-python-1.0.1.tar` & `ohnlp-backbone-xlang-python-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:18:24.400888 ohnlp-backbone-xlang-python-1.0.1/
--rw-rw-rw-   0        0        0    11558 2023-05-25 17:32:33.000000 ohnlp-backbone-xlang-python-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      213 2023-06-05 16:18:24.399888 ohnlp-backbone-xlang-python-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      739 2023-06-05 15:53:15.000000 ohnlp-backbone-xlang-python-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 16:18:24.398888 ohnlp-backbone-xlang-python-1.0.1/ohnlp_backbone_xlang_python.egg-info/
--rw-rw-rw-   0        0        0      213 2023-06-05 16:18:24.000000 ohnlp-backbone-xlang-python-1.0.1/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-05 16:18:24.000000 ohnlp-backbone-xlang-python-1.0.1/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:18:24.000000 ohnlp-backbone-xlang-python-1.0.1/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      501 2023-06-05 16:18:24.000000 ohnlp-backbone-xlang-python-1.0.1/ohnlp_backbone_xlang_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:18:24.000000 ohnlp-backbone-xlang-python-1.0.1/ohnlp_backbone_xlang_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 16:18:24.400888 ohnlp-backbone-xlang-python-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1281 2023-06-05 16:18:20.000000 ohnlp-backbone-xlang-python-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:20:24.728199 ohnlp-backbone-xlang-python-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-05-25 17:32:33.000000 ohnlp-backbone-xlang-python-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      213 2023-06-05 16:20:24.727200 ohnlp-backbone-xlang-python-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      739 2023-06-05 15:53:15.000000 ohnlp-backbone-xlang-python-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:20:24.726201 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      501 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:20:24.728199 ohnlp-backbone-xlang-python-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-06-05 16:20:18.000000 ohnlp-backbone-xlang-python-1.0.2/setup.py
```

### Comparing `ohnlp-backbone-xlang-python-1.0.1/LICENSE` & `ohnlp-backbone-xlang-python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.1/README.md` & `ohnlp-backbone-xlang-python-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.1/setup.py` & `ohnlp-backbone-xlang-python-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import setuptools
 from setuptools import setup
 
-with open("requirements.txt") as f:
-    requirements = f.readlines()
-
 setup(
     name="ohnlp-backbone-xlang-python",
-    version="1.0.1",
+    version="1.0.2",
     description="Python support for OHNLP Toolkit Backbone Components",
     author="Andrew Wen",
     author_email="contact@ohnlp.org",
     packages=setuptools.find_packages(),
     install_requires=[
         'certifi==2023.5.7',
         'charset-normalizer==3.1.0',
```

