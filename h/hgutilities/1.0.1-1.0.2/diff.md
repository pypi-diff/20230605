# Comparing `tmp/hgutilities-1.0.1.tar.gz` & `tmp/hgutilities-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgutilities-1.0.1.tar", last modified: Mon Jun  5 20:06:47 2023, max compression
+gzip compressed data, was "hgutilities-1.0.2.tar", last modified: Mon Jun  5 20:16:33 2023, max compression
```

## Comparing `hgutilities-1.0.1.tar` & `hgutilities-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:06:47.181950 hgutilities-1.0.1/
--rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-05 19:53:05.000000 hgutilities-1.0.1/LICENSE.md
--rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:06:47.181665 hgutilities-1.0.1/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     7063 2023-06-05 20:01:22.000000 hgutilities-1.0.1/README.md
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:06:47.169021 hgutilities-1.0.1/hgutilities/
--rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:06:47.174746 hgutilities-1.0.1/hgutilities/defaults/
--rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/defaults/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     2881 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/defaults/docs.py
--rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/defaults/inherit.py
--rw-r-----   0 henry     (1000) henry     (1000)     1518 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/defaults/loaddefaults.py
--rw-r-----   0 henry     (1000) henry     (1000)     2502 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/defaults/processkwargs.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:06:47.177916 hgutilities-1.0.1/hgutilities/plotting/
--rw-r-----   0 henry     (1000) henry     (1000)     1098 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/plotting/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     2595 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/plotting/animate.py
--rw-r-----   0 henry     (1000) henry     (1000)     5255 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/plotting/figure.py
--rw-r-----   0 henry     (1000) henry     (1000)     2538 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/plotting/figures.py
--rw-r-----   0 henry     (1000) henry     (1000)      386 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/plotting/plotfunctions.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:06:47.181006 hgutilities-1.0.1/hgutilities/utils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/utils/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/utils/dicts.py
--rw-r-----   0 henry     (1000) henry     (1000)     1419 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/utils/groups.py
--rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/utils/paths.py
--rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-05 19:53:05.000000 hgutilities-1.0.1/hgutilities/utils/plots.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:06:47.171635 hgutilities-1.0.1/hgutilities.egg-info/
--rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:06:47.000000 hgutilities-1.0.1/hgutilities.egg-info/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)      701 2023-06-05 20:06:47.000000 hgutilities-1.0.1/hgutilities.egg-info/SOURCES.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-05 20:06:47.000000 hgutilities-1.0.1/hgutilities.egg-info/dependency_links.txt
--rw-r-----   0 henry     (1000) henry     (1000)       32 2023-06-05 20:06:47.000000 hgutilities-1.0.1/hgutilities.egg-info/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-05 20:06:47.000000 hgutilities-1.0.1/hgutilities.egg-info/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-05 20:06:47.182046 hgutilities-1.0.1/setup.cfg
--rw-r-----   0 henry     (1000) henry     (1000)     1299 2023-06-05 20:06:35.000000 hgutilities-1.0.1/setup.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.102892 hgutilities-1.0.2/
+-rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-05 19:53:05.000000 hgutilities-1.0.2/LICENSE.md
+-rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:16:33.102640 hgutilities-1.0.2/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     7063 2023-06-05 20:01:22.000000 hgutilities-1.0.2/README.md
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.089474 hgutilities-1.0.2/hgutilities/
+-rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.095716 hgutilities-1.0.2/hgutilities/defaults/
+-rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2881 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/docs.py
+-rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/inherit.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1518 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/loaddefaults.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2502 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/processkwargs.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.098814 hgutilities-1.0.2/hgutilities/plotting/
+-rw-r-----   0 henry     (1000) henry     (1000)     1098 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2595 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/animate.py
+-rw-r-----   0 henry     (1000) henry     (1000)     5255 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/figure.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2538 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/figures.py
+-rw-r-----   0 henry     (1000) henry     (1000)      386 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/plotfunctions.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.101933 hgutilities-1.0.2/hgutilities/utils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/dicts.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1419 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/groups.py
+-rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/paths.py
+-rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/plots.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.092600 hgutilities-1.0.2/hgutilities.egg-info/
+-rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)      701 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/SOURCES.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/dependency_links.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/requires.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/top_level.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-05 20:16:33.102987 hgutilities-1.0.2/setup.cfg
+-rw-r-----   0 henry     (1000) henry     (1000)     1302 2023-06-05 20:16:03.000000 hgutilities-1.0.2/setup.py
```

### Comparing `hgutilities-1.0.1/LICENSE.md` & `hgutilities-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/PKG-INFO` & `hgutilities-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.1
+Version: 1.0.2
 Summary: A triple of tools used for plotting, handling key-words, and utilities
 Home-page: UNKNOWN
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
 License: UNKNOWN
 Keywords: python,matplotlib,plotting,default,keywords,utils
 Platform: UNKNOWN
```

### Comparing `hgutilities-1.0.1/README.md` & `hgutilities-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/defaults/docs.py` & `hgutilities-1.0.2/hgutilities/defaults/docs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/defaults/inherit.py` & `hgutilities-1.0.2/hgutilities/defaults/inherit.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/defaults/loaddefaults.py` & `hgutilities-1.0.2/hgutilities/defaults/loaddefaults.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/defaults/processkwargs.py` & `hgutilities-1.0.2/hgutilities/defaults/processkwargs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/plotting/__init__.py` & `hgutilities-1.0.2/hgutilities/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/plotting/animate.py` & `hgutilities-1.0.2/hgutilities/plotting/animate.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/plotting/figure.py` & `hgutilities-1.0.2/hgutilities/plotting/figure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/plotting/figures.py` & `hgutilities-1.0.2/hgutilities/plotting/figures.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/utils/groups.py` & `hgutilities-1.0.2/hgutilities/utils/groups.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/utils/paths.py` & `hgutilities-1.0.2/hgutilities/utils/paths.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities/utils/plots.py` & `hgutilities-1.0.2/hgutilities/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/hgutilities.egg-info/PKG-INFO` & `hgutilities-1.0.2/hgutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.1
+Version: 1.0.2
 Summary: A triple of tools used for plotting, handling key-words, and utilities
 Home-page: UNKNOWN
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
 License: UNKNOWN
 Keywords: python,matplotlib,plotting,default,keywords,utils
 Platform: UNKNOWN
```

### Comparing `hgutilities-1.0.1/hgutilities.egg-info/SOURCES.txt` & `hgutilities-1.0.2/hgutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.1/setup.py` & `hgutilities-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
 LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
                     "Plotting: a front end for matplotlib to easily create subplots.\n"
                     "Utils: a collection of generally useful functions")
 
 # Setting up
 setup(
@@ -19,15 +19,15 @@
     version=VERSION,
     author="Henry Ginn",
     author_email="<henryginn137@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=["matplotlib", "numpy", "screeninfo", "PIL"],
+    install_requires=["matplotlib", "numpy", "screeninfo", "pillow"],
     keywords=["python", "matplotlib", "plotting", "default", "keywords", "utils"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
```

