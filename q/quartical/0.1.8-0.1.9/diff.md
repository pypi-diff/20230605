# Comparing `tmp/quartical-0.1.8.tar.gz` & `tmp/quartical-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartical-0.1.8.tar", last modified: Thu Nov 17 08:59:04 2022, max compression
+gzip compressed data, was "quartical-0.1.9.tar", last modified: Thu Nov 24 10:13:17 2022, max compression
```

## Comparing `quartical-0.1.8.tar` & `quartical-0.1.9.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.594570 quartical-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-17 08:59:04.000000 quartical-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-17 08:59:04.000000 quartical-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-11-17 08:59:04.594570 quartical-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-11-17 08:59:04.000000 quartical-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.582570 quartical-0.1.8/quartical/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.582570 quartical-0.1.8/quartical/apps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4407 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/apps/backup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10511 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/apps/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.586570 quartical-0.1.8/quartical/calibration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11975 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/calibration/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (121)    10814 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/calibration/constructor.py
--rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/calibration/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/calibration/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.586570 quartical-0.1.8/quartical/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/config/converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     8773 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/config/external.py
--rw-r--r--   0 runner    (1001) docker     (121)     4407 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/config/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    12310 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/config/helpstrings.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/config/internal.py
--rw-r--r--   0 runner    (1001) docker     (121)     4308 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/config/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/config/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.586570 quartical-0.1.8/quartical/data_handling/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/data_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11452 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/data_handling/angles.py
--rw-r--r--   0 runner    (1001) docker     (121)     9049 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/data_handling/bda.py
--rw-r--r--   0 runner    (1001) docker     (121)     8269 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/data_handling/chunking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5408 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/data_handling/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    15845 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/data_handling/ms_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    17299 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/data_handling/predict.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/data_handling/selection.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/data_handling/wisdom.py
--rw-r--r--   0 runner    (1001) docker     (121)     6913 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.586570 quartical-0.1.8/quartical/flagging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/flagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8950 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/flagging/flagging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/flagging/flagging_kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.586570 quartical-0.1.8/quartical/gains/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.586570 quartical-0.1.8/quartical/gains/amplitude/
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/amplitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19879 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/amplitude/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/gains/complex/
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18923 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/complex/diag_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    18881 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/complex/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/gains/crosshand_phase/
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/crosshand_phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19270 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/crosshand_phase/kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    16182 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/gains/delay/
--rw-r--r--   0 runner    (1001) docker     (121)     6636 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/delay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24050 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/delay/kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6517 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/gain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/gains/general/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3453 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/general/convenience.py
--rw-r--r--   0 runner    (1001) docker     (121)    23088 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/general/factories.py
--rw-r--r--   0 runner    (1001) docker     (121)    12700 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/general/flagging.py
--rw-r--r--   0 runner    (1001) docker     (121)    16519 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/general/generics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3550 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/general/inversion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/gains/phase/
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21754 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/phase/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/gains/rotation_measure/
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/rotation_measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20628 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/rotation_measure/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/gains/tec/
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/tec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6669 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/gains/tec/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/interpolation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6648 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/interpolation/interpolants.py
--rw-r--r--   0 runner    (1001) docker     (121)    10963 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/interpolation/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/logging/
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/scheduling/
--rw-r--r--   0 runner    (1001) docker     (121)     5754 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/scheduling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.590570 quartical-0.1.8/quartical/statistics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5641 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/statistics/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/statistics/stat_kernels.py
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/statistics/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.594570 quartical-0.1.8/quartical/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (121)    12149 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/utils/dask.py
--rw-r--r--   0 runner    (1001) docker     (121)     7373 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/utils/intervals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/utils/maths.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/utils/numba.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/utils/timings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.594570 quartical-0.1.8/quartical/weights/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/weights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7974 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/weights/robust.py
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical/weights/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.582570 quartical-0.1.8/quartical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2854 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-17 08:59:04.000000 quartical-0.1.8/quartical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 08:59:04.594570 quartical-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-11-17 08:59:04.000000 quartical-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.594570 quartical-0.1.8/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3918 2022-11-17 08:59:04.000000 quartical-0.1.8/testing/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.594570 quartical-0.1.8/testing/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 08:59:04.000000 quartical-0.1.8/testing/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-11-17 08:59:04.000000 quartical-0.1.8/testing/fixtures/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-11-17 08:59:04.000000 quartical-0.1.8/testing/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-11-17 08:59:04.000000 quartical-0.1.8/testing/fixtures/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-11-17 08:59:04.000000 quartical-0.1.8/testing/fixtures/gains.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.096158 quartical-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2022-11-24 10:13:16.000000 quartical-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2022-11-24 10:13:16.000000 quartical-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2022-11-24 10:13:17.096158 quartical-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2022-11-24 10:13:16.000000 quartical-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4407 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/apps/backup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10511 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/apps/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical/calibration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11975 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10814 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7043 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5932 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8808 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/external.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4407 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12372 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/helpstrings.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1797 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/internal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4410 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3275 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/data_handling/
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11452 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/angles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9049 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/bda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8269 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/chunking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6021 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16419 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/ms_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17299 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/wisdom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7000 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/flagging/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/flagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/flagging/flagging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4157 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/flagging/flagging_kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/amplitude/
+-rw-r--r--   0 runner    (1001) docker     (122)     2420 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/amplitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19879 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/amplitude/kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/complex/
+-rw-r--r--   0 runner    (1001) docker     (122)     1285 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18923 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/complex/diag_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18881 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/complex/kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/crosshand_phase/
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/crosshand_phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19270 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/crosshand_phase/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16182 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/delay/
+-rw-r--r--   0 runner    (1001) docker     (122)     6636 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/delay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24050 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/delay/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6517 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/gain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/general/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3453 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23088 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12700 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/flagging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16519 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/generics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3550 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/inversion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/phase/
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21754 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/phase/kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/gains/rotation_measure/
+-rw-r--r--   0 runner    (1001) docker     (122)     2580 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/rotation_measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20628 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/rotation_measure/kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/gains/tec/
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/tec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/tec/kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6648 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/interpolation/interpolants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10963 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/interpolation/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (122)     5754 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/scheduling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/statistics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5641 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/statistics/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/statistics/stat_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/statistics/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12149 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/dask.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7373 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1539 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/maths.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/numba.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/timings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/weights/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/weights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7974 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/weights/robust.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/weights/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2854 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 10:13:17.096158 quartical-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1897 2022-11-24 10:13:16.000000 quartical-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3921 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/testing/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2793 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/gains.py
```

### Comparing `quartical-0.1.8/LICENSE` & `quartical-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/PKG-INFO` & `quartical-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartical
-Version: 0.1.8
+Version: 0.1.9
 Summary: Fast calibration implementation exploiting complex optimisation.
 Home-page: https://github.com/JSKenyon/QuartiCal
 Author: Jonathan Kenyon
 Author-email: jonosken@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `quartical-0.1.8/README.md` & `quartical-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/apps/backup.py` & `quartical-0.1.9/quartical/apps/backup.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/apps/summary.py` & `quartical-0.1.9/quartical/apps/summary.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/calibration/calibrate.py` & `quartical-0.1.9/quartical/calibration/calibrate.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/calibration/constructor.py` & `quartical-0.1.9/quartical/calibration/constructor.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/calibration/mapping.py` & `quartical-0.1.9/quartical/calibration/mapping.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/calibration/solver.py` & `quartical-0.1.9/quartical/calibration/solver.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/config/converters.py` & `quartical-0.1.9/quartical/config/converters.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/config/external.py` & `quartical-0.1.9/quartical/config/external.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,37 +81,38 @@
     )
     beam_m_axis: str = field(
         default="Y",
         metadata=dict(choices=["X", "~X", "Y", "~Y", "L", "~L", "M", "~M"])
     )
     invert_uvw: bool = True
     source_chunks: int = 500
-    apply_p_jones: bool = True
+    apply_p_jones: bool = False
 
     def __post_init__(self):
         self.validate_choice_fields()
 
 
 @dataclass
 class Outputs(Input):
     gain_directory: str = "gains.qc"
     log_directory: str = "logs.qc"
+    log_to_terminal: bool = True
     overwrite: bool = False
     products: Optional[List[str]] = field(
         default=None,
         metadata=dict(choices=["corrected_data",
                                "corrected_residual",
                                "residual",
                                "weight",
                                "corrected_weight",
                                "model_data"])
     )
     columns: Optional[List[str]] = None
     flags: bool = True
-    apply_p_jones_inv: bool = True
+    apply_p_jones_inv: bool = False
     subtract_directions: Optional[List[int]] = None
     net_gains: Optional[List[Any]] = None
 
     def __post_init__(self):
         self.validate_choice_fields()
         assert not (bool(self.products) ^ bool(self.columns)), \
             "Neither or both of products and columns must be specified."
```

### Comparing `quartical-0.1.8/quartical/config/helper.py` & `quartical-0.1.9/quartical/config/helper.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/config/helpstrings.yaml` & `quartical-0.1.9/quartical/config/helpstrings.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 output:
   gain_directory:
     Name of directory in which QuartiCal gain outputs will be stored. Accepts
     both local and s3 paths. QuartiCal will always produce gain outputs.
   log_directory:
     Name of directory in which QuartiCal logging outputs will be stored. s3
     is not currently supported for these outputs.
+  log_to_terminal:
+    Enable or disable logging to terminal.
   overwrite:
     Whether or not the contents of the output directory may be overwritten.
     Will trigger an error when False and output.directory already exists.
   products:
     The desired output data products. Multiple data products can be specified
     as a list e.g. [residual, corrected_residual]. Any required measurement
     set outputs should be specified here. Note that the output names of the
```

### Comparing `quartical-0.1.8/quartical/config/internal.py` & `quartical-0.1.9/quartical/config/internal.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/config/parser.py` & `quartical-0.1.9/quartical/config/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,33 +36,37 @@
 
     logger.success("{} successfully generated. Go forth and calibrate!",
                    config_file_path)
 
     return
 
 
-def log_final_config(config):
+def log_final_config(config, config_files=[]):
     """Logs the final state of the configuration object.
 
     Given the overlapping nature of the various configuration options, this
     produces a pretty log message describing the final configuration state.
 
     Args:
         config: A FinalConfig object.
+        config_files: A list of filenames.
     """
 
     config = oc.structured(config)
 
     # This guards against attempting to get the terminal size when the output
     # is being piped/redirected.
     if sys.stdout.isatty():
         columns, _ = os.get_terminal_size(0)
     else:
         columns = 80  # Fall over to some sensible default.
 
+    for cf in config_files:
+        logger.info(f"Using user-defined config file: {cf}")
+
     log_message = "Final configuration state:"
 
     current_section = None
 
     for section, options in config.items():
 
         if current_section != section:
@@ -102,16 +106,14 @@
     # We use sys.argv unless the bypass is set - this is needed for testing.
     for arg in (bypass_sysargv or sys.argv):
         if arg.endswith(('.yaml', '.yml')):
             if arg in config_files:
                 raise ValueError(f"Config file {arg} is duplicated.")
             config_files.append(arg)
 
-            logger.info("User defined config file: {}", arg)
-
     for file in config_files:
         (bypass_sysargv or sys.argv).remove(file)  # Remove config files.
 
     # Get all specified configuration - multiple yaml files and cli.
     yml_config = [oc.load(file) for file in config_files]
     cli_config = [] if bypass_sysargv else [oc.from_cli()]
     additional_config = [*yml_config, *cli_config]
@@ -124,8 +126,8 @@
     # Log the final state of the configuration object so that users are aware
     # of what the ultimate configuration was.
 
     config_obj = oc.to_object(config)  # Ensures post_init methods are run.
 
     additional_validation(config_obj)
 
-    return config_obj
+    return config_obj, config_files
```

### Comparing `quartical-0.1.8/quartical/config/preprocess.py` & `quartical-0.1.9/quartical/config/preprocess.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/data_handling/angles.py` & `quartical-0.1.9/quartical/data_handling/angles.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/data_handling/bda.py` & `quartical-0.1.9/quartical/data_handling/bda.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/data_handling/chunking.py` & `quartical-0.1.9/quartical/data_handling/chunking.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/data_handling/model_handler.py` & `quartical-0.1.9/quartical/data_handling/model_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,27 @@
         predict_schemes = [{}]*len(data_xds_list)
 
     # NOTE: At this point we are ready to construct the model array. First,
     # however, we need to apply parallactic angle corrections to model columns
     # which require them. P Jones is applied to predicted components
     # internally, so we only need to consider model columns for now.
 
+    n_corr = {xds.dims["corr"] for xds in data_xds_list}.pop()
+
     if model_opts.apply_p_jones:
+        # NOTE: Applying parallactic angle when there are fewer than four
+        # correlations is problematic for linear feeds as it amounts to
+        # rotating information to/from correlations which are not present i.e.
+        # it is not reversible. We support it for input models but warn the
+        # user that it is not a good idea.
+        if n_corr != 4:
+            logger.warning(
+                "input_model.apply_p_jones is not recommended for data with "
+                "less than four correlations. Proceed with caution."
+            )
         model_columns = model_vis_recipe.ingredients.model_columns
         data_xds_list = apply_parangles(data_xds_list,
                                         parangle_xds_list,
                                         model_columns)
 
     # Initialise a list to contain the xdss after the model data has been
     # assigned.
@@ -99,17 +111,18 @@
 
                 # Adding and subtracting direction dependent models is not
                 # supported. If we have an operation with a single
                 # direction-dependent term, it is assumed to apply to the first
                 # direction only.
 
                 if len(in_a) > 1 and len(in_b) > 1:
-                    raise(ValueError("Model recipes do not support add or "
-                                     "subtract operations between two "
-                                     "direction-dependent inputs."))
+                    raise ValueError(
+                        "Model recipes do not support add or subtract "
+                        "operations between two direction-dependent inputs."
+                    )
                 elif len(in_a) > len(in_b):
                     result = [op(in_a[0], in_b[0]), *in_a[1:]]
                 elif len(in_a) < len(in_b):
                     result = [op(in_a[0], in_b[0]), *in_b[1:]]
                 else:
                     result = [op(in_a[0], in_b[0])]
                 in_a = result
```

### Comparing `quartical-0.1.8/quartical/data_handling/ms_handler.py` & `quartical-0.1.9/quartical/data_handling/ms_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -385,15 +385,26 @@
         output_opts: An Outputs config object.
 
     Returns:
         output_data_xds_list: A list of xarray.DataSet objects containing MS
             data with postprocessing operations applied.
     """
 
+    n_corr = {xds.dims["corr"] for xds in data_xds_list}.pop()
+
     if output_opts.apply_p_jones_inv:
+        # NOTE: Applying parallactic angle when there are fewer than four
+        # correlations is problematic for linear feeds as it amounts to
+        # rotating information to/from correlations which are not present i.e.
+        # it is not reversible. Thus, we elect not to support it.
+        if n_corr != 4:
+            raise ValueError(
+                "output.apply_p_jones_inv is not supported for data with "
+                "less than four correlations. Please disable this setting."
+            )
         derot_vars = ["_RESIDUAL", "_CORRECTED_DATA", "_CORRECTED_RESIDUAL"]
 
         output_data_xds_list = apply_parangles(data_xds_list,
                                                parangle_xds_list,
                                                derot_vars,
                                                derotate=True)
     else:
```

### Comparing `quartical-0.1.8/quartical/data_handling/predict.py` & `quartical-0.1.9/quartical/data_handling/predict.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/executor.py` & `quartical-0.1.9/quartical/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,34 +34,38 @@
 
 def _execute(exitstack):
     """Runs the application."""
 
     helper.help()  # Check to see if the user asked for help.
 
     # Get all the config. This should never be used directly.
-    opts = parser.parse_inputs()
+    opts, config_files = parser.parse_inputs()
 
     # Split out all the configuration objects. Mitigates god-object problems.
     ms_opts = opts.input_ms
     model_opts = opts.input_model
     solver_opts = opts.solver
     output_opts = opts.output
     mad_flag_opts = opts.mad_flags
     dask_opts = opts.dask
     chain_opts = internal.gains_to_chain(opts)  # Special handling.
 
     # Init the logging proxy - an object which helps us ensure that logging
     # works for both threads an processes. It is easily picklable.
 
     time_str = time.strftime("%Y%m%d_%H%M%S")
-    proxy_logger = ProxyLogger(output_opts.log_directory, time_str)
+    proxy_logger = ProxyLogger(
+        output_opts.log_directory,
+        time_str,
+        output_opts.log_to_terminal
+    )
     proxy_logger.configure()
 
     # Now that we know where to put the log, log the final config state.
-    parser.log_final_config(opts)
+    parser.log_final_config(opts, config_files)
 
     model_vis_recipe = preprocess.transcribe_recipe(model_opts.recipe)
 
     if dask_opts.scheduler == "distributed":
 
         # NOTE: This is needed to allow threads to spawn processes in a
         # distributed enviroment. This *may* be dangerous. Monitor.
```

### Comparing `quartical-0.1.8/quartical/flagging/flagging.py` & `quartical-0.1.9/quartical/flagging/flagging.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/flagging/flagging_kernels.py` & `quartical-0.1.9/quartical/flagging/flagging_kernels.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/__init__.py` & `quartical-0.1.9/quartical/gains/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/amplitude/__init__.py` & `quartical-0.1.9/quartical/gains/amplitude/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/amplitude/kernel.py` & `quartical-0.1.9/quartical/gains/amplitude/kernel.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/complex/__init__.py` & `quartical-0.1.9/quartical/gains/complex/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/complex/diag_kernel.py` & `quartical-0.1.9/quartical/gains/complex/diag_kernel.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/complex/kernel.py` & `quartical-0.1.9/quartical/gains/complex/kernel.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/crosshand_phase/__init__.py` & `quartical-0.1.9/quartical/gains/crosshand_phase/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/crosshand_phase/kernel.py` & `quartical-0.1.9/quartical/gains/crosshand_phase/kernel.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/datasets.py` & `quartical-0.1.9/quartical/gains/datasets.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/delay/__init__.py` & `quartical-0.1.9/quartical/gains/delay/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/delay/kernel.py` & `quartical-0.1.9/quartical/gains/delay/kernel.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/gain.py` & `quartical-0.1.9/quartical/gains/gain.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/general/convenience.py` & `quartical-0.1.9/quartical/gains/general/convenience.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/general/factories.py` & `quartical-0.1.9/quartical/gains/general/factories.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/general/flagging.py` & `quartical-0.1.9/quartical/gains/general/flagging.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/general/generics.py` & `quartical-0.1.9/quartical/gains/general/generics.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/general/inversion.py` & `quartical-0.1.9/quartical/gains/general/inversion.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/phase/__init__.py` & `quartical-0.1.9/quartical/gains/phase/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/phase/kernel.py` & `quartical-0.1.9/quartical/gains/phase/kernel.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/rotation_measure/__init__.py` & `quartical-0.1.9/quartical/gains/rotation_measure/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/rotation_measure/kernel.py` & `quartical-0.1.9/quartical/gains/rotation_measure/kernel.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/tec/__init__.py` & `quartical-0.1.9/quartical/gains/tec/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/gains/tec/kernel.py` & `quartical-0.1.9/quartical/gains/tec/kernel.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/interpolation/interpolants.py` & `quartical-0.1.9/quartical/interpolation/interpolants.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/interpolation/interpolate.py` & `quartical-0.1.9/quartical/interpolation/interpolate.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/logging/__init__.py` & `quartical-0.1.9/quartical/logging/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,21 +23,22 @@
         # in the 7th frame upward.
         logger_opt = logger.opt(depth=7, exception=record.exc_info)
         logger_opt.log(record.levelname, record.getMessage())
 
 
 class ProxyLogger(object):
 
-    def __init__(self, output_dir, birth=None):
+    def __init__(self, output_dir, birth=None, log_to_term=True):
 
         self.birth = birth or time.strftime("%Y%m%d_%H%M%S")
         self.output_dir = Path(output_dir)
+        self.log_to_term = log_to_term
 
     def __reduce__(self):
-        return (ProxyLogger, (self.output_dir, self.birth))
+        return (ProxyLogger, (self.output_dir, self.birth, self.log_to_term))
 
     def configure(self):
         logging.basicConfig(handlers=[InterceptHandler()], level="WARNING")
 
         # Put together a formatting string for the logger.
 
         tim_fmt = "<green>{time:YYYY-MM-DD HH:mm:ss}</green>"
@@ -48,21 +49,22 @@
         fmt = " | ".join([tim_fmt, lvl_fmt, src_fmt, msg_fmt])
 
         output_path = Path(self.output_dir)
         output_name = Path(f"{self.birth}.log.qc")
 
         logger.remove()  # Remove existing handlers.
 
-        logger.add(
-            sys.stderr,
-            level="INFO",
-            format=fmt,
-            enqueue=True,
-            colorize=True
-        )
+        if self.log_to_term:
+            logger.add(
+                sys.stderr,
+                level="INFO",
+                format=fmt,
+                enqueue=True,
+                colorize=True
+            )
 
         logger.add(
             str(output_path / output_name),
             level="DEBUG",
             format=fmt,
             enqueue=True,
             colorize=False
```

### Comparing `quartical-0.1.8/quartical/scheduling/__init__.py` & `quartical-0.1.9/quartical/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/statistics/logging.py` & `quartical-0.1.9/quartical/statistics/logging.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/statistics/stat_kernels.py` & `quartical-0.1.9/quartical/statistics/stat_kernels.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/statistics/statistics.py` & `quartical-0.1.9/quartical/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/utils/dask.py` & `quartical-0.1.9/quartical/utils/dask.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/utils/intervals.py` & `quartical-0.1.9/quartical/utils/intervals.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/utils/maths.py` & `quartical-0.1.9/quartical/utils/maths.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/weights/robust.py` & `quartical-0.1.9/quartical/weights/robust.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical/weights/weights.py` & `quartical-0.1.9/quartical/weights/weights.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/quartical.egg-info/PKG-INFO` & `quartical-0.1.9/quartical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartical
-Version: 0.1.8
+Version: 0.1.9
 Summary: Fast calibration implementation exploiting complex optimisation.
 Home-page: https://github.com/JSKenyon/QuartiCal
 Author: Jonathan Kenyon
 Author-email: jonosken@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `quartical-0.1.8/quartical.egg-info/SOURCES.txt` & `quartical-0.1.9/quartical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/setup.py` & `quartical-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "colorama",
     "bokeh",
     "xarray>=0.20.0"
 ]
 
 setup(
     name='quartical',
-    version='0.1.8',
+    version='0.1.9',
     description="Fast calibration implementation exploiting complex "
                 "optimisation.",
     url='https://github.com/JSKenyon/QuartiCal',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
```

### Comparing `quartical-0.1.8/testing/conftest.py` & `quartical-0.1.9/testing/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,11 +127,11 @@
 
 
 @pytest.fixture(scope="module")
 def base_opts(ms_name):
     """Get basic config from .yaml file."""
 
     # We use bypass_sysargv to avoid mucking with the CLI.
-    options = parse_inputs(bypass_sysargv=['goquartical', str(conf_path)])
+    options, _ = parse_inputs(bypass_sysargv=['goquartical', str(conf_path)])
     options.input_ms.path = ms_name  # Ensure the ms path is correct.
 
     return options
```

### Comparing `quartical-0.1.8/testing/fixtures/calibration.py` & `quartical-0.1.9/testing/fixtures/calibration.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/testing/fixtures/config.py` & `quartical-0.1.9/testing/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/testing/fixtures/data_handling.py` & `quartical-0.1.9/testing/fixtures/data_handling.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.8/testing/fixtures/gains.py` & `quartical-0.1.9/testing/fixtures/gains.py`

 * *Files identical despite different names*

