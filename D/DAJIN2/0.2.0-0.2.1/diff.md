# Comparing `tmp/DAJIN2-0.2.0.tar.gz` & `tmp/DAJIN2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DAJIN2-0.2.0.tar", last modified: Mon Jun  5 05:29:31 2023, max compression
+gzip compressed data, was "DAJIN2-0.2.1.tar", last modified: Mon Jun  5 07:55:38 2023, max compression
```

## Comparing `DAJIN2-0.2.0.tar` & `DAJIN2-0.2.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.428880 DAJIN2-0.2.0/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.0/LICENSE
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.0/MANIFEST.in
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-05 05:29:31.424101 DAJIN2-0.2.0/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2918 2023-06-04 20:44:56.000000 DAJIN2-0.2.0/README.md
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-05 05:29:31.428880 DAJIN2-0.2.0/setup.cfg
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1077 2023-06-05 05:28:49.000000 DAJIN2-0.2.0/setup.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.005903 DAJIN2-0.2.0/src/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.266428 DAJIN2-0.2.0/src/DAJIN2/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11052 2023-06-05 05:29:01.000000 DAJIN2-0.2.0/src/DAJIN2/DAJIN2.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3881 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/batch.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.473150 DAJIN2-0.2.0/src/DAJIN2/core/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/__init__.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.596245 DAJIN2-0.2.0/src/DAJIN2/core/classification/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/classification/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/classification/classify.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/classification/detect_sv.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.788226 DAJIN2-0.2.0/src/DAJIN2/core/clustering/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/clustering.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/make_score.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/merge_clusters.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4239 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/return_labels.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.916369 DAJIN2-0.2.0/src/DAJIN2/core/consensus/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      311 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/consensus/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5873 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/consensus/consensus.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/consensus/subset.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10880 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/core_execute.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.222099 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      472 2023-06-05 05:23:44.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4912 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/call_midsv.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7398 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/correct_knockin.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10324 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/correct_sequence_error.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5883 2023-06-05 05:23:44.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/extract_knockin_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7038 2023-06-05 05:23:44.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/extract_mutation_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4356 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/format_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/mappy_align.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/replace_NtoD.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5139 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/validate_inputs.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.315369 DAJIN2-0.2.0/src/DAJIN2/core/report/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       39 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/report/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12958 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/report/report_bam.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/report/report_files.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2826 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/gui.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.360915 DAJIN2-0.2.0/src/DAJIN2/postprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/postprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/postprocess/report.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1127 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/single.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.060594 DAJIN2-0.2.0/src/DAJIN2/static/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.385436 DAJIN2-0.2.0/src/DAJIN2/static/css/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/static/css/style.css
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/template_igvjs.html
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.407586 DAJIN2-0.2.0/src/DAJIN2/templates/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/templates/index.html
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/view.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.410614 DAJIN2-0.2.0/src/DAJIN2.egg-info/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1670 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/SOURCES.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/dependency_links.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       46 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/entry_points.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      217 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/requires.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/top_level.txt
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.943211 DAJIN2-0.2.1/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.1/LICENSE
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.1/MANIFEST.in
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-05 07:55:38.937802 DAJIN2-0.2.1/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2918 2023-06-04 20:44:56.000000 DAJIN2-0.2.1/README.md
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-05 07:55:38.943211 DAJIN2-0.2.1/setup.cfg
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1077 2023-06-05 07:55:09.000000 DAJIN2-0.2.1/setup.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.133951 DAJIN2-0.2.1/src/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.285153 DAJIN2-0.2.1/src/DAJIN2/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11052 2023-06-05 07:55:25.000000 DAJIN2-0.2.1/src/DAJIN2/DAJIN2.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3881 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/batch.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.395823 DAJIN2-0.2.1/src/DAJIN2/core/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/__init__.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.452089 DAJIN2-0.2.1/src/DAJIN2/core/classification/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/classification/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/classification/classify.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/classification/detect_sv.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.566106 DAJIN2-0.2.1/src/DAJIN2/core/clustering/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/clustering.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/make_score.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/merge_clusters.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4239 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/clustering/return_labels.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.621218 DAJIN2-0.2.1/src/DAJIN2/core/consensus/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      311 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/consensus/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5873 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/consensus/consensus.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/consensus/subset.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10880 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/core_execute.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.809781 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      472 2023-06-05 05:23:44.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4912 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/call_midsv.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7398 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/correct_knockin.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10324 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/correct_sequence_error.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5900 2023-06-05 07:54:08.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_knockin_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7561 2023-06-05 07:53:53.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_mutation_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4356 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/format_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/mappy_align.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/replace_NtoD.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5139 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/preprocess/validate_inputs.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.857096 DAJIN2-0.2.1/src/DAJIN2/core/report/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       39 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/report/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12958 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/report/report_bam.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/core/report/report_files.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2826 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/gui.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.889255 DAJIN2-0.2.1/src/DAJIN2/postprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/postprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/postprocess/report.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1127 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/single.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.167118 DAJIN2-0.2.1/src/DAJIN2/static/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.906771 DAJIN2-0.2.1/src/DAJIN2/static/css/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/static/css/style.css
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/template_igvjs.html
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.923288 DAJIN2-0.2.1/src/DAJIN2/templates/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/templates/index.html
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.1/src/DAJIN2/view.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 07:55:38.366079 DAJIN2-0.2.1/src/DAJIN2.egg-info/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1670 2023-06-05 07:55:38.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       46 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/entry_points.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      237 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/requires.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-05 07:55:37.000000 DAJIN2-0.2.1/src/DAJIN2.egg-info/top_level.txt
```

### Comparing `DAJIN2-0.2.0/LICENSE` & `DAJIN2-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/PKG-INFO` & `DAJIN2-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.2.0
+Version: 0.2.1
 Summary: One-step genotyping tools for Nanopore amplicon sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `DAJIN2-0.2.0/README.md` & `DAJIN2-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/setup.py` & `DAJIN2-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 with open("requirements.txt") as requirements_file:
     install_requirements = requirements_file.read().splitlines()
 
 setuptools.setup(
     name="DAJIN2",
-    version="0.2.0",
+    version="0.2.1",
     author="Akihiro Kuno",
     author_email="akuno@md.tsukuba.ac.jp",
     description="One-step genotyping tools for Nanopore amplicon sequencing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akikuno/DAJIN2",
     install_requires=install_requirements,
```

### Comparing `DAJIN2-0.2.0/src/DAJIN2/DAJIN2.py` & `DAJIN2-0.2.1/src/DAJIN2/DAJIN2.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import wslPath
 
 from DAJIN2 import gui, view
 from DAJIN2.core import core_execute
 from DAJIN2.postprocess import report
 from DAJIN2.preprocess.validate_inputs import validate_files, validate_genome_and_fetch_urls
 
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 
 # prevent BLAS from using all cores
 os.environ["OMP_NUM_THREADS"] = "1"
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["VECLIB_MAXIMUM_THREADS"] = "1"
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
```

### Comparing `DAJIN2-0.2.0/src/DAJIN2/batch.py` & `DAJIN2-0.2.1/src/DAJIN2/batch.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/classification/classify.py` & `DAJIN2-0.2.1/src/DAJIN2/core/classification/classify.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/clustering/clustering.py` & `DAJIN2-0.2.1/src/DAJIN2/core/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/clustering/make_score.py` & `DAJIN2-0.2.1/src/DAJIN2/core/clustering/make_score.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/clustering/merge_clusters.py` & `DAJIN2-0.2.1/src/DAJIN2/core/clustering/merge_clusters.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/clustering/return_labels.py` & `DAJIN2-0.2.1/src/DAJIN2/core/clustering/return_labels.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/consensus/consensus.py` & `DAJIN2-0.2.1/src/DAJIN2/core/consensus/consensus.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/core_execute.py` & `DAJIN2-0.2.1/src/DAJIN2/core/core_execute.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/call_midsv.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/call_midsv.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/correct_knockin.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/correct_knockin.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/correct_sequence_error.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/correct_sequence_error.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import re
 from collections import defaultdict
 import numpy as np
 import scipy
-from statsmodels.nonparametric.smoothers_lowess import lowess as  sm_lowess
+from statsmodels.nonparametric.smoothers_lowess import lowess as sm_lowess
+
 
 def get_counts_homopolymer(indels_sample, indels_control, sequence):
     # Define a regular expression pattern for repeat regions
     repeat_pattern = r"A{4,}|C{4,}|G{4,}|T{4,}|N{4,}"
     # Find all match of repeat pattern in the sequence
     repeat_regions = list(match.span() for match in re.finditer(repeat_pattern, sequence))
     # Initialize default dictionaries to hold counts
@@ -33,25 +34,27 @@
         # Append the start, end, and total log mutations to the region count
         mutation_counts_regions.append((start, end, total_mutations_log))
         # Append the log mutation count to each position
         for position, value in enumerate(total_mutations_log):
             mutation_counts[position].append(value)
     return mutation_counts, mutation_counts_regions
 
+
 def _smooth_data(input_x, input_y, input_xgrid):
     # Sample 50 data points from the input x and y
     sampled_indices = np.random.choice(len(input_x), 50, replace=True)
     sampled_y = input_y[sampled_indices]
     sampled_x = input_x[sampled_indices]
     # Apply lowess smoothing to the sampled data
-    smoothed_y = sm_lowess(sampled_y, sampled_x, frac=1./5., it=5, return_sorted = False)
+    smoothed_y = sm_lowess(sampled_y, sampled_x, frac=1.0 / 5.0, it=5, return_sorted=False)
     # Interpolate the smoothed data onto the input grid
-    interpolated_y_grid = scipy.interpolate.interp1d(sampled_x, smoothed_y, fill_value='extrapolate')(input_xgrid)
+    interpolated_y_grid = scipy.interpolate.interp1d(sampled_x, smoothed_y, fill_value="extrapolate")(input_xgrid)
     return interpolated_y_grid
 
+
 def return_thresholds(mutation_counts) -> list(float):
     # Initialize empty lists to hold x and y data
     mutation_positions = []
     mutation_counts_log = []
     # Populate the x and y data with the mutation counts and positions
     for position, counts in mutation_counts.items():
         position_values = [position] * len(counts)
@@ -60,25 +63,27 @@
     # Convert x and y data to numpy arrays
     mutation_positions = np.array(mutation_positions)
     mutation_counts_log = np.array(mutation_counts_log)
     # Define a grid of x values from the minimum to the maximum position
     x_grid = np.linspace(mutation_positions.min(), mutation_positions.max(), mutation_positions.max() + 1)
     # Smooth the y data K times and stack the results
     num_smoothings = 100
-    smoothed_data = np.stack([_smooth_data(mutation_positions, mutation_counts_log, x_grid) for _ in range(num_smoothings)]).T
+    smoothed_data = np.stack(
+        [_smooth_data(mutation_positions, mutation_counts_log, x_grid) for _ in range(num_smoothings)]
+    ).T
     # Calculate the mean and standard error of the smoothed data
     mean_smoothed_data = np.nanmean(smoothed_data, axis=1)
     stderr_smoothed_data = scipy.stats.sem(smoothed_data, axis=1)
     stderr_smoothed_data = np.nanstd(smoothed_data, axis=1, ddof=0)
     # Define the thresholds as the mean plus 1.95 times the standard error
     thresholds = mean_smoothed_data + 1.95 * stderr_smoothed_data
     return thresholds
 
 
-def get_errors_in_homopolyer(mutation_counts_regions, thresholds) ->set(int):
+def get_errors_in_homopolyer(mutation_counts_regions, thresholds) -> set(int):
     # Initialize a set to hold the locations of mutations
     sequence_error_loci = set()
     # Iterate through each region and its associated mutation counts
     for start, end, log_mutations in mutation_counts_regions:
         # +-1 because 0-index is not considered as homopolymer
         if start > end:
             region = set(range(end, start - 1))
@@ -100,17 +105,18 @@
             if start > end:
                 mutations.add(start - 1 - mutation_index)
             else:
                 mutations.add(end + mutation_index)
         sequence_error_loci |= region - mutations
     return sequence_error_loci
 
+
 ###########################################################
 # main
 ###########################################################
 
+
 def extract_errors_in_homopolymer(indels_sample, indels_control, sequence) -> set(int):
     mutation_counts, mutation_counts_regions = get_counts_homopolymer(indels_sample, indels_control, sequence)
     thresholds = return_thresholds(mutation_counts)
     errors_in_homopolyer = get_errors_in_homopolyer(mutation_counts_regions, thresholds)
     return errors_in_homopolyer
-
```

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/extract_knockin_loci.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_knockin_loci.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/extract_mutation_loci.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/extract_mutation_loci.py`

 * *Files 8% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         indels_control = _count_indels(read_midsv(filepath_control), len(sequence))
         indels_sample_normalized = _normalize_indels(indels_sample, coverage_sample)
         indels_control_normalized = _normalize_indels(indels_control, coverage_control)
         indels_kmer_sample = _split_kmer(indels_sample_normalized, kmer=10)
         indels_kmer_control = _split_kmer(indels_control_normalized, kmer=10)
         anomaly_loci = _extract_anomaly_loci(indels_kmer_sample, indels_kmer_control)
         dissimilar_loci = _extract_dissimilar_loci(indels_kmer_sample, indels_kmer_control)
-        errors_in_homopolymer = extract_errors_in_homopolymer(indels_sample, indels_control, sequence)
+        # Extract error loci in homopolymer regions
+        error_loci_homopolymer = dict()
+        for mut in ["+", "-", "*"]:
+            candidate_loci = anomaly_loci[mut] & dissimilar_loci[mut]
+            indels_sample_mut = indels_sample[mut]
+            indels_control_mut = indels_control[mut]
+            error_loci = extract_errors_in_homopolymer(indels_sample_mut, indels_control_mut, sequence, candidate_loci)
+            error_loci_homopolymer.update({mut: error_loci})
         mutation_loci = dict()
-        for mut in anomaly_loci:
-            mutation_loci.update({mut: (anomaly_loci[mut] & dissimilar_loci[mut]) - errors_in_homopolymer})
+        for mut in ["+", "-", "*"]:
+            candidate_loci = anomaly_loci[mut] & dissimilar_loci[mut]
+            error_loci = error_loci_homopolymer[mut]
+            # Discard error loci in homopolymer regions
+            mutation_loci.update({mut: candidate_loci - error_loci})
         mutation_loci_transposed = _transpose_mutation_loci(mutation_loci, len(sequence))
         MUTATION_LOCI_ALLELES.update({allele: mutation_loci_transposed})
     return MUTATION_LOCI_ALLELES
```

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/format_inputs.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/format_inputs.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/mappy_align.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/mappy_align.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/replace_NtoD.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/replace_NtoD.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/validate_inputs.py` & `DAJIN2-0.2.1/src/DAJIN2/core/preprocess/validate_inputs.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/report/report_bam.py` & `DAJIN2-0.2.1/src/DAJIN2/core/report/report_bam.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/core/report/report_files.py` & `DAJIN2-0.2.1/src/DAJIN2/core/report/report_files.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/gui.py` & `DAJIN2-0.2.1/src/DAJIN2/gui.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/postprocess/report.py` & `DAJIN2-0.2.1/src/DAJIN2/postprocess/report.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/single.py` & `DAJIN2-0.2.1/src/DAJIN2/single.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/template_igvjs.html` & `DAJIN2-0.2.1/src/DAJIN2/template_igvjs.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/templates/index.html` & `DAJIN2-0.2.1/src/DAJIN2/templates/index.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2/view.py` & `DAJIN2-0.2.1/src/DAJIN2/view.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.0/src/DAJIN2.egg-info/PKG-INFO` & `DAJIN2-0.2.1/src/DAJIN2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.2.0
+Version: 0.2.1
 Summary: One-step genotyping tools for Nanopore amplicon sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `DAJIN2-0.2.0/src/DAJIN2.egg-info/SOURCES.txt` & `DAJIN2-0.2.1/src/DAJIN2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

