# Comparing `tmp/loreme-0.1.0.tar.gz` & `tmp/loreme-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loreme-0.1.0.tar", last modified: Mon Jun  5 16:42:52 2023, max compression
+gzip compressed data, was "loreme-0.1.1.tar", last modified: Mon Jun  5 20:22:19 2023, max compression
```

## Comparing `loreme-0.1.0.tar` & `loreme-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 16:42:52.759858 loreme-0.1.0/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-05 04:30:20.000000 loreme-0.1.0/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1780 2023-06-05 16:42:52.759126 loreme-0.1.0/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1265 2023-06-05 04:30:20.000000 loreme-0.1.0/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 16:42:52.737167 loreme-0.1.0/loreme.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1780 2023-06-05 16:42:52.000000 loreme-0.1.0/loreme.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      717 2023-06-05 16:42:52.000000 loreme-0.1.0/loreme.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-05 16:42:52.000000 loreme-0.1.0/loreme.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-05 16:42:52.000000 loreme-0.1.0/loreme.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-05 16:42:52.000000 loreme-0.1.0/loreme.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-05 16:42:52.000000 loreme-0.1.0/loreme.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-05 04:30:20.000000 loreme-0.1.0/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-05 16:42:52.760073 loreme-0.1.0/setup.cfg
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 16:42:52.733135 loreme-0.1.0/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 16:42:52.757514 loreme-0.1.0/src/loreme/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      847 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/check_gpu_availability.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3098 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/dorado.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4872 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2553 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/export_bedgraph.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/gene_body_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/intersect.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    33392 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/loreme.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5191 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/mean.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/merge.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/methylation_hist.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/parse_gff.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2610 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/pbcpg.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6487 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/plot.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2440 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/plot_bedtools.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/plot_genes.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/plot_repeats.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/promoter_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-05 04:30:20.000000 loreme-0.1.0/src/loreme/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 20:22:19.211691 loreme-0.1.1/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-05 04:30:20.000000 loreme-0.1.1/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2882 2023-06-05 20:22:19.209466 loreme-0.1.1/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2367 2023-06-05 20:21:59.000000 loreme-0.1.1/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 20:22:19.161918 loreme-0.1.1/loreme.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2882 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      717 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-05 20:22:19.000000 loreme-0.1.1/loreme.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-05 19:39:48.000000 loreme-0.1.1/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-05 20:22:19.212123 loreme-0.1.1/setup.cfg
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 20:22:19.153668 loreme-0.1.1/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-05 20:22:19.208506 loreme-0.1.1/src/loreme/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1512 2023-06-05 20:07:53.000000 loreme-0.1.1/src/loreme/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/check_gpu_availability.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3098 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/dorado.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4872 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2553 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/export_bedgraph.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/gene_body_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/intersect.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    33140 2023-06-05 19:18:15.000000 loreme-0.1.1/src/loreme/loreme.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5191 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/mean.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/merge.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/methylation_hist.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/parse_gff.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2610 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/pbcpg.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6487 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/plot.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2440 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/plot_bedtools.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/plot_genes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/plot_repeats.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/promoter_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-05 04:30:20.000000 loreme-0.1.1/src/loreme/version.py
```

### Comparing `loreme-0.1.0/LICENSE` & `loreme-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/PKG-INFO` & `loreme-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-Metadata-Version: 2.1
-Name: loreme
-Version: 0.1.0
-Summary: Extract Methylation calls from ONT or PB long read data
-Author-email: Anthony Aylward <aaylward@salk.edu>
-Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
-Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # LoReMe pipeline
 
 TODO: make a 'loreme clean' subcommand to remove downloads before uninstalling
 
-Analysis of CpG methylation calls from PacBio HiFi or ONT data. See also the [full documentation](https://salk-tm.gitlab.io/loreme/index.html)
+LoReMe (Long Read Methylaton) is a Python package facilitating analysis of
+DNA methylation signals from [Pacific Biosciences](https://www.pacb.com/technology/hifi-sequencing/)
+or [Oxford Nanopore](https://nanoporetech.com/applications/dna-nanopore-sequencing)
+long read sequencing data.
+
+It consists of an API and CLI for three distinct applications:
+
+1. Pacific Biosciences data processing. PB reads in SAM/BAM format are aligned
+to a reference genome with the special-purpose aligner [pbmm2](https://github.com/PacificBiosciences/pbmm2>),
+a modified version of [minimap2](https://lh3.github.io/minimap2/).
+Methylation calls are then extracted from the aligned reads by [pb-CpG-tools](https://github.com/PacificBiosciences/pb-CpG-tools).
+
+2. Oxford nanopore basecalling. ONT reads are optionally converted from FAST5
+to [POD5](https://github.com/nanoporetech/pod5-file-format) format, then
+basecalled and aligned to a reference with [dorado](https://github.com/nanoporetech/dorado>).
+(dorado alignment also uses minimap2 under the hood).
+
+3. Postprocessing and QC of methylation calls. Several functions are available
+to generate diagnostic statistics and plots.
+
+See also the [full documentation](https://salk-tm.gitlab.io/loreme/index.html).
 
 Other tools of interest: [methylartist](https://github.com/adamewing/methylartist) and [modbamtools](https://github.com/rrazaghi/modbamtools)  ([modbamtools docs](https://rrazaghi.github.io/modbamtools/)), [methplotlib](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7214038/)
 
 ## Installation
 
 ### Conda
```

### Comparing `loreme-0.1.0/loreme.egg-info/SOURCES.txt` & `loreme-0.1.1/loreme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/pyproject.toml` & `loreme-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loreme"
-version = "0.1.0" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.1.1" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
     { name="Anthony Aylward", email="aaylward@salk.edu" },
 ]
 description = "Extract Methylation calls from ONT or PB long read data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `loreme-0.1.0/src/loreme/check_gpu_availability.py` & `loreme-0.1.1/src/loreme/check_gpu_availability.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/dorado.py` & `loreme-0.1.1/src/loreme/dorado.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/download.py` & `loreme-0.1.1/src/loreme/download.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/env.py` & `loreme-0.1.1/src/loreme/env.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/export_bedgraph.py` & `loreme-0.1.1/src/loreme/export_bedgraph.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/gene_body_methylation.py` & `loreme-0.1.1/src/loreme/gene_body_methylation.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/intersect.py` & `loreme-0.1.1/src/loreme/intersect.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/loreme.py` & `loreme-0.1.1/src/loreme/loreme.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,26 +232,18 @@
 
 def _export_bedgraph(args):
     export_bedgraph(args.bedmethyl, chromosomes=args.chromosomes,
                     coverage=args.coverage)
 
 
 def parse_arguments():
-    """
-    Get arguments from command line with argparse.
-    """
     parser = argparse.ArgumentParser(
-        description="""Analysis of DNA methylation data from PB or ONT long reads.
-
-PB reads are aligned with `pbmm2 <https://github.com/PacificBiosciences/pbmm2>`_
-and postprocessed by `pb-CpG-tools <https://github.com/PacificBiosciences/pb-CpG-tools>`_ .
-
-ONT reads are optionally converted to `POD5 <https://github.com/nanoporetech/pod5-file-format>`_
-format and basecalled with `dorado <https://github.com/nanoporetech/dorado>`_ .
-""")
+        description="""Analysis of DNA methylation signals from `Pacific Biosciences <https://www.pacb.com/technology/hifi-sequencing/>`_
+or `Oxford Nanopore <https://nanoporetech.com/applications/dna-nanopore-sequencing>`_
+long read sequencing data.""")
     parser.add_argument('--version', action='version',
                     version='%(prog)s {version}'.format(version=__version__))
     subparsers = parser.add_subparsers()
 
     parser_download_pbcpg = subparsers.add_parser('download-pbcpg',
                                                   help='download pb-CpG-tools')
     parser_download_pbcpg.set_defaults(func=_download_pbcpg)
```

### Comparing `loreme-0.1.0/src/loreme/mean.py` & `loreme-0.1.1/src/loreme/mean.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/merge.py` & `loreme-0.1.1/src/loreme/merge.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/methylation_hist.py` & `loreme-0.1.1/src/loreme/methylation_hist.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/parse_gff.py` & `loreme-0.1.1/src/loreme/parse_gff.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/pbcpg.py` & `loreme-0.1.1/src/loreme/pbcpg.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/plot.py` & `loreme-0.1.1/src/loreme/plot.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/plot_bedtools.py` & `loreme-0.1.1/src/loreme/plot_bedtools.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/plot_genes.py` & `loreme-0.1.1/src/loreme/plot_genes.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/plot_repeats.py` & `loreme-0.1.1/src/loreme/plot_repeats.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.0/src/loreme/promoter_methylation.py` & `loreme-0.1.1/src/loreme/promoter_methylation.py`

 * *Files identical despite different names*

