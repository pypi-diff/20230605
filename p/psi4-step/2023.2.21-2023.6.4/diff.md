# Comparing `tmp/psi4_step-2023.2.21.tar.gz` & `tmp/psi4_step-2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psi4_step-2023.2.21.tar", last modified: Wed Feb 22 00:28:32 2023, max compression
+gzip compressed data, was "psi4_step-2023.6.4.tar", last modified: Mon Jun  5 13:17:59 2023, max compression
```

## Comparing `psi4_step-2023.2.21.tar` & `psi4_step-2023.6.4.tar`

### file list

```diff
@@ -1,85 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.797880 psi4_step-2023.2.21/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-02-22 00:28:32.797880 psi4_step-2023.2.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.789880 psi4_step-2023.2.21/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.789880 psi4_step-2023.2.21/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.789880 psi4_step-2023.2.21/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9473 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.789880 psi4_step-2023.2.21/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.789880 psi4_step-2023.2.21/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.789880 psi4_step-2023.2.21/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.797880 psi4_step-2023.2.21/psi4_step/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      428 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-22 00:28:32.797880 psi4_step-2023.2.21/psi4_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    52653 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/accelerated_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/accelerated_optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/accelerated_optimization_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.797880 psi4_step-2023.2.21/psi4_step/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12556 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/data/MOPAC_PM7_Hessian.flow
--rwxr-xr-x   0 runner    (1001) docker     (123)    11273 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/data/MOPAC_PM7_SPE.flow
--rwxr-xr-x   0 runner    (1001) docker     (123)    12933 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/data/MOPAC_PM7_surrogate.flow
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/data/opt_log.out
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/data/seamm-psi4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/initialization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/initialization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)    80716 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/psi4_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/psi4_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/psi4_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/tk_accelerated_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/tk_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/tk_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/psi4_step/tk_psi4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.793880 psi4_step-2023.2.21/psi4_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-02-22 00:28:32.000000 psi4_step-2023.2.21/psi4_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-22 00:28:32.000000 psi4_step-2023.2.21/psi4_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 00:28:32.000000 psi4_step-2023.2.21/psi4_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-22 00:28:32.000000 psi4_step-2023.2.21/psi4_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 00:28:32.000000 psi4_step-2023.2.21/psi4_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 00:28:32.000000 psi4_step-2023.2.21/psi4_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 00:28:18.000000 psi4_step-2023.2.21/psi4_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-22 00:28:32.797880 psi4_step-2023.2.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 00:28:32.797880 psi4_step-2023.2.21/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/tests/test_psi4_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-02-22 00:28:14.000000 psi4_step-2023.2.21/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.097945 psi4_step-2023.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-05 13:17:59.097945 psi4_step-2023.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.089945 psi4_step-2023.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.089945 psi4_step-2023.6.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.089945 psi4_step-2023.6.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9473 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.089945 psi4_step-2023.6.4/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.089945 psi4_step-2023.6.4/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.089945 psi4_step-2023.6.4/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.097945 psi4_step-2023.6.4/psi4_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      428 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-05 13:17:59.097945 psi4_step-2023.6.4/psi4_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52653 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/accelerated_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/accelerated_optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/accelerated_optimization_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.097945 psi4_step-2023.6.4/psi4_step/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12556 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/data/MOPAC_PM7_Hessian.flow
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11273 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/data/MOPAC_PM7_SPE.flow
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12933 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/data/MOPAC_PM7_surrogate.flow
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/data/opt_log.out
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/data/seamm-psi4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/initialization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/initialization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90749 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/psi4_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/psi4_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/psi4_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/thermochemistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/thermochemistry_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/thermochemistry_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/tk_accelerated_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/tk_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/tk_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/tk_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/psi4_step/tk_thermochemistry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.097945 psi4_step-2023.6.4/psi4_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-05 13:17:59.000000 psi4_step-2023.6.4/psi4_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-05 13:17:59.000000 psi4_step-2023.6.4/psi4_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:17:59.000000 psi4_step-2023.6.4/psi4_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-05 13:17:59.000000 psi4_step-2023.6.4/psi4_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 13:17:59.000000 psi4_step-2023.6.4/psi4_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 13:17:59.000000 psi4_step-2023.6.4/psi4_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:17:41.000000 psi4_step-2023.6.4/psi4_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-05 13:17:59.097945 psi4_step-2023.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:59.097945 psi4_step-2023.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/tests/test_psi4_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-05 13:17:34.000000 psi4_step-2023.6.4/versioneer.py
```

### Comparing `psi4_step-2023.2.21/CONTRIBUTING.rst` & `psi4_step-2023.6.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/HISTORY.rst` & `psi4_step-2023.6.4/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2023.6.4 -- Enhancements
+   * Added thermochemistry substep to compute the vibrational and other corrections for
+     thermochemistry.
+   * Added ability to create .cube files for plotting the density and orbitals.
+     
 2023.2.21 -- Added control over SCF convergence
    * Able to set convergence criteria.
    * Options for damping. level shifting and second-order SCF
    * Set default for number of steps for optimization to 6*nAtoms to
      make it more explicit.
      
 2023.2.17 -- Checking more thoroughly for errors in Psi4
```

### Comparing `psi4_step-2023.2.21/LICENSE` & `psi4_step-2023.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/PKG-INFO` & `psi4_step-2023.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psi4_step
-Version: 2023.2.21
+Version: 2023.6.4
 Summary: A SEAMM plug-in to setup, run and analyze quantum chemistry calculations using Psi4
 Home-page: https://github.com/molssi-seamm/psi4_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Psi4,DFT,quantum chemistry,CCSD
 Platform: Linux
@@ -93,14 +93,19 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.6.4 -- Enhancements
+   * Added thermochemistry substep to compute the vibrational and other corrections for
+     thermochemistry.
+   * Added ability to create .cube files for plotting the density and orbitals.
+     
 2023.2.21 -- Added control over SCF convergence
    * Able to set convergence criteria.
    * Options for damping. level shifting and second-order SCF
    * Set default for number of steps for optimization to 6*nAtoms to
      make it more explicit.
      
 2023.2.17 -- Checking more thoroughly for errors in Psi4
```

### Comparing `psi4_step-2023.2.21/README.rst` & `psi4_step-2023.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/Makefile` & `psi4_step-2023.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/_static/SEAMM inverted.png` & `psi4_step-2023.6.4/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/_static/SEAMM logo.png` & `psi4_step-2023.6.4/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/_static/molssi_main_logo.png` & `psi4_step-2023.6.4/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/_static/molssi_main_logo_inverted_white.png` & `psi4_step-2023.6.4/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/_static/molssi_square.png` & `psi4_step-2023.6.4/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/_static/nsf.png` & `psi4_step-2023.6.4/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/conf.py` & `psi4_step-2023.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/developer_guide/installation.rst` & `psi4_step-2023.6.4/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/getting_started/index.rst` & `psi4_step-2023.6.4/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/index.rst` & `psi4_step-2023.6.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/docs/make.bat` & `psi4_step-2023.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/__init__.py` & `psi4_step-2023.6.4/psi4_step/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,51 +4,56 @@
 psi4_step
 A step for Psi4 in a SEAMM flowchart
 """
 
 # Bring up the classes so that they appear to be directly in
 # the psi4_step package.
 
-from psi4_step.psi4_metadata import methods  # noqa: F401
-from psi4_step.psi4_metadata import dft_functionals  # noqa: F401
-from psi4_step.psi4_metadata import optimization_methods  # noqa: F401
-from psi4_step.psi4_metadata import optimization_convergence  # noqa: F401
-from psi4_step.psi4_metadata import metadata  # noqa: F401
-
-from psi4_step.psi4 import Psi4  # noqa: F401
-from psi4_step.psi4_parameters import Psi4Parameters  # noqa: F401
-from psi4_step.psi4_step import Psi4Step  # noqa: F401
-from psi4_step.tk_psi4 import TkPsi4  # noqa: F401
-
-from psi4_step.initialization import Initialization  # noqa: F401
-from psi4_step.initialization_parameters import InitializationParameters  # noqa: F401
-from psi4_step.initialization_step import InitializationStep  # noqa: F401
-from psi4_step.tk_initialization import TkInitialization  # noqa: F401
-
-from psi4_step.energy import Energy  # noqa: F401
-from psi4_step.energy_parameters import EnergyParameters  # noqa: F401
-from psi4_step.energy_step import EnergyStep  # noqa: F401
-from psi4_step.tk_energy import TkEnergy  # noqa: F401
-
-from psi4_step.optimization import Optimization  # noqa: F401
-from psi4_step.optimization_parameters import OptimizationParameters  # noqa: F401
-from psi4_step.optimization_step import OptimizationStep  # noqa: F401
-from psi4_step.tk_optimization import TkOptimization  # noqa: F401
+from .psi4_metadata import methods  # noqa: F401
+from .psi4_metadata import dft_functionals  # noqa: F401
+from .psi4_metadata import optimization_methods  # noqa: F401
+from .psi4_metadata import optimization_convergence  # noqa: F401
+from .psi4_metadata import metadata  # noqa: F401
+
+from .psi4 import Psi4  # noqa: F401
+from .psi4_parameters import Psi4Parameters  # noqa: F401
+from .psi4_step import Psi4Step  # noqa: F401
+from .tk_psi4 import TkPsi4  # noqa: F401
+
+from .initialization import Initialization  # noqa: F401
+from .initialization_parameters import InitializationParameters  # noqa: F401
+from .initialization_step import InitializationStep  # noqa: F401
+from .tk_initialization import TkInitialization  # noqa: F401
+
+from .energy import Energy  # noqa: F401
+from .energy_parameters import EnergyParameters  # noqa: F401
+from .energy_step import EnergyStep  # noqa: F401
+from .tk_energy import TkEnergy  # noqa: F401
+
+from .optimization import Optimization  # noqa: F401
+from .optimization_parameters import OptimizationParameters  # noqa: F401
+from .optimization_step import OptimizationStep  # noqa: F401
+from .tk_optimization import TkOptimization  # noqa: F401
 
-# from psi4_step.accelerated_optimization import AcceleratedOptimization  # noqa: F401
-# from psi4_step.accelerated_optimization_parameters import (  # noqa: F401
+# from .accelerated_optimization import AcceleratedOptimization  # noqa: F401
+# from .accelerated_optimization_parameters import (  # noqa: F401
 #     AcceleratedOptimizationParameters,
 # )
-# from psi4_step.accelerated_optimization_step import (  # noqa: F401
+# from .accelerated_optimization_step import (  # noqa: F401
 #     AcceleratedOptimizationStep,
 # )
-# from psi4_step.tk_accelerated_optimization import (  # noqa: F401
+# from .tk_accelerated_optimization import (  # noqa: F401
 #     TkAcceleratedOptimization,
 # )
 
+from .thermochemistry_step import ThermochemistryStep  # noqa: F401
+from .thermochemistry import Thermochemistry  # noqa: F401
+from .thermochemistry_parameters import ThermochemistryParameters  # noqa: F401
+from .tk_thermochemistry import TkThermochemistry  # noqa: F401
+
 # Handle versioneer
 from ._version import get_versions
 
 __author__ = """Paul Saxe"""
 __email__ = "psaxe@molssi.org"
 versions = get_versions()
 __version__ = versions["version"]
```

### Comparing `psi4_step-2023.2.21/psi4_step/accelerated_optimization.py` & `psi4_step-2023.6.4/psi4_step/accelerated_optimization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/accelerated_optimization_parameters.py` & `psi4_step-2023.6.4/psi4_step/accelerated_optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/accelerated_optimization_step.py` & `psi4_step-2023.6.4/psi4_step/accelerated_optimization_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/data/MOPAC_PM7_Hessian.flow` & `psi4_step-2023.6.4/psi4_step/data/MOPAC_PM7_Hessian.flow`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/data/MOPAC_PM7_SPE.flow` & `psi4_step-2023.6.4/psi4_step/data/MOPAC_PM7_SPE.flow`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/data/MOPAC_PM7_surrogate.flow` & `psi4_step-2023.6.4/psi4_step/data/MOPAC_PM7_surrogate.flow`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/data/configuration.txt` & `psi4_step-2023.6.4/psi4_step/data/configuration.txt`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/data/references.bib` & `psi4_step-2023.6.4/psi4_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/energy_parameters.py` & `psi4_step-2023.6.4/psi4_step/energy_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,14 +268,49 @@
             "help_text": (
                 "Whether to create tables as needed for "
                 "results being saved into tables."
             ),
         },
     }
 
+    output = {
+        "density": {
+            "default": "no",
+            "kind": "boolean",
+            "default_units": "",
+            "enumeration": ("yes", "no"),
+            "format_string": "",
+            "description": "Plot total density:",
+            "help_text": "Whether to plot the total charge density.",
+        },
+        "orbitals": {
+            "default": "no",
+            "kind": "boolean",
+            "default_units": "",
+            "enumeration": ("yes", "no"),
+            "format_string": "",
+            "description": "Plot orbitals:",
+            "help_text": "Whether to plot orbitals.",
+        },
+        "selected orbitals": {
+            "default": "-1, HOMO, LUMO, +1",
+            "kind": "string",
+            "default_units": "",
+            "enumeration": ("all", "-1, HOMO, LUMO, +1"),
+            "format_string": "",
+            "description": "Selected orbitals:",
+            "help_text": "Which orbitals to plot.",
+        },
+    }
+
     def __init__(self, defaults={}, data=None):
         """Initialize the instance, by default from the default
         parameters given in the class"""
 
         super().__init__(
-            defaults={**EnergyParameters.parameters, **defaults}, data=data
+            defaults={
+                **EnergyParameters.parameters,
+                **EnergyParameters.output,
+                **defaults,
+            },
+            data=data,
         )
```

### Comparing `psi4_step-2023.2.21/psi4_step/energy_step.py` & `psi4_step-2023.6.4/psi4_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/initialization.py` & `psi4_step-2023.6.4/psi4_step/initialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         result.append("")
         result.append("#" * 80)
         result.append(f"# {self.header}")
         result.append("#" * 80)
 
         result.append(f"set basis {P['basis']}")
         result.append("")
-        # result.append(f"initial.symmetrize({P['symmetry_tolerance']})")
+        result.append(f"initial.symmetrize({P['symmetry_tolerance']})")
         result.append("point_group = initial.point_group().symbol()")
 
         # Dump the properties to a json file
         filename = f"@{self._id[-1]}+properties.json"
         result.append("")
         result.append("variables = {'point group': point_group}")
         result.append("")
```

### Comparing `psi4_step-2023.2.21/psi4_step/initialization_step.py` & `psi4_step-2023.6.4/psi4_step/initialization_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/installer.py` & `psi4_step-2023.6.4/psi4_step/installer.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/optimization.py` & `psi4_step-2023.6.4/psi4_step/optimization.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,21 @@
 
 logger = logging.getLogger(__name__)
 job = printing.getPrinter()
 printer = printing.getPrinter("psi4")
 
 
 class Optimization(psi4_step.Energy):
-    def __init__(self, flowchart=None, title="Optimization", extension=None):
+    def __init__(
+        self,
+        flowchart=None,
+        title="Optimization",
+        extension=None,
+        logger=logger,
+    ):
         """Initialize the node"""
 
         logger.debug("Creating Optimization {}".format(self))
 
         super().__init__(flowchart=flowchart, title=title, extension=extension)
 
         self._calculation = "optimization"
```

### Comparing `psi4_step-2023.2.21/psi4_step/optimization_parameters.py` & `psi4_step-2023.6.4/psi4_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/optimization_step.py` & `psi4_step-2023.6.4/psi4_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/optimizer.py` & `psi4_step-2023.6.4/psi4_step/optimizer.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/psi4.py` & `psi4_step-2023.6.4/psi4_step/psi4.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,14 +418,15 @@
 
         #     node = node.next()
 
         # Start the input data
         input_data = []
         input_data.append("import json")
         input_data.append("import numpy as np")
+        input_data.append("from pathlib import Path")
         input_data.append("import pprint")
         input_data.append("")
         input_data.append(f"memory {memory}")
         input_data.append("")
         input_data.append(pre_code)
         input_data.append("")
 
@@ -457,44 +458,63 @@
 
         files = {"input.dat": "\n".join(input_data)}
         self.logger.info("input.dat:\n" + files["input.dat"])
 
         directory = Path(self.directory)
         directory.mkdir(parents=True, exist_ok=True)
 
-        return_files = ["output.dat", "*properties.json", "*structure.json"]
-        exe_path = Path(options["psi4_path"])
-        env = {
-            "PSIPATH": str(exe_path),
-            "PATH": str(exe_path),
-        }
-
-        local = seamm.ExecLocal()
-        exe = exe_path / "psi4"
-        result = local.run(
-            cmd=[str(exe), f"-n {n_threads}"],
-            files=files,
-            return_files=return_files,
-            env=env,
-            directory=directory,
-            in_situ=True,
-        )  # yapf: disable
-
-        if result is None:
-            self.logger.error("There was an error running Psi4")
-            raise RuntimeError("There was an error running Psi4")
-
-        self.logger.debug("\n" + pprint.pformat(result))
-
-        failed = False
-        if "output.dat" in result["files"]:
-            if result["output.dat"]["data"] is not None:
-                if "*** Psi4 exiting successfully." not in result["output.dat"]["data"]:
-                    self.logger.warning("Psi4 did not complete successfully.")
-                    failed = True
+        return_files = ["output.dat", "*.json", "*.cube"]
+
+        # Check for already having run
+        path = Path(self.directory) / "success.dat"
+        if path.exists():
+            result = {}
+            path = Path(self.directory) / "stdout.txt"
+            if path.exists():
+                result["stdout"] = path.read_text()
+            result["stderr"] = ""
+            failed = False
+        else:
+            exe_path = Path(options["psi4_path"])
+            env = {
+                "PSIPATH": str(exe_path),
+                "PATH": str(exe_path),
+            }
+
+            local = seamm.ExecLocal()
+            exe = exe_path / "psi4"
+            result = local.run(
+                cmd=[str(exe), f"-n {n_threads}"],
+                files=files,
+                return_files=return_files,
+                env=env,
+                directory=directory,
+                in_situ=True,
+            )  # yapf: disable
+
+            if result is None:
+                self.logger.error("There was an error running Psi4")
+                raise RuntimeError("There was an error running Psi4")
+
+            self.logger.debug("\n" + pprint.pformat(result))
+
+            failed = False
+            if "output.dat" in result["files"]:
+                if result["output.dat"]["data"] is not None:
+                    if (
+                        "*** Psi4 exiting successfully."
+                        not in result["output.dat"]["data"]
+                    ):
+                        self.logger.warning("Psi4 did not complete successfully.")
+                        failed = True
+            if not failed:
+                # Write a small file to say that LAMMPS ran successfully, so cancel
+                # skip if rerunning.
+                path = Path(self.directory) / "success.dat"
+                path.write_text("success")
 
         # Analyze the results
         self.analyze()
 
         if failed:
             raise RuntimeError("Psi4 did not complete successfully.")
```

### Comparing `psi4_step-2023.2.21/psi4_step/psi4_metadata.py` & `psi4_step-2023.6.4/psi4_step/psi4_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1621,811 +1621,1147 @@
     The type of the data: string, integer, or float.
 
 units : str
     Optional units for the result. If present, the value should be in these units.
 """
 metadata["results"] = {
     "(T) CORRECTION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd(t)"],
         "type": "float",
         "units": "",
     },
     "-D ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "dispersion correction energy",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "-D GRADIENT": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "gradient of the dispersion correction energy",
         "dimensionality": [3, "n_atoms"],
         "methods": ["dft"],
         "type": "float",
         "units": "E_h/a_0",
     },
     "32-POLE": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "5th order electrical multipole",
         "dimensionality": ["triangular", 3, 3, 3, 3, 3],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
     "AAA (T) CORRECTION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "AAB (T) CORRECTION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "ABB (T) CORRECTION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "B3LYP-D3(BJ) DISPERSION CORRECTION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the dispersion correction energy",
         "dimensionality": "scalar",
         "methods": ["dft"],
         "type": "float",
         "units": "E_h",
     },
     "BBB (T) CORRECTION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "CC D1 DIAGNOSTIC": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)"],
         "type": "float",
     },
     "CC D2 DIAGNOSTIC": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)"],
         "type": "float",
     },
     "CC NEW D1 DIAGNOSTIC": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)"],
         "type": "float",
     },
     "CC T1 DIAGNOSTIC": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)"],
         "type": "float",
     },
     "CCSD CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the correlation energy for a CCSD calculation",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "CCSD OPPOSITE-SPIN CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "CCSD SAME-SPIN CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "CCSD TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the total electronic energy from a CCSD calculation",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "CCSD(T) CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "CCSD(T) TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "CURRENT CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the correlation energy for the current method",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "CURRENT DIPOLE": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the electrical dipole moment for the current method",
         "dimensionality": [3],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "D",
     },
     "CURRENT DIPOLE X": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the electrical dipole moment for the current method",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "D",
     },
     "CURRENT DIPOLE Y": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the electrical dipole moment for the current method",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "D",
     },
     "CURRENT DIPOLE Z": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the electrical dipole moment for the current method",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "D",
     },
     "CURRENT ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the electronic energy from the current method",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "property": "total energy#Psi4#{model}",
         "type": "float",
         "units": "E_h",
     },
     "CURRENT GRADIENT": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the gradient of the energy for the current method",
         "dimensionality": [3, "n_atoms"],
         "methods": ["dft", "hf"],
         "type": "float",
         "units": "E_h/a_0",
     },
     "CURRENT REFERENCE ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "DFT FUNCTIONAL TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "total energy of DFT functional",
         "dimensionality": "scalar",
         "methods": ["dft"],
         "type": "float",
         "units": "E_h",
     },
     "DFT TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "Total DFT energy including dispersion",
         "dimensionality": "scalar",
         "methods": ["dft"],
         "type": "float",
         "units": "E_h",
     },
     "DFT VV10 ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "VV10 energy in DFT",
         "dimensionality": "scalar",
         "methods": ["dft"],
         "type": "float",
         "units": "E_h",
     },
     "DFT XC ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "DFT exchange-correlation energy",
         "dimensionality": "scalar",
         "methods": ["dft"],
         "type": "float",
         "units": "E_h",
     },
     "DIPOLE": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical dipole moment",
         "dimensionality": [3],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "D",
     },
     "DIPOLE X": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical dipole moment",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "D",
     },
     "DIPOLE Y": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical dipole moment",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "D",
     },
     "DIPOLE Z": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical dipole moment",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "D",
     },
     "DISPERSION CORRECTION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "energy of the dispersion correction",
         "dimensionality": "scalar",
         "methods": ["dft"],
         "type": "float",
         "units": "E_h",
     },
     "ELECTROSTATIC POTENTIAL": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the electrostatic potential at the nuclei",
         "dimensionality": ["n_atoms"],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "Eelec": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the electronic energy",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "property": "electronic energy#Psi4#{model}",
         "type": "float",
         "units": "E_h",
     },
     "HEXADECAPOLE": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical hexadecapole moment",
         "dimensionality": ["triangular", 3, 3, 3, 3],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
     "HF TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the Hartree-Fock electronic energy",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "LCCD CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd"],
         "type": "float",
         "units": "E_h",
     },
     "LCCD OPPOSITE-SPIN CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd"],
         "type": "float",
         "units": "E_h",
     },
     "LCCD SAME-SPIN CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd"],
         "type": "float",
         "units": "E_h",
     },
     "LCCD TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd"],
         "type": "float",
         "units": "E_h",
     },
     "LCCSD (+LMP2) TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)"],
         "type": "float",
         "units": "E_h",
     },
     "LOWDIN_CHARGES": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "atomic charges using Lowdin's method",
         "dimensionality": ["n_atoms"],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "e",
     },
     "MAYER_INDICES": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "Mayer's bond indices",
         "dimensionality": ["triangular", "n_atoms", "n_atoms"],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
     "MP2 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP2 OPPOSITE-SPIN CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP2 SAME-SPIN CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP2 SINGLES ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp2"],
         "type": "float",
         "units": "E_h",
     },
     "MP2 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP2.5 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP2.5 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP3 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP3 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP4 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP4 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP4(SDQ) CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP4(SDQ) TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP4(SDTQ) CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP4(SDTQ) TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MP4(T) CORRECTION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp4"],
         "type": "float",
         "units": "E_h",
     },
     "MULLIKEN_CHARGES": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "atomic charges using Mulliken's method",
         "dimensionality": ["n_atoms"],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "e",
     },
     "NUCLEAR REPULSION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "property": "nuclear repulsion energy",
         "type": "float",
         "units": "E_h",
     },
     "OCTUPOLE": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical octupole moment",
         "dimensionality": ["triangular", 3, 3, 3],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
     "ONE-ELECTRON ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the one-electron energy",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "OPTIMIZATION ITERATIONS": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3"],
         "type": "float",
     },
     "PCM POLARIZATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the PCM polarization energy",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "property": "dielectric energy#Psi4#{model}",
         "type": "float",
         "units": "E_h",
     },
     "QUADRUPOLE": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical quadrupole moment",
         "dimensionality": ["triangular", 3, 3],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
     "SCF DIPOLE": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical dipole moment from SCF",
         "dimensionality": [3],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
     "SCF DIPOLE X": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical dipole moment from SCF",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
     "SCF DIPOLE Y": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical dipole moment from SCF",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
     "SCF DIPOLE Z": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "electrical dipole moment from SCF",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
     "SCF ITERATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "SCF ITERATIONS": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "number of itereations in the SCF",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "integer",
     },
     "SCF TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "SCF TOTAL GRADIENT": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": [3, "n_atoms"],
         "methods": ["dft", "hf"],
         "type": "float",
         "units": "E_h/a_0",
     },
     "SCS-MP2 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp2", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCS-MP2 OPPOSITE-SPIN CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp2"],
         "type": "float",
         "units": "E_h",
     },
     "SCS-MP2 SAME-SPIN CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp2"],
         "type": "float",
         "units": "E_h",
     },
     "SCS-MP2 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp2", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCS-MP2-VDW CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCS-MP2-VDW TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCS-MP3 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCS-MP3 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCS-MP3-VDW CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCS-MP3-VDW TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCSN-MP2 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCSN-MP2 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCSN-MP3 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SCSN-MP3 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SOS-MP2 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SOS-MP2 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SOS-MP3 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SOS-MP3 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SOS-PI-MP2 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SOS-PI-MP2 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["lccd", "mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SOS-PI-MP3 CORRELATION ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "SOS-PI-MP3 TOTAL ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["mp3"],
         "type": "float",
         "units": "E_h",
     },
     "TWO-ELECTRON ENERGY": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the two-electron energy",
         "dimensionality": "scalar",
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
         "units": "E_h",
     },
     "WIBERG_LOWDIN_INDICES": {
-        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "the Wiber-Lowdin bond indices",
         "dimensionality": ["triangular", "n_atoms", "n_atoms"],
         "methods": ["ccsd", "ccsd(t)", "dft", "hf", "lccd", "mp2", "mp3", "mp4"],
         "type": "float",
     },
-}  # yapf: disable
+    "B": {
+        "calculation": ["thermochemistry"],
+        "description": "rotational constants",
+        "dimensionality": [3],
+        "type": "float",
+        "units": "cm^-1",
+    },
+    "Cp_elec": {
+        "calculation": ["thermochemistry"],
+        "description": "electronic Cp",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "Cp_rot": {
+        "calculation": ["thermochemistry"],
+        "description": "rotational Cp",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "Cp_tot": {
+        "calculation": ["thermochemistry"],
+        "description": "total Cp",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "Cp_trans": {
+        "calculation": ["thermochemistry"],
+        "description": "translational Cp",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "Cp_vib": {
+        "calculation": ["thermochemistry"],
+        "description": "vibrational Cp",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "Cv_elec": {
+        "calculation": ["thermochemistry"],
+        "description": "electronic Cv",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "Cv_rot": {
+        "calculation": ["thermochemistry"],
+        "description": "rotational Cv",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "Cv_tot": {
+        "calculation": ["thermochemistry"],
+        "description": "total Cv",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "Cv_trans": {
+        "calculation": ["thermochemistry"],
+        "description": "translational Cv",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "Cv_vib": {
+        "calculation": ["thermochemistry"],
+        "description": "vibrational Cv",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "E0": {
+        "calculation": ["thermochemistry"],
+        "description": "electronic energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "E_h",
+    },
+    "E_corr": {
+        "calculation": ["thermochemistry"],
+        "description": "total correction to the energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "E_elec": {
+        "calculation": ["thermochemistry"],
+        "description": "electronic correction to the energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "E_rot": {
+        "calculation": ["thermochemistry"],
+        "description": "rotational correction to the energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "E_tot": {
+        "calculation": ["thermochemistry"],
+        "description": "corrected energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "E_h",
+    },
+    "E_trans": {
+        "calculation": ["thermochemistry"],
+        "description": "translational correction to the energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "E_vib": {
+        "calculation": ["thermochemistry"],
+        "description": "vibrational correction to the energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "G_corr": {
+        "calculation": ["thermochemistry"],
+        "description": "total correction to the free energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "G_elec": {
+        "calculation": ["thermochemistry"],
+        "description": "electronic correction to the free energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "G_rot": {
+        "calculation": ["thermochemistry"],
+        "description": "rotational correction to the free energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "G_tot": {
+        "calculation": ["thermochemistry"],
+        "description": "corrected free energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "E_h",
+    },
+    "G_trans": {
+        "calculation": ["thermochemistry"],
+        "description": "translational correction to the free energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "G_vib": {
+        "calculation": ["thermochemistry"],
+        "description": "vibrational correction to the free energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "H_corr": {
+        "calculation": ["thermochemistry"],
+        "description": "total correction to the enthalpy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "H_elec": {
+        "calculation": ["thermochemistry"],
+        "description": "electronic correction to the enthalpy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "H_rot": {
+        "calculation": ["thermochemistry"],
+        "description": "rotational correction to the enthalpy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "H_tot": {
+        "calculation": ["thermochemistry"],
+        "description": "corrected enthalpy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "E_h",
+    },
+    "H_trans": {
+        "calculation": ["thermochemistry"],
+        "description": "translational correction to the enthalpy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "H_vib": {
+        "calculation": ["thermochemistry"],
+        "description": "vibrational correction to the enthalpy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "P": {
+        "calculation": ["thermochemistry"],
+        "description": "pressure",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "atm",
+    },
+    "S_corr": {
+        "calculation": ["thermochemistry"],
+        "description": "total correction to the entropy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "S_elec": {
+        "calculation": ["thermochemistry"],
+        "description": "electronic correction to the entropy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "S_rot": {
+        "calculation": ["thermochemistry"],
+        "description": "rotational correction to the entropy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "S_tot": {
+        "calculation": ["thermochemistry"],
+        "description": "corrected entropy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "S_trans": {
+        "calculation": ["thermochemistry"],
+        "description": "translational correction to the entropy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "S_vib": {
+        "calculation": ["thermochemistry"],
+        "description": "vibrational correction to the entropy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "J/mol/K",
+    },
+    "T": {
+        "calculation": ["thermochemistry"],
+        "description": "temperature",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "K",
+    },
+    "ZPE_corr": {
+        "calculation": ["thermochemistry"],
+        "description": "total zero-point energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "ZPE_elec": {
+        "calculation": ["thermochemistry"],
+        "description": "electronic zero-point energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "ZPE_rot": {
+        "calculation": ["thermochemistry"],
+        "description": "rotational zero-point energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "ZPE_tot": {
+        "calculation": ["thermochemistry"],
+        "description": "energy with zero-point",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "E_h",
+    },
+    "ZPE_trans": {
+        "calculation": ["thermochemistry"],
+        "description": "translational zero-point energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "ZPE_vib": {
+        "calculation": ["thermochemistry"],
+        "description": "vibrational zero-point energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "kJ/mol",
+    },
+    "degeneracy": {
+        "calculation": ["thermochemistry"],
+        "description": "degeneracy for the modes",
+        "dimensionality": ["n_atoms"],
+        "type": "integer",
+        "units": "",
+    },
+    "gamma": {
+        "calculation": ["thermochemistry"],
+        "description": "symmetry of the modes",
+        "dimensionality": ["n_atoms"],
+        "type": "string",
+        "units": "",
+    },
+    "omega": {
+        "calculation": ["thermochemistry"],
+        "description": "vibrational frequencies",
+        "dimensionality": ["n_atoms", 2],
+        "type": "string",
+        "units": "cm^-1",
+    },
+    "sigma": {
+        "calculation": ["thermochemistry"],
+        "description": "symmetry number",
+        "dimensionality": "scalar",
+        "type": "integer",
+        "units": "",
+    },
+}
```

### Comparing `psi4_step-2023.2.21/psi4_step/psi4_parameters.py` & `psi4_step-2023.6.4/psi4_step/psi4_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/psi4_step.py` & `psi4_step-2023.6.4/psi4_step/psi4_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/tk_accelerated_optimization.py` & `psi4_step-2023.6.4/psi4_step/tk_accelerated_optimization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/tk_energy.py` & `psi4_step-2023.6.4/psi4_step/tk_energy.py`

 * *Files 22% similar despite different names*

```diff
@@ -131,32 +131,66 @@
         self["advanced_method"].combobox.bind("<FocusOut>", self.reset_calculation)
 
         for key in ("use damping", "use level shift", "use soscf"):
             self[key].bind("<<ComboboxSelected>>", self.reset_convergence)
             self[key].bind("<Return>", self.reset_convergence)
             self[key].bind("<FocusOut>", self.reset_convergence)
 
+        # A tab for output -- orbitals, etc.
+        notebook = self["notebook"]
+        self["output frame"] = oframe = ttk.Frame(notebook)
+        notebook.insert(self["results frame"], oframe, text="Output", sticky="new")
+
+        # Frame to isolate widgets
+        p_frame = self["plot frame"] = ttk.LabelFrame(
+            self["output frame"],
+            borderwidth=4,
+            relief="sunken",
+            text="Plots",
+            labelanchor="n",
+            padding=10,
+        )
+
+        for key in psi4_step.EnergyParameters.output:
+            self[key] = P[key].widget(p_frame)
+
+        # Set the callbacks for changes
+        for widget in ("orbitals",):
+            w = self[widget]
+            w.combobox.bind("<<ComboboxSelected>>", self.reset_plotting)
+            w.combobox.bind("<Return>", self.reset_plotting)
+            w.combobox.bind("<FocusOut>", self.reset_plotting)
+        p_frame.grid(row=0, column=0, sticky="new")
+        oframe.columnconfigure(0, weight=1)
+
+        self.reset_plotting()
+
         # Top level needs to call reset_dialog
         if self.node.calculation == "energy":
             self.reset_dialog()
 
         self.logger.debug("Finished creating the dialog")
 
-    def reset_dialog(self, widget=None):
+        return frame
+
+    def reset_dialog(self, row=0, widget=None):
         """Layout the widgets as needed for the current state"""
 
         frame = self["frame"]
-        for slave in frame.grid_slaves():
-            slave.grid_forget()
+        if row == 0:
+            for slave in frame.grid_slaves():
+                slave.grid_forget()
 
-        self["calculation"].grid(row=0, column=0)
+        self["calculation"].grid(row=row, column=0)
         self.reset_calculation()
-        self["convergence"].grid(row=1, column=0)
+        row += 1
+        self["convergence"].grid(row=row, column=0)
         self.reset_convergence()
-        return 2
+        row += 1
+        return row
 
     def reset_calculation(self, widget=None):
         level = self["level"].get()
 
         if level == "recommended":
             long_method = self["method"].get()
             if self.is_expr(long_method):
@@ -287,7 +321,36 @@
                 self[key].grid(row=row, column=1, sticky=tk.EW)
                 widgets2.append(self[key])
                 row += 1
 
         frame.columnconfigure(0, minsize=150)
         sw.align_labels(widgets, sticky=tk.E)
         sw.align_labels(widgets2, sticky=tk.E)
+
+    def reset_plotting(self, widget=None):
+        frame = self["plot frame"]
+        for slave in frame.grid_slaves():
+            slave.grid_forget()
+
+        plot_orbitals = self["orbitals"].get() == "yes"
+
+        widgets = []
+
+        row = 0
+        for key in (
+            "density",
+            "orbitals",
+        ):
+            self[key].grid(row=row, column=0, columnspan=4, sticky=tk.EW)
+            widgets.append(self[key])
+            row += 1
+
+        if plot_orbitals:
+            key = "selected orbitals"
+            self[key].grid(row=row, column=1, columnspan=4, sticky=tk.EW)
+            row += 1
+
+        sw.align_labels(widgets, sticky=tk.E)
+        frame.columnconfigure(0, minsize=50)
+        frame.columnconfigure(4, weight=1)
+
+        return row
```

### Comparing `psi4_step-2023.2.21/psi4_step/tk_initialization.py` & `psi4_step-2023.6.4/psi4_step/tk_initialization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step/tk_optimization.py` & `psi4_step-2023.6.4/psi4_step/tk_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,24 +79,24 @@
         * reset_optimization handles the layout of the optimization
           section.
         """
 
         logger.debug("TkOptimization.create_dialog")
 
         # Let parent classes do their thing.
-        super().create_dialog(title=title)
+        frame = super().create_dialog(title=title)
 
         # Shortcut for parameters
         P = self.node.parameters
 
         logger.debug("Parameters:\n{}".format(pprint.pformat(P.to_dict())))
 
         # Frame to isolate widgets
         opt_frame = self["optimization"] = ttk.LabelFrame(
-            self["frame"],
+            frame,
             borderwidth=4,
             relief="sunken",
             text="Geometry Optimization",
             labelanchor="n",
             padding=10,
         )
 
@@ -112,14 +112,16 @@
             "<FocusOut>", self.reset_optimization
         )
 
         # Top level needs to call reset_dialog
         if self.node.calculation == "optimization":
             self.reset_dialog()
 
+        return frame
+
     def reset_dialog(self, widget=None):
         """Layout the widgets, letting our parents go first."""
         rows = super().reset_dialog()
 
         self["optimization"].grid(row=0, column=1, rowspan=rows, sticky=tk.N)
         # row += 1
```

### Comparing `psi4_step-2023.2.21/psi4_step/tk_psi4.py` & `psi4_step-2023.6.4/psi4_step/tk_psi4.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/psi4_step.egg-info/PKG-INFO` & `psi4_step-2023.6.4/psi4_step.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psi4-step
-Version: 2023.2.21
+Version: 2023.6.4
 Summary: A SEAMM plug-in to setup, run and analyze quantum chemistry calculations using Psi4
 Home-page: https://github.com/molssi-seamm/psi4_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Psi4,DFT,quantum chemistry,CCSD
 Platform: Linux
@@ -93,14 +93,19 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.6.4 -- Enhancements
+   * Added thermochemistry substep to compute the vibrational and other corrections for
+     thermochemistry.
+   * Added ability to create .cube files for plotting the density and orbitals.
+     
 2023.2.21 -- Added control over SCF convergence
    * Able to set convergence criteria.
    * Options for damping. level shifting and second-order SCF
    * Set default for number of steps for optimization to 6*nAtoms to
      make it more explicit.
      
 2023.2.17 -- Checking more thoroughly for errors in Psi4
```

### Comparing `psi4_step-2023.2.21/psi4_step.egg-info/SOURCES.txt` & `psi4_step-2023.6.4/psi4_step.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -45,19 +45,23 @@
 psi4_step/optimization_parameters.py
 psi4_step/optimization_step.py
 psi4_step/optimizer.py
 psi4_step/psi4.py
 psi4_step/psi4_metadata.py
 psi4_step/psi4_parameters.py
 psi4_step/psi4_step.py
+psi4_step/thermochemistry.py
+psi4_step/thermochemistry_parameters.py
+psi4_step/thermochemistry_step.py
 psi4_step/tk_accelerated_optimization.py
 psi4_step/tk_energy.py
 psi4_step/tk_initialization.py
 psi4_step/tk_optimization.py
 psi4_step/tk_psi4.py
+psi4_step/tk_thermochemistry.py
 psi4_step.egg-info/PKG-INFO
 psi4_step.egg-info/SOURCES.txt
 psi4_step.egg-info/dependency_links.txt
 psi4_step.egg-info/entry_points.txt
 psi4_step.egg-info/requires.txt
 psi4_step.egg-info/top_level.txt
 psi4_step.egg-info/zip-safe
```

### Comparing `psi4_step-2023.2.21/setup.py` & `psi4_step-2023.6.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,18 +65,20 @@
         'org.molssi.seamm': [
             'Psi4 = psi4_step:Psi4Step',
         ],
         'org.molssi.seamm.tk': [
             'Psi4 = psi4_step:Psi4Step',
         ],
         'org.molssi.seamm.psi4': [
+            'Thermochemistry = psi4_step:ThermochemistryStep',
             'Energy = psi4_step:EnergyStep',
             'Initialization = psi4_step:InitializationStep',
             'Optimization = psi4_step:OptimizationStep',
         ],
         'org.molssi.seamm.psi4.tk': [
+            'Thermochemistry = psi4_step:ThermochemistryStep',
             'Energy = psi4_step:EnergyStep',
             'Initialization = psi4_step:InitializationStep',
             'Optimization = psi4_step:OptimizationStep',
         ],
     }
-)
+)
```

### Comparing `psi4_step-2023.2.21/tests/test_psi4_step.py` & `psi4_step-2023.6.4/tests/test_psi4_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2023.2.21/versioneer.py` & `psi4_step-2023.6.4/versioneer.py`

 * *Files identical despite different names*

