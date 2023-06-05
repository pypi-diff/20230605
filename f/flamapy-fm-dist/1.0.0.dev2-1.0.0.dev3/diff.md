# Comparing `tmp/flamapy-fm-dist-1.0.0.dev2.tar.gz` & `tmp/flamapy-fm-dist-1.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-fm-dist-1.0.0.dev2.tar", last modified: Mon Jun  5 16:41:18 2023, max compression
+gzip compressed data, was "flamapy-fm-dist-1.0.0.dev3.tar", last modified: Mon Jun  5 21:33:03 2023, max compression
```

## Comparing `flamapy-fm-dist-1.0.0.dev2.tar` & `flamapy-fm-dist-1.0.0.dev3.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:41:18.033941 flamapy-fm-dist-1.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-05 16:41:05.000000 flamapy-fm-dist-1.0.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 16:41:18.033941 flamapy-fm-dist-1.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-05 16:41:05.000000 flamapy-fm-dist-1.0.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:41:18.033941 flamapy-fm-dist-1.0.0.dev2/flamapy_fm_dist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 16:41:17.000000 flamapy-fm-dist-1.0.0.dev2/flamapy_fm_dist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-05 16:41:17.000000 flamapy-fm-dist-1.0.0.dev2/flamapy_fm_dist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:41:17.000000 flamapy-fm-dist-1.0.0.dev2/flamapy_fm_dist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 16:41:17.000000 flamapy-fm-dist-1.0.0.dev2/flamapy_fm_dist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-05 16:41:17.000000 flamapy-fm-dist-1.0.0.dev2/flamapy_fm_dist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:41:17.000000 flamapy-fm-dist-1.0.0.dev2/flamapy_fm_dist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:41:18.033941 flamapy-fm-dist-1.0.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-05 16:41:05.000000 flamapy-fm-dist-1.0.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:41:18.033941 flamapy-fm-dist-1.0.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:41:05.000000 flamapy-fm-dist-1.0.0.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-05 16:41:05.000000 flamapy-fm-dist-1.0.0.dev2/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.088681 flamapy-fm-dist-1.0.0.dev3/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/command_line/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/command_line/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/python/FLAMAFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/flamapy/interfaces/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 21:33:03.000000 flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:33:03.092681 flamapy-fm-dist-1.0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-05 21:32:49.000000 flamapy-fm-dist-1.0.0.dev3/setup.py
```

### Comparing `flamapy-fm-dist-1.0.0.dev2/LICENSE` & `flamapy-fm-dist-1.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `flamapy-fm-dist-1.0.0.dev2/PKG-INFO` & `flamapy-fm-dist-1.0.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-fm-dist
-Version: 1.0.0.dev2
+Version: 1.0.0.dev3
 Summary: Flamapy feature model is a distribution of the flama framework containing all plugins required to analyze feature models. It also offers a richier API and a complete command line interface and documentation.
 Home-page: https://github.com/flamapy/flamapy-feature-model
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flamapy-fm-dist Version: 1.0.0.dev2 Summary:
+Metadata-Version: 2.1 Name: flamapy-fm-dist Version: 1.0.0.dev3 Summary:
 Flamapy feature model is a distribution of the flama framework containing all
 plugins required to analyze feature models. It also offers a richier API and a
 complete command line interface and documentation. Home-page: https://
 github.com/flamapy/flamapy-feature-model Author: Flamapy Author-email:
 flamapy@us.es License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
```

### Comparing `flamapy-fm-dist-1.0.0.dev2/README.md` & `flamapy-fm-dist-1.0.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `flamapy-fm-dist-1.0.0.dev2/flamapy_fm_dist.egg-info/PKG-INFO` & `flamapy-fm-dist-1.0.0.dev3/flamapy_fm_dist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-fm-dist
-Version: 1.0.0.dev2
+Version: 1.0.0.dev3
 Summary: Flamapy feature model is a distribution of the flama framework containing all plugins required to analyze feature models. It also offers a richier API and a complete command line interface and documentation.
 Home-page: https://github.com/flamapy/flamapy-feature-model
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flamapy-fm-dist Version: 1.0.0.dev2 Summary:
+Metadata-Version: 2.1 Name: flamapy-fm-dist Version: 1.0.0.dev3 Summary:
 Flamapy feature model is a distribution of the flama framework containing all
 plugins required to analyze feature models. It also offers a richier API and a
 complete command line interface and documentation. Home-page: https://
 github.com/flamapy/flamapy-feature-model Author: Flamapy Author-email:
 flamapy@us.es License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
```

### Comparing `flamapy-fm-dist-1.0.0.dev2/setup.py` & `flamapy-fm-dist-1.0.0.dev3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-fm-dist",
-    version="1.0.0.dev2",
+    version="1.0.0.dev3",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="Flamapy feature model is a distribution of the flama framework containing all plugins required to analyze feature models. It also offers a richier API and a complete command line interface and documentation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/flamapy-feature-model",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_namespace_packages(include=['flamapy.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
     install_requires=[
```

