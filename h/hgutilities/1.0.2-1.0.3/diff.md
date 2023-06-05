# Comparing `tmp/hgutilities-1.0.2.tar.gz` & `tmp/hgutilities-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgutilities-1.0.2.tar", last modified: Mon Jun  5 20:16:33 2023, max compression
+gzip compressed data, was "hgutilities-1.0.3.tar", last modified: Mon Jun  5 20:39:56 2023, max compression
```

## Comparing `hgutilities-1.0.2.tar` & `hgutilities-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,68 @@
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.102892 hgutilities-1.0.2/
--rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-05 19:53:05.000000 hgutilities-1.0.2/LICENSE.md
--rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:16:33.102640 hgutilities-1.0.2/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     7063 2023-06-05 20:01:22.000000 hgutilities-1.0.2/README.md
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.089474 hgutilities-1.0.2/hgutilities/
--rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.095716 hgutilities-1.0.2/hgutilities/defaults/
--rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     2881 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/docs.py
--rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/inherit.py
--rw-r-----   0 henry     (1000) henry     (1000)     1518 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/loaddefaults.py
--rw-r-----   0 henry     (1000) henry     (1000)     2502 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/defaults/processkwargs.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.098814 hgutilities-1.0.2/hgutilities/plotting/
--rw-r-----   0 henry     (1000) henry     (1000)     1098 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     2595 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/animate.py
--rw-r-----   0 henry     (1000) henry     (1000)     5255 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/figure.py
--rw-r-----   0 henry     (1000) henry     (1000)     2538 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/figures.py
--rw-r-----   0 henry     (1000) henry     (1000)      386 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/plotting/plotfunctions.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.101933 hgutilities-1.0.2/hgutilities/utils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/dicts.py
--rw-r-----   0 henry     (1000) henry     (1000)     1419 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/groups.py
--rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/paths.py
--rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-05 19:53:05.000000 hgutilities-1.0.2/hgutilities/utils/plots.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:16:33.092600 hgutilities-1.0.2/hgutilities.egg-info/
--rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)      701 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/SOURCES.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/dependency_links.txt
--rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-05 20:16:33.000000 hgutilities-1.0.2/hgutilities.egg-info/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-05 20:16:33.102987 hgutilities-1.0.2/setup.cfg
--rw-r-----   0 henry     (1000) henry     (1000)     1302 2023-06-05 20:16:03.000000 hgutilities-1.0.2/setup.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.589147 hgutilities-1.0.3/
+-rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-05 19:53:05.000000 hgutilities-1.0.3/LICENSE.md
+-rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:39:56.588866 hgutilities-1.0.3/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     7063 2023-06-05 20:01:22.000000 hgutilities-1.0.3/README.md
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.557078 hgutilities-1.0.3/hgutilities/
+-rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.562492 hgutilities-1.0.3/hgutilities/defaults/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.563188 hgutilities-1.0.3/hgutilities/defaults/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/defaults/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2881 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/docs.py
+-rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/inherit.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1518 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/loaddefaults.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2502 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/processkwargs.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.566440 hgutilities-1.0.3/hgutilities/plotting/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.567265 hgutilities-1.0.3/hgutilities/plotting/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.567826 hgutilities-1.0.3/hgutilities/plotting/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1098 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2595 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/animate.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.574084 hgutilities-1.0.3/hgutilities/plotting/datatypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.574859 hgutilities-1.0.3/hgutilities/plotting/datatypes/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.575675 hgutilities-1.0.3/hgutilities/plotting/datatypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      219 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/bar.py
+-rw-r-----   0 henry     (1000) henry     (1000)      992 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/bars.py
+-rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/colorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)      244 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/data.py
+-rw-r-----   0 henry     (1000) henry     (1000)      222 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/line.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1630 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/lines.py
+-rw-r-----   0 henry     (1000) henry     (1000)      370 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/pie.py
+-rw-r-----   0 henry     (1000) henry     (1000)      979 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/surface.py
+-rw-r-----   0 henry     (1000) henry     (1000)     5255 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/figure.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2538 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/figures.py
+-rw-r-----   0 henry     (1000) henry     (1000)      386 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotfunctions.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.580530 hgutilities-1.0.3/hgutilities/plotting/plottypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.581286 hgutilities-1.0.3/hgutilities/plotting/plottypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3209 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3354 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotbars.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2613 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotcolorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6683 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotlines.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1249 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotpie.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3691 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotsurface.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.585054 hgutilities-1.0.3/hgutilities/plotting/plotutils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      690 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/figuresize.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4445 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/griddimensions.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4425 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/plotshape.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1287 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/savefigure.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.588176 hgutilities-1.0.3/hgutilities/utils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/dicts.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1419 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/groups.py
+-rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/paths.py
+-rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/plots.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.559404 hgutilities-1.0.3/hgutilities.egg-info/
+-rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     1912 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/SOURCES.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/dependency_links.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/requires.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/top_level.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-05 20:39:56.589240 hgutilities-1.0.3/setup.cfg
+-rw-r-----   0 henry     (1000) henry     (1000)     1302 2023-06-05 20:39:36.000000 hgutilities-1.0.3/setup.py
```

### Comparing `hgutilities-1.0.2/LICENSE.md` & `hgutilities-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/PKG-INFO` & `hgutilities-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.2
+Version: 1.0.3
 Summary: A triple of tools used for plotting, handling key-words, and utilities
 Home-page: UNKNOWN
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
 License: UNKNOWN
 Keywords: python,matplotlib,plotting,default,keywords,utils
 Platform: UNKNOWN
```

### Comparing `hgutilities-1.0.2/README.md` & `hgutilities-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/defaults/docs.py` & `hgutilities-1.0.3/hgutilities/defaults/docs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/defaults/inherit.py` & `hgutilities-1.0.3/hgutilities/defaults/inherit.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/defaults/loaddefaults.py` & `hgutilities-1.0.3/hgutilities/defaults/loaddefaults.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/defaults/processkwargs.py` & `hgutilities-1.0.3/hgutilities/defaults/processkwargs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/plotting/__init__.py` & `hgutilities-1.0.3/hgutilities/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/plotting/animate.py` & `hgutilities-1.0.3/hgutilities/plotting/animate.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/plotting/figure.py` & `hgutilities-1.0.3/hgutilities/plotting/figure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/plotting/figures.py` & `hgutilities-1.0.3/hgutilities/plotting/figures.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/utils/groups.py` & `hgutilities-1.0.3/hgutilities/utils/groups.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/utils/paths.py` & `hgutilities-1.0.3/hgutilities/utils/paths.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities/utils/plots.py` & `hgutilities-1.0.3/hgutilities/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.2/hgutilities.egg-info/PKG-INFO` & `hgutilities-1.0.3/hgutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.2
+Version: 1.0.3
 Summary: A triple of tools used for plotting, handling key-words, and utilities
 Home-page: UNKNOWN
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
 License: UNKNOWN
 Keywords: python,matplotlib,plotting,default,keywords,utils
 Platform: UNKNOWN
```

### Comparing `hgutilities-1.0.2/setup.py` & `hgutilities-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
 LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
                     "Plotting: a front end for matplotlib to easily create subplots.\n"
                     "Utils: a collection of generally useful functions")
 
 # Setting up
 setup(
```

