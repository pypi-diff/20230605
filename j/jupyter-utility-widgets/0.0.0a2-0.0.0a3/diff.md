# Comparing `tmp/jupyter-utility-widgets-0.0.0a2.tar.gz` & `tmp/jupyter-utility-widgets-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-utility-widgets-0.0.0a2.tar", last modified: Fri May  5 16:07:38 2023, max compression
+gzip compressed data, was "jupyter-utility-widgets-0.0.0a3.tar", last modified: Mon Jun  5 10:15:33 2023, max compression
```

## Comparing `jupyter-utility-widgets-0.0.0a2.tar` & `jupyter-utility-widgets-0.0.0a3.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:38.228983 jupyter-utility-widgets-0.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-05 16:07:38.224983 jupyter-utility-widgets-0.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:38.224983 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/file_explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:38.224983 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/selector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/selector/index_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:38.224983 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:07:38.228983 jupyter-utility-widgets-0.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.687356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/file_explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.687356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/figures/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/figures/specgram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/selector/index_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.687356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/setup.cfg
```

### Comparing `jupyter-utility-widgets-0.0.0a2/LICENSE` & `jupyter-utility-widgets-0.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a2/PKG-INFO` & `jupyter-utility-widgets-0.0.0a3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.0a2
+Version: 0.0.0a3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
 
@@ -15,8 +15,14 @@
 may require jupyterlab installation.
 
 ## Widgets
 
 1. Index Selector
     A simple combination of widgets that help exploring a list of options.  
     see `examples/index_selector.ipynb`
+2. File Selector
+    A combination of widgets that help exploring the file system
+    see `examples/file_selector.ipynb`
+3. Spectrogram Viewer
+    A class for viewing spectrogram of data, with a simultaneous zoomed view.
+    see `examples/spectrogram.ipynb`
```

### Comparing `jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/selector/index_selector.py` & `jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/selector/index_selector.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/PKG-INFO` & `jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.0a2
+Version: 0.0.0a3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
 
@@ -15,8 +15,14 @@
 may require jupyterlab installation.
 
 ## Widgets
 
 1. Index Selector
     A simple combination of widgets that help exploring a list of options.  
     see `examples/index_selector.ipynb`
+2. File Selector
+    A combination of widgets that help exploring the file system
+    see `examples/file_selector.ipynb`
+3. Spectrogram Viewer
+    A class for viewing spectrogram of data, with a simultaneous zoomed view.
+    see `examples/spectrogram.ipynb`
```

