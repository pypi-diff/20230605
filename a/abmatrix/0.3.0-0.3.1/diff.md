# Comparing `tmp/abmatrix-0.3.0.tar.gz` & `tmp/abmatrix-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.3.0.tar", last modified: Sun Jun  4 19:02:00 2023, max compression
+gzip compressed data, was "abmatrix-0.3.1.tar", last modified: Mon Jun  5 05:32:06 2023, max compression
```

## Comparing `abmatrix-0.3.0.tar` & `abmatrix-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:02:00.836068 abmatrix-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-04 19:02:00.836068 abmatrix-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-04 19:01:51.000000 abmatrix-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:02:00.832068 abmatrix-0.3.0/abmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 19:01:51.000000 abmatrix-0.3.0/abmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-04 19:01:51.000000 abmatrix-0.3.0/abmatrix/abmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:02:00.832068 abmatrix-0.3.0/abmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-04 19:02:00.000000 abmatrix-0.3.0/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-04 19:02:00.000000 abmatrix-0.3.0/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 19:02:00.000000 abmatrix-0.3.0/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 19:02:00.000000 abmatrix-0.3.0/abmatrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 19:01:51.000000 abmatrix-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-04 19:02:00.836068 abmatrix-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:32:06.242778 abmatrix-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-05 05:32:06.242778 abmatrix-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-05 05:31:53.000000 abmatrix-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:32:06.242778 abmatrix-0.3.1/abmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:31:53.000000 abmatrix-0.3.1/abmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-05 05:31:53.000000 abmatrix-0.3.1/abmatrix/abmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:32:06.242778 abmatrix-0.3.1/abmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-05 05:32:06.000000 abmatrix-0.3.1/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-05 05:32:06.000000 abmatrix-0.3.1/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 05:32:06.000000 abmatrix-0.3.1/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 05:32:06.000000 abmatrix-0.3.1/abmatrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 05:31:53.000000 abmatrix-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 05:32:06.242778 abmatrix-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:32:06.242778 abmatrix-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-05 05:31:53.000000 abmatrix-0.3.1/tests/test_subset.py
```

### Comparing `abmatrix-0.3.0/PKG-INFO` & `abmatrix-0.3.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abmatrix
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python module to read and parse AB Matrix files
 Author-email: Daniel Garrigan <popgendad@proton.me>
 Project-URL: Homepage, https://github.com/wisdomhealth-inc/abmatrix
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -25,23 +25,24 @@
 
 abmatrix.abmatrix.**read**(abmatrixfile)
 
 Read an AB Matrix file, read header and lazy load genotype data
 
 ---
 
-abmatrix.abmatrix.**write**(abmatrixfile)
+abmatrix.abmatrix.**write**(abmatrixfile, genotypes)
 
 Write an AB Matrix file from in-memory instance of class
 
 ---
 
-abmatrix.abmatrix.**subset**(locus_list, sample_list)
+abmatrix.abmatrix.**subset**(locus_list, samples=sample_list)
 
-Get subset of AB Matrix data set
+Get subset of AB Matrix data set. Returns genotype matrix as list
+of dictionaries.
 
 ---
 
 abmatrix.abmatrix.**close**()
 
 Close instance of abmatrix data set
 
@@ -50,23 +51,23 @@
 ## Example
 ```python
 from abmatrix import abmatrix
 
 # Initialize
 myabmatrix = abmatrix.abmatrix()
 
-myabmatrix.open("test_abmatrix.zip")
+myabmatrix.read("test_abmatrix.zip")
 
-TRAIT_LIST = [
+SNP_IDS = [
     "442_HPS3",
     "054_FGF4_chr12",
     "077_TYRP_LH",
     "077_TYRP1_SH",
     "441_USH2A_roan",
     "277_MC1R_cockersable_Eh",
 ]
 
-output = myabmatrix.reduce(TRAIT_LIST)
-print(output)
+genotypes = myabmatrix.subset(SNP_IDS)
+myabmatrix.write("test_abmatrix_subset.ab", genotypes)
 
 myabmatrix.close()
 ```
```

### Comparing `abmatrix-0.3.0/README.md` & `abmatrix-0.3.1/abmatrix.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: abmatrix
+Version: 0.3.1
+Summary: Python module to read and parse AB Matrix files
+Author-email: Daniel Garrigan <popgendad@proton.me>
+Project-URL: Homepage, https://github.com/wisdomhealth-inc/abmatrix
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # abmatrix
 
 [![Upload Python Package](https://github.com/wisdomhealth-inc/abmatrix/actions/workflows/python-publish.yml/badge.svg)](https://github.com/wisdomhealth-inc/abmatrix/actions/workflows/python-publish.yml)
 
 Python3 module defining a class called `abmatrix` to read and parse AB Matrix files
 
 ## Module contents
@@ -14,23 +25,24 @@
 
 abmatrix.abmatrix.**read**(abmatrixfile)
 
 Read an AB Matrix file, read header and lazy load genotype data
 
 ---
 
-abmatrix.abmatrix.**write**(abmatrixfile)
+abmatrix.abmatrix.**write**(abmatrixfile, genotypes)
 
 Write an AB Matrix file from in-memory instance of class
 
 ---
 
-abmatrix.abmatrix.**subset**(locus_list, sample_list)
+abmatrix.abmatrix.**subset**(locus_list, samples=sample_list)
 
-Get subset of AB Matrix data set
+Get subset of AB Matrix data set. Returns genotype matrix as list
+of dictionaries.
 
 ---
 
 abmatrix.abmatrix.**close**()
 
 Close instance of abmatrix data set
 
@@ -39,23 +51,23 @@
 ## Example
 ```python
 from abmatrix import abmatrix
 
 # Initialize
 myabmatrix = abmatrix.abmatrix()
 
-myabmatrix.open("test_abmatrix.zip")
+myabmatrix.read("test_abmatrix.zip")
 
-TRAIT_LIST = [
+SNP_IDS = [
     "442_HPS3",
     "054_FGF4_chr12",
     "077_TYRP_LH",
     "077_TYRP1_SH",
     "441_USH2A_roan",
     "277_MC1R_cockersable_Eh",
 ]
 
-output = myabmatrix.reduce(TRAIT_LIST)
-print(output)
+genotypes = myabmatrix.subset(SNP_IDS)
+myabmatrix.write("test_abmatrix_subset.ab", genotypes)
 
 myabmatrix.close()
 ```
```

### Comparing `abmatrix-0.3.0/abmatrix/abmatrix.py` & `abmatrix-0.3.1/abmatrix/abmatrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,28 +58,39 @@
                 else:
                     locus_id = line.rstrip("\n").split("\t")[0]
                     self.index[locus_id] = offset
                 offset += len(line)
         else:
             raise FileNotFoundError
 
-    def write(self, filename, locus_list):
+    def write(self, filename, genotypes):
+        # Update header metadata
+        new_sample_list = []
+        for key in genotypes[0].keys():
+            if key != "id":
+                new_sample_list.append(key)
+        new_sample_size = len(new_sample_list)
+        new_locus_size = len(genotypes)
+        new_header = self.header
+        new_header["Num Samples"] = new_sample_size
+        new_header["Total Samples"] = new_sample_size
+        new_header["Num SNPs"] = new_locus_size
+        new_header["Total SNPs"] = new_locus_size
+
         with open(filename, "w") as f:
             f.write("[Header]\n")
-            for key, value in self.header.items():
+            for key, value in new_header.items():
                 f.write("{}\t{}\n".format(key, value))
             f.write("[Data]\n")
-            sorted_samples = sorted(self.sample_index.items(), key=lambda x:x[1])
-            for id in sorted_samples:
-                f.write("\t{}".format(id[0]))
-            f.write("\n")
-            for locus in locus_list:
+            sample_header = "\t".join(new_sample_list)
+            f.write("\t{}\n".format(sample_header))
+            for locus in genotypes:
                 f.write(locus["id"])
-                for id in sorted_samples:
-                    f.write("\t{}".format(locus[id[0]]))
+                for sample in new_sample_list:
+                    f.write("\t{}".format(locus[sample]))
                 f.write("\n")
 
     def subset(self, locus_list, **kwargs):
         output_list = []
         if "samples" in kwargs:
             sample_list = kwargs["samples"]
         else:
```

