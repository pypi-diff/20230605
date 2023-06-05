# Comparing `tmp/DAJIN2-0.1.9.tar.gz` & `tmp/DAJIN2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DAJIN2-0.1.9.tar", last modified: Tue Oct 25 02:24:53 2022, max compression
+gzip compressed data, was "DAJIN2-0.2.0.tar", last modified: Mon Jun  5 05:29:31 2023, max compression
```

## Comparing `DAJIN2-0.1.9.tar` & `DAJIN2-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,64 @@
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.530000 DAJIN2-0.1.9/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1090 2021-11-02 03:02:14.000000 DAJIN2-0.1.9/LICENSE
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       51 2022-10-21 03:50:00.000000 DAJIN2-0.1.9/MANIFEST.in
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1326 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      882 2022-10-22 00:26:32.000000 DAJIN2-0.1.9/README.md
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/setup.cfg
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1078 2022-10-25 02:24:42.000000 DAJIN2-0.1.9/setup.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.560000 DAJIN2-0.1.9/src/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.590000 DAJIN2-0.1.9/src/DAJIN2/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4305 2022-10-20 03:39:06.000000 DAJIN2-0.1.9/src/DAJIN2/DAJIN2.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-06-01 03:40:28.000000 DAJIN2-0.1.9/src/DAJIN2/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2440 2022-10-20 04:06:14.000000 DAJIN2-0.1.9/src/DAJIN2/batch.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.640000 DAJIN2-0.1.9/src/DAJIN2/core/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-18 23:05:02.000000 DAJIN2-0.1.9/src/DAJIN2/core/__init__.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.670000 DAJIN2-0.1.9/src/DAJIN2/core/classification/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       72 2022-10-14 23:47:26.000000 DAJIN2-0.1.9/src/DAJIN2/core/classification/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1291 2022-10-14 08:26:46.000000 DAJIN2-0.1.9/src/DAJIN2/core/classification/classify.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2022-10-14 23:47:16.000000 DAJIN2-0.1.9/src/DAJIN2/core/classification/detect_sv.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.700000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       70 2022-10-15 20:47:06.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3282 2022-10-25 02:14:38.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/clustering_main.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3390 2022-10-09 04:32:38.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/make_scores.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1242 2022-10-25 01:23:36.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/mask_control.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1533 2022-10-09 03:39:40.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/return_labels.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6564 2022-10-25 02:24:14.000000 DAJIN2-0.1.9/src/DAJIN2/core/clustering/screen_diffloci.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.730000 DAJIN2-0.1.9/src/DAJIN2/core/consensus/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       33 2022-10-15 01:49:44.000000 DAJIN2-0.1.9/src/DAJIN2/core/consensus/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6882 2022-10-15 21:01:44.000000 DAJIN2-0.1.9/src/DAJIN2/core/consensus/consensus_main.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6870 2022-10-24 08:13:24.000000 DAJIN2-0.1.9/src/DAJIN2/core/core.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.760000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      106 2022-10-15 20:45:00.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      432 2022-10-07 03:32:56.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/calc_midsv.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4546 2022-10-24 08:12:10.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/check_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4141 2022-10-20 03:27:22.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/format_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3435 2022-10-25 00:21:36.000000 DAJIN2-0.1.9/src/DAJIN2/core/preprocess/mappy_align.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.790000 DAJIN2-0.1.9/src/DAJIN2/core/report/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       52 2022-10-05 02:14:58.000000 DAJIN2-0.1.9/src/DAJIN2/core/report/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11038 2022-10-21 06:50:06.000000 DAJIN2-0.1.9/src/DAJIN2/core/report/report_bam.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1154 2022-10-05 02:03:22.000000 DAJIN2-0.1.9/src/DAJIN2/core/report/report_files.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2427 2022-10-21 04:05:16.000000 DAJIN2-0.1.9/src/DAJIN2/gui.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.820000 DAJIN2-0.1.9/src/DAJIN2/postprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-20 07:45:58.000000 DAJIN2-0.1.9/src/DAJIN2/postprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2254 2022-10-20 03:51:18.000000 DAJIN2-0.1.9/src/DAJIN2/postprocess/report.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      208 2022-10-20 04:06:30.000000 DAJIN2-0.1.9/src/DAJIN2/single.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.850000 DAJIN2-0.1.9/src/DAJIN2/static/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.870000 DAJIN2-0.1.9/src/DAJIN2/static/css/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-07 04:06:40.000000 DAJIN2-0.1.9/src/DAJIN2/static/css/style.css
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.930000 DAJIN2-0.1.9/src/DAJIN2/templates/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1692 2022-10-07 07:26:20.000000 DAJIN2-0.1.9/src/DAJIN2/templates/index.html
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2582 2022-10-18 20:42:58.000000 DAJIN2-0.1.9/src/DAJIN2/view.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2022-10-25 02:24:52.610000 DAJIN2-0.1.9/src/DAJIN2.egg-info/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1326 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1342 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/SOURCES.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/dependency_links.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       46 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/entry_points.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      217 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/requires.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2022-10-25 02:24:54.000000 DAJIN2-0.1.9/src/DAJIN2.egg-info/top_level.txt
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.428880 DAJIN2-0.2.0/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.0/LICENSE
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.0/MANIFEST.in
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-05 05:29:31.424101 DAJIN2-0.2.0/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2918 2023-06-04 20:44:56.000000 DAJIN2-0.2.0/README.md
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-05 05:29:31.428880 DAJIN2-0.2.0/setup.cfg
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1077 2023-06-05 05:28:49.000000 DAJIN2-0.2.0/setup.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.005903 DAJIN2-0.2.0/src/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.266428 DAJIN2-0.2.0/src/DAJIN2/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11052 2023-06-05 05:29:01.000000 DAJIN2-0.2.0/src/DAJIN2/DAJIN2.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3881 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/batch.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.473150 DAJIN2-0.2.0/src/DAJIN2/core/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/__init__.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.596245 DAJIN2-0.2.0/src/DAJIN2/core/classification/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/classification/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/classification/classify.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/classification/detect_sv.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.788226 DAJIN2-0.2.0/src/DAJIN2/core/clustering/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/clustering.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/make_score.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/merge_clusters.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4239 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/clustering/return_labels.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.916369 DAJIN2-0.2.0/src/DAJIN2/core/consensus/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      311 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/consensus/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5873 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/consensus/consensus.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/consensus/subset.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10880 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/core_execute.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.222099 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      472 2023-06-05 05:23:44.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4912 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/call_midsv.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7398 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/correct_knockin.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10324 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/correct_sequence_error.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5883 2023-06-05 05:23:44.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/extract_knockin_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7038 2023-06-05 05:23:44.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/extract_mutation_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4356 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/format_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/mappy_align.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/replace_NtoD.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5139 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/preprocess/validate_inputs.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.315369 DAJIN2-0.2.0/src/DAJIN2/core/report/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       39 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/report/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12958 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/report/report_bam.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/core/report/report_files.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2826 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/gui.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.360915 DAJIN2-0.2.0/src/DAJIN2/postprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/postprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/postprocess/report.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1127 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/single.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.060594 DAJIN2-0.2.0/src/DAJIN2/static/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.385436 DAJIN2-0.2.0/src/DAJIN2/static/css/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/static/css/style.css
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/template_igvjs.html
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:31.407586 DAJIN2-0.2.0/src/DAJIN2/templates/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/templates/index.html
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.0/src/DAJIN2/view.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 05:29:30.410614 DAJIN2-0.2.0/src/DAJIN2.egg-info/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1670 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       46 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/entry_points.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      217 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/requires.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-05 05:29:29.000000 DAJIN2-0.2.0/src/DAJIN2.egg-info/top_level.txt
```

### Comparing `DAJIN2-0.1.9/LICENSE` & `DAJIN2-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Akihiro Kuno
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Akihiro Kuno
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `DAJIN2-0.1.9/setup.py` & `DAJIN2-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-import setuptools
-from pathlib import Path
-
-from pathlib import Path
-
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
-
-with open("requirements.txt") as requirements_file:
-    install_requirements = requirements_file.read().splitlines()
-
-setuptools.setup(
-    name="DAJIN2",
-    version="0.1.9",
-    author="Akihiro Kuno",
-    author_email="akuno@md.tsukuba.ac.jp",
-    description="One-step genotyping tools for Nanopore amplicon sequencing",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/akikuno/DAJIN2",
-    install_requires=install_requirements,
-    packages=setuptools.find_packages(where="src",),
-    package_dir={"": "src"},
-    entry_points={"console_scripts": ["DAJIN2=DAJIN2.DAJIN2:main"]},
-    include_package_data=True,
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: POSIX",
-    ],
-    python_requires=">=3.7",
-)
+import setuptools
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
+with open("requirements.txt") as requirements_file:
+    install_requirements = requirements_file.read().splitlines()
+
+setuptools.setup(
+    name="DAJIN2",
+    version="0.2.0",
+    author="Akihiro Kuno",
+    author_email="akuno@md.tsukuba.ac.jp",
+    description="One-step genotyping tools for Nanopore amplicon sequencing",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/akikuno/DAJIN2",
+    install_requires=install_requirements,
+    packages=setuptools.find_packages(
+        where="src",
+    ),
+    package_dir={"": "src"},
+    entry_points={"console_scripts": ["DAJIN2=DAJIN2.DAJIN2:main"]},
+    include_package_data=True,
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: POSIX",
+        "Development Status :: 3 - Alpha",
+    ],
+    python_requires=">=3.7",
+)
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2/core/preprocess/check_inputs.py` & `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/validate_inputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
-from pathlib import Path
-import re
-import mappy
+
 import hashlib
-from urllib.request import urlopen
+import re
+from pathlib import Path
 from urllib.error import URLError
+from urllib.request import urlopen
+
+import mappy
 
 
 def exists(input_file: str):
     if not Path(input_file).exists():
         raise FileNotFoundError(f"{input_file} is not found")
 
 
@@ -41,15 +43,15 @@
     if not len(name) == len(seq) > 0:
         raise AttributeError(f"{fasta_path} is not a FASTA format")
     if len(name) > len(set(name)):
         raise AttributeError(f"{fasta_path} must include unique identifiers")
     if len(seq) > len(set(seq)):
         raise AttributeError(f"{fasta_path} must include unique DNA sequences")
     if name.count("control") == 0:
-        raise AttributeError(f"{fasta_path} must include a 'control' sequence")
+        raise AttributeError(f"One of the headers in the {fasta_path} must be '>control'")
 
 
 def check_files(SAMPLE: str, CONTROL: str, ALLELE: str) -> None:
     exists(CONTROL)
     exists(SAMPLE)
     exists(ALLELE)
     fastq_extension(CONTROL)
@@ -86,53 +88,63 @@
 
 
 ########################################################################
 # Check genome and UCSC server
 ########################################################################
 
 
-def available_url(urls: list[str]) -> tuple[str, bool]:
-    flag_fail = False
-    url = ""
+def _check_url_availabilities(urls: list[str]) -> list[bool]:
+    availabilities = []
     for url in urls:
         try:
-            _ = urlopen(url)
+            _ = urlopen(url, timeout=10)
         except URLError:
-            flag_fail = True
+            availabilities.append(False)
         else:
-            flag_fail = False
-            break
-    return url, flag_fail
+            availabilities.append(True)
+    return availabilities
+
 
+def _extract_available_urls(urls: list[str], availabilities: list[bool]) -> list[str]:
+    available_urls = []
+    for url, flag in zip(urls, availabilities):
+        if flag:
+            available_urls.append(url)
+    return available_urls
 
-def available_genome(genome: str, ucsc_url: str):
+
+def _is_listed(genome: str, ucsc_url: str) -> None:
     url = f"{ucsc_url}/cgi-bin/das/{genome}/dna?segment=1:1,10"
-    response = urlopen(url)
+    response = urlopen(url, timeout=10)
     content = response.read()
     response.close()
     if not content:
         raise AttributeError(
             f"{genome} is not listed in UCSC genome browser. Available genomes are in {ucsc_url}/cgi-bin/das/dsn"
         )
 
 
-def check_and_fetch_genome(GENOME: str) -> tuple(str, str):
+def check_and_fetch_genome(GENOME: str) -> tuple[str, str]:
     # Check UCSC Server
     UCSC_URLS = [
         "https://genome.ucsc.edu/",
         "https://genome-asia.ucsc.edu/",
         "https://genome-euro.ucsc.edu/",
     ]
-    UCSC_URL, flag_fail = available_url(UCSC_URLS)
-    if flag_fail:
-        raise URLError("UCSC Servers are currently down")
+    url_availabilities = _check_url_availabilities(UCSC_URLS)
+    if not any(url_availabilities):
+        raise URLError("All servers of UCSC Genome Browsers are currently down. Please wait for a while and try again.")
+
+    UCSC_URL = _extract_available_urls(UCSC_URLS, url_availabilities)[0]
+
     # Check UCSC Download Server
     GOLDENPATH_URLS = [
         "https://hgdownload.cse.ucsc.edu/goldenPath",
         "http://hgdownload-euro.soe.ucsc.edu/goldenPath",
     ]
-    GOLDENPATH_URL, flag_fail = available_url(GOLDENPATH_URLS)
-    if flag_fail:
-        raise URLError("UCSC Download Servers are currently down")
+    url_availabilities = _check_url_availabilities(UCSC_URLS)
+    if not any(url_availabilities):
+        raise URLError("All servers of UCSC GoldenPath are currently down. Please wait for a while and try again.")
+    GOLDENPATH_URL = _extract_available_urls(GOLDENPATH_URLS, url_availabilities)[0]
     # Check input genome
-    available_genome(GENOME, UCSC_URL)
+    _is_listed(GENOME, UCSC_URL)
     return UCSC_URL, GOLDENPATH_URL
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2/core/preprocess/format_inputs.py` & `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/format_inputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 from __future__ import annotations
 
+import os
+import re
 from pathlib import Path
 from urllib.request import urlopen
-import re
+
 import mappy
 import midsv
+import wslPath
 
 ########################################################################
 # Make directories
 ########################################################################
 
 
-def make_directories(TEMPDIR: Path):
-    subdirectoris = ["cache", "fasta", "sam", "midsv", "report", "result"]
-    for subdir in subdirectoris:
+def make_directories(TEMPDIR: Path, SUBDIRS: list[str], SUBDIRS_REPORT: list[str], SAMPLE_NAME: str, CONTROL_NAME: str):
+    for subdir in SUBDIRS:
         Path(TEMPDIR, subdir).mkdir(parents=True, exist_ok=True)
-    reportdirectories = ["HTML", "FASTA", "VCF", "BAM", ".igvjs"]
-    for reportdir in reportdirectories:
-        Path(TEMPDIR, "report", reportdir).mkdir(parents=True, exist_ok=True)
+    for reportdir in SUBDIRS_REPORT:
+        Path(TEMPDIR, "report", reportdir, SAMPLE_NAME).mkdir(parents=True, exist_ok=True)
+    Path(TEMPDIR, "report", "BAM", CONTROL_NAME).mkdir(parents=True, exist_ok=True)
+    Path(TEMPDIR, "cache", ".igvjs").mkdir(parents=True, exist_ok=True)
+
+
+########################################################################
+# Convert Path
+########################################################################
+
+
+def convert_to_posix_path(path: str) -> str:
+    try:
+        path = wslPath.toPosix(path)
+    except ValueError:
+        pass
+    return str(path)
 
 
 ########################################################################
 # Extract basename
 ########################################################################
 
 
@@ -49,14 +65,25 @@
         name = re.sub(r'[\\|/|:|?|.|,|\'|"|<|>|\| |]', "-", name)
         header.append(name)
         sequence.append(seq.upper())
     return {h: s for h, s in zip(header, sequence)}
 
 
 ########################################################################
+# Update threads
+########################################################################
+
+
+def update_threads(threads):
+    threads_updated = min(int(threads), os.cpu_count() - 1)
+    threads_updated = max(1, threads_updated)
+    return threads_updated
+
+
+########################################################################
 # Fetch genome coodinate and chrom size
 ########################################################################
 
 
 # TODO TEST
 def fetch_coodinate(genome: str, ucsc_url: str, seq: str) -> dict:
     ucsc_blat = f"{ucsc_url}/cgi-bin/hgBlat?db={genome}&type=BLAT&userSeq={seq}"
@@ -75,29 +102,18 @@
     for req in request:
         req = req.split("\t")
         if chrom == req[0]:
             chrom_size = int(req[1])
     return chrom_size
 
 
-def get_coodinates_and_chromsize(
-    TEMPDIR, GENOME, DICT_ALLELE, UCSC_URL, GOLDENPATH_URL, IS_CACHE_GENOME: bool
-) -> tuple:
-    path_genome_coodinates = Path(TEMPDIR, "cache", "genome_coodinates.jsonl")
-    path_chrome_size = Path(TEMPDIR, "cache", "chrome_size.txt")
-    if IS_CACHE_GENOME:
-        GENOME_COODINATES = midsv.read_jsonl(path_genome_coodinates)[0]
-        CHROME_SIZE = int(path_chrome_size.read_text())
-    else:
-        GENOME_COODINATES = fetch_coodinate(GENOME, UCSC_URL, DICT_ALLELE["control"])
-        CHROME_SIZE = fetch_chrom_size(GENOME_COODINATES["chr"], GENOME, GOLDENPATH_URL)
-    return GENOME_COODINATES, CHROME_SIZE
-
-
 def cache_coodinates_and_chromsize(TEMPDIR, GENOME, GENOME_COODINATES, CHROME_SIZE):
+    """
+    Save (1) genome_symbol.txt, (2) genome_coodinates.jsonl, (3) chrome_size.txt
+    """
     # Save info to the cache directory
     Path(TEMPDIR, "cache", "genome_symbol.txt").write_text(GENOME + "\n")
     midsv.write_jsonl([GENOME_COODINATES], Path(TEMPDIR, "cache", "genome_coodinates.jsonl"))
     Path(TEMPDIR, "cache", "chrome_size.txt").write_text(str(CHROME_SIZE))
     # Save info to the .igvjs directory
     Path(TEMPDIR, "report", ".igvjs", "genome_symbol.txt").write_text(GENOME + "\n")
     midsv.write_jsonl([GENOME_COODINATES], Path(TEMPDIR, "report", ".igvjs", "genome_coodinates.jsonl"))
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2/core/preprocess/mappy_align.py` & `DAJIN2-0.2.0/src/DAJIN2/core/preprocess/mappy_align.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 from __future__ import annotations
+
 from collections.abc import Generator
-from copy import deepcopy
 from pathlib import Path
-from typing import Union
+
 import cstag
 import mappy
 
 
 def revcomp(sequence: str) -> str:
     complement = {"A": "T", "C": "G", "G": "C", "T": "A"}
     return "".join(complement[nt] for nt in sequence[::-1])
 
 
-def to_sam(path_reference_fasta: str, path_query_fastq: str, cslong: bool = True) -> Generator[str]:
+def to_sam(
+    path_reference_fasta: str | Path,
+    path_query_fastx: str | Path,
+    preset: str = "map-ont",
+    threads: int = 1,
+    cslong: bool = True,
+) -> Generator[str]:
     """Align seqences using mappy and Convert PAF to SAM
 
     Args:
         path_reference_fasta (str): Path of reference fasta
-        path_query_fastq (str): Path of query fasta/fastq
+        path_query_fastx (str): Path of query fasta/fastq
         cslong (bool, optional): long formatted CS tag if True. Defaults to True
 
     Returns:
         list: List of SAM
     """
+    path_reference_fasta = str(path_reference_fasta)
+    path_query_fastx = str(path_query_fastx)
     # SQ header
     SAM = [f"@SQ\tSN:{n}\tLN:{len(s)}" for n, s, _ in mappy.fastx_read(path_reference_fasta)]
     # Mappy
-    ref = mappy.Aligner(path_reference_fasta)
+    ref = mappy.Aligner(path_reference_fasta, preset=preset, n_threads=threads)
     if not ref:
         raise AttributeError(f"Failed to load {path_reference_fasta}")
-    for MAPPY_NAME, MAPPY_SEQ, MAPPY_QUAL in mappy.fastx_read(path_query_fastq):
+    for MAPPY_NAME, MAPPY_SEQ, MAPPY_QUAL in mappy.fastx_read(path_query_fastx):
         for hit in ref.map(MAPPY_SEQ, cs=True):
-            query_seq = deepcopy(MAPPY_SEQ)
-            query_qual = deepcopy(MAPPY_QUAL)
+            query_seq = MAPPY_SEQ
+            query_qual = MAPPY_QUAL
             # flag
             if hit.is_primary:
                 flag = 0 if hit.strand == 1 else 16
             else:
                 flag = 2048 if hit.strand == 1 else 2064
             # Append softclips to CIGAR
             cigar = hit.cigar_str
@@ -45,15 +53,16 @@
                 cigar = softclip + cigar if hit.strand == 1 else cigar + softclip
             if len(MAPPY_SEQ) - hit.q_en > 0:
                 softclip = str(len(MAPPY_SEQ) - hit.q_en) + "S"
                 cigar = cigar + softclip if hit.strand == 1 else softclip + cigar
             # Revcomp
             if hit.strand == -1:
                 query_seq = revcomp(query_seq)
-                query_qual = query_qual[::-1]
+                if query_qual:
+                    query_qual = query_qual[::-1]
             query_seq = query_seq.upper()
             # cslong
             cs = "cs:Z:" + hit.cs
             if cslong:
                 cs = cstag.lengthen(hit.cs, cigar, query_seq)
             # summarize
             alignment = [
@@ -72,26 +81,34 @@
             ]
             alignment = [str(a) for a in alignment]
             SAM.append("\t".join(alignment))
     for record in SAM:
         yield record
 
 
-def output_sam(TEMPDIR, path_fasta, name_fasta, path_fastq, name_fastq):
-    sam = to_sam(str(path_fasta), path_fastq)
-    output_sam = Path(TEMPDIR, "sam", f"{name_fastq}_{name_fasta}.sam")
+def output_sam(
+    tmpdir: Path,
+    path_fasta: str | Path,
+    name_fasta: str,
+    path_fastq: str | Path,
+    name_fastq: str,
+    preset: str = "map-ont",
+    threads: int = 1,
+):
+    sam = to_sam(path_fasta, path_fastq, preset=preset, threads=threads)
+    output_sam = Path(tmpdir, "sam", f"{name_fastq}_{preset}_{name_fasta}.sam")
     output_sam.write_text("\n".join(sam))
 
 
 ########################################################################
 # Create faidx
 ########################################################################
 
 
-def make_faidx(path_fasta: Union[Path, str]) -> str:
+def make_faidx(path_fasta: Path | str) -> str:
     fasta = Path(path_fasta).read_text().split()
     name = fasta[0].strip(">")
     length = len("".join(fasta[1:]))
     offset = len(fasta[0]) + 1
     linebase = len(fasta[1])
     linewidth = len(fasta[1]) + 1
     faidx = list(map(str, [name, length, offset, linebase, linewidth]))
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2/core/report/report_bam.py` & `DAJIN2-0.2.0/src/DAJIN2/core/report/report_bam.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
-import re
+
 import random
-from pathlib import Path
-from typing import Union
+import re
 from collections import defaultdict
 from itertools import groupby
-from copy import deepcopy
-import pysam
+from pathlib import Path
+from typing import Union
+
 import midsv
+import pysam
 
 
 def revcomp(sequence: str) -> str:
     complement = {"A": "T", "C": "G", "G": "C", "T": "A"}
     return "".join(complement[nt] for nt in sequence[::-1])
 
 
@@ -171,28 +172,29 @@
         sam_update[3] = str(genome_end - (sam_start + sam_length) + 2)
         sam_update[9] = revcomp(sam_content[9])
         sam_update[10] = sam_content[10][::-1]
         sam_reversed.append(sam_update)
     return sam_reversed
 
 
-def realign(sam: list[list[str]], genome_coodinates: dict, chrom_size: int) -> list[str]:
+def realign(sam: list[list[str]], GENOME_COODINATES: dict, CHROME_SIZE: int) -> list[str]:
     sam_headers = [s for s in sam if s[0].startswith("@")]
     sam_contents = [s for s in sam if not s[0].startswith("@")]
     for s in sam_headers:
         if s[0] != "@SQ":
             continue
-        s[1] = f'SN:{genome_coodinates["chr"]}'
-        s[2] = f"LN:{chrom_size}"
+        s[1] = f'SN:{GENOME_COODINATES["chr"]}'
+        s[2] = f"LN:{CHROME_SIZE}"
     for s in sam_contents:
-        s[2] = genome_coodinates["chr"]
-    if genome_coodinates["strand"] == "-":
-        sam_contents = reverse_sam(sam_contents, genome_coodinates["end"])
+        s[2] = GENOME_COODINATES["chr"]
+    if GENOME_COODINATES["strand"] == "-":
+        sam_contents = reverse_sam(sam_contents, GENOME_COODINATES["end"])
     else:
-        s[3] = str(int(s[3]) + genome_coodinates["start"] - 1)
+        for s in sam_contents:
+            s[3] = str(int(s[3]) + GENOME_COODINATES["start"] - 1)
     return sam_headers + sam_contents
 
 
 def group_by_name(sam_contents: list[str], clust_sample: list[dict]) -> dict[list]:
     sam_contents.sort()
     clust_sample_qname = sorted(clust_sample, key=lambda x: x["QNAME"])
     clust_sample_qname_set = set()
@@ -240,50 +242,78 @@
 
 
 ###############################################################################
 # Output
 ###############################################################################
 
 
-def output_bam(TEMPDIR, RESULT_SAMPLE, SAMPLE_NAME, GENOME, GENOME_COODINATES, CHROME_SIZE, THREADS):
+def output_bam_control(TEMPDIR, CONTROL_NAME, GENOME, GENOME_COODINATES, CHROME_SIZE, THREADS):
     randomnum = random.randint(100_000, 999_999)
-    path_sam = Path(TEMPDIR, "sam", f"{SAMPLE_NAME}_control.sam")
-    sam = midsv.read_sam(path_sam)
-
-    sam_update = deepcopy(sam)
+    intput_path_sam = Path(TEMPDIR, "sam", f"{CONTROL_NAME}_map-ont_control.sam")
+    sam = list(midsv.read_sam(intput_path_sam))
+    # Update sam
+    sam_update = sam.copy()
     sam_update = remove_overlapped_reads(sam_update)
     sam_update = remove_microhomology(sam_update)
-
-    path_sam_update = Path(TEMPDIR, "report", "bam", f"tmp{randomnum}_{SAMPLE_NAME}_control.sam")
     if GENOME:
         sam_update = realign(sam_update, GENOME_COODINATES, CHROME_SIZE)
-        write_sam(sam_update, path_sam_update)
-    else:
-        write_sam(sam_update, path_sam_update)
-
-    path_bam = Path(TEMPDIR, "report", "bam", f"{SAMPLE_NAME}.bam")
-    pysam.sort("-@", f"{THREADS}", "-o", str(path_bam), str(path_sam_update))
+    # Output SAM/BAM
+    output_path_sam = Path(TEMPDIR, "report", "BAM", f"tmp{randomnum}_{CONTROL_NAME}_control.sam")
+    output_path_bam = Path(TEMPDIR, "report", "BAM", CONTROL_NAME, f"{CONTROL_NAME}.bam")
+    write_sam(sam_update, output_path_sam)
+    pysam.sort("-@", f"{THREADS}", "-o", str(output_path_bam), str(output_path_sam))
+    pysam.index("-@", f"{THREADS}", str(output_path_bam))
+    # igvjs
+    sam_headers = [s for s in sam_update if s[0].startswith("@")]
+    sam_contents = [s for s in sam_update if not s[0].startswith("@")]
+    qnames = [s[0] for s in sam_contents[:10000]]
+    qnames = set(list(set(qnames))[:100])
+    sam_subset = [s for s in sam_update if s[0] in qnames]
+    output_path_sam = Path(TEMPDIR, "report", "BAM", f"tmp{randomnum}_{CONTROL_NAME}_control_cache.sam")
+    write_sam(sam_headers + sam_subset, output_path_sam)
+    path_bam = Path(TEMPDIR, "cache", ".igvjs", f"{CONTROL_NAME}_control.bam")
+    pysam.sort("-@", f"{THREADS}", "-o", str(path_bam), str(output_path_sam))
     pysam.index("-@", f"{THREADS}", str(path_bam))
+    # Remove temporary files
+    sam_temp = Path(TEMPDIR, "report", "BAM").glob(f"tmp{randomnum}*.sam")
+    [s.unlink() for s in sam_temp]
+
 
+def output_bam_sample(TEMPDIR, RESULT_SAMPLE, SAMPLE_NAME, GENOME, GENOME_COODINATES, CHROME_SIZE, THREADS):
+    randomnum = random.randint(100_000, 999_999)
+    input_path_sam = Path(TEMPDIR, "sam", f"{SAMPLE_NAME}_map-ont_control.sam")
+    sam = list(midsv.read_sam(input_path_sam))
+    # Update sam
+    sam_update = sam.copy()
+    sam_update = remove_overlapped_reads(sam_update)
+    sam_update = remove_microhomology(sam_update)
+    if GENOME:
+        sam_update = realign(sam_update, GENOME_COODINATES, CHROME_SIZE)
+    # Output SAM/BAM
+    output_path_sam = Path(TEMPDIR, "report", "BAM", f"tmp{randomnum}_{SAMPLE_NAME}_control.sam")
+    output_path_bam = Path(TEMPDIR, "report", "BAM", SAMPLE_NAME, f"{SAMPLE_NAME}.bam")
+    write_sam(sam_update, output_path_sam)
+    pysam.sort("-@", f"{THREADS}", "-o", str(output_path_bam), str(output_path_sam))
+    pysam.index("-@", f"{THREADS}", str(output_path_bam))
+    # Prepare SAM according to LABEL
     sam_headers = [s for s in sam_update if s[0].startswith("@")]
     sam_contents = [s for s in sam_update if not s[0].startswith("@")]
     sam_groups = group_by_name(sam_contents, RESULT_SAMPLE)
     qnames_by_name = subset_qnames(RESULT_SAMPLE)
-
+    # Output SAM/BAM
     for name, sam_content in sam_groups.items():
         # BAM
-        path_sam = Path(TEMPDIR, "report", "bam", f"tmp{randomnum}_{name}.sam")
-        path_bam = Path(TEMPDIR, "report", "bam", f"{SAMPLE_NAME}_{name}.bam")
-        write_sam(sam_headers + sam_content, path_sam)
-        pysam.sort("-@", f"{THREADS}", "-o", str(path_bam), str(path_sam))
-        pysam.index("-@", f"{THREADS}", str(path_bam))
+        output_path_sam = Path(TEMPDIR, "report", "bam", f"tmp{randomnum}_{name}.sam")
+        output_path_bam = Path(TEMPDIR, "report", "BAM", SAMPLE_NAME, f"{SAMPLE_NAME}_{name}.bam")
+        write_sam(sam_headers + sam_content, output_path_sam)
+        pysam.sort("-@", f"{THREADS}", "-o", str(output_path_bam), str(output_path_sam))
+        pysam.index("-@", f"{THREADS}", str(output_path_bam))
         # igvjs
         sam_subset = subset_reads(name, sam_content, qnames_by_name)
-        path_sam = Path(TEMPDIR, "report", "bam", f"tmp{randomnum}_{name}_subset.sam")
-        path_bam = Path(TEMPDIR, "report", ".igvjs", f"{SAMPLE_NAME}_{name}.bam")
-        write_sam(sam_headers + sam_subset, path_sam)
-        pysam.sort("-@", f"{THREADS}", "-o", str(path_bam), str(path_sam))
-        pysam.index("-@", f"{THREADS}", str(path_bam))
-
+        output_path_sam = Path(TEMPDIR, "report", "bam", f"tmp{randomnum}_{name}_subset.sam")
+        write_sam(sam_headers + sam_subset, output_path_sam)
+        output_path_bam = Path(TEMPDIR, "report", ".igvjs", SAMPLE_NAME, f"{name}.bam")
+        pysam.sort("-@", f"{THREADS}", "-o", str(output_path_bam), str(output_path_sam))
+        pysam.index("-@", f"{THREADS}", str(output_path_bam))
     # Remove temporary files
     sam_temp = Path(TEMPDIR, "report", "bam").glob(f"tmp{randomnum}*.sam")
     [s.unlink() for s in sam_temp]
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2/core/report/report_files.py` & `DAJIN2-0.2.0/src/DAJIN2/core/report/report_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
-import cstag
+
 import textwrap
 
+import cstag
+
 
 def to_fasta(header: str, cons_seq: str) -> str:
     header = ">" + header
     cons_seq_wrap = textwrap.wrap(cons_seq, 80)
     fasta = "\n".join([header, *cons_seq_wrap]) + "\n"
     return fasta
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2/gui.py` & `DAJIN2-0.2.0/src/DAJIN2/gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,27 @@
-from flask import Flask, render_template, request
-from werkzeug.utils import secure_filename
+import os
+import socket
 import webbrowser
-from threading import Timer
-from waitress import serve
+from contextlib import closing, redirect_stderr
 from pathlib import Path
+from threading import Timer
+
 import pandas as pd
-from . import batch
+from flask import Flask, render_template, request
+from waitress import serve
+from werkzeug.utils import secure_filename
+
+from DAJIN2 import batch
 
 
-def open_browser():
-    webbrowser.open_new("http://127.0.0.1:2000/")
+def find_free_port():
+    with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
+        s.bind(("", 0))
+        s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        return s.getsockname()[1]
 
 
 def upload_files(files):
     for file in files:
         path = Path(app.config["UPLOAD_FOLDER"], secure_filename(file.filename))
         file.save(path)
 
@@ -79,12 +87,17 @@
     allele={PATH_ALLELE}
     genome={genome}
     threads={threads}
     arguments={arguments["file"]}
     """
 
 
-def execute():
-    print("Assess 'http://127.0.0.1:2000/' if browser does not automatically open.")
-    Timer(1, open_browser).start()
-    serve(app, host="0.0.0.0", port=2000)
+def open_browser(PORT):
+    webbrowser.open_new(f"http://127.0.0.1:{PORT}/")
+
 
+def execute():
+    PORT = find_free_port()
+    print(f"Assess 'http://127.0.0.1:{PORT}/' if a browser does not automatically open.")
+    Timer(1, open_browser, [PORT]).start()
+    with redirect_stderr(open(os.devnull, "w")):
+        serve(app, host="0.0.0.0", port=PORT)
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2/postprocess/report.py` & `DAJIN2-0.2.0/src/DAJIN2/postprocess/report.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
-import pandas as pd
+
 import shutil
 from pathlib import Path
+
 import midsv
+import pandas as pd
 import plotly.express as px
 
 
-def all_info(batch_directory: Path) -> pd.DataFrame:
+def extract_all_info(batch_directory: Path) -> pd.DataFrame:
     df_results = pd.DataFrame()
-    colum = ["SAMPLE", "QNAME", "NAME", "READNUM", "PERCENT", "LABEL", "ALLELE", "SV"]
-    for path_result in batch_directory.iterdir():
+    colum = ["SAMPLE", "QNAME", "NAME", "READNUM", "PERCENT", "LABEL", "ALLELE"]
+    for path_result in sorted(batch_directory.iterdir()):
         sample_name = path_result.stem
         result_jsonl = midsv.read_jsonl(path_result)
         df_clust_sample = pd.DataFrame(result_jsonl)
         df_clust_sample["SAMPLE"] = sample_name
         df_clust_sample = df_clust_sample[colum]
         df_results = pd.concat([df_results, df_clust_sample])
     return df_results
 
 
-def summary_info(df_all: pd.DataFrame) -> pd.DataFrame:
-    df_summary = df_all.drop(columns=["QNAME", "LABEL", "ALLELE", "SV"]).drop_duplicates()
+def summarize_info(df_all: pd.DataFrame) -> pd.DataFrame:
+    df_summary = df_all.drop(columns=["QNAME", "LABEL", "ALLELE"]).drop_duplicates()
     return df_summary
 
 
 def output_plot(df_summary: pd.DataFrame, report_directory: Path):
     df_plot = df_summary.copy()
     name = df_plot.NAME.tolist()
     names = [n.split("_") for n in name]
@@ -35,26 +37,27 @@
         x="SAMPLE",
         y="PERCENT",
         color="ALLELETYPE",
         text="PERCENT",
         labels={"SAMPLE": "Samples", "PERCENT": "% of reads", "ALLELETYPE": "Alelle type"},
     )
     fig.update_traces(textposition="inside", cliponaxis=False)
+    fig.update_xaxes(categoryorder="category ascending")
     output_filename = str(Path(report_directory, "read_plot"))
     fig.write_html(f"{output_filename}.html")
     # if kaleido is installed, output a pdf
     try:
         fig.write_image(f"{output_filename}.pdf")
     except ValueError:
         pass
 
 
 def report(name: str):
     report_directory = Path("DAJINResults", name)
     report_directory.mkdir(exist_ok=True, parents=True)
-    for dir in Path("DAJINResults", ".tempdir", name, "report").iterdir():
-        shutil.copytree(dir, Path(report_directory, dir.stem), dirs_exist_ok=True)
-    df_all = all_info(Path("DAJINResults", ".tempdir", name, "result"))
+    for directory in Path("DAJINResults", ".tempdir", name, "report").iterdir():
+        shutil.copytree(directory, Path(report_directory, directory.stem), dirs_exist_ok=True)
+    df_all = extract_all_info(Path("DAJINResults", ".tempdir", name, "result"))
     df_all.to_csv(Path(report_directory, "read_all.csv"), index=False)
-    df_summary = summary_info(df_all)
+    df_summary = summarize_info(df_all)
     df_summary.to_csv(Path(report_directory, "read_summary.csv"), index=False)
     output_plot(df_summary, report_directory)
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2/templates/index.html` & `DAJIN2-0.2.0/src/DAJIN2/templates/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 <head>
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <title>DAJIN</title>
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" rel="stylesheet"
         integrity="sha384-Zenh87qX5JnK2Jl0vWa8Ck2rdkQ2Bzep5IDxbcnCeuOxjzrPF/et3URy9Bv1WTRi" crossorigin="anonymous">
+    <link href="/static/css/style.css" rel="stylesheet" type="text/css" media="all">
 </head>
 
 <body>
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js"
         integrity="sha384-OERcA2EqjJCMA+/3y+gxIOqMEjwtxJY7qPCqsdltbNJuaOe923+mo//f6V8Qbsw3"
         crossorigin="anonymous"></script>
 
@@ -27,15 +28,15 @@
         <h2> Control FASTQ </h2>
         <input class="form-control" type="file" name="control" accept=".fastq, .fq, .fastq.gz, .fq.gz" required />
 
         <h2> Allele FASTA </h2>
         <input class="form-control" type="file" name="allele" accept=".fasta, .fa" multiple required />
 
         <h2> Genome (optional) </h2>
-        <input class="form-control" type="text" name="genome" placeholder="(e.g. mm19)" />
+        <input class="form-control" type="text" name="genome" placeholder="(e.g. hg38)" />
 
         <h2> Threads (optional) </h2>
         <input class="form-control" type="number" name="threads" min="1" />
 
         <br>
 
         <input class="btn btn-primary" type="submit" name="submit" value="Run DAJIN" />
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 
 
+
 ****** DAJIN2 ******
 ***** Name *****
 [name                ]
 ***** Sample FASTQs *****
 [File]
 ***** Control FASTQ *****
 [File]
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2/view.py` & `DAJIN2-0.2.0/src/DAJIN2/view.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,38 @@
+import http.server
 import os
 import re
-from pathlib import Path
-import http.server
+import socket
 import socketserver
 import webbrowser
-import socket
-from contextlib import closing
-from jinja2 import Template, Environment, FileSystemLoader
+from contextlib import closing, redirect_stderr
+from pathlib import Path
+from threading import Timer
+
+from jinja2 import Environment, FileSystemLoader, Template
 
 
 def find_free_port():
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
         s.bind(("", 0))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         return s.getsockname()[1]
 
 
+def open_browser(PORT):
+    webbrowser.open_new(f"http://127.0.0.1:{PORT}/")
+
+
 def execute(name: str):
     DIR_IGVJS = Path("DAJINResults", name, ".igvjs")
     if not DIR_IGVJS.exists():
-        raise FileNotFoundError("BAM files for DAJIN view is not found. Execute DAJIN first.")
-    env = Environment(loader=FileSystemLoader("./", encoding="utf8"))
-    template = env.get_template("src/DAJIN2/template_igvjs.html")
+        raise FileNotFoundError(f"BAM files are not found in {DIR_IGVJS.parent}. Please run DAJIN first.")
+    path_view = Path(__file__).parent
+    env = Environment(loader=FileSystemLoader(path_view, encoding="utf8"))
+    template = env.get_template("template_igvjs.html")
     params_genome = {"genome": {"exist": False}}
     params_reference = dict()
     path_genome = Path(DIR_IGVJS, "genome_symbol.txt")
     if path_genome.exists():
         path_coodinates = Path(DIR_IGVJS, "genome_coodinates.jsonl")
         GENOME = path_genome.read_text().strip()
         CHROME, START, END, _ = eval(path_coodinates.read_text().strip()).values()
@@ -57,13 +64,14 @@
     params_genome.update(**params_reference, **params_tracks)
     params = params_genome.copy()
 
     HTML_IGVJS = template.render(params)
     Path(DIR_IGVJS, "index.html").write_text(HTML_IGVJS)
     PORT = find_free_port()
     Handler = http.server.SimpleHTTPRequestHandler
+
     os.chdir(Path("DAJINResults", name, ".igvjs"))
     with socketserver.TCPServer(("", PORT), Handler) as httpd:
-        print(f"serving at port: http://127.0.0.1:{PORT}")
-        httpd.serve_forever()
-        webbrowser.open(f"http://127.0.0.1:{PORT}", autoraise=True)
-    os.chdir("../../../")
+        print(f"Assess 'http://127.0.0.1:{PORT}/' if a browser does not automatically open.")
+        Timer(1, open_browser, [PORT]).start()
+        with redirect_stderr(open(os.devnull, "w")):
+            httpd.serve_forever()
```

### Comparing `DAJIN2-0.1.9/src/DAJIN2.egg-info/SOURCES.txt` & `DAJIN2-0.2.0/src/DAJIN2.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,39 +3,46 @@
 README.md
 setup.py
 src/DAJIN2/DAJIN2.py
 src/DAJIN2/__init__.py
 src/DAJIN2/batch.py
 src/DAJIN2/gui.py
 src/DAJIN2/single.py
+src/DAJIN2/template_igvjs.html
 src/DAJIN2/view.py
 src/DAJIN2.egg-info/PKG-INFO
 src/DAJIN2.egg-info/SOURCES.txt
 src/DAJIN2.egg-info/dependency_links.txt
 src/DAJIN2.egg-info/entry_points.txt
 src/DAJIN2.egg-info/requires.txt
 src/DAJIN2.egg-info/top_level.txt
 src/DAJIN2/core/__init__.py
-src/DAJIN2/core/core.py
+src/DAJIN2/core/core_execute.py
 src/DAJIN2/core/classification/__init__.py
 src/DAJIN2/core/classification/classify.py
 src/DAJIN2/core/classification/detect_sv.py
 src/DAJIN2/core/clustering/__init__.py
-src/DAJIN2/core/clustering/clustering_main.py
-src/DAJIN2/core/clustering/make_scores.py
-src/DAJIN2/core/clustering/mask_control.py
+src/DAJIN2/core/clustering/clustering.py
+src/DAJIN2/core/clustering/make_score.py
+src/DAJIN2/core/clustering/merge_clusters.py
 src/DAJIN2/core/clustering/return_labels.py
-src/DAJIN2/core/clustering/screen_diffloci.py
 src/DAJIN2/core/consensus/__init__.py
-src/DAJIN2/core/consensus/consensus_main.py
+src/DAJIN2/core/consensus/consensus.py
+src/DAJIN2/core/consensus/subset.py
 src/DAJIN2/core/preprocess/__init__.py
-src/DAJIN2/core/preprocess/calc_midsv.py
-src/DAJIN2/core/preprocess/check_inputs.py
+src/DAJIN2/core/preprocess/call_midsv.py
+src/DAJIN2/core/preprocess/correct_knockin.py
+src/DAJIN2/core/preprocess/correct_sequence_error.py
+src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
+src/DAJIN2/core/preprocess/extract_knockin_loci.py
+src/DAJIN2/core/preprocess/extract_mutation_loci.py
 src/DAJIN2/core/preprocess/format_inputs.py
 src/DAJIN2/core/preprocess/mappy_align.py
+src/DAJIN2/core/preprocess/replace_NtoD.py
+src/DAJIN2/core/preprocess/validate_inputs.py
 src/DAJIN2/core/report/__init__.py
 src/DAJIN2/core/report/report_bam.py
 src/DAJIN2/core/report/report_files.py
 src/DAJIN2/postprocess/__init__.py
 src/DAJIN2/postprocess/report.py
 src/DAJIN2/static/css/style.css
 src/DAJIN2/templates/index.html
```

