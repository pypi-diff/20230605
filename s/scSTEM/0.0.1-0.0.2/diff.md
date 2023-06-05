# Comparing `tmp/scSTEM-0.0.1.tar.gz` & `tmp/scSTEM-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scSTEM-0.0.1.tar", last modified: Mon Jun  5 07:09:05 2023, max compression
+gzip compressed data, was "scSTEM-0.0.2.tar", last modified: Mon Jun  5 07:16:30 2023, max compression
```

## Comparing `scSTEM-0.0.1.tar` & `scSTEM-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hms       (1001) hms       (1001)        0 2023-06-05 07:09:05.110448 scSTEM-0.0.1/
--rw-rw-r--   0 hms       (1001) hms       (1001)     6000 2023-06-05 07:09:05.110448 scSTEM-0.0.1/PKG-INFO
--rw-rw-r--   0 hms       (1001) hms       (1001)     4681 2023-06-05 07:03:43.000000 scSTEM-0.0.1/README.md
-drwxrwxr-x   0 hms       (1001) hms       (1001)        0 2023-06-05 07:09:05.110448 scSTEM-0.0.1/STEM/
--rw-rw-r--   0 hms       (1001) hms       (1001)       65 2023-03-16 02:41:45.000000 scSTEM-0.0.1/STEM/__init__.py
--rw-rw-r--   0 hms       (1001) hms       (1001)     3539 2023-03-16 02:42:34.000000 scSTEM-0.0.1/STEM/evaluate.py
--rw-rw-r--   0 hms       (1001) hms       (1001)     8735 2023-03-16 08:19:45.000000 scSTEM-0.0.1/STEM/model.py
--rw-rw-r--   0 hms       (1001) hms       (1001)     3057 2023-03-16 02:43:13.000000 scSTEM-0.0.1/STEM/utils.py
-drwxrwxr-x   0 hms       (1001) hms       (1001)        0 2023-06-05 07:09:05.110448 scSTEM-0.0.1/scSTEM.egg-info/
--rw-rw-r--   0 hms       (1001) hms       (1001)     6000 2023-06-05 07:09:05.000000 scSTEM-0.0.1/scSTEM.egg-info/PKG-INFO
--rw-rw-r--   0 hms       (1001) hms       (1001)      229 2023-06-05 07:09:05.000000 scSTEM-0.0.1/scSTEM.egg-info/SOURCES.txt
--rw-rw-r--   0 hms       (1001) hms       (1001)        1 2023-06-05 07:09:05.000000 scSTEM-0.0.1/scSTEM.egg-info/dependency_links.txt
--rw-rw-r--   0 hms       (1001) hms       (1001)       59 2023-06-05 07:09:05.000000 scSTEM-0.0.1/scSTEM.egg-info/requires.txt
--rw-rw-r--   0 hms       (1001) hms       (1001)        5 2023-06-05 07:09:05.000000 scSTEM-0.0.1/scSTEM.egg-info/top_level.txt
--rw-rw-r--   0 hms       (1001) hms       (1001)       38 2023-06-05 07:09:05.110448 scSTEM-0.0.1/setup.cfg
--rw-rw-r--   0 hms       (1001) hms       (1001)      770 2023-06-05 07:08:32.000000 scSTEM-0.0.1/setup.py
+drwxrwxr-x   0 hms       (1001) hms       (1001)        0 2023-06-05 07:16:30.917285 scSTEM-0.0.2/
+-rw-rw-r--   0 hms       (1001) hms       (1001)     6000 2023-06-05 07:16:30.917285 scSTEM-0.0.2/PKG-INFO
+-rw-rw-r--   0 hms       (1001) hms       (1001)     4681 2023-06-05 07:03:43.000000 scSTEM-0.0.2/README.md
+drwxrwxr-x   0 hms       (1001) hms       (1001)        0 2023-06-05 07:16:30.917285 scSTEM-0.0.2/STEM/
+-rw-rw-r--   0 hms       (1001) hms       (1001)       65 2023-03-16 02:41:45.000000 scSTEM-0.0.2/STEM/__init__.py
+-rw-rw-r--   0 hms       (1001) hms       (1001)     3539 2023-03-16 02:42:34.000000 scSTEM-0.0.2/STEM/evaluate.py
+-rw-rw-r--   0 hms       (1001) hms       (1001)     8735 2023-03-16 08:19:45.000000 scSTEM-0.0.2/STEM/model.py
+-rw-rw-r--   0 hms       (1001) hms       (1001)     3057 2023-03-16 02:43:13.000000 scSTEM-0.0.2/STEM/utils.py
+drwxrwxr-x   0 hms       (1001) hms       (1001)        0 2023-06-05 07:16:30.917285 scSTEM-0.0.2/scSTEM.egg-info/
+-rw-rw-r--   0 hms       (1001) hms       (1001)     6000 2023-06-05 07:16:30.000000 scSTEM-0.0.2/scSTEM.egg-info/PKG-INFO
+-rw-rw-r--   0 hms       (1001) hms       (1001)      229 2023-06-05 07:16:30.000000 scSTEM-0.0.2/scSTEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 hms       (1001) hms       (1001)        1 2023-06-05 07:16:30.000000 scSTEM-0.0.2/scSTEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 hms       (1001) hms       (1001)       43 2023-06-05 07:16:30.000000 scSTEM-0.0.2/scSTEM.egg-info/requires.txt
+-rw-rw-r--   0 hms       (1001) hms       (1001)        5 2023-06-05 07:16:30.000000 scSTEM-0.0.2/scSTEM.egg-info/top_level.txt
+-rw-rw-r--   0 hms       (1001) hms       (1001)       38 2023-06-05 07:16:30.917285 scSTEM-0.0.2/setup.cfg
+-rw-rw-r--   0 hms       (1001) hms       (1001)      743 2023-06-05 07:16:25.000000 scSTEM-0.0.2/setup.py
```

### Comparing `scSTEM-0.0.1/PKG-INFO` & `scSTEM-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scSTEM
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Method for Mapping Single-cell and Spatial Transcriptomics Data with Transfer Learning
 Home-page: https://github.com/WhirlFirst/STEM
 Author: whirl
 Author-email: hmsh653@gmail.com
 License: UNKNOWN
 Description: # <a href='https://github.com/WhirlFirst/STEM'><img src='img/STEM.png' align="Middle" height="200" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scSTEM Version: 0.0.1 Summary: A Method for Mapping
+Metadata-Version: 2.1 Name: scSTEM Version: 0.0.2 Summary: A Method for Mapping
 Single-cell and Spatial Transcriptomics Data with Transfer Learning Home-page:
 https://github.com/WhirlFirst/STEM Author: whirl Author-email:
 hmsh653@gmail.com License: UNKNOWN Description: # [img/STEM.png] # Welcome! ##
 1. Introduction and installation STEM is a tool for building single-cell level
 spatial transcriptomic landscapes using SC data with ST data. STEM extracts the
 spatial information from the gene expressions and eliminates the domain gap
 between spatial transcriptomics and single-cell RNA-seq data. ### Installation
```

### Comparing `scSTEM-0.0.1/README.md` & `scSTEM-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scSTEM-0.0.1/STEM/evaluate.py` & `scSTEM-0.0.2/STEM/evaluate.py`

 * *Files identical despite different names*

### Comparing `scSTEM-0.0.1/STEM/model.py` & `scSTEM-0.0.2/STEM/model.py`

 * *Files identical despite different names*

### Comparing `scSTEM-0.0.1/STEM/utils.py` & `scSTEM-0.0.2/STEM/utils.py`

 * *Files identical despite different names*

### Comparing `scSTEM-0.0.1/scSTEM.egg-info/PKG-INFO` & `scSTEM-0.0.2/scSTEM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scSTEM
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Method for Mapping Single-cell and Spatial Transcriptomics Data with Transfer Learning
 Home-page: https://github.com/WhirlFirst/STEM
 Author: whirl
 Author-email: hmsh653@gmail.com
 License: UNKNOWN
 Description: # <a href='https://github.com/WhirlFirst/STEM'><img src='img/STEM.png' align="Middle" height="200" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scSTEM Version: 0.0.1 Summary: A Method for Mapping
+Metadata-Version: 2.1 Name: scSTEM Version: 0.0.2 Summary: A Method for Mapping
 Single-cell and Spatial Transcriptomics Data with Transfer Learning Home-page:
 https://github.com/WhirlFirst/STEM Author: whirl Author-email:
 hmsh653@gmail.com License: UNKNOWN Description: # [img/STEM.png] # Welcome! ##
 1. Introduction and installation STEM is a tool for building single-cell level
 spatial transcriptomic landscapes using SC data with ST data. STEM extracts the
 spatial information from the gene expressions and eliminates the domain gap
 between spatial transcriptomics and single-cell RNA-seq data. ### Installation
```

### Comparing `scSTEM-0.0.1/setup.py` & `scSTEM-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scSTEM",
-    version="0.0.1",
+    version="0.0.2",
     author="whirl",
     author_email="hmsh653@gmail.com",
     description="A Method for Mapping Single-cell and Spatial Transcriptomics Data with Transfer Learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WhirlFirst/STEM",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     install_requires=[
-        "pytorch>=1.13.1",
         "scanpy>=1.8.2",
         "tqdm>=4.60.0",
         "seaborn>=0.11.1",
     ],
 )
```

