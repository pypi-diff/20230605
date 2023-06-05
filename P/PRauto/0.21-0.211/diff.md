# Comparing `tmp/PRauto-0.21.tar.gz` & `tmp/PRauto-0.211.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.21.tar", last modified: Mon Jun  5 01:57:59 2023, max compression
+gzip compressed data, was "PRauto-0.211.tar", last modified: Mon Jun  5 02:03:26 2023, max compression
```

## Comparing `PRauto-0.21.tar` & `PRauto-0.211.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.636839 PRauto-0.21/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.21/LICENSE
--rw-rw-rw-   0        0        0      348 2023-06-05 01:57:59.636839 PRauto-0.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.602530 PRauto-0.21/PRauto.egg-info/
--rw-rw-rw-   0        0        0      348 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2088 2023-04-21 03:50:22.000000 PRauto-0.21/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.606531 PRauto-0.21/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.21/prauto/__init__.py
--rw-rw-rw-   0        0        0     3178 2023-06-02 04:51:18.000000 PRauto-0.21/prauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.614442 PRauto-0.21/prauto/prepauto/
--rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.21/prauto/prepauto/__init__.py
--rw-rw-rw-   0        0        0    14202 2023-05-10 05:53:19.000000 PRauto-0.21/prauto/prepauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.633841 PRauto-0.21/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.21/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     3061 2023-06-02 01:56:52.000000 PRauto-0.21/prauto/retriever/__main__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.21/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     5901 2023-06-02 02:00:27.000000 PRauto-0.21/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4276 2023-04-26 06:35:58.000000 PRauto-0.21/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-06-05 01:57:59.637839 PRauto-0.21/setup.cfg
--rw-rw-rw-   0        0        0     1249 2023-06-05 01:57:35.000000 PRauto-0.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.915933 PRauto-0.211/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.211/LICENSE
+-rw-rw-rw-   0        0        0      349 2023-06-05 02:03:26.915168 PRauto-0.211/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.899472 PRauto-0.211/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 02:03:26.000000 PRauto-0.211/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2088 2023-04-21 03:50:22.000000 PRauto-0.211/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.902472 PRauto-0.211/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.211/prauto/__init__.py
+-rw-rw-rw-   0        0        0     3181 2023-06-05 02:01:10.000000 PRauto-0.211/prauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.905471 PRauto-0.211/prauto/prepauto/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.211/prauto/prepauto/__init__.py
+-rw-rw-rw-   0        0        0    14202 2023-05-10 05:53:19.000000 PRauto-0.211/prauto/prepauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:03:26.913456 PRauto-0.211/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.211/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-06-05 02:01:33.000000 PRauto-0.211/prauto/retriever/__main__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.211/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     5901 2023-06-02 02:00:27.000000 PRauto-0.211/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4276 2023-04-26 06:35:58.000000 PRauto-0.211/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-06-05 02:03:26.915933 PRauto-0.211/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-06-05 02:02:19.000000 PRauto-0.211/setup.py
```

### Comparing `PRauto-0.21/LICENSE` & `PRauto-0.211/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.21/README.md` & `PRauto-0.211/README.md`

 * *Files identical despite different names*

### Comparing `PRauto-0.21/prauto/__main__.py` & `PRauto-0.211/prauto/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
-from retriever.get_fasta import *
-from retriever.get_pdb import *
-from retriever.get_ligand import *
+from .retriever.get_fasta import *
+from .retriever.get_pdb import *
+from .retriever.get_ligand import *
 from tqdm.auto import tqdm
 from tkinter import Tk
 from tkinter import filedialog
 
 root = Tk()
 root.withdraw()
```

### Comparing `PRauto-0.21/prauto/prepauto/__main__.py` & `PRauto-0.211/prauto/prepauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.21/prauto/retriever/__main__.py` & `PRauto-0.211/prauto/retriever/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
-from get_fasta import *
-from get_pdb import *
-from get_ligand import *
+from .get_fasta import *
+from .get_pdb import *
+from .get_ligand import *
 from tqdm.auto import tqdm
 from tkinter import Tk
 from tkinter import filedialog
 
 root = Tk()
 root.withdraw()
```

### Comparing `PRauto-0.21/prauto/retriever/get_fasta.py` & `PRauto-0.211/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.21/prauto/retriever/get_ligand.py` & `PRauto-0.211/prauto/retriever/get_ligand.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.21/prauto/retriever/get_pdb.py` & `PRauto-0.211/prauto/retriever/get_pdb.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.21/setup.py` & `PRauto-0.211/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages, Extension
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.21',
+        version = '0.211',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
```

