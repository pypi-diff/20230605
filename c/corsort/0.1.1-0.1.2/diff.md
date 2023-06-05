# Comparing `tmp/corsort-0.1.1.tar.gz` & `tmp/corsort-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corsort-0.1.1.tar", last modified: Fri Apr  7 14:56:03 2023, max compression
+gzip compressed data, was "corsort-0.1.2.tar", last modified: Mon Jun  5 12:11:46 2023, max compression
```

## Comparing `corsort-0.1.1.tar` & `corsort-0.1.2.tar`

### file list

```diff
@@ -1,91 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:56:03.650547 corsort-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-07 14:55:50.000000 corsort-0.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-07 14:55:50.000000 corsort-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-07 14:55:50.000000 corsort-0.1.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-07 14:55:50.000000 corsort-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-07 14:55:50.000000 corsort-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-07 14:56:03.654547 corsort-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-07 14:55:50.000000 corsort-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:56:03.646547 corsort-0.1.1/corsort/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/chain_and_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/cor_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/cor_sort_borda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/cor_sort_delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/cor_sort_gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/cor_sort_gain_lexi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/distance_to_sorted_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/entropy_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/jit_scorers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/jit_sorts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/sort_asort_quickselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/sort_ford_johnson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/sort_largest_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/sort_merge_bfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/sort_merge_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/sort_quick.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/util_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/wrap_full_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-07 14:55:50.000000 corsort-0.1.1/corsort/wrap_sort_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:56:03.646547 corsort-0.1.1/corsort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-07 14:56:03.000000 corsort-0.1.1/corsort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-07 14:56:03.000000 corsort-0.1.1/corsort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 14:56:03.000000 corsort-0.1.1/corsort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 14:56:03.000000 corsort-0.1.1/corsort.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-07 14:56:03.000000 corsort-0.1.1/corsort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 14:56:03.000000 corsort-0.1.1/corsort.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:56:03.646547 corsort-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:56:03.646547 corsort-0.1.1/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/logo/logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:56:03.646547 corsort-0.1.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/notebooks/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:56:03.650547 corsort-0.1.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/chain_and_y.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/cor_sort.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/cor_sort_borda.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/cor_sort_delegate.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/cor_sort_gain.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/cor_sort_gain_lexi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/distance_to_sorted_array.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/entropy_bound.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/jit_scorers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/jit_sorts.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/merge.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/montecarlo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/partition.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/presets.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/print_order.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/sort.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/sort_asort_quickselect.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/sort_ford_johnson.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/sort_largest_interval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/sort_merge_bfs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/sort_merge_dfs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/sort_quick.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/wrap_full_jit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/reference/wrap_sort_scorer.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 14:55:50.000000 corsort-0.1.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-07 14:56:03.654547 corsort-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-07 14:55:50.000000 corsort-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:56:03.650547 corsort-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-07 14:55:50.000000 corsort-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-07 14:55:50.000000 corsort-0.1.1/tests/test_corsort.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-07 14:55:50.000000 corsort-0.1.1/tests/test_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-07 14:55:50.000000 corsort-0.1.1/tests/test_wrap_full_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-07 14:55:50.000000 corsort-0.1.1/tests/test_wrap_sort_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:11:46.053695 corsort-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-05 12:11:33.000000 corsort-0.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-05 12:11:33.000000 corsort-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-05 12:11:33.000000 corsort-0.1.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-05 12:11:33.000000 corsort-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-05 12:11:33.000000 corsort-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-05 12:11:46.053695 corsort-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-05 12:11:33.000000 corsort-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:11:46.045695 corsort-0.1.2/corsort/
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21385 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/chain_and_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/corsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/corsort_borda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/corsort_chain_decomposition_merge_v.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/corsort_chain_decomposition_merge_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/corsort_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/corsort_gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/corsort_gain_lexi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/distance_to_sorted_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/entropy_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/jit_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26359 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/jit_sorts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/multi_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/print_order_as_letters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/scorers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort_asort_quickselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort_binary_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort_ford_johnson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort_largest_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort_merge_bottom_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort_merge_top_down.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort_multizip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort_quick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/sort_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/split_pointer_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/transitive_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/util_chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/util_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/wrap_full_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-05 12:11:33.000000 corsort-0.1.2/corsort/wrap_sort_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:11:46.045695 corsort-0.1.2/corsort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-05 12:11:45.000000 corsort-0.1.2/corsort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-05 12:11:45.000000 corsort-0.1.2/corsort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:11:45.000000 corsort-0.1.2/corsort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:11:45.000000 corsort-0.1.2/corsort.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 12:11:45.000000 corsort-0.1.2/corsort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 12:11:45.000000 corsort-0.1.2/corsort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:11:46.045695 corsort-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:11:46.045695 corsort-0.1.2/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/logo/logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:11:46.045695 corsort-0.1.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/notebooks/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:11:46.053695 corsort-0.1.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/chain_and_y.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/corsort.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/corsort_borda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/corsort_chain_decomposition_merge_v.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/corsort_chain_decomposition_merge_x.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/corsort_delegate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/corsort_gain.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/corsort_gain_lexi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/distance_to_sorted_array.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/entropy_bound.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/jit_scorers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/jit_sorts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/merge.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/montecarlo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/multi_merge.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/partition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/presets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/print_order_as_letters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/scorers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort_asort_quickselect.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort_binary_insertion.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort_ford_johnson.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort_largest_interval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort_merge_bottom_up.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort_merge_top_down.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort_multizip.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort_quick.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/sort_shell.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/split_pointer_lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/util_chains.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/util_latex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/wrap_full_jit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/reference/wrap_sort_scorer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 12:11:33.000000 corsort-0.1.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-05 12:11:46.053695 corsort-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-05 12:11:33.000000 corsort-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:11:46.053695 corsort-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 12:11:33.000000 corsort-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-05 12:11:33.000000 corsort-0.1.2/tests/test_corsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 12:11:33.000000 corsort-0.1.2/tests/test_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 12:11:33.000000 corsort-0.1.2/tests/test_wrap_full_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-05 12:11:33.000000 corsort-0.1.2/tests/test_wrap_sort_scorer.py
```

### Comparing `corsort-0.1.1/CONTRIBUTING.rst` & `corsort-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/LICENSE` & `corsort-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/README.rst` & `corsort-0.1.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 .. image:: https://codecov.io/gh/emczg/corsort/branch/main/graphs/badge.svg
         :target: https://app.codecov.io/gh/emczg/corsort/tree/main/
         :alt: Code Coverage
 
 |
 
 .. image:: https://github.com/emczg/corsort/raw/main/docs/logo/logo.png
-    :alt: CorSort logo
+    :alt: Corsort logo
     :target: https://emczg.github.io/corsort/
 
 
 Comparison-Oriented Sort.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://emczg.github.io/corsort/.
 
 
 --------
 Features
 --------
 
-* Implement Corsort, an efficient anytime sorting algorithm.
-* Compare Corsort with classical algorithms through Monte-Carlo simulations.
+* Implement Corsort and Multizip sort, some efficient anytime sorting algorithms.
+* Compare them with classical algorithms through Monte-Carlo simulations.
 
 -------
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `francois-durand/package_helper_2`_ project template.
```

### Comparing `corsort-0.1.1/corsort/__init__.py` & `corsort-0.1.2/corsort/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 """Top-level package for Corsort."""
 
 __author__ = """Emma Caizergues"""
 __email__ = 'emma.caizergues@gmail.com'
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 
-from corsort.chain_and_y import ChainAndY, print_order
-from corsort.cor_sort import CorSort
-from corsort.cor_sort_borda import CorSortBorda
-from corsort.cor_sort_delegate import CorSortDelegate
-from corsort.cor_sort_gain import CorSortGain
-from corsort.cor_sort_gain_lexi import CorSortGainLexi
+from corsort.chain_and_y import ChainAndY, linear_extensions
+from corsort.corsort import Corsort
+from corsort.corsort_borda import CorsortBorda
+from corsort.corsort_chain_decomposition_merge_v import CorsortChainDecompositionMergeV
+from corsort.corsort_chain_decomposition_merge_x import CorsortChainDecompositionMergeX
+from corsort.corsort_delegate import CorsortDelegate
+from corsort.corsort_gain import CorsortGain
+from corsort.corsort_gain_lexi import CorsortGainLexi
 from corsort.distance_to_sorted_array import distance_to_sorted_array
 from corsort.entropy_bound import entropy_bound
-from corsort.jit_scorers import scorer_spaced, scorer_drift
-from corsort.jit_sorts import jit_corsort_borda, jit_corsort_drift_max_spaced, \
-    jit_corsort_drift_plus_spaced, jit_corsort_drift_max_drift, jit_corsort_drift_plus_drift, \
-    jit_corsort_spaced_max_spaced, jit_corsort_spaced_plus_spaced, jit_corsort_spaced_max_drift, \
-    jit_corsort_spaced_plus_drift, heapify, jit_heapsort
+from corsort.jit_scorers import jit_scorer_rho, jit_scorer_delta
+from corsort.jit_sorts import jit_corsort_borda, jit_corsort_delta_max_rho, \
+    jit_corsort_delta_sum_rho, jit_corsort_delta_max_delta, jit_corsort_delta_sum_delta, \
+    jit_corsort_rho_max_rho, jit_corsort_rho_sum_rho, jit_corsort_rho_max_delta, \
+    jit_corsort_rho_sum_delta, heapify, jit_heapsort
 from corsort.merge import merge
 from corsort.montecarlo import print_res, evaluate, evaluate_convergence, evaluate_comparisons
+from corsort.multi_merge import multi_merge
 from corsort.partition import partition
 from corsort.presets import colors, sorts, color_dict, auto_colors
+from corsort.print_order_as_letters import print_order_as_letters
+from corsort.scorers import scorer_delta, scorer_rho
 from corsort.sort import Sort
 from corsort.sort_asort_quickselect import SortAsortQuickselect
+from corsort.sort_binary_insertion import SortBinaryInsertion
 from corsort.sort_ford_johnson import SortFordJohnson
 from corsort.sort_largest_interval import SortLargestInterval
-from corsort.sort_merge_bfs import SortMergeBfs
-from corsort.sort_merge_dfs import SortMergeDfs
+from corsort.sort_merge_bottom_up import SortMergeBottomUp
+from corsort.sort_merge_top_down import SortMergeTopDown
+from corsort.sort_multizip import SortMultizip
 from corsort.sort_quick import SortQuick
+from corsort.sort_shell import SortShell
+from corsort.split_pointer_lists import split_pointer_lists
+from corsort.util_chains import longest_chain_starting_at, longest_chain, greedy_chain_decomposition
 from corsort.util_latex import print_corsort_execution
-from corsort.wrap_full_jit import WrapFullJit
+from corsort.wrap_full_jit import WrapFullJit, JitCorsortBorda, JitHeapsort, \
+    JitCorsortDeltaMaxDelta, JitCorsortDeltaMaxRho, JitCorsortDeltaSumDelta, JitCorsortDeltaSumRho, \
+    JitCorsortRhoMaxDelta, JitCorsortRhoMaxRho, JitCorsortRhoSumDelta, JitCorsortRhoSumRho
 from corsort.wrap_sort_scorer import WrapSortScorer
```

### Comparing `corsort-0.1.1/corsort/chain_and_y.py` & `corsort-0.1.2/corsort/chain_and_y.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,16 +500,16 @@
         Returns
         -------
         :class:`~numpy.ndarray`
             Estimated order of the nodes.
 
         Examples
         --------
-            >>> ChainAndY(2, 2, 1, 3).order_delta
-            array([2, 3, 0, 5, 1, 4, 6, 7])
+            >>> ChainAndY(2, 2, 1, 3).order_delta  # doctest: +ELLIPSIS
+            array([2, 3, 0, 5, 1, 4, 6, 7]...)
         """
         return np.argsort(self.delta)
 
     @property
     def order_rho(self):
         """
         Order of the nodes, according to estimator rho.
@@ -517,16 +517,16 @@
         Returns
         -------
         :class:`~numpy.ndarray`
             Estimated order of the nodes.
 
         Examples
         --------
-            >>> ChainAndY(2, 2, 1, 3).order_rho
-            array([2, 3, 0, 5, 1, 6, 4, 7])
+            >>> ChainAndY(2, 2, 1, 3).order_rho  # doctest: +ELLIPSIS
+            array([2, 3, 0, 5, 1, 6, 4, 7]...)
         """
         return np.argsort(self.rho)
 
     @property
     def order_average_height(self):
         """
         Order of the nodes, according to average height.
@@ -534,16 +534,16 @@
         Returns
         -------
         :class:`~numpy.ndarray`
             Estimated order of the nodes.
 
         Examples
         --------
-            >>> ChainAndY(2, 2, 1, 3).order_average_height
-            array([2, 3, 0, 5, 4, 6, 1, 7])
+            >>> ChainAndY(2, 2, 1, 3).order_average_height  # doctest: +ELLIPSIS
+            array([2, 3, 0, 5, 4, 6, 1, 7]...)
         """
         return np.argsort(self.average_height)
 
 
 def _average_height_c(a, b, c, d):
     """
     Average height for branch `c`.
@@ -629,28 +629,7 @@
         for places_x in combinations(range(x + y), x):
             extension = np.zeros(x + y, dtype=int)
             extension[np.array(places_x)] = chain_1
             mask_y = np.ones(x + y, dtype=bool)
             mask_y[np.array(places_x)] = False
             extension[mask_y] = chain_2
             yield extension
-
-
-def print_order(order):
-    """
-    Print a small list of integers as letters.
-
-    Parameters
-    ----------
-    order: :class:`list`
-        Size should be 26 at most.
-
-    Returns
-    -------
-    str
-
-    Examples
-    --------
-        >>> print_order([4, 2, 3, 1, 0])
-        (ecdba)
-    """
-    print("(" + "".join([string.ascii_lowercase[i] for i in order]) + ")")
```

### Comparing `corsort-0.1.1/corsort/cor_sort.py` & `corsort-0.1.2/corsort/corsort.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import numpy as np
 
 from corsort.distance_to_sorted_array import distance_to_sorted_array
 from corsort.sort import Sort
+from corsort.scorers import scorer_rho, scorer_delta
 
 
-class CorSort(Sort):
+class Corsort(Sort):
     """
-    CorSort.
+    Corsort.
 
     Parameters
     ----------
     compute_history: :class:`bool`
         If True, then compute the history of the distance to the sorted array.
+    record_leq: :class:`bool`
+        If True, then record all the states of the `leq_` matrix.
+    final_scorer: callable
+        Scorer used to compute the tentative estimate of the sorted list.
 
     Attributes
     ----------
     leq_: :class:`~numpy.ndarray`.
         Matrix of size `(n_, n_)`. Coefficient (i, j) is
         +1 if we know perm_[i] <= perm_[j],
         -1 if we know perm_[i] > perm_[j],
@@ -27,41 +32,42 @@
         words, the position estimates are the Borda scores.
 
     Notes
     -----
     Cf. also the attributes defined in the parent class :class:`~corsort.Sort`.
     """
 
-    def __init__(self, compute_history=False, record_leq=False):
+    def __init__(self, compute_history=False, record_leq=False, final_scorer=scorer_rho):
         super().__init__(compute_history=compute_history)
         self.record_leq = record_leq
+        self.final_scorer = final_scorer
         # Computed attributes
         self.leq_ = None
         self.position_estimates_ = None
         self.history_leq_ = None
 
     def update_position_estimates(self):
         """
         Update position estimate of each item.
 
         Examples
         --------
-            >>> corsort = CorSort()
+            >>> corsort = Corsort(final_scorer=scorer_delta)
             >>> corsort.n_ = 4
             >>> corsort.leq_ = np.array([
             ...     [ 1,  1,  1,  1],
             ...     [-1,  1, -1, -1],
             ...     [-1,  1,  1,  0],
             ...     [-1,  1,  0,  1],
             ... ])
             >>> corsort.update_position_estimates()
             >>> corsort.position_estimates_
-            array([0. , 3. , 1.5, 1.5])
+            array([-3,  3,  0,  0])
         """
-        self.position_estimates_ = (np.sum(self.leq_, axis=0) + self.n_) / 2 - 1
+        self.position_estimates_ = self.final_scorer(self.leq_)
 
     def distance_to_sorted_array(self):
         """
         Distance to sorted array.
 
         Returns
         -------
@@ -79,15 +85,15 @@
         i: :class:`int`
             Index of the small item.
         j: :class:`int`
             Index of the big item.
 
         Examples
         --------
-            >>> corsort = CorSort()
+            >>> corsort = Corsort()
             >>> corsort.n_ = 4
 
         Assume that we know perm[0] < perm[1], and perm[2] < perm[3]:
 
             >>> corsort.leq_ = np.array([
             ...     [ 1,  1,  0,  0],
             ...     [-1,  1,  0,  0],
@@ -141,15 +147,15 @@
         """
         raise NotImplementedError
 
     def _initialize_algo_aux(self):
         """
         Examples
         --------
-            >>> my_sort = CorSort(compute_history=True)
+            >>> my_sort = Corsort(compute_history=True)
             >>> my_sort._initialize_algo(perm=np.array(['b', 'a']))
             >>> my_sort.test_i_lt_j(0, 1)
             False
             >>> my_sort.n_comparisons_
             1
             >>> my_sort.history_distances_
             [1]
```

### Comparing `corsort-0.1.1/corsort/cor_sort_borda.py` & `corsort-0.1.2/corsort/corsort_borda.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import numpy as np
 from corsort.entropy_bound import entropy_bound
-from corsort.cor_sort import CorSort
+from corsort.corsort import Corsort
 
 
-class CorSortBorda(CorSort):
+class CorsortBorda(Corsort):
     """
-    CorSort based on the Borda score.
+    Corsort based on the Borda score.
 
     Examples
     --------
         >>> np.random.seed(22)
         >>> n = 15
         >>> perm = np.random.permutation(n)
-        >>> corsort = CorSortBorda(compute_history=True)
+        >>> corsort = CorsortBorda(compute_history=True)
         >>> corsort(perm).n_comparisons_
-        44
+        38
         >>> entropy_bound(n)  # doctest: +ELLIPSIS
         40.24212...
         >>> corsort.history_distances_ # doctest: +NORMALIZE_WHITESPACE
-        [55, 42, 51, 49, 49, 48, 40, 39, 33, 29, 29, 28, 28, 28, 28, 26, 26, 21, 20, 16, 14, 11, 10, 9, 8, 7,
-         8, 7, 6, 7, 7, 7, 7, 5, 5, 4, 4, 4, 3, 2, 3, 2, 1, 0, 0]
+        [55, 42, 51, 49, 49, 49, 43, 37, 36, 35, 34, 32, 32, 33, 26, 22, 17, 19, 20, 18, 13,
+        11, 11, 11, 11, 6, 6, 7, 9, 7, 5, 5, 4, 2, 2, 2, 1, 2, 1]
         >>> corsort.__name__
         'corsort_borda'
     """
 
     __name__ = 'corsort_borda'
 
     def next_compare(self):
```

### Comparing `corsort-0.1.1/corsort/cor_sort_delegate.py` & `corsort-0.1.2/corsort/corsort_delegate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import numpy as np
-from corsort.cor_sort import CorSort
+from corsort.corsort import Corsort
 from corsort.sort_quick import SortQuick
+from corsort.scorers import scorer_delta
 
 
-class CorSortDelegate(CorSort):
+class CorsortDelegate(Corsort):
     """
-    CorSort that delegates the choice of pairwise comparisons to another sorting algorithm.
+    Corsort that delegates the choice of pairwise comparisons to another sorting algorithm.
 
     Parameters
     ----------
     sort: Sort
         A sorting algorithm.
 
     Examples
     --------
-        >>> corsort = CorSortDelegate(SortQuick(), compute_history=True)
+        >>> corsort = CorsortDelegate(SortQuick(), compute_history=True)
         >>> corsort(np.array(['e', 'b', 'a', 'c', 'd'])).n_comparisons_
         8
         >>> corsort.history_comparisons_
         [(1, 0), (2, 0), (3, 0), (4, 0), (2, 1), (1, 3), (1, 4), (3, 4)]
         >>> corsort.history_distances_
         [5, 1, 1, 1, 1, 2, 1, 0, 0]
         >>> corsort.__name__
         'corsort_delegate_quicksort'
     """
 
-    def __init__(self, sort, compute_history=False, record_leq=False):
-        super().__init__(compute_history=compute_history, record_leq=record_leq)
+    def __init__(self, sort, compute_history=False, record_leq=False, final_scorer=scorer_delta):
+        super().__init__(compute_history=compute_history, record_leq=record_leq, final_scorer=final_scorer)
         self.sort = sort
         self.__name__ = "corsort_delegate_" + self.sort.__name__
 
     def next_compare(self):
         self.sort(self.perm_)
         return self.sort.history_comparisons_
```

### Comparing `corsort-0.1.1/corsort/cor_sort_gain.py` & `corsort-0.1.2/corsort/corsort_gain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from corsort.cor_sort import CorSort
+from corsort.corsort import Corsort
 
 
-class CorSortGain(CorSort):
+class CorsortGain(Corsort):
     """
-    CorSort based on a `gain` function.
+    Corsort based on a `gain` function.
     """
 
     def gain(self, i, j):
         """
         Gain to be expected when comparing perm[i] and perm[j].
 
         Notes
```

### Comparing `corsort-0.1.1/corsort/cor_sort_gain_lexi.py` & `corsort-0.1.2/corsort/corsort_gain_lexi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import numpy as np
 from corsort.entropy_bound import entropy_bound
-from corsort.cor_sort_gain import CorSortGain
+from corsort.corsort_gain import CorsortGain
 
 
-class CorSortGainLexi(CorSortGain):
+class CorsortGainLexi(CorsortGain):
     """
-    CorSort with lexicographic gain (information gain, difference of position estimates).
+    Corsort with lexicographic gain (information gain, difference of position estimates).
 
     Examples
     --------
         >>> np.random.seed(22)
         >>> n_ = 15
         >>> p = np.random.permutation(n_)
-        >>> corsort = CorSortGainLexi(compute_history=True)
+        >>> corsort = CorsortGainLexi(compute_history=True)
         >>> corsort(p).n_comparisons_
         39
         >>> entropy_bound(n_) # doctest: +ELLIPSIS
         40.24212...
         >>> corsort.history_distances_ # doctest: +NORMALIZE_WHITESPACE
-        [55, 42, 51, 49, 49, 43, 39, 38, 37, 36, 28, 27, 22, 21, 20, 19, 13, 14, 13, 15,
-        12, 13, 13, 11, 10, 6, 5, 5, 4, 2, 2, 1, 2, 2, 2, 1, 2, 1, 1, 0]
+        [55, 42, 51, 49, 49, 43, 39, 38, 37, 36, 28, 27, 22, 21, 20, 19, 13, 14, 13, 13, 13, 14, 13, 11,
+        10, 6, 6, 5, 5, 3, 2, 1, 2, 2, 2, 1, 1, 1, 1, 0]
         >>> corsort.__name__
         'corsort_lexi'
     """
 
     __name__ = 'corsort_lexi'
 
     def gain_i_lt_j(self, i, j):
```

### Comparing `corsort-0.1.1/corsort/distance_to_sorted_array.py` & `corsort-0.1.2/corsort/distance_to_sorted_array.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/corsort/entropy_bound.py` & `corsort-0.1.2/corsort/entropy_bound.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/corsort/jit_scorers.py` & `corsort-0.1.2/corsort/jit_scorers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from numba import njit
 import numpy as np
 
 
 @njit
-def scorer_spaced(n, downs, ups):
+def jit_scorer_rho(n, downs, ups):
     """
     Estimates scores of nodes by dividing the number of the descendants by the size of the family plus one.
     The rational is to consider that the family should be in average evenly spaced in the sorted result.
 
     Parameters
     ----------
     n: :class:`int`
@@ -25,15 +25,15 @@
 
     Examples
     --------
 
     >>> my_n = 5
     >>> my_downs = np.array([0, 1, 2])
     >>> my_ups = np.array([2, 2, 3])
-    >>> scorer_spaced(my_n, my_downs, my_ups)
+    >>> jit_scorer_rho(my_n, my_downs, my_ups)
     array([[0.5       , 0.5       , 0.5       , 0.5       , 0.5       ],
            [0.33333333, 0.5       , 0.66666667, 0.5       , 0.5       ],
            [0.33333333, 0.33333333, 0.75      , 0.5       , 0.5       ],
            [0.25      , 0.25      , 0.6       , 0.8       , 0.5       ]])
     """
     ncp = len(ups) + 1
     leq = np.eye(n, dtype=np.int8)
@@ -53,15 +53,15 @@
                         tot[jj] += 1
                         down[jj] += 1
         res[(k + 1), :] = down / tot
     return res
 
 
 @njit
-def scorer_drift(n, downs, ups):
+def jit_scorer_delta(n, downs, ups):
     """
     Estimates scores of nodes by the difference between the numbers of descendants and ascendants.
     The rational is to consider that an item should be in average halfway between
     its highest and lowest possible values.
 
     Parameters
     ----------
@@ -80,15 +80,15 @@
 
     Examples
     --------
 
     >>> my_n = 5
     >>> my_downs = np.array([0, 1, 2])
     >>> my_ups = np.array([2, 2, 3])
-    >>> scorer_drift(my_n, my_downs, my_ups)
+    >>> jit_scorer_delta(my_n, my_downs, my_ups)
     array([[ 0,  0,  0,  0,  0],
            [-1,  0,  1,  0,  0],
            [-1, -1,  2,  0,  0],
            [-2, -2,  1,  3,  0]])
     """
     ncp = len(ups) + 1
     leq = np.eye(n, dtype=np.int8)
```

### Comparing `corsort-0.1.1/corsort/jit_sorts.py` & `corsort-0.1.2/corsort/jit_sorts.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,17 +84,17 @@
                         pos[jj] += 1
         scores.append(pos.copy())
         states.append(perm[np.argsort(pos)])
     return states, scores, comparisons
 
 
 @njit
-def jit_corsort_drift_max_spaced(perm):
+def jit_corsort_delta_max_rho(perm):
     """
-    Corsort with drift core scorer, max-knowledge tie-break, and spaced outpus scorer.
+    Corsort with delta core scorer, max-knowledge tie-break, and rho output scorer.
     Currently, the best corsort for trajectory.
 
     Parameters
     ----------
     perm: :class:`~numpy.ndarray`
         A random permutation.
 
@@ -108,15 +108,15 @@
         List of performed comparison. Each element is a tuple (index of lower item, index of higher item).
 
     Examples
     --------
 
     >>> np.random.seed(42)
     >>> p = np.random.permutation(10)
-    >>> st, sc, co = jit_corsort_drift_max_spaced(p)
+    >>> st, sc, co = jit_corsort_delta_max_rho(p)
     >>> st[0]
     array([8, 1, 5, 0, 7, 2, 9, 4, 3, 6])
     >>> st[10]
     array([0, 1, 2, 4, 3, 6, 5, 7, 8, 9])
     >>> st[-1]
     array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     >>> p[:5]
@@ -173,17 +173,17 @@
         score = down/info
         scores.append(score)
         states.append(perm[np.argsort(score)])
     return states, scores, comparisons
 
 
 @njit
-def jit_corsort_drift_plus_spaced(perm):
+def jit_corsort_delta_sum_rho(perm):
     """
-    Corsort with drift core scorer, plus-knowledge tie-break, and spaced outpus scorer.
+    Corsort with delta core scorer, sum-knowledge tie-break, and rho output scorer.
 
     Parameters
     ----------
     perm: :class:`~numpy.ndarray`
         A random permutation.
 
     Returns
@@ -196,15 +196,15 @@
         List of performed comparison. Each element is a tuple (index of lower item, index of higher item).
 
     Examples
     --------
 
     >>> np.random.seed(42)
     >>> p = np.random.permutation(10)
-    >>> st, sc, co = jit_corsort_drift_plus_spaced(p)
+    >>> st, sc, co = jit_corsort_delta_sum_rho(p)
     >>> st[0]
     array([8, 1, 5, 0, 7, 2, 9, 4, 3, 6])
     >>> st[10]
     array([0, 1, 2, 4, 3, 6, 5, 7, 8, 9])
     >>> st[-1]
     array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     >>> p[:5]
@@ -261,17 +261,17 @@
         score = down/info
         scores.append(score)
         states.append(perm[np.argsort(score)])
     return states, scores, comparisons
 
 
 @njit
-def jit_corsort_drift_max_drift(perm):
+def jit_corsort_delta_max_delta(perm):
     """
-    Corsort with drift core scorer, max-knowledge tie-break, and drift outpus scorer.
+    Corsort with delta core scorer, max-knowledge tie-break, and delta output scorer.
 
     Parameters
     ----------
     perm: :class:`~numpy.ndarray`
         A random permutation.
 
     Returns
@@ -284,15 +284,15 @@
         List of performed comparison. Each element is a tuple (index of lower item, index of higher item).
 
     Examples
     --------
 
     >>> np.random.seed(42)
     >>> p = np.random.permutation(10)
-    >>> st, sc, co = jit_corsort_drift_max_drift(p)
+    >>> st, sc, co = jit_corsort_delta_max_delta(p)
     >>> st[0]
     array([8, 1, 5, 0, 7, 2, 9, 4, 3, 6])
     >>> st[10]
     array([0, 1, 2, 4, 3, 6, 5, 7, 8, 9])
     >>> st[-1]
     array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     >>> p[:5]
@@ -347,17 +347,17 @@
         score = pos.copy()
         scores.append(score)
         states.append(perm[np.argsort(score)])
     return states, scores, comparisons
 
 
 @njit
-def jit_corsort_drift_plus_drift(perm):
+def jit_corsort_delta_sum_delta(perm):
     """
-    Corsort with drift core scorer, plus-knowledge tie-break, and drift outpus scorer.
+    Corsort with delta core scorer, sum-knowledge tie-break, and delta output scorer.
 
     Parameters
     ----------
     perm: :class:`~numpy.ndarray`
         A random permutation.
 
     Returns
@@ -370,15 +370,15 @@
         List of performed comparison. Each element is a tuple (index of lower item, index of higher item).
 
     Examples
     --------
 
     >>> np.random.seed(42)
     >>> p = np.random.permutation(10)
-    >>> st, sc, co = jit_corsort_drift_plus_drift(p)
+    >>> st, sc, co = jit_corsort_delta_sum_delta(p)
     >>> st[0]
     array([8, 1, 5, 0, 7, 2, 9, 4, 3, 6])
     >>> st[10]
     array([0, 1, 2, 4, 3, 6, 5, 7, 8, 9])
     >>> st[-1]
     array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     >>> p[:5]
@@ -433,17 +433,17 @@
         score = pos.copy()
         scores.append(score)
         states.append(perm[np.argsort(score)])
     return states, scores, comparisons
 
 
 @njit
-def jit_corsort_spaced_max_spaced(perm):
+def jit_corsort_rho_max_rho(perm):
     """
-    Corsort with spaced core scorer, max-knowledge tie-break, and spaced outpus scorer.
+    Corsort with rho core scorer, max-knowledge tie-break, and rho output scorer.
 
     Parameters
     ----------
     perm: :class:`~numpy.ndarray`
         A random permutation.
 
     Returns
@@ -456,15 +456,15 @@
         List of performed comparison. Each element is a tuple (index of lower item, index of higher item).
 
     Examples
     --------
 
     >>> np.random.seed(42)
     >>> p = np.random.permutation(10)
-    >>> st, sc, co = jit_corsort_spaced_max_spaced(p)
+    >>> st, sc, co = jit_corsort_rho_max_rho(p)
     >>> st[0]
     array([8, 1, 5, 0, 7, 2, 9, 4, 3, 6])
     >>> st[10]
     array([0, 1, 2, 4, 3, 6, 5, 7, 8, 9])
     >>> st[-1]
     array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     >>> p[:5]
@@ -518,17 +518,17 @@
         score = down/info
         scores.append(score)
         states.append(perm[np.argsort(score)])
     return states, scores, comparisons
 
 
 @njit
-def jit_corsort_spaced_plus_spaced(perm):
+def jit_corsort_rho_sum_rho(perm):
     """
-    Corsort with spaced core scorer, plus-knowledge tie-break, and spaced outpus scorer.
+    Corsort with rho core scorer, sum-knowledge tie-break, and rho output scorer.
 
     Parameters
     ----------
     perm: :class:`~numpy.ndarray`
         A random permutation.
 
     Returns
@@ -541,15 +541,15 @@
         List of performed comparison. Each element is a tuple (index of lower item, index of higher item).
 
     Examples
     --------
 
     >>> np.random.seed(42)
     >>> p = np.random.permutation(10)
-    >>> st, sc, co = jit_corsort_spaced_plus_spaced(p)
+    >>> st, sc, co = jit_corsort_rho_sum_rho(p)
     >>> st[0]
     array([8, 1, 5, 0, 7, 2, 9, 4, 3, 6])
     >>> st[10]
     array([0, 1, 2, 4, 3, 6, 5, 7, 8, 9])
     >>> st[-1]
     array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     >>> p[:5]
@@ -603,17 +603,17 @@
         score = down/info
         scores.append(score)
         states.append(perm[np.argsort(score)])
     return states, scores, comparisons
 
 
 @njit
-def jit_corsort_spaced_max_drift(perm):
+def jit_corsort_rho_max_delta(perm):
     """
-    Corsort with spaced core scorer, max-knowledge tie-break, and drift outpus scorer.
+    Corsort with rho core scorer, max-knowledge tie-break, and delta output scorer.
 
     Parameters
     ----------
     perm: :class:`~numpy.ndarray`
         A random permutation.
 
     Returns
@@ -626,15 +626,15 @@
         List of performed comparison. Each element is a tuple (index of lower item, index of higher item).
 
     Examples
     --------
 
     >>> np.random.seed(42)
     >>> p = np.random.permutation(10)
-    >>> st, sc, co = jit_corsort_spaced_max_drift(p)
+    >>> st, sc, co = jit_corsort_rho_max_delta(p)
     >>> st[0]
     array([8, 1, 5, 0, 7, 2, 9, 4, 3, 6])
     >>> st[10]
     array([0, 1, 2, 4, 3, 6, 5, 7, 8, 9])
     >>> st[-1]
     array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     >>> p[:5]
@@ -693,17 +693,17 @@
         score = pos.copy()
         scores.append(score)
         states.append(perm[np.argsort(score)])
     return states, scores, comparisons
 
 
 @njit
-def jit_corsort_spaced_plus_drift(perm):
+def jit_corsort_rho_sum_delta(perm):
     """
-    Corsort with spaced core scorer, plus-knowledge tie-break, and drift outpus scorer.
+    Corsort with rho core scorer, sum-knowledge tie-break, and delta output scorer.
 
     Parameters
     ----------
     perm: :class:`~numpy.ndarray`
         A random permutation.
 
     Returns
@@ -716,15 +716,15 @@
         List of performed comparison. Each element is a tuple (index of lower item, index of higher item).
 
     Examples
     --------
 
     >>> np.random.seed(42)
     >>> p = np.random.permutation(10)
-    >>> st, sc, co = jit_corsort_spaced_plus_drift(p)
+    >>> st, sc, co = jit_corsort_rho_sum_delta(p)
     >>> st[0]
     array([8, 1, 5, 0, 7, 2, 9, 4, 3, 6])
     >>> st[10]
     array([0, 1, 2, 4, 3, 6, 5, 7, 8, 9])
     >>> st[-1]
     array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     >>> p[:5]
```

### Comparing `corsort-0.1.1/corsort/merge.py` & `corsort-0.1.2/corsort/merge.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/corsort/montecarlo.py` & `corsort-0.1.2/corsort/montecarlo.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,17 +222,16 @@
     """
     res = defaultdict(dict)
     for n in n_list:
         for sort in sort_list:
             print(f"Evaluate comparisons of {sort.__name__} for n = {n}")
             convergence_times = np.zeros(nt, dtype=int)
             if pool is not None:
-                for k, instant in enumerate(pool.imap_unordered(sort,
-                                                          tqdm([np.random.permutation(n)
-                                                                for _ in range(nt)]))):
+                for k, instant in enumerate(pool.imap_unordered(sort, tqdm([np.random.permutation(n)
+                                                                            for _ in range(nt)]))):
                     convergence_times[k] = instant.n_comparisons_
             else:
                 for k in tqdm(range(nt)):
                     sort(np.random.permutation(n))
                     convergence_times[k] = sort.n_comparisons_
             res[sort.__name__][n] = convergence_times
     return res
```

### Comparing `corsort-0.1.1/corsort/partition.py` & `corsort-0.1.2/corsort/partition.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/corsort/presets.py` & `corsort-0.1.2/corsort/presets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from matplotlib import pylab as plt
 
 colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
 
-sorts = ['corsort_drift_max_spaced', 'mergesort_bfs', 'ford_johnson_spaced',
-         'mergesort_dfs_spaced', 'mergesort_dfs', 'mergesort_bfs_spaced',
+sorts = ['corsort_delta_max_rho', 'mergesort_bottom_up', 'ford_johnson_rho',
+         'mergesort_top_down_rho', 'mergesort_top_down', 'mergesort_bottom_up_rho',
          'quicksort', 'heapsort']
 
 color_dict = {k: v for k, v in zip(sorts, colors)}
-color_dict['ford_johnson'] = color_dict['ford_johnson_spaced']
+color_dict['ford_johnson'] = color_dict['ford_johnson_rho']
 
 
 def auto_colors(sort_list):
     """
     Maps a list of sorts to standard pyplot colors.
 
     Parameters
@@ -22,15 +22,16 @@
     -------
     :class:`dict`
 
     Examples
     --------
 
     >>> from corsort.sort_ford_johnson import SortFordJohnson
-    >>> from corsort.sort_merge_bfs import SortMergeBfs
-    >>> from corsort.sort_merge_dfs import SortMergeDfs
+    >>> from corsort.sort_merge_bottom_up import SortMergeBottomUp
+    >>> from corsort.sort_merge_top_down import SortMergeTopDown
     >>> from corsort.sort_quick import SortQuick
-    >>> s_list = [SortFordJohnson(), SortQuick, SortMergeBfs(), SortMergeDfs]
-    >>> auto_colors(s_list)
-    {'ford_johnson': '#1f77b4', 'SortQuick': '#ff7f0e', 'mergesort_bfs': '#2ca02c', 'SortMergeDfs': '#d62728'}
+    >>> s_list = [SortFordJohnson(), SortQuick(), SortMergeBottomUp(), SortMergeTopDown()]
+    >>> auto_colors(s_list)  # doctest: +NORMALIZE_WHITESPACE
+    {'ford_johnson': '#1f77b4', 'quicksort': '#ff7f0e', 'mergesort_bottom_up': '#2ca02c',
+    'mergesort_top_down': '#d62728'}
     """
     return {k.__name__: v for k, v in zip(sort_list, colors)}
```

### Comparing `corsort-0.1.1/corsort/sort.py` & `corsort-0.1.2/corsort/sort.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/corsort/sort_asort_quickselect.py` & `corsort-0.1.2/corsort/sort_asort_quickselect.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/corsort/sort_ford_johnson.py` & `corsort-0.1.2/corsort/sort_ford_johnson.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/corsort/sort_largest_interval.py` & `corsort-0.1.2/corsort/sort_largest_interval.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/corsort/sort_merge_dfs.py` & `corsort-0.1.2/corsort/sort_merge_top_down.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 import numpy as np
 from corsort.sort import Sort
 from corsort.distance_to_sorted_array import distance_to_sorted_array
 from corsort.merge import merge
 
 
-class SortMergeDfs(Sort):
+class SortMergeTopDown(Sort):
     """
-    Merge sort, DFS version (i.e. "natural" recursive version).
+    Merge sort, top-down version (DFS, i.e. "natural" recursive version).
 
     Examples
     --------
-        >>> merge_sort = SortMergeDfs(compute_history=True)
+        >>> merge_sort = SortMergeTopDown(compute_history=True)
         >>> my_xs = np.array([4, 1, 7, 6, 0, 8, 2, 3, 5])
         >>> merge_sort(my_xs).n_comparisons_
         19
         >>> merge_sort.history_comparisons_  # doctest: +NORMALIZE_WHITESPACE
         [(1, 0), (3, 2), (1, 3), (0, 3), (4, 5), (7, 8), (6, 7), (4, 6), (6, 5), (7, 5),
         (8, 5), (4, 1), (1, 6), (6, 0), (7, 0), (0, 8), (8, 3), (3, 5), (2, 5)]
         >>> merge_sort.history_distances_
         [17, 16, 15, 15, 15, 15, 15, 15, 15, 14, 13, 12, 8, 8, 5, 2, 2, 0, 0, 0]
         >>> merge_sort.sorted_list_
         array([0, 1, 2, 3, 4, 5, 6, 7, 8])
     """
 
-    __name__ = 'mergesort_dfs'
+    __name__ = 'mergesort_top_down'
 
     def __init__(self, compute_history=False):
         super().__init__(compute_history=compute_history)
         self.sorted_indices_ = None
 
     def _initialize_algo_aux(self):
         self.sorted_indices_ = np.arange(self.n_)
 
     def _call_aux(self):
-        _merge_sort_dfs(self.sorted_indices_, lt=self.test_i_lt_j)
+        _merge_sort_top_down(self.sorted_indices_, lt=self.test_i_lt_j)
 
     def distance_to_sorted_array(self):
         return distance_to_sorted_array(self.perm_[self.sorted_indices_])
 
     @property
     def sorted_list_(self):
         return self.perm_[self.sorted_indices_]
 
 
-def _merge_sort_dfs(collection, lt=None, i=0, j=None):
+def _merge_sort_top_down(collection, lt=None, i=0, j=None):
     """
-    Merge sort (DFS).
+    Merge sort, top-down (DFS).
 
     Parameters
     ----------
     collection: class: `list`
         A list to sort.
     lt: class: `function`
         A function that takes two elements x and y return the boolean x < y.
@@ -57,34 +57,34 @@
         Index of the left boundary.
     j: :class:`int`
         Index of the right boundary.
 
     Examples
     --------
         >>> my_xs = [7, 3, 2, 1, 4, 6, 0, 5]
-        >>> _merge_sort_dfs(my_xs)
+        >>> _merge_sort_top_down(my_xs)
         >>> my_xs
         [0, 1, 2, 3, 4, 5, 6, 7]
 
         >>> my_xs = [4, 1, 7, 6, 0, 8, 2, 3, 5]
-        >>> _merge_sort_dfs(my_xs)
+        >>> _merge_sort_top_down(my_xs)
         >>> my_xs
         [0, 1, 2, 3, 4, 5, 6, 7, 8]
 
         >>> my_xs = np.array([4, 1, 7, 6, 0, 8, 2, 3, 5])
         >>> indices = np.arange(9)
         >>> def my_lt(my_i, my_j):
         ...     return my_xs[my_i] < my_xs[my_j]
-        >>> _merge_sort_dfs(indices, my_lt)
+        >>> _merge_sort_top_down(indices, my_lt)
         >>> my_xs[indices]
         array([0, 1, 2, 3, 4, 5, 6, 7, 8])
     """
     if lt is None:
         def lt(x, y):
             return x < y
     if j is None:
         j = len(collection)
     if j - i > 1:
         middle = (i + j) // 2
-        _merge_sort_dfs(collection, lt, i, middle)
-        _merge_sort_dfs(collection, lt, middle, j)
+        _merge_sort_top_down(collection, lt, i, middle)
+        _merge_sort_top_down(collection, lt, middle, j)
         merge(collection, i, middle, j, lt=lt)
```

### Comparing `corsort-0.1.1/corsort/sort_quick.py` & `corsort-0.1.2/corsort/sort_quick.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/corsort/util_latex.py` & `corsort-0.1.2/corsort/util_latex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,27 @@
-import numpy as np
 from string import Template
-from itertools import permutations
-from corsort.cor_sort_delegate import CorSortDelegate
+from corsort.corsort_delegate import CorsortDelegate
 from corsort.wrap_full_jit import WrapFullJit
-from corsort.jit_sorts import jit_corsort_drift_max_spaced
+from corsort.jit_sorts import jit_corsort_delta_max_rho
+from corsort.transitive_reduction import transitive_reduction
 
 
-def print_legend(k, state, distance):
+def _print_legend(k, state, distance):
     if k == 0:
         positioning = ""
     elif k % 2 == 1:
         positioning = Template(r", right = \lrgap of x$ref").safe_substitute(ref=k-1)
     else:
         positioning = Template(r", below = \interspace of x$ref").safe_substitute(ref=k-2)
     state_as_str = "".join([str(element) for element in state])
     print(Template(r"\node[draw$positioning] (x$k) {$X_$k=($state_as_str), \tau_$k=$distance$};").safe_substitute(
         positioning=positioning, k=k, distance=distance, state_as_str=state_as_str))
 
 
-def transitive_reduction(leq):
-    mask_keep = (leq == 1)
-    comparisons = [(i, j) for i, j in zip(*np.where(leq == 1)) if i != j]
-    for (i, j), (k, l) in permutations(comparisons, 2):
-        if j == k:
-            mask_keep[i, l] = False
-    comparisons = [(i, j) for i, j in zip(*np.where(mask_keep)) if i != j]
-    return comparisons
-
-
-def print_graph(k, leq, history_comparisons, state, perm):
+def _print_graph(k, leq, history_comparisons, state, perm):
     print(Template(r"\node[above = \intraspace of x$k] (x${k}p) {\execution{").safe_substitute(k=k))
     n_ancestors = (leq > 0).sum(axis=1)
     n_descendants = (leq > 0).sum(axis=0)
     next_comparison = history_comparisons[k] if k < len(history_comparisons) else {}
     rows = []
     for i, x in enumerate(state):
         n_anc = n_ancestors[i]
@@ -43,15 +32,15 @@
         ))
     print(", \n".join(rows) + "%")
     comparisons = transitive_reduction(leq)
     comparisons_as_str = ", ".join([f"{perm[i]}/{perm[j]}" for i, j in comparisons])
     print(Template(r"}{$comparisons_as_str}};").safe_substitute(comparisons_as_str=comparisons_as_str))
 
 
-def print_preamble():
+def _print_preamble():
     print(r"""
 \begin{tikzpicture}
 \def\interspace{3cm}
 \def\intraspace{.1cm}
 \def\lrgap{1.5cm}
 \newcommand{\execution}[2]{%
     \begin{tikzpicture}[scale=.7, transform shape]
@@ -62,15 +51,15 @@
         }
         \foreach \i/\j in {#2}{\draw[<-] (\i) -- (\j) ;}
     \end{tikzpicture}%
 }
     """)
 
 
-def print_end():
+def _print_end():
     print(r"\end{tikzpicture}")
 
 
 def print_corsort_execution(perm):
     r"""
     Print an execution of corsort in LaTeX.
 
@@ -162,20 +151,27 @@
             2/-2/2/6/,
             3/0/3/6/,
             1/-4/1/6/,
             5/4/5/6/%
         }{4/5, 2/3, 3/4, 1/2}};
         \end{tikzpicture}
     """
-    corsort = CorSortDelegate(
-        sort=WrapFullJit(jit_sort=jit_corsort_drift_max_spaced),
+    corsort = CorsortDelegate(
+        sort=WrapFullJit(jit_sort=jit_corsort_delta_max_rho, record_states=True),
         compute_history=True,
         record_leq=True
     )
     corsort(perm)
-    print_preamble()
+    _print_preamble()
+    # raise ValueError(str(corsort.sort.record_states))
+    # if corsort.sort.history_states_ is None:
+    #     raise ValueError("A")
+    # if corsort.history_distances_ is None:
+    #     raise ValueError("B")
+    # if corsort.history_leq_ is None:
+    #     raise ValueError("C")
     for k, (state, distance, leq) in enumerate(zip(corsort.sort.history_states_,
                                                    corsort.history_distances_,
                                                    corsort.history_leq_)):
-        print_legend(k, state, distance)
-        print_graph(k, leq, corsort.history_comparisons_, state, perm)
-    print_end()
+        _print_legend(k, state, distance)
+        _print_graph(k, leq, corsort.history_comparisons_, state, perm)
+    _print_end()
```

### Comparing `corsort-0.1.1/corsort/wrap_sort_scorer.py` & `corsort-0.1.2/corsort/wrap_sort_scorer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 from corsort.distance_to_sorted_array import distance_to_sorted_array
 from corsort.sort_quick import SortQuick
-from corsort.jit_scorers import scorer_spaced
+from corsort.jit_scorers import jit_scorer_rho
 
 
 class WrapSortScorer:
     """
     Examples
     --------
         >>> my_sort = SortQuick(compute_history=False)
-        >>> jit_sort = WrapSortScorer(scorer=scorer_spaced, sort=my_sort, compute_history=False)
+        >>> jit_sort = WrapSortScorer(scorer=jit_scorer_rho, sort=my_sort, compute_history=False)
         >>> my_xs = np.array([4, 1, 7, 6, 0, 8, 2, 3, 5])
         >>> jit_sort(my_xs).n_comparisons_
         16
         >>> jit_sort.__name__
-        'quicksort_spaced'
+        'quicksort_rho'
         >>> jit_sort.history_comparisons_  # doctest: +NORMALIZE_WHITESPACE
         [(1, 0), (0, 2), (0, 3), (4, 0), (0, 5), (6, 0), (7, 0), (0, 8),
         (4, 1), (1, 6), (1, 7), (6, 7), (3, 2), (2, 5), (8, 2), (8, 3)]
         >>> jit_sort.history_comparisons_values_  # doctest: +NORMALIZE_WHITESPACE
         [(1, 4), (4, 7), (4, 6), (0, 4), (4, 8), (2, 4), (3, 4), (4, 5),
         (0, 1), (1, 2), (1, 3), (2, 3), (6, 7), (7, 8), (5, 7), (5, 6)]
     """
@@ -26,15 +26,15 @@
     def __init__(self, scorer, sort, compute_history=False):
         """
         Examples
         --------
         Before using the algorithm, `history_comparisons_values_` is None:
 
             >>> my_sort = SortQuick()
-            >>> jit_sort = WrapSortScorer(scorer=scorer_spaced, sort=my_sort)
+            >>> jit_sort = WrapSortScorer(scorer=jit_scorer_rho, sort=my_sort)
             >>> print(jit_sort.history_comparisons_values_)
             None
         """
         # Parameters
         self.scorer = scorer
         self.sort = sort
         self.compute_history = compute_history
```

### Comparing `corsort-0.1.1/corsort.egg-info/SOURCES.txt` & `corsort-0.1.2/corsort.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,34 +4,45 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 corsort/__init__.py
 corsort/chain_and_y.py
-corsort/cor_sort.py
-corsort/cor_sort_borda.py
-corsort/cor_sort_delegate.py
-corsort/cor_sort_gain.py
-corsort/cor_sort_gain_lexi.py
+corsort/corsort.py
+corsort/corsort_borda.py
+corsort/corsort_chain_decomposition_merge_v.py
+corsort/corsort_chain_decomposition_merge_x.py
+corsort/corsort_delegate.py
+corsort/corsort_gain.py
+corsort/corsort_gain_lexi.py
 corsort/distance_to_sorted_array.py
 corsort/entropy_bound.py
 corsort/jit_scorers.py
 corsort/jit_sorts.py
 corsort/merge.py
 corsort/montecarlo.py
+corsort/multi_merge.py
 corsort/partition.py
 corsort/presets.py
+corsort/print_order_as_letters.py
+corsort/scorers.py
 corsort/sort.py
 corsort/sort_asort_quickselect.py
+corsort/sort_binary_insertion.py
 corsort/sort_ford_johnson.py
 corsort/sort_largest_interval.py
-corsort/sort_merge_bfs.py
-corsort/sort_merge_dfs.py
+corsort/sort_merge_bottom_up.py
+corsort/sort_merge_top_down.py
+corsort/sort_multizip.py
 corsort/sort_quick.py
+corsort/sort_shell.py
+corsort/split_pointer_lists.py
+corsort/transitive_reduction.py
+corsort/util_chains.py
 corsort/util_latex.py
 corsort/wrap_full_jit.py
 corsort/wrap_sort_scorer.py
 corsort.egg-info/PKG-INFO
 corsort.egg-info/SOURCES.txt
 corsort.egg-info/dependency_links.txt
 corsort.egg-info/not-zip-safe
@@ -47,36 +58,46 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 docs/logo/logo.png
 docs/logo/logo_small.png
 docs/notebooks/index.rst
 docs/reference/chain_and_y.rst
-docs/reference/cor_sort.rst
-docs/reference/cor_sort_borda.rst
-docs/reference/cor_sort_delegate.rst
-docs/reference/cor_sort_gain.rst
-docs/reference/cor_sort_gain_lexi.rst
+docs/reference/corsort.rst
+docs/reference/corsort_borda.rst
+docs/reference/corsort_chain_decomposition_merge_v.rst
+docs/reference/corsort_chain_decomposition_merge_x.rst
+docs/reference/corsort_delegate.rst
+docs/reference/corsort_gain.rst
+docs/reference/corsort_gain_lexi.rst
 docs/reference/distance_to_sorted_array.rst
 docs/reference/entropy_bound.rst
 docs/reference/index.rst
 docs/reference/jit_scorers.rst
 docs/reference/jit_sorts.rst
 docs/reference/merge.rst
 docs/reference/montecarlo.rst
+docs/reference/multi_merge.rst
 docs/reference/partition.rst
 docs/reference/presets.rst
-docs/reference/print_order.rst
+docs/reference/print_order_as_letters.rst
+docs/reference/scorers.rst
 docs/reference/sort.rst
 docs/reference/sort_asort_quickselect.rst
+docs/reference/sort_binary_insertion.rst
 docs/reference/sort_ford_johnson.rst
 docs/reference/sort_largest_interval.rst
-docs/reference/sort_merge_bfs.rst
-docs/reference/sort_merge_dfs.rst
+docs/reference/sort_merge_bottom_up.rst
+docs/reference/sort_merge_top_down.rst
+docs/reference/sort_multizip.rst
 docs/reference/sort_quick.rst
+docs/reference/sort_shell.rst
+docs/reference/split_pointer_lists.rst
+docs/reference/util_chains.rst
+docs/reference/util_latex.rst
 docs/reference/wrap_full_jit.rst
 docs/reference/wrap_sort_scorer.rst
 tests/__init__.py
 tests/test_corsort.py
 tests/test_sort.py
 tests/test_wrap_full_jit.py
 tests/test_wrap_sort_scorer.py
```

### Comparing `corsort-0.1.1/docs/Makefile` & `corsort-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/docs/conf.py` & `corsort-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/docs/installation.rst` & `corsort-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/docs/logo/logo.png` & `corsort-0.1.2/docs/logo/logo.png`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/docs/logo/logo_small.png` & `corsort-0.1.2/docs/logo/logo_small.png`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/docs/make.bat` & `corsort-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `corsort-0.1.1/setup.py` & `corsort-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     keywords='corsort',
     name='corsort',
     packages=find_packages(),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/emczg/corsort',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `corsort-0.1.1/tests/test_corsort.py` & `corsort-0.1.2/tests/test_corsort.py`

 * *Files identical despite different names*

