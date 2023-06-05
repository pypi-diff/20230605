# Comparing `tmp/simcardems-2023.5.4.tar.gz` & `tmp/simcardems-2023.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simcardems-2023.5.4.tar", last modified: Tue May 23 20:04:29 2023, max compression
+gzip compressed data, was "simcardems-2023.5.5.tar", last modified: Mon Jun  5 10:52:52 2023, max compression
```

## Comparing `simcardems-2023.5.4.tar` & `simcardems-2023.5.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.361799 simcardems-2023.5.4/
--rw-r--r--   0 root         (0) root         (0)    26526 2023-05-23 19:54:13.000000 simcardems-2023.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3845 2023-05-23 20:04:29.361799 simcardems-2023.5.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3141 2023-05-23 19:54:13.000000 simcardems-2023.5.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-23 20:04:29.365799 simcardems-2023.5.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      296 2023-05-23 19:54:14.000000 simcardems-2023.5.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.349799 simcardems-2023.5.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.357799 simcardems-2023.5.4/src/simcardems/
--rw-r--r--   0 root         (0) root         (0)     3453 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/__main__.py
--rw-r--r--   0 root         (0) root         (0)    10005 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/benchmark.py
--rw-r--r--   0 root         (0) root         (0)     5423 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     9241 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/cli.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/config.py
--rw-r--r--   0 root         (0) root         (0)    18669 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/datacollector.py
--rw-r--r--   0 root         (0) root         (0)    10019 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/ep_model.py
--rw-r--r--   0 root         (0) root         (0)    17148 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/geometry.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/gui.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/lvgeometry.py
--rw-r--r--   0 root         (0) root         (0)    11482 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/mechanics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.357799 simcardems-2023.5.4/src/simcardems/models/
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      333 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/cell_model.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.357799 simcardems-2023.5.4/src/simcardems/models/explicit_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      819 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/explicit_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60760 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    14164 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/explicit_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.361799 simcardems-2023.5.4/src/simcardems/models/fully_coupled_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6993 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    60344 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    12046 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.361799 simcardems-2023.5.4/src/simcardems/models/fully_coupled_Tor_Land/
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6989 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    70634 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    12043 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.361799 simcardems-2023.5.4/src/simcardems/models/pureEP_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60636 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
--rw-r--r--   0 root         (0) root         (0)     5730 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/newton_solver.py
--rw-r--r--   0 root         (0) root         (0)    21897 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/postprocess.py
--rw-r--r--   0 root         (0) root         (0)     7156 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/runner.py
--rw-r--r--   0 root         (0) root         (0)     6485 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/save_load_functions.py
--rw-r--r--   0 root         (0) root         (0)     4515 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/slabgeometry.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/time_stepper.py
--rw-r--r--   0 root         (0) root         (0)     5462 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/utils.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/value_extractor.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-23 19:54:14.000000 simcardems-2023.5.4/src/simcardems/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.357799 simcardems-2023.5.4/src/simcardems.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3845 2023-05-23 20:04:29.000000 simcardems-2023.5.4/src/simcardems.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2052 2023-05-23 20:04:29.000000 simcardems-2023.5.4/src/simcardems.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 20:04:29.000000 simcardems-2023.5.4/src/simcardems.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-23 20:04:29.000000 simcardems-2023.5.4/src/simcardems.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 19:54:37.000000 simcardems-2023.5.4/src/simcardems.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-23 20:04:29.000000 simcardems-2023.5.4/src/simcardems.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-23 20:04:29.000000 simcardems-2023.5.4/src/simcardems.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:04:29.361799 simcardems-2023.5.4/tests/
--rw-r--r--   0 root         (0) root         (0)      523 2023-05-23 19:54:14.000000 simcardems-2023.5.4/tests/test_boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-23 19:54:14.000000 simcardems-2023.5.4/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-05-23 19:54:14.000000 simcardems-2023.5.4/tests/test_datacollector.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-23 19:54:14.000000 simcardems-2023.5.4/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-05-23 19:54:14.000000 simcardems-2023.5.4/tests/test_mechanics_model.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-23 19:54:14.000000 simcardems-2023.5.4/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-05-23 19:54:14.000000 simcardems-2023.5.4/tests/test_postprocessing.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-05-23 19:54:14.000000 simcardems-2023.5.4/tests/test_runner.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-23 19:54:14.000000 simcardems-2023.5.4/tests/test_save_load_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.997527 simcardems-2023.5.5/
+-rw-r--r--   0 root         (0) root         (0)    26526 2023-06-05 10:34:58.000000 simcardems-2023.5.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-06-05 10:52:51.997527 simcardems-2023.5.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-06-05 10:34:58.000000 simcardems-2023.5.5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-06-05 10:52:51.997527 simcardems-2023.5.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-05 10:34:58.000000 simcardems-2023.5.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.981526 simcardems-2023.5.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems/
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    10005 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     9241 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/config.py
+-rw-r--r--   0 root         (0) root         (0)    18669 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/datacollector.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/ep_model.py
+-rw-r--r--   0 root         (0) root         (0)    17148 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/geometry.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/gui.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/lvgeometry.py
+-rw-r--r--   0 root         (0) root         (0)    11482 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/mechanics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems/models/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      819 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60760 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    14164 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6993 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    60344 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12046 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.993527 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    70634 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12043 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.993527 simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60636 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
+-rw-r--r--   0 root         (0) root         (0)     5730 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/newton_solver.py
+-rw-r--r--   0 root         (0) root         (0)    21900 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/runner.py
+-rw-r--r--   0 root         (0) root         (0)     6485 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/save_load_functions.py
+-rw-r--r--   0 root         (0) root         (0)     4515 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/slabgeometry.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/time_stepper.py
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/value_extractor.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-05 10:34:58.000000 simcardems-2023.5.5/src/simcardems/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.989527 simcardems-2023.5.5/src/simcardems.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:35:22.000000 simcardems-2023.5.5/src/simcardems.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      337 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-05 10:52:51.000000 simcardems-2023.5.5/src/simcardems.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:52:51.997527 simcardems-2023.5.5/tests/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_datacollector.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_mechanics_model.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_postprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-05 10:34:58.000000 simcardems-2023.5.5/tests/test_save_load_functions.py
```

### Comparing `simcardems-2023.5.4/LICENSE` & `simcardems-2023.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/PKG-INFO` & `simcardems-2023.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.5.4
+Version: 2023.5.5
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.5.4/README.md` & `simcardems-2023.5.5/README.md`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/setup.cfg` & `simcardems-2023.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/__init__.py` & `simcardems-2023.5.5/src/simcardems/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/benchmark.py` & `simcardems-2023.5.5/src/simcardems/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     \\hline
     {body}
     \\end{{tabular}}
     \\end{{center}}
     """,
     ).format(
         c="c" * (len(dxs) + 1),
-        heading=" &".join(["feature"] + [f"dt={dx}" for dx in dxs]) + "\\\\ \n",
+        heading=" &".join(["feature"] + [f"dx={dx}" for dx in dxs]) + "\\\\ \n",
         body=body,
     )
     return table
 
 
 def create_table_dt(feature_keys, features, fixed_dx, dts):
     body = ""
```

### Comparing `simcardems-2023.5.4/src/simcardems/boundary_conditions.py` & `simcardems-2023.5.5/src/simcardems/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/cli.py` & `simcardems-2023.5.5/src/simcardems/cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/config.py` & `simcardems-2023.5.5/src/simcardems/config.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/datacollector.py` & `simcardems-2023.5.5/src/simcardems/datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/ep_model.py` & `simcardems-2023.5.5/src/simcardems/ep_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/geometry.py` & `simcardems-2023.5.5/src/simcardems/geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/gui.py` & `simcardems-2023.5.5/src/simcardems/gui.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/lvgeometry.py` & `simcardems-2023.5.5/src/simcardems/lvgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/mechanics_model.py` & `simcardems-2023.5.5/src/simcardems/mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/__init__.py` & `simcardems-2023.5.5/src/simcardems/models/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/em_model.py` & `simcardems-2023.5.5/src/simcardems/models/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/explicit_ORdmm_Land/__init__.py` & `simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/explicit_ORdmm_Land/cell_model.py` & `simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/explicit_ORdmm_Land/em_model.py` & `simcardems-2023.5.5/src/simcardems/models/explicit_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py` & `simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py` & `simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py` & `simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py` & `simcardems-2023.5.5/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/fully_coupled_Tor_Land/__init__.py` & `simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/fully_coupled_Tor_Land/active_model.py` & `simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py` & `simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/fully_coupled_Tor_Land/em_model.py` & `simcardems-2023.5.5/src/simcardems/models/fully_coupled_Tor_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py` & `simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/models/pureEP_ORdmm_Land/em_model.py` & `simcardems-2023.5.5/src/simcardems/models/pureEP_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/newton_solver.py` & `simcardems-2023.5.5/src/simcardems/newton_solver.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/postprocess.py` & `simcardems-2023.5.5/src/simcardems/postprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,15 +577,15 @@
     return activation_map
 
 
 def extract_sub_results(
     results_file: utils.PathLike,
     output_file: utils.PathLike,
     t_start: float = 0.0,
-    t_end: float | None = None,
+    t_end: Optional[float] = None,
     names: Optional[Dict[str, List[str]]] = None,
 ) -> DataCollector:
     """Extract sub results from another results file.
     This can be useful if you have stored a lot of data in one file
     and you want to create a smaller file containing only a subset
     of the data (e.g only the last beat)
```

### Comparing `simcardems-2023.5.4/src/simcardems/runner.py` & `simcardems-2023.5.5/src/simcardems/runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/save_load_functions.py` & `simcardems-2023.5.5/src/simcardems/save_load_functions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/slabgeometry.py` & `simcardems-2023.5.5/src/simcardems/slabgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/time_stepper.py` & `simcardems-2023.5.5/src/simcardems/time_stepper.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/utils.py` & `simcardems-2023.5.5/src/simcardems/utils.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems/value_extractor.py` & `simcardems-2023.5.5/src/simcardems/value_extractor.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/src/simcardems.egg-info/PKG-INFO` & `simcardems-2023.5.5/src/simcardems.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.5.4
+Version: 2023.5.5
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.5.4/src/simcardems.egg-info/SOURCES.txt` & `simcardems-2023.5.5/src/simcardems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/tests/test_boundary_conditions.py` & `simcardems-2023.5.5/tests/test_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/tests/test_cli.py` & `simcardems-2023.5.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/tests/test_datacollector.py` & `simcardems-2023.5.5/tests/test_datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/tests/test_geometry.py` & `simcardems-2023.5.5/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/tests/test_mechanics_model.py` & `simcardems-2023.5.5/tests/test_mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/tests/test_models.py` & `simcardems-2023.5.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/tests/test_postprocessing.py` & `simcardems-2023.5.5/tests/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/tests/test_runner.py` & `simcardems-2023.5.5/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.5.4/tests/test_save_load_functions.py` & `simcardems-2023.5.5/tests/test_save_load_functions.py`

 * *Files identical despite different names*

