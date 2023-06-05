# Comparing `tmp/ohnlp-backbone-xlang-python-1.0.2.tar.gz` & `tmp/ohnlp-backbone-xlang-python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.2.tar", last modified: Mon Jun  5 16:20:24 2023, max compression
+gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.3.tar", last modified: Mon Jun  5 16:30:27 2023, max compression
```

## Comparing `ohnlp-backbone-xlang-python-1.0.2.tar` & `ohnlp-backbone-xlang-python-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:20:24.728199 ohnlp-backbone-xlang-python-1.0.2/
--rw-rw-rw-   0        0        0    11558 2023-05-25 17:32:33.000000 ohnlp-backbone-xlang-python-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      213 2023-06-05 16:20:24.727200 ohnlp-backbone-xlang-python-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      739 2023-06-05 15:53:15.000000 ohnlp-backbone-xlang-python-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 16:20:24.726201 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/
--rw-rw-rw-   0        0        0      213 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      501 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:20:24.000000 ohnlp-backbone-xlang-python-1.0.2/ohnlp_backbone_xlang_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 16:20:24.728199 ohnlp-backbone-xlang-python-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-06-05 16:20:18.000000 ohnlp-backbone-xlang-python-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:30:27.348736 ohnlp-backbone-xlang-python-1.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-05-25 17:32:33.000000 ohnlp-backbone-xlang-python-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      213 2023-06-05 16:30:27.348736 ohnlp-backbone-xlang-python-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      739 2023-06-05 15:53:15.000000 ohnlp-backbone-xlang-python-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:30:27.328736 ohnlp-backbone-xlang-python-1.0.3/ohnlp/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:31:44.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:30:27.329736 ohnlp-backbone-xlang-python-1.0.3/ohnlp/toolkit/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:31:44.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp/toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:30:27.333736 ohnlp-backbone-xlang-python-1.0.3/ohnlp/toolkit/backbone/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:31:44.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp/toolkit/backbone/__init__.py
+-rw-rw-rw-   0        0        0     7655 2023-06-01 21:38:52.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp/toolkit/backbone/api.py
+-rw-rw-rw-   0        0        0     1589 2023-05-26 20:57:11.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp/toolkit/backbone/backbone_module_launcher.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:30:27.346737 ohnlp-backbone-xlang-python-1.0.3/ohnlp_backbone_xlang_python.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-06-05 16:30:27.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-06-05 16:30:27.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:30:27.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      501 2023-06-05 16:30:27.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp_backbone_xlang_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 16:30:27.000000 ohnlp-backbone-xlang-python-1.0.3/ohnlp_backbone_xlang_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:30:27.349737 ohnlp-backbone-xlang-python-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-06-05 16:30:25.000000 ohnlp-backbone-xlang-python-1.0.3/setup.py
```

### Comparing `ohnlp-backbone-xlang-python-1.0.2/LICENSE` & `ohnlp-backbone-xlang-python-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.2/README.md` & `ohnlp-backbone-xlang-python-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.2/setup.py` & `ohnlp-backbone-xlang-python-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import setuptools
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="ohnlp-backbone-xlang-python",
-    version="1.0.2",
+    version="1.0.3",
     description="Python support for OHNLP Toolkit Backbone Components",
     author="Andrew Wen",
     author_email="contact@ohnlp.org",
-    packages=setuptools.find_packages(),
+    packages=find_packages(),
     install_requires=[
         'certifi==2023.5.7',
         'charset-normalizer==3.1.0',
         'cloudpickle==2.2.1',
         'crcmod==1.7',
         'dill==0.3.1.1',
         'dnspython==2.3.0',
```

