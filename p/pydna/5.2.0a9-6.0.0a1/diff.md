# Comparing `tmp/pydna-5.2.0a9.tar.gz` & `tmp/pydna-6.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydna-5.2.0a9.tar", max compression
+gzip compressed data, was "pydna-6.0.0a1.tar", max compression
```

## Comparing `pydna-5.2.0a9.tar` & `pydna-6.0.0a1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rwxr-xr-x   0        0        0     6255 2022-11-30 15:25:25.861757 pydna-5.2.0a9/LICENSE.txt
--rwxr-xr-x   0        0        0    15208 2023-01-31 17:06:46.726455 pydna-5.2.0a9/README.md
--rw-r--r--   0        0        0     2236 2023-02-01 06:41:48.902261 pydna-5.2.0a9/pyproject.toml
--rw-r--r--   0        0        0    13198 2023-02-01 06:41:48.906261 pydna-5.2.0a9/src/pydna/__init__.py
--rw-r--r--   0        0        0     1101 2023-01-28 15:12:11.214007 pydna-5.2.0a9/src/pydna/_pretty.py
--rw-r--r--   0        0        0    10903 2023-01-28 15:12:11.214007 pydna-5.2.0a9/src/pydna/_thermodynamic_data.py
--rw-r--r--   0        0        0     2099 2023-01-28 15:12:11.214007 pydna-5.2.0a9/src/pydna/all.py
--rwxr-xr-x   0        0        0     5644 2023-01-28 15:12:11.214007 pydna-5.2.0a9/src/pydna/amplicon.py
--rw-r--r--   0        0        0    19254 2023-01-28 15:12:11.214007 pydna-5.2.0a9/src/pydna/amplify.py
--rw-r--r--   0        0        0    19479 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/assembly.py
--rw-r--r--   0        0        0     3491 2023-01-28 10:48:48.707481 pydna-5.2.0a9/src/pydna/codon.py
--rw-r--r--   0        0        0    10562 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/common_sub_strings.py
--rwxr-xr-x   0        0        0      971 2023-01-28 10:48:48.707481 pydna-5.2.0a9/src/pydna/conftest.py
--rw-r--r--   0        0        0     8357 2023-01-28 10:48:48.707481 pydna-5.2.0a9/src/pydna/contig.py
--rwxr-xr-x   0        0        0    26343 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/design.py
--rw-r--r--   0        0        0     1315 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/download.py
--rw-r--r--   0        0        0    43477 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/dseq.py
--rw-r--r--   0        0        0    46162 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/dseqrecord.py
--rw-r--r--   0        0        0     3471 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/editor.py
--rwxr-xr-x   0        0        0     1394 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/fakeseq.py
--rw-r--r--   0        0        0     8682 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/gateway.py
--rwxr-xr-x   0        0        0     3673 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/gel.py
--rw-r--r--   0        0        0     9008 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/genbank.py
--rw-r--r--   0        0        0     1766 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/genbankfile.py
--rw-r--r--   0        0        0    20867 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/genbankfixer.py
--rw-r--r--   0        0        0     5741 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/genbankrecord.py
--rw-r--r--   0        0        0     1744 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/goldengate.py
--rw-r--r--   0        0        0     2936 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/gui.py
--rwxr-xr-x   0        0        0     3404 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/ladders.py
--rw-r--r--   0        0        0     1822 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/myenzymes.py
--rw-r--r--   0        0        0     7261 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/myprimers.py
--rw-r--r--   0        0        0     5175 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/parsers.py
--rw-r--r--   0        0        0     2635 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/primer.py
--rw-r--r--   0        0        0     1710 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/readers.py
--rw-r--r--   0        0        0     4292 2023-01-28 10:48:48.715481 pydna-5.2.0a9/src/pydna/seq.py
--rwxr-xr-x   0        0        0    22964 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/seqrecord.py
--rw-r--r--   0        0        0     1955 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/sequence_picker.py
--rw-r--r--   0        0        0     9752 2023-01-28 15:12:11.218007 pydna-5.2.0a9/src/pydna/tm.py
--rw-r--r--   0        0        0    23402 2023-01-28 15:12:11.222007 pydna-5.2.0a9/src/pydna/utils.py
--rw-r--r--   0        0        0    16690 1970-01-01 00:00:00.000000 pydna-5.2.0a9/setup.py
--rw-r--r--   0        0        0    16490 1970-01-01 00:00:00.000000 pydna-5.2.0a9/PKG-INFO
+-rwxr-xr-x   0        0        0     6255 2023-06-05 10:13:56.394878 pydna-6.0.0a1/LICENSE.txt
+-rwxr-xr-x   0        0        0    13820 2023-06-05 10:13:56.394878 pydna-6.0.0a1/README.md
+-rw-r--r--   0        0        0     2937 2023-06-05 10:14:33.755828 pydna-6.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0    12827 2023-06-05 10:14:33.755828 pydna-6.0.0a1/src/pydna/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/_pretty.py
+-rw-r--r--   0        0        0    10903 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/_thermodynamic_data.py
+-rw-r--r--   0        0        0     2099 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/all.py
+-rwxr-xr-x   0        0        0     5732 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/amplicon.py
+-rw-r--r--   0        0        0    18635 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/amplify.py
+-rw-r--r--   0        0        0    19159 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/assembly.py
+-rw-r--r--   0        0        0     2053 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/biosubclasses.py
+-rw-r--r--   0        0        0     2408 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/codon.py
+-rw-r--r--   0        0        0    11157 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/common_sub_strings.py
+-rwxr-xr-x   0        0        0      975 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/conftest.py
+-rw-r--r--   0        0        0     7967 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/contig.py
+-rwxr-xr-x   0        0        0    26230 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/design.py
+-rw-r--r--   0        0        0     1315 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/download.py
+-rw-r--r--   0        0        0    42601 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/dseq.py
+-rw-r--r--   0        0        0    45167 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/dseqrecord.py
+-rw-r--r--   0        0        0     3471 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/editor.py
+-rwxr-xr-x   0        0        0     1343 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/fakeseq.py
+-rw-r--r--   0        0        0     8425 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/gateway.py
+-rwxr-xr-x   0        0        0     3537 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/gel.py
+-rw-r--r--   0        0        0     8809 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/genbank.py
+-rw-r--r--   0        0        0     1704 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/genbankfile.py
+-rw-r--r--   0        0        0    20690 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/genbankfixer.py
+-rw-r--r--   0        0        0     5714 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/genbankrecord.py
+-rw-r--r--   0        0        0     1747 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/goldengate.py
+-rw-r--r--   0        0        0     2958 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/gui.py
+-rwxr-xr-x   0        0        0     3574 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/ladders.py
+-rw-r--r--   0        0        0     1802 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/myenzymes.py
+-rw-r--r--   0        0        0     7164 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/myprimers.py
+-rw-r--r--   0        0        0     7997 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/parsers.py
+-rw-r--r--   0        0        0     2533 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/primer.py
+-rw-r--r--   0        0        0     1710 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/readers.py
+-rw-r--r--   0        0        0     4123 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/seq.py
+-rwxr-xr-x   0        0        0    21956 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/seqrecord.py
+-rw-r--r--   0        0        0     1642 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/sequence_picker.py
+-rw-r--r--   0        0        0     2629 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/threading_timer_decorator_exit.py
+-rw-r--r--   0        0        0     9753 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/tm.py
+-rw-r--r--   0        0        0    23408 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/utils.py
+-rw-r--r--   0        0        0    15140 1970-01-01 00:00:00.000000 pydna-6.0.0a1/PKG-INFO
```

### Comparing `pydna-5.2.0a9/LICENSE.txt` & `pydna-6.0.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydna-5.2.0a9/README.md` & `pydna-6.0.0a1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,139 +1,68 @@
 # ![icon](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/pydna.resized.png) pydna
 
-| [![Tests & Coverage](https://github.com/BjornFJohansson/pydna/workflows/Tests%20&%20Coverage/badge.svg)](https://github.com/BjornFJohansson/pydna/actions?query=workflow%3A%22Tests+%26+Coverage%22)                |[![codecov](https://codecov.io/gh/BjornFJohansson/pydna/branch/master/graph/badge.svg)](https://codecov.io/gh/BjornFJohansson/pydna/branch/master)    | [![PyPI version](https://badge.fury.io/py/pydna.svg)](https://badge.fury.io/py/pydna)                                                   |[![Anaconda-Server Badge](https://anaconda.org/bjornfjohansson/pydna/badges/version.svg)](https://anaconda.org/bjornfjohansson/pydna)   | [![Google group : pydna](https://img.shields.io/badge/Google%20Group-pydna-blue.svg)](https://groups.google.com/g/pydna)        |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)                                                                                  |[![GitHub issues](https://img.shields.io/github/issues/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/issues)                   | [![Anaconda-Server Badge2](https://anaconda.org/bjornfjohansson/pydna/badges/license.svg)](https://anaconda.org/bjornfjohansson/pydna)  |[![GitHub stars](https://img.shields.io/github/stars/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/stargazers)   |                                                                                                                                 |
+| [![Tests & Coverage](https://github.com/BjornFJohansson/pydna/actions/workflows/pydna_test_and_coverage_workflow.yml/badge.svg?branch=dev_bjorn)](https://github.com/BjornFJohansson/pydna/actions/workflows/pydna_test_and_coverage_workflow.yml) | [![codecov](https://codecov.io/gh/BjornFJohansson/pydna/branch/master/graph/badge.svg)](https://codecov.io/gh/BjornFJohansson/pydna/branch/master) | [![PyPI version](https://badge.fury.io/py/pydna.svg)](https://badge.fury.io/py/pydna)    | [![Google group : pydna](https://img.shields.io/badge/Google%20Group-pydna-blue.svg)](https://groups.google.com/g/pydna)              |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
+| [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)                                                                   | [![GitHub issues](https://img.shields.io/github/issues/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/issues)                | [![Anaconda-Server Badge2](https://anaconda.org/bjornfjohansson/pydna/badges/license.svg)](https://anaconda.org/bjornfjohansson/pydna) | [![GitHub stars](https://img.shields.io/github/stars/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/stargazers) |
+
 
 
 Planning genetic constructs with many parts and assembly steps, such as recombinant
-metabolic pathways :petri_dish:, are often difficult to **properly** document as is evident from the
-state of such documentation in the scientific literature :radioactive:.
+metabolic pathways :petri_dish:, are often difficult to **properly** document as is evident from the poor
+state of documentation in the scientific literature :radioactive:.
 
 
 The pydna python package provide a human-readable formal descriptions of :dna: cloning and genetic assembly
-strategies in Python :snake: which allow for simulation and verification.
-
-
-Pydna can perhaps be thought of as [executable documentation](https://en.wikipedia.org/wiki/Literate_programming) for cloning.
+strategies in Python :snake: which allow for simulation and verification. Pydna can be used as [executable documentation](https://en.wikipedia.org/wiki/Literate_programming) for cloning.
 
 
 A cloning strategy expressed in pydna is **complete**, **unambiguous** and **stable**.
 
 
 Pydna provides simulation of:
 
+- Primer design
+- PCR
 - Restriction digestion
 - Ligation
-- PCR
-- Primer design
+- Gel electrophoresis of DNA with generation of gel images
+- Homologous recombination
 - Gibson assembly
 - Golden gate assembly
-- Homologous recombination
-- Gel electrophoresis of DNA with generation of gel images
+
 
 Virtually any sub-cloning experiment can be described in pydna, and its execution yield
 the sequences of intermediate and final DNA molecules.
 
-Pydna has been designed to be understandable for biologists with only some basic understanding of Python.
+Pydna has been designed with the goal of being understandable for biologists with only some basic understanding of Python.
 
 Pydna can formalize planning and sharing of cloning strategies and is especially useful for complex or combinatorial
 DNA molecule constructions.
 
-
-To get started, we have compiled some [simple examples](https://github.com/MetabolicEngineeringGroupCBMA/pydna-examples#pydna-examples).
+To get started, I have compiled some [simple examples](https://github.com/MetabolicEngineeringGroupCBMA/pydna-examples#pydna-examples).
 For more elaborate use, look at some assembly strategies of D-xylose metabolic pathways [MetabolicEngineeringGroupCBMA/ypk-xylose-pathways](https://github.com/MetabolicEngineeringGroupCBMA/ypk-xylose-pathways#pereira-et-al-2016).
 
 
-There is an open access paper in BMC Bioinformatics describing pydna:
-
-[![abstr](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/BMC_resized.png)](http://www.biomedcentral.com/1471-2105/16/142/abstract)
-
-Please reference the above paper:
-
-
-Pereira, F., Azevedo, F., Carvalho, Â., Ribeiro, G. F., Budde, M. W., & Johansson, B. (2015). Pydna: a simulation and documentation tool for DNA assembly strategies using python. BMC Bioinformatics, 16(142), 142.
-
 
-if using pydna in a scientific publication.
 
 
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
 
 
 ## Usage
 
 Most pydna functionality is implemented as methods for the double stranded DNA sequence record
 classes Dseq and Dseqrecord, which are subclasses of the [Biopython](http://biopython.org/wiki/Main_Page) [Seq](http://biopython.org/wiki/Seq) and [SeqRecord](http://biopython.org/wiki/SeqRecord) classes.
 
-These classes make cut and paste cloning and PCR very simple:
-
-
-    >>> from pydna.dseq import Dseq
-    >>> seq = Dseq("GGATCCAAA","TTTGGATCC",ovhg=0)
-    >>> seq
-    Dseq(-9)
-    GGATCCAAA
-    CCTAGGTTT
-    >>> from Bio.Restriction import BamHI
-    >>> a,b = seq.cut(BamHI)
-    >>> a
-    Dseq(-5)
-    G
-    CCTAG
-    >>> b
-    Dseq(-8)
-    GATCCAAA
-        GTTT
-    >>> a+b
-    Dseq(-9)
-    GGATCCAAA
-    CCTAGGTTT
-    >>> b+a
-    Dseq(-13)
-    GATCCAAAG
-        GTTTCCTAG
-    >>> b+a+b
-    Dseq(-17)
-    GATCCAAAGGATCCAAA
-        GTTTCCTAGGTTT
-    >>> b+a+a
-    Traceback (most recent call last):
-      File "<stdin>", line 1, in <module>
-      File "/usr/local/lib/python2.7/dist-packages/pydna/dsdna.py", line 217, in __add__
-        raise TypeError("sticky ends not compatible!")
-    TypeError: sticky ends not compatible!
-    >>>
-
-As the example above shows, pydna keeps track of sticky ends.
-
-Notably, homologous recombination and Gibson assembly between linear DNA fragments
-can be easily simulated without any additional information besides the primary sequence of the fragments.
-
-Gel electrophoresis of DNA fragments can be simulated using the included gel module
-
-
-    Jupyter QtConsole 4.7.7
-    Python 3.8.5 | packaged by conda-forge | (default, Aug 29 2020, 01:22:49)
-    Type 'copyright', 'credits' or 'license' for more information
-    IPython 7.18.1 -- An enhanced Interactive Python. Type '?' for help.
-
-    In [1]: from pydna.gel import gel
-
-    In [2]: from pydna.ladders import PennStateLadder
-
-    In [3]: from pydna.dseqrecord import Dseqrecord
+These classes make PCR primer design, PCR simulation and cut-and-paste cloning very simple:
 
-    In [4]: gel([PennStateLadder,[Dseqrecord("A"*2000)]])
-    Out[4]:
+[![example](https://raw.githubusercontent.com/BjornFJohansson/pydna/master/docs/example.png)](https://github.com/BjornFJohansson/pydna/blob/master/docs/example.ipynb)
 
-
-
-![](https://raw.githubusercontent.com/BjornFJohansson/pydna/master/scripts/pydna_gel.png)
+As the example above shows, pydna keeps track of sticky ends and features.
 
 
 Pydna can be very compact. The eleven lines of Python below simulates the construction of a recombinant plasmid.
 DNA sequences are downloaded from Genbank by accession numbers that are guaranteed to be stable over time.
 
     from pydna.genbank import Genbank
     gb = Genbank("myself@email.com") # Tell Genbank who you are!
@@ -153,20 +82,17 @@
 
 Pydna can automate the simulation of [sub cloning](http://en.wikipedia.org/wiki/Subcloning) experiments using
 python. This is helpful to generate examples for teaching purposes.
 
 Read the documentation (below) or the [cookbook](https://github.com/BjornFJohansson/pydna/blob/master/docs/cookbook/cookbook.ipynb) with example files
 for further information.
 
-Please post a message in the [google group](https://groups.google.com/d/forum/pydna)
-for pydna if you need help or have problems, questions or comments :sos:.
-
-Feedback & suggestions are very welcome!
+Feedback & suggestions are very welcome! Please post a message in the [google group](https://groups.google.com/d/forum/pydna) for pydna if you need help or have problems, questions or comments :sos:.
 
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
 
 ## Who is using pydna?
 
 Taylor, L. J., & Strebel, K. (2017).
 Pyviko: an automated Python tool to design gene knockouts in complex viruses with overlapping genes.
 BMC Microbiology, 17(1), 12.
@@ -180,157 +106,169 @@
 
 
 [An Automated Protein Synthesis Pipeline with Transcriptic and Snakemake](http://blog.booleanbiotech.com/transcriptic_protein_synthesis_pipeline.html)
 
 
 and other projects on [github](https://github.com/BjornFJohansson/pydna/network/dependents?package_id=UGFja2FnZS01MjQ2MjYzNQ%3D%3D)
 
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+There is an open access paper in BMC Bioinformatics describing pydna:
+
+[![abstr](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/BMC_resized.png)](http://www.biomedcentral.com/1471-2105/16/142/abstract)
+
+Please reference the above paper:
+
+
+Pereira, F., Azevedo, F., Carvalho, Â., Ribeiro, G. F., Budde, M. W., & Johansson, B. (2015). Pydna: a simulation and documentation tool for DNA assembly strategies using python. BMC Bioinformatics, 16(142), 142.
 
 
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+When using pydna.
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
 ## Documentation
 
 Documentation is built using [Sphinx](http://www.sphinx-doc.org/) from [docstrings](https://www.python.org/dev/peps/pep-0257/)
 in the code and displayed at readthedocs [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)
 
 The [numpy](www.numpy.org) [docstring format](https://github.com/numpy/numpy/blob/release/doc/HOWTO_DOCUMENT.rst.txt) is used.
 
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
 ## Installation using pip
 
 Pip is included in recent Python versions and is the
 officially [recommended](http://python-packaging-user-guide.readthedocs.org/en/latest) tool.
 
 Pip installs the minimal installation requirements automatically, but not the optional requirements (see below).
 
     pip install pydna
 
 or use the --pre switch to get the latest version of pydna.
 
     pip install pydna --pre
 
+for optional functionality do:
+
+    pip install pydna[gel,download,express,gui]
+
+Remove options inside the square brackets as required, but be sure not to leave spaces as pip will not recognize the options. See below under "Optional dependencies".
+
 ### Windows:
 
 You should be able to pip install pydna from the Windows terminal as biopython now can be installed with pip as well.
 
     C:\> pip install pydna
 
-By default python and pip are not on the PATH. You can re-install Python and select this option during installation,
-or give the full path for pip. Try something like this, depending on where your copy of Python is installed:
+By default python and pip are not on the PATH. You can re-install Python and select this option during installation, or give the full path for pip. Try something like this, depending on where your copy of Python is installed:
 
     C:\Python37\Scripts\pip install pydna
 
-### Installing requirements
-
-If you want to install requirements before installing pydna, you can do:
-
-	pip install -r requirements.txt
-
-And for the optional requirements:
-
-	pip install -r requirements_optional.txt
-
-For testing:
-
-	pip install -r requirements_test.txt
-
-or
-
-	conda install --file requirements.txt
-
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
 ## Source Code
 
 Pydna is developed on [Github](https://github.com/BjornFJohansson/pydna) :octocat:.
 
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
 ## Minimal installation dependencies
 
 Pydna versions before 1.0.0 were compatible with python 2.7 only.
 The list below is the minimal requirements for installing pydna.
 Biopython has c-extensions, but the other modules are pure python.
 
 - [Python 3.8, 3.9, 3.10 or 3.11](http://www.python.org)
-- [appdirs >= 1.3.0](https://pypi.python.org/pypi/appdirs)
+- [appdirs >=1.4.4](https://pypi.python.org/pypi/appdirs)
 - [biopython >= 1.80](http://pypi.python.org/pypi/biopython)
-- [networkx >= 1.8.1](http://pypi.python.org/pypi/networkx)
-- [prettytable >= 0.7.2](https://pypi.python.org/pypi/PrettyTable)
+- [networkx >=2.8.8](http://pypi.python.org/pypi/networkx)
+- [prettytable >=3.5.0](https://pypi.python.org/pypi/PrettyTable)
+- [pyperclip >=1.8.2](https://pypi.python.org/pypi/PrettyTable)
+- [pyfiglet >=0.8.post1](https://pypi.python.org/pypi/PrettyTable)
 
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
 ## Optional dependencies
 
-If the modules listed below in the first column are installed, they will provide the functionality
-listed in the second column.
+If the modules listed below in the first column are installed, they will provide the functionality listed in the second column.
 
-| Dependency                                          | Function in pydna                                      |
-|-----------------------------------------------------|--------------------------------------------------------|
-| [pyparsing](https://pypi.python.org/pypi/pyparsing) | fix corrupt Genbank files with pydna.genbankfixer      |
-| [requests](https://pypi.org/project/requests)       | download sequences with pydna.download                 |
-| [CAI](https://pypi.org/project/CAI)                 | codon adaptation index calculations in several modules |
-| [numpy](http://www.numpy.org)                       | gel simulation with pydna.gel                          |
-| [scipy](https://www.scipy.org)                      | “                                                      |
-| [matplotlib](http://matplotlib.org)                 | “                                                      |
-| [pillow](https://github.com/python-pillow/Pillow)   | “                                                      |
+| Dependency                                                  | Function in pydna                                      |
+|-------------------------------------------------------------|--------------------------------------------------------|
+| [scipy >=1.8.0](https://www.scipy.org)                      | gel simulation with pydna.gel                          |
+| [matplotlib >=3.4.3](http://matplotlib.org)                 | “                                                      |
+| [pillow >=8.4.0](https://github.com/python-pillow/Pillow)   | “                                                      |
+| [numpy](http://www.numpy.org)                               | "                                                      |
+| [pyparsing >=2.4.7](https://pypi.python.org/pypi/pyparsing) | fix corrupt Genbank files with pydna.genbankfixer      |
+| [requests >=2.26.0](https://pypi.org/project/requests)      | download sequences with pydna.download                 |
+| [cai2 >=1.0.5](https://pypi.python.org/pypi/cai2)           | codon adaptation index calculations in several modules |
+| [pyqt5 >=5.15.0](https://pypi.python.org/pypi/pyqt5)        | codon adaptation index calculations in several modules |
 
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
 ## Requirements for running tests and analyzing code coverage
 
 - [pytest](https://pypi.org/project/pytest)
 - [pytest-cov](https://pypi.org/project/pytest-cov)
-- [pytest-mock](https://pypi.org/project/pytest-mock)
 - [pytest-doctestplus](https://pypi.org/project/pytest-doctestplus)
 - [coverage](https://pypi.org/project/coverage)
 - [nbval](https://pypi.org/project/nbval)
 - [requests-mock](https://pypi.org/project/requests-mock)
 
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
+## Releases
 
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
-
-## Changelog
-
-See the [change log](docs/CHANGELOG.md) for recent changes.
+See the [releases](https://github.com/BjornFJohansson/pydna/releases) for changes and releases.
 
-![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
 ## Automatic testing & Release process
 
-There are three github actions associated with this package:
+There are two github actions for this package:
 
 - `pydna_test_and_coverage_workflow.yml`
+- `pydna_pypi_build_workflow.yml`
 
-The `pydna_test_and_coverage_workflow.yml` is triggered on all pushed non-tagged commits.
-This workflow run tests, doctests and a series of Jupyter notebooks using pytest.
+The `pydna_test_and_coverage_workflow.yml` is triggered on all pushed commits for all branches.
+This workflow run tests, doctests and a series of Jupyter notebooks using pytest on Linux, Windows and macOS and all
+supported python versions.
 
-The two other workflows build a setuptools wheel and packages for different Python versions
-on Linux, Windows and macOS.
+The other workflow builds a PyPI packages using poetry on
 
 These are triggered by publishing a github release manually from the github interface.
 
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+## Building a PyPI package with [Poetry](https://pypi.org/project/poetry)
+
+1. Commit changes to git
+2. Tag the commit according to the [Semantic Versioning](https://semver.org) format, for example "v2.0.1a3". Do not forget the "v" or poetry will not recognize the tag.
+
+        git tag v2.0.1a3
 
-## Building a PyPI package
+3. Pydna uses the poetry [poetry-dynamic-versioning](https://pypi.org/project/poetry-dynamic-versioning) plugin.
 
+        poetry dynamic-versioning # This sets the version number in the source files
 
-	poetry build # run this command in the root directory where the pyproject.toml file is located
+4. Verify the version
 
+        poetry version
 
-Pydna uses the poetry plugin []()
+5. Build package:
 
+        poetry build # run this command in the root directory where the pyproject.toml file is located
 
+6. Verify the filename of the files in the dist/ folder, they should match
 
+7. Publish to pypi
 
+        poetry publish
 
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
 
-### History
+## History
 
 Pydna was made public in 2012 on [Google code](https://code.google.com/archive/p/pydna).
 
 
 :microbe:
```

### Comparing `pydna-5.2.0a9/pyproject.toml` & `pydna-6.0.0a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -14,49 +14,70 @@
              "Programming Language :: Python :: 3.7",
              "Programming Language :: Python :: 3.8",
              "Programming Language :: Python :: 3.9",
              "Programming Language :: Python :: 3.10",
              "Programming Language :: Python :: 3.11",
              "Topic :: Education",
              "Topic :: Scientific/Engineering :: Bio-Informatics", ]
+[project.urls]
+homepage = "https://github.com/BjornFJohansson/pydna#-pydna"
+documentation = "https://pydna.readthedocs.io/?badge=latest"
+repository = "https://github.com/BjornFJohansson/pydna/tree/dev_bjorn"
+changelog = "https://github.com/BjornFJohansson/pydna/blob/master/docs/CHANGELOG.md#changelog"
 [tool.poetry]
 name = "pydna"
-version = "5.2.0-a.9"
+version = "6.0.0-a.1"
 description = "Representing double stranded DNA and functions for simulating cloning and homologous recombination between DNA molecules."
 authors = ["BjornFJohansson <bjornjobb@gmail.com>"]
 license = "BSD"
 readme = "README.md"
 [tool.poetry.dependencies]
-python = "^3.8"
-appdirs = "^1.4.4"
-biopython = "^1.80"
-networkx = "^2.8.8"
-prettytable = "^3.5.0"
-pyperclip = "^1.8.2"
-pyfiglet = "^0.8.post1"
-
-scipy = { version = "1.8.0", optional = true }
-matplotlib = { version = "3.4.3", optional = true }
-pillow = { version = "8.4.0", optional = true }
-
-pyparsing = { version = "^2.4.7", optional = true }
-requests = { version = "2.26.0", optional = true }
-
-CAI = { version = "1.0.3", optional = true }
+python = ">=3.8"
+appdirs = ">=1.4.4"
+biopython = ">=1.80"
+networkx = ">=2.8.8"
+pydivsufsort = ">=0.0.11"
+prettytable = ">=3.5.0"
+pyperclip = ">=1.8.2"
+pyfiglet = ">=0.8.post1"
+scipy = { version = ">=1.8.0", optional = true }
+matplotlib = { version = ">=3.4.3", optional = true }
+pillow = { version = ">=8.4.0", optional = true }
+pyparsing = { version = ">=2.4.7", optional = true }
+requests = { version = ">=2.26.0", optional = true }
+cai2 = { version = ">=1.0.5", optional = true }
+pyqt5 = { version = ">=5.15.0", optional = true }
 
 [tool.poetry.extras]
 gel = ["scipy", "matplotlib", "pillow"]
 download = ["pyparsing", "requests"]
-express = ["CAI"]
-test = ["pytest", "pytest-cov", "pytest-mock", "pytest-doctestplus", "coverage", "nbval", "requests-mock"]
+gui = ["pyqt5"]
+express = ["cai2"]
 [build-system]
 requires = ["poetry-core",
             "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 [tool.poetry-dynamic-versioning.substitution]
 folders = [
   { path = "src"}
+]
+[tool.poetry.group.test] # This part can be left out
+[tool.poetry.group.test.dependencies]
+pytest = ">=7.2.0"
+pytest-cov = ">=4.0.0"
+pytest-doctestplus = ">=0.12.1"
+pytest-profiling = ">=1.7.0"
+coverage = ">=7.1.0"
+nbval = ">=0.9.6"
+requests-mock = ">=1.10.0"
+pyparsing = ">=2.4.7"
+[tool.pytest.ini_options]
+minversion = "6.0.2"
+python_files = "test_*.py"
+testpaths = [
+    "tests",
+    "src",
 ]
```

### Comparing `pydna-5.2.0a9/src/pydna/__init__.py` & `pydna-6.0.0a1/src/pydna/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -145,103 +145,83 @@
 __author__ = "Björn Johansson"
 __copyright__ = "Copyright 2013 - 2021 Björn Johansson"
 __credits__ = ["Björn Johansson", "Mark Budde"]
 __license__ = "BSD"
 __maintainer__ = "Björn Johansson"
 __email__ = "bjorn_johansson@bio.uminho.pt"
 __status__ = "Development"  # "Production" #"Prototype"
-__version__ = "5.2.0-a.9"
+__version__ = "6.0.0-a.1"
 
 # create config directory
-_os.environ["pydna_config_dir"] = _os.getenv("pydna_config_dir",
-                                             _appdirs.user_config_dir("pydna"))
+_os.environ["pydna_config_dir"] = _os.getenv("pydna_config_dir", _appdirs.user_config_dir("pydna"))
 config_dir = _Path(_os.environ["pydna_config_dir"])
 config_dir.mkdir(parents=True, exist_ok=True)
 
 # set path for the pydna.ini file
-_ini_path = config_dir/"pydna.ini"
+_ini_path = config_dir / "pydna.ini"
 
 # define user_data_dir
 user_data_dir = _Path(_appdirs.user_data_dir("pydna"))
 
-default_ini = {"ape": "put/path/to/ape/here",
-               "cached_funcs": "pydna.genbank.genbank.nucleotide",
-               "data_dir": str(user_data_dir),
-               "email": "someone@example.com",
-               "enzymes": str(user_data_dir/"enzymes.md"),
-               "log_dir": _appdirs.user_log_dir("pydna"),
-               "loglevel": str(_logging.WARNING),
-               "primers": str(user_data_dir/"primers.md")}
+default_ini = {
+    "ape": "put/path/to/ape/here",
+    "cached_funcs": "pydna.genbank.genbank.nucleotide",
+    "data_dir": str(user_data_dir),
+    "email": "someone@example.com",
+    "enzymes": str(user_data_dir / "enzymes.md"),
+    "log_dir": _appdirs.user_log_dir("pydna"),
+    "loglevel": str(_logging.WARNING),
+    "primers": str(user_data_dir / "primers.md"),
+    "assembly_limit": str(10),
+}
 
 # initiate a config parser instance
 _parser = _configparser.ConfigParser()
 
 # if a pydna.ini exists, it is read
-if _os.path.exists(_ini_path):
+if _ini_path.exists():
     _parser.read(_ini_path)
 else:  # otherwise it is created with default settings
     _parser["main"] = default_ini
     with open(_ini_path, "w", encoding="utf-8") as f:  # TODO needs encoding?
         _parser.write(f)
 
 # pydna related environmental variables are set
 # from pydna.ini if they are not set already
 _main = _parser["main"]
 
 for key in default_ini:
-    _os.environ[f"pydna_{key}"] = _os.getenv(f"pydna_{key}",
-                                             _main.get(key,
-                                                       default_ini[key]))
+    _os.environ[f"pydna_{key}"] = _os.getenv(f"pydna_{key}", _main.get(key, default_ini[key]))
 
 logdir = _Path(_os.environ["pydna_log_dir"])
 
 # create log directory if not present
 logdir.mkdir(parents=True, exist_ok=True)
 _logmsg = "Log directory {}".format(logdir)
 
 # create logger
 _logger = _logging.getLogger("pydna")
 _logger.setLevel(int(_os.environ["pydna_loglevel"]))
-_hdlr = _handlers.RotatingFileHandler(logdir/"pydna.log",
-                                      mode="a",
-                                      maxBytes=10 * 1024 * 1024,
-                                      backupCount=10,
-                                      encoding="utf-8")
+_hdlr = _handlers.RotatingFileHandler(
+    logdir / "pydna.log", mode="a", maxBytes=10 * 1024 * 1024, backupCount=10, encoding="utf-8"
+)
 
-_formatter = _logging.Formatter(("%(asctime)s %(levelname)s"
-                                 " %(funcName)s %(message)s"))
+_formatter = _logging.Formatter(("%(asctime)s %(levelname)s" " %(funcName)s %(message)s"))
 _hdlr.setFormatter(_formatter)
 _logger.addHandler(_hdlr)
 _logger.info(_logmsg)
-_logger.info("Environmental variable pydna_ape          = %s",
-             _os.environ["pydna_ape"])
-_logger.info(
-    "Environmental variable pydna_cached_funcs = %s",
-    _os.environ["pydna_cached_funcs"]
-)
-_logger.info(
-    "Environmental variable pydna_data_dir     = %s",
-    _os.environ["pydna_data_dir"]
-)
-_logger.info(
-    "Environmental variable pydna_email        = %s",
-    _os.environ["pydna_email"]
-)
-_logger.info(
-    "Environmental variable pydna_log_dir      = %s",
-    _os.environ["pydna_log_dir"]
-)
-_logger.info(
-    "Environmental variable pydna_loglevel     = %s",
-    _os.environ["pydna_loglevel"]
-)
-_logger.info(
-    "Environmental variable pydna_primers      = %s",
-    _os.environ["pydna_primers"]
-)
+_logger.info("Environmental variable pydna_ape          = %s", _os.environ["pydna_ape"])
+_logger.info("Environmental variable pydna_cached_funcs = %s", _os.environ["pydna_cached_funcs"])
+_logger.info("Environmental variable pydna_data_dir     = %s", _os.environ["pydna_data_dir"])
+_logger.info("Environmental variable pydna_email        = %s", _os.environ["pydna_email"])
+_logger.info("Environmental variable pydna_log_dir      = %s", _os.environ["pydna_log_dir"])
+_logger.info("Environmental variable pydna_loglevel     = %s", _os.environ["pydna_loglevel"])
+_logger.info("Environmental variable pydna_primers      = %s", _os.environ["pydna_primers"])
+_logger.info("Environmental variable pydna_assembly_limit = %s", _os.environ["pydna_assembly_limit"])
+
 # create cache directory if not present
 
 _Path(_os.environ["pydna_data_dir"]).mkdir(parents=True, exist_ok=True)
 
 # find out if optional dependecies for gel module are in place
 
 
@@ -256,21 +236,17 @@
     del util
     return _missing
 
 
 _missing = _missing_modules_for_gel()
 
 if _missing:
-    _logger.warning(
-        "gel simulation will NOT be available."
-        " Missing modules: %s", ", ".join(_missing)
-    )
+    _logger.warning("gel simulation will NOT be available." " Missing modules: %s", ", ".join(_missing))
 else:
-    _logger.info("gel simulation is available,"
-                 " optional dependencies were found.")
+    _logger.info("gel simulation is available," " optional dependencies were found.")
 
 
 _logger.info("__version__ = %s", __version__)
 
 
 class _PydnaWarning(Warning):
     """Pydna warning.
@@ -395,14 +371,15 @@
     return _table
 
 
 def logo():
     """Ascii-art logotype of pydna."""
     from pydna._pretty import pretty_str as _pretty_str
     from pyfiglet import Figlet
+
     f = Figlet()
     return _pretty_str(f.renderText(f'pydna {__version__}'))
 
 
 if __name__ == "__main__":
     import os as _os
```

### Comparing `pydna-5.2.0a9/src/pydna/_pretty.py` & `pydna-6.0.0a1/src/pydna/_pretty.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 for for nicer string output in the IPython shell and Jupyter notebook.
 """
 
 from prettytable import PrettyTable as _Pt
 from prettytable import MARKDOWN as _md
 from copy import copy as _copy
 
+
 class pretty_str(str):
     """Thanks to Min RK, UC Berkeley for this."""
 
     def _repr_pretty_(self, p, cycle):
         p.text(self)
```

### Comparing `pydna-5.2.0a9/src/pydna/_thermodynamic_data.py` & `pydna-6.0.0a1/src/pydna/_thermodynamic_data.py`

 * *Files identical despite different names*

### Comparing `pydna-5.2.0a9/src/pydna/all.py` & `pydna-6.0.0a1/src/pydna/all.py`

 * *Files identical despite different names*

### Comparing `pydna-5.2.0a9/src/pydna/amplicon.py` & `pydna-6.0.0a1/src/pydna/amplicon.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,24 +39,15 @@
 
     template : Dseqrecord
         Dseqrecord object holding the template (circular or linear)
 
 
     """
 
-    def __init__(
-        self,
-        record,
-        *args,
-        template=None,
-        forward_primer=None,
-        reverse_primer=None,
-        **kwargs
-    ):
-
+    def __init__(self, record, *args, template=None, forward_primer=None, reverse_primer=None, **kwargs):
         super().__init__(record, *args)
         self.template = template
         self.forward_primer = forward_primer
         self.reverse_primer = reverse_primer
         self.__dict__.update(kwargs)
 
         # https://medium.com/@chipiga86/circular-references-without-memory-
@@ -117,47 +108,49 @@
         figure:string
              A string containing a text representation of the primers
              annealing on the template (see example above).
 
         """
 
         f = """
-            {sp1}5{faz}...{raz}3
+            {sp1}5{faz}{middle1}{raz}3
              {sp3}{rap}
             {sp3}3{rp}5
             5{fp}3
              {fap:>{fplength}}
-            {sp2}3{fzc}...{rzc}5
+            {sp2}3{fzc}{middle2}{rzc}5
             """.format(
             fp=self.forward_primer.seq,
             fap="|" * len(self.forward_primer.footprint),
             fplength=len(self.forward_primer.seq),
             rp=self.reverse_primer.seq[::-1],
             rap="|" * len(self.reverse_primer.footprint),
             faz=self.forward_primer.footprint,
             raz=self.reverse_primer.footprint.reverse_complement(),
             fzc=self.forward_primer.footprint.complement(),
             rzc=self.reverse_primer.footprint[::-1],
-            sp1=" "
-            * (len(self.forward_primer.seq) - len(self.forward_primer.footprint)),
-            sp2=" "
-            * (len(self.forward_primer.seq) - len(self.forward_primer.footprint)),
+            sp1=" " * (len(self.forward_primer.seq) - len(self.forward_primer.footprint)),
+            sp2=" " * (len(self.forward_primer.seq) - len(self.forward_primer.footprint)),
             sp3=" " * (3 + len(self.forward_primer.seq)),
+            middle1="...",
+            middle2="...",
         )
+
+        # type_, watson, rcrick = self.template.figure().splitlines()
+        # f2 = (f"{watson}\n"
+
+        #       f"{rcrick}\n")
+        # print(f2)
         return _pretty_str(_textwrap.dedent(f).strip("\n"))
 
     def set_forward_primer_footprint(self, length):
-        self.forward_primer = _Primer(
-            self.forward_primer.tail + self.seq[:length], footprint=length
-        )
+        self.forward_primer = _Primer(self.forward_primer.tail + self.seq[:length], footprint=length)
 
     def set_reverse_primer_footprint(self, length):
-        self.reverse_primer = _Primer(
-            self.reverse_primer.tail + self.seq[:length], footprint=length
-        )
+        self.reverse_primer = _Primer(self.reverse_primer.tail + self.seq[:length], footprint=length)
 
     def program(self):
         return _program(self)
 
     def dbd_program(self):
         return _dbd_program(self)
```

### Comparing `pydna-5.2.0a9/src/pydna/amplify.py` & `pydna-6.0.0a1/src/pydna/amplify.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 PCR product. The Anneal class should be used if more flexibility is required.
 
 Primers with 5' tails as well as inverse PCR on circular templates are handled
 correctly."""
 
 from pydna._pretty import pretty_str as _pretty_str
 from pydna.utils import flatten as _flatten
-from pydna.utils import memorize as _memorize
+
+# from pydna.utils import memorize as _memorize
 from pydna.utils import rc as _rc
 from pydna.amplicon import Amplicon as _Amplicon
 from pydna.primer import Primer as _Primer
 from pydna.seqrecord import SeqRecord as _SeqRecord
 from pydna.dseqrecord import Dseqrecord as _Dseqrecord
 from Bio.SeqFeature import SeqFeature as _SeqFeature
 from Bio.SeqFeature import SimpleLocation as _SimpleLocation
@@ -95,40 +96,35 @@
         "N": "(A|G|C|T)",
     }
 
     # Make regex pattern that reflects extended IUPAC DNA code
     for key in table:
         head = head.replace(key, table[key])
 
-    positions = [
-        m.start() for m in _re.finditer("(?={})".format(head), template, _re.I)
-    ]
+    positions = [m.start() for m in _re.finditer("(?={})".format(head), template, _re.I)]
 
     if positions:
         tail = prc[limit:].lower()
         length = len(tail)
         results = []
         for match_start in positions:
-            tm = template[match_start + limit:
-                          match_start + limit + length].lower()
-            footprint = len(list(_itertools.takewhile(lambda x: x[0] == x[1],
-                                                      zip(tail,
-                                                          tm))))
+            tm = template[match_start + limit : match_start + limit + length].lower()
+            footprint = len(list(_itertools.takewhile(lambda x: x[0] == x[1], zip(tail, tm))))
             results.append((match_start, footprint + limit))
         return results
     return []
 
 
-class _Memoize(type):
-    @_memorize("pydna.amplify.Anneal")
-    def __call__(cls, *args, **kwargs):
-        return super().__call__(*args, **kwargs)
+# class _Memoize(type):
+#     @_memorize("pydna.amplify.Anneal")
+#     def __call__(cls, *args, **kwargs):
+#         return super().__call__(*args, **kwargs)
 
 
-class Anneal(object, metaclass=_Memoize):
+class Anneal(object):  # ), metaclass=_Memoize):
     """The Anneal class has the following important attributes:
 
     Attributes
     ----------
     forward_primers : list
         Description of `forward_primers`.
     reverse_primers : list
@@ -173,15 +169,15 @@
         ...        "gatc"*240 +
         ...        "ctatcgactgtatcatctgatagcac")
         >>> from Bio.SeqRecord import SeqRecord
         >>> p1 = read(">p1\ntacactcaccgtctatcattatc", ds = False)
         >>> p2 = read(">p2\ngtgctatcagatgatacagtcg", ds = False)
         >>> ann = Anneal((p1, p2), t)
         >>> print(ann.report())
-        Template name 1011 nt linear:
+        Template name 1011 bp linear limit=13:
         p1 anneals forward (--->) at 23
         p2 anneals reverse (<---) at 989
         >>> ann.products
         [Amplicon(1011)]
         >>> amplicon_list = ann.products
         >>> amplicon = amplicon_list.pop()
         >>> amplicon
@@ -224,20 +220,20 @@
 
         self.forward_primers = []
         self.reverse_primers = []
 
         twl = len(self.template.seq.watson)
         tcl = len(self.template.seq.crick)
 
-        if self.template.linear:
-            tw = self.template.seq.watson
-            tc = self.template.seq.crick
-        else:
+        if self.template.circular:
             tw = self.template.seq.watson + self.template.seq.watson
             tc = self.template.seq.crick + self.template.seq.crick
+        else:
+            tw = self.template.seq.watson
+            tc = self.template.seq.crick
 
         for p in self.primers:
             self.forward_primers.extend(
                 (
                     _Primer(
                         p,
                         #          template = self.template,
@@ -270,14 +266,15 @@
                 end = fp.position
                 self.template.features.append(
                     _SeqFeature(
                         _SimpleLocation(start, end, strand=1),
                         type="primer_bind",
                         qualifiers={
                             "label": [fp.name],
+                            "PCR_conditions": [f"primer sequence:{fp.seq}"],
                             "ApEinfo_fwdcolor": ["#baffa3"],
                             "ApEinfo_revcolor": ["#ffbaba"],
                         },
                     )
                 )
             else:
                 start = len(self.template) - fp._fp + fp.position
@@ -288,14 +285,15 @@
                             _SimpleLocation(start, len(self.template)),
                             _SimpleLocation(0, end),
                         ]
                     ),
                     type="primer_bind",
                     qualifiers={
                         "label": [fp.name],
+                        "PCR_conditions": [f"primer sequence:{fp.seq}"],
                         "ApEinfo_fwdcolor": ["#baffa3"],
                         "ApEinfo_revcolor": ["#ffbaba"],
                     },
                 )
                 self.template.features.append(sf)
 
         for rp in self.reverse_primers:
@@ -304,86 +302,67 @@
                 end = rp.position + rp._fp
                 self.template.features.append(
                     _SeqFeature(
                         _SimpleLocation(start, end, strand=-1),
                         type="primer_bind",
                         qualifiers={
                             "label": [rp.name],
+                            "PCR_conditions": [f"primer sequence:{rp.seq}"],
                             "ApEinfo_fwdcolor": ["#baffa3"],
                             "ApEinfo_revcolor": ["#ffbaba"],
                         },
                     )
                 )
             else:
                 start = rp.position
                 end = rp.position + rp._fp - len(self.template)
                 self.template.features.append(
                     _SeqFeature(
                         _CompoundLocation(
                             [
-                                _SimpleLocation(0,
-                                                 end,
-                                                 strand=-1),
-                                _SimpleLocation(start,
-                                                 len(self.template),
-                                                 strand=-1),
+                                _SimpleLocation(0, end, strand=-1),
+                                _SimpleLocation(start, len(self.template), strand=-1),
                             ],
                         ),
                         type="primer_bind",
                         qualifiers={"label": [rp.name]},
                     )
                 )
 
     @property
     def products(self):
-
         if self._products:
             return self._products
 
         self._products = []
 
         for fp in self.forward_primers:
             for rp in self.reverse_primers:
-
                 if self.template.circular:
                     tmpl = self.template.shifted(fp.position - fp._fp)
                     tmpl = tmpl[:] * 2
                     for f in tmpl.features:
                         for x, y in zip(f.location.parts, f.location.parts[1:]):
                             if x.end == y.start + len(self.template):
                                 f.location = _SimpleLocation(
                                     x.start,
                                     y.end + len(self.template),
                                     strand=f.location.strand,
                                 )
                     if fp.position > rp.position:
-                        tmpl = tmpl[
-                            : len(self.template)
-                            - fp.position
-                            + rp.position
-                            + rp._fp
-                            + fp._fp
-                        ]
+                        tmpl = tmpl[: len(self.template) - fp.position + rp.position + rp._fp + fp._fp]
                     else:
                         tmpl = tmpl[: rp.position + rp._fp - (fp.position - fp._fp)]
                 elif fp.position <= rp.position:
                     tmpl = self.template[fp.position - fp._fp : rp.position + rp._fp]
                 else:
                     continue
-                prd = (
-                    _Dseqrecord(fp.tail)
-                    + tmpl
-                    + _Dseqrecord(rp.tail).reverse_complement()
-                )
+                prd = _Dseqrecord(fp.tail) + tmpl + _Dseqrecord(rp.tail).reverse_complement()
 
-                full_tmpl_features = [
-                    f
-                    for f in tmpl.features
-                    if f.location.start == 0 and f.location.end == len(tmpl)
-                ]
+                full_tmpl_features = [f for f in tmpl.features if f.location.start == 0 and f.location.end == len(tmpl)]
 
                 new_identifier = ""
                 if full_tmpl_features:
                     ft = full_tmpl_features[0]
                     if "label" in ft.qualifiers:
                         new_identifier = " ".join(ft.qualifiers["label"])
                     elif "note" in ft.qualifiers:
@@ -399,61 +378,50 @@
                     or "{}bp_PCR_prod".format(len(prd))[:16]
                 )
                 prd.id = (
                     _identifier_from_string(new_identifier)[:16]
                     or self.kwargs.get("id")
                     or "{}bp_{}".format(str(len(prd))[:14], prd.useguid())
                 )
-                prd.description = self.kwargs.get(
-                    "description"
-                ) or "pcr_product_{}_{}".format(fp.description, rp.description)
-
-                amplicon = _Amplicon(
-                    prd,
-                    template=self.template,
-                    forward_primer=fp,
-                    reverse_primer=rp,
-                    **self.kwargs
+                prd.description = self.kwargs.get("description") or "pcr_product_{}_{}".format(
+                    fp.description, rp.description
                 )
 
+                amplicon = _Amplicon(prd, template=self.template, forward_primer=fp, reverse_primer=rp, **self.kwargs)
+
                 # amplicon.forward_primer.amplicon = amplicon
                 # amplicon.reverse_primer.amplicon = amplicon
 
                 self._products.append(amplicon)
 
         return self._products
 
     def __repr__(self):
-        """ returns a short string representation """
-        return "Reaction(products = {})".format(
-            len(self.forward_primers * len(self.reverse_primers))
-        )
+        """returns a short string representation"""
+        return "Reaction(products = {})".format(len(self.forward_primers * len(self.reverse_primers)))
 
     def __str__(self):
         """returns a short report describing if or where primer
         anneal on the template."""
 
-        mystring = "Template {name} {size} nt {top}:\n".format(
+        mystring = "Template {name} {size} bp {top} limit={limit}:\n".format(
             name=self.template.name,
             size=len(self.template),
             top={True: "circular", False: "linear"}[self.template.circular],
+            limit=self.limit,
         )
         if self.forward_primers:
             for p in self.forward_primers:
-                mystring += "{name} anneals forward (--->) at {pos}\n".format(
-                    name=p.name, pos=p.position
-                )
+                mystring += "{name} anneals forward (--->) at {pos}\n".format(name=p.name, pos=p.position)
         else:
             mystring += "No forward primers anneal...\n"
         # mystring +="\n"
         if self.reverse_primers:
             for p in self.reverse_primers:
-                mystring += "{name} anneals reverse (<---) at {pos}\n".format(
-                    name=p.name, pos=p.position
-                )
+                mystring += "{name} anneals reverse (<---) at {pos}\n".format(name=p.name, pos=p.position)
         else:
             mystring += "No reverse primers anneal...\n"
         return _pretty_str(mystring.strip())
 
     report = __str__
 
 
@@ -518,27 +486,25 @@
     >>>
 
     """
 
     output = _flatten(args)  # flatten
     new = []
     for s in output:
-
         if hasattr(s, "watson"):
             s = _SeqRecord(_Seq(s.watson))
         elif hasattr(s, "transcribe"):
             s = _SeqRecord(s)
         elif isinstance(s, str):
             s = _SeqRecord(_Seq(s))
         elif hasattr(s, "features"):
             pass
         else:
             raise TypeError(
-                "arguments need to be a string, Bio.Seq, SeqRecord"
-                ", Primer, Dseqrecord or Amplicon object"
+                "arguments need to be a string, Bio.Seq, SeqRecord" ", Primer, Dseqrecord or Amplicon object"
             )
         new.append(s)
 
     # A single Amplicon object
     if len(new) == 1 and hasattr(new[0], "forward_primer"):
         new = [new[0].forward_primer, new[0].reverse_primer, new[0].template]
 
@@ -546,19 +512,18 @@
         new[-1] = _Dseqrecord(s)
 
     anneal_primers = Anneal(new[:-1], new[-1], **kwargs)
 
     if len(anneal_primers.products) == 1:
         return anneal_primers.products[0]
     elif len(anneal_primers.products) == 0:
-        raise ValueError("No PCR product! {}".format(anneal_primers.report()))
-    raise ValueError("PCR not specific! {}".format(anneal_primers.report()))
+        raise ValueError(f"No PCR product! {anneal_primers.report()}")
+    raise ValueError("PCR not specific! {format(anneal_primers.report()}")
 
 
 if __name__ == "__main__":
-
     cached = _os.getenv("pydna_cached_funcs", "")
     _os.environ["pydna_cached_funcs"] = ""
     import doctest
 
     doctest.testmod(verbose=True, optionflags=doctest.ELLIPSIS)
     _os.environ["pydna_cached_funcs"] = cached
```

### Comparing `pydna-5.2.0a9/src/pydna/assembly.py` & `pydna-6.0.0a1/src/pydna/assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,42 +38,49 @@
     y : actgt
     z : aaagttct
 
 
 The NetworkX package is used to trace linear and circular paths through the
 graph.
 """
+import os as _os
 from Bio.SeqFeature import ExactPosition as _ExactPosition
 from Bio.SeqFeature import SimpleLocation as _SimpleLocation
 from Bio.SeqFeature import CompoundLocation as _CompoundLocation
 from pydna.utils import rc as _rc
-from pydna.utils import memorize as _memorize
+
+# from pydna.utils import memorize as _memorize
 from pydna._pretty import pretty_str as _pretty_str
 from pydna.contig import Contig as _Contig
 from pydna.common_sub_strings import common_sub_strings
+from pydna.common_sub_strings import terminal_overlap
 from pydna.dseqrecord import Dseqrecord as _Dseqrecord
 import networkx as _nx
 from copy import deepcopy as _deepcopy
 import itertools as _itertools
 import logging as _logging
 
+# from func_timeout import func_set_timeout
+# from wrapt_timeout_decorator import timeout
+from pydna.threading_timer_decorator_exit import exit_after
+
 _module_logger = _logging.getLogger("pydna." + __name__)
 
 
 # TODO use quicker inits for contig
 # TODO remove maxnodes for init
 
 
-class _Memoize(type):
-    @_memorize("pydna.assembly.Assembly")
-    def __call__(cls, *args, **kwargs):
-        return super().__call__(*args, **kwargs)
+# class _Memoize(type):
+#     @_memorize("pydna.assembly.Assembly")
+#     def __call__(cls, *args, **kwargs):
+#         return super().__call__(*args, **kwargs)
 
 
-class Assembly(object, metaclass=_Memoize):
+class Assembly(object):  # , metaclass=_Memoize):
     """Assembly of a list of linear DNA fragments into linear or circular
     constructs. The Assembly is meant to replace the Assembly method as it
     is easier to use. Accepts a list of Dseqrecords (source fragments) to
     initiate an Assembly object. Several methods are available for analysis
     of overlapping sequences, graph construction and assembly.
 
     Parameters
@@ -111,15 +118,14 @@
     >>> x.assemble_circular()[0].seq.watson
     'acgatgctatactgCCCCCtgtgctgtgctctaTTTTTtattctggctgtatcGGGGGt'
 
 
     """
 
     def __init__(self, frags=None, limit=25, algorithm=common_sub_strings):
-
         # Fragments is a string subclass with some extra properties
         # The order of the fragments has significance
         fragments = []
         for f in frags:
             fragments.append(
                 {
                     "upper": str(f.seq).upper(),
@@ -153,15 +159,14 @@
             "end_rc": "begin_rc",
         }
 
         # all combinations of fragments are compared.
         # see https://docs.python.org/3.10/library/itertools.html
         # itertools.combinations('ABCD', 2)-->  AB AC AD BC BD CD
         for first, secnd in _itertools.combinations(fragments, 2):
-
             if first["upper"] == secnd["upper"]:
                 continue
 
             firrc = rcfragments[first["mixed"]]
             secrc = rcfragments[secnd["mixed"]]
 
             # matches is a list of tuples of three integers describing
@@ -222,40 +227,35 @@
         for f in fragments:
             f["nodes"] = sorted(set(f["nodes"]))
 
         for f in rcfragments.values():
             f["nodes"] = sorted(set(f["nodes"]))
 
         for f in _itertools.chain(fragments, rcfragments.values()):
-
             # nodes are sorted in place in the order of their position
             # duplicates are removed (same position and sequence)
             # along the fragment since nodes are a tuple (position(int),
             # sequence(str))
 
             before = G.order()
             G.add_nodes_from(
                 (node, {"order": order + od, "length": length})
-                for od, (start, length, node) in enumerate(
-                    n for n in f["nodes"] if n[2] not in G
-                )
+                for od, (start, length, node) in enumerate(n for n in f["nodes"] if n[2] not in G)
             )
             order += G.order() - before
 
             for (start1, length1, node1), (
                 start2,
                 length2,
                 node2,
             ) in _itertools.combinations(f["nodes"], 2):
-
                 feats = [
                     ft
                     for ft in f["features"]
-                    if start1 <= ft.location.start
-                    and start2 + G.nodes[node2]["length"] >= ft.location.end
+                    if start1 <= ft.location.start and start2 + G.nodes[node2]["length"] >= ft.location.end
                 ]
 
                 for feat in feats:
                     feat.location += -start1
 
                 G.add_edge(
                     node1,
@@ -263,107 +263,85 @@
                     piece=slice(start1, start2),  # slice
                     features=feats,  # features
                     seq=f["mixed"],  # mixed case string
                     name=f["name"],
                 )  # string
 
         self.G = _nx.create_empty_copy(G)
-        self.G.add_edges_from(
-            sorted(
-                G.edges(data=True), key=lambda t: len(t[2].get("seq", 1)), reverse=True
-            )
-        )
+        self.G.add_edges_from(sorted(G.edges(data=True), key=lambda t: len(t[2].get("seq", 1)), reverse=True))
         self.nodemap = {**nodemap, **{nodemap[i]: i for i in nodemap}}
         self.limit = limit
         self.fragments = fragments
         self.rcfragments = rcfragments
         self.algorithm = algorithm
 
+    @exit_after(int(_os.getenv("pydna_assembly_limit", 10)))
     def assemble_linear(self, start=None, end=None, max_nodes=None):
-
         G = _nx.MultiDiGraph(self.G)
 
         G.add_nodes_from(["begin", "begin_rc", "end", "end_rc"], length=0)
 
         # add edges from "begin" to nodes in the first
         # sequence in self.fragments
         firstfragment = self.fragments[0]
         for start, length, node in firstfragment["nodes"][::-1]:
             G.add_edge(
                 "begin",
                 node,
                 piece=slice(0, start),
-                features=[
-                    f
-                    for f in firstfragment["features"]
-                    if start + length >= f.location.end
-                ],
+                features=[f for f in firstfragment["features"] if start + length >= f.location.end],
                 seq=firstfragment["mixed"],
                 name=firstfragment["name"],
             )
 
         # add edges from "begin_rc" to nodes in the reverse complement of the
         # first sequence
         firstfragmentrc = self.rcfragments[firstfragment["mixed"]]
         for start, length, node in firstfragmentrc["nodes"][::-1]:
             G.add_edge(
                 "begin_rc",
                 node,
                 piece=slice(0, start),
-                features=[
-                    f
-                    for f in firstfragmentrc["features"]
-                    if start + length >= f.location.end
-                ],
+                features=[f for f in firstfragmentrc["features"] if start + length >= f.location.end],
                 seq=firstfragmentrc["mixed"],
                 name=firstfragmentrc["name"],
             )
 
         # add edges from nodes in last sequence to "end"
         lastfragment = self.fragments[-1]
         for start, length, node in lastfragment["nodes"]:
             G.add_edge(
                 node,
                 "end",
                 piece=slice(start, len(lastfragment["mixed"])),
-                features=[
-                    f for f in lastfragment["features"] if start <= f.location.end
-                ],
+                features=[f for f in lastfragment["features"] if start <= f.location.end],
                 seq=lastfragment["mixed"],
                 name=lastfragment["name"],
             )
 
         # add edges from nodes in last reverse complement sequence to "end_rc"
         lastfragmentrc = self.rcfragments[lastfragment["mixed"]]
         for start, length, node in lastfragmentrc["nodes"]:
             G.add_edge(
                 node,
                 "end_rc",
                 piece=slice(start, len(lastfragmentrc["mixed"])),
-                features=[
-                    f for f in lastfragmentrc["features"] if start <= f.location.end
-                ],
+                features=[f for f in lastfragmentrc["features"] if start <= f.location.end],
                 seq=lastfragmentrc["mixed"],
                 name=lastfragmentrc["name"],
             )
 
         max_nodes = max_nodes or len(self.fragments)
 
         linearpaths = list(
             _itertools.chain(
                 _nx.all_simple_paths(_nx.DiGraph(G), "begin", "end", cutoff=max_nodes),
-                _nx.all_simple_paths(
-                    _nx.DiGraph(G), "begin", "end_rc", cutoff=max_nodes
-                ),
-                _nx.all_simple_paths(
-                    _nx.DiGraph(G), "begin_rc", "end", cutoff=max_nodes
-                ),
-                _nx.all_simple_paths(
-                    _nx.DiGraph(G), "begin_rc", "end_rc", cutoff=max_nodes
-                ),
+                _nx.all_simple_paths(_nx.DiGraph(G), "begin", "end_rc", cutoff=max_nodes),
+                _nx.all_simple_paths(_nx.DiGraph(G), "begin_rc", "end", cutoff=max_nodes),
+                _nx.all_simple_paths(_nx.DiGraph(G), "begin_rc", "end_rc", cutoff=max_nodes),
             )
         )
 
         lps = {}
 
         for lp in linearpaths:
             edgelol = []
@@ -382,15 +360,15 @@
                     if ((e["seq"], e["piece"].stop) == (z["seq"], z["piece"].start))
                 ]:
                     continue
                 ct = "".join(e["seq"][e["piece"]] for u, v, e in edges)
                 key = ct.upper()
 
                 if key in lps:
-                    continue    # TODO: is this test needed?
+                    continue  # TODO: is this test needed?
                 sg = _nx.DiGraph()
                 sg.add_edges_from(edges)
                 sg.add_nodes_from((n, d) for n, d in G.nodes(data=True) if n in lp)
 
                 edgefeatures = []
                 offset = 0
                 for u, v, e in edges:
@@ -414,31 +392,30 @@
                 )
                 for lp in lps.values()
             ),
             key=len,
             reverse=True,
         )
 
+    @exit_after(int(_os.getenv("pydna_assembly_limit", 10)))
     def assemble_circular(self):
         cps = {}  # circular assembly
         cpsrc = {}
         cpaths = sorted(_nx.simple_cycles(self.G), key=len)
         cpaths_sorted = []
         for cpath in cpaths:
             order, node = min((self.G.nodes[node]["order"], node) for node in cpath)
             i = cpath.index(node)
             cpaths_sorted.append((order, cpath[i:] + cpath[:i]))
         cpaths_sorted.sort()
 
         for (
             _,
             cp,
-        ) in (
-            cpaths_sorted
-        ):  # cpaths is a list of nodes representing a circular assembly
+        ) in cpaths_sorted:  # cpaths is a list of nodes representing a circular assembly
             edgelol = []  # edgelol is a list of lists of all edges along cp
             cp += cp[0:1]
             for u, v in zip(cp, cp[1:]):
                 e = []
                 for d in self.G[u][v].values():
                     e.append((u, v, d))
                 edgelol.append(e)
@@ -470,20 +447,16 @@
                     offset += e["piece"].stop - e["piece"].start
                     for f in edgefeatures:
                         if f.location.start > len(ct) and f.location.end > len(ct):
                             f.location += -len(ct)
                         elif f.location.end > len(ct):
                             f.location = _CompoundLocation(
                                 (
-                                    _SimpleLocation(
-                                        f.location.start, _ExactPosition(len(ct))
-                                    ),
-                                    _SimpleLocation(
-                                        _ExactPosition(0), f.location.end - len(ct)
-                                    ),
+                                    _SimpleLocation(f.location.start, _ExactPosition(len(ct))),
+                                    _SimpleLocation(_ExactPosition(0), f.location.end - len(ct)),
                                 )
                             )
 
                 cps[key] = cpsrc[_rc(key)] = (
                     ct,
                     edgefeatures,
                     sg,
@@ -511,17 +484,15 @@
         # https://pyformat.info
         return _pretty_str(
             "Assembly\n"
             "fragments..: {sequences}\n"
             "limit(bp)..: {limit}\n"
             "G.nodes....: {nodes}\n"
             "algorithm..: {al}".format(
-                sequences=" ".join(
-                    "{}bp".format(len(x["mixed"])) for x in self.fragments
-                ),
+                sequences=" ".join("{}bp".format(len(x["mixed"])) for x in self.fragments),
                 limit=self.limit,
                 nodes=self.G.order(),
                 al=self.algorithm.__name__,
             )
         )
```

### Comparing `pydna-5.2.0a9/src/pydna/codon.py` & `pydna-6.0.0a1/src/pydna/codon.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,118 +4,122 @@
 
 # PMID: 22645496
 
 # https://www.genome.jp/kegg/catalog/org_list.html
 
 weights = {}
 
-weights["sce"] = {'TTT': 1.0,
-                  'TTG': 1.0,
-                  'TAT': 1.0,
-                  'TAG': 0.479,
-                  'TGT': 1.0,
-                  'TGG': 1.0,
-                  'TCT': 1.0,
-                  'TCG': 0.364,
-                  'ATT': 1.0,
-                  'ATG': 1.0,
-                  'AAT': 1.0,
-                  'AAG': 0.736,
-                  'AGT': 0.602,
-                  'AGG': 0.433,
-                  'ACT': 1.0,
-                  'ACG': 0.393,
-                  'GTT': 1.0,
-                  'GTG': 0.488,
-                  'GAT': 1.0,
-                  'GAG': 0.422,
-                  'GGT': 1.0,
-                  'GGG': 0.252,
-                  'GCT': 1.0,
-                  'GCG': 0.292,
-                  'CTT': 0.451,
-                  'CTG': 0.386,
-                  'CAT': 1.0,
-                  'CAG': 0.444,
-                  'CGT': 0.3,
-                  'CGG': 0.082,
-                  'CCT': 0.738,
-                  'CCG': 0.289,
-                  'TTA': 0.962,
-                  'TTC': 0.706,
-                  'TAA': 1.0,
-                  'TAC': 0.787,
-                  'TGA': 0.643,
-                  'TGC': 0.588,
-                  'TCA': 0.795,
-                  'TCC': 0.605,
-                  'ATA': 0.59,
-                  'ATC': 0.57,
-                  'AAA': 1.0,
-                  'AAC': 0.696,
-                  'AGA': 1.0,
-                  'AGC': 0.415,
-                  'ACA': 0.876,
-                  'ACC': 0.628,
-                  'GTA': 0.533,
-                  'GTC': 0.533,
-                  'GAA': 1.0,
-                  'GAC': 0.538,
-                  'GGA': 0.456,
-                  'GGC': 0.409,
-                  'GCA': 0.765,
-                  'GCC': 0.595,
-                  'CTA': 0.493,
-                  'CTC': 0.2,
-                  'CAA': 1.0,
-                  'CAC': 0.571,
-                  'CGA': 0.141,
-                  'CGC': 0.122,
-                  'CCA': 1.0,
-                  'CCC': 0.37}
+weights["sce"] = {
+    'TTT': 1.0,
+    'TTG': 1.0,
+    'TAT': 1.0,
+    'TAG': 0.479,
+    'TGT': 1.0,
+    'TGG': 1.0,
+    'TCT': 1.0,
+    'TCG': 0.364,
+    'ATT': 1.0,
+    'ATG': 1.0,
+    'AAT': 1.0,
+    'AAG': 0.736,
+    'AGT': 0.602,
+    'AGG': 0.433,
+    'ACT': 1.0,
+    'ACG': 0.393,
+    'GTT': 1.0,
+    'GTG': 0.488,
+    'GAT': 1.0,
+    'GAG': 0.422,
+    'GGT': 1.0,
+    'GGG': 0.252,
+    'GCT': 1.0,
+    'GCG': 0.292,
+    'CTT': 0.451,
+    'CTG': 0.386,
+    'CAT': 1.0,
+    'CAG': 0.444,
+    'CGT': 0.3,
+    'CGG': 0.082,
+    'CCT': 0.738,
+    'CCG': 0.289,
+    'TTA': 0.962,
+    'TTC': 0.706,
+    'TAA': 1.0,
+    'TAC': 0.787,
+    'TGA': 0.643,
+    'TGC': 0.588,
+    'TCA': 0.795,
+    'TCC': 0.605,
+    'ATA': 0.59,
+    'ATC': 0.57,
+    'AAA': 1.0,
+    'AAC': 0.696,
+    'AGA': 1.0,
+    'AGC': 0.415,
+    'ACA': 0.876,
+    'ACC': 0.628,
+    'GTA': 0.533,
+    'GTC': 0.533,
+    'GAA': 1.0,
+    'GAC': 0.538,
+    'GGA': 0.456,
+    'GGC': 0.409,
+    'GCA': 0.765,
+    'GCC': 0.595,
+    'CTA': 0.493,
+    'CTC': 0.2,
+    'CAA': 1.0,
+    'CAC': 0.571,
+    'CGA': 0.141,
+    'CGC': 0.122,
+    'CCA': 1.0,
+    'CCC': 0.37,
+}
 
 
 # PMID: 6390186
 # PMID: 11589713
 
 
-start = {"sce": {"ATG": 1.000, "TTG": 0.069, "ATA": 0.005},
-         "eco": {}}
+start = {"sce": {"ATG": 1.000, "TTG": 0.069, "ATA": 0.005}, "eco": {}}
 
 
 # Zhang, S. P., Zubay, G., & Goldman, E. (1991).
 # Low-usage codons in Escherichia
 # coli, yeast, fruit fly and primates. Gene, 105(1), 61–72.
 # https://www.embl.de/pepcore/pepcore_services/cloning/choice_expression_systems/codons8
 # AGG ACG         CGA CGG CGC CCG CTC GCG
 
 
-rare_codons = {"sce": ["CGA", "CGG", "CGC", "CCG", "CTC", "GCG"],
-               "eco": ["AGG", "AGA", "ATA", "CTA", "CGA", "CGG",
-                       "CCC", "TCG"]}
-
-stop = {"sce": {"TAA": 0.470, "TAG": 0.230, "TGA": 0.300},  #
-        "eco": {}}
-
-
-n_end = {"sce": {"Val": ">30 h",
-                 "Met": ">30 h",
-                 "Gly": ">30 h",
-                 "Pro": ">5 h",
-                 "Ala": ">30 h",
-                 "Ser": ">30 h",
-                 "Thr": ">30 h",
-                 "Cys": ">30 h",
-                 "Ile": "30 min",
-                 "Glu": "30 min",
-                 "His": "3 min",
-                 "Tyr": "10 min",
-                 "Gln": "10 min",
-                 "Asp": "3 min",
-                 "Asn": "3 min",
-                 "Phe": "3 min",
-                 "Leu": "3 min",
-                 "Trp": "3 min",
-                 "Lys": "3 min",
-                 "Arg": "2 min"},
-         "eco": {}
-         }
+rare_codons = {
+    "sce": ["CGA", "CGG", "CGC", "CCG", "CTC", "GCG"],
+    "eco": ["AGG", "AGA", "ATA", "CTA", "CGA", "CGG", "CCC", "TCG"],
+}
+
+stop = {"sce": {"TAA": 0.470, "TAG": 0.230, "TGA": 0.300}, "eco": {}}  #
+
+
+n_end = {
+    "sce": {
+        "Val": ">30 h",
+        "Met": ">30 h",
+        "Gly": ">30 h",
+        "Pro": ">5 h",
+        "Ala": ">30 h",
+        "Ser": ">30 h",
+        "Thr": ">30 h",
+        "Cys": ">30 h",
+        "Ile": "30 min",
+        "Glu": "30 min",
+        "His": "3 min",
+        "Tyr": "10 min",
+        "Gln": "10 min",
+        "Asp": "3 min",
+        "Asn": "3 min",
+        "Phe": "3 min",
+        "Leu": "3 min",
+        "Trp": "3 min",
+        "Lys": "3 min",
+        "Arg": "2 min",
+    },
+    "eco": {},
+}
```

### Comparing `pydna-5.2.0a9/src/pydna/common_sub_strings.py` & `pydna-6.0.0a1/src/pydna/common_sub_strings.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,326 +8,320 @@
 """This module is based on the Py-rstr-max package that
 was written by Romain Brixtel (rbrixtel_at_gmail_dot_com)
 (https://brixtel.users.greyc.fr) and is available from
 https://code.google.com/p/py-rstr-max
 https://github.com/gip0/py-rstr-max
 the original code was covered by an MIT licence."""
 
-from array import array as _array
-import itertools as _itertools
-from operator import itemgetter as _itemgetter
-
-
-def radixpass(a, b, r, s, n, k):
-    c = _array("i", [0] * (k + 1))
-    for i in range(n):
-        c[r[a[i] + s]] += 1
-
-    somme = 0
-    for i in range(k + 1):
-        freq, c[i] = c[i], somme
-        somme += freq
-
-    for i in range(n):
-        b[c[r[a[i] + s]]] = a[i]
-        c[r[a[i] + s]] += 1
-
-
-def direct_kark_sort(s):
-    alphabet = [None] + sorted(set(s))
-    k = len(alphabet)
-    n = len(s)
-    t = dict((c, i) for i, c in enumerate(alphabet))
-    SA = _array("i", [0] * (n + 3))
-    kark_sort(_array("i", [t[c] for c in s] + [0] * 3), SA, n, k)
-    return SA[:n]
-
-
-def kark_sort(s, SA, n, K):
-    n0 = (n + 2) // 3
-    n1 = (n + 1) // 3
-    n2 = n // 3
-    n02 = n0 + n2
-
-    SA12 = _array("i", [0] * (n02 + 3))
-    SA0 = _array("i", [0] * n0)
-
-    s12 = [i for i in range(n + (n0 - n1)) if i % 3]
-    s12.extend([0] * 3)
-    s12 = _array("i", s12)
-
-    radixpass(s12, SA12, s, 2, n02, K)
-    radixpass(SA12, s12, s, 1, n02, K)
-    radixpass(s12, SA12, s, 0, n02, K)
-
-    name = 0
-    c0, c1, c2 = -1, -1, -1
-    for i in range(n02):
-        if s[SA12[i]] != c0 or s[SA12[i] + 1] != c1 or s[SA12[i] + 2] != c2:
-            name += 1
-            c0 = s[SA12[i]]
-            c1 = s[SA12[i] + 1]
-            c2 = s[SA12[i] + 2]
-        if SA12[i] % 3 == 1:
-            s12[SA12[i] // 3] = name
-        else:
-            s12[SA12[i] // 3 + n0] = name
-
-    if name < n02:
-        kark_sort(s12, SA12, n02, name + 1)
-        for i in range(n02):
-            s12[SA12[i]] = i + 1
-    else:
-        for i in range(n02):
-            SA12[s12[i] - 1] = i
-
-    s0 = _array("i", [SA12[i] * 3 for i in range(n02) if SA12[i] < n0])
-    radixpass(s0, SA0, s, 0, n0, K)
-
-    p = j = k = 0
-    t = n0 - n1
-    while k < n:
-        i = SA12[t] * 3 + 1 if SA12[t] < n0 else (SA12[t] - n0) * 3 + 2
-        j = SA0[p] if p < n0 else 0
-
-        if SA12[t] < n0:
-            test = (
-                (s12[SA12[t] + n0] <= s12[j // 3]) if (s[i] == s[j]) else (s[i] < s[j])
-            )
-        elif s[i] == s[j]:
-            test = (
-                s12[SA12[t] - n0 + 1] <= s12[j // 3 + n0]
-                if (s[i + 1] == s[j + 1])
-                else s[i + 1] < s[j + 1]
-            )
-        else:
-            test = s[i] < s[j]
-
-        if test:
-            SA[k] = i
-            t += 1
-            if t == n02:
-                k += 1
-                while p < n0:
-                    SA[k] = SA0[p]
-                    p += 1
-                    k += 1
-
-        else:
-            SA[k] = j
-            p += 1
-            if p == n0:
-                k += 1
-                while t < n02:
-                    SA[k] = (
-                        (SA12[t] * 3) + 1 if SA12[t] < n0 else ((SA12[t] - n0) * 3) + 2
-                    )
-                    t += 1
-                    k += 1
-        k += 1
-
-
-class Rstr_max:
-    def __init__(self):
-        self.array_str = []
-
-    def add_str(self, str_unicode):
-        self.array_str.append(str_unicode)
-
-    def step1_sort_suffix(self):
-        char_frontier = chr(2)
-
-        self.global_suffix = char_frontier.join(self.array_str)
-
-        nbChars = len(self.global_suffix)
-        init = [-1] * nbChars
-        self.idxString = _array("i", init)
-        self.idxPos = _array("i", init)
-        self.endAt = _array("i", init)
-
-        k = idx = 0
-        for mot in self.array_str:
-            last = k + len(mot)
-            for p in range(len(mot)):
-                self.idxString[k] = idx
-                self.idxPos[k] = p
-                self.endAt[k] = last
-                k += 1
-            idx += 1
-            k += 1
-
-        self.res = direct_kark_sort(self.global_suffix)
-
-    def step2_lcp(self):
-        n = len(self.res)
-        init = [0] * n
-        rank = _array("i", init)
-        LCP = _array("i", init)
-
-        s = self.global_suffix
-        suffix__array = self.res
-        endAt = self.endAt
-
-        for i in range(len(self.array_str), n):
-            v = self.res[i]
-            rank[v] = i
-
-        l = 0
-        for j in range(n):
-            if l > 0:
-                l -= 1
-            i = rank[j]
-            j2 = suffix__array[i - 1]
-            if i:
-                while l + j < endAt[j] and l + j2 < endAt[j2] and s[j + l] == s[j2 + l]:
-                    l += 1
-                LCP[i - 1] = l
-            else:
-                l = 0
-        self.lcp = LCP
-
-    def step3_rstr(self):
-        prev_len = 0
-        idx = 0
-        results = {}
-        len_lcp = len(self.lcp) - 1
-
-        class Stack:
-            pass
-
-        stack = Stack()
-        stack._top = 0
-        stack.lst_max = []
-
-        # if len(self.res) == 0 :
-        #  return {}
-
-        pos1 = self.res[0]
-        for idx in range(len_lcp):
-            current_len = self.lcp[idx]
-            pos2 = self.res[idx + 1]
-            end_ = max(pos1, pos2) + current_len
-            n = prev_len - current_len
-            if n < 0:
-                # pushMany
-                stack.lst_max.append([-n, idx, end_])
-                stack._top += -n
-            elif n > 0:
-                self.removeMany(stack, results, n, idx)
-            elif stack._top > 0 and end_ > stack.lst_max[-1][-1]:
-                # setMax
-                stack.lst_max[-1][-1] = end_
-
-            prev_len = current_len
-            pos1 = pos2
-
-        if stack._top > 0:
-            self.removeMany(stack, results, stack._top, idx + 1)
-
-        return results
-
-    def removeMany(self, stack, results, m, idxEnd):
-        prevStart = -1
-        while m > 0:
-            n, idxStart, maxEnd = stack.lst_max.pop()
-            if prevStart != idxStart:
-                # idStr = self.idxString[maxEnd-1]
-                # pos = self.idxPos[maxEnd-1]
-                id_ = (maxEnd, idxEnd - idxStart + 1)
-                if id_ not in results or results[id_][0] < stack._top:
-                    results[id_] = (stack._top, idxStart)
-                prevStart = idxStart
-            m -= n
-            stack._top -= n
-        if m < 0:
-            stack.lst_max.append([-m, idxStart, maxEnd - n - m])
-            stack._top -= m
-
-    def go(self):
-        self.step1_sort_suffix()
-        self.step2_lcp()
-        r = self.step3_rstr()
-        return r
-
-
-def common_sub_strings(stringx: str, stringy: str, limit=25):
-    """Finds all common substrings between stringx and stringy
-    longer than limit. This function is case sensitive.
-    The substrings may overlap.
-
-    returns a list of tuples describing the substrings
-    The list is sorted longest -> shortest.
-
-    Parameters
-    ----------
-    stringx : str
-    stringy : str
-    limit : int, optional
-
-    Returns
-    -------
-    list of tuple
-        [(startx1,starty1,length1),(startx2,starty2,length2), ...]
 
-        startx1 = startposition in x, where substring 1 starts
-        starty1 = position in y where substring 1 starts
-        length1 = lenght of substring
-
-
-    Examples
-    --------
-
-    >>> from pydna.common_sub_strings import common_sub_strings
-    >>> common_sub_strings("gatgatttcggtagtta", "gtcagtatgtctatctatcgcg", limit=3)
-    [(1, 6, 3), (7, 17, 3), (10, 4, 3), (12, 3, 3)]
+# from array import array as _array
+# import itertools as _itertools
+from operator import itemgetter as _itemgetter
 
-    ::
 
-        Overlaps   Symbols
-        (1, 6,  3)   ---
-        (7, 17, 3)   +++
-        (10, 4, 3)   ...
-        (12, 3, 3)   ===
+# def _kark_sort(s, SA, n, K):
+#     def radixpass(a, b, r, s, n, k):
+#         c = _array("i", [0] * (k + 1))
+#         for i in range(n):
+#             c[r[a[i] + s]] += 1
+
+#         somme = 0
+#         for i in range(k + 1):
+#             freq, c[i] = c[i], somme
+#             somme += freq
+
+#         for i in range(n):
+#             b[c[r[a[i] + s]]] = a[i]
+#             c[r[a[i] + s]] += 1
+
+#     n0 = (n + 2) // 3
+#     n1 = (n + 1) // 3
+#     n2 = n // 3
+#     n02 = n0 + n2
+
+#     SA12 = _array("i", [0] * (n02 + 3))
+#     SA0 = _array("i", [0] * n0)
+
+#     s12 = [i for i in range(n + (n0 - n1)) if i % 3]
+#     s12.extend([0] * 3)
+#     s12 = _array("i", s12)
+
+#     radixpass(s12, SA12, s, 2, n02, K)
+#     radixpass(SA12, s12, s, 1, n02, K)
+#     radixpass(s12, SA12, s, 0, n02, K)
+
+#     name = 0
+#     c0, c1, c2 = -1, -1, -1
+#     for i in range(n02):
+#         if s[SA12[i]] != c0 or s[SA12[i] + 1] != c1 or s[SA12[i] + 2] != c2:
+#             name += 1
+#             c0 = s[SA12[i]]
+#             c1 = s[SA12[i] + 1]
+#             c2 = s[SA12[i] + 2]
+#         if SA12[i] % 3 == 1:
+#             s12[SA12[i] // 3] = name
+#         else:
+#             s12[SA12[i] // 3 + n0] = name
+
+#     if name < n02:
+#         _kark_sort(s12, SA12, n02, name + 1)
+#         for i in range(n02):
+#             s12[SA12[i]] = i + 1
+#     else:
+#         for i in range(n02):
+#             SA12[s12[i] - 1] = i
+
+#     s0 = _array("i", [SA12[i] * 3 for i in range(n02) if SA12[i] < n0])
+#     radixpass(s0, SA0, s, 0, n0, K)
+
+#     p = j = k = 0
+#     t = n0 - n1
+#     while k < n:
+#         i = SA12[t] * 3 + 1 if SA12[t] < n0 else (SA12[t] - n0) * 3 + 2
+#         j = SA0[p] if p < n0 else 0
+
+#         if SA12[t] < n0:
+#             test = (s12[SA12[t] + n0] <= s12[j // 3]) if (s[i] == s[j]) else (s[i] < s[j])
+#         elif s[i] == s[j]:
+#             test = s12[SA12[t] - n0 + 1] <= s12[j // 3 + n0] if (s[i + 1] == s[j + 1]) else s[i + 1] < s[j + 1]
+#         else:
+#             test = s[i] < s[j]
+#         if test:
+#             SA[k] = i
+#             t += 1
+#             if t == n02:
+#                 k += 1
+#                 while p < n0:
+#                     SA[k] = SA0[p]
+#                     p += 1
+#                     k += 1
+#         else:
+#             SA[k] = j
+#             p += 1
+#             if p == n0:
+#                 k += 1
+#                 while t < n02:
+#                     SA[k] = (SA12[t] * 3) + 1 if SA12[t] < n0 else ((SA12[t] - n0) * 3) + 2
+#                     t += 1
+#                     k += 1
+#         k += 1
+
+
+# class _Rstr_max:
+#     def __init__(self):
+#         self.array_str = []
+
+#     def add_str(self, str_unicode):
+#         self.array_str.append(str_unicode)
+
+#     def _step1_sort_suffix(self):
+#         char_frontier = chr(2)
+
+#         self.global_suffix = char_frontier.join(self.array_str)
+
+#         nbChars = len(self.global_suffix)
+#         init = [-1] * nbChars
+#         self.idxString = _array("i", init)
+#         self.idxPos = _array("i", init)
+#         self.endAt = _array("i", init)
+
+#         k = idx = 0
+#         for mot in self.array_str:
+#             last = k + len(mot)
+#             for p in range(len(mot)):
+#                 self.idxString[k] = idx
+#                 self.idxPos[k] = p
+#                 self.endAt[k] = last
+#                 k += 1
+#             idx += 1
+#             k += 1
+
+#         s = self.global_suffix
+#         alphabet = [None] + sorted(set(s))
+#         k = len(alphabet)
+#         n = len(s)
+#         t = dict((c, i) for i, c in enumerate(alphabet))
+#         SA = _array("i", [0] * (n + 3))
+#         _kark_sort(_array("i", [t[c] for c in s] + [0] * 3), SA, n, k)
+#         self.res = SA[:n]
+
+#     def _step2_lcp(self):
+#         n = len(self.res)
+#         init = [0] * n
+#         rank = _array("i", init)
+#         LCP = _array("i", init)
+
+#         s = self.global_suffix
+#         suffix__array = self.res
+#         endAt = self.endAt
+
+#         for i in range(len(self.array_str), n):
+#             v = self.res[i]
+#             rank[v] = i
+
+#         l = 0
+#         for j in range(n):
+#             if l > 0:
+#                 l -= 1
+#             i = rank[j]
+#             j2 = suffix__array[i - 1]
+#             if i:
+#                 while l + j < endAt[j] and l + j2 < endAt[j2] and s[j + l] == s[j2 + l]:
+#                     l += 1
+#                 LCP[i - 1] = l
+#             else:
+#                 l = 0
+#         self.lcp = LCP
+
+#     def _step3_rstr(self):
+#         prev_len = 0
+#         idx = 0
+#         results = {}
+#         len_lcp = len(self.lcp) - 1
+
+#         class Stack:
+#             pass
+
+#         stack = Stack()
+#         stack._top = 0
+#         stack.lst_max = []
+
+#         # if len(self.res) == 0 :
+#         #  return {}
+
+#         pos1 = self.res[0]
+#         for idx in range(len_lcp):
+#             current_len = self.lcp[idx]
+#             pos2 = self.res[idx + 1]
+#             end_ = max(pos1, pos2) + current_len
+#             n = prev_len - current_len
+#             if n < 0:
+#                 # pushMany
+#                 stack.lst_max.append([-n, idx, end_])
+#                 stack._top += -n
+#             elif n > 0:
+#                 self.removeMany(stack, results, n, idx)
+#             elif stack._top > 0 and end_ > stack.lst_max[-1][-1]:
+#                 # setMax
+#                 stack.lst_max[-1][-1] = end_
+
+#             prev_len = current_len
+#             pos1 = pos2
+
+#         if stack._top > 0:
+#             self.removeMany(stack, results, stack._top, idx + 1)
+
+#         return results
+
+#     def removeMany(self, stack, results, m, idxEnd):
+#         prevStart = -1
+#         while m > 0:
+#             n, idxStart, maxEnd = stack.lst_max.pop()
+#             if prevStart != idxStart:
+#                 # idStr = self.idxString[maxEnd-1]
+#                 # pos = self.idxPos[maxEnd-1]
+#                 id_ = (maxEnd, idxEnd - idxStart + 1)
+#                 if id_ not in results or results[id_][0] < stack._top:
+#                     results[id_] = (stack._top, idxStart)
+#                 prevStart = idxStart
+#             m -= n
+#             stack._top -= n
+#         if m < 0:
+#             stack.lst_max.append([-m, idxStart, maxEnd - n - m])
+#             stack._top -= m
+
+#     def go(self):
+#         self._step1_sort_suffix()
+#         self._step2_lcp()
+#         return self._step3_rstr()
+
+
+# def common_sub_strings_py(stringx: str, stringy: str, limit=25):
+#     """Finds all common substrings between stringx and stringy
+#     longer than limit. This function is case sensitive.
+#     The substrings may overlap.
+
+#     returns a list of tuples describing the substrings
+#     The list is sorted longest -> shortest.
+
+#     Parameters
+#     ----------
+#     stringx : str
+#     stringy : str
+#     limit : int, optional
+
+#     Returns
+#     -------
+#     list of tuple
+#         [(startx1, starty1, length1),(startx2, starty2, length2), ...]
+
+#         startx1 = startposition in x, where substring 1 starts
+#         starty1 = position in y where substring 1 starts
+#         length1 = lenght of substring
+
+
+#     Examples
+#     --------
+
+#     >>> from pydna.common_sub_strings import common_sub_strings
+#     >>> common_sub_strings("gatgatttcggtagtta", "gtcagtatgtctatctatcgcg", limit=3)
+#     [(1, 6, 3), (7, 17, 3), (10, 4, 3), (12, 3, 3)]
+
+#     ::
+
+#         Overlaps   Symbols
+#         (1, 6,  3)   ---
+#         (7, 17, 3)   +++
+#         (10, 4, 3)   ...
+#         (12, 3, 3)   ===
+
+
+#                     ===
+#         gatgatttcggtagtta           stringx
+#          ---   +++...
+
+#             ...
+#         gtcagtatgtctatctatcgcg      stringy
+#            ===---        +++
+
+#     """
+#     rstr = _Rstr_max()
+#     rstr.add_str("&".join((stringx, stringy)))
+#     r = rstr.go()
+#     match = {}
+#     for (offset_end, nb), (l, start_plage) in r.items():
+#         if l < limit:
+#             continue
+#         startsx = []
+#         startsy = []
+#         for o in range(start_plage, start_plage + nb):
+#             offset = rstr.idxPos[rstr.res[o]]
+#             if offset > len(stringx):
+#                 startsy.append(offset - len(stringx) - 1)
+#             else:
+#                 startsx.append(offset)
+
+#         for a, b in _itertools.product(startsx, startsy):
+#             match[(a, b)] = max(match.get((a, b)) or 0, l)
 
+#     match = [(key[0], key[1], val) for key, val in list(match.items())]
 
-                    ===
-        gatgatttcggtagtta           stringx
-         ---   +++...
-
-            ...
-        gtcagtatgtctatctatcgcg      stringy
-           ===---        +++
+#     match.sort()
 
-    """
+#     match.sort(key=_itemgetter(2), reverse=True)
 
-    rstr = Rstr_max()
-    rstr.add_str(stringx + "&" + stringy)
-    r = rstr.go()
-    match = {}  # _defaultdict(int)
-    for (offset_end, nb), (l, start_plage) in r.items():
-        startsx = []
-        startsy = []
-        if l < limit:
-            continue
-        for o in range(start_plage, start_plage + nb):
-            offset = rstr.idxPos[rstr.res[o]]
-            if offset > len(stringx):
-                startsy.append(offset - len(stringx) - 1)
-            else:
-                startsx.append(offset)
+#     return match
 
-        for a, b in _itertools.product(startsx, startsy):
-            match[(a, b)] = max(match.get((a, b)) or 0, l)
 
-    match = [(key[0], key[1], val) for key, val in list(match.items())]
+def common_sub_strings(stringx: str, stringy: str, limit=25):
+    from pydivsufsort import common_substrings
 
+    match = common_substrings(stringx, stringy, limit=limit)
     match.sort()
-
     match.sort(key=_itemgetter(2), reverse=True)
-
     return match
 
 
 def terminal_overlap(stringx: str, stringy: str, limit=15):
     """Finds the the flanking common substrings between stringx and stringy
     longer than limit. This means that the results only contains substrings
     that starts or ends at the the ends of stringx and stringy.
@@ -368,16 +362,15 @@
                         gcatcgtagtctatttgcttac      stringy
                         0
 
     """
     return [
         m
         for m in common_sub_strings(stringx, stringy, limit)
-        if (m[0] == 0 and m[1] + m[2] == len(stringy))
-        or (m[1] == 0 and m[0] + m[2] == len(stringx))
+        if (m[0] == 0 and m[1] + m[2] == len(stringy)) or (m[1] == 0 and m[0] + m[2] == len(stringx))
     ]
 
 
 if __name__ == "__main__":
     import os as _os
 
     cached = _os.getenv("pydna_cached_funcs", "")
```

### Comparing `pydna-5.2.0a9/src/pydna/conftest.py` & `pydna-6.0.0a1/src/pydna/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """conftest.py"""
 
-#import pathlib
-#import os
+# import pathlib
+# import os
 
-#cwd = pathlib.Path(__file__).parent
+# cwd = pathlib.Path(__file__).parent
 
 # def pytest_runtest_setup(item):
 #     # called for running each test in 'a' directory
 #     #os.chdir(cwd)
 #     pass
 
 
-#def pytest_configure(config):
+# def pytest_configure(config):
 #    """
 #    Allows plugins and conftest files to perform initial configuration.
 #    This hook is called for every plugin and initial conftest
 #    file after command line options have been parsed.
 #    """
 #    os.chdir(cwd)
 #    print(f"cwd set to {cwd} in {__file__}")
```

### Comparing `pydna-5.2.0a9/src/pydna/contig.py` & `pydna-6.0.0a1/src/pydna/contig.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,43 +27,35 @@
     def from_SeqRecord(cls, record, *args, graph=None, nodemap=None, **kwargs):
         obj = super().from_SeqRecord(record, *args, **kwargs)
         obj.graph = graph
         obj.nodemap = nodemap
         return obj
 
     def __repr__(self):
-        return "Contig({}{})".format({True: "-", False: "o"}[self.linear], len(self))
+        return "Contig({}{})".format({True: "-", False: "o"}[not self.circular], len(self))
 
     def _repr_pretty_(self, p, cycle):
         """returns a short string representation of the object"""
-        p.text("Contig({}{})".format({True: "-", False: "o"}[self.linear], len(self)))
+        p.text("Contig({}{})".format({True: "-", False: "o"}[not self.circular], len(self)))
 
     def _repr_html_(self):
         return "<pre>" + self.figure() + "</pre>"
 
     def reverse_complement(self):
         answer = type(self)(super().reverse_complement())
         g = _nx.DiGraph()
         nm = self.nodemap
-        g.add_edges_from(
-            [(nm[v], nm[u], d) for u, v, d in list(self.graph.edges(data=True))[::-1]]
-        )
+        g.add_edges_from([(nm[v], nm[u], d) for u, v, d in list(self.graph.edges(data=True))[::-1]])
         g.add_nodes_from((nm[n], d) for n, d in list(self.graph.nodes(data=True))[::-1])
         for u, v, ed in g.edges(data=True):
-            ed["name"] = (
-                ed["name"][:-3]
-                if ed["name"].endswith("_rc")
-                else "{}_rc".format(ed["name"])[:13]
-            )
+            ed["name"] = ed["name"][:-3] if ed["name"].endswith("_rc") else "{}_rc".format(ed["name"])[:13]
             ed["seq"] = _rc(ed["seq"])
             ln = len(ed["seq"])
             start, stop = ed["piece"].start, ed["piece"].stop
-            ed["piece"] = slice(
-                ln - stop - g.nodes[u]["length"], ln - start - g.nodes[v]["length"]
-            )
+            ed["piece"] = slice(ln - stop - g.nodes[u]["length"], ln - start - g.nodes[v]["length"])
             ed["features"] = [f._flip(ln) for f in ed["features"]]
         answer.graph = g
         answer.nodemap = {v: k for k, v in self.nodemap.items()}
         return answer
 
     rc = reverse_complement
 
@@ -162,15 +154,15 @@
           --------------------------
 
 
         """
         nodes = list(self.graph.nodes(data=True))
         edges = list(self.graph.edges(data=True))
 
-        if self.linear:
+        if not self.circular:
             r"""
             frag20| 6
                    \/
                    /\
                     6|frag23| 6
                              \/
                              /\
@@ -183,36 +175,28 @@
 
             fig = ("{name}|{o2:>2}\n" "{space2} \\/\n" "{space2} /\\\n").format(
                 name=f[2]["name"], o2=nodes[1][1]["length"], space2=" " * space2
             )
             space = space2  # len(f.name)
 
             for i, f in enumerate(edges[1:-1]):
-                name = "{o1:>2}|{name}|".format(
-                    o1=nodes[i + 1][1]["length"], name=f[2]["name"]
-                )
+                name = "{o1:>2}|{name}|".format(o1=nodes[i + 1][1]["length"], name=f[2]["name"])
                 space2 = len(name)
 
-                fig += (
-                    "{space} {name}{o2:>2}\n"
-                    "{space} {space2}\\/\n"
-                    "{space} {space2}/\\\n"
-                ).format(
+                fig += ("{space} {name}{o2:>2}\n" "{space} {space2}\\/\n" "{space} {space2}/\\\n").format(
                     name=name,
                     o2=nodes[i + 2][1]["length"],
                     space=" " * space,
                     space2=" " * space2,
                 )
 
                 space += space2
 
             f = edges[-1]
-            fig += ("{space} {o1:>2}|{name}").format(
-                name=f[2]["name"], o1=nodes[-2][1]["length"], space=" " * (space)
-            )
+            fig += ("{space} {o1:>2}|{name}").format(name=f[2]["name"], o1=nodes[-2][1]["length"], space=" " * (space))
 
         else:  # circular
             r"""
              -|2577|61
             |       \/
             |       /\
             |       61|5681|98
@@ -232,33 +216,25 @@
             space = len(f[2]["name"]) + 3
 
             fig = (" -|{name}|{o2:>2}\n" "|{space}\\/\n" "|{space}/\\\n").format(
                 name=f[2]["name"], o2=nodes[1][1]["length"], space=" " * space
             )
 
             for i, f in enumerate(edges[1:]):
-                name = "{o1:>2}|{name}|".format(
-                    o1=nodes[i + 1][1]["length"], name=f[2]["name"]
-                )
+                name = "{o1:>2}|{name}|".format(o1=nodes[i + 1][1]["length"], name=f[2]["name"])
                 space2 = len(name)
-                fig += (
-                    "|{space}{name}{o2:>2}\n"
-                    "|{space}{space2}\\/\n"
-                    "|{space}{space2}/\\\n"
-                ).format(
+                fig += ("|{space}{name}{o2:>2}\n" "|{space}{space2}\\/\n" "|{space}{space2}/\\\n").format(
                     o2=nodes[i + 2][1]["length"],
                     name=name,
                     space=" " * space,
                     space2=" " * space2,
                 )
                 space += space2
 
-            fig += "|{space}{o1:>2}-\n".format(
-                space=" " * (space), o1=nodes[0][1]["length"]
-            )
+            fig += "|{space}{o1:>2}-\n".format(space=" " * (space), o1=nodes[0][1]["length"])
             fig += "|{space}   |\n".format(space=" " * (space))
             fig += " {space}".format(space="-" * (space + 3))
         return _pretty_str(_textwrap.dedent(fig))
 
 
 if __name__ == "__main__":
     import os as _os
```

### Comparing `pydna-5.2.0a9/src/pydna/design.py` & `pydna-6.0.0a1/src/pydna/design.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 from pydna.dseqrecord import Dseqrecord as _Dseqrecord
 from pydna.primer import Primer as _Primer
 import logging as _logging
 
 _module_logger = _logging.getLogger("pydna." + __name__)
 
 
-def primer_design(
-    template, fp=None, rp=None, limit=13, target_tm=55.0, tm_func=_tm_default, **kwargs
-):
+def primer_design(template, fp=None, rp=None, limit=13, target_tm=55.0, tm_func=_tm_default, **kwargs):
     """This function designs a forward primer and a reverse primer for PCR amplification
     of a given template sequence.
 
     The template argument is a Dseqrecord object or equivalent containing the template sequence.
 
     The optional fp and rp arguments can contain an existing primer for the sequence (either the forward or reverse primer).
     One or the other primers can be specified, not both (since then there is nothing to design!, use the pydna.amplify.pcr function instead).
@@ -116,49 +114,50 @@
     >>> ampl.forward_primer
     myprimer 27-mer:5'-atgactgctaaccct..ttg-3'
     >>> ampl.reverse_primer
     r64 37-mer:5'-catcgtaagtttcga..gtt-3'
     """
 
     def design(target_tm, template):
-        """ returns a string """
+        """returns a string"""
         tmp = 0
         length = limit
         p = str(template.seq[:length])
         while tmp < target_tm:
             length += 1
             p = str(template.seq[:length])
             tmp = tm_func(p)
         ps = p[:-1]
         tmps = tm_func(str(ps))
         _module_logger.debug(((p, tmp), (ps, tmps)))
         return min((abs(target_tm - tmp), p), (abs(target_tm - tmps), ps))[1]
+
     if not fp and not rp:
         _module_logger.debug("no primer given, design forward primer:")
         fp = _Primer((design(target_tm, template)))
         target_tm = tm_func(str(fp.seq))
         _module_logger.debug("no primer given, design reverse primer:")
         rp = _Primer(design(target_tm, template.reverse_complement()))
     elif fp and not rp:
         try:
             fp = _Anneal((fp,), template).forward_primers.pop()
         except IndexError:
             raise ValueError("Forward primer does not anneal")
-        except Exception: # pragma: no cover
+        except Exception:  # pragma: no cover
             print("Unexpected error")
             raise
         target_tm = tm_func(fp.footprint)
         _module_logger.debug("forward primer given, design reverse primer:")
         rp = _Primer(design(target_tm, template.reverse_complement()))
     elif not fp and rp:
         try:
             rp = _Anneal((rp,), template).reverse_primers.pop()
         except IndexError:
             raise ValueError("Reverse primer does not anneal")
-        except Exception: # pragma: no cover
+        except Exception:  # pragma: no cover
             print("Unexpected error")
             raise
         target_tm = tm_func(rp.footprint)
         _module_logger.debug("reverse primer given, design forward primer:")
         fp = _Primer(design(target_tm, template))
     else:
         raise ValueError("Specify maximum one of the two primers.")
@@ -182,17 +181,15 @@
 
     prod = ampl.products[0]
 
     if len(ampl.products) > 1:
         import warnings as _warnings
         from pydna import _PydnaWarning
 
-        _warnings.warn(
-            "designed primers do not yield a unique PCR product", _PydnaWarning
-        )
+        _warnings.warn("designed primers do not yield a unique PCR product", _PydnaWarning)
 
     return prod
 
 
 def assembly_fragments(f, overlap=35, maxlink=40):
     """This function return a list of :mod:`pydna.amplicon.Amplicon` objects where
     primers have been modified with tails so that the fragments can be fused in
@@ -203,24 +200,33 @@
 
     we can modify the reverse primer of a and forward primer of b with tails to allow
     fusion by fusion PCR, Gibson assembly or in-vivo homologous recombination.
     The basic requirements for the primers for the three techniques are the same.
 
     ::
 
-                                <-->
 
-       _________ a _________           __________ b ________
-      /                     \\         /                     \\
-      agcctatcatcttggtctctgca         TTTATATCGCATGACTCTTCTTT
-      |||||||||||||||||||||||         |||||||||||||||||||||||
-                       <gacgt                          <AGAAA
-      agcct>                          TTTAT>
-      |||||||||||||||||||||||         |||||||||||||||||||||||
-      tcggatagtagaaccagagacgt         AAATATAGCGTACTGAGAAGAAA
+
+            _________ a _________
+           /                     \\
+           agcctatcatcttggtctctgca
+                             |||||
+                            <gacgt
+           agcct>
+           |||||
+           tcggatagtagaaccagagacgt
+
+                                   __________ b ________
+                                  /                     \\
+                                  TTTATATCGCATGACTCTTCTTT
+                                                    |||||
+                                                   <AGAAA
+                                  TTTAT>
+                                  |||||
+                                  AAATATAGCGTACTGAGAAGAAA
 
 
            agcctatcatcttggtctctgcaTTTATATCGCATGACTCTTCTTT
            ||||||||||||||||||||||||||||||||||||||||||||||
            tcggatagtagaaccagagacgtAAATATAGCGTACTGAGAAGAAA
            \\___________________ c ______________________/
 
@@ -566,91 +572,71 @@
     |                    |
      --------------------
     >>>
 
     """
     # sanity check for arguments
     nf = [item for item in f if len(item) > maxlink]
-    if not all(
-        hasattr(i[0], "template") or hasattr(i[1], "template") for i in zip(nf, nf[1:])
-    ):
-        raise ValueError(
-            "Every second fragment larger than maxlink has to be an Amplicon object"
-        )
+    if not all(hasattr(i[0], "template") or hasattr(i[1], "template") for i in zip(nf, nf[1:])):
+        raise ValueError("Every second fragment larger than maxlink has to be an Amplicon object")
 
     _module_logger.debug("### assembly fragments ###")
     _module_logger.debug("overlap     = %s", overlap)
     _module_logger.debug("max_link    = %s", maxlink)
 
     f = [_copy.copy(f) for f in f]
 
     first_fragment_length = len(f[0])
     last_fragment_length = len(f[-1])
 
     if first_fragment_length <= maxlink:
         # first fragment should be removed and added to second fragment (new first fragment) forward primer
         f[1].forward_primer = f[0].seq._data.decode("ASCII") + f[1].forward_primer
-        _module_logger.debug(
-            "first fragment removed since len(f[0]) = %s", first_fragment_length
-        )
+        _module_logger.debug("first fragment removed since len(f[0]) = %s", first_fragment_length)
         f = f[1:]
     else:
-        _module_logger.debug(
-            "first fragment stays since len(f[0]) = %s", first_fragment_length
-        )
+        _module_logger.debug("first fragment stays since len(f[0]) = %s", first_fragment_length)
 
     if last_fragment_length <= maxlink:
-        f[-2].reverse_primer = (
-            f[-1].seq.reverse_complement()._data.decode("ASCII") + f[-2].reverse_primer
-        )
+        f[-2].reverse_primer = f[-1].seq.reverse_complement()._data.decode("ASCII") + f[-2].reverse_primer
         f = f[:-1]
-        _module_logger.debug(
-            "last fragment removed since len(f[%s]) = %s", len(f), last_fragment_length
-        )
+        _module_logger.debug("last fragment removed since len(f[%s]) = %s", len(f), last_fragment_length)
     else:
-        _module_logger.debug(
-            "last fragment stays since len(f[%s]) = %s", len(f), last_fragment_length
-        )
+        _module_logger.debug("last fragment stays since len(f[%s]) = %s", len(f), last_fragment_length)
 
     empty = _Dseqrecord("")
 
     _module_logger.debug(f)
 
     _module_logger.debug("loop through fragments in groups of three:")
 
     tail_length = _math.ceil(overlap / 2)
 
     for i in range(len(f) - 1):
-
         first = f[i]
         secnd = f[i + 1]
 
         secnd_len = len(secnd)
 
         _module_logger.debug("first = %s", str(first.seq))
         _module_logger.debug("secnd = %s", str(secnd.seq))
 
         if secnd_len <= maxlink:
-            _module_logger.debug(
-                "secnd is smaller or equal to maxlink; should be added to primer(s)"
-            )
+            _module_logger.debug("secnd is smaller or equal to maxlink; should be added to primer(s)")
             third = f[i + 2]
             _module_logger.debug("third = %s", str(third.seq))
             if hasattr(f[i], "template") and hasattr(third, "template"):
                 _module_logger.debug(
                     "secnd is is flanked by amplicons, so half of secnd should be added each flanking primers"
                 )
 
                 first.reverse_primer = (
-                    secnd.seq.reverse_complement()._data.decode("ASCII")[secnd_len // 2 :]
-                    + first.reverse_primer
-                )
-                third.forward_primer = (
-                    secnd.seq._data.decode("ASCII")[secnd_len // 2 :] + third.forward_primer
+                    secnd.seq.reverse_complement()._data.decode("ASCII")[secnd_len // 2 :] + first.reverse_primer
                 )
+                third.forward_primer = secnd.seq._data.decode("ASCII")[secnd_len // 2 :] + third.forward_primer
 
                 lnk = (
                     third.seq.reverse_complement()._data.decode("ASCII")
                     + secnd.reverse_complement().seq._data.decode("ASCII")[: secnd_len // 2]
                 )[-tail_length:]
                 _module_logger.debug("1 %s", lnk)
                 first.reverse_primer = lnk + first.reverse_primer
@@ -658,17 +644,15 @@
                 lnk = (first.seq._data.decode("ASCII") + secnd.seq._data.decode("ASCII")[: secnd_len // 2])[
                     -tail_length:
                 ]
                 _module_logger.debug("2 %s", lnk)
                 third.forward_primer = lnk + third.forward_primer
 
             elif hasattr(first, "template"):
-                first.reverse_primer = (
-                    secnd.seq.reverse_complement()._data.decode("ASCII") + first.reverse_primer
-                )
+                first.reverse_primer = secnd.seq.reverse_complement()._data.decode("ASCII") + first.reverse_primer
                 lnk = str(third.seq[:overlap].reverse_complement())
                 first.reverse_primer = lnk + first.reverse_primer
             elif hasattr(third, "template"):
                 third.forward_primer = secnd.seq._data.decode("ASCII") + third.forward_primer
                 lnk = str(first.seq[-overlap:])
                 third.forward_primer = lnk + third.forward_primer
             secnd = empty
@@ -693,29 +677,26 @@
         f[i + 1] = secnd
 
     _module_logger.debug("loop ended")
 
     f = [item for item in f if len(item)]
 
     return [
-        _pcr(p.forward_primer, p.reverse_primer, p.template)
+        _pcr(p.forward_primer, p.reverse_primer, p.template, limit=min((p.forward_primer._fp, p.reverse_primer._fp)))
         if hasattr(p, "template")
         else p
         for p in f
     ]
 
 
 def circular_assembly_fragments(f, overlap=35, maxlink=40):
-
     fragments = assembly_fragments(f + f[0:1], overlap=overlap, maxlink=maxlink)
 
     if hasattr(fragments[0], "template"):
-        fragments[0] = _pcr(
-            (fragments[-1].forward_primer, fragments[0].reverse_primer), fragments[0]
-        )
+        fragments[0] = _pcr((fragments[-1].forward_primer, fragments[0].reverse_primer), fragments[0])
     return fragments[:-1]
 
 
 if __name__ == "__main__":
     import os as _os
 
     cached = _os.getenv("pydna_cached_funcs", "")
```

### Comparing `pydna-5.2.0a9/src/pydna/download.py` & `pydna-6.0.0a1/src/pydna/download.py`

 * *Files identical despite different names*

### Comparing `pydna-5.2.0a9/src/pydna/dseq.py` & `pydna-6.0.0a1/src/pydna/dseq.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,21 +156,18 @@
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
       File "/usr/local/lib/python2.7/dist-packages/pydna_/dsdna.py", line 169, in __init__
         else:
     ValueError: ovhg defined without crick strand!
 
 
-    The shape of the fragment is set by either:
-
-    1. linear   = False, True
-    2. circular = True, False
+    The shape of the fragment is set by circular = True, False
 
     Note that both ends of the DNA fragment has to be compatible to set
-    circular = True (or linear = False).
+    circular = True.
 
 
     >>> Dseq("aaa","ttt")
     Dseq(-3)
     aaa
     ttt
     >>> Dseq("aaa","ttt",ovhg=0)
@@ -181,18 +178,14 @@
     Dseq(-4)
      aaa
     ttt
     >>> Dseq("aaa","ttt",ovhg=-1)
     Dseq(-4)
     aaa
      ttt
-    >>> Dseq("aaa", "ttt", linear = False ,ovhg=0)
-    Dseq(o3)
-    aaa
-    ttt
     >>> Dseq("aaa", "ttt", circular = True , ovhg=0)
     Dseq(o3)
     aaa
     ttt
 
     >>> a=Dseq("tttcccc","aaacccc")
     >>> a
@@ -236,15 +229,15 @@
     >>> s[2:4]
     'at'
     >>> s[2:4:-1]
     ''
     >>> s[::2]
     'gac'
     >>> from pydna.dseq import Dseq
-    >>> d=Dseq(s, linear=True)
+    >>> d=Dseq(s, circular=False)
     >>> d[2:3]
     Dseq(-1)
     a
     t
     >>> d[2:4]
     Dseq(-2)
     at
@@ -294,193 +287,190 @@
     --------
     pydna.dseqrecord.Dseqrecord
 
     """
 
     trunc = 30
 
-    def __init__(self,
-                 watson,
-                 crick=None,
-                 ovhg=None,
-                 linear=None,
-                 circular=None,
-                 pos=0):
-
+    def __init__(
+        self,
+        watson,
+        crick=None,
+        ovhg=None,
+        # linear=None,
+        circular=False,
+        pos=0,
+    ):
         if crick is None:
             if ovhg is None:
                 crick = _rc(watson)
                 ovhg = 0
                 try:
                     self._data = bytes(watson, encoding="ASCII")
                 except TypeError:
                     self._data = watson
                     watson = watson.decode("ASCII")
                     crick = crick.decode("ASCII")
             else:  # ovhg given, but no crick strand
                 raise ValueError("ovhg defined without crick strand!")
         else:  # crick strand given
             if ovhg is None:  # ovhg not given
-
                 olaps = _common_sub_strings(
                     str(watson).lower(),
                     str(_rc(crick).lower()),
                     int(_math.log(len(watson)) / _math.log(4)),
                 )
                 try:
                     F, T, L = olaps[0]
                 except IndexError:
-                    raise ValueError("Could not anneal the two strands."
-                                     " Please provide ovhg value")
+                    raise ValueError("Could not anneal the two strands." " Please provide ovhg value")
                 ovhgs = [ol[1] - ol[0] for ol in olaps if ol[2] == L]
                 if len(ovhgs) > 1:
-                    raise ValueError("More than one way of annealing the"
-                                     " strands. Please provide ovhg value")
+                    raise ValueError("More than one way of annealing the" " strands. Please provide ovhg value")
                 ovhg = T - F
 
                 sns = (ovhg * " ") + _pretty_str(watson)
                 asn = (-ovhg * " ") + _pretty_str(_rc(crick))
 
-                self._data = bytes("".join(
-                    [
-                        a.strip() or b.strip()
-                        for a, b in _itertools.zip_longest(sns, asn, fillvalue=" ")
-                    ]
-                ), encoding="ASCII")
+                self._data = bytes(
+                    "".join([a.strip() or b.strip() for a, b in _itertools.zip_longest(sns, asn, fillvalue=" ")]),
+                    encoding="ASCII",
+                )
 
             else:  # ovhg given
                 if ovhg == 0:
                     if len(watson) == len(crick):
                         self._data = bytes(watson, encoding="ASCII")
                     elif len(watson) > len(crick):
                         self._data = bytes(watson, encoding="ASCII")
                     else:
-                        self._data = bytes(watson + _rc(crick[: len(crick) - len(watson)]),encoding="ASCII")
+                        self._data = bytes(watson + _rc(crick[: len(crick) - len(watson)]), encoding="ASCII")
                 elif ovhg > 0:
                     if ovhg + len(watson) > len(crick):
                         self._data = bytes(_rc(crick[-ovhg:]) + watson, encoding="ASCII")
                     else:
                         self._data = bytes(
-                            _rc(crick[-ovhg:])
-                            + watson
-                            + _rc(crick[: len(crick) - ovhg - len(watson)]),
-                            encoding="ASCII")
+                            _rc(crick[-ovhg:]) + watson + _rc(crick[: len(crick) - ovhg - len(watson)]),
+                            encoding="ASCII",
+                        )
                 else:  # ovhg < 0
                     if -ovhg + len(crick) > len(watson):
-                        self._data = bytes(watson + _rc(
-                            crick[: -ovhg + len(crick) - len(watson)]
-                        ), encoding="ASCII")
+                        self._data = bytes(watson + _rc(crick[: -ovhg + len(crick) - len(watson)]), encoding="ASCII")
                     else:
                         self._data = bytes(watson, encoding="ASCII")
 
-        self._circular = (bool(circular)
-                          and bool(linear) ^ bool(circular)
-                          or linear is False
-                          and circular is None)
+        # self._circular = (bool(circular)
+        #                   and bool(linear) ^ bool(circular)
+        #                   or linear is False
+        #                   and circular is None)
 
-        self._linear = not self._circular
+        # self._linear = not self._circular
+        self.circular = circular
         self.watson = _pretty_str(watson)
         self.crick = _pretty_str(crick)
         self.length = len(self._data)
         self._ovhg = ovhg
         self.pos = pos
 
     @classmethod
-    def quick(cls, watson: str, crick: str, ovhg=0,
-              linear=True, circular=False, pos=0):
+    def quick(
+        cls,
+        watson: str,
+        crick: str,
+        ovhg=0,
+        # linear=True,
+        circular=False,
+        pos=0,
+    ):
         obj = cls.__new__(cls)  # Does not call __init__
         obj.watson = _pretty_str(watson)
         obj.crick = _pretty_str(crick)
         obj._ovhg = ovhg
-        obj._circular = circular
-        obj._linear = linear
-        obj.length = max(len(watson) + max(0, ovhg),
-                         len(crick) + max(0, -ovhg))
+        obj.circular = circular
+        # obj._linear = linear
+        obj.length = max(len(watson) + max(0, ovhg), len(crick) + max(0, -ovhg))
         obj.pos = pos
         wb = bytes(watson, encoding="ASCII")
         cb = bytes(crick, encoding="ASCII")
-        obj._data = (
-            _rc(cb[-max(0, ovhg) or len(cb):])
-            + wb
-            + _rc(cb[: max(0, len(cb) - ovhg - len(wb))]))
+        obj._data = _rc(cb[-max(0, ovhg) or len(cb) :]) + wb + _rc(cb[: max(0, len(cb) - ovhg - len(wb))])
         return obj
 
     @classmethod
-    def from_string(cls, dna: str, *args, linear=True, circular=False, **kwargs):
+    def from_string(
+        cls,
+        dna: str,
+        *args,
+        # linear=True,
+        circular=False,
+        **kwargs
+    ):
         obj = cls.__new__(cls)  # Does not call __init__
         obj.watson = _pretty_str(dna)
         obj.crick = _pretty_str(_rc(dna))
         obj._ovhg = 0
-        obj._circular = circular
-        obj._linear = linear
+        obj.circular = circular
+        # obj._linear = linear
         obj.length = len(dna)
         obj.pos = 0
         obj._data = bytes(dna, encoding="ASCII")
-        # obj.alphabet = _generic_dna
         return obj
 
     @classmethod
-    def from_representation(cls,
-                            dsdna: str,
-                            *args,
-                            **kwargs):
+    def from_representation(cls, dsdna: str, *args, **kwargs):
         obj = cls.__new__(cls)  # Does not call __init__
         w, c, *r = [ln for ln in dsdna.splitlines() if ln]
-        ovhg = obj._ovhg = len(w)-len(w.lstrip()) - (len(c) - len(c.lstrip()))
+        ovhg = obj._ovhg = len(w) - len(w.lstrip()) - (len(c) - len(c.lstrip()))
         watson = obj.watson = _pretty_str(w.strip())
         crick = obj.crick = _pretty_str(c.strip()[::-1])
-        obj._circular = False
-        obj._linear = True
-        obj.length = max(len(watson) + max(0, ovhg),
-                         len(crick) + max(0, -ovhg))
+        obj.circular = False
+        # obj._linear = True
+        obj.length = max(len(watson) + max(0, ovhg), len(crick) + max(0, -ovhg))
         obj.pos = 0
         wb = bytes(watson, encoding="ASCII")
         cb = bytes(crick, encoding="ASCII")
-        obj._data = (
-            _rc(cb[-max(0, ovhg) or len(cb):])
-            + wb
-            + _rc(cb[: max(0, len(cb) - ovhg - len(wb))]))
+        obj._data = _rc(cb[-max(0, ovhg) or len(cb) :]) + wb + _rc(cb[: max(0, len(cb) - ovhg - len(wb))])
         return obj
 
     @property
     def ovhg(self):
         """The ovhg property. This cannot be set directly, but is a
         consequence of how the watson and crick strands anneal to
         each other"""
         return self._ovhg
 
-    @property
-    def linear(self):
-        """The linear property can not be set directly.
-        Use an empty slice [:] to create a linear object."""
-        return self._linear
-
-    @property
-    def circular(self):
-        """The circular property can not be set directly.
-        Use :meth:`looped` to create a circular Dseq object"""
-        return self._circular
+    # @property
+    # def linear(self):
+    #     """The linear property can not be set directly.
+    #     Use an empty slice [:] to create a linear object."""
+    #     return self._linear
+
+    # @property
+    # def circular(self):
+    #     """The circular property can not be set directly.
+    #     Use :meth:`looped` to create a circular Dseq object"""
+    #     return self._circular
 
     def mw(self):
         """This method returns the molecular weight of the DNA molecule
         in g/mol. The following formula is used::
 
                MW = (A x 313.2) + (T x 304.2) +
                     (C x 289.2) + (G x 329.2) +
                     (N x 308.9) + 79.0
         """
         nts = (self.watson + self.crick).lower()
 
-        return ( 313.2 * nts.count("a") +
-                 304.2 * nts.count("t") +
-                 289.2 * nts.count("c") +
-                 329.2 * nts.count("g") +
-                 308.9 * nts.count("n") +
-                 79.0 )
-
+        return (
+            313.2 * nts.count("a")
+            + 304.2 * nts.count("t")
+            + 289.2 * nts.count("c")
+            + 329.2 * nts.count("g")
+            + 308.9 * nts.count("n")
+            + 79.0
+        )
 
     def upper(self):
         """Return an upper case copy of the sequence.
 
         >>> from pydna.dseq import Dseq
         >>> my_seq = Dseq("aAa")
         >>> my_seq
@@ -502,15 +492,15 @@
         pydna.dseq.Dseq.lower
 
         """
         return self.quick(
             self.watson.upper(),
             self.crick.upper(),
             ovhg=self.ovhg,
-            linear=self.linear,
+            # linear=self.linear,
             circular=self.circular,
             pos=self.pos,
         )
 
     def lower(self):
         """Return a lower case copy of the sequence.
 
@@ -534,15 +524,15 @@
         --------
         pydna.dseq.Dseq.upper
         """
         return self.quick(
             self.watson.lower(),
             self.crick.lower(),
             ovhg=self.ovhg,
-            linear=self.linear,
+            # linear=self.linear,
             circular=self.circular,
             pos=self.pos,
         )
 
     def find(self, sub, start=0, end=_sys.maxsize):
         """This method behaves like the python string method of the same name.
 
@@ -578,60 +568,59 @@
         Dseq(-7)
         agt
           attca
         >>> seq.find("taa")
         2
         """
 
-        if self.linear:
+        if not self.circular:
             return _Seq.find(self, sub, start, end)
 
         return (_pretty_str(self) + _pretty_str(self)).find(sub, start, end)
 
     def __getitem__(self, sl):
         """Returns a subsequence. This method is used by the slice notation"""
 
-        if self.linear:
-
+        if not self.circular:
             x = len(self.crick) - self._ovhg - len(self.watson)
 
             sns = (self._ovhg * " " + self.watson + x * " ")[sl]
             asn = (-self._ovhg * " " + self.crick[::-1] + -x * " ")[sl]
 
-            ovhg = max(
-                (len(sns) - len(sns.lstrip()), -len(asn) + len(asn.lstrip())), key=abs
-            )
+            ovhg = max((len(sns) - len(sns.lstrip()), -len(asn) + len(asn.lstrip())), key=abs)
 
-            return Dseq(sns.strip(), asn[::-1].strip(), ovhg=ovhg, linear=True)
+            return Dseq(
+                sns.strip(),
+                asn[::-1].strip(),
+                ovhg=ovhg,
+                # linear=True
+            )
         else:
             sl = slice(sl.start or 0, sl.stop or len(self), sl.step)
             if sl.start > len(self) or sl.stop > len(self):
                 return Dseq("")
             if sl.start < sl.stop:
                 return Dseq(
-                    self.watson[sl], self.crick[::-1][sl][::-1], ovhg=0, linear=True
+                    self.watson[sl],
+                    self.crick[::-1][sl][::-1],
+                    ovhg=0,
+                    # linear=True
                 )
             else:
                 try:
                     stp = abs(sl.step)
                 except TypeError:
                     stp = 1
                 start = sl.start
                 stop = sl.stop
 
-                w = (
-                    self.watson[(start or len(self)) :: stp]
-                    + self.watson[: (stop or 0) : stp]
-                )
-                c = (
-                    self.crick[len(self) - stop :: stp]
-                    + self.crick[: len(self) - start : stp]
-                )
+                w = self.watson[(start or len(self)) :: stp] + self.watson[: (stop or 0) : stp]
+                c = self.crick[len(self) - stop :: stp] + self.crick[: len(self) - start : stp]
 
-                return Dseq(w, c, ovhg=0, linear=True)
+                return Dseq(w, c, ovhg=0)  # , linear=True)
 
     def __eq__(self, other):
         """Compare to another Dseq object OR an object that implements
         watson, crick and ovhg properties. This comparison is case
         insensitive.
 
         """
@@ -648,17 +637,16 @@
         return same
 
     def __repr__(self):
         """Returns a representation of the sequence, truncated if
         longer than 30 bp"""
 
         if len(self) > Dseq.trunc:
-
             if self._ovhg > 0:
-                d = self.crick[-self._ovhg:][::-1]
+                d = self.crick[-self._ovhg :][::-1]
                 hej = len(d)
                 if len(d) > 10:
                     d = "{}..{}".format(d[:4], d[-4:])
                 a = len(d) * " "
 
             elif self._ovhg < 0:
                 a = self.watson[: max(0, -self._ovhg)]
@@ -670,15 +658,15 @@
                 a = ""
                 d = ""
                 hej = 0
 
             x = self._ovhg + len(self.watson) - len(self.crick)
 
             if x > 0:
-                c = self.watson[len(self.crick) - self._ovhg:]
+                c = self.watson[len(self.crick) - self._ovhg :]
                 y = len(c)
                 if len(c) > 10:
                     c = "{}..{}".format(c[:4], c[-4:])
                 f = len(c) * " "
             elif x < 0:
                 f = self.crick[:-x][::-1]
                 y = len(f)
@@ -699,33 +687,31 @@
             b = self.watson[x1:x2]
             e = self.crick[x3:x4][::-1]
 
             if len(b) > 10:
                 b = "{}..{}".format(b[:4], b[-4:])
                 e = "{}..{}".format(e[:4], e[-4:])
 
-            return _pretty_str(
-                "{klass}({top}{size})\n" "{a}{b}{c}\n" "{d}{e}{f}"
-            ).format(
+            return _pretty_str("{klass}({top}{size})\n" "{a}{b}{c}\n" "{d}{e}{f}").format(
                 klass=self.__class__.__name__,
-                top={True: "-", False: "o"}[self.linear],
+                top={False: "-", True: "o"}[self.circular],
                 size=len(self),
                 a=a,
                 b=b,
                 c=c,
                 d=d,
                 e=e,
                 f=f,
             )
 
         else:
             return _pretty_str(
                 "{}({}{})\n{}\n{}".format(
                     self.__class__.__name__,
-                    {True: "-", False: "o"}[self.linear],
+                    {False: "-", True: "o"}[self.circular],
                     len(self),
                     self._ovhg * " " + self.watson,
                     -self._ovhg * " " + self.crick[::-1],
                 )
             )
 
     def reverse_complement(self, inplace=False):
@@ -750,23 +736,23 @@
 
         """
         ovhg = len(self.watson) - len(self.crick) + self._ovhg
         return Dseq.quick(
             self.crick,
             self.watson,
             ovhg=ovhg,
-            linear=self.linear,
+            # linear=self.linear,
             circular=self.circular,
         )
 
     rc = reverse_complement  # alias for reverse_complement
 
     def shifted(self, shift):
         """Shifted version of a circular Dseq object."""
-        if self.linear:
+        if not self.circular:
             raise TypeError("DNA is not circular.")
         shift = shift % len(self)
         if not shift:
             return self
         else:
             return (self[shift:] + self[:shift]).looped()
 
@@ -815,23 +801,21 @@
         type5, sticky5 = self.five_prime_end()
         type3, sticky3 = self.three_prime_end()
         if type5 == type3 and str(sticky5) == str(_rc(sticky3)):
             nseq = Dseq.quick(
                 self.watson,
                 self.crick[-self._ovhg :] + self.crick[: -self._ovhg],
                 ovhg=0,
-                linear=False,
+                # linear=False,
                 circular=True,
             )
-            assert len(nseq.crick) == len(nseq.watson)
+            # assert len(nseq.crick) == len(nseq.watson)
             return nseq
         else:
-            raise TypeError(
-                "DNA cannot be circularized.\n" "5' and 3' sticky ends not compatible!"
-            )
+            raise TypeError("DNA cannot be circularized.\n" "5' and 3' sticky ends not compatible!")
 
     def tolinear(self):  # pragma: no cover
         """Returns a blunt, linear copy of a circular Dseq object. This can
         only be done if the Dseq object is circular, otherwise a
         TypeError is raised.
 
         This method is deprecated, use slicing instead. See example below.
@@ -852,24 +836,21 @@
         >>>
 
         """
         import warnings as _warnings
         from pydna import _PydnaDeprecationWarning
 
         _warnings.warn(
-            "tolinear method is obsolete; "
-            "please use obj[:] "
-            "instead of obj.tolinear().",
+            "tolinear method is obsolete; " "please use obj[:] " "instead of obj.tolinear().",
             _PydnaDeprecationWarning,
         )
-        if self.linear:
+        if not self.circular:
             raise TypeError("DNA is not circular.\n")
         selfcopy = _copy.copy(self)
-        selfcopy._linear = True
-        selfcopy._circular = False
+        selfcopy.circular = False
         return selfcopy  # self.__class__(self.watson, linear=True)
 
     def five_prime_end(self):
         """Returns a tuple describing the structure of the 5' end of
         the DNA fragment
 
         Examples
@@ -907,15 +888,15 @@
             return "5'", self.watson.lower()
         if not self.watson and self.crick:
             return "3'", self.crick.lower()
         if self._ovhg < 0:
             sticky = self.watson[: -self._ovhg].lower()
             type_ = "5'"
         elif self._ovhg > 0:
-            sticky = self.crick[-self._ovhg:].lower()
+            sticky = self.crick[-self._ovhg :].lower()
             type_ = "3'"
         else:
             sticky = ""
             type_ = "blunt"
         return type_, sticky
 
     def three_prime_end(self):
@@ -992,34 +973,26 @@
         except AttributeError:
             pass
 
         self_type, self_tail = self.three_prime_end()
         other_type, other_tail = other.five_prime_end()
 
         if self_type == other_type and str(self_tail) == str(_rc(other_tail)):
-            answer = Dseq.quick(
-                self.watson + other.watson,
-                other.crick + self.crick,
-                self._ovhg
-            )
+            answer = Dseq.quick(self.watson + other.watson, other.crick + self.crick, self._ovhg)
         elif not self:
             answer = _copy.copy(other)
         elif not other:
             answer = _copy.copy(self)
         else:
             raise TypeError("sticky ends not compatible!")
         return answer
 
     def __mul__(self, number):
         if not isinstance(number, int):
-            raise TypeError(
-                "TypeError: can't multiply Dseq by non-int of type {}".format(
-                    type(number)
-                )
-            )
+            raise TypeError("TypeError: can't multiply Dseq by non-int of type {}".format(type(number)))
         if number <= 0:
             return self.__class__("")
         new = _copy.copy(self)
         for i in range(number - 1):
             new += self
         return new
 
@@ -1108,16 +1081,15 @@
         crick, ovhg = self._fill_in_five_prime(nucleotides)
         watson = self._fill_in_three_prime(nucleotides)
         return Dseq(watson, crick, ovhg)
 
     def transcribe(self):
         return _Seq(self.watson).transcribe()
 
-    def translate(self, table="Standard", stop_symbol="*",
-                  to_stop=False, cds=False, gap="-"):
+    def translate(self, table="Standard", stop_symbol="*", to_stop=False, cds=False, gap="-"):
         return _Seq(_translate_str(str(self), table, stop_symbol, to_stop, cds, gap=gap))
 
     def mung(self):
         """
         Simulates treatment a nuclease with 5'-3' and 3'-5' single
         strand specific exonuclease activity (such as mung bean nuclease [#]_)
 
@@ -1153,19 +1125,15 @@
 
         References
         ----------
         .. [#] http://en.wikipedia.org/wiki/Mung_bean_nuclease
 
 
         """
-        return Dseq(
-            self.watson[
-                max(0, -self.ovhg) : min(len(self.watson), len(self.crick) - self.ovhg)
-            ]
-        )
+        return Dseq(self.watson[max(0, -self.ovhg) : min(len(self.watson), len(self.crick) - self.ovhg)])
 
     def T4(self, nucleotides=None):
         """Fill in five prime protruding ends and chewing back
         three prime protruding ends by a DNA polymerase providing both
         5'-3' DNA polymerase activity and 3'-5' nuclease acitivty
         (such as T4 DNA polymerase). This can be done in presence of any
         combination of the four A, G, C or T. Removing one or more nucleotides
@@ -1281,15 +1249,15 @@
             batch = CommOnly
         ana = batch.search(self)
         ncut = {enz: sitelist for (enz, sitelist) in ana.items() if sitelist}
         return _RestrictionBatch(ncut)
 
     def cseguid(self):
         """Circular uSEGUID (cSEGUID) for the sequence."""
-        if self.linear:
+        if not self.circular:
             raise TypeError("cseguid is only defined for circular sequences.")
         return _cseg(str(self.watson))
 
     def lseguid(self):
         """Linear uSEGUID (lSEGUID) for the sequence."""
         if self.circular:
             raise TypeError("lseguid is only defined for linear sequences.")
@@ -1329,35 +1297,33 @@
         >>> a
         Dseq(o3)
         gat
         cta
         >>> a.isblunt()
         False
         """
-        return self._ovhg == 0 and len(self.watson) == len(self.crick) and self._linear
+        return self._ovhg == 0 and len(self.watson) == len(self.crick) and not self.circular
 
     def cas9(self, RNA: str):
         """docstring."""
         bRNA = bytes(RNA, "ASCII")
         slices = []
         cuts = [0]
         for m in _re.finditer(bRNA, self._data):
-            cuts.append(m.start()+17)
+            cuts.append(m.start() + 17)
         cuts.append(self.length)
         slices = tuple(slice(x, y, 1) for x, y in zip(cuts, cuts[1:]))
         return slices
 
     def terminal_transferase(self, nucleotides="a"):
         """docstring."""
         ovhg = self.ovhg
         if self.ovhg >= 0:
             ovhg += len(nucleotides)
-        return Dseq(self.watson + nucleotides,
-                    self.crick + nucleotides,
-                    ovhg)
+        return Dseq(self.watson + nucleotides, self.crick + nucleotides, ovhg)
 
     def cut(self, *enzymes):
         """Returns a list of linear Dseq fragments produced in the digestion.
         If there are no cuts, an empty list is returned.
 
         Parameters
         ----------
@@ -1399,93 +1365,103 @@
         cctaggnnncttaag
         >>>
 
         """
 
         pad = "n" * 50
 
-        if self.linear:
-            dsseq = self.mung()
+        if self.circular:
+            dsseq = Dseq.from_string(
+                self._data.decode("ASCII"),
+                # linear=True,
+                circular=False,
+            )
         else:
-            dsseq = Dseq.from_string(self._data.decode("ASCII"),
-                                     linear=True,
-                                     circular=False)
+            dsseq = self.mung()
+
         if len(enzymes) == 1 and hasattr(enzymes[0], "intersection"):
             # argument is probably a RestrictionBatch
             enzymecuts = []
             for e in enzymes[0]:
-                cuts = e.search(
-                    _Seq(pad + dsseq.watson + dsseq.watson[:e.size-1] + pad)
-                    if self.circular
-                    else dsseq)
+                cuts = e.search(_Seq(pad + dsseq.watson + dsseq.watson[: e.size - 1] + pad) if self.circular else dsseq)
                 enzymecuts.append((cuts, e))
             enzymecuts.sort()
             enzymes = [e for (c, e) in enzymecuts if c]
         else:
             # argument is probably a list of restriction enzymes
             enzymes = [
                 e
                 for e in list(dict.fromkeys(_flatten(enzymes)))
-                if e.search(
-                    _Seq(pad + dsseq.watson + dsseq.watson[: e.size - 1] + pad)
-                    if self.circular
-                    else dsseq
-                )
+                if e.search(_Seq(pad + dsseq.watson + dsseq.watson[: e.size - 1] + pad) if self.circular else dsseq)
             ]  # flatten
 
         if not enzymes:
             return ()
 
-        if self.linear:
+        if not self.circular:
             frags = [self]
         else:
             l = len(self)
             for e in enzymes:
-
-                wpos = [x - len(pad) - 1 for x in e.search(_Seq(pad + self.watson + self.watson[: e.size - 1]) + pad)][::-1]
-                cpos = [x - len(pad) - 1 for x in e.search(_Seq(pad + self.crick + self.crick[: e.size - 1]) + pad)][::-1]
+                wpos = [x - len(pad) - 1 for x in e.search(_Seq(pad + self.watson + self.watson[: e.size - 1]) + pad)][
+                    ::-1
+                ]
+                cpos = [x - len(pad) - 1 for x in e.search(_Seq(pad + self.crick + self.crick[: e.size - 1]) + pad)][
+                    ::-1
+                ]
 
                 for w, c in _itertools.product(wpos, cpos):
                     if w % len(self) == (self.length - c + e.ovhg) % len(self):
-                        frags = [Dseq(self.watson[w % l :] + self.watson[: w % l],
-                                      self.crick[c % l :] + self.crick[: c % l],
-                                      ovhg=e.ovhg,
-                                      pos=min(w, len(dsseq) - c))]
+                        frags = [
+                            Dseq(
+                                self.watson[w % l :] + self.watson[: w % l],
+                                self.crick[c % l :] + self.crick[: c % l],
+                                ovhg=e.ovhg,
+                                pos=min(w, len(dsseq) - c),
+                            )
+                        ]
                         # breakpoint()
                         break
                 else:
                     continue
                 break
 
         newfrags = []
 
         # print(repr(frags[0]))
         # print(frags[0].pos)
 
         for enz in enzymes:
             for frag in frags:
-
                 ws = [x - 1 for x in enz.search(_Seq(frag.watson + "n"))]
                 cs = [x - 1 for x in enz.search(_Seq(frag.crick + "n"))]
 
-                sitepairs = [(sw, sc) for sw, sc in _itertools.product(ws, cs[::-1]) if (sw + max(0, frag.ovhg) - max(0, enz.ovhg)== len(frag.crick) - sc - min(0, frag.ovhg) + min(0, enz.ovhg))]
+                sitepairs = [
+                    (sw, sc)
+                    for sw, sc in _itertools.product(ws, cs[::-1])
+                    if (
+                        sw + max(0, frag.ovhg) - max(0, enz.ovhg)
+                        == len(frag.crick) - sc - min(0, frag.ovhg) + min(0, enz.ovhg)
+                    )
+                ]
 
                 sitepairs.append((self.length, 0))
 
                 w2, c1 = sitepairs[0]
-                newfrags.append(Dseq(frag.watson[:w2],
-                                     frag.crick[c1:],
-                                     ovhg=frag.ovhg,
-                                     pos=frag.pos))
+                newfrags.append(Dseq(frag.watson[:w2], frag.crick[c1:], ovhg=frag.ovhg, pos=frag.pos))
 
                 for (w1, c2), (w2, c1) in zip(sitepairs[:-1], sitepairs[1:]):
-                    newfrags.append(Dseq(frag.watson[w1:w2],
-                                         frag.crick[c1:c2],
-                                         ovhg=enz.ovhg,
-                                         pos=frag.pos + w1 - max(0, enz.ovhg) + max(0, frag.ovhg)))
+                    newfrags.append(
+                        Dseq(
+                            frag.watson[w1:w2],
+                            frag.crick[c1:c2],
+                            ovhg=enz.ovhg,
+                            pos=frag.pos + w1 - max(0, enz.ovhg) + max(0, frag.ovhg),
+                        )
+                    )
             frags = newfrags
             newfrags = []
 
         return tuple(frags)
 
     def _firstcut(self, *enzymes):
         rb = _RestrictionBatch(_flatten(enzymes))
@@ -1493,29 +1469,20 @@
         crick = _FormattedSeq(_Seq(self.crick), linear=False)
         enzdict = dict(sorted(rb.search(watson).items(), key=_itemgetter(1)))
         ln = self.length
         for enzyme, wposlist in enzdict.items():
             for cpos in enzyme.search(crick)[::-1]:
                 for wpos in wposlist:
                     if cpos == (ln - wpos + enzyme.ovhg + 2) or ln:
-                        return (wpos-1, cpos-1, enzyme.ovhg)
+                        return (wpos - 1, cpos - 1, enzyme.ovhg)
         return ()
 
-# wpos - max(0, enzyme.ovhg) == len(crick) - cpos + min(0, enzyme.ovhg) + 2
-# cpos == len(self.watson) - wpos + enzyme.ovhg + 2
 
 if __name__ == "__main__":
+    import os as _os
 
-    a = Dseq("aaaaaaaGGTACCggtctcaaaa")
-    from Bio.Restriction import BsaI
-    a._firstcut(BsaI)
-
-
-
-    # import os as _os
-
-    # cached = _os.getenv("pydna_cached_funcs", "")
-    # _os.environ["pydna_cached_funcs"] = ""
-    # import doctest
+    cached = _os.getenv("pydna_cached_funcs", "")
+    _os.environ["pydna_cached_funcs"] = ""
+    import doctest
 
-    # doctest.testmod(verbose=True, optionflags=doctest.ELLIPSIS)
-    # _os.environ["pydna_cached_funcs"] = cached
+    doctest.testmod(verbose=True, optionflags=doctest.ELLIPSIS)
+    _os.environ["pydna_cached_funcs"] = cached
```

### Comparing `pydna-5.2.0a9/src/pydna/dseqrecord.py` & `pydna-6.0.0a1/src/pydna/dseqrecord.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 The Dseq and Dseqrecord classes support the notion of circular and linear DNA topology.
 """
 from Bio.Restriction import RestrictionBatch as _RestrictionBatch
 from Bio.Restriction import CommOnly
 from pydna.dseq import Dseq as _Dseq
 from pydna._pretty import pretty_str as _pretty_str
 from pydna.utils import flatten as _flatten
-from pydna.utils import memorize as _memorize
+
+# from pydna.utils import memorize as _memorize
 from pydna.utils import rc as _rc
 from pydna.utils import shift_location as _shift_location
 from pydna.common_sub_strings import common_sub_strings as _common_sub_strings
 from Bio.SeqFeature import SeqFeature as _SeqFeature
 from Bio import SeqIO
 from Bio.SeqFeature import CompoundLocation as _CompoundLocation
 from Bio.SeqFeature import SimpleLocation as _SimpleLocation
@@ -39,16 +40,18 @@
 
 _module_logger = _logging.getLogger("pydna." + __name__)
 
 
 try:
     from IPython.display import display as _display
 except ImportError:
+
     def _display_html(item, raw=None):
         return item
+
 else:
     from IPython.display import display_html as _display_html
 
 
 class Dseqrecord(_SeqRecord):
     """Dseqrecord is a double stranded version of the Biopython SeqRecord [#]_ class.
     The Dseqrecord object holds a Dseq object describing the sequence.
@@ -122,148 +125,170 @@
     References
     ----------
 
     .. [#] http://biopython.org/wiki/SeqRecord
 
     """
 
-    def __init__(self,
-                 record,
-                 *args,
-                 linear=None,
-                 circular=None,
-                 n=5e-14,  # mol ( = 0.05 pmol)
-                 **kwargs):
-
+    def __init__(
+        self,
+        record,
+        *args,
+        # linear=None,
+        circular=None,
+        n=5e-14,  # mol ( = 0.05 pmol)
+        **kwargs,
+    ):
         _module_logger.info("### Dseqrecord initialized ###")
-        _module_logger.info("argument linear = %s", linear)
+        # _module_logger.info("argument linear = %s", linear)
         _module_logger.info("argument circular = %s", circular)
 
-        if not (linear is None and circular is None):
-            circular = (
-                bool(circular)
-                and bool(linear) ^ bool(circular)
-                or linear is False
-                and circular is None
-            )
-            linear = not circular
+        # if not (linear is None and circular is None):
+        #     circular = (bool(circular) and bool(linear) ^ bool(circular)
+        #                 or linear is False and circular is None)
+        #     linear = not circular
 
-        _module_logger.info("linear = %s", linear)
+        # _module_logger.info("linear = %s", linear)
         _module_logger.info("circular = %s", circular)
 
         if isinstance(record, str):
             _module_logger.info("record is a string")
             super().__init__(
-                _Dseq(record, linear=linear, circular=circular),
-                *args, **kwargs)
+                _Dseq.from_string(
+                    record,
+                    # linear=linear,
+                    circular=bool(circular),
+                ),
+                *args,
+                **kwargs,
+            )
 
         # record is a Dseq object ?
         elif hasattr(record, "watson"):
-            if record.circular and linear:
+            if circular == False:
                 record = record[:]
-            elif record.linear and circular:
+            elif circular == True:
                 record = record.looped()
             _module_logger.info("record is a Dseq object")
             super().__init__(record, *args, **kwargs)
 
         # record is a Bio.Seq object ?
         elif hasattr(record, "transcribe"):
             _module_logger.info("record is a Seq object")
             super().__init__(
-                _Dseq(str(record), linear=linear, circular=circular),
-                *args, **kwargs)
+                _Dseq(
+                    str(record),
+                    # linear=linear,
+                    circular=bool(circular),
+                ),
+                *args,
+                **kwargs,
+            )
 
         # record is a Bio.SeqRecord or Dseqrecord object ?
         elif hasattr(record, "features"):
             _module_logger.info("record is a Bio.SeqRecord or Dseqrecord object")
             for key, value in list(record.__dict__.items()):
                 setattr(self, key, value)
-            record.letter_annotations = {}
+            self.letter_annotations = {}
             # record.seq is a Dseq object ?
             if hasattr(record.seq, "watson"):
                 new_seq = _copy.copy(record.seq)
-                if new_seq.circular and linear:
+                if circular is False:
                     new_seq = new_seq[:]
-                elif new_seq.linear and circular:
+                elif circular is True:
                     new_seq = new_seq.looped()
                 self.seq = new_seq
             # record.seq is Bio.SeqRecord object ?
             else:
-                self.seq = _Dseq(str(self.seq), linear=linear,
-                                 circular=circular)
+                self.seq = _Dseq(
+                    str(record.seq),
+                    # linear=linear,
+                    circular=bool(circular),
+                )
         else:
             raise ValueError("don't know what to do with {}".format(record))
 
         self.map_target = None
         self.n = n  # amount, set to 5E-14 which is 5 pmols
         self.annotations.update({"molecule_type": "DNA"})
 
     @classmethod
-    def from_string(cls,
-                    record: str = "",
-                    *args,
-                    linear=True,
-                    circular=False,
-                    n=5e-14,
-                    **kwargs):
+    def from_string(
+        cls,
+        record: str = "",
+        *args,
+        # linear=True,
+        circular=False,
+        n=5e-14,
+        **kwargs,
+    ):
         """docstring."""
         # def from_string(cls, record:str="", *args,
         # linear=True, circular=False, n = 5E-14, **kwargs):
         obj = cls.__new__(cls)  # Does not call __init__
-        obj._seq = _Dseq.quick(record,
-                               _rc(record),
-                               ovhg=0,
-                               linear=linear,
-                               circular=circular)
+        obj._per_letter_annotations = {}
+        obj.seq = _Dseq.quick(
+            record,
+            _rc(record),
+            ovhg=0,
+            # linear=linear,
+            circular=circular,
+        )
         obj.id = _pretty_str("id")
         obj.name = _pretty_str("name")
         obj.description = _pretty_str("description")
         obj.dbxrefs = []
         obj.annotations = {"molecule_type": "DNA"}
-        obj._per_letter_annotations = {}
         obj.features = []
         obj.map_target = None
         obj.n = n
         obj.__dict__.update(kwargs)
         return obj
 
     @classmethod
     def from_SeqRecord(
-        cls, record: _SeqRecord, *args, linear=True, circular=False, n=5e-14, **kwargs
+        cls,
+        record: _SeqRecord,
+        *args,
+        # linear=True,
+        circular=False,
+        n=5e-14,
+        **kwargs,
     ):
         obj = cls.__new__(cls)  # Does not call __init__
-        obj._seq = _Dseq.quick(
+        obj._per_letter_annotations = record._per_letter_annotations
+        obj.seq = _Dseq.quick(
             str(record.seq),
             _rc(str(record.seq)),
             ovhg=0,
-            linear=linear,
+            # linear=linear,
             circular=circular,
         )
         obj.id = record.id
         obj.name = record.name
         obj.description = record.description
         obj.dbxrefs = record.dbxrefs
         obj.annotations = {"molecule_type": "DNA"}
         obj.annotations.update(record.annotations)
-        obj._per_letter_annotations = record._per_letter_annotations
         obj.features = record.features
         obj.map_target = None
         obj.n = n
         return obj
 
-    @property
-    def linear(self):
-        """The linear property can not be set directly.
-        Use :meth:`looped` or :meth:`tolinear`"""
-        return self.seq.linear
+    # @property
+    # def linear(self):
+    #     """The linear property can not be set directly.
+    #     Use :meth:`looped` or :meth:`tolinear`"""
+    #     return self.seq.linear
 
     @property
     def circular(self):
         """The circular property can not be set directly.
-        Use :meth:`looped` or :meth:`tolinear`"""
+        Use :meth:`looped`"""
         return self.seq.circular
 
     def m(self):
         """This method returns the mass of the DNA molecule in grams. This is
         calculated as the product between the molecular weight of the Dseq object
         and the"""
         return self.seq.mw() * self.n  # Da(g/mol) * mol = g
@@ -288,20 +313,15 @@
         Dseq(-2)
         gt
         ca
 
         """
         return super().extract_feature(n)
 
-    def add_feature(self,
-                    x=None,
-                    y=None,
-                    seq=None,
-                    type_="misc",
-                    strand=1, *args, **kwargs):
+    def add_feature(self, x=None, y=None, seq=None, type_="misc", strand=1, *args, **kwargs):
         """Add a feature of type misc to the feature list of the sequence.
 
         Parameters
         ----------
         x  : int
             Indicates start of the feature
         y  : int
@@ -320,42 +340,34 @@
                                    strand=1),
                     type='misc',
                     qualifiers=...)]
         """
         if x and y and self.circular and x > y:
             pass
         else:
-            super().add_feature(x,
-                                y,
-                                seq,
-                                type_,
-                                strand=1,
-                                *args, **kwargs)
+            super().add_feature(x, y, seq, type_, strand=strand, *args, **kwargs)
             return
 
         qualifiers = {}
         qualifiers.update(kwargs)
 
         location = _CompoundLocation(
-                    (_SimpleLocation(x, self.seq.length, strand=strand),
-                     _SimpleLocation(0, y, strand=strand)))
+            (_SimpleLocation(x, self.seq.length, strand=strand), _SimpleLocation(0, y, strand=strand))
+        )
 
-        sf = _SeqFeature(location,
-                         type=type_,
-                         qualifiers=qualifiers)
+        sf = _SeqFeature(location, type=type_, qualifiers=qualifiers)
 
         if "label" not in qualifiers:
             qualifiers["label"] = [f"ft{len(location)}"]
 
         if sf.extract(self).isorf():
             qualifiers["label"] = [f"orf{len(location)}"]
 
         self.features.append(sf)
 
-
     def useguid(self):
         """Url safe SEGUID for the sequence.
 
         This checksum is the same as seguid but with base64.urlsafe
         encoding instead of the normal base64. This means that
         the characters + and / are replaced with - and _ so that
         the checksum can be part of a URL.
@@ -387,15 +399,15 @@
         'CTJbs6Fat8kLQxHj-_SC0kGEiYs'
 
         >>> a=Dseqrecord("gagtatcgtacat", circular=True)
         >>> a.cseguid()
         'CTJbs6Fat8kLQxHj-_SC0kGEiYs'
 
         """
-        if self.linear:
+        if not self.circular:
             raise TypeError("cseguid is only defined for circular sequences.")
         return self.seq.cseguid()
 
     def lseguid(self):
         """Url safe lSEGUID for a linear sequence.
 
         Only defined for linear double stranded sequences.
@@ -451,24 +463,21 @@
         for fn, fo in zip(new.features, self.features):
             if five_prime[0] == "5'":
                 pass
                 # fn.location = fn.location + self.seq.ovhg
             elif five_prime[0] == "3'":
                 fn.location = fn.location + (-self.seq.ovhg)
             if fn.location.start < 0:
-                loc1 = _SimpleLocation(len(new) + fn.location.start,
-                                        len(new), strand=fn.strand)
+                loc1 = _SimpleLocation(len(new) + fn.location.start, len(new), strand=fn.strand)
                 loc2 = _SimpleLocation(0, fn.location.end, strand=fn.strand)
                 fn.location = _CompoundLocation([loc1, loc2])
 
             if fn.location.end > len(new):
-                loc1 = _SimpleLocation(fn.location.start,
-                                        len(new), strand=fn.strand)
-                loc2 = _SimpleLocation(0, fn.location.end - len(new),
-                                        strand=fn.strand)
+                loc1 = _SimpleLocation(fn.location.start, len(new), strand=fn.strand)
+                loc2 = _SimpleLocation(0, fn.location.end - len(new), strand=fn.strand)
                 fn.location = _CompoundLocation([loc1, loc2])
 
             fn.qualifiers = fo.qualifiers
         # breakpoint()
         return new
 
     def tolinear(self):  # pragma: no cover
@@ -490,17 +499,15 @@
         >>>
 
         """
         import warnings as _warnings
         from pydna import _PydnaDeprecationWarning
 
         _warnings.warn(
-            "tolinear method is obsolete; "
-            "please use obj[:] "
-            "instead of obj.tolinear().",
+            "tolinear method is obsolete; " "please use obj[:] " "instead of obj.tolinear().",
             _PydnaDeprecationWarning,
         )
         new = _copy.copy(self)
         for key, value in list(self.__dict__.items()):
             setattr(new, key, value)
         # new._seq = self.seq.tolinear()
         for fn, fo in zip(new.features, self.features):
@@ -585,23 +592,24 @@
         .. [#] http://biopython.org/wiki/SeqIO
 
         """
         msg = ""
         if not filename:
             filename = "{name}.{type}".format(name=self.locus, type=f)
             # generate a name if no name was given
-        if not isinstance(filename, str):  # is filename a string???
-            raise ValueError("filename has to be a string, got", type(filename))
+        # if not isinstance(filename, str):  # is filename a string???
+        #     raise ValueError("filename has to be a string, got", type(filename))
         name, ext = _os.path.splitext(filename)
         msg = f"<font face=monospace><a href='{filename}' target='_blank'>{filename}</a></font><br>"
         if not _os.path.isfile(filename):
             with open(filename, "w", encoding="utf8") as fp:
                 fp.write(self.format(f))
         else:
             from pydna.readers import read
+
             old_file = read(filename)
 
             if self.seq != old_file.seq:
                 # If new sequence is different, the old file is
                 # renamed with "_OLD_" suffix:
                 oldmtime = _datetime.datetime.fromtimestamp(_os.path.getmtime(filename)).isoformat()
                 tstmp = int(_time.time() * 1_000_000)
@@ -662,17 +670,15 @@
                 pattern = r"(lSEGUID|cSEGUID|uSEGUID)_(\S{27})(_[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}\.[0-9]{6}){0,1}"
                 # cSEGUID_NNNNNNNNNNNNNNNNNNNNNNNNNNN_2020-10-10T11:11:11.111111
                 oldstamp = _re.search(pattern, old_file.description)
                 newstamp = _re.search(pattern, self.description)
                 newdescription = self.description
                 if oldstamp and newstamp:
                     if oldstamp.group(0)[:35] == newstamp.group(0)[:35]:
-                        newdescription = newdescription.replace(
-                                         newstamp.group(0),
-                                         oldstamp.group(0))
+                        newdescription = newdescription.replace(newstamp.group(0), oldstamp.group(0))
                 elif oldstamp:
                     newdescription += " " + oldstamp.group(0)
                 newobj = _copy.copy(self)
                 newobj.description = newdescription
 
                 with open(filename, "w", encoding="utf8") as fp:
                     fp.write(newobj.format(f))
@@ -683,26 +689,24 @@
 
     def find(self, other):
         # TODO allow strings, seqs, seqrecords or Dseqrecords
         # TODO check for linearity of other, raise exception if not
         # TODO add tests and docstring for this method
         o = str(other.seq).upper()
 
-        if self.linear:
+        if not self.circular:
             s = str(self.seq).upper()
         else:
-            s = (
-                str(self.seq).upper() + str(self.seq).upper()[: len(other) - 1]
-            )  # allow wrapping around origin
+            s = str(self.seq).upper() + str(self.seq).upper()[: len(other) - 1]  # allow wrapping around origin
         return s.find(o)
 
     def __str__(self):
-        return ("Dseqrecord\n" "circular: {}\n" "size: {}\n").format(
-            self.circular, len(self)
-        ) + _SeqRecord.__str__(self)
+        return ("Dseqrecord\n" "circular: {}\n" "size: {}\n").format(self.circular, len(self)) + _SeqRecord.__str__(
+            self
+        )
 
     def __contains__(self, other):
         if other.lower() in str(self.seq).lower():
             return True
         else:
             s = self.seq.watson.replace(" ", "")
             ln = len(s)
@@ -795,15 +799,14 @@
             self.matching_reads = None
             self.not_matching_reads = None
             reads = traces
 
         matching_reads = []
 
         for read_ in reads:
-
             matches = _common_sub_strings(str(self.seq).lower(), str(read_.seq), limit)
 
             if not matches:
                 continue
 
             if len(matches) > 1:
                 newmatches = [
@@ -834,22 +837,18 @@
                     type="trace",
                 )
             )
 
         return [x.annotations["filename"] for x in matching_reads]
 
     def __repr__(self):
-        return "Dseqrecord({}{})".format(
-            {True: "-", False: "o"}[self.linear], len(self)
-        )
+        return "Dseqrecord({}{})".format({True: "-", False: "o"}[not self.circular], len(self))
 
     def _repr_pretty_(self, p, cycle):
-        p.text(
-            "Dseqrecord({}{})".format({True: "-", False: "o"}[self.linear], len(self))
-        )
+        p.text("Dseqrecord({}{})".format({True: "-", False: "o"}[not self.circular], len(self)))
 
     def __add__(self, other):
         if hasattr(other, "seq") and hasattr(other.seq, "watson"):
             other = _copy.deepcopy(other)
             other_five_prime = other.seq.five_prime_end()
             if other_five_prime[0] == "5'":
                 # add other.seq.ovhg
@@ -865,19 +864,15 @@
         else:
             answer = Dseqrecord(_SeqRecord.__add__(self, Dseqrecord(other)))
             answer.n = self.n
         return answer
 
     def __mul__(self, number):
         if not isinstance(number, int):
-            raise TypeError(
-                "TypeError: can't multiply Dseqrecord by non-int of type {}".format(
-                    type(number)
-                )
-            )
+            raise TypeError("TypeError: can't multiply Dseqrecord by non-int of type {}".format(type(number)))
         if self.circular:
             raise TypeError("TypeError: can't multiply circular Dseqrecord.")
         if number > 0:
             new = _copy.copy(self)
             for i in range(1, number):
                 new += self
             return new
@@ -885,27 +880,23 @@
             return self.__class__("")
 
     def __getitem__(self, sl):
         """docstring."""
         answer = Dseqrecord(_copy.copy(self))
         answer.seq = self.seq.__getitem__(sl)
         # answer.seq.alphabet = self.seq.alphabet
-
+        # breakpoint()
         sl_start = sl.start or 0  # 6
-        sl_stop = sl.stop or len(answer.seq)  # 1
+        sl_stop = sl.stop or len(self.seq)  # 1
 
-        if self.linear or sl_start < sl_stop:
+        if not self.circular or sl_start < sl_stop:
             answer.features = super().__getitem__(sl).features
         elif self.circular and sl_start > sl_stop:
             answer.features = self.shifted(sl_start).features
-            answer.features = [
-                f
-                for f in answer.features
-                if f.location.parts[-1].end <= answer.seq.length
-            ]
+            answer.features = [f for f in answer.features if f.location.parts[-1].end <= answer.seq.length]
         else:
             answer = Dseqrecord("")
         identifier = "part_{id}".format(id=self.id)
         if answer.features:
             sf = max(answer.features, key=len)  # default
             if "label" in sf.qualifiers:
                 identifier = " ".join(sf.qualifiers["label"])
@@ -926,25 +917,23 @@
 
     def __ne__(self, other):
         """docstring."""
         return not self.__eq__(other)
 
     def __hash__(self):
         """__hash__ must be based on __eq__."""
-        return hash(
-            (str(self.seq).lower(), str(tuple(sorted(self.__dict__.items()))))
-            )
+        return hash((str(self.seq).lower(), str(tuple(sorted(self.__dict__.items())))))
 
     def linearize(self, *enzymes):
         """Similar to :func:`cut.
 
         Throws an exception if there is not excactly one cut
         i.e. none or more than one digestion products.
         """
-        if self.seq._linear:
+        if not self.seq.circular:
             raise TypeError("Can only linearize circular molecules!")
         fragments = self.cut(*enzymes)
         if len(fragments) > 1:
             raise TypeError("More than one fragment is formed!")
         elif not fragments:
             raise TypeError("The enzyme(s) do not cut!")
         answer = fragments[0]
@@ -975,23 +964,22 @@
     def cutters(self, batch: _RestrictionBatch = None):
         """docstring."""
         return self.seq.cutters(batch=batch or CommOnly)
 
     def number_of_cuts(self, *enzymes):
         """The number of cuts by digestion with the Restriction enzymes
         contained in the iterable."""
-        return sum([len(enzyme.search(self.seq)) for enzyme
-                    in _flatten(enzymes)])
+        return sum([len(enzyme.search(self.seq)) for enzyme in _flatten(enzymes)])
 
     def cas9(self, RNA: str):
         """docstring."""
         fragments = []
         result = []
         for target in (self.seq, self.seq.rc()):
-            fragments = [self[sl.start:sl.stop] for sl in target.cas9(RNA)]
+            fragments = [self[sl.start : sl.stop] for sl in target.cas9(RNA)]
             result.append(fragments)
         return result
 
     def reverse_complement(self):
         """Reverse complement.
 
         Examples
@@ -1015,36 +1003,36 @@
         pydna.dseq.Dseq.reverse_complement
 
         """
         answer = type(self)(super().reverse_complement())
         answer.name = "{}_rc".format(self.name[:13])
         answer.description = self.description + "_rc"
         answer.id = self.id + "_rc"
-        answer.seq._circular = self.seq.circular
-        answer.seq._linear = self.seq.linear
+        answer.seq.circular = self.seq.circular
+        # answer.seq._linear = self.seq.linear
         return answer
 
     rc = reverse_complement
 
-    @_memorize("pydna.dseqrecord.Dseqrecord.synced")
+    # @_memorize("pydna.dseqrecord.Dseqrecord.synced")
     def synced(self, ref, limit=25):
         """This method returns a new circular sequence (Dseqrecord object), which has been rotated
         in such a way that there is maximum overlap between the sequence and
         ref, which may be a string, Biopython Seq, SeqRecord object or
         another Dseqrecord object.
 
         The reason for using this could be to rotate a new recombinant plasmid so
         that it starts at the same position after cloning. See the example below:
 
 
         Examples
         --------
 
         >>> from pydna.dseqrecord import Dseqrecord
-        >>> a=Dseqrecord("gaat",circular=True)
+        >>> a=Dseqrecord("gaat", circular=True)
         >>> a.seq
         Dseq(o4)
         gaat
         ctta
         >>> d = a[2:] + a[:2]
         >>> d.seq
         Dseq(-4)
@@ -1059,15 +1047,15 @@
         >>> recombinant.synced(a).seq
         Dseq(o7)
         gaCCCat
         ctGGGta
 
         """
 
-        if self.linear:
+        if not self.circular:
             raise TypeError("Only circular DNA can be synced!")
 
         newseq = _copy.copy(self)
 
         s = str(self.seq.watson).lower()
         s_rc = str(self.seq.crick).lower()
 
@@ -1106,15 +1094,15 @@
             newseq = newseq.rc()
 
         if start == 0:
             result = newseq
         else:
             result = newseq.shifted(start)
         _module_logger.info("synced")
-        return Dseqrecord(result)
+        return result
 
     def upper(self):
         """Returns an uppercase copy.
         >>> from pydna.dseqrecord import Dseqrecord
         >>> my_seq = Dseqrecord("aAa")
         >>> my_seq.seq
         Dseq(-3)
@@ -1192,46 +1180,43 @@
         self._copy_to_clipboard("fasta")
         return None
 
     def figure(self, feature=0, highlight="\x1b[48;5;11m", plain="\x1b[0m"):
         """docstring."""
         if self.features:
             f = self.features[feature]
-            locations = sorted(self.features[feature].location.parts,
-                               key=_SimpleLocation.start.fget)
+            locations = sorted(self.features[feature].location.parts, key=_SimpleLocation.start.fget)
             strand = f.strand
         else:
             locations = [_SimpleLocation(0, 0, 1)]
             strand = 1
 
-        ovhg = self.seq.ovhg+len(self.seq.watson)-len(self.seq.crick)
+        ovhg = self.seq.ovhg + len(self.seq.watson) - len(self.seq.crick)
 
         w = f"{self.seq.ovhg*chr(32)}{self.seq.watson}{-ovhg*chr(32)}"
         c = f"{-self.seq.ovhg*chr(32)}{self.seq.crick[::-1]}{ovhg*chr(32)}"
 
         if strand == 1:
             s1, s2 = w, c
         else:
             s1, s2 = c, w
 
-        wfe = [f"{highlight}{s1[part.start:part.end]}{plain}"
-               for part in locations]
+        wfe = [f"{highlight}{s1[part.start:part.end]}{plain}" for part in locations]
 
         wfe.append("")
 
-        wof = [s1[0:locations[0].start]]
-        for f, s in zip(locations,
-                        locations[1:]):
-            wof.append(s1[f.end:s.start])
-        wof.append(s1[locations[-1].end:len(self)])
+        wof = [s1[0 : locations[0].start]]
+        for f, s in zip(locations, locations[1:]):
+            wof.append(s1[f.end : s.start])
+        wof.append(s1[locations[-1].end : len(self)])
 
-        topology = {True: '-', False: 'o'}[self.linear]
+        topology = {True: '-', False: 'o'}[not self.circular]
         result = f"{self.__class__.__name__}({topology}{len(self)})\n"
 
-        s1 = "".join(f+s for f, s in zip(wof, wfe))
+        s1 = "".join(f + s for f, s in zip(wof, wfe))
 
         if strand == 1:
             result += f"{s1}\n{s2}"
         else:
             result += f"{s2}\n{s1}"
         return _pretty_str(result)
 
@@ -1275,28 +1260,25 @@
         Dseqrecord(o4)
         >>> b.seq
         Dseq(o4)
         aata
         ttat
 
         """
-        if self.linear:
-            raise TypeError("Sequence is linear, origin can only be "
-                            "shifted for circular sequences.\n")
+        if not self.circular:
+            raise TypeError("Sequence is linear, origin can only be " "shifted for circular sequences.\n")
         ln = len(self)
         if not shift % ln:
             return self  # shift is a multiple of ln or 0
         else:
             shift %= ln  # 0<=shift<=ln
         newseq = (self.seq[shift:] + self.seq[:shift]).looped()
         newfeatures = _copy.deepcopy(self.features)
         for feature in newfeatures:
-            feature.location = _shift_location(feature.location,
-                                               -shift,
-                                               ln)
+            feature.location = _shift_location(feature.location, -shift, ln)
         newfeatures.sort(key=_operator.attrgetter("location.start"))
         answer = _copy.copy(self)
         answer.features = newfeatures
         answer.seq = newseq
         return answer
 
     def cut(self, *enzymes):
@@ -1343,48 +1325,43 @@
         features = _copy.deepcopy(self.features)
 
         if self.circular:
             try:
                 x, y, oh = self.seq._firstcut(*enzymes)
             except ValueError:
                 return ()
-            dsr = _Dseq(self.seq.watson[x:] + self.seq.watson[:x],
-                        self.seq.crick[y:] + self.seq.crick[:y],
-                        oh)
+            dsr = _Dseq(self.seq.watson[x:] + self.seq.watson[:x], self.seq.crick[y:] + self.seq.crick[:y], oh)
             newstart = min(x, (self.seq.length - y))
             for f in features:
-                f.location = shift_location(f.location,
-                                            -newstart,
-                                            self.seq.length)
+                f.location = shift_location(f.location, -newstart, self.seq.length)
                 f.location, *rest = f.location.parts
                 for part in rest:
                     if 0 in part:
                         f.location._end = part.end + self.seq.length
                     else:
                         f.location += part
             frags = dsr.cut(enzymes) or [dsr]
         else:
             frags = self.seq.cut(enzymes)
             if not frags:
                 return ()
         dsfs = []
         for fr in frags:
-            dsf = Dseqrecord(fr, linear=True, n=self.n)
+            dsf = Dseqrecord(fr, n=self.n)
             start = fr.pos
             end = fr.pos + fr.length
-            dsf.features = [_copy.deepcopy(fe)
-                            for fe in features
-                            if start <= fe.location.start
-                            and end >= fe.location.end]
+            dsf.features = [
+                _copy.deepcopy(fe) for fe in features if start <= fe.location.start and end >= fe.location.end
+            ]
             for feature in dsf.features:
                 feature.location += -start
             dsfs.append(dsf)
         return tuple(dsfs)
 
 
 if __name__ == "__main__":
     cache = _os.getenv("pydna_cache")
     _os.environ["pydna_cache"] = "nocache"
     import doctest
 
     doctest.testmod(verbose=True, optionflags=doctest.ELLIPSIS)
-    _os.environ["pydna_cache"] = cache
+    # _os.environ["pydna_cache"] = cache
```

### Comparing `pydna-5.2.0a9/src/pydna/editor.py` & `pydna-6.0.0a1/src/pydna/editor.py`

 * *Files identical despite different names*

### Comparing `pydna-5.2.0a9/src/pydna/fakeseq.py` & `pydna-6.0.0a1/src/pydna/fakeseq.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 # as part of this package.
 """docstring."""
 
 
 class FakeSeq(object):
     """docstring."""
 
-    def __init__(self,
-                 length,
-                 n=50e-15,  # 50 fmol = 0.05 pmol
-                 rf=0):
+    def __init__(self, length, n=50e-15, rf=0):  # 50 fmol = 0.05 pmol
         self._length = int(length)
         self.n = n
         self.rf = rf
 
     def m(self):
         """Mass of the DNA molecule in grams."""
         # M(Da) * n (mol) = g
```

### Comparing `pydna-5.2.0a9/src/pydna/gateway.py` & `pydna-6.0.0a1/src/pydna/gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 The NetworkX package is used to trace linear and circular paths through the
 graph.
 """
 from Bio.SeqFeature import ExactPosition as _ExactPosition
 from Bio.SeqFeature import SimpleLocation as _SimpleLocation
 from Bio.SeqFeature import CompoundLocation as _CompoundLocation
 from pydna.utils import rc as _rc
-from pydna.utils import memorize as _memorize
+
 from pydna._pretty import pretty_str as _pretty_str
 from pydna.contig import Contig as _Contig
 from pydna.common_sub_strings import common_sub_strings
 from pydna.dseqrecord import Dseqrecord as _Dseqrecord
 import networkx as _nx
 from copy import deepcopy as _deepcopy
 import itertools as _itertools
@@ -44,15 +44,16 @@
     "Y": "[CTY]",
     "K": "[GTK]",
     "V": "[ACGVMSR]",
     "H": "[ACTHMYW]",
     "D": "[AGTDRWK]",
     "B": "[CGTBSKY]",
     "X": "X",
-    "N": "[ACGTBDHKMNRSVWY]" }
+    "N": "[ACGTBDHKMNRSVWY]",
+}
 
 atts = """
 attP1 AAATAATGATTTTATTTTGACTGATAGTGACCTGTTCGTTGCAACAMATTGATRAGCAATKMTTTYTTATAATGCCMASTTT GTACAAA AAAGYWGAACGAGAAACGTAAAATGATATAAATATCAATATATTAAATTAGATTTTGCATAAAAAACAGACTACATAATRCTGTAAAACACAACATATSCAGTCAYWWTG CMASTWT AAAGYWG
 attP2 AAATAATGATTTTATTTTGACTGATAGTGACCTGTTCGTTGCAACAMATTGATRAGCAATKMTTTYTTATAATGCCMASTTT GTACAAG AAAGYWGAACGAGAAACGTAAAATGATATAAATATCAATATATTAAATTAGATTTTGCATAAAAAACAGACTACATAATRCTGTAAAACACAACATATSCAGTCAYWWTG CMASTWT AAAGYWG
 attP3 AAATAATGATTTTATTTTGACTGATAGTGACCTGTTCGTTGCAACAMATTGATRAGCAATKMTTTYTTATAATGCCMASTTT GTATAAT AAAGYWGAACGAGAAACGTAAAATGATATAAATATCAATATATTAAATTAGATTTTGCATAAAAAACAGACTACATAATRCTGTAAAACACAACATATSCAGTCAYWWTG CMASTWT AAAGYWG
 attP4 AAATAATGATTTTATTTTGACTGATAGTGACCTGTTCGTTGCAACAMATTGATRAGCAATKMTTTYTTATAATGCCMASTTT GTATAGA AAAGYWGAACGAGAAACGTAAAATGATATAAATATCAATATATTAAATTAGATTTTGCATAAAAAACAGACTACATAATRCTGTAAAACACAACATATSCAGTCAYWWTG CMASTWT AAAGYWG
 attP5 AAATAATGATTTTATTTTGACTGATAGTGACCTGTTCGTTGCAACAMATTGATRAGCAATKMTTTYTTATAATGCCMASTTT GTATACA AAAGYWGAACGAGAAACGTAAAATGATATAAATATCAATATATTAAATTAGATTTTGCATAAAAAACAGACTACATAATRCTGTAAAACACAACATATSCAGTCAYWWTG CMASTWT AAAGYWG
@@ -80,49 +81,31 @@
 retable = str.maketrans(ambiguous_dna_regex)
 
 for line in (line for line in atts.splitlines() if line.strip()):
     name, *parts = line.split()
     for part in parts:
         part.translate(retable)
 
-class _Memoize(type):
-    @_memorize("pydna.gateway.Gateway")
-    def __call__(cls, *args, **kwargs):
-        return super().__call__(*args, **kwargs)
-
 
-class Gateway(object, metaclass=_Memoize):
+class Gateway(object):
     """Assembly of linear DNA fragments into linear or circular constructs.
 
     The Assembly is meant to replace the Assembly method as it
     is easier to use. Accepts a list of Dseqrecords (source fragments) to
     initiate an Assembly object. Several methods are available for analysis
     of overlapping sequences, graph construction and assembly.
 
     Parameters
     ----------
     fragments : list
         a list of Dseqrecord objects.
     """
 
     def __init__(self, molecules=None):
-        self.molecules =molecules
-
-
-
-
-
-
-
-
-
-
-
-
-
+        self.molecules = molecules
 
 
 """
 Created on Sat Aug 21 15:41:42 2021
 
 @author: bjorn
 
@@ -147,44 +130,14 @@
 M11	        ATAACTTCGTATA	cgaTAcca	TATACGAAGTTAT
 lox 71	    TACCGTTCGTATA	NNNTANNN	TATACGAAGTTAT
 lox 66	    ATAACTTCGTATA	NNNTANNN	TATACGAACGGTA
 
 """
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
 """
 
 https://blog.addgene.org/plasmids-101-cre-lox
 
 https://en.wikipedia.org/wiki/Cre-Lox_recombination
 
 13bp	      8bp	   13bp
@@ -202,8 +155,8 @@
 M2	        ATAACTTCGTATA	AgaaAcca	TATACGAAGTTAT
 M3	        ATAACTTCGTATA	taaTACCA	TATACGAAGTTAT
 M7	        ATAACTTCGTATA	AgaTAGAA	TATACGAAGTTAT
 M11	        ATAACTTCGTATA	cgaTAcca	TATACGAAGTTAT
 lox71	    TACCGTTCGTATA	NNNTANNN	TATACGAAGTTAT
 lox66	    ATAACTTCGTATA	NNNTANNN	TATACGAACGGTA
 
-"""
+"""
```

### Comparing `pydna-5.2.0a9/src/pydna/gel.py` & `pydna-6.0.0a1/src/pydna/gel.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,26 +15,22 @@
 import math as _math
 from scipy.interpolate import CubicSpline as _CubicSpline
 from pydna.ladders import GeneRuler_1kb_plus as _mwstd
 
 
 def interpolator(mwstd):
     """docstring."""
-    interpolator = _CubicSpline([len(fr) for fr in mwstd[::-1]],
-                                [fr.rf for fr in mwstd[::-1]],
-                                bc_type="natural",
-                                extrapolate=False)
+    interpolator = _CubicSpline(
+        [len(fr) for fr in mwstd[::-1]], [fr.rf for fr in mwstd[::-1]], bc_type="natural", extrapolate=False
+    )
     interpolator.mwstd = mwstd
     return interpolator
 
 
-def gel(samples=None,
-        gel_length=600,
-        margin=50,
-        interpolator=interpolator(mwstd=_mwstd)):
+def gel(samples=None, gel_length=600, margin=50, interpolator=interpolator(mwstd=_mwstd)):
     """docstring."""
     max_intensity = 256
     lane_width = 50
     lanesep = 10
     start = 10
     samples = samples or [interpolator.mwstd]
     width = int(60 + (lane_width + lanesep) * len(samples))
@@ -51,26 +47,25 @@
 
     for lane_number, lane in enumerate(samples):
         for band in lane:
             log = _math.log(len(band), 10)
             height = (band.m() / (240 * log)) * 1e10
             peak_centre = interpolator(len(band)) * scale + start
             max_spread = 10
-            if len(band) <= 50:
-                peak_centre += 50
-                max_spread *= 4
-                max_intensity /= 10
+            # if len(band) <= 50:
+            #     peak_centre += 50
+            #     max_spread *= 4
+            #     max_intensity /= 10
             band_spread = max_spread / log
             for i in range(max_spread, 0, -1):
                 y1 = peak_centre - i
                 y2 = peak_centre + i
                 intensity = (
-                    height * _math.exp(
-                        -float(((y1 - peak_centre) ** 2)) / (2 * (band_spread ** 2))
-                    ) * max_intensity)
+                    height * _math.exp(-float(((y1 - peak_centre) ** 2)) / (2 * (band_spread**2))) * max_intensity
+                )
                 for y in range(int(y1), int(y2)):
                     try:
                         lanes[lane_number][y] += intensity
                     except IndexError:
                         pass
 
     for i, lane in enumerate(lanes):
@@ -81,22 +76,24 @@
 
     for i, lane in enumerate(lanes):
         x1 = 50 + i * (lane_width + lanesep)
         x2 = x1 + lane_width
         for y, intensity in enumerate(lane):
             y1 = y
             y2 = y + 1
-            draw.rectangle((x1, y1, x2, y2), fill=(intensity,
-                                                   intensity,
-                                                   intensity))
+            draw.rectangle((x1, y1, x2, y2), fill=(intensity, intensity, intensity))
 
     return image
 
-    #  im.rotate(90, expand=1)
-    #  im_invert = ImageOps.invert(im)
+
+# Inverting and rotating the gel
+# im = gel([ GeneRuler_1kb_plus, [band, ]])
+# from PIL import ImageOps
+# im_invert = ImageOps.invert(im)
+# im.rotate(90, expand=1)
 
 
 if __name__ == "__main__":
     import os as _os
 
     cached = _os.getenv("pydna_cached_funcs", "")
     _os.environ["pydna_cached_funcs"] = ""
```

### Comparing `pydna-5.2.0a9/src/pydna/genbank.py` & `pydna-6.0.0a1/src/pydna/genbank.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,38 +43,32 @@
     >>> gb=Genbank("bjornjobb@gmail.com")
     >>> rec = gb.nucleotide("LP002422.1")   # <- entry from genbank
     >>> print(len(rec))
     1
     """
 
     def __init__(self, users_email: str, *args, tool="pydna", **kwargs):
-
-        if not _re.match(
-            r"[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,4}", users_email, _re.IGNORECASE
-        ):
+        if not _re.match(r"[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,4}", users_email, _re.IGNORECASE):
             raise ValueError("email address {} is not valid.".format(users_email))
 
         _module_logger.info("#### Genbank ititiation ####")
         _module_logger.info("Genbank initiated with email: %s", users_email)
         _module_logger.info("Genbank initiated with tool : %s", tool)
 
         if users_email == "someone@example.com":
-            raise ValueError(
-                "you have to set your email address in order to download from Genbank"
-            )
+            raise ValueError("you have to set your email address in order to download from Genbank")
         self.email = users_email
         self.tool = tool
 
     def __repr__(self):
         """This method returns a short representation containing the email used to initiate."""
         return "GenbankConnection({})".format(self.email)
 
     @_memorize("pydna.genbank.Genbank.nucleotide")
     def nucleotide(self, item: str, seq_start=None, seq_stop=None, strand=1):
-
         """This method downloads a genbank nuclotide record from genbank. This method is
         cached by default. This can be controlled by editing the **pydna_cached_funcs** environment
         variable. The best way to do this permanently is to edit the edit the
         `pydna.ini` file. See the documentation of :func:`pydna.open_config_folder`
 
         Item is a string containing one genbank accession number
         for a nucleotide file. Genbank nucleotide accession numbers have this format:
@@ -115,35 +109,33 @@
         ----------
 
         .. [#]   http://www.dsimb.inserm.fr/~fuchs/M2BI/AnalSeq/Annexes/Sequences/Accession_Numbers.htm
         .. [#]   http://www.ncbi.nlm.nih.gov/books/NBK25499/#chapter4.EFetch
         """
         matches = (
             (1, _re.search(r"(REGION:\s(?P<start>\d+)\.\.(?P<stop>\d+))", item)),
-            (2, _re.search(r"(REGION: complement\((?P<start>\d+)\.\.(?P<stop>\d+)\))", item),),
+            (
+                2,
+                _re.search(r"(REGION: complement\((?P<start>\d+)\.\.(?P<stop>\d+)\))", item),
+            ),
             (1, _re.search(r"(:|\s)(?P<start>\d+)-(?P<stop>\d+)", item)),
             (2, _re.search(r"(:|\s)c(?P<start>\d+)-(?P<stop>\d+)", item)),
         )
 
         for strand_, match in matches:
             if match:
                 seq_start = match.group("start")
                 seq_stop = match.group("stop")
                 item = item[: match.start()]
                 strand = strand_
                 break
 
         if strand not in [1, 2]:
             try:
-                strand = {"c": 2,
-                          "crick": 2,
-                          "antisense": 2,
-                          "2": 2,
-                          "-": 2,
-                          "-1": 2}[strand.lower()]
+                strand = {"c": 2, "crick": 2, "antisense": 2, "2": 2, "-": 2, "-1": 2}[strand.lower()]
             except (KeyError, AttributeError):
                 strand = 1
 
         _module_logger.info("#### Genbank download ####")
         _module_logger.info("item  %s", item)
         _module_logger.info("start %s", seq_start)
         _module_logger.info("stop  %s", seq_stop)
@@ -165,20 +157,15 @@
             seq_stop=seq_stop,
             strand=strand,
             retmode="text",
         ).read()
 
         _module_logger.info("text[:160]  %s", text[:160])
 
-        return _GenbankRecord(
-            _read(text),
-            item=item,
-            start=seq_start,
-            stop=seq_stop,
-            strand=strand)
+        return _GenbankRecord(_read(text), item=item, start=seq_start, stop=seq_stop, strand=strand)
 
 
 def genbank(accession: str = "CS570233.1", *args, **kwargs):
     """
     Download a genbank nuclotide record.
 
     This function takes the same paramenters as the
```

### Comparing `pydna-5.2.0a9/src/pydna/genbankfile.py` & `pydna-6.0.0a1/src/pydna/genbankfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,25 +17,19 @@
     def from_SeqRecord(cls, record, *args, path=None, **kwargs):
         obj = super().from_SeqRecord(record, *args, **kwargs)
         obj.path = path
         return obj
 
     def __repr__(self):
         """returns a short string representation of the object"""
-        return "File({})({}{})".format(
-            self.id, {True: "-", False: "o"}[self.linear], len(self)
-        )
+        return "File({})({}{})".format(self.id, {True: "-", False: "o"}[not self.circular], len(self))
 
     def _repr_pretty_(self, p, cycle):
         """returns a short string representation of the object"""
-        p.text(
-            "File({})({}{})".format(
-                self.id, {True: "-", False: "o"}[self.linear], len(self)
-            )
-        )
+        p.text("File({})({}{})".format(self.id, {True: "-", False: "o"}[not self.circular], len(self)))
 
     def _repr_html_(self):
         return "<a href='{path}' target='_blank'>{path}</a><br>".format(path=self.path)
 
     def reverse_complement(self):
         answer = type(self)(super().reverse_complement(), path=self.path)
         return answer
```

### Comparing `pydna-5.2.0a9/src/pydna/genbankfixer.py` & `pydna-6.0.0a1/src/pydna/genbankfixer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,30 +29,26 @@
 
 GoodLocus = (
     _pp.Literal("LOCUS")
     + _pp.Word(_pp.alphas + _pp.nums + "-_()." + "\\").setResultsName("name")
     + _pp.Word(_pp.nums).setResultsName("size")
     + _pp.Suppress(_pp.CaselessLiteral("bp"))
     + _pp.Word(_pp.alphas + "-").setResultsName("seqtype")
-    + (_pp.CaselessLiteral("linear") | _pp.CaselessLiteral("circular")).setResultsName(
-        "topology"
-    )
+    + (_pp.CaselessLiteral("linear") | _pp.CaselessLiteral("circular")).setResultsName("topology")
     + _pp.Optional(_pp.Word(_pp.alphas), default="   ").setResultsName("divcode")
     + _pp.Regex(r"(\d{2})-(\S{3})-(\d{4})").setResultsName("date")
 )
 
 # Older versions of ApE don't include a LOCUS name! Need separate def for this case:
 BrokenLocus1 = (
     _pp.Literal("LOCUS").setResultsName("name")
     + _pp.Word(_pp.nums).setResultsName("size")
     + _pp.Suppress(_pp.CaselessLiteral("bp"))
     + _pp.Word(_pp.alphas + "-").setResultsName("seqtype")
-    + (_pp.CaselessLiteral("linear") | _pp.CaselessLiteral("circular")).setResultsName(
-        "topology"
-    )
+    + (_pp.CaselessLiteral("linear") | _pp.CaselessLiteral("circular")).setResultsName("topology")
     + _pp.Optional(_pp.Word(_pp.alphas), default="   ").setResultsName("divcode")
     + _pp.Regex(r"(\d{2})-(\S{3})-(\d{4})").setResultsName("date")
 )
 
 # LOCUS       YEplac181	5741 bp 	DNA	SYN
 BrokenLocus2 = (
     _pp.Literal("LOCUS")
@@ -97,16 +93,15 @@
 # All entries in a genbank file headed by an all-caps title with no space between start-of-line and title
 CapWord = _pp.Word("ABCDEFGHIJKLMNOPQRSTUVWXYZ")
 # after titled line, all subsequent lines have to have at least one space in front of them
 # this is how we split up the genbank record
 SpacedLine = _pp.White(min=1) + _pp.CharsNotIn("\n") + _pp.LineEnd()
 # HeaderLine = CapWord + CharsNotIn("\n") + LineEnd()
 GenericEntry = _pp.Group(
-    CapWord
-    + _pp.Combine(_pp.CharsNotIn("\n") + _pp.LineEnd() + _pp.ZeroOrMore(SpacedLine))
+    CapWord + _pp.Combine(_pp.CharsNotIn("\n") + _pp.LineEnd() + _pp.ZeroOrMore(SpacedLine))
 ).setResultsName("generics", listAllMatches=True)
 
 
 # ===============================================================================
 # Definition Entry
 # SuppressedSpacedLine =  Suppress(White(min=1)) + CharsNotIn("\n") + LineEnd()
 # DefinitionEntry =  Suppress(Literal("DEFINITION")) + Combine(CharsNotIn("\n") + LineEnd() + ZeroOrMore( SuppressedSpacedLine ))
@@ -136,31 +131,33 @@
 # if you don't know where something is, don't use it or guess and move on
 
 LPAREN = _pp.Suppress("(")
 RPAREN = _pp.Suppress(")")
 SEP = _pp.Suppress(_pp.Literal(".."))
 
 # recognize numbers w. < & > uncertainty specs, then strip the <> chars to make it fixed
-gbIndex = _pp.Word(_pp.nums + "<>").setParseAction(
-    lambda s, l, t: int(t[0].replace("<", "").replace(">", ""))
-)
+gbIndex = _pp.Word(_pp.nums + "<>").setParseAction(lambda s, l, t: int(t[0].replace("<", "").replace(">", "")))
 SimpleSlice = _pp.Group(gbIndex + SEP + gbIndex) | _pp.Group(gbIndex).setParseAction(
     lambda s, l, t: [[t[0][0], t[0][0]]]
 )
 
 # recursive def for nested function syntax:  f( g(), g() )
 complexSlice = _pp.Forward()
-complexSlice << (_pp.Literal("complement") | _pp.Literal("join")) + LPAREN + (
-    _pp.delimitedList(complexSlice) | _pp.delimitedList(SimpleSlice)
-) + RPAREN
+(
+    complexSlice
+    << (_pp.Literal("complement") | _pp.Literal("join"))
+    + LPAREN
+    + (_pp.delimitedList(complexSlice) | _pp.delimitedList(SimpleSlice))
+    + RPAREN
+)
 featLocation = _pp.Group(SimpleSlice | complexSlice)
 
 
 def parseGBLoc(s, l, t):
-    """retwingles parsed genbank location strings, assumes no joins of RC and FWD sequences """
+    """retwingles parsed genbank location strings, assumes no joins of RC and FWD sequences"""
     strand = 1
     locationlist = []
 
     # see if there are any complement operators
     for entry in t[0]:
         if entry == "complement":
             strand = -1
@@ -193,68 +190,55 @@
     + _pp.Word(_pp.alphas + _pp.nums + "_-")
     + _pp.Suppress("=")
     + _pp.QuotedString('"', multiline=True).setParseAction(strip_multiline)
 )
 
 # UnQuoted KeyVal: /key=value  (I'm assuming it doesn't do multilines this way? wrong! ApE does store long labels this way! sigh.)
 # NoQuoteFeaturekeyval = Group(Suppress('/') + Word(alphas+nums+"_-") + Suppress('=') + OneOrMore(CharsNotIn("\n")) )
-keyvalspacedline = (
-    _pp.White(exact=21)
-    + _pp.CharsNotIn("/")
-    + _pp.OneOrMore(_pp.CharsNotIn("\n"))
-    + _pp.LineEnd()
-)
+keyvalspacedline = _pp.White(exact=21) + _pp.CharsNotIn("/") + _pp.OneOrMore(_pp.CharsNotIn("\n")) + _pp.LineEnd()
 NoQuoteFeaturekeyval = _pp.Group(
     _pp.Suppress("/")
     + _pp.Word(_pp.alphas + _pp.nums + "_-")
     + _pp.Suppress("=")
-    + _pp.Combine(
-        _pp.CharsNotIn("\n") + _pp.LineEnd() + _pp.ZeroOrMore(keyvalspacedline)
-    )
+    + _pp.Combine(_pp.CharsNotIn("\n") + _pp.LineEnd() + _pp.ZeroOrMore(keyvalspacedline))
 )
 
 # Special Case for Numerical Vals:  /bases=12  OR  /bases="12"
 NumFeaturekeyval = _pp.Group(
     _pp.Suppress("/")
     + _pp.Word(_pp.alphas + _pp.nums + "_-")
     + _pp.Suppress("=")
     + (_pp.Suppress('"') + _pp.Word(_pp.nums).setParseAction(toInt) + _pp.Suppress('"'))
     | (_pp.Word(_pp.nums).setParseAction(toInt))
 )
 
 # Key Only KeyVal: /pseudo
 # post-parse convert it into a pair to resemble the structure of the first three cases i.e. [pseudo, True]
-FlagFeaturekeyval = _pp.Group(
-    _pp.Suppress("/") + _pp.Word(_pp.alphas + _pp.nums + "_-")
-).setParseAction(lambda s, l, t: [[t[0][0], True]])
+FlagFeaturekeyval = _pp.Group(_pp.Suppress("/") + _pp.Word(_pp.alphas + _pp.nums + "_-")).setParseAction(
+    lambda s, l, t: [[t[0][0], True]]
+)
 
 Feature = _pp.Group(
-    _pp.Word(_pp.alphas + _pp.nums + "_-").setParseAction(
-        lambda s, l, t: [["type", t[0]]]
-    )
+    _pp.Word(_pp.alphas + _pp.nums + "_-").setParseAction(lambda s, l, t: [["type", t[0]]])
     + featLocation.setResultsName("location")
-    + _pp.OneOrMore(
-        NumFeaturekeyval | QuoteFeaturekeyval | NoQuoteFeaturekeyval | FlagFeaturekeyval
-    )
+    + _pp.OneOrMore(NumFeaturekeyval | QuoteFeaturekeyval | NoQuoteFeaturekeyval | FlagFeaturekeyval)
 )
 
 FeaturesEntry = (
     _pp.Literal("FEATURES")
     + _pp.Literal("Location/Qualifiers")
     + _pp.Group(_pp.OneOrMore(Feature)).setResultsName("features")
 )
 
 # ===============================================================================
 # GenBank Sequence Parser
 
 # sequence is just a column-spaced big table of dna nucleotides
 # should it recognize full IUPAC alphabet?  NCBI uses n for unknown region
-Sequence = _pp.OneOrMore(
-    _pp.Suppress(_pp.Word(_pp.nums)) + _pp.OneOrMore(_pp.Word("ACGTacgtNn"))
-)
+Sequence = _pp.OneOrMore(_pp.Suppress(_pp.Word(_pp.nums)) + _pp.OneOrMore(_pp.Word("ACGTacgtNn")))
 
 # Group(  ) hides the setResultsName names def'd inside, such that one needs to first access this group and then access the dict of contents inside
 SequenceEntry = _pp.Suppress(_pp.Literal("ORIGIN")) + Sequence.setParseAction(
     lambda s, l, t: "".join(t)
 ).setResultsName("sequence")
 
 
@@ -294,21 +278,19 @@
             newdict[e[0]] = newdict[e[0]] + strip_indent(e[1])
         else:
             newdict[e[0]] = strip_indent(e[1])
     return newdict
 
 
 def toJSON(gbkstring):
-
     parsed = multipleGB.parseString(gbkstring)
 
     jseqlist = []
 
     for seq in parsed:
-
         # for item in seq.asList():
         #    print(item)
 
         # import sys;sys.exit(42)
 
         # Print to STDOUT some details (useful for long multi-record parses)
         # print(seq['name'], ":  length:", len(seq['sequence']) , " #features:" , len(seq['features'].asList()))
@@ -366,17 +348,15 @@
             return str_ + "\n"
 
     # multiple lines so wrap:
     for linenum in range(1 + int(len(str_) / rowlen)):
         if linenum == 0 and not padfirst:
             wrappedstr += str_[linenum * rowlen : (linenum + 1) * rowlen] + "\n"
         else:
-            wrappedstr += (
-                " " * leftpad + str_[linenum * rowlen : (linenum + 1) * rowlen] + "\n"
-            )
+            wrappedstr += " " * leftpad + str_[linenum * rowlen : (linenum + 1) * rowlen] + "\n"
     #    if str_.startswith("/translation="):
     #        print(str_)
     #        print(wrappedstr)
     #        print(".................................")
     return wrappedstr
 
 
@@ -496,17 +476,15 @@
                         "ApEinfo_fwdcolor",
                         "ApEinfo_revcolor",
                         "label",
                     ]:
                         fstr += wrapstring("/" + str(k) + "=" + str(feat[k]), 21, 80)
                     # standard: wrap val in quotes
                     else:
-                        fstr += wrapstring(
-                            "/" + str(k) + "=" + '"' + str(feat[k]) + '"', 21, 80
-                        )
+                        fstr += wrapstring("/" + str(k) + "=" + '"' + str(feat[k]) + '"', 21, 80)
             featuresstr += fstr
 
     # the spaced, numbered sequence
     gborigin = "ORIGIN\n" + originstr(jseq["sequence"]) + "//\n"
 
     return locusstr + gbprops + featuresstr + gborigin
```

### Comparing `pydna-5.2.0a9/src/pydna/genbankrecord.py` & `pydna-6.0.0a1/src/pydna/genbankrecord.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,17 @@
 # license.  Please see the LICENSE.txt file that should have been included
 # as part of this package.
 
 from pydna.dseqrecord import Dseqrecord as _Dseqrecord
 from pydna._pretty import pretty_str as _ps
 import os as _os
 
-class GenbankRecord(_Dseqrecord):
-
-    def __init__(self,
-                 record,
-                 *args,
-                 item="accession",
-                 start=None,
-                 stop=None,
-                 strand=1,
-                 **kwargs):
 
+class GenbankRecord(_Dseqrecord):
+    def __init__(self, record, *args, item="accession", start=None, stop=None, strand=1, **kwargs):
         super().__init__(record, *args, **kwargs)
         self.item = item
         self.start = start
         self.stop = stop
         self.strand = strand
         self._repr = item
         if self.start != None and self.stop != None:
@@ -36,22 +28,15 @@
                 stop=self.stop or "",
                 strand=self.strand,
                 text=self._repr,
             )
         )
 
     @classmethod
-    def from_string(cls,
-                    record: str = "",
-                    *args,
-                    item="accession",
-                    start=None,
-                    stop=None,
-                    strand=1,
-                    **kwargs):
+    def from_string(cls, record: str = "", *args, item="accession", start=None, stop=None, strand=1, **kwargs):
         """docstring."""
         obj = super().from_string(record, *args, **kwargs)
         obj.item = item
         obj.start = start
         obj.stop = stop
         obj.strand = strand
         obj._repr = item
@@ -66,17 +51,15 @@
                 strand=obj.strand,
                 text=obj._repr,
             )
         )
         return obj
 
     @classmethod
-    def from_SeqRecord(
-        cls, record, *args, item="accession", start=None, stop=None, strand=1, **kwargs
-    ):
+    def from_SeqRecord(cls, record, *args, item="accession", start=None, stop=None, strand=1, **kwargs):
         obj = super().from_SeqRecord(record, *args, **kwargs)
         obj.item = item
         obj.start = start
         obj.stop = stop
         obj.strand = strand
         obj._repr = item
         if obj.start is not None and obj.stop is not None:
@@ -92,24 +75,22 @@
             )
         )
         return obj
 
     def __getitem__(self, sl):
         answer = super().__getitem__(sl)
         answer.item = self.item
-        answer.start = self.start or 0 + sl.start
-        answer.stop = self.start or 0 + sl.stop
+        answer.start = (self.start or 0) + (sl.start or 0)
+        answer.stop = (self.start or 0) + (sl.stop or 0)
         answer.strand = self.strand
         return answer
 
     def __repr__(self):
         """returns a short string representation of the object"""
-        return "Gbnk({}{} {})".format({True: "-", False: "o"}[self.linear],
-                                       len(self),
-                                       self._repr)
+        return "Gbnk({}{} {})".format({True: "-", False: "o"}[not self.circular], len(self), self._repr)
 
     def _repr_pretty_(self, p, cycle):
         """returns a short string representation of the object"""
         p.text(self.__repr__())
 
     def _repr_html_(self):
         return self.hyperlink
@@ -125,42 +106,53 @@
         return answer
 
     rc = reverse_complement
 
     def pydna_code(self):
         """docstring."""  # FIXME
 
-        code = ("from pydna.genbank import Genbank\n"
-                f"gb = Genbank('{_os.environ['pydna_email']}')\n"
-                f"seq = gb.nucleotide('{self.item}'")
+        code = (
+            "from pydna.genbank import Genbank\n"
+            f"gb = Genbank('{_os.environ['pydna_email']}')\n"
+            f"seq = gb.nucleotide('{self.item}'"
+        )
         if self.start and self.start:
-
-            code += (",\n"
-                     f"                    seq_start={self.start},\n"
-                     f"                    seq_stop={self.stop},\n"
-                     f"                    strand={self.strand})")
+            code += (
+                ",\n"
+                f"                    seq_start={self.start},\n"
+                f"                    seq_stop={self.stop},\n"
+                f"                    strand={self.strand})"
+            )
         else:
             code += ")"
 
         return _ps(code)
 
     def biopython_code(self):
         """docstring."""  # FIXME
 
-        code = ("from Bio.genbank import Genbank\n"
-                f"gb = Genbank('{_os.environ['pydna_email']}')\n"
-                f"seq = gb.nucleotide('{self.item}'")
-        if self.start and self.start:
-
-            code += (",\n"
-                     f"                    seq_start={self.start},\n"
-                     f"                    seq_stop={self.stop},\n"
-                     f"                    strand={self.strand})")
+        code = (
+            "from Bio import Entrez, SeqIO\n"
+            f"Entrez.email = '{_os.environ['pydna_email']}'\n"
+            "handle = Entrez.efetch(db='nuccore',\n"
+            f"                       id='{self.item}',\n"
+            "                       rettype='gbwithparts',\n"
+            "                       retmode='text',"
+        )
+        if self.start and self.stop:
+            code += (
+                "\n"
+                f"                       seq_start={self.start},\n"
+                f"                       seq_stop={self.stop},\n"
+                f"                       strand={self.strand})\n"
+            )
         else:
-            code += ")"
+            code += ")\n"
+
+        code += "record = SeqIO.read(handle, 'genbank')"
 
         return _ps(code)
 
 
 if __name__ == "__main__":
     import os as _os
```

### Comparing `pydna-5.2.0a9/src/pydna/goldengate.py` & `pydna-6.0.0a1/src/pydna/goldengate.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 _module_logger = _logging.getLogger("pydna." + __name__)
 
 from Bio.Restriction import BsaI, BsmBI, BbsI, FokI
 
 DNA = _Dseqrecord("gatcGAAGACtagagtctgattcg")
 
-a,b = DNA.cut(BbsI)
+a, b = DNA.cut(BbsI)
 
-assert a+b == DNA
+assert a + b == DNA
 
 
 # MoClo
 
 # https://edinburgh-genome-foundry.github.io/GoldenHinges
```

### Comparing `pydna-5.2.0a9/src/pydna/gui.py` & `pydna-6.0.0a1/src/pydna/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 # This code is part of the Python-dna distribution and governed by its
 # license.  Please see the LICENSE.txt file that should have been included
 # as part of this package.
 
 """A DNA sequence widget."""
 
 import sys
+import os
 from PyQt5 import QtWidgets
 from PyQt5.QtWidgets import QMainWindow
 from PyQt5.QtWidgets import QGridLayout
 from PyQt5.QtWidgets import QPlainTextEdit
 from PyQt5.QtWidgets import QWidget
 from PyQt5.QtWidgets import QDesktopWidget
 from PyQt5.QtGui import QFont
 from PyQt5.QtCore import QSize
-import os
 from multiprocessing import Process
 
 
 class SequenceWindow(QMainWindow):
     """docstring."""
 
     def __init__(self, record):
@@ -41,33 +41,35 @@
         font.setPointSize(16)
         centralWidget.setFont(font)
         textw = QPlainTextEdit()
 
         text = str(record.seq)
         html = ""
         for fl in record.features[0].location.parts:
-            html = (f"{text[:fl.start]}<span style='background-color:#ffff00;'>"
-                    f"{text[fl.start:fl.end]}</span>"
-                    f"{text[fl.end:]}")
+            html = (
+                f"{text[:fl.start]}<span style='background-color:#ffff00;'>"
+                f"{text[fl.start:fl.end]}</span>"
+                f"{text[fl.end:]}"
+            )
 
         textw.appendHtml(html)
         textw.setReadOnly(True)
         gridLayout.addWidget(textw, 0, 0)
 
+
 def run_app(record):
     if os.fork() != 0:
         return
     app = QtWidgets.QApplication(sys.argv)
     app.mainWin = SequenceWindow(record)
     app.mainWin.show()
     app.exec_()
 
 
 if __name__ == '__main__':
-
     t = """
         LOCUS       myDNA                     12 bp    DNA     linear       02-JAN-2023
         DEFINITION  .
         ACCESSION
         VERSION
         SOURCE      .
           ORGANISM  .
```

### Comparing `pydna-5.2.0a9/src/pydna/ladders.py` & `pydna-6.0.0a1/src/pydna/ladders.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,15 @@
 a gel image. Exampel can be found in scripts/molecular_weight_standards.ods.
 """
 
 
 from pydna.fakeseq import FakeSeq as _FakeSeq
 
 
-PennStateLadder = [
-    _FakeSeq(int(n))
-    for n in (10000, 7750, 5000, 4000, 3000, 2000, 1500, 1000, 750, 500)
-]
+PennStateLadder = [_FakeSeq(int(n)) for n in (10000, 7750, 5000, 4000, 3000, 2000, 1500, 1000, 750, 500)]
 
 
 GeneRuler_1kb = [
     _FakeSeq(int(n))
     for n in (
         10000,
         8000,
@@ -41,19 +38,22 @@
         1000,
         750,
         500,
         250,
     )
 ]
 
+# Google spreadsheet to make the ladders below
+# https://docs.google.com/spreadsheets/d/1vN0y75ibxPrG6yJQjq1uF2FXP0L-qGSn_fzInUHeTs4/edit#gid=0
 
 GeneRuler_1kb_plus = [
     _FakeSeq(ln, n=n * 1e-15, rf=rf)
     for ln, n, rf in (
-        (20000, 1.538, 0.000),  # ( length, fmol, Rf )
+        # (length, fmol, Rf )
+        (20000, 1.538, 0.000),
         (10000, 3.077, 0.040),
         (7000, 4.396, 0.096),
         (5000, 23.077, 0.154),
         (4000, 7.692, 0.201),
         (3000, 10.256, 0.261),
         (2000, 15.385, 0.362),
         (1500, 82.051, 0.443),
@@ -67,14 +67,15 @@
     )
 ]
 
 
 HI_LO_DNA_MARKER = [
     _FakeSeq(ln, n=n * 1e-15, rf=rf)
     for ln, n, rf in (
+        # (length, fmol, Rf )
         (10000, 4.545, 0.000),
         (8000, 5.682, 0.013),
         (6000, 11.364, 0.037),
         (4000, 22.727, 0.081),
         (3000, 42.929, 0.131),
         (2000, 113.636, 0.236),
         (1550, 97.752, 0.302),
```

### Comparing `pydna-5.2.0a9/src/pydna/myenzymes.py` & `pydna-6.0.0a1/src/pydna/myenzymes.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,23 +30,19 @@
     with open(_os.environ["pydna_enzymes"], encoding="utf-8") as _f:
         _text = _f.read()
 except FileNotFoundError:
     _module_logger.warning("%s not found.", _os.environ["pydna_enzymes"])
 except IsADirectoryError:
     _module_logger.warning("%s is a directory.", _os.environ["pydna_enzymes"])
 except IOError:
-    _module_logger.warning(
-        "%s found, but could not be read.", _os.environ["pydna_enzymes"]
-    )
+    _module_logger.warning("%s found, but could not be read.", _os.environ["pydna_enzymes"])
 except Exception as e:
     _module_logger.warning(_traceback.format_exc())
 
-myenzymes = _RestrictionBatch(
-    [e for e in _AllEnzymes if str(e).lower() in _text.lower()]
-)
+myenzymes = _RestrictionBatch([e for e in _AllEnzymes if str(e).lower() in _text.lower()])
 
 if __name__ == "__main__":
     cache = _os.getenv("pydna_cache")
     _os.environ["pydna_cache"] = "nocache"
     import doctest
 
     doctest.testmod(verbose=True, optionflags=doctest.ELLIPSIS)
```

### Comparing `pydna-5.2.0a9/src/pydna/myprimers.py` & `pydna-6.0.0a1/src/pydna/myprimers.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,31 +59,25 @@
     primers at the top of the list.
 
     The primer list remembers the numbers of accessed primers.
     The indices of accessed primers are stored in the .accessed
     property.
     """
 
-    def __init__(self,
-                 initlist: Iterable = None,
-                 path: (str, Path) = None,
-                 *args,
-                 identifier: str = "p",
-                 **kwargs):
+    def __init__(self, initlist: Iterable = None, path: (str, Path) = None, *args, identifier: str = "p", **kwargs):
         if initlist:
             self.data = initlist
             self.path = None
         else:
             self.path = Path(path or _os.environ["pydna_primers"])
             self.path.parent.mkdir(parents=True, exist_ok=True)
             self.data = _parse_primers(self.path.read_text())[::-1]
         # super().__init__(*args, **kwargs)
         self.accessed_indices = []
-        if (identifier.isidentifier() and not _iskeyword(identifier)
-           and identifier not in _kw):
+        if identifier.isidentifier() and not _iskeyword(identifier) and identifier not in _kw:
             self.identifier = identifier
         else:
             raise ValueError(f"{identifier} is not a valid identifier.")
 
     def __getitem__(self, i):
         """Save indices of accessed items."""
         if isinstance(i, slice):
@@ -91,15 +85,15 @@
             for ind in range(i.start, i.stop, i.step or 1):
                 if ind not in self.accessed_indices:
                     self.accessed_indices.append(ind)
         else:
             try:
                 result = self.data[i]
             except IndexError as e:
-                raise(e)
+                raise (e)
             else:
                 if i not in self.accessed_indices:
                     self.accessed_indices.append(i)
         return result
 
     def __setitem__(self, i, item):
         """Items already present can be set to the same value."""
```

### Comparing `pydna-5.2.0a9/src/pydna/primer.py` & `pydna-6.0.0a1/src/pydna/primer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,15 @@
 from pydna.seq import Seq as _Seq
 from pydna.seqrecord import SeqRecord as _SeqRecord
 
 
 class Primer(_SeqRecord):
     """Primer and its position on a template, footprint and tail."""
 
-    def __init__(self,
-                 record,
-                 *args,
-                 amplicon=None,
-                 position=None,
-                 footprint=0,
-                 **kwargs):
-
+    def __init__(self, record, *args, amplicon=None, position=None, footprint=0, **kwargs):
         if hasattr(record, "features"):  # Seqrecord
             self.__dict__.update(record.__dict__)
             self.__dict__.update(kwargs)
         elif hasattr(record, "transcribe"):  # Seq
             super().__init__(record, *args, **kwargs)
         else:  # string?
             super().__init__(_Seq(record), *args, **kwargs)
@@ -61,14 +54,15 @@
         """Return the reverse complement of the sequence."""
         answer = super().reverse_complement(*args, **kwargs)
         answer.amplicon = None
         answer.position = None
         answer._fp = len(self)
         return answer
 
+
 if __name__ == "__main__":
     import os as _os
 
     cached = _os.getenv("pydna_cached_funcs", "")
     _os.environ["pydna_cached_funcs"] = ""
     import doctest
```

### Comparing `pydna-5.2.0a9/src/pydna/readers.py` & `pydna-6.0.0a1/src/pydna/readers.py`

 * *Files identical despite different names*

### Comparing `pydna-5.2.0a9/src/pydna/seq.py` & `pydna-6.0.0a1/src/pydna/seq.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,34 +26,31 @@
 
 _module_logger = _logging.getLogger("pydna." + __name__)
 
 
 class Seq(_Seq):
     """docstring."""
 
-    def __init__(self, data, length=None):
-        super().__init__(data, length=None)
-
     def gc(self):
         """Return GC content."""
         return round(_GC(self._data.upper().decode("ASCII")), 3)
 
     def cai(self, organism="sce"):
         """docstring."""
-        from CAI import CAI as _CAI
-        return round(_CAI(self._data.upper().decode("ASCII"),
-                          weights=_weights[organism]), 3)
+        from pydna.utils import cai as _cai
+
+        return _cai(self._data.upper().decode("ASCII"), organism=organism)
 
     def rarecodons(self, organism="sce"):
         """docstring."""
         rare = _rare_codons[organism]
         s = self._data.upper().decode("ASCII")
         slices = []
-        for i in range(0, len(self)//3):
-            x, y = i*3, i*3+3
+        for i in range(0, len(self) // 3):
+            x, y = i * 3, i * 3 + 3
             trip = s[x:y]
             if trip in rare:
                 slices.append(slice(x, y, 1))
         return slices
 
     def startcodon(self, organism="sce"):
         """docstring."""
@@ -61,41 +58,38 @@
 
     def stopcodon(self, organism="sce"):
         """docstring."""
         return _stop[organism].get(self._data.upper().decode("ASCII")[-3:])
 
     def express(self, organism="sce"):
         """docstring."""
-        x = _PrettyTable(["cds", "len", "cai", "gc", "sta", "stp",
-                          "n-end"]+_rare_codons[organism]+["rare"])
+        x = _PrettyTable(["cds", "len", "cai", "gc", "sta", "stp", "n-end"] + _rare_codons[organism] + ["rare"])
         val = []
 
-        val.append(f"{self._data.upper().decode('ASCII')[:3]}..."
-                   f"{self._data.upper().decode('ASCII')[-3:]}")
-        val.append(len(self)/3)
+        val.append(f"{self._data.upper().decode('ASCII')[:3]}..." f"{self._data.upper().decode('ASCII')[-3:]}")
+        val.append(len(self) / 3)
         val.append(self.cai(organism))
         val.append(self.gc())
         val.append(self.startcodon())
         val.append(self.stopcodon())
         val.append(_n_end[organism].get(_seq3(self[3:6].translate())))
         s = self._data.upper().decode("ASCII")
-        trps = [s[i*3:i*3+3] for i in range(0, len(s)//3)]
+        trps = [s[i * 3 : i * 3 + 3] for i in range(0, len(s) // 3)]
         tot = 0
         for cdn in _rare_codons[organism]:
             cnt = trps.count(cdn)
             tot += cnt
             val.append(cnt)
-        val.append(round(tot/len(trps), 3))
+        val.append(round(tot / len(trps), 3))
         x.add_row(val)
         return x
 
     def orfs(self, minsize=30):
         """docstring."""
-        orf = _re.compile(f"ATG(?:...){{{minsize},}}?(?:TAG|TAA|TGA)",
-                          flags=_re.IGNORECASE)
+        orf = _re.compile(f"ATG(?:...){{{minsize},}}?(?:TAG|TAA|TGA)", flags=_re.IGNORECASE)
         start = 0
         matches = []
         s = self._data.decode("ASCII")
 
         while True:
             match = orf.search(s, pos=start)
             if match:
@@ -122,16 +116,16 @@
 
         References
         ----------
         .. [#] http://wiki.christophchamp.com/index.php/SEGUID
         """
         return _useg(self._data)
 
-if __name__ == "__main__":
 
+if __name__ == "__main__":
     import os as _os
 
     cached = _os.getenv("pydna_cached_funcs", "")
     _os.environ["pydna_cached_funcs"] = ""
     import doctest
 
     doctest.testmod(verbose=True, optionflags=doctest.ELLIPSIS)
```

### Comparing `pydna-5.2.0a9/src/pydna/seqrecord.py` & `pydna-6.0.0a1/src/pydna/seqrecord.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 the :class:`pydna._pretty_str.pretty_str` class instread of str for a
 nicer output in the IPython shell.
 """
 
 
 from Bio.SeqFeature import SeqFeature as _SeqFeature
 from pydna._pretty import pretty_str as _pretty_str
+
 # from pydna.utils import seguid as _seg
 from pydna.common_sub_strings import common_sub_strings as _common_sub_strings
 
 from Bio.Data.CodonTable import TranslationError as _TranslationError
 from Bio.SeqRecord import SeqRecord as _SeqRecord
 from Bio.SeqFeature import SimpleLocation as _SimpleLocation
 from Bio.SeqFeature import CompoundLocation as _CompoundLocation
@@ -45,42 +46,31 @@
     A subclass of the Biopython SeqRecord class.
 
     Has a number of extra methods and uses
     the :class:`pydna._pretty_str.pretty_str` class instread of str for a
     nicer output in the IPython shell.
     """
 
-    def __init__(self,
-                 *args,
-                 id="id",
-                 name="name",
-                 description="description",
-                 **kwargs):
-
-        super().__init__(*args,
-                         id = id,
-                         name = name,
-                         description = description,
-                         **kwargs)
+    def __init__(self, *args, id="id", name="name", description="description", **kwargs):
+        super().__init__(*args, id=id, name=name, description=description, **kwargs)
         self._fix_attributes()
 
     def _fix_attributes(self):
         self.id = _pretty_str(self.id)
         self.name = _pretty_str(self.name)
         self.description = _pretty_str(self.description)
 
         self.annotations.update({"molecule_type": "DNA"})
         self.map_target = None
 
         if not hasattr(self.seq, "transcribe"):
             self.seq = _Seq(self.seq)
 
         self.seq._data = b"".join(self.seq._data.split())  # remove whitespaces
-        self.annotations = {_pretty_str(k): _pretty_str(v) for k, v in
-                            self.annotations.items()}
+        self.annotations = {_pretty_str(k): _pretty_str(v) for k, v in self.annotations.items()}
 
     @classmethod
     def from_Bio_SeqRecord(clc, sr: _SeqRecord):
         """Creates a pydnaSeqRecord from a Biopython SeqRecord."""
         # https://stackoverflow.com/questions/15404256/changing-the-\
         # class-of-a-python-object-casting
         sr.__class__ = clc
@@ -94,17 +84,15 @@
 
     @locus.setter
     def locus(self, value):
         """Alias for name property."""
         if len(value) > 16:
             shortvalue = value[:16]
             _warn(
-                ("locus property {} truncated"
-                 "to 16 chars {}").format(value,
-                                          shortvalue),
+                ("locus property {} truncated" "to 16 chars {}").format(value, shortvalue),
                 _PydnaWarning,
                 stacklevel=2,
             )
             value = shortvalue
         self.name = value
         return
 
@@ -219,20 +207,15 @@
             "#66ffff",
         )
 
         for i, f in enumerate(self.features):
             f.qualifiers["ApEinfo_fwdcolor"] = [cols[i % len(cols)]]
             f.qualifiers["ApEinfo_revcolor"] = [cols[::-1][i % len(cols)]]
 
-    def add_feature(self,
-                    x=None,
-                    y=None,
-                    seq=None,
-                    type_="misc",
-                    strand=1, *args, **kwargs):
+    def add_feature(self, x=None, y=None, seq=None, type_="misc", strand=1, *args, **kwargs):
         """Add a feature of type misc to the feature list of the sequence.
 
         Parameters
         ----------
         x  : int
             Indicates start of the feature
         y  : int
@@ -275,29 +258,24 @@
         if "label" not in qualifiers:
             qualifiers["label"] = ["ft{}".format(y - x)]
 
             if self[x:y].isorf() or self[x:y].reverse_complement().isorf():
                 qualifiers["label"] = ["orf{}".format(y - x)]
 
         try:
-            location = _SimpleLocation(x,
-                                       y,
-                                       strand=strand)
+            location = _SimpleLocation(x, y, strand=strand)
         except ValueError as err:
             if self.circular:
                 location = _CompoundLocation(
-                    (_SimpleLocation(x, self.seq.length, strand=strand),
-                     _SimpleLocation(0, y, strand=strand))
-                                              )
+                    (_SimpleLocation(x, self.seq.length, strand=strand), _SimpleLocation(0, y, strand=strand))
+                )
             else:
                 raise err
 
-        sf = _SeqFeature(location,
-                         type=type_,
-                         qualifiers=qualifiers)
+        sf = _SeqFeature(location, type=type_, qualifiers=qualifiers)
 
         self.features.append(sf)
 
         """
         In [11]: a.seq.translate()
         Out[11]: Seq('K', ExtendedIUPACProtein())
         """
@@ -314,18 +292,15 @@
         >>> print(a.list_features())
         +-----+---------------+-----+-----+-----+-----+------+------+
         | Ft# | Label or Note | Dir | Sta | End | Len | type | orf? |
         +-----+---------------+-----+-----+-----+-----+------+------+
         |   0 | L:ft2         | --> | 2   | 4   |   2 | misc |  no  |
         +-----+---------------+-----+-----+-----+-----+------+------+
         """
-        x = _PrettyTable(
-            ["Ft#", "Label or Note", "Dir",
-             "Sta", "End", "Len", "type", "orf?"]
-        )
+        x = _PrettyTable(["Ft#", "Label or Note", "Dir", "Sta", "End", "Len", "type", "orf?"])
         x.align["Ft#"] = "r"  # Left align
         x.align["Label or Note"] = "l"  # Left align
         x.align["Len"] = "r"
         x.align["Sta"] = "l"
         x.align["End"] = "l"
         x.align["type"] = "l"
         x.padding_width = 1  # One space between column edges and contents
@@ -347,16 +322,15 @@
                     lbl[:16],
                     {1: "-->", -1: "<--", 0: "---", None: "---"}[sf.strand],
                     sf.location.start,
                     sf.location.end,
                     len(sf),
                     sf.type,
                     {True: "yes", False: "no"}[
-                        self.extract_feature(i).isorf()
-                        or self.extract_feature(i).reverse_complement().isorf()
+                        self.extract_feature(i).isorf() or self.extract_feature(i).reverse_complement().isorf()
                     ],
                 ]
             )
         return x
 
     def extract_feature(self, n):
         """Extract feature and return a new SeqRecord object.
@@ -433,20 +407,15 @@
             result = _pretty_str(self.annotations["comment"])
         return result
 
     def datefunction():
         """docstring."""
         return datetime.datetime.now().replace(microsecond=0).isoformat()
 
-    def stamp(self,
-              algorithm,
-              now=datefunction,
-              tool="pydna",
-              separator=" ",
-              comment=""):
+    def stamp(self, algorithm, now=datefunction, tool="pydna", separator=" ", comment=""):
         """Add a uSEGUID or cSEGUID checksum.
 
         The checksum is stored in object.annotations["comment"].
         This shows in the COMMENTS section of a formatted genbank file.
 
         For blunt linear sequences:
 
@@ -468,44 +437,41 @@
         >>> a.stamp("uSEGUID")
         'gBw0Jp907Tg_yX3jNgS4qQWttjU'
         >>> a.annotations["comment"][:41]
         'pydna uSEGUID gBw0Jp907Tg_yX3jNgS4qQWttjU'
         """
         oldcomment = self.annotations.get("comment", "")
 
-        algorithm = _re.sub("seguid",
-                            "SEGUID",
-                            algorithm,
-                            flags=_re.IGNORECASE)
+        algorithm = _re.sub("seguid", "SEGUID", algorithm, flags=_re.IGNORECASE)
 
         chksum = getattr(self.seq, algorithm.lower())()
 
-        pattern = (r"(?i)(?P<algorithm>(c|l|u)?SEGUID)"
-                   r"(?:_|\s|:){1,5}(?P<sha1>\S{27})"
-                   r"(?P<iso>(?:\s([1-9][0-9]*)?[0-9]{4})-(1[0-2]|0[1-9])-"
-                   r"(3[01]|0[1-9]|[12][0-9])T(2[0-3]|[01][0-9]):([0-5][0-9])"
-                   r":([0-5][0-9])(\.[0-9]+)?(Z|[+-](?:2[0-3]|[01][0-9]):"
-                   r"[0-5][0-9])?)?")
+        pattern = (
+            r"(?i)(?P<algorithm>(c|l|u)?SEGUID)"
+            r"(?:_|\s|:){1,5}(?P<sha1>\S{27})"
+            r"(?P<iso>(?:\s([1-9][0-9]*)?[0-9]{4})-(1[0-2]|0[1-9])-"
+            r"(3[01]|0[1-9]|[12][0-9])T(2[0-3]|[01][0-9]):([0-5][0-9])"
+            r":([0-5][0-9])(\.[0-9]+)?(Z|[+-](?:2[0-3]|[01][0-9]):"
+            r"[0-5][0-9])?)?"
+        )
 
         oldstamp = _re.search(pattern, oldcomment)
 
         if oldstamp:
             old_stamp = oldstamp.group(0)
             old_algorithm = oldstamp.group("algorithm")
             old_chksum = oldstamp.group("sha1")
             old_iso = oldstamp.group("iso")
             if chksum == old_chksum and algorithm == old_algorithm:
                 return _pretty_str(oldstamp.group(0))
             else:
-                _warn(f"Stamp change.\nNew: {algorithm} {chksum}\nOld: {old_stamp}",
-                      _PydnaWarning)
+                _warn(f"Stamp change.\nNew: {algorithm} {chksum}\nOld: {old_stamp}", _PydnaWarning)
 
         # now = datetime.datetime.now().replace(microsecond=0).isoformat()
-        self.annotations["comment"] = (f"{oldcomment}\n"
-                                       f"{tool} {algorithm} {chksum} {now()} {comment}").strip()
+        self.annotations["comment"] = (f"{oldcomment}\n" f"{tool} {algorithm} {chksum} {now()} {comment}").strip()
         return _pretty_str(chksum)
 
     def lcs(self, other, *args, limit=25, **kwargs):
         """Return the longest common substring between the sequence.
 
         and another sequence (other). The other sequence can be a string,
         Seq, SeqRecord, Dseq or DseqRecord.
@@ -539,17 +505,15 @@
             if hasattr(r, "watson"):
                 r = str(r.watson).lower()
             else:
                 r = str(r).lower()
         else:
             r = str(other.lower())
 
-        olaps = _common_sub_strings(str(self.seq).lower(),
-                                    r,
-                                    limit=limit or 25)
+        olaps = _common_sub_strings(str(self.seq).lower(), r, limit=limit or 25)
 
         try:
             start_in_self, start_in_other, length = olaps.pop(0)
         except IndexError:
             result = _SeqFeature()
         else:
             label = "sequence" if not hasattr(other, "name") else other.name
@@ -573,17 +537,19 @@
         return self.seq.cai(organism=organism)
 
     def rarecodons(self, organism="sce"):
         """docstring."""
         sfs = []
         for slc in self.seq.rarecodons(organism):
             cdn = self.seq._data[slc].decode("ASCII")
-            sfs.append(_SeqFeature(_SimpleLocation(slc.start, slc.stop),
-                                   type=f"rare_codon_{organism}",
-                                   qualifiers={"label": [cdn]}))
+            sfs.append(
+                _SeqFeature(
+                    _SimpleLocation(slc.start, slc.stop), type=f"rare_codon_{organism}", qualifiers={"label": [cdn]}
+                )
+            )
         return sfs
 
     def startcodon(self, organism="sce"):
         """docstring."""
         return self.seq.startcodon()
 
     def stopcodon(self, organism="sce"):
@@ -613,29 +579,27 @@
         except AttributeError:
             # I don't know how to compare to other
             return NotImplemented
 
     def __eq__(self, other):
         """docstring."""
         try:
-            if (self.seq == other.seq and
-               str(self.__dict__) == str(other.__dict__)):
+            if self.seq == other.seq and str(self.__dict__) == str(other.__dict__):
                 return True
         except AttributeError:
             pass
         return False
 
     def __ne__(self, other):
         """docstring."""
         return not self.__eq__(other)
 
     def __hash__(self):
         """__hash__ must be based on __eq__."""
-        return hash((str(self.seq).lower(),
-                     str(tuple(sorted(self.__dict__.items())))))
+        return hash((str(self.seq).lower(), str(tuple(sorted(self.__dict__.items())))))
 
     def __str__(self):
         """docstring."""
         return _pretty_str(super().__str__())
 
     def __repr__(self):
         """docstring."""
@@ -691,14 +655,15 @@
         object behaviour)!
         """
         return bool(self.seq)
 
     def dump(self, filename, protocol=None):
         """docstring."""
         from pathlib import Path
+
         pth = Path(filename)
         if not pth.suffix:
             pth = pth.with_suffix(".pickle")
         with open(pth, 'wb') as f:
             _pickle.dump(self, f, protocol=protocol)
         return _pretty_str(pth)
 
@@ -706,11 +671,9 @@
 if __name__ == "__main__":
     import os as _os
 
     cached = _os.getenv("pydna_cached_funcs", "")
     _os.environ["pydna_cached_funcs"] = ""
     import doctest
 
-    doctest.testmod(verbose=True,
-                    optionflags=(doctest.ELLIPSIS |
-                                 doctest.NORMALIZE_WHITESPACE))
+    doctest.testmod(verbose=True, optionflags=(doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE))
     _os.environ["pydna_cached_funcs"] = cached
```

### Comparing `pydna-5.2.0a9/src/pydna/sequence_picker.py` & `pydna-6.0.0a1/src/pydna/sequence_picker.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,47 +13,51 @@
 
 _module_logger = _logging.getLogger("pydna." + __name__)
 
 
 email = _os.getenv("pydna_email")
 tool = "pydna"
 
+
 def genbank_accession(s: str):
     """docstring."""
     s = Dseqrecord(s)
 
     NCBIWWW.email = email
-    NCBIWWW.tool =  tool
+    NCBIWWW.tool = tool
 
-    result_handle = NCBIWWW.qblast("blastn",
-                                   "nt",
-                                   str(s.seq),
-                                   hitlist_size=1,
-                                   alignments=1,
-                                   descriptions=1,
-                                   expect=1e-8,
-                                   megablast=True,
-                                   service="megablast",
-                                   ungapped_alignment=True)
+    result_handle = NCBIWWW.qblast(
+        "blastn",
+        "nt",
+        str(s.seq),
+        hitlist_size=1,
+        alignments=1,
+        descriptions=1,
+        expect=1e-8,
+        megablast=True,
+        service="megablast",
+        ungapped_alignment=True,
+    )
 
     blast_records = NCBIXML.read(result_handle)
     best_alignment, *rest = blast_records.alignments
     best_hsp, *rest = best_alignment.hsps
     dbs = best_hsp.sbjct
     start, stop = sorted((best_hsp.sbjct_start, best_hsp.sbjct_end))
-    result = Dseqrecord(dbs,
-                        linear=True,
-                        id=s.name,
-                        name=s.name,
-                        description=(f"{best_alignment.accession} "
-                                     f"REGION: {start}..{stop}"))
+    result = Dseqrecord(
+        dbs,
+        linear=True,
+        id=s.name,
+        name=s.name,
+        description=(f"{best_alignment.accession} " f"REGION: {start}..{stop}"),
+    )
     return result
 
 
 if __name__ == "__main__":
     cached = _os.getenv("pydna_cached_funcs", "")
     _os.environ["pydna_cached_funcs"] = ""
     import doctest
 
     doctest.testmod(verbose=True, optionflags=doctest.ELLIPSIS)
     _os.environ["pydna_cached_funcs"] = cached
-    pass
+    pass
```

### Comparing `pydna-5.2.0a9/src/pydna/tm.py` & `pydna-6.0.0a1/src/pydna/tm.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,23 +115,19 @@
 
     according to:
 
     Rychlik, Spencer, and Rhoads, 1990, Optimization of the anneal
     ing temperature for DNA amplification in vitro
     http://www.ncbi.nlm.nih.gov/pubmed/2243783
     """
-    tmp = 81.5 + 0.41 * _GC(seq) * 100 + 16.6 * _math.log10(K) - 675/len(seq)
+    tmp = 81.5 + 0.41 * _GC(seq) * 100 + 16.6 * _math.log10(K) - 675 / len(seq)
     return tmp
 
 
-def ta_default(fp: str,
-               rp: str,
-               seq: str,
-               tm=tm_default,
-               tm_product=tm_product):
+def ta_default(fp: str, rp: str, seq: str, tm=tm_default, tm_product=tm_product):
     """Ta calculation.
 
     according to:
 
     Rychlik, Spencer, and Rhoads, 1990, Optimization of the anneal
     ing temperature for DNA amplification in vitro
     http://www.ncbi.nlm.nih.gov/pubmed/2243783
@@ -157,15 +153,15 @@
      |3min|30s  \ 59.1°C _____|____|60s/kb
      |    |      \______/ 0:32|5min|GC 51%
      |    |       30s         |    |1051bp
 
     """
 
     taq_extension_rate = 45  # seconds/kB PCR product length (1min/kb)
-    extension_time_taq = max(30, int(taq_extension_rate*len(amplicon)/1000))
+    extension_time_taq = max(30, int(taq_extension_rate * len(amplicon) / 1000))
     # seconds
 
     f = _textwrap.dedent(
         r"""
         |95°C|95°C               |    |tmf:{tmf:.1f}
         |____|_____          72°C|72°C|tmr:{tmr:.1f}
         |3min|30s  \ {ta:.1f}°C _____|____|{rate}s/kb
@@ -180,17 +176,18 @@
                     amplicon.reverse_primer.footprint,
                     str(amplicon.seq),
                 ),
                 1,
             ),
             tmf=tm(amplicon.forward_primer.footprint),
             tmr=tm(amplicon.reverse_primer.footprint),
-            GC=int(amplicon.gc()*100),
+            GC=int(amplicon.gc() * 100),
             *map(int, divmod(extension_time_taq, 60)),
-        )).strip()
+        )
+    ).strip()
 
     return _pretty_str(f)
 
 
 taq_program = program
 
 
@@ -212,64 +209,68 @@
      |____|____      |    |tmr:84.4
      |30s |10s \ 72°C|72°C|15s/kb
      |    |     \____|____|GC 52%
      |    |      3:45|5min|15058bp
 
     """
     PfuSso7d_extension_rate = 15  # seconds/kB PCR product
-    extension_time_PfuSso7d = max(10,
-                                  int(PfuSso7d_extension_rate
-                                      * len(amplicon)/1000))  # seconds
+    extension_time_PfuSso7d = max(10, int(PfuSso7d_extension_rate * len(amplicon) / 1000))  # seconds
 
     # The program returned is eaither a two step or three step progrem
     # This depends on the tm and length of the primers in the
     # original instructions from finnzyme. These do not seem to be
 
     # Ta calculation for enzymes with dsDNA binding domains like phusion or Pfu-Sso7d
     # https://www.finnzymes.fi/tm_determination.html
 
     tmf = tm(amplicon.forward_primer.footprint)
     tmr = tm(amplicon.reverse_primer.footprint)
 
     if tmf >= 69.0 and tmr >= 69.0:
-
-        f = _textwrap.dedent(r"""
+        f = _textwrap.dedent(
+            r"""
                               |98°C|98°C      |    |tmf:{tmf:.1f}
                               |____|____      |    |tmr:{tmr:.1f}
                               |30s |10s \ 72°C|72°C|{rate}s/kb
                               |    |     \____|____|GC {GC_prod}%
                               |    |     {0:2}:{1:0>2}|5min|{size}bp
                               """.format(
                 rate=PfuSso7d_extension_rate,
                 tmf=tmf,
                 tmr=tmr,
-                GC_prod=int(amplicon.gc()*100),
+                GC_prod=int(amplicon.gc() * 100),
                 size=len(amplicon.seq),
-                *map(int, divmod(extension_time_PfuSso7d, 60)))).strip()
+                *map(int, divmod(extension_time_PfuSso7d, 60)),
+            )
+        ).strip()
     else:
         f = _textwrap.dedent(
             r"""
              |98°C|98°C               |    |tmf:{tmf:.1f}
              |____|_____          72°C|72°C|tmr:{tmr:.1f}
              |30s |10s  \ {ta:.1f}°C _____|____|{rate}s/kb
              |    |      \______/{0:2}:{1:0>2}|5min|GC {GC}%
              |    |       10s         |    |{size}bp
              """.format(
-             rate=PfuSso7d_extension_rate,
-             size=len(amplicon.seq),
-             ta=round(
-              ta(amplicon.forward_primer.footprint,
-                 amplicon.reverse_primer.footprint,
-                 amplicon.seq,),
-                 1,
+                rate=PfuSso7d_extension_rate,
+                size=len(amplicon.seq),
+                ta=round(
+                    ta(
+                        amplicon.forward_primer.footprint,
+                        amplicon.reverse_primer.footprint,
+                        amplicon.seq,
+                    ),
+                    1,
                 ),
                 tmf=tmf,
                 tmr=tmr,
-                GC=int(amplicon.gc()*100),
-                *map(int, divmod(extension_time_PfuSso7d, 60)))).strip()
+                GC=int(amplicon.gc() * 100),
+                *map(int, divmod(extension_time_PfuSso7d, 60)),
+            )
+        ).strip()
 
     return _pretty_str(f)
 
 
 pfu_sso7d_program = dbd_program
 
 
@@ -319,18 +320,15 @@
 
     for i in range(len(STR) - 1):
         n1 = ord(STR[i])
         n2 = ord(STR[i + 1])
         dH += _thermodynamic_data.dHBr[n1 - 97][n2 - 97]
         dS += _thermodynamic_data.dSBr[n1 - 97][n2 - 97]
 
-    tm = (
-        dH / (1.9872 * _math.log(pri / 1600) + dS)
-        + (16.6 * _math.log(saltc)) / _math.log(10)
-    ) - 273.15
+    tm = (dH / (1.9872 * _math.log(pri / 1600) + dS) + (16.6 * _math.log(saltc)) / _math.log(10)) - 273.15
 
     return tm
 
 
 if __name__ == "__main__":
     import os as _os
```

### Comparing `pydna-5.2.0a9/src/pydna/utils.py` & `pydna-6.0.0a1/src/pydna/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 # -*- coding: utf-8 -*-
 # Copyright 2013-2023 by Björn Johansson.  All rights reserved.
 # This code is part of the Python-dna distribution and governed by its
 # license.  Please see the LICENSE.txt file that should have been included
 # as part of this package.
 """Miscellaneous functions."""
 
-from Bio.Data.IUPACData import (ambiguous_dna_complement as
-                                _ambiguous_dna_complement)
+from Bio.Data.IUPACData import ambiguous_dna_complement as _ambiguous_dna_complement
 from Bio.Seq import _maketrans
 from pydna._pretty import pretty_str as _pretty_str
 from Bio.SeqUtils.CheckSum import seguid as _seguid
 import shelve as _shelve
 import os as _os
 import re as _re
 import logging as _logging
 import base64 as _base64
 import pickle as _pickle
 import hashlib as _hashlib
 import keyword as _keyword
 import collections as _collections
 import itertools as _itertools
-
+from array import array as _array
 import sys as _sys
 import re
 import textwrap
 import itertools
 import math
 import random
 import subprocess as _subprocess
@@ -58,113 +57,129 @@
         elif oe == ns:
             part = newparts.pop()
             part._end = ne
             ns = part.start
         if ns < ne:
             newparts.append(_sl(ns, ne, strand))
         else:
-            parttuple = (_sl(ns, lim, strand),
-                         _sl(0,  ne,  strand))
+            parttuple = (_sl(ns, lim, strand), _sl(0, ne, strand))
             newparts.extend(parttuple if strand == 1 else parttuple[::-1])
     try:
         newloc = _cl(newparts)
     except ValueError:
         newloc, *n = newparts
     assert len(newloc) == len(original_location)
     return newloc
 
 
+# def smallest_rotation(s):
+#     """Smallest rotation of a string.
+
+#     Algorithm described in Pierre Duval, Jean. 1983. Factorizing Words
+#     over an Ordered Alphabet. Journal of Algorithms & Computational Technology
+#     4 (4) (December 1): 363–381. and Algorithms on strings and sequences based
+#     on Lyndon words, David Eppstein 2011.
+#     https://gist.github.com/dvberkel/1950267
+
+#     Examples
+#     --------
+#     >>> from pydna.utils import smallest_rotation
+#     >>> smallest_rotation("taaa")
+#     'aaat'
+
+#     """
+#     prev, rep = None, 0
+#     ds = _array("u", 2 * s)
+#     lens, lends = len(s), len(ds)
+#     old = 0
+#     k = 0
+#     w = ""
+#     while k < lends:
+#         i, j = k, k + 1
+#         while j < lends and ds[i] <= ds[j]:
+#             i = (ds[i] == ds[j]) and i + 1 or k
+#             j += 1
+#         while k < i + 1:
+#             k += j - i
+#             prev = w
+#             w = ds[old:k]
+#             old = k
+#             if w == prev:
+#                 rep += 1
+#             else:
+#                 prev, rep = w, 1
+#             if len(w) * rep == lens:
+#                 return "".join(w * rep)
+
+
 def smallest_rotation(s):
     """Smallest rotation of a string.
 
     Algorithm described in Pierre Duval, Jean. 1983. Factorizing Words
     over an Ordered Alphabet. Journal of Algorithms & Computational Technology
     4 (4) (December 1): 363–381. and Algorithms on strings and sequences based
     on Lyndon words, David Eppstein 2011.
     https://gist.github.com/dvberkel/1950267
 
     Examples
     --------
     >>> from pydna.utils import smallest_rotation
     >>> smallest_rotation("taaa")
     'aaat'
-
     """
-    prev, rep = None, 0
-    ds = 2 * s
-    lens = len(s)
-    lends = len(ds)
-    old = 0
-    k = 0
-    w = ""
-    while k < lends:
-        i, j = k, k + 1
-        while j < lends and ds[i] <= ds[j]:
-            i = (ds[i] == ds[j]) and i + 1 or k
-            j += 1
-        while k < i + 1:
-            k += j - i
-            prev = w
-            w = ds[old:k]
-            old = k
-            if w == prev:
-                rep += 1
-            else:
-                prev, rep = w, 1
-            if len(w) * rep == lens:
-                return w * rep
+    from pydivsufsort import min_rotation
 
+    k = min_rotation(s)
+    return s[k:] + s[:k]
 
-def cai(seq: str,
-        organism: str = "sce"):
+
+def cai(seq: str, organism: str = "sce", weights: dict = _weights):
     """docstring."""
-    from CAI import CAI as _CAI
-    return round(_CAI(seq.upper(), weights=_weights[organism]), 3)
+    from cai2 import CAI as _CAI
+
+    return round(_CAI(seq.upper(), weights=weights[organism]), 3)
 
 
-def rarecodons(seq: str,
-               organism="sce"):
+def rarecodons(seq: str, organism="sce"):
     """docstring."""
     rare = _rare_codons[organism]
     s = seq.upper()
     slices = []
-    for i in range(0, len(seq)//3):
-        x, y = i*3, i*3+3
+    for i in range(0, len(seq) // 3):
+        x, y = i * 3, i * 3 + 3
         trip = s[x:y]
         if trip in rare:
             slices.append(slice(x, y, 1))
     return slices
 
 
 def express(seq: str, organism="sce"):
     """docstring.
 
 
     **NOT IMPLEMENTED YET**
     """
-    x = _PrettyTable(["cds", "len", "cai", "gc", "sta", "stp",
-                      "n-end"]+_rare_codons[organism]+["rare"])
+    x = _PrettyTable(["cds", "len", "cai", "gc", "sta", "stp", "n-end"] + _rare_codons[organism] + ["rare"])
     val = []
 
-    val.append(f"{self._data.upper().decode('ASCII')[:3]}..."
-               f"{self._data.upper().decode('ASCII')[-3:]}")
-    val.append(len(self)/3)
+    val.append(f"{self._data.upper().decode('ASCII')[:3]}..." f"{self._data.upper().decode('ASCII')[-3:]}")
+    val.append(len(self) / 3)
     val.append(cai(organism))
     val.append(gc())
     val.append(startcodon())
     val.append(stopcodon())
     val.append(_n_end[organism].get(_seq3(self[3:6].translate())))
     s = self._data.upper().decode("ASCII")
-    trps = [s[i*3:i*3+3] for i in range(0, len(s)//3)]
+    trps = [s[i * 3 : i * 3 + 3] for i in range(0, len(s) // 3)]
     tot = 0
     for cdn in _rare_codons[organism]:
         cnt = trps.count(cdn)
         tot += cnt
         val.append(cnt)
-    val.append(round(tot/len(trps), 3))
+    val.append(round(tot / len(trps), 3))
     x.add_row(val)
     return x
 
 
 def open_folder(pth):
     """docstring."""
     if _sys.platform == "win32":
@@ -193,38 +208,32 @@
     """
     return sequence.translate(_complement_table)
 
 
 def memorize(filename):
     """Cache functions and classes.
 
-    see pydna.download and pydna.Assembly for use
+    see pydna.download
     """
 
     def decorator(f):
         def wrappee(*args, **kwargs):
             _module_logger.info("#### memorizer ####")
             _module_logger.info("cache filename                   = %s", filename)
             _module_logger.info(
                 "os.environ['pydna_cached_funcs'] = %s",
-                _os.environ["pydna_cached_funcs"],
+                _os.getenv("pydna_cached_funcs", ""),
             )
-            if filename not in _os.environ["pydna_cached_funcs"]:
-                _module_logger.info(
-                    "cache filename not among cached functions, made it new!"
-                )
+            if filename not in _os.getenv("pydna_cached_funcs", ""):
+                _module_logger.info("cache filename not among cached functions, made it new!")
                 return f(*args, **kwargs)
-            key = _base64.urlsafe_b64encode(
-                _hashlib.sha1(_pickle.dumps((args, kwargs))).digest()
-            ).decode("ascii")
+            key = _base64.urlsafe_b64encode(_hashlib.sha1(_pickle.dumps((args, kwargs))).digest()).decode("ascii")
             _module_logger.info("key = %s", key)
             cache = _shelve.open(
-                _os.path.join(
-                    _os.environ["pydna_data_dir"], identifier_from_string(filename)
-                ),
+                _os.path.join(_os.environ["pydna_data_dir"], identifier_from_string(filename)),
                 writeback=False,
             )
             try:
                 result = cache[key]
             except KeyError:
                 _module_logger.info(
                     "no result for key %s in shelve %s",
@@ -275,14 +284,15 @@
     --------
     >>> from pydna.utils import seguid
     >>> seguid("aaa")
     'YG7G6b2Kj/KtFOX63j8mRHHoIlE'
     """
     return _pretty_str(_seguid(seq.upper()))
 
+
 def useguid(seq: str) -> _pretty_str:
     """Returns the url safe SEGUID checksum for the sequence.
     This is the SEGUID checksum with the '+' and '/' characters of standard
     Base64 encoding are respectively replaced by '-' and '_'.
 
     Examples
     --------
@@ -322,37 +332,35 @@
     value.
 
         dsDNA    ovhg
 
           nnn...    2
         nnnnn...
 
-          nnnn...    1
+         nnnn...    1
         nnnnn...
 
         nnnnn...    0
         nnnnn...
 
         nnnnn...   -1
-          nnnn...
+         nnnn...
 
         nnnnn...   -2
           nnn...
 
 
     """
     watson = watson.upper()
     crick = crick.upper()
-    lw = len(watson)
-    lc = len(crick)
+    lw, lc = len(watson), len(crick)
     if overhang == 0 and lw == lc:
         return lseguid_blunt(watson)
     else:
-        w, c, o = min(((watson, crick, overhang),
-                       (crick, watson, lw - lc + overhang)))
+        w, c, o = min(((watson, crick, overhang), (crick, watson, lw - lc + overhang)))
 
     return useguid(f"{o*chr(32)}{w}\n{-o*chr(32)}{c[::-1]}")
 
 
 def cseguid(seq: str) -> _pretty_str:
     """Url safe cSEGUID for a string representing a circular double stranded
     DNA molecule.
@@ -365,32 +373,31 @@
     --------
     >>> from pydna.utils import cseguid
     >>> cseguid("attt")
     'oopV-6158nHJqedi8lsshIfcqYA'
     >>> cseguid("ttta")
     'oopV-6158nHJqedi8lsshIfcqYA'
     """
-    return useguid(min(smallest_rotation(seq.upper()),
-                       smallest_rotation(str(rc(seq)).upper())))
+    return useguid(min(smallest_rotation(seq.upper()), smallest_rotation(str(rc(seq)).upper())))
 
 
 def flatten(*args):
     """Flattens an iterable of iterables.
 
     Down to str, bytes, bytearray or any of the pydna or Biopython seq objects
     """
     output = []
     args = list(args)
     while args:
         top = args.pop()
         if (
-                isinstance(top, _collections.abc.Iterable)
-                and not isinstance(top, (str, bytes, bytearray))
-                and not hasattr(top, "reverse_complement")
-                ):
+            isinstance(top, _collections.abc.Iterable)
+            and not isinstance(top, (str, bytes, bytearray))
+            and not hasattr(top, "reverse_complement")
+        ):
             args.extend(top)
         else:
             output.append(top)
     return output[::-1]
 
 
 def seq31(seq):
@@ -450,61 +457,52 @@
     nr_of_codons = int(len(seq) / 3)
     sequence = [seq[i * 3 : i * 3 + 3].title() for i in range(nr_of_codons)]
     padding = " " * 2
     return padding.join([threecode.get(aa, "X") for aa in sequence])
 
 
 def parse_text_table(rawtable, tabs=4):
-
     table = textwrap.dedent(rawtable.expandtabs(tabs)).strip()
     max_row_length = max([len(row.strip()) for row in table.splitlines()])
     rows = [row.ljust(max_row_length) for row in table.splitlines()]
     table = "\n".join(rows)
     empty_column_regex = r"(?:\n?\s{%s}\n)+" % len(rows)
     transposed_table = "\n".join(["".join(c) for c in zip(*rows)])
     cols = re.split(empty_column_regex, transposed_table)
     list_of_lists_cr = []
 
     for col in cols:
-        columnlist = [
-            "".join(c).strip() for c in zip(*[a for a in col.splitlines() if a])
-        ]
+        columnlist = ["".join(c).strip() for c in zip(*[a for a in col.splitlines() if a])]
         maxlen = max([len(c) for c in columnlist])
         columnlist = [c.ljust(maxlen) for c in columnlist]
         list_of_lists_cr.append(columnlist)
 
     list_of_lists_rc = [list(i) for i in zip(*list_of_lists_cr)]
 
-    formatted = _pretty_str("\n".join(" ".join(cell) for cell in
-                            list_of_lists_rc))
+    formatted = _pretty_str("\n".join(" ".join(cell) for cell in list_of_lists_rc))
 
-    columnsplit = _pretty_str("\n|||\n".join(
-        [
-            "\n".join(
-                [
-                    x.strip()
-                    for x in ["".join(c) for c in zip(*col.strip("\n").splitlines())]
-                ]
-            )
-            for col in cols
-        ]
-    ))
+    columnsplit = _pretty_str(
+        "\n|||\n".join(
+            ["\n".join([x.strip() for x in ["".join(c) for c in zip(*col.strip("\n").splitlines())]]) for col in cols]
+        )
+    )
 
     rowsplit = "\n---\n".join(["\n".join(a).strip() for a in zip(*list_of_lists_cr)])
     rowsplit = _pretty_str("\n".join(row.strip() for row in rowsplit.splitlines()))
 
-    return (formatted,
-            columnsplit,
-            rowsplit,
-            list_of_lists_rc,
-            list_of_lists_cr,)
+    return (
+        formatted,
+        columnsplit,
+        rowsplit,
+        list_of_lists_rc,
+        list_of_lists_cr,
+    )
 
 
 def join_list_to_table(rawlist):
-
     if "|||\n" in rawlist:
         raw_columns = rawlist.split("|||\n")
         cols = [col.splitlines() for col in raw_columns]
     elif "---\n" in rawlist:
         rawrows = rawlist.split("---\n")
         rows = [row.splitlines() for row in rawrows]
         cols = list(itertools.zip_longest(*rows, fillvalue=""))
@@ -537,35 +535,26 @@
 
 def expandtolist(content):
     """docstring."""
     resultlist = []
     for line in re.finditer(r"(?P<item>[^\(\)]*?)(?P<brack>\[.*?\])", content):
         text2rep = line.group("item")
         bracket = line.group("brack")
-        padding = max(
-            [len(str(x).strip()) for x in re.split(r"\.\.|,",
-                                                   bracket.strip("[ ]"))]
-        )
+        padding = max([len(str(x).strip()) for x in re.split(r"\.\.|,", bracket.strip("[ ]"))])
         inbracket = [item.strip("[ ]") for item in bracket.split(",")]
         expanded = []
 
         for item in inbracket:
-            if re.match(r"(\d+\.\.\d+)|([a-z]+\.\."
-                        r"[a-z]+)|([A-Z]+\.\.[A-Z]+)", item):
+            if re.match(r"(\d+\.\.\d+)|([a-z]+\.\." r"[a-z]+)|([A-Z]+\.\.[A-Z]+)", item):
                 low, high = item.split(
                     "..",
                 )
                 if low.isdigit() and high.isdigit():
-                    r = [
-                        "{:{}d}".format(x, padding)
-                        for x in range(int(low), 1 + int(high))
-                    ]
-                if (low.islower() and high.islower()) or (
-                    low.isupper() and high.isupper()
-                ):
+                    r = ["{:{}d}".format(x, padding) for x in range(int(low), 1 + int(high))]
+                if (low.islower() and high.islower()) or (low.isupper() and high.isupper()):
                     r = [chr(a) for a in range(ord(low), 1 + ord(high))]
                 expanded.extend(r)
             else:
                 expanded.append(item.strip())
 
         resultlist.append([text2rep + x for x in expanded])
 
@@ -665,27 +654,22 @@
         "GGA",
         "GGG",
     )
 
     starts = ("ATG",)
     stops = ("TAA", "TAG", "TGA")
 
-    return (
-        random.choice(starts)
-        + "".join([random.choice(cdns) for x in range(length)])
-        + random.choice(stops)
-    )
+    return random.choice(starts) + "".join([random.choice(cdns) for x in range(length)]) + random.choice(stops)
 
 
 def randomprot(length, maxlength=None):
     """docstring."""
     if maxlength and maxlength > length:
         length = int(round(random.triangular(length, maxlength)))
-    return "".join([random.choice("ACDEFGHIKLMNPQRSTVWY")
-                    for x in range(length)])
+    return "".join([random.choice("ACDEFGHIKLMNPQRSTVWY") for x in range(length)])
 
 
 def eq(*args, **kwargs):
     """Compare two or more DNA sequences for equality.
 
     Compares two or more DNA sequences for equality i.e. if they
     represent the same double stranded DNA molecule.
@@ -779,30 +763,26 @@
             topology = "circular"
     elif "circular" in kwargs:
         if kwargs["circular"] is True:
             topology = "circular"
         if kwargs["circular"] is False:
             topology = "linear"
     else:
-        topology = set([arg.circular if
-                        hasattr(arg, "circular") else None for arg in args])
+        topology = set([arg.circular if hasattr(arg, "circular") else None for arg in args])
 
         if len(topology) != 1:
             raise ValueError("sequences have different topologies")
         topology = topology.pop()
         if topology in (False, None):
             topology = "linear"
         elif topology is True:
             topology = "circular"
 
     args = [arg.seq if hasattr(arg, "seq") else arg for arg in args]
-    args_string_list = [
-        arg.watson.lower() if hasattr(arg, "watson") else str(arg).lower()
-        for arg in args
-    ]
+    args_string_list = [arg.watson.lower() if hasattr(arg, "watson") else str(arg).lower() for arg in args]
 
     length = set((len(s) for s in args_string_list))
 
     if len(length) != 1:
         return False
     same = True
 
@@ -814,14 +794,15 @@
     elif topology == "linear":
         # force linear comparison of all given sequences
         for s1, s2 in _itertools.combinations(args_string_list, 2):
             if not (s1 == s2 or s1 == rc(s2)):
                 same = False
     return same
 
+
 if __name__ == "__main__":
     import os as _os
 
     cached = _os.getenv("pydna_cached_funcs", "")
     _os.environ["pydna_cached_funcs"] = ""
     import doctest
```

### Comparing `pydna-5.2.0a9/setup.py` & `pydna-6.0.0a1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,310 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydna
+Version: 6.0.0a1
+Summary: Representing double stranded DNA and functions for simulating cloning and homologous recombination between DNA molecules.
+License: BSD
+Author: BjornFJohansson
+Author-email: bjornjobb@gmail.com
+Requires-Python: >=3.8
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: download
+Provides-Extra: express
+Provides-Extra: gel
+Provides-Extra: gui
+Requires-Dist: appdirs (>=1.4.4)
+Requires-Dist: biopython (>=1.80)
+Requires-Dist: cai2 (>=1.0.5) ; extra == "express"
+Requires-Dist: matplotlib (>=3.4.3) ; extra == "gel"
+Requires-Dist: networkx (>=2.8.8)
+Requires-Dist: pillow (>=8.4.0) ; extra == "gel"
+Requires-Dist: prettytable (>=3.5.0)
+Requires-Dist: pydivsufsort (>=0.0.11)
+Requires-Dist: pyfiglet (>=0.8.post1)
+Requires-Dist: pyparsing (>=2.4.7) ; extra == "download"
+Requires-Dist: pyperclip (>=1.8.2)
+Requires-Dist: pyqt5 (>=5.15.0) ; extra == "gui"
+Requires-Dist: requests (>=2.26.0) ; extra == "download"
+Requires-Dist: scipy (>=1.8.0) ; extra == "gel"
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# ![icon](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/pydna.resized.png) pydna
 
-packages = \
-['pydna']
+| [![Tests & Coverage](https://github.com/BjornFJohansson/pydna/actions/workflows/pydna_test_and_coverage_workflow.yml/badge.svg?branch=dev_bjorn)](https://github.com/BjornFJohansson/pydna/actions/workflows/pydna_test_and_coverage_workflow.yml) | [![codecov](https://codecov.io/gh/BjornFJohansson/pydna/branch/master/graph/badge.svg)](https://codecov.io/gh/BjornFJohansson/pydna/branch/master) | [![PyPI version](https://badge.fury.io/py/pydna.svg)](https://badge.fury.io/py/pydna)    | [![Google group : pydna](https://img.shields.io/badge/Google%20Group-pydna-blue.svg)](https://groups.google.com/g/pydna)              |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
+| [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)                                                                   | [![GitHub issues](https://img.shields.io/github/issues/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/issues)                | [![Anaconda-Server Badge2](https://anaconda.org/bjornfjohansson/pydna/badges/license.svg)](https://anaconda.org/bjornfjohansson/pydna) | [![GitHub stars](https://img.shields.io/github/stars/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/stargazers) |
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['appdirs>=1.4.4,<2.0.0',
- 'biopython>=1.80,<2.0',
- 'networkx>=2.8.8,<3.0.0',
- 'prettytable>=3.5.0,<4.0.0',
- 'pyfiglet>=0.8.post1,<0.9',
- 'pyperclip>=1.8.2,<2.0.0']
-
-extras_require = \
-{'download': ['pyparsing>=2.4.7,<3.0.0', 'requests==2.26.0'],
- 'express': ['CAI==1.0.3'],
- 'gel': ['scipy==1.8.0', 'matplotlib==3.4.3', 'pillow==8.4.0']}
-
-setup_kwargs = {
-    'name': 'pydna',
-    'version': '5.2.0a9',
-    'description': 'Representing double stranded DNA and functions for simulating cloning and homologous recombination between DNA molecules.',
-    'long_description': '# ![icon](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/pydna.resized.png) pydna\n\n| [![Tests & Coverage](https://github.com/BjornFJohansson/pydna/workflows/Tests%20&%20Coverage/badge.svg)](https://github.com/BjornFJohansson/pydna/actions?query=workflow%3A%22Tests+%26+Coverage%22)                |[![codecov](https://codecov.io/gh/BjornFJohansson/pydna/branch/master/graph/badge.svg)](https://codecov.io/gh/BjornFJohansson/pydna/branch/master)    | [![PyPI version](https://badge.fury.io/py/pydna.svg)](https://badge.fury.io/py/pydna)                                                   |[![Anaconda-Server Badge](https://anaconda.org/bjornfjohansson/pydna/badges/version.svg)](https://anaconda.org/bjornfjohansson/pydna)   | [![Google group : pydna](https://img.shields.io/badge/Google%20Group-pydna-blue.svg)](https://groups.google.com/g/pydna)        |\n|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|\n| [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)                                                                                  |[![GitHub issues](https://img.shields.io/github/issues/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/issues)                   | [![Anaconda-Server Badge2](https://anaconda.org/bjornfjohansson/pydna/badges/license.svg)](https://anaconda.org/bjornfjohansson/pydna)  |[![GitHub stars](https://img.shields.io/github/stars/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/stargazers)   |                                                                                                                                 |\n\n\nPlanning genetic constructs with many parts and assembly steps, such as recombinant\nmetabolic pathways :petri_dish:, are often difficult to **properly** document as is evident from the\nstate of such documentation in the scientific literature :radioactive:.\n\n\nThe pydna python package provide a human-readable formal descriptions of :dna: cloning and genetic assembly\nstrategies in Python :snake: which allow for simulation and verification.\n\n\nPydna can perhaps be thought of as [executable documentation](https://en.wikipedia.org/wiki/Literate_programming) for cloning.\n\n\nA cloning strategy expressed in pydna is **complete**, **unambiguous** and **stable**.\n\n\nPydna provides simulation of:\n\n- Restriction digestion\n- Ligation\n- PCR\n- Primer design\n- Gibson assembly\n- Golden gate assembly\n- Homologous recombination\n- Gel electrophoresis of DNA with generation of gel images\n\nVirtually any sub-cloning experiment can be described in pydna, and its execution yield\nthe sequences of intermediate and final DNA molecules.\n\nPydna has been designed to be understandable for biologists with only some basic understanding of Python.\n\nPydna can formalize planning and sharing of cloning strategies and is especially useful for complex or combinatorial\nDNA molecule constructions.\n\n\nTo get started, we have compiled some [simple examples](https://github.com/MetabolicEngineeringGroupCBMA/pydna-examples#pydna-examples).\nFor more elaborate use, look at some assembly strategies of D-xylose metabolic pathways [MetabolicEngineeringGroupCBMA/ypk-xylose-pathways](https://github.com/MetabolicEngineeringGroupCBMA/ypk-xylose-pathways#pereira-et-al-2016).\n\n\nThere is an open access paper in BMC Bioinformatics describing pydna:\n\n[![abstr](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/BMC_resized.png)](http://www.biomedcentral.com/1471-2105/16/142/abstract)\n\nPlease reference the above paper:\n\n\nPereira, F., Azevedo, F., Carvalho, Â., Ribeiro, G. F., Budde, M. W., & Johansson, B. (2015). Pydna: a simulation and documentation tool for DNA assembly strategies using python. BMC Bioinformatics, 16(142), 142.\n\n\nif using pydna in a scientific publication.\n\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n\n\n## Usage\n\nMost pydna functionality is implemented as methods for the double stranded DNA sequence record\nclasses Dseq and Dseqrecord, which are subclasses of the [Biopython](http://biopython.org/wiki/Main_Page) [Seq](http://biopython.org/wiki/Seq) and [SeqRecord](http://biopython.org/wiki/SeqRecord) classes.\n\nThese classes make cut and paste cloning and PCR very simple:\n\n\n    >>> from pydna.dseq import Dseq\n    >>> seq = Dseq("GGATCCAAA","TTTGGATCC",ovhg=0)\n    >>> seq\n    Dseq(-9)\n    GGATCCAAA\n    CCTAGGTTT\n    >>> from Bio.Restriction import BamHI\n    >>> a,b = seq.cut(BamHI)\n    >>> a\n    Dseq(-5)\n    G\n    CCTAG\n    >>> b\n    Dseq(-8)\n    GATCCAAA\n        GTTT\n    >>> a+b\n    Dseq(-9)\n    GGATCCAAA\n    CCTAGGTTT\n    >>> b+a\n    Dseq(-13)\n    GATCCAAAG\n        GTTTCCTAG\n    >>> b+a+b\n    Dseq(-17)\n    GATCCAAAGGATCCAAA\n        GTTTCCTAGGTTT\n    >>> b+a+a\n    Traceback (most recent call last):\n      File "<stdin>", line 1, in <module>\n      File "/usr/local/lib/python2.7/dist-packages/pydna/dsdna.py", line 217, in __add__\n        raise TypeError("sticky ends not compatible!")\n    TypeError: sticky ends not compatible!\n    >>>\n\nAs the example above shows, pydna keeps track of sticky ends.\n\nNotably, homologous recombination and Gibson assembly between linear DNA fragments\ncan be easily simulated without any additional information besides the primary sequence of the fragments.\n\nGel electrophoresis of DNA fragments can be simulated using the included gel module\n\n\n    Jupyter QtConsole 4.7.7\n    Python 3.8.5 | packaged by conda-forge | (default, Aug 29 2020, 01:22:49)\n    Type \'copyright\', \'credits\' or \'license\' for more information\n    IPython 7.18.1 -- An enhanced Interactive Python. Type \'?\' for help.\n\n    In [1]: from pydna.gel import gel\n\n    In [2]: from pydna.ladders import PennStateLadder\n\n    In [3]: from pydna.dseqrecord import Dseqrecord\n\n    In [4]: gel([PennStateLadder,[Dseqrecord("A"*2000)]])\n    Out[4]:\n\n\n\n![](https://raw.githubusercontent.com/BjornFJohansson/pydna/master/scripts/pydna_gel.png)\n\n\nPydna can be very compact. The eleven lines of Python below simulates the construction of a recombinant plasmid.\nDNA sequences are downloaded from Genbank by accession numbers that are guaranteed to be stable over time.\n\n    from pydna.genbank import Genbank\n    gb = Genbank("myself@email.com") # Tell Genbank who you are!\n    gene = gb.nucleotide("X06997") # Kluyveromyces lactis LAC12 gene for lactose permease.\n    from pydna.parsers import parse_primers\n    primer_f,primer_r = parse_primers(\'\'\' >760_KlLAC12_rv (20-mer)\n                                          ttaaacagattctgcctctg\n\n                                          >759_KlLAC12_fw (19-mer)\n                                          aaatggcagatcattcgag \'\'\')\n    from pydna.amplify import pcr\n    pcr_prod = pcr(primer_f,primer_r, gene)\n    vector = gb.nucleotide("AJ001614") # pCAPs cloning vector\n    from Bio.Restriction import EcoRV\n    lin_vector = vector.linearize(EcoRV)\n    rec_vec =  ( lin_vector + pcr_prod ).looped()\n\nPydna can automate the simulation of [sub cloning](http://en.wikipedia.org/wiki/Subcloning) experiments using\npython. This is helpful to generate examples for teaching purposes.\n\nRead the documentation (below) or the [cookbook](https://github.com/BjornFJohansson/pydna/blob/master/docs/cookbook/cookbook.ipynb) with example files\nfor further information.\n\nPlease post a message in the [google group](https://groups.google.com/d/forum/pydna)\nfor pydna if you need help or have problems, questions or comments :sos:.\n\nFeedback & suggestions are very welcome!\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n\n## Who is using pydna?\n\nTaylor, L. J., & Strebel, K. (2017).\nPyviko: an automated Python tool to design gene knockouts in complex viruses with overlapping genes.\nBMC Microbiology, 17(1), 12.\n[PubMed](https://www.ncbi.nlm.nih.gov/pubmed/28061810)\n\n\nWang, Y., Xue, H., Pourcel, C., Du, Y., & Gautheret, D. (2021).\n2-kupl: mapping-free variant detection from DNA-seq data of matched samples.\nIn Cold Spring Harbor Laboratory (p. 2021.01.17.427048). [DOI](https://doi.org/10.1101/2021.01.17.427048)\n[PubMed](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8180056)\n\n\n[An Automated Protein Synthesis Pipeline with Transcriptic and Snakemake](http://blog.booleanbiotech.com/transcriptic_protein_synthesis_pipeline.html)\n\n\nand other projects on [github](https://github.com/BjornFJohansson/pydna/network/dependents?package_id=UGFja2FnZS01MjQ2MjYzNQ%3D%3D)\n\n\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n## Documentation\n\nDocumentation is built using [Sphinx](http://www.sphinx-doc.org/) from [docstrings](https://www.python.org/dev/peps/pep-0257/)\nin the code and displayed at readthedocs [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)\n\nThe [numpy](www.numpy.org) [docstring format](https://github.com/numpy/numpy/blob/release/doc/HOWTO_DOCUMENT.rst.txt) is used.\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n## Installation using pip\n\nPip is included in recent Python versions and is the\nofficially [recommended](http://python-packaging-user-guide.readthedocs.org/en/latest) tool.\n\nPip installs the minimal installation requirements automatically, but not the optional requirements (see below).\n\n    pip install pydna\n\nor use the --pre switch to get the latest version of pydna.\n\n    pip install pydna --pre\n\n### Windows:\n\nYou should be able to pip install pydna from the Windows terminal as biopython now can be installed with pip as well.\n\n    C:\\> pip install pydna\n\nBy default python and pip are not on the PATH. You can re-install Python and select this option during installation,\nor give the full path for pip. Try something like this, depending on where your copy of Python is installed:\n\n    C:\\Python37\\Scripts\\pip install pydna\n\n### Installing requirements\n\nIf you want to install requirements before installing pydna, you can do:\n\n\tpip install -r requirements.txt\n\nAnd for the optional requirements:\n\n\tpip install -r requirements_optional.txt\n\nFor testing:\n\n\tpip install -r requirements_test.txt\n\nor\n\n\tconda install --file requirements.txt\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n## Source Code\n\nPydna is developed on [Github](https://github.com/BjornFJohansson/pydna) :octocat:.\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n## Minimal installation dependencies\n\nPydna versions before 1.0.0 were compatible with python 2.7 only.\nThe list below is the minimal requirements for installing pydna.\nBiopython has c-extensions, but the other modules are pure python.\n\n- [Python 3.8, 3.9, 3.10 or 3.11](http://www.python.org)\n- [appdirs >= 1.3.0](https://pypi.python.org/pypi/appdirs)\n- [biopython >= 1.80](http://pypi.python.org/pypi/biopython)\n- [networkx >= 1.8.1](http://pypi.python.org/pypi/networkx)\n- [prettytable >= 0.7.2](https://pypi.python.org/pypi/PrettyTable)\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n## Optional dependencies\n\nIf the modules listed below in the first column are installed, they will provide the functionality\nlisted in the second column.\n\n| Dependency                                          | Function in pydna                                      |\n|-----------------------------------------------------|--------------------------------------------------------|\n| [pyparsing](https://pypi.python.org/pypi/pyparsing) | fix corrupt Genbank files with pydna.genbankfixer      |\n| [requests](https://pypi.org/project/requests)       | download sequences with pydna.download                 |\n| [CAI](https://pypi.org/project/CAI)                 | codon adaptation index calculations in several modules |\n| [numpy](http://www.numpy.org)                       | gel simulation with pydna.gel                          |\n| [scipy](https://www.scipy.org)                      | “                                                      |\n| [matplotlib](http://matplotlib.org)                 | “                                                      |\n| [pillow](https://github.com/python-pillow/Pillow)   | “                                                      |\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n## Requirements for running tests and analyzing code coverage\n\n- [pytest](https://pypi.org/project/pytest)\n- [pytest-cov](https://pypi.org/project/pytest-cov)\n- [pytest-mock](https://pypi.org/project/pytest-mock)\n- [pytest-doctestplus](https://pypi.org/project/pytest-doctestplus)\n- [coverage](https://pypi.org/project/coverage)\n- [nbval](https://pypi.org/project/nbval)\n- [requests-mock](https://pypi.org/project/requests-mock)\n\n\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n## Changelog\n\nSee the [change log](docs/CHANGELOG.md) for recent changes.\n\n![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)\n\n## Automatic testing & Release process\n\nThere are three github actions associated with this package:\n\n- `pydna_test_and_coverage_workflow.yml`\n\nThe `pydna_test_and_coverage_workflow.yml` is triggered on all pushed non-tagged commits.\nThis workflow run tests, doctests and a series of Jupyter notebooks using pytest.\n\nThe two other workflows build a setuptools wheel and packages for different Python versions\non Linux, Windows and macOS.\n\nThese are triggered by publishing a github release manually from the github interface.\n\n\n## Building a PyPI package\n\n\n\tpoetry build # run this command in the root directory where the pyproject.toml file is located\n\n\nPydna uses the poetry plugin []()\n\n\n\n\n\n\n### History\n\nPydna was made public in 2012 on [Google code](https://code.google.com/archive/p/pydna).\n\n\n:microbe:\n\n\n:portugal:\n',
-    'author': 'BjornFJohansson',
-    'author_email': 'bjornjobb@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
 
 
-setup(**setup_kwargs)
+Planning genetic constructs with many parts and assembly steps, such as recombinant
+metabolic pathways :petri_dish:, are often difficult to **properly** document as is evident from the poor
+state of documentation in the scientific literature :radioactive:.
+
+
+The pydna python package provide a human-readable formal descriptions of :dna: cloning and genetic assembly
+strategies in Python :snake: which allow for simulation and verification. Pydna can be used as [executable documentation](https://en.wikipedia.org/wiki/Literate_programming) for cloning.
+
+
+A cloning strategy expressed in pydna is **complete**, **unambiguous** and **stable**.
+
+
+Pydna provides simulation of:
+
+- Primer design
+- PCR
+- Restriction digestion
+- Ligation
+- Gel electrophoresis of DNA with generation of gel images
+- Homologous recombination
+- Gibson assembly
+- Golden gate assembly
+
+
+Virtually any sub-cloning experiment can be described in pydna, and its execution yield
+the sequences of intermediate and final DNA molecules.
+
+Pydna has been designed with the goal of being understandable for biologists with only some basic understanding of Python.
+
+Pydna can formalize planning and sharing of cloning strategies and is especially useful for complex or combinatorial
+DNA molecule constructions.
+
+To get started, I have compiled some [simple examples](https://github.com/MetabolicEngineeringGroupCBMA/pydna-examples#pydna-examples).
+For more elaborate use, look at some assembly strategies of D-xylose metabolic pathways [MetabolicEngineeringGroupCBMA/ypk-xylose-pathways](https://github.com/MetabolicEngineeringGroupCBMA/ypk-xylose-pathways#pereira-et-al-2016).
+
+
+
+
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+
+
+## Usage
+
+Most pydna functionality is implemented as methods for the double stranded DNA sequence record
+classes Dseq and Dseqrecord, which are subclasses of the [Biopython](http://biopython.org/wiki/Main_Page) [Seq](http://biopython.org/wiki/Seq) and [SeqRecord](http://biopython.org/wiki/SeqRecord) classes.
+
+These classes make PCR primer design, PCR simulation and cut-and-paste cloning very simple:
+
+[![example](https://raw.githubusercontent.com/BjornFJohansson/pydna/master/docs/example.png)](https://github.com/BjornFJohansson/pydna/blob/master/docs/example.ipynb)
+
+As the example above shows, pydna keeps track of sticky ends and features.
+
+
+Pydna can be very compact. The eleven lines of Python below simulates the construction of a recombinant plasmid.
+DNA sequences are downloaded from Genbank by accession numbers that are guaranteed to be stable over time.
+
+    from pydna.genbank import Genbank
+    gb = Genbank("myself@email.com") # Tell Genbank who you are!
+    gene = gb.nucleotide("X06997") # Kluyveromyces lactis LAC12 gene for lactose permease.
+    from pydna.parsers import parse_primers
+    primer_f,primer_r = parse_primers(''' >760_KlLAC12_rv (20-mer)
+                                          ttaaacagattctgcctctg
+
+                                          >759_KlLAC12_fw (19-mer)
+                                          aaatggcagatcattcgag ''')
+    from pydna.amplify import pcr
+    pcr_prod = pcr(primer_f,primer_r, gene)
+    vector = gb.nucleotide("AJ001614") # pCAPs cloning vector
+    from Bio.Restriction import EcoRV
+    lin_vector = vector.linearize(EcoRV)
+    rec_vec =  ( lin_vector + pcr_prod ).looped()
+
+Pydna can automate the simulation of [sub cloning](http://en.wikipedia.org/wiki/Subcloning) experiments using
+python. This is helpful to generate examples for teaching purposes.
+
+Read the documentation (below) or the [cookbook](https://github.com/BjornFJohansson/pydna/blob/master/docs/cookbook/cookbook.ipynb) with example files
+for further information.
+
+Feedback & suggestions are very welcome! Please post a message in the [google group](https://groups.google.com/d/forum/pydna) for pydna if you need help or have problems, questions or comments :sos:.
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+
+## Who is using pydna?
+
+Taylor, L. J., & Strebel, K. (2017).
+Pyviko: an automated Python tool to design gene knockouts in complex viruses with overlapping genes.
+BMC Microbiology, 17(1), 12.
+[PubMed](https://www.ncbi.nlm.nih.gov/pubmed/28061810)
+
+
+Wang, Y., Xue, H., Pourcel, C., Du, Y., & Gautheret, D. (2021).
+2-kupl: mapping-free variant detection from DNA-seq data of matched samples.
+In Cold Spring Harbor Laboratory (p. 2021.01.17.427048). [DOI](https://doi.org/10.1101/2021.01.17.427048)
+[PubMed](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8180056)
+
+
+[An Automated Protein Synthesis Pipeline with Transcriptic and Snakemake](http://blog.booleanbiotech.com/transcriptic_protein_synthesis_pipeline.html)
+
+
+and other projects on [github](https://github.com/BjornFJohansson/pydna/network/dependents?package_id=UGFja2FnZS01MjQ2MjYzNQ%3D%3D)
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+There is an open access paper in BMC Bioinformatics describing pydna:
+
+[![abstr](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/BMC_resized.png)](http://www.biomedcentral.com/1471-2105/16/142/abstract)
+
+Please reference the above paper:
+
+
+Pereira, F., Azevedo, F., Carvalho, Â., Ribeiro, G. F., Budde, M. W., & Johansson, B. (2015). Pydna: a simulation and documentation tool for DNA assembly strategies using python. BMC Bioinformatics, 16(142), 142.
+
+
+When using pydna.
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+## Documentation
+
+Documentation is built using [Sphinx](http://www.sphinx-doc.org/) from [docstrings](https://www.python.org/dev/peps/pep-0257/)
+in the code and displayed at readthedocs [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)
+
+The [numpy](www.numpy.org) [docstring format](https://github.com/numpy/numpy/blob/release/doc/HOWTO_DOCUMENT.rst.txt) is used.
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+## Installation using pip
+
+Pip is included in recent Python versions and is the
+officially [recommended](http://python-packaging-user-guide.readthedocs.org/en/latest) tool.
+
+Pip installs the minimal installation requirements automatically, but not the optional requirements (see below).
+
+    pip install pydna
+
+or use the --pre switch to get the latest version of pydna.
+
+    pip install pydna --pre
+
+for optional functionality do:
+
+    pip install pydna[gel,download,express,gui]
+
+Remove options inside the square brackets as required, but be sure not to leave spaces as pip will not recognize the options. See below under "Optional dependencies".
+
+### Windows:
+
+You should be able to pip install pydna from the Windows terminal as biopython now can be installed with pip as well.
+
+    C:\> pip install pydna
+
+By default python and pip are not on the PATH. You can re-install Python and select this option during installation, or give the full path for pip. Try something like this, depending on where your copy of Python is installed:
+
+    C:\Python37\Scripts\pip install pydna
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+## Source Code
+
+Pydna is developed on [Github](https://github.com/BjornFJohansson/pydna) :octocat:.
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+## Minimal installation dependencies
+
+Pydna versions before 1.0.0 were compatible with python 2.7 only.
+The list below is the minimal requirements for installing pydna.
+Biopython has c-extensions, but the other modules are pure python.
+
+- [Python 3.8, 3.9, 3.10 or 3.11](http://www.python.org)
+- [appdirs >=1.4.4](https://pypi.python.org/pypi/appdirs)
+- [biopython >= 1.80](http://pypi.python.org/pypi/biopython)
+- [networkx >=2.8.8](http://pypi.python.org/pypi/networkx)
+- [prettytable >=3.5.0](https://pypi.python.org/pypi/PrettyTable)
+- [pyperclip >=1.8.2](https://pypi.python.org/pypi/PrettyTable)
+- [pyfiglet >=0.8.post1](https://pypi.python.org/pypi/PrettyTable)
+
+
+## Optional dependencies
+
+If the modules listed below in the first column are installed, they will provide the functionality listed in the second column.
+
+| Dependency                                                  | Function in pydna                                      |
+|-------------------------------------------------------------|--------------------------------------------------------|
+| [scipy >=1.8.0](https://www.scipy.org)                      | gel simulation with pydna.gel                          |
+| [matplotlib >=3.4.3](http://matplotlib.org)                 | “                                                      |
+| [pillow >=8.4.0](https://github.com/python-pillow/Pillow)   | “                                                      |
+| [numpy](http://www.numpy.org)                               | "                                                      |
+| [pyparsing >=2.4.7](https://pypi.python.org/pypi/pyparsing) | fix corrupt Genbank files with pydna.genbankfixer      |
+| [requests >=2.26.0](https://pypi.org/project/requests)      | download sequences with pydna.download                 |
+| [cai2 >=1.0.5](https://pypi.python.org/pypi/cai2)           | codon adaptation index calculations in several modules |
+| [pyqt5 >=5.15.0](https://pypi.python.org/pypi/pyqt5)        | codon adaptation index calculations in several modules |
+
+
+## Requirements for running tests and analyzing code coverage
+
+- [pytest](https://pypi.org/project/pytest)
+- [pytest-cov](https://pypi.org/project/pytest-cov)
+- [pytest-doctestplus](https://pypi.org/project/pytest-doctestplus)
+- [coverage](https://pypi.org/project/coverage)
+- [nbval](https://pypi.org/project/nbval)
+- [requests-mock](https://pypi.org/project/requests-mock)
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+## Releases
+
+See the [releases](https://github.com/BjornFJohansson/pydna/releases) for changes and releases.
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+## Automatic testing & Release process
+
+There are two github actions for this package:
+
+- `pydna_test_and_coverage_workflow.yml`
+- `pydna_pypi_build_workflow.yml`
+
+The `pydna_test_and_coverage_workflow.yml` is triggered on all pushed commits for all branches.
+This workflow run tests, doctests and a series of Jupyter notebooks using pytest on Linux, Windows and macOS and all
+supported python versions.
+
+The other workflow builds a PyPI packages using poetry on
+
+These are triggered by publishing a github release manually from the github interface.
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+## Building a PyPI package with [Poetry](https://pypi.org/project/poetry)
+
+1. Commit changes to git
+2. Tag the commit according to the [Semantic Versioning](https://semver.org) format, for example "v2.0.1a3". Do not forget the "v" or poetry will not recognize the tag.
+
+        git tag v2.0.1a3
+
+3. Pydna uses the poetry [poetry-dynamic-versioning](https://pypi.org/project/poetry-dynamic-versioning) plugin.
+
+        poetry dynamic-versioning # This sets the version number in the source files
+
+4. Verify the version
+
+        poetry version
+
+5. Build package:
+
+        poetry build # run this command in the root directory where the pyproject.toml file is located
+
+6. Verify the filename of the files in the dist/ folder, they should match
+
+7. Publish to pypi
+
+        poetry publish
+
+![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+
+## History
+
+Pydna was made public in 2012 on [Google code](https://code.google.com/archive/p/pydna).
+
+
+:microbe:
+
+
+:portugal:
+
```

