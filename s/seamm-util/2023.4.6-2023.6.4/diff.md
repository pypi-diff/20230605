# Comparing `tmp/seamm_util-2023.4.6.tar.gz` & `tmp/seamm_util-2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_util-2023.4.6.tar", last modified: Thu Apr  6 15:43:51 2023, max compression
+gzip compressed data, was "seamm_util-2023.6.4.tar", last modified: Mon Jun  5 02:11:55 2023, max compression
```

## Comparing `seamm_util-2023.4.6.tar` & `seamm_util-2023.6.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:43:51.058423 seamm_util-2023.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-06 15:43:51.062423 seamm_util-2023.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:43:51.046423 seamm_util-2023.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8689 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/requirements_install.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:43:51.062423 seamm_util-2023.4.6/seamm_util/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-06 15:43:51.062423 seamm_util-2023.4.6/seamm_util/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23511 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/check_executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/compact_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    63121 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/elemental_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/include_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/md_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    30207 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/seamm_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/seamm_json.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/seamm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/water_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/seamm_util/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:43:51.050423 seamm_util-2023.4.6/seamm_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-06 15:43:51.000000 seamm_util-2023.4.6/seamm_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-06 15:43:51.000000 seamm_util-2023.4.6/seamm_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:43:51.000000 seamm_util-2023.4.6/seamm_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-06 15:43:51.000000 seamm_util-2023.4.6/seamm_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 15:43:51.000000 seamm_util-2023.4.6/seamm_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-06 15:43:51.062423 seamm_util-2023.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:43:51.054423 seamm_util-2023.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:43:51.058423 seamm_util-2023.4.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/blank_lines.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/blank_lines.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/blank_lines.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/empty_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/empty_file.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/empty_file.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file1.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file1.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_#include.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_#include.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_#include.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_end.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_end.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_end.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_include1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_include1.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_include1.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_middle.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_middle.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/file_middle.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/include_blank_lines.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/include_blank_lines.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/include_blank_lines.txt.gz
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/include_empty_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/include_empty_file.txt.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/data/include_empty_file.txt.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:43:51.058423 seamm_util-2023.4.6/tests/results/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/results/simple_plot.html
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/results/two_plots.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:43:51.058423 seamm_util-2023.4.6/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/templates/line.html_template
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/test_open_bzip2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/test_open_gzipped.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/test_plotting_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-06 15:43:36.000000 seamm_util-2023.4.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:11:55.539641 seamm_util-2023.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-05 02:11:55.539641 seamm_util-2023.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:11:55.527641 seamm_util-2023.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8689 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/requirements_install.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:11:55.547641 seamm_util-2023.6.4/seamm_util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-05 02:11:55.547641 seamm_util-2023.6.4/seamm_util/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23511 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/check_executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/compact_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63121 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/elemental_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/include_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/md_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30207 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/seamm_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/seamm_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/seamm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/water_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/seamm_util/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:11:55.531641 seamm_util-2023.6.4/seamm_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-05 02:11:55.000000 seamm_util-2023.6.4/seamm_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-05 02:11:55.000000 seamm_util-2023.6.4/seamm_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 02:11:55.000000 seamm_util-2023.6.4/seamm_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 02:11:55.000000 seamm_util-2023.6.4/seamm_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 02:11:55.000000 seamm_util-2023.6.4/seamm_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-05 02:11:55.547641 seamm_util-2023.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:11:55.535641 seamm_util-2023.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:11:55.539641 seamm_util-2023.6.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/blank_lines.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/blank_lines.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/blank_lines.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/empty_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/empty_file.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/empty_file.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file1.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file1.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_#include.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_#include.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_#include.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_end.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_end.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_end.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_include1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_include1.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_include1.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_middle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_middle.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/file_middle.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/include_blank_lines.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/include_blank_lines.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/include_blank_lines.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/include_empty_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/include_empty_file.txt.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/data/include_empty_file.txt.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:11:55.539641 seamm_util-2023.6.4/tests/results/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/results/simple_plot.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/results/two_plots.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 02:11:55.539641 seamm_util-2023.6.4/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/templates/line.html_template
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/test_open_bzip2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/test_open_gzipped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/test_plotting_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-05 02:11:34.000000 seamm_util-2023.6.4/versioneer.py
```

### Comparing `seamm_util-2023.4.6/CONTRIBUTING.rst` & `seamm_util-2023.6.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/HISTORY.rst` & `seamm_util-2023.6.4/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 =======
 History
 =======
 
+2023.6.4 -- Added more unit conversions to support thermochemistry
+  * added E_h/K --> kJ/mol/K
+
 2023.4.6 -- Added more unit conversions to support Buckingham potentials
   * added e.g. eV*Å^6 to kcal/mol*Å^6 to support Buckingham pontetials
     
 2023.2.28 -- Added a compact JSON encoder
   * To make the schema-type JSON more human-readable.
     
 2022.11.3 -- More conversions involving substance (mol) to number
```

### Comparing `seamm_util-2023.4.6/LICENSE` & `seamm_util-2023.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/PKG-INFO` & `seamm_util-2023.6.4/seamm_util.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seamm_util
-Version: 2023.4.6
+Name: seamm-util
+Version: 2023.6.4
 Summary: seamm_util
 Home-page: https://github.com/molssi-seamm/seamm_util
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: seamm_util
 Platform: Linux
@@ -80,14 +80,17 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.6.4 -- Added more unit conversions to support thermochemistry
+  * added E_h/K --> kJ/mol/K
+
 2023.4.6 -- Added more unit conversions to support Buckingham potentials
   * added e.g. eV*Å^6 to kcal/mol*Å^6 to support Buckingham pontetials
     
 2023.2.28 -- Added a compact JSON encoder
   * To make the schema-type JSON more human-readable.
     
 2022.11.3 -- More conversions involving substance (mol) to number
```

### Comparing `seamm_util-2023.4.6/README.rst` & `seamm_util-2023.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/docs/Makefile` & `seamm_util-2023.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/docs/conf.py` & `seamm_util-2023.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/docs/index.rst` & `seamm_util-2023.6.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/docs/installation.rst` & `seamm_util-2023.6.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/docs/make.bat` & `seamm_util-2023.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/__init__.py` & `seamm_util-2023.6.4/seamm_util/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/argument_parser.py` & `seamm_util-2023.6.4/seamm_util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/check_executable.py` & `seamm_util-2023.6.4/seamm_util/check_executable.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/compact_json_encoder.py` & `seamm_util-2023.6.4/seamm_util/compact_json_encoder.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/dictionary.py` & `seamm_util-2023.6.4/seamm_util/dictionary.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/elemental_data.py` & `seamm_util-2023.6.4/seamm_util/elemental_data.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/include_open.py` & `seamm_util-2023.6.4/seamm_util/include_open.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/md_statistics.py` & `seamm_util-2023.6.4/seamm_util/md_statistics.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/output.py` & `seamm_util-2023.6.4/seamm_util/output.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/plotting.py` & `seamm_util-2023.6.4/seamm_util/plotting.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/printing.py` & `seamm_util-2023.6.4/seamm_util/printing.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/seamm_file.py` & `seamm_util-2023.6.4/seamm_util/seamm_file.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/seamm_json.py` & `seamm_util-2023.6.4/seamm_util/seamm_json.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/units.py` & `seamm_util-2023.6.4/seamm_util/units.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,36 +150,50 @@
 
 _d.add_transformation("1 / [substance]", "", lambda ureg, x: x * factor)
 _d.add_transformation("", "1 / [substance]", lambda ureg, x: x / factor)
 
 _d.add_transformation("[mass] / [substance]", "[mass]", lambda ureg, x: x * factor)
 _d.add_transformation("[mass]", "[mass] / [substance]", lambda ureg, x: x / factor)
 
+# kJ/mol/Å --> eV/Å
 _d.add_transformation(
     "[length] * [mass] / [substance] / [time] ** 2",
     "[length] * [mass] / [time] ** 2",
     lambda ureg, x: x * factor,
 )
 _d.add_transformation(
     "[length] * [mass] / [time] ** 2",
     "[length] * [mass] / [substance] / [time] ** 2",
     lambda ureg, x: x / factor,
 )
 
+# kJ/mol --> eV
 _d.add_transformation(
     "[length] ** 2 * [mass] / [substance] / [time] ** 2",
     "[length] ** 2 * [mass] / [time] ** 2",
     lambda ureg, x: x * factor,
 )
 _d.add_transformation(
     "[length] ** 2 * [mass] / [time] ** 2",
     "[length] ** 2 * [mass] / [substance] / [time] ** 2",
     lambda ureg, x: x / factor,
 )
 
+# kJ/mol/K --> eV/K
+_d.add_transformation(
+    "[length] ** 2 * [mass] / [substance] / [temperature] / [time] ** 2",
+    "[length] ** 2 * [mass] / [temperature] / [time] ** 2",
+    lambda ureg, x: x * factor,
+)
+_d.add_transformation(
+    "[length] ** 2 * [mass] / [temperature] / [time] ** 2",
+    "[length] ** 2 * [mass] / [substance] / [temperature] / [time] ** 2",
+    lambda ureg, x: x / factor,
+)
+
 # kJ/mol/Å^2 --> eV/Å^2
 _d.add_transformation(
     "[mass] / [substance] / [time] ** 2",
     "[mass] / [time] ** 2",
     lambda ureg, x: x * factor,
 )
```

### Comparing `seamm_util-2023.4.6/seamm_util/variable_names.py` & `seamm_util-2023.6.4/seamm_util/variable_names.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/water_models.py` & `seamm_util-2023.6.4/seamm_util/water_models.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util/zenodo.py` & `seamm_util-2023.6.4/seamm_util/zenodo.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/seamm_util.egg-info/PKG-INFO` & `seamm_util-2023.6.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seamm-util
-Version: 2023.4.6
+Name: seamm_util
+Version: 2023.6.4
 Summary: seamm_util
 Home-page: https://github.com/molssi-seamm/seamm_util
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: seamm_util
 Platform: Linux
@@ -80,14 +80,17 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.6.4 -- Added more unit conversions to support thermochemistry
+  * added E_h/K --> kJ/mol/K
+
 2023.4.6 -- Added more unit conversions to support Buckingham potentials
   * added e.g. eV*Å^6 to kcal/mol*Å^6 to support Buckingham pontetials
     
 2023.2.28 -- Added a compact JSON encoder
   * To make the schema-type JSON more human-readable.
     
 2022.11.3 -- More conversions involving substance (mol) to number
```

### Comparing `seamm_util-2023.4.6/seamm_util.egg-info/SOURCES.txt` & `seamm_util-2023.6.4/seamm_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/setup.py` & `seamm_util-2023.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/results/simple_plot.html` & `seamm_util-2023.6.4/tests/results/simple_plot.html`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/results/two_plots.html` & `seamm_util-2023.6.4/tests/results/two_plots.html`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/templates/line.html_template` & `seamm_util-2023.6.4/tests/templates/line.html_template`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/test_dictionary.py` & `seamm_util-2023.6.4/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/test_open.py` & `seamm_util-2023.6.4/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/test_open_bzip2.py` & `seamm_util-2023.6.4/tests/test_open_bzip2.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/test_open_gzipped.py` & `seamm_util-2023.6.4/tests/test_open_gzipped.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/test_plotting.py` & `seamm_util-2023.6.4/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/test_plotting_figure.py` & `seamm_util-2023.6.4/tests/test_plotting_figure.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/tests/test_units.py` & `seamm_util-2023.6.4/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `seamm_util-2023.4.6/versioneer.py` & `seamm_util-2023.6.4/versioneer.py`

 * *Files identical despite different names*

