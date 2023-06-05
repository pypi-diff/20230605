# Comparing `tmp/primerJinn-0.1.5.dev1.tar.gz` & `tmp/primerJinn-1.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primerJinn-0.1.5.dev1.tar", last modified: Thu May 25 18:29:24 2023, max compression
+gzip compressed data, was "primerJinn-1.0.0.dev1.tar", last modified: Mon Jun  5 20:35:42 2023, max compression
```

## Comparing `primerJinn-0.1.5.dev1.tar` & `primerJinn-1.0.0.dev1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-25 18:29:24.882906 primerJinn-0.1.5.dev1/
--rw-r--r--   0 semiquant   (502) staff       (20)    10982 2023-05-25 18:29:24.882661 primerJinn-0.1.5.dev1/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)    10553 2023-05-24 21:35:04.000000 primerJinn-0.1.5.dev1/README.md
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-25 18:29:24.882455 primerJinn-0.1.5.dev1/primerJinn.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)    10982 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      224 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)      162 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       71 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-25 18:29:24.882957 primerJinn-0.1.5.dev1/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     1697 2023-05-23 21:36:38.000000 primerJinn-0.1.5.dev1/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-06-05 20:35:42.425469 primerJinn-1.0.0.dev1/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10982 2023-06-05 20:35:42.425208 primerJinn-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)    10553 2023-05-24 21:35:04.000000 primerJinn-1.0.0.dev1/README.md
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-06-05 20:35:42.425019 primerJinn-1.0.0.dev1/primerJinn.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10982 2023-06-05 20:35:42.000000 primerJinn-1.0.0.dev1/primerJinn.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      224 2023-06-05 20:35:42.000000 primerJinn-1.0.0.dev1/primerJinn.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-06-05 20:35:42.000000 primerJinn-1.0.0.dev1/primerJinn.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)      162 2023-06-05 20:35:42.000000 primerJinn-1.0.0.dev1/primerJinn.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       71 2023-06-05 20:35:42.000000 primerJinn-1.0.0.dev1/primerJinn.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-06-05 20:35:42.000000 primerJinn-1.0.0.dev1/primerJinn.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-06-05 20:35:42.425516 primerJinn-1.0.0.dev1/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     1697 2023-06-05 20:35:25.000000 primerJinn-1.0.0.dev1/setup.py
```

### Comparing `primerJinn-0.1.5.dev1/PKG-INFO` & `primerJinn-1.0.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primerJinn
-Version: 0.1.5.dev1
+Version: 1.0.0.dev1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/primerJinn
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Classifier: Programming Language :: Python :: 3
```

### Comparing `primerJinn-0.1.5.dev1/README.md` & `primerJinn-1.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `primerJinn-0.1.5.dev1/primerJinn.egg-info/PKG-INFO` & `primerJinn-1.0.0.dev1/primerJinn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primerJinn
-Version: 0.1.5.dev1
+Version: 1.0.0.dev1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/primerJinn
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Classifier: Programming Language :: Python :: 3
```

### Comparing `primerJinn-0.1.5.dev1/setup.py` & `primerJinn-1.0.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         os.system("wget https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.14.0/ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("tar -xzvf ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("export PATH=$PATH:%s" % os.path.abspath("$(pwd)/ncbi-blast-2.14.0+/bin"))
 
 
 setup(
     name='primerJinn',
-    version='0.1.5.dev1',
+    version='1.0.0.dev1',
     url='https://github.com/SemiQuant/primerJinn',
     install_requires=dependencies,
     description='In silico PCR tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jason D Limberis',
     author_email='Jason.Limberis@ucsf.edu',
```

