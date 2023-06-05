# Comparing `tmp/mutalyzer-algebra-1.2.0.tar.gz` & `tmp/mutalyzer-algebra-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutalyzer-algebra-1.2.0.tar", last modified: Tue Nov 15 11:24:33 2022, max compression
+gzip compressed data, was "mutalyzer-algebra-1.2.1.tar", last modified: Mon Jun  5 08:45:02 2023, max compression
```

## Comparing `mutalyzer-algebra-1.2.0.tar` & `mutalyzer-algebra-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-15 11:24:33.671733 mutalyzer-algebra-1.2.0/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1089 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)     2569 2022-11-15 11:24:33.671733 mutalyzer-algebra-1.2.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     1830 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-15 11:24:33.671733 mutalyzer-algebra-1.2.0/algebra/
--rw-rw-r--   0 mark      (1000) mark      (1000)      373 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8607 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/__main__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-15 11:24:33.671733 mutalyzer-algebra-1.2.0/algebra/lcs/
--rw-rw-r--   0 mark      (1000) mark      (1000)      237 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/lcs/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     9631 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/lcs/all_lcs.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1502 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/lcs/distance_only.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-15 11:24:33.671733 mutalyzer-algebra-1.2.0/algebra/relations/
--rw-rw-r--   0 mark      (1000) mark      (1000)      709 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/relations/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/relations/relation.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3330 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/relations/sequence_based.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4993 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/relations/supremal_based.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1595 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/relations/variant_based.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3747 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/utils.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-15 11:24:33.671733 mutalyzer-algebra-1.2.0/algebra/variants/
--rw-rw-r--   0 mark      (1000) mark      (1000)      304 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/variants/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8216 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/variants/parser.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8654 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/algebra/variants/variant.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-15 11:24:33.671733 mutalyzer-algebra-1.2.0/mutalyzer_algebra.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2569 2022-11-15 11:24:33.000000 mutalyzer-algebra-1.2.0/mutalyzer_algebra.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      686 2022-11-15 11:24:33.000000 mutalyzer-algebra-1.2.0/mutalyzer_algebra.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2022-11-15 11:24:33.000000 mutalyzer-algebra-1.2.0/mutalyzer_algebra.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       51 2022-11-15 11:24:33.000000 mutalyzer-algebra-1.2.0/mutalyzer_algebra.egg-info/entry_points.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       30 2022-11-15 11:24:33.000000 mutalyzer-algebra-1.2.0/mutalyzer_algebra.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       14 2022-11-15 11:24:33.000000 mutalyzer-algebra-1.2.0/mutalyzer_algebra.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      884 2022-11-15 11:24:33.671733 mutalyzer-algebra-1.2.0/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)       39 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-15 11:24:33.671733 mutalyzer-algebra-1.2.0/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2022-11-15 11:22:58.000000 mutalyzer-algebra-1.2.0/tests/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1089 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/LICENSE
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2602 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1863 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.824218 mutalyzer-algebra-1.2.1/algebra/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      373 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8607 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/__main__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.824218 mutalyzer-algebra-1.2.1/algebra/lcs/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      237 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/lcs/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     9631 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/lcs/all_lcs.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1502 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/lcs/distance_only.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/algebra/relations/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      698 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/relation.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3330 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/sequence_based.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4998 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/supremal_based.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1595 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/variant_based.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3747 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/utils.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/algebra/variants/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      304 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/variants/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8743 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/variants/parser.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8654 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/variants/variant.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2602 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      686 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       51 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/entry_points.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       30 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       14 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      884 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)       39 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/tests/__init__.py
```

### Comparing `mutalyzer-algebra-1.2.0/LICENSE` & `mutalyzer-algebra-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.0/PKG-INFO` & `mutalyzer-algebra-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer-algebra
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Boolean Algebra for Genetic Variants
 Home-page: https://github.com/mutalyzer/algebra
 Author: Mark A. Santcroos, Jonathan K. Vis
 Author-email: m.a.santcroos@lumc.nl, j.k.vis@lumc.nl
 License: MIT
 Keywords: algebra,genomics,graph,string,genetics,edit-distance,alignment,compare,sequence,variants,lcs,relations,hgvs
 Platform: UNKNOWN
@@ -25,15 +25,15 @@
 variant is fully contained in another or a variant fully contains another;
 overlap, i.e., two variants have (at least) one common element; and
 disjoint, i.e., no common elements that allows for a comprehensive
 classification of the relation for every pair of variants by taking all
 minimal Longest Common Subsequence (LCS) alignments into account.
 
 [Jonathan K. Vis, Mark A. Santcroos, Walter A. Kosters and Jeroen F.J. Laros.
-"A Boolean Algebra for Genetic Variants." (2021)](https://arxiv.org/abs/2112.14494)
+"A Boolean Algebra for Genetic Variants." In: *Bioinformatics* (2023).](https://doi.org/10.1093/bioinformatics/btad001)
 
 Installation
 ------------
 
 Use pip to install from the Python Package Index (PyPI).
 
 ```bash
@@ -87,12 +87,12 @@
 # returns: Relation.CONTAINS
 compare(reference, lhs, rhs)
 ```
 
 See Also
 --------
 
-A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://v3.mutalyzer.nl/algebra)
+A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://mutalyzer.nl/algebra)
 
 [Mutalyzer Algebra on PyPI](https://pypi.org/project/mutalyzer-algebra/)
```

### Comparing `mutalyzer-algebra-1.2.0/README.md` & `mutalyzer-algebra-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 variant is fully contained in another or a variant fully contains another;
 overlap, i.e., two variants have (at least) one common element; and
 disjoint, i.e., no common elements that allows for a comprehensive
 classification of the relation for every pair of variants by taking all
 minimal Longest Common Subsequence (LCS) alignments into account.
 
 [Jonathan K. Vis, Mark A. Santcroos, Walter A. Kosters and Jeroen F.J. Laros.
-"A Boolean Algebra for Genetic Variants." (2021)](https://arxiv.org/abs/2112.14494)
+"A Boolean Algebra for Genetic Variants." In: *Bioinformatics* (2023).](https://doi.org/10.1093/bioinformatics/btad001)
 
 Installation
 ------------
 
 Use pip to install from the Python Package Index (PyPI).
 
 ```bash
@@ -68,10 +68,10 @@
 # returns: Relation.CONTAINS
 compare(reference, lhs, rhs)
 ```
 
 See Also
 --------
 
-A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://v3.mutalyzer.nl/algebra)
+A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://mutalyzer.nl/algebra)
 
 [Mutalyzer Algebra on PyPI](https://pypi.org/project/mutalyzer-algebra/)
```

### Comparing `mutalyzer-algebra-1.2.0/algebra/__main__.py` & `mutalyzer-algebra-1.2.1/algebra/__main__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.0/algebra/lcs/all_lcs.py` & `mutalyzer-algebra-1.2.1/algebra/lcs/all_lcs.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.0/algebra/lcs/distance_only.py` & `mutalyzer-algebra-1.2.1/algebra/lcs/distance_only.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.0/algebra/relations/__init__.py` & `mutalyzer-algebra-1.2.1/algebra/relations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from [1]_. Variants are given as alleles, i.e., a list of variants
 applied to some reference sequence. Both variants are subject to the same
 reference sequence.
 
 References
 ----------
 [1] J.K. Vis, M.A. Santcroos, W.A. Kosters and J.F.J. Laros.
-"A Boolean Algebra for Genetic Variants".
-In: arXiv preprint 2112.14494 (2021).
+"A Boolean Algebra for Genetic Variants." In: Bioinformatics (2023).
 """
 
 
 from .relation import Relation
 from .variant_based import (are_disjoint, are_equivalent, compare,
                             contains, have_overlap, is_contained)
```

### Comparing `mutalyzer-algebra-1.2.0/algebra/relations/sequence_based.py` & `mutalyzer-algebra-1.2.1/algebra/relations/sequence_based.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.0/algebra/relations/supremal_based.py` & `mutalyzer-algebra-1.2.1/algebra/relations/supremal_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         The minimum offset around the variant.
 
     See Also
     --------
     `spanning_variant` : The minimum spanning (delins) variant.
     """
 
-    offset = max(offset, len(variant), 1)
+    offset = max(offset, len(variant) // 2, 1)
 
     while True:
         start = max(0, variant.start - offset)
         end = min(len(reference), variant.end + offset)
 
         observed = reference[start:variant.start] + variant.sequence + reference[variant.end:end]
```

### Comparing `mutalyzer-algebra-1.2.0/algebra/relations/variant_based.py` & `mutalyzer-algebra-1.2.1/algebra/relations/variant_based.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.0/algebra/utils.py` & `mutalyzer-algebra-1.2.1/algebra/utils.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.0/algebra/variants/parser.py` & `mutalyzer-algebra-1.2.1/algebra/variants/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,33 @@
         return match_plus(lambda ch: ch in DNA_NUCLEOTIDES, "nucleotide")
 
     def match_location():
         start = match_number()
         end = match_number() if match_optional("_") else start
         return start - 1, end
 
+    def match_insertion():
+        def match_inserted_part():
+            sequence = match_sequence()
+            number = 1
+            if match_optional("["):
+                number = match_number()
+                match("]")
+            return sequence * number
+
+        compound = match_optional("[")
+        sequence = match_inserted_part()
+        if not compound:
+            return sequence
+
+        while match_optional(";"):
+            sequence += match_inserted_part()
+        match("]")
+        return sequence
+
     def match_variant(reference):
         start, end = match_location()
         ctx_pos = pos
 
         if match_optional("dup"):
             try:
                 sequence = match_sequence()
@@ -129,21 +148,21 @@
                 sequence = ""
             else:
                 if len(sequence) != end - start:
                     raise ValueError(f"inconsistent deleted length at {pos}")
                 if reference is not None and sequence != reference[start:end]:
                     raise ValueError(f"'{sequence}' not found in reference at {start}")
             if match_optional("ins"):
-                return Variant(start, end, match_sequence())
+                return Variant(start, end, match_insertion())
             return Variant(start, end, "")
 
         if match_optional("ins"):
             if end - start != 2:
                 raise ValueError(f"invalid inserted range at {pos}")
-            return Variant(start + 1, start + 1, match_sequence())
+            return Variant(start + 1, start + 1, match_insertion())
 
         try:
             sequence = match_sequence()
         except ValueError:
             sequence = ""
 
         if match_optional(">"):
```

### Comparing `mutalyzer-algebra-1.2.0/algebra/variants/variant.py` & `mutalyzer-algebra-1.2.1/algebra/variants/variant.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.0/mutalyzer_algebra.egg-info/PKG-INFO` & `mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer-algebra
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Boolean Algebra for Genetic Variants
 Home-page: https://github.com/mutalyzer/algebra
 Author: Mark A. Santcroos, Jonathan K. Vis
 Author-email: m.a.santcroos@lumc.nl, j.k.vis@lumc.nl
 License: MIT
 Keywords: algebra,genomics,graph,string,genetics,edit-distance,alignment,compare,sequence,variants,lcs,relations,hgvs
 Platform: UNKNOWN
@@ -25,15 +25,15 @@
 variant is fully contained in another or a variant fully contains another;
 overlap, i.e., two variants have (at least) one common element; and
 disjoint, i.e., no common elements that allows for a comprehensive
 classification of the relation for every pair of variants by taking all
 minimal Longest Common Subsequence (LCS) alignments into account.
 
 [Jonathan K. Vis, Mark A. Santcroos, Walter A. Kosters and Jeroen F.J. Laros.
-"A Boolean Algebra for Genetic Variants." (2021)](https://arxiv.org/abs/2112.14494)
+"A Boolean Algebra for Genetic Variants." In: *Bioinformatics* (2023).](https://doi.org/10.1093/bioinformatics/btad001)
 
 Installation
 ------------
 
 Use pip to install from the Python Package Index (PyPI).
 
 ```bash
@@ -87,12 +87,12 @@
 # returns: Relation.CONTAINS
 compare(reference, lhs, rhs)
 ```
 
 See Also
 --------
 
-A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://v3.mutalyzer.nl/algebra)
+A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://mutalyzer.nl/algebra)
 
 [Mutalyzer Algebra on PyPI](https://pypi.org/project/mutalyzer-algebra/)
```

### Comparing `mutalyzer-algebra-1.2.0/mutalyzer_algebra.egg-info/SOURCES.txt` & `mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.0/setup.cfg` & `mutalyzer-algebra-1.2.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mutalyzer-algebra
-version = 1.2.0
+version = 1.2.1
 description = A Boolean Algebra for Genetic Variants
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Mark A. Santcroos, Jonathan K. Vis
 author_email = m.a.santcroos@lumc.nl, j.k.vis@lumc.nl
 url = https://github.com/mutalyzer/algebra
 keywords = algebra, genomics, graph, string, genetics, edit-distance, alignment, compare, sequence, variants, lcs, relations, hgvs
```

