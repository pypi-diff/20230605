# Comparing `tmp/scutls-0.2.0.tar.gz` & `tmp/scutls-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.2.0.tar", max compression
+gzip compressed data, was "scutls-0.2.1.tar", max compression
```

## Comparing `scutls-0.2.0.tar` & `scutls-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      583 2023-05-11 17:04:40.763821 scutls-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-11 17:04:56.253239 scutls-0.2.0/scutls/__init__.py
--rw-r--r--   0        0        0     6256 2023-05-10 15:48:41.694697 scutls-0.2.0/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.0/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.0/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.0/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.0/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     4939 2023-05-10 22:02:20.277174 scutls-0.2.0/scutls/barcode.py
--rw-r--r--   0        0        0     1074 2023-05-10 15:45:19.722039 scutls-0.2.0/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.0/scutls/download.py
--rw-r--r--   0        0        0     3603 2023-05-08 14:34:45.400997 scutls-0.2.0/scutls/fastq.py
--rw-r--r--   0        0        0     9127 2023-05-10 22:03:04.285591 scutls-0.2.0/scutls/util.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.0/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-06-05 20:05:32.972181 scutls-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-05 20:05:52.115138 scutls-0.2.1/scutls/__init__.py
+-rw-r--r--   0        0        0     6256 2023-05-10 15:48:41.694697 scutls-0.2.1/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.1/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.1/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.1/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.1/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     4938 2023-06-02 19:36:09.942327 scutls-0.2.1/scutls/barcode.py
+-rw-r--r--   0        0        0     1074 2023-05-10 15:45:19.722039 scutls-0.2.1/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.1/scutls/download.py
+-rw-r--r--   0        0        0     3845 2023-06-02 19:44:04.605614 scutls-0.2.1/scutls/fastq.py
+-rw-r--r--   0        0        0     9201 2023-06-05 20:04:42.981372 scutls-0.2.1/scutls/util.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.1/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.1/PKG-INFO
```

### Comparing `scutls-0.2.0/pyproject.toml` & `scutls-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scutls"
-version = "0.2.0"
+version = "0.2.1"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
```

### Comparing `scutls-0.2.0/scutls/arguments.py` & `scutls-0.2.1/scutls/arguments.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.0/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.2.1/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.0/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.2.1/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.2.0/scutls/assets/genome_ucsc.json` & `scutls-0.2.1/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.0/scutls/barcode.py` & `scutls-0.2.1/scutls/barcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def barcode(input = None, output = None, output2 = None, contain = None, locate = None, pos = 0, error = 1, rc_barcode = False, nproc = 1):
     """barcode subcommand
     Paramters
     ---------
 
     input : str
-        output file name, auto detects .gz
+        input file name, auto detects .gz
     output : str
         output file name, auto detects .gz, contains fastq that contains specified barcode via contain
     contain: str
         barcode to detect, if multiple barcode, separate with comma: "AATTCCC,AGGGCCC,CCGGCG"
         # optional for "contain" sub-command:
         error: int
             allowed nucleotide mismatches (can be INDELs) when aligning, default to 1
```

### Comparing `scutls-0.2.0/scutls/cli.py` & `scutls-0.2.1/scutls/cli.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.0/scutls/download.py` & `scutls-0.2.1/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.0/scutls/fastq.py` & `scutls-0.2.1/scutls/fastq.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import argparse
 from Bio import SeqIO, bgzf
 from Bio.Seq import Seq
 from .util import _open
 import os
 
-def fastq(input = None, output = None, unique = None, join = None):
+def fastq(input = None, output = None, unique = None, join = None, rc = None, nproc = 1):
     """fastq subcommand
     Paramters
     ---------
 
     input : str
-        output file name, auto detects .gz
+        input file name, auto detects .gz
     output : str
         output file name, auto detects .gz
     unique : str
         output unique fastq records by record ID
     join : str
         fastq file name to join to the input fastq, auto detects .gz
             "join" means to append each read to corresponding lines in input, not "cat"
+    nproc: int
+        number of parallel jobs, default to 1
+        funtions that support nproc: rc
+
+    # TODO:
+    rc : str
+        boolean, to reverse complement the reads, supports multi-processing
 
     """
 
     args = list(locals().keys())
 
     local = locals()
     if all(bool(local[key]) is not True for key in args): # use True since args can be either None or False
@@ -44,15 +51,14 @@
                     SeqIO.write(sequences = unique_records.values(), handle = outgz, format="fastq")
             else:
                 SeqIO.write(unique_records.values(), output, "fastq")
 
         print("Done!")
 
     # join fastq file to input fastq if "-j":
-        # make fastq file unique:
     if join:
         print("Saving to " + output + " ...")
 
         if not os.path.dirname(output) == "":
             os.makedirs(os.path.dirname(output), exist_ok=True)
 
         f_input = _open(input)
@@ -83,14 +89,16 @@
             f_out.write(record_quality + record_j_quality + "\n")
 
         f_input.close()
         f_join.close()
         f_out.close()
         print("Done!")
 
+    # reverse complement fastq if "-rc":
+    # todo
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--input',  '-i', type   = str)
     parser.add_argument('--output', '-o', type   = str)
     parser.add_argument('--unique', '-u', action = 'store_true')
     parser.add_argument('--join',   '-j', type   = str)
```

### Comparing `scutls-0.2.0/scutls/util.py` & `scutls-0.2.1/scutls/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,17 @@
     if not "," in pattern:
         if rc_barcode:
             pattern = str(Seq(pattern).reverse_complement())
         barcode_pattern = "(" + pattern + "){e<=" + str(error) + "}"
     else:
         barcode_pattern = ""
         barcodes = pattern.split(",")
+        if rc_barcode:
+            barcodes = barcodes[::-1]
+            
         for barcode in barcodes:
             if rc_barcode:
                 pattern = str(Seq(pattern).reverse_complement())
             barcode_pattern += "(" + barcode + "){e<=" + str(error) + "}(.*?)"
     return(barcode_pattern)
 
 # obtain fastq coordinates for specified barcode
```

### Comparing `scutls-0.2.0/setup.py` & `scutls-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.2.0/PKG-INFO` & `scutls-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.2.0
+Version: 0.2.1
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

