# Comparing `tmp/nctoolkit-0.9.2.tar.gz` & `tmp/nctoolkit-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nctoolkit-0.9.2.tar", last modified: Tue Apr 25 11:10:34 2023, max compression
+gzip compressed data, was "nctoolkit-0.9.3.tar", last modified: Mon Jun  5 17:36:25 2023, max compression
```

## Comparing `nctoolkit-0.9.2.tar` & `nctoolkit-0.9.3.tar`

### file list

```diff
@@ -1,94 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.764715 nctoolkit-0.9.2/cheatsheet/
--rw-r--r--   0 runner    (1001) docker     (123)   257155 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/cheatsheet/nctoolkit_cheatsheet.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   362394 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/cheatsheet/nctoolkit_cheatsheet.pptx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.764715 nctoolkit-0.9.2/checklists/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-25 11:10:22.000000 nctoolkit-0.9.2/checklists/api_checker.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.768715 nctoolkit-0.9.2/data/
--rw-r--r--   0 runner    (1001) docker     (123)   802316 2023-04-25 11:10:23.000000 nctoolkit-0.9.2/data/geotiff.tif
--rw-r--r--   0 runner    (1001) docker     (123)   488867 2023-04-25 11:10:23.000000 nctoolkit-0.9.2/data/test1.html
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-04-25 11:10:23.000000 nctoolkit-0.9.2/data/test2.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/nctoolkit/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/add_etc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/anomaly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58907 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1932 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/append.py
--rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/cdo_command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/cellareas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/centres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/cleanup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/clear.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7360 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/compare.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7520 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/compare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/corr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/create_ensemble.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5265 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/distgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3666 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/esoteric.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/fill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/fldstat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/format.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/generate_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/inttime.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1559 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/masking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/matchpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/meridonials.py
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/mp_adders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/mp_matchers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/mp_matchups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/nco_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/phenology.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2558 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/reduce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/reduce_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6416 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/regrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2188 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/rename.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/rollstat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    46030 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/runthis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/session.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/setters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/split.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19267 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/static_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/strip_vars.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15954 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/subset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1080 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/sumall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/temp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/temporal_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/temporals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/thresholds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4202 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/to_lonlat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/to_nc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3594 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/toxarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/tozlev.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/unify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/validator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22629 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/validator_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19600 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/verticals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/nctoolkit/zonals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/nctoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-25 11:10:34.000000 nctoolkit-0.9.2/nctoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:10:34.776715 nctoolkit-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3245 2023-04-25 11:10:24.000000 nctoolkit-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:36:25.344592 nctoolkit-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-05 17:36:14.000000 nctoolkit-0.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 17:36:14.000000 nctoolkit-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-05 17:36:14.000000 nctoolkit-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-05 17:36:25.344592 nctoolkit-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-05 17:36:14.000000 nctoolkit-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:36:25.336592 nctoolkit-0.9.3/cheatsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)   257155 2023-06-05 17:36:14.000000 nctoolkit-0.9.3/cheatsheet/nctoolkit_cheatsheet.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   362394 2023-06-05 17:36:14.000000 nctoolkit-0.9.3/cheatsheet/nctoolkit_cheatsheet.pptx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:36:25.336592 nctoolkit-0.9.3/checklists/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-05 17:36:14.000000 nctoolkit-0.9.3/checklists/api_checker.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:36:25.336592 nctoolkit-0.9.3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   802316 2023-06-05 17:36:14.000000 nctoolkit-0.9.3/data/geotiff.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   488867 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/data/test1.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/data/test2.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:36:25.344592 nctoolkit-0.9.3/nctoolkit/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/add_etc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/anomaly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58885 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/append.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24608 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/cdo_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2166 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/cellareas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/centres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/cleanup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/clear.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7789 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7515 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/compare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/corr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/create_ensemble.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/distgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3667 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/esoteric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/fill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/fldstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/format.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/generate_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/inttime.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1557 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/masking.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/matchpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/meridonials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/mp_adders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/mp_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/mp_matchups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/nco_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/phenology.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2572 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/reduce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/reduce_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6401 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/regrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2228 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/rename.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/rollstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45968 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/runthis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      767 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/split.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19599 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/static_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/strip_vars.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16127 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/subset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/sumall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/temp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/temporal_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/temporals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/thresholds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4202 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/to_lonlat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/to_nc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3592 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/toxarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/tozlev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/unify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22712 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/validator_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19509 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/verticals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/nctoolkit/zonals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:36:25.344592 nctoolkit-0.9.3/nctoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-05 17:36:25.000000 nctoolkit-0.9.3/nctoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:36:25.344592 nctoolkit-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3245 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:36:25.344592 nctoolkit-0.9.3/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/testing/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 17:36:15.000000 nctoolkit-0.9.3/testing/test_scripting.py
```

### Comparing `nctoolkit-0.9.2/CODE_OF_CONDUCT.md` & `nctoolkit-0.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/LICENSE` & `nctoolkit-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/MANIFEST.in` & `nctoolkit-0.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/PKG-INFO` & `nctoolkit-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nctoolkit
-Version: 0.9.2
+Version: 0.9.3
 Summary: Fast and easy analysis of netCDF data in Python
 Home-page: https://github.com/pmlmodelling/nctoolkit
 Author: Robert Wilson
 Author-email: rwi@pml.ac.uk
 Maintainer: Robert Wilson
 Project-URL: Bug Tracker, https://github.com/pmlmodelling/nctoolkit/issues
 Project-URL: Documentation, https://nctoolkit.readthedocs.io/en/stable
```

### Comparing `nctoolkit-0.9.2/README.md` & `nctoolkit-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/cheatsheet/nctoolkit_cheatsheet.pdf` & `nctoolkit-0.9.3/cheatsheet/nctoolkit_cheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/cheatsheet/nctoolkit_cheatsheet.pptx` & `nctoolkit-0.9.3/cheatsheet/nctoolkit_cheatsheet.pptx`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/checklists/api_checker.ipynb` & `nctoolkit-0.9.3/checklists/api_checker.ipynb`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/data/geotiff.tif` & `nctoolkit-0.9.3/data/geotiff.tif`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/data/test1.html` & `nctoolkit-0.9.3/data/test1.html`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/data/test2.html` & `nctoolkit-0.9.3/data/test2.html`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/__init__.py` & `nctoolkit-0.9.3/nctoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/add_etc.py` & `nctoolkit-0.9.3/nctoolkit/add_etc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 import warnings
 import pandas as pd
 
 
 from nctoolkit.cleanup import cleanup
 from nctoolkit.runthis import run_this, run_cdo, tidy_command
 from nctoolkit.session import session_info, append_safe, remove_safe
-from nctoolkit.show import nc_variables, nc_years, nc_times
+from nctoolkit.show import nc_variables, nc_times
 from nctoolkit.temp_file import temp_file
 from nctoolkit.utils import version_above
 from nctoolkit.api import open_data
 import nctoolkit.api as api
 
-def day_stat(self, operation = None,  x=None):
+
+def day_stat(self, operation=None, x=None):
     """
     Do not use
     """
 
     if not isinstance(operation, str):
         raise ValueError("operation must be a str")
 
-    if operation not in  ["subtract", "divide"]:
+    if operation not in ["subtract", "divide"]:
         raise ValueError("only subtract")
 
     if operation == "subtract":
         stat = "sub"
 
     if operation == "divide":
         stat = "div"
@@ -52,16 +53,14 @@
 
     self.history.append(the_command)
 
     self._hold_history = copy.deepcopy(self.history)
     cleanup()
 
 
-
-
 def arithall(self, stat="divc", x=None):
     """
     Method to add, subtract etc. a constant from a dataset
     This is used by add etc.
     """
 
     if len(self) == 0:
@@ -82,56 +81,53 @@
     # throw error if there is a problem with var
     if var is not None:
         if not isinstance(var, str):
             raise TypeError("var supplied is not a string")
         if var not in nc_variables(ff):
             raise ValueError("var supplied is not available in the dataset")
 
-
-   
-
     new = False
     # throw error if the file to operate with does not exist
     if ff is not None:
         if os.path.exists(ff) is False:
             raise ValueError(f"{ff} does not exist!")
 
     # check compatibility
 
-    n_min  = self.contents.nlevels.min()
+    n_min = self.contents.nlevels.min()
 
-    ds = open_data(ff, checks = False)
+    ds = open_data(ff, checks=False)
     contents = ds.contents
 
     n_max = contents.nlevels.max()
 
     if n_max > n_min:
-        raise ValueError(f"Problem raised by incompatible number of vertical levels. {n_max} versus {n_min}. Please check dataset contents.")
+        raise ValueError(
+            f"Problem raised by incompatible number of vertical levels. {n_max} versus {n_min}. Please check dataset contents."
+        )
 
     if version_above(session_info["cdo"], "1.9.8"):
         new = True
     else:
         warnings.warn("Use CDO>=1.9.10 for smarter operations")
         self.run()
 
     bad_vars = False
 
     if var is None:
         for x in self:
             n_vars = len(nc_variables(ff))
             x_vars = len(nc_variables(x))
 
-            #if n_vars > x_vars:
-                #raise ValueError("Incompatible number of variables in datasets!")
+            # if n_vars > x_vars:
+            # raise ValueError("Incompatible number of variables in datasets!")
 
             if n_vars != x_vars:
                 if n_vars > 1:
-                    raise ValueError(
-                        "Incompatible number of variables in datasets!"
-                    )
+                    raise ValueError("Incompatible number of variables in datasets!")
 
     # grab the method string
     if new:
         if method == "mul":
             nc_str = "Multiplying by a"
         if method == "sub":
             nc_operation = "subtraction"
@@ -167,15 +163,14 @@
                     )
                     .drop(columns="time")
                 )
 
             ff_times_df = ff_times_df.astype("int")
 
     if new:
-
         self1 = self.copy()
 
         if len(self1) == 0:
             raise ValueError("This does not work on empty datasets!")
 
         # If the dataset has to be merged,
         # then this operation will not work without running it first
@@ -185,15 +180,17 @@
         for x in self1:
             x_times = nc_times(x)
             if x_times != []:
                 if isinstance(x_times[0], str):
                     years = [int(x.split("T")[0].split("-")[0]) for x in x_times]
                     months = [int(x.split("T")[0].split("-")[1]) for x in x_times]
                     days = [int(x.split("T")[0].split("-")[2]) for x in x_times]
-                    df = pd.DataFrame({"year": years, "month": months, "day": months}).astype("int")
+                    df = pd.DataFrame(
+                        {"year": years, "month": months, "day": months}
+                    ).astype("int")
                     self_times.append(df)
 
                 else:
                     years = [x.year for x in x_times]
                     months = [x.month for x in x_times]
                     days = [x.day for x in x_times]
                     hours = [x.hour for x in x_times]
@@ -201,15 +198,14 @@
                         {"year": years, "month": months, "day": days, "hour": hours}
                     ).astype("int")
                     df["path"] = x
                     self_times.append(df)
             else:
                 self_times.append(None)
 
-
         possible_switch = True
         for x in self_times:
             if x is None:
                 possible_switch = False
 
     # figure out if a yearly will do
     possible_switch = True
@@ -275,16 +271,24 @@
                 warnings.warn(f"{nc_str} multi-year monthly time series")
 
     # figure out if this is a multi-year daily ts
     possible_switch = True
     if new:
         if ff_times_df.groupby(["month", "year", "day"]).size().max() == 1:
             for ss in self_times:
-                x11=  ss.loc[:, ["month", "year", "day"]].drop_duplicates().reset_index(drop=True)
-                x12 = ff_times_df.loc[:, ["month", "year", "day"]].drop_duplicates().reset_index(drop=True)
+                x11 = (
+                    ss.loc[:, ["month", "year", "day"]]
+                    .drop_duplicates()
+                    .reset_index(drop=True)
+                )
+                x12 = (
+                    ff_times_df.loc[:, ["month", "year", "day"]]
+                    .drop_duplicates()
+                    .reset_index(drop=True)
+                )
 
                 if (
                     ss.loc[:, ["month", "year", "day"]]
                     .drop_duplicates()
                     .reset_index(drop=True)
                     .equals(
                         ff_times_df.loc[:, ["month", "year", "day"]]
@@ -300,38 +304,34 @@
                 new = False
                 warnings.warn(f"{nc_str} multi-year daily time series")
 
     if new:
         raise ValueError("Unable to carry out operation given times in datasets!")
 
     if new is False:
-
         # make sure the ff file is not removed from safe list in subsequent
         # actions prior to running
         if (ff is not None) and (session_info["lazy"]):
             append_safe(ff)
             self._safe.append(ff)
 
         if len(self.history) == len(self._hold_history):
-
             for x in self:
-
                 # check that the datasets can actually be worked with
                 if var is None:
                     if (len(nc_variables(ff)) != len(nc_variables(x))) and (
                         len(nc_variables(ff)) != 1
                     ):
                         raise ValueError(
                             "Datasets have incompatible variable numbers for the operation!"
                         )
 
             prior_command = ""
 
         else:
-
             prior_command = self.history[-1].replace("cdo ", " ").replace("  ", " ")
 
         # we need to make sure you can chain multiple adds etc.#
         # the approach below will work, but can probably be improved on
 
         if var is None:
             if "infile09178" in prior_command:
@@ -345,20 +345,18 @@
                 cdo_command = (
                     f"cdo -{method} {prior_command} infile09178 -selname,{var} {ff}"
                 )
 
         # run the command if not lazy
 
         if session_info["lazy"] is False:
-
             new_files = []
             new_commands = []
 
             for FF in self:
-
                 target = temp_file(".nc")
                 the_command = cdo_command.replace("infile09178", FF) + " " + target
                 the_command = tidy_command(the_command)
                 target = run_cdo(the_command, target, precision=self._precision)
                 new_files.append(target)
                 new_commands.append(the_command)
 
@@ -434,19 +432,21 @@
         ff = x
 
     if not isinstance(ff, str):
         raise TypeError("You have not provided an int, float, dataset or file path!")
 
     operation(self=self, method="mul", ff=ff, var=var)
 
+
 __mul__ = multiply
 
+
 def rmse(self, x=None):
     """
-    Calculate the root-mean-square-error of two datasets 
+    Calculate the root-mean-square-error of two datasets
 
     Parameters
     ------------
     x:  DataSet or netCDF file
         This must have an identifical structure to your dataset
 
     ------------
@@ -468,31 +468,29 @@
 
     self.run()
     n_times = len(self.times)
 
     ds1 = self.copy()
     # subtract the data in one dataset from the other
     ds1.subtract(ds2)
-    #square the differences
+    # square the differences
     ds1.power(2)
     # sum up over all time steps
     ds1.tsum()
     # divide by the number of time steps
     ds1.divide(n_times)
-    #square the results
+    # square the results
     ds1.sqrt()
     ds1.run()
 
     self.current = ds1.current
     self.history = ds1.history
     self._hold_history = ds1._hold_history
 
 
-
-
 def subtract(self, x=None, var=None):
     """
     Subtract from a dataset
     This will subtract a constant, another dataset or a netCDF file from the dataset.
 
     Parameters
     ------------
@@ -539,14 +537,15 @@
         ff = x
 
     if not isinstance(ff, str):
         raise TypeError("You have not provided an int, float, dataset or file path!")
 
     operation(self=self, method="sub", ff=ff, var=var)
 
+
 __sub__ = subtract
 
 
 def add(self, x=None, var=None):
     """
     Add to a dataset
     This will add a constant, another dataset or a netCDF file to the dataset.
@@ -599,14 +598,15 @@
         ff = x
 
     if not isinstance(ff, str):
         raise TypeError("You have not provided an int, float, dataset or file path!")
 
     operation(self=self, method="add", ff=ff, var=var)
 
+
 __add__ = add
 
 
 def divide(self, x=None, var=None):
     """
     Divide the data
     This will divide the dataset by a constant, another dataset or a netCDF file.
@@ -656,14 +656,15 @@
         ff = x
 
     if not isinstance(ff, str):
         raise TypeError("You have not provided an int, float, dataset or file path!")
 
     operation(self=self, method="div", ff=ff, var=var)
 
+
 __truediv__ = divide
 
 
 def abs(self):
     """
     Method to get the absolute value of variables
 
@@ -701,14 +702,15 @@
     if not isinstance(x, (int, float)):
         raise TypeError("x is not a float or int")
 
     cdo_command = f"cdo -pow,{x}"
 
     run_this(cdo_command, self, output="ensemble")
 
+
 __pow__ = power
 
 
 def exp(self):
     """
     Method to get the exponential of variables
 
@@ -787,9 +789,7 @@
 
     >>> ds.sqrt()
 
     """
     cdo_command = f"cdo -sqrt"
 
     run_this(cdo_command, self, output="ensemble")
-
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/anomaly.py` & `nctoolkit-0.9.3/nctoolkit/anomaly.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nctoolkit.runthis import run_cdo, tidy_command
 from nctoolkit.show import nc_years
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import remove_safe, session_info
 from nctoolkit.utils import version_below
 
 
-def annual_anomaly(self, baseline=None, metric="absolute", window=1, align = "right"):
+def annual_anomaly(self, baseline=None, metric="absolute", window=1, align="right"):
     """
     Calculate annual anomalies for each variable based on a baseline period
     The anomaly is derived by first calculating the climatological annual mean for the
     given baseline period. Annual means are then calculated for each year and the
     anomaly is calculated compared with the baseline mean. This will be calculated on a
     per-file basis in a multi-file dataset.
 
@@ -125,17 +125,17 @@
                 f"cdo -div -runmean,{window} -yearmean {ff} -timmean "
                 f"-selyear,{baseline[0]}/{baseline[1]} {ff} {target}"
             )
 
         # run the command and save the temp file
 
         cdo_command = tidy_command(cdo_command)
-        cdo_command = cdo_command.replace("cdo ", f"cdo --timestat_date {align} ").replace(
-                    "  ", " "
-                )
+        cdo_command = cdo_command.replace(
+            "cdo ", f"cdo --timestat_date {align} "
+        ).replace("  ", " ")
 
         target = run_cdo(cdo_command, target, precision=self._precision)
 
         # updae the new files and commands
         new_files.append(target)
         new_commands.append(cdo_command)
 
@@ -203,15 +203,14 @@
                     "Variables have different grids. This causes problems with the CDO version installed. Select specific variables before monthly_anomaly or upgrade to CDO>=1.9.10. See npoints in dataset contents to identify differences in grids"
                 )
 
     new_files = []
     new_commands = []
 
     for ff in self:
-
         if len([yy for yy in baseline if yy not in nc_years(ff)]) > 0:
             raise ValueError("Check that the years in baseline are in the dataset!")
         # create the target file
         target = temp_file("nc")
         # create system command
         cdo_command = (
             f"cdo -ymonsub -monmean {ff} -ymonmean -selyear,"
```

### Comparing `nctoolkit-0.9.2/nctoolkit/api.py` & `nctoolkit-0.9.3/nctoolkit/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,20 @@
     return "Warning: " + str(msg) + "\n"
 
 
 warnings.formatwarning = custom_formatwarning
 
 # set up the session info
 letters = string.ascii_lowercase
+try:
+    login = os.getlogin()
+except:
+    login = "" 
 session_info["stamp"] = (
-    "nctoolkit" + "".join(random.choice(letters) for i in range(8)) + "nctoolkit"
+    "nctoolkit_" + login + "_" +   "".join(random.choice(letters) for i in range(8)) + "nctoolkit"
 )
 session_info["temp_dir"] = "/tmp/"
 session_info["user_dir"] = False
 session_info["thread_safe"] = False
 session_info["lazy"] = True
 session_info["precision"] = None
 session_info["parallel"] = False
@@ -118,19 +122,21 @@
 
 def coast_check():
     try:
         import geoviews
         import cartopy
         from cartopy import crs
         import cartopy.crs as ccrs
+
         projection = ccrs.PlateCarree()
         return True
     except:
         return False
 
+
 session_info["coast"] = coast_check()
 
 
 session_info["interactive"] = sys.__stdin__.isatty()
 
 
 if platform.system() == "Linux":
@@ -242,30 +248,28 @@
                                 kwargs[key] + " is not valid session info!"
                             )
         else:
             session_info[key] = kwargs[key]
 
             # update safe-lists etc. if running in parallel
             if kwargs[key] and key == "parallel" and find:
-
                 if len(temp_dirs) > 0:
                     for ff in temp_dirs:
                         append_tempdirs(ff)
 
                 if len(nc_safe) > 0:
                     for ff in nc_safe:
                         nc_safe_par.append(ff)
 
                 if len(nc_protected) > 0:
                     for ff in nc_protected:
                         nc_protected_par.append(ff)
                         nc_protected.remove(ff)
 
             if (kwargs[key] is False) and key == "parallel" and find:
-
                 if len(temp_dirs_par) > 0:
                     for ff in temp_dirs_par:
                         append_tempdirs(ff)
 
                 if len(nc_safe_par) > 0:
                     for ff in nc_safe_par:
                         nc_safe.append(ff)
@@ -377,30 +381,28 @@
                 else:
                     raise ValueError(kwargs[key] + " is not valid session info!")
         else:
             session_info[key] = kwargs[key]
 
             # update safe-lists etc. if running in parallel
             if kwargs[key] and key == "parallel":
-
                 if len(temp_dirs) > 0:
                     for ff in temp_dirs:
                         append_tempdirs(ff)
 
                 if len(nc_safe) > 0:
                     for ff in nc_safe:
                         nc_safe_par.append(ff)
 
                 if len(nc_protected) > 0:
                     for ff in nc_protected:
                         nc_protected_par.append(ff)
                         nc_protected.remove(ff)
 
             if (kwargs[key] is False) and key == "parallel":
-
                 if len(temp_dirs_par) > 0:
                     for ff in temp_dirs_par:
                         append_tempdirs(ff)
 
                 if len(nc_safe_par) > 0:
                     for ff in nc_safe_par:
                         nc_safe.append(ff)
@@ -505,15 +507,14 @@
     """
     if os.path.isfile(file_path):
         file_info = os.stat(file_path)
         return file_info.st_size
 
 
 def from_xarray(ds):
-
     """
     Convert an xarray dataset to an nctoolkit dataset
     This will first save the xarray dataset as a temporary netCDF file.
 
     Parameters
     ---------------
     ds : xarray dataset
@@ -665,17 +666,15 @@
     if wait is not None:
         stop_time = min(wait, stop_time)
     if file_stop is not None:
         stop_time = min(file_stop, stop_time)
 
     if isinstance(x, str):
         if source != "file" or os.path.exists(x) is False:
-
             if is_url(x):
-
                 if thredds is False:
                     new_x = temp_file(".nc")
                     print(f"Downloading {x}")
                     print("\033[A                             \033[A")
 
                     if ftp_details is not None and x.startswith("ftp"):
                         user = ftp_details["user"]
@@ -708,15 +707,14 @@
                             if (end - start) > wait:
                                 break
                     if os.path.exists(new_x) is False:
                         raise ValueError(f"Could not download {x}")
 
                     x = new_x
                 else:
-
                     if checks:
                         if wait is not None:
                             with time_limit(stop_time):
                                 out = subprocess.run(
                                     "cdo sinfo " + x,
                                     shell=True,
                                     stdout=subprocess.PIPE,
@@ -760,25 +758,21 @@
         orig_size = len(x)
         x = list(dict.fromkeys(x))
         if len(x) < orig_size:
             warnings.warn(message="Duplicates in data set have been removed!")
 
     if isinstance(x, list):
         if source == "url":
-
             for ff in x:
-
                 if is_url(ff) is False:
                     raise ValueError(f"{x} is not a url")
 
             new_files = []
             for ff in x:
-
                 if is_url(ff):
-
                     if thredds is False:
                         new_x = temp_file(".nc")
                         print(f"Downloading {ff}")
                         print("\033[A                             \033[A")
 
                         if ftp_details is not None and x.startswith("ftp"):
                             user = ftp_details["user"]
@@ -814,25 +808,23 @@
                             raise ValueError(f"Could not download {x}")
 
                         new_files.append(new_x)
                 x = new_files
 
     if isinstance(x, list) and source != "url":
         if thredds is False:
-
             for ff in x:
                 if os.path.exists(ff) is False:
                     raise FileNotFoundError(f"{ff} does not exist!")
             for ff in x:
                 append_safe(ff)
                 append_protected(ff)
 
             if len(x) > 1:
                 for ff in x:
-
                     if os.path.exists(ff) is False:
                         raise FileNotFoundError("Data set " + ff + " does not exist!")
 
     # if there is only one file in the list, change it to a single file
     if isinstance(x, list):
         if len(x) == 1:
             x = x[0]
@@ -1191,15 +1183,14 @@
 
         self._grid = None
         self._weights = None
         # track number of held over commands
         self._ncommands = 0
 
     def __getitem__(self, index):
-
         return self.current[index]
 
     def __len__(self):
         return len(self.current)
 
     def __iter__(self):
         for ff in self.current:
@@ -1242,15 +1233,14 @@
 
         smallest_file = ""
         largest_file = ""
         min_size = 1e15
         max_size = -1
 
         for ff in self:
-
             all_sizes.append(file_size(ff))
 
             if file_size(ff) > max_size:
                 max_size = file_size(ff)
                 largest_file = ff
 
             if file_size(ff) < min_size:
@@ -1398,28 +1388,26 @@
     def show_contents(self, n=None):
         """
         Detailed list of variables contained in a dataset.
         This will only display the variables in the first file of an ensemble.
         """
 
         try:
-
             if n is None:
                 n = len(self)
 
             list_contents = []
 
             use_names = True
 
             for ff in self:
                 if "nctoolkit" in ff:
                     use_names = False
 
             for ff in self[0:n]:
-
                 dataset = Dataset(ff)
 
                 out = subprocess.run(
                     "cdo sinfon " + ff,
                     shell=True,
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
@@ -1520,15 +1508,14 @@
                     df["unit"] = units
 
                 df = df.assign(nlevels=lambda x: x.nlevels.astype("int")).assign(
                     npoints=lambda x: x.npoints.astype("int")
                 )
 
                 try:
-
                     times = []
 
                     ds = xr.open_dataset(ff, decode_times=False)
                     time_name = [x for x in ds.variables if "time" in x]
 
                     # get time name
 
@@ -1928,10 +1915,7 @@
     from nctoolkit.zip import zip
 
     from nctoolkit.zonals import zonal_mean
     from nctoolkit.zonals import zonal_min
     from nctoolkit.zonals import zonal_max
     from nctoolkit.zonals import zonal_range
     from nctoolkit.zonals import zonal_sum
-
-    # Deprecated methods
-    # from nctoolkit.deprecated import set_missing
```

### Comparing `nctoolkit-0.9.2/nctoolkit/append.py` & `nctoolkit-0.9.3/nctoolkit/append.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,17 +46,15 @@
 
     # check files are not already in the dataset
 
     check_list = self.current
 
     for ff in x:
         if ff in check_list:
-            warnings.warn(
-                "You are trying to add a file that is already in the dataset"
-            )
+            warnings.warn("You are trying to add a file that is already in the dataset")
 
     for ff in x:
         if os.path.exists(ff) is False:
             raise ValueError(f"{ff} does not exist!")
 
     for ff in x:
         append_safe(ff)
```

### Comparing `nctoolkit-0.9.2/nctoolkit/assign.py` & `nctoolkit-0.9.3/nctoolkit/assign.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,24 +93,24 @@
     "ln",
     "sin",
     "cos",
     "tan",
     "int",
     "float",
     "log10",
-    "thickness"
+    "thickness",
 ]
 
 translation = dict()
 for ff in funs:
     if ff in dir(np):
         translation[ff] = ff
 
 translation["int"] = "int"
-#translation["deltaz"] = "cdeltaz"
+# translation["deltaz"] = "cdeltaz"
 translation["float"] = "float"
 
 translation["arcsin"] = "asin"
 translation["arccos"] = "acos"
 translation["arctan"] = "atan"
 
 # translate the spatials
@@ -150,14 +150,15 @@
 
 translation["lon"] = "clon"
 translation["lat"] = "clat"
 
 translation["longitude"] = "clon"
 translation["latitude"] = "clat"
 
+
 # split using all possible mathematical operators
 def split1(mystr):
     return re.split("([+-/*()<>=])", mystr)
 
 
 def is_lambda(v):
     LAMBDA = lambda: 0
@@ -223,15 +224,14 @@
             all_str = list(inspect.getsourcelines(start))[0]
             all_str = "".join(all_str)
             start = all_str.replace("'", "").replace("\\n", "")[1:-1].replace("  ", " ")
             start = start.replace("\n", "")
         except:
             start = dill.source.getsource(start).replace("\n", "").strip()
     except:
-
         if interactive:
             import readline
 
             start = [
                 str(readline.get_history_item(i + 1))
                 for i in range(readline.get_current_history_length())
             ]
@@ -328,15 +328,14 @@
         starts = starts.replace(".match_points(", ".assign(")
 
     starts = starts.split(";")
     starts = [x for x in starts if ("lambda" in x) or ("drop" in x)]
     starts = ("; ").join(starts)
 
     for start in starts.split(";"):
-
         patternl = re.compile("lambda \w*:")
         lambda_value = patternl.findall(start)[0][-2]
 
         start = (
             " ".join(split1(start))
             .replace("  ", " ")
             .replace(" ( ", "(")
@@ -383,15 +382,14 @@
 
         start = start.replace(" [", "[").replace("(", "( ").replace(" . ", ".")
 
         # pattern to identify functions
         fun_pattern = re.compile("[a-zA-Z\_][a-zA-Z\_z.0-9]*\(")
 
         for x in fun_pattern.findall(start):
-
             check = True
             while check:
                 x_terms = re.finditer(x.replace("(", "\\(").replace("[", "\\["), start)
 
                 terminate = len(
                     re.findall(x.replace("(", "\\(").replace("[", "\\["), start)
                 )
@@ -431,15 +429,14 @@
                 ]
             )
         )
 
         for x in terms:
             if ("[" in x and f"{lambda_value}." in x) is False:
                 if fun_pattern.search(x) is not None:
-
                     fix = True
                     n = 0
                     n_limit = start.count("x")
                     while fix:
                         for y in re.finditer(
                             x.replace("(", "\\(").replace("[", "\\["), start
                         ):
@@ -501,15 +498,14 @@
                                 new_start += " " + y
                             else:
                                 new_start += " " + str(new_x)
                         start = new_start
                         error_message = None
 
                     except:
-
                         if x_fun in translation.keys():
                             x_term = between_brackets(x)
                             if (f"{lambda_value}." in x_term) is False:
                                 if x_fun not in ["timestep"]:
                                     raise ValueError(
                                         f"Error for {x}: nctoolkit functions must take dataset variables as args!"
                                     )
@@ -667,15 +663,14 @@
 
         new_start = []
 
         def new_split(mystr):
             return re.split("([+-/*()&|<>=!^])", mystr)
 
         for tt in start.split(";"):
-
             tt_frag = []
             l_pattern = re.compile("lambda (\w*):")
             l_string = l_pattern.findall(tt)[0]
             tt1 = tt.replace(f"lambda {l_string}:", " ")
             tt1 = re.sub(" ", "", tt1)
             tt1 = " ".join(new_split(tt1)).replace(" . ", ".")
             tt1 = re.sub(" +", " ", tt1)
@@ -726,15 +721,14 @@
 
     def split_this(mystr):
         return re.split("([+-/*()<>|&=])", mystr)
 
     command = " ".join(split_this(command)).replace(" . ", ".").replace(";", " ; ")
 
     for term in command.split(" "):
-
         if "." in term:
             pattern1 = re.compile(r"[a-zA-Z]")
             if len(pattern1.findall(term)) > 0 and "^" not in term:
                 if term.split(".")[0] in frame.f_back.f_locals:
                     try:
                         new_term = eval(term, globals(), frame.f_back.f_locals)
                         if isinstance(new_term, str):
```

### Comparing `nctoolkit-0.9.2/nctoolkit/cdo_command.py` & `nctoolkit-0.9.3/nctoolkit/cdo_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,12 +44,11 @@
     cdo_command = "cdo " + command + " "
 
     if ("merge " in cdo_command) or ("mergetime " in cdo_command) or ensemble:
         output = "one"
         self._merged = True
 
     for mm in cdo_methods:
-
         if " " + mm + "," in cdo_command:
             cdo_command = cdo_command.replace(" " + mm + ",", " -" + mm + ",")
 
     run_this(cdo_command, self, output=output)
```

### Comparing `nctoolkit-0.9.2/nctoolkit/cellareas.py` & `nctoolkit-0.9.3/nctoolkit/cellareas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 
 from nctoolkit.cleanup import cleanup
-from nctoolkit.session import remove_safe, session_info
+from nctoolkit.session import remove_safe
 from nctoolkit.runthis import run_this, tidy_command, run_cdo
 from nctoolkit.show import nc_variables
 from nctoolkit.temp_file import temp_file
 
 
 def cell_area(self, join=True):
     """
@@ -38,20 +38,18 @@
 
     # release if you need to join the cell areas to the original file
     if join:
         self.run()
 
     # first run the join case
     if join:
-
         new_files = []
         new_commands = []
 
         for ff in self:
-
             if "cell_area" in nc_variables(ff):
                 raise ValueError("cell_area is already a variable")
 
             target = temp_file(".nc")
 
             cdo_command = f"cdo -merge {ff} -gridarea {ff} {target}"
             cdo_command = tidy_command(cdo_command)
@@ -70,15 +68,14 @@
             remove_safe(ff)
 
         self._hold_history = copy.deepcopy(self.history)
 
         cleanup()
 
     else:
-
         cdo_command = "cdo -gridarea"
         run_this(cdo_command, self, output="ensemble")
 
     # add units
 
     self.set_units({"cell_area": "m^2"})
```

### Comparing `nctoolkit-0.9.2/nctoolkit/centres.py` & `nctoolkit-0.9.3/nctoolkit/centres.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 def centre(self, by="latitude", by_area=False):
     """
     Calculate the latitudinal or longitudinal centre for each year/month combination in files.
     This applies to each file in an ensemble.
 
     Parameters
     -------------
```

### Comparing `nctoolkit-0.9.2/nctoolkit/checks.py` & `nctoolkit-0.9.3/nctoolkit/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import xarray as xr
 from nctoolkit.temp_file import temp_file
-from nctoolkit.api import open_data
 from netCDF4 import Dataset
 import subprocess
 import warnings
 
+
 def is_corrupt(self):
     """
-    Check if files are corrupt 
+    Check if files are corrupt
     """
 
     for ff in self:
-
         the_temp = temp_file() + "nc"
         command = f"cdo -copy {ff}  {the_temp}"
         out = subprocess.Popen(
             command,
             shell=True,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
@@ -26,15 +25,14 @@
             print(f"{ff} appears to be corrupt")
             return True
         else:
             blash = None
     return False
 
 
-
 def check(self):
     """
     Check contents of files for common data problems.
     """
 
     print("*****************************************")
     print("Checking data types")
@@ -70,29 +68,29 @@
         for ff in self:
             dataset = Dataset(ff)
             times = [x for x in dataset.variables.keys() if "time" in x]
             if len(times) > 0:
                 for tt in times:
                     time_var = dataset.variables[tt][:]
                     if "int" in str(time_var.dtype):
-                        the_warns.append(f"{tt} has integer data type. Consider setting it to double using as_double")
-
+                        the_warns.append(
+                            f"{tt} has integer data type. Consider setting it to double using as_double"
+                        )
 
         if len(the_warns) > 0:
             the_warns = list(set(the_warns))
             for tt in the_warns:
                 print(tt)
     except:
         print("Unable to check data types. This file is likely not CF-compliant")
 
     print("*****************************************")
     print("Running CF-compliance checks")
     print("*****************************************")
 
-
     cf_checker = True
     try:
         import cfchecker
     except:
         cf_checker = False
         print(
             "cfchecker is not available. Run 'pip install cfchecker' to check files for CF-compliance!"
@@ -105,15 +103,17 @@
                 try:
                     ds = xr.open_dataset(ff, decode_times=False)
                     if "Conventions" not in list(ds.attrs.keys()):
                         print(f"No CF-conventions in {ff}")
                     else:
                         version = ds.attrs["Conventions"].split("-")[1]
                 except:
-                    warnings.warn("Note: there are issues opening this file using xarray. You may want to look closely to see if there are formatting issues that will have negative downstream impacts!")
+                    warnings.warn(
+                        "Note: there are issues opening this file using xarray. You may want to look closely to see if there are formatting issues that will have negative downstream impacts!"
+                    )
 
                 if len(version) > 0:
                     command = f"cfchecks -v {version} {ff}"
                 else:
                     command = f"cfchecks {ff}"
 
                 out = subprocess.Popen(
@@ -134,15 +134,14 @@
                 end = [
                     index
                     for index, value in enumerate(result_split)
                     if "ERRORS dete" in value
                 ][0]
                 for i in range(0, len(splits)):
                     if i < (len(splits) - 1):
-
                         i_result = result_split[splits[i] : splits[i + 1]]
                         i_result = "\n".join(i_result)
                         if "ERROR: " in i_result:
                             i_result = i_result.replace(
                                 "Checking variable:", "Issue with variable:"
                             )
                             print(i_result)
@@ -151,15 +150,17 @@
                         i_result = "\n".join(i_result)
                         if "ERROR: " in i_result:
                             i_result = i_result.replace(
                                 "Checking variable:", "Issue with variable:"
                             )
                             print(i_result)
         except:
-            warnings.warn("Problem running CF-compliance checks. Have a look at the cfchecker installation")
+            warnings.warn(
+                "Problem running CF-compliance checks. Have a look at the cfchecker installation"
+            )
 
     print("*****************************************")
     print("Checking grid consistency")
     print("*****************************************")
 
     try:
         for ff in self:
```

### Comparing `nctoolkit-0.9.2/nctoolkit/cleanup.py` & `nctoolkit-0.9.3/nctoolkit/cleanup.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,24 +58,17 @@
     # the files to be deleted are in the temporary folder
 
     delete_these = [x for x in delete_these if os.path.exists(x)]
 
     if len(delete_these) == 0:
         return None
 
-    # ignore stuff less than a minute old...
-
-    if session_info["parallel"]:
-        for dd in delete_these:
-            if os.path.exists(dd) and file_age_in_seconds(dd) > 60:
-                nc_remove(dd)
-    else:
-        for dd in delete_these:
-            if os.path.exists(dd):
-                nc_remove(dd)
+    for dd in delete_these:
+        if os.path.exists(dd):
+            nc_remove(dd)
 
     # only update the session size on linux
 
     if session_info["user_dir"] is False:
         if platform.system() == "Linux":
             result = os.statvfs("/tmp/")
             result = result.f_frsize * result.f_bavail
@@ -158,15 +151,14 @@
             else:
                 print(
                     f"{len(mylist)} files were created by nctoolkit in prior or current"
                     f" sessions. Consider running deep_clean!"
                 )
 
     else:
-
         temp_folder = tempfile.gettempdir()
 
         mylist = [f for f in glob.glob(f"{temp_folder}/*")]
         mylist = [f for f in mylist if "nctoolkit" in f]
 
         if len(mylist) > 0:
             if len(mylist) == 1:
@@ -187,15 +179,14 @@
     """
 
     if session_info["user_dir"]:
         return None
 
     # only use this on linux
     if platform.system() == "Linux":
-
         # get files as a list
 
         ff_list = self.current
 
         # First step is to figure out how much space is in /tmp
         # Do nothing if it is less than 0.5 GB
```

### Comparing `nctoolkit-0.9.2/nctoolkit/clear.py` & `nctoolkit-0.9.3/nctoolkit/clear.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import os
 import warnings
 
+
 def reset(self):
     """
     Simple method to fully reset a datset
 
     """
 
     self.current = self._start
-    self._execute =  False
-    self._history =  []
+    self._execute = False
+    self._history = []
     self._hold_history = []
     self._merged = False
-    self_safe =  []
+    self_safe = []
     if os.path.exists(self[0]):
         self._thredds = False
     else:
         self._thredds = True
-    self_zip =  False
-    self_format =  None
-    self._precision =  'default'
-    self._grid =  None
-    self._weights =  None
-    self._ncommands =  0
-    warnings.warn("The dataset has been reset to the starting point due to a run failure! Please change commands, where applicable, and re-run.")
-
-
+    self_zip = False
+    self_format = None
+    self._precision = "default"
+    self._grid = None
+    self._weights = None
+    self._ncommands = 0
+    warnings.warn(
+        "The dataset has been reset to the starting point due to a run failure! Please change commands, where applicable, and re-run."
+    )
```

### Comparing `nctoolkit-0.9.2/nctoolkit/compare.py` & `nctoolkit-0.9.3/nctoolkit/compare.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,109 +1,147 @@
 from nctoolkit.runthis import run_this
 
+
 def is_integer(x):
     try:
         y = int(str(x))
         return True
     except:
         return False
 
+
 def fix_expr(expression):
     """
     Function to to convert operations to something cdo can handle
     """
 
     expression = expression.replace(" ", "")
 
     # equal constant case
     if expression.startswith("==-"):
-        if expression.replace("==-", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace("==-", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace("==", "eqc")
         expression = expression.replace("eqc", "eqc,")
         return expression
     # equal constant case
     if expression.startswith("=="):
-        if expression.replace("==", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace("==", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace("==", "eqc")
         expression = expression.replace("eqc", "eqc,")
         return expression
 
     # not equal constant case
     if expression.startswith("!=-"):
-        if expression.replace("!=-", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace("!=-", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace("!=", "nec")
         expression = expression.replace("nec", "nec,")
         return expression
     # not equal constant case
     if expression.startswith("!="):
-        if expression.replace("!=", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace("!=", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace("!=", "nec")
         expression = expression.replace("nec", "nec,")
         return expression
 
     # less than or equal to constant case
     if expression.startswith("<=-"):
-        if expression.replace("<=-", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace("<=-", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace("<=", "lec")
         expression = expression.replace("lec", "lec,")
         return expression
 
     # less than or equal to constant case
     if expression.startswith("<="):
-        if expression.replace("<=", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace("<=", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace("<=", "lec")
         expression = expression.replace("lec", "lec,")
         return expression
 
     # less than or equal to constant case
     if expression.startswith("<-"):
-        if expression.replace("<-", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace("<-", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace("<", "ltc")
         expression = expression.replace("ltc", "ltc,")
         return expression
     # less than or equal to constant case
     if expression.startswith("<"):
-        if expression.replace("<", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace("<", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace("<", "ltc")
         expression = expression.replace("ltc", "ltc,")
         return expression
 
     # greater than or equal to constant case
     if expression.startswith(">=-"):
-        if expression.replace(">=-", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace(">=-", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace(">=", "gec")
         expression = expression.replace("gec", "gec,")
         return expression
 
     if expression.startswith(">="):
-        if expression.replace(">=", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace(">=", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace(">=", "gec")
         expression = expression.replace("gec", "gec,")
         return expression
 
     # greater than or equal to constant case
     if expression.startswith(">-"):
-        if expression.replace(">-", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace(">-", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace(">", "gtc")
         expression = expression.replace("gtc", "gtc,")
         return expression
 
     if expression.startswith(">"):
-        if expression.replace(">", "").replace(".", "", 1).replace("e", "").isdigit() is False:
+        if (
+            expression.replace(">", "").replace(".", "", 1).replace("e", "").isdigit()
+            is False
+        ):
             raise ValueError(expression + " is not valid!")
         expression = expression.replace(">", "gtc")
         expression = expression.replace("gtc", "gtc,")
         return expression
 
     raise ValueError(expression + " is not valid!")
 
@@ -141,93 +179,88 @@
 
     expression = fix_expr(expression)
     cdo_command = f"cdo -{expression}"
     run_this(cdo_command, self, output="ensemble")
 
 
 def __eq__(self, x):
-
     if not isinstance(x, str):
         try:
             test = float(x)
             x_new = x
             if not is_integer(x):
                 x_new = str(float(x)).replace("+", "")
             self.compare(f"=={x_new}")
         except:
             self.eq(x)
     else:
         self.eq(x)
 
 
 def __gt__(self, x):
-
     if not isinstance(x, str):
         try:
             test = float(x)
             x_new = x
             if not is_integer(x):
                 x_new = str(float(x)).replace("+", "")
             self.compare(f">{x_new}")
         except:
             self.gt(x)
     else:
         self.gt(x)
 
-def __lt__(self, x):
 
+def __lt__(self, x):
     if not isinstance(x, str):
         try:
             test = float(x)
             x_new = x
             if not is_integer(x):
                 x_new = str(float(x)).replace("+", "")
             self.compare(f"<{x_new}")
         except:
             self.lt(x)
     else:
         self.lt(x)
 
-def __le__(self, x):
 
+def __le__(self, x):
     if not isinstance(x, str):
         try:
             test = float(x)
             x_new = x
             if not is_integer(x):
                 x_new = str(float(x)).replace("+", "")
             self.compare(f"<={x_new}")
         except:
             self.le(x)
     else:
         self.le(x)
 
 
 def __ge__(self, x):
-
     if not isinstance(x, str):
         try:
             test = float(x)
             x_new = x
             if not is_integer(x):
                 x_new = str(float(x)).replace("+", "")
             self.compare(f">={x_new}")
         except:
             self.ge(x)
     else:
         self.ge(x)
 
-def __ne__(self, x):
 
+def __ne__(self, x):
     if not isinstance(x, str):
         try:
             test = float(x)
             x_new = x
             if not is_integer(x):
                 x_new = str(float(x)).replace("+", "")
             self.compare(f"!={x_new}")
         except:
             self.ne(x)
     else:
         self.ne(x)
-
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/compare_data.py` & `nctoolkit-0.9.3/nctoolkit/compare_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from nctoolkit.temp_file import temp_file
 from nctoolkit.runthis import run_cdo
 from nctoolkit.session import remove_safe
 from nctoolkit.cleanup import cleanup
-import nctoolkit.api as api 
+import nctoolkit.api as api
 import os
 
+
 def ne(self, x):
     """
     Method to calculate if variable in dataset is not equal to that in another file or dataset
     This currently only works with single file datasets
 
     Parameters
     -------------
@@ -38,15 +39,14 @@
     if x_ff is None:
         raise ValueError("x needs to be a file path or nctoolkit dataset")
 
     if os.path.exists(x_ff) is False:
         raise ValueError(f"{x_ff} does not exist!")
 
     for ff in self:
-
         temp = temp_file(".nc")
 
         cdo_command = f"cdo -ne {ff} {x_ff} {temp}"
 
         target = run_cdo(cdo_command, temp, precision=self._precision)
         new_files.append(target)
 
@@ -56,14 +56,15 @@
     self.current = new_files
 
     for ff in new_files:
         remove_safe(ff)
 
     cleanup()
 
+
 def ge(self, x):
     """
     Method to calculate if variable in dataset is greater than or equal to that in another file or dataset
     This currently only works with single file datasets
 
     Parameters
     -------------
@@ -93,15 +94,14 @@
     if x_ff is None:
         raise ValueError("x needs to be a file path or nctoolkit dataset")
 
     if os.path.exists(x_ff) is False:
         raise ValueError(f"{x_ff} does not exist!")
 
     for ff in self:
-
         temp = temp_file(".nc")
 
         cdo_command = f"cdo -ge {ff} {x_ff} {temp}"
 
         target = run_cdo(cdo_command, temp, precision=self._precision)
         new_files.append(target)
 
@@ -111,14 +111,15 @@
     self.current = new_files
 
     for ff in new_files:
         remove_safe(ff)
 
     cleanup()
 
+
 def le(self, x):
     """
     Method to calculate if variable in dataset is less than or equal to that in another file or dataset
     This currently only works with single file datasets
 
     Parameters
     -------------
@@ -148,15 +149,14 @@
     if x_ff is None:
         raise ValueError("x needs to be a file path or nctoolkit dataset")
 
     if os.path.exists(x_ff) is False:
         raise ValueError(f"{x_ff} does not exist!")
 
     for ff in self:
-
         temp = temp_file(".nc")
 
         cdo_command = f"cdo -le {ff} {x_ff} {temp}"
 
         target = run_cdo(cdo_command, temp, precision=self._precision)
         new_files.append(target)
 
@@ -204,15 +204,14 @@
     if x_ff is None:
         raise ValueError("x needs to be a file path or nctoolkit dataset")
 
     if os.path.exists(x_ff) is False:
         raise ValueError(f"{x_ff} does not exist!")
 
     for ff in self:
-
         temp = temp_file(".nc")
 
         cdo_command = f"cdo -lt {ff} {x_ff} {temp}"
 
         target = run_cdo(cdo_command, temp, precision=self._precision)
         new_files.append(target)
 
@@ -259,17 +258,15 @@
 
     if x_ff is None:
         raise ValueError("ff needs to be a file path or nctoolkit dataset")
 
     if os.path.exists(x_ff) is False:
         raise ValueError(f"{x_ff} does not exist!")
 
-
     for ff in self:
-
         temp = temp_file(".nc")
 
         cdo_command = f"cdo -gt {ff} {x_ff} {temp}"
 
         target = run_cdo(cdo_command, temp, precision=self._precision)
         new_files.append(target)
 
@@ -279,14 +276,15 @@
     self.current = new_files
 
     for ff in new_files:
         remove_safe(ff)
 
     cleanup()
 
+
 def eq(self, x):
     """
     Method to calculate if variable in dataset is equal to that in another file or dataset
     This currently only works with single file datasets
 
     Parameters
     -------------
@@ -316,15 +314,14 @@
     if x_ff is None:
         raise ValueError("x needs to be a file path or nctoolkit dataset")
 
     if os.path.exists(x_ff) is False:
         raise ValueError(f"{x_ff} does not exist!")
 
     for ff in self:
-
         temp = temp_file(".nc")
 
         cdo_command = f"cdo -eq {ff} {x_ff} {temp}"
 
         target = run_cdo(cdo_command, temp, precision=self._precision)
         new_files.append(target)
 
@@ -333,8 +330,7 @@
 
     self.current = new_files
 
     for ff in new_files:
         remove_safe(ff)
 
     cleanup()
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/corr.py` & `nctoolkit-0.9.3/nctoolkit/corr.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from nctoolkit.runthis import run_cdo, tidy_command
 from nctoolkit.show import nc_variables
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import remove_safe, get_safe
 
 
 def cor(self, var1=None, var2=None, method="fld"):
-
     if len(self) == 0:
         raise ValueError("Failure due to empty dataset!")
 
     # Make sure variables are given
     if (var1 is None) or (var2 is None):
         raise ValueError("Both variables are not given")
 
@@ -32,35 +31,35 @@
             raise ValueError(f"{var1} is not in the dataset")
 
         if var2 not in nc_variables(ff):
             raise ValueError(f"{var2} is not in the dataset")
 
     if var1 != var2:
         contents = self.contents
-        df = contents.query("variable in [@var1, @var2]").loc[:,["variable", "data_type"]]
+        df = contents.query("variable in [@var1, @var2]").loc[
+            :, ["variable", "data_type"]
+        ]
         # if
         if len([x for x in df.index if "file" in str(x)]) == 0:
             df.index = ["file" for x in range(len(df.index))]
         df = (
-            df
-            .pivot(values = "data_type", columns = "variable")
-            .rename(columns = {var1:"var1"})
-            .rename(columns = {var2:"var2"})
+            df.pivot(values="data_type", columns="variable")
+            .rename(columns={var1: "var1"})
+            .rename(columns={var2: "var2"})
         )
         if len(df.query("var1 != var2")) > 0:
-            raise ValueError(f"{var1} and {var2} have different data types. Please select data type with set_precision. Suggestion: F32.")
-
-
+            raise ValueError(
+                f"{var1} and {var2} have different data types. Please select data type with set_precision. Suggestion: F32."
+            )
 
     # Calculate the correlations in each file
     new_files = []
     new_commands = []
 
     for ff in self:
-
         # create the temp file for targeting
         target = temp_file(".nc")
 
         # create the cdo command and run it
 
         cdo_command = (
             f"cdo -{method}cor -selname,{var1} {ff} -selname,{var2} {ff} {target}"
```

### Comparing `nctoolkit-0.9.2/nctoolkit/create_ensemble.py` & `nctoolkit-0.9.3/nctoolkit/create_ensemble.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/crop.py` & `nctoolkit-0.9.3/nctoolkit/crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     if nco:
         self.run()
 
     if isinstance(nco_vars, str):
         nco_vars = [nco_vars]
 
     # check validity of lon/lat supplied
-    if not isinstance(lon, list) or  not isinstance(lat, list):
+    if not isinstance(lon, list) or not isinstance(lat, list):
         raise TypeError("Check that lon/lat ranges are tuples")
 
     if len(lon) != 2:
         raise ValueError("lon is a list of more than 2 variables")
 
     if len(lat) != 2:
         raise ValueError("lat is a list of more than 2 variables")
@@ -93,19 +93,17 @@
         else:
             raise ValueError("The lonlat box supplied is not valid!")
 
     new_files = []
     new_commands = []
 
     for ff in self:
-
         # find the names of lonlat
 
         if nco_vars is not None:
-
             var_str = f" -v {str_flatten(nco_vars)}"
         else:
             var_str = " "
 
         out = subprocess.run(
             f"cdo griddes {ff}",
             shell=True,
```

### Comparing `nctoolkit-0.9.2/nctoolkit/distgrid.py` & `nctoolkit-0.9.3/nctoolkit/distgrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     new_files = []
 
     commands = []
 
     bases = []
 
     for ff in self:
-
         # We need to split the file by name
         # But, first we need to check if there is space in the output folder
         # If there isn't, we need to switch to the /var/tmp
 
         if platform.system() == "Linux":
             if session_info["temp_dir"] == "/tmp/":
                 result = os.statvfs("/tmp/")
```

### Comparing `nctoolkit-0.9.2/nctoolkit/drop.py` & `nctoolkit-0.9.3/nctoolkit/drop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from nctoolkit.flatten import str_flatten
 from nctoolkit.runthis import run_this
 
+
 def fix_ind(x):
     if x < 0:
         return x
     else:
         return x + 1
 
+
 def drop(self, **kwargs):
     """
     Remove variables
     This will remove stated variables from files in the dataset.
 
     Parameters
     -------------
@@ -73,15 +75,14 @@
             if not isinstance(vars, list):
                 vars = [vars]
 
             for vv in vars:
                 if not isinstance(vv, int):
                     raise TypeError(f"{vv} is not an int")
 
-
             vars = [fix_ind(x) for x in vars]
             vars = str_flatten(vars, ",")
 
             # create the cdo command and run it
             cdo_command = f"cdo -delete,timestep={vars}"
             run_this(cdo_command, self, output="ensemble")
```

### Comparing `nctoolkit-0.9.2/nctoolkit/ensembles.py` & `nctoolkit-0.9.3/nctoolkit/ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,14 @@
     ignore_time : boolean
         If True the mean is calculated over all time steps. If False, the ensemble mean
         is calculated for each time steps; for example, if the ensemble is made up of
         monthly files the mean for each month will be calculated.
     """
 
     if nco is False:
-
         self.run()
 
         if len(self) == 1:
             warnings.warn(message="There is only one file in the dataset")
 
         if ignore_time is False:
             cdo_command = "cdo --sortname -ensmean"
```

### Comparing `nctoolkit-0.9.2/nctoolkit/esoteric.py` & `nctoolkit-0.9.3/nctoolkit/esoteric.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,65 +5,75 @@
 
 from .temp_file import temp_file
 from .cleanup import cleanup
 from .runthis import run_this
 from .runthis import run_nco
 from .api import open_data
 
+
 def fix_nemo_ersem_grid(self):
     """
     A quick hack to change the grid file in North West European shelf Nemo grids.
 
     """
 
     ds = open_data(self[0])
 
     lon_name = [x for x in ds.to_xarray().coords if "lon" in x][0]
     lat_name = [x for x in ds.to_xarray().coords if "lat" in x][0]
     lons = ds.to_xarray()[lon_name].values.flatten()
-    if len(set(list(pd.DataFrame({"lon":lons}).groupby("lon").size().sort_values()))) == 1:
+    if (
+        len(set(list(pd.DataFrame({"lon": lons}).groupby("lon").size().sort_values())))
+        == 1
+    ):
         raise ValueError("There appears to be nothing to fix!")
-    lons =  list(set(lons))
-    
+    lons = list(set(lons))
+
     for i in range(1, len(lons)):
-        if np.round(lons[i] - lons[i-1], 5) == np.round(lons[i+1] - lons[i], 5):
+        if np.round(lons[i] - lons[i - 1], 5) == np.round(lons[i + 1] - lons[i], 5):
             break
-    xinc = np.round(lons[i] - lons[i-1], 5)
-    
+    xinc = np.round(lons[i] - lons[i - 1], 5)
+
     lats = ds.to_xarray()[lat_name].values.flatten()
-    lats =  list(set(lats))
-    
+    lats = list(set(lats))
+
     for i in range(1, len(lats)):
-        if np.round(lats[i] - lats[i-1], 5) == np.round(lats[i+1] - lats[i], 5):
+        if np.round(lats[i] - lats[i - 1], 5) == np.round(lats[i + 1] - lats[i], 5):
             break
-    yinc = np.round(lats[i] - lats[i-1], 5)
+    yinc = np.round(lats[i] - lats[i - 1], 5)
     grid_file = temp_file().replace(".", "")
     ysize = ds.to_xarray()[lon_name].shape[0]
     xsize = ds.to_xarray()[lat_name].shape[1]
     xfirst = min(lons)
     lats = ds.to_xarray()[lat_name].values.flatten()
-    yfirst = min(pd.DataFrame({"lat":lats}).groupby("lat").size().sort_values().reset_index()["lat"][0:-1])
-    with open(grid_file, 'a') as file:
-        file.write('#\n')
-        file.write('# gridID 1\n')
-        file.write('#\n')
-        file.write('gridtype = lonlat\n')
-        file.write(f'gridsize = {xsize*ysize}\n')
-        file.write(f'xsize = {xsize}\n')
-        file.write(f'ysize = {ysize}\n')
-        file.write('xname = lon\n')
-        file.write('xlongname= longitude\n')
-        file.write('xunits= degrees_east\n')
-        file.write('yname = lat\n')
-        file.write('ylongname= latitude\n')
-        file.write('yunits= degrees_north\n')
-        file.write(f'xfirst= {xfirst}\n')
-        file.write(f'xinc= {xinc}\n')
-        file.write(f'yfirst= {yfirst}\n')
-        file.write(f'yinc= {yinc}\n')
+    yfirst = min(
+        pd.DataFrame({"lat": lats})
+        .groupby("lat")
+        .size()
+        .sort_values()
+        .reset_index()["lat"][0:-1]
+    )
+    with open(grid_file, "a") as file:
+        file.write("#\n")
+        file.write("# gridID 1\n")
+        file.write("#\n")
+        file.write("gridtype = lonlat\n")
+        file.write(f"gridsize = {xsize*ysize}\n")
+        file.write(f"xsize = {xsize}\n")
+        file.write(f"ysize = {ysize}\n")
+        file.write("xname = lon\n")
+        file.write("xlongname= longitude\n")
+        file.write("xunits= degrees_east\n")
+        file.write("yname = lat\n")
+        file.write("ylongname= latitude\n")
+        file.write("yunits= degrees_north\n")
+        file.write(f"xfirst= {xfirst}\n")
+        file.write(f"xinc= {xinc}\n")
+        file.write(f"yfirst= {yfirst}\n")
+        file.write(f"yinc= {yinc}\n")
     self.cdo_command(f"setgrid,{grid_file}")
     self.run()
 
 
 def no_leaps(self):
     """
     Remove leap years.
@@ -101,15 +111,15 @@
         raise ValueError("Grid type supplies is not supported")
 
     cdo_command = f"cdo -setgridtype,{grid}"
 
     run_this(cdo_command, self, output="ensemble")
 
 
-def assign_coords(self, lon_name=None, lat_name=None, time_name = None):
+def assign_coords(self, lon_name=None, lat_name=None, time_name=None):
     """
     Assign coordinates to variables
 
     Parameters
     -------------
     lon_name : str
         Name of the longitude dimension
@@ -160,17 +170,15 @@
         self.history.append(nco_command)
         self._hold_history = copy.deepcopy(self.history)
 
     if time_name is not None:
         nco_command = "ncatted "
 
         for vv in self.variables:
-            nco_command += (
-                "-a coordinates," + vv + ",c,c,'" + time_name + " ' "
-            )
+            nco_command += "-a coordinates," + vv + ",c,c,'" + time_name + " ' "
 
         target = temp_file("nc")
 
         nco_command += self[0] + " " + target
 
         target = run_nco(nco_command, target)
 
@@ -307,15 +315,14 @@
 
     for xx in x.keys():
         if x[xx] == "float32":
             x[xx] = "float"
         if x[xx] == "float64":
             x[xx] = "double"
 
-
     the_command = ""
     for xx in x:
         the_command += f" -s '{xx}={x[xx]}({xx})'"
 
     self.nco_command(f"ncap2 {the_command}")
 
 
@@ -340,10 +347,7 @@
 
     for xx in x:
         if not isinstance(xx, str):
             raise ValueError("Please provide a list of strings to as_double")
 
     for xx in x:
         self.nco_command(f"ncap2 -s '{xx}=double({xx})'")
-
-
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/fldstat.py` & `nctoolkit-0.9.3/nctoolkit/fldstat.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import remove_safe
 
 
 def boxstat(self, stat="mean", x=1, y=1):
     """Method to calculate the spatial stat from a dataset"""
 
-
     if not isinstance(x, int):
         raise ValueError("x should be int")
     if not isinstance(y, int):
         raise ValueError("y should be int")
 
     if x <= 0:
         raise ValueError("x should be positive")
@@ -249,30 +248,28 @@
     if len(self) == 0:
         raise ValueError("Failure due to empty dataset!")
 
     if isinstance(by_area, bool) is False:
         raise TypeError("by_area is not boolean")
 
     if len(self) == 1 or (by_area is False):
-
         if by_area:
             self.run()
 
             cdo_command = f"cdo -fldsum -mul {self.current[0]} -gridarea "
         else:
             cdo_command = "cdo -fldsum"
 
         run_this(cdo_command, self, output="ensemble")
 
         return None
 
     new_files = []
     new_commands = []
     for ff in self:
-
         target = temp_file("nc")
 
         cdo_command = f"cdo -fldsum -mul {ff} -gridarea {ff} {target}"
         cdo_command = tidy_command(cdo_command)
         target = run_cdo(cdo_command, target=target, precision=self._precision)
         new_files.append(target)
         new_commands.append(cdo_command)
```

### Comparing `nctoolkit-0.9.2/nctoolkit/format.py` & `nctoolkit-0.9.3/nctoolkit/format.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/generate_grid.py` & `nctoolkit-0.9.3/nctoolkit/generate_grid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/inttime.py` & `nctoolkit-0.9.3/nctoolkit/inttime.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/masking.py` & `nctoolkit-0.9.3/nctoolkit/masking.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     -------------
     lon : list
         Longitude range to mask. Must be of the form: [lon_min, lon_max]
     lat : list
         Latitude range to mask. Must be of the form: [lat_min, lat_max]
     """
 
-    if not isinstance(lon, list) or  not isinstance(lat, list):
+    if not isinstance(lon, list) or not isinstance(lat, list):
         raise TypeError("Check that lon/lat ranges are tuples")
 
     if len(lon) != 2:
         raise ValueError("lon is a list of more than 2 variables")
 
     if len(lat) != 2:
         raise ValueError("lat is a list of more than 2 variables")
@@ -41,13 +41,12 @@
         raise ValueError("Check lat order")
     if lon[1] < lon[0]:
         raise ValueError("Check lon order")
 
     # now, clip to the lonlat box we need
 
     if (lon[0] >= -180) and (lon[1] <= 180) and (lat[0] >= -90) and (lat[1] <= 90):
-
         lat_box = str_flatten(lon + lat)
         cdo_command = f"cdo -masklonlatbox,{lat_box}"
         run_this(cdo_command, self, output="ensemble")
     else:
         raise ValueError("The lonlat box supplied is not valid!")
```

### Comparing `nctoolkit-0.9.2/nctoolkit/matchpoint.py` & `nctoolkit-0.9.3/nctoolkit/matchpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-
-
 def open_matchpoint():
-
     return Matchpoint()
 
 
 class Matchpoint(object):
     """
     A modifiable ensemble of netCDF files
     """
```

### Comparing `nctoolkit-0.9.2/nctoolkit/mergers.py` & `nctoolkit-0.9.3/nctoolkit/mergers.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,39 @@
 
 from nctoolkit.runthis import run_this
 from nctoolkit.session import session_info
 from nctoolkit.show import nc_variables, nc_times
 from nctoolkit.utils import version_below
 from nctoolkit.api import open_data
 
+
 def chunks(l, n):
     n = max(1, n)
-    return (l[i:i+n] for i in range(0, len(l), n))
+    return (l[i : i + n] for i in range(0, len(l), n))
+
 
 import inspect
 from functools import wraps
 
+
 def check_checker(f):
     varnames = inspect.getfullargspec(f)[0]
+
     @wraps(f)
     def wrapper(*a, **kw):
-        explicit_params = set(list(varnames[:len(a)]) + list(kw.keys()))
+        explicit_params = set(list(varnames[: len(a)]) + list(kw.keys()))
         if "check" not in explicit_params:
             kw["check"] = "default"
         return f(*a, **kw)
+
     return wrapper
 
+
 @check_checker
-def merge(self, join="variables", match=["year", "month", "day"], check = True):
+def merge(self, join="variables", match=["year", "month", "day"], check=True):
     """
     Merge a multi-file ensemble into a single file
     2 methods are available. 1) merging files with different variables, but the same time steps.
     2) merging files with the same variables, with different times.
 
     Parameters
     -------------
@@ -44,22 +50,24 @@
         Optional argument when join = 'variables'. A list or str stating what must match in the netCDF files.
         Defaults to year/month/day. This list must be some combination of
         year/month/day. An error will be thrown if the elements of time in match
         do not match across all netCDF files. The only exception is if there is a
         single date file in the ensemble.
     check: bool
         By default nctoolkit out checks in case files do not have the same variables etc. Set check to False if you are confident merging will be problem free.
-        If you are unsure if files have the same variables, set check to True to find out. Note: if you do not explicitly provide check and there are more than 30 
+        If you are unsure if files have the same variables, set check to True to find out. Note: if you do not explicitly provide check and there are more than 30
         files in a dataset, checks will be turned off.
     """
 
     if check == "default":
         if len(self) > 30:
             check = False
-            warnings.warn(message = "Large ensemble, so no checks are being carried out prior to merging. Set check=True if you require files to be checked for variable compatability!")
+            warnings.warn(
+                message="Large ensemble, so no checks are being carried out prior to merging. Set check=True if you require files to be checked for variable compatability!"
+            )
         else:
             check = True
 
     if not isinstance(join, str):
         raise TypeError("join supplied is not a str")
 
     join_valid = False
@@ -102,33 +110,35 @@
         # check variable names are consistent
 
         if check:
             var_list = set()
             for ff in self:
                 var_list.add(",".join(nc_variables(ff)))
             if len(var_list) > 1:
-                raise ValueError("You are trying to merge files with different variables!")
+                raise ValueError(
+                    "You are trying to merge files with different variables!"
+                )
 
         cdo_command = "cdo --sortname -mergetime"
 
         if len(self) < 400:
             run_this(cdo_command, self, output="one")
         else:
             new_ds = open_data()
             files = chunks(self, 365)
             ii = 0
             for ff in files:
                 ii += 1
-                ds = open_data(ff, checks = False)
-                ds.merge("time", check = check)
-                #run_this(cdo_command, ds, output="one")
+                ds = open_data(ff, checks=False)
+                ds.merge("time", check=check)
+                # run_this(cdo_command, ds, output="one")
                 ds.run()
                 new_ds.append(ds)
 
-            new_ds.merge("time", check = check)
+            new_ds.merge("time", check=check)
             new_ds.run()
             self.current = new_ds.current
 
         if session_info["lazy"]:
             self._merged = True
         return None
```

### Comparing `nctoolkit-0.9.2/nctoolkit/meridonials.py` & `nctoolkit-0.9.3/nctoolkit/meridonials.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/mp_adders.py` & `nctoolkit-0.9.3/nctoolkit/mp_adders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 import pandas as pd
 from nctoolkit.api import open_data, open_thredds
-import xarray as xr
 from nctoolkit.matchpoint import open_matchpoint
 import nctoolkit.api as api
 
 
-def match_points(ds=None, df = None, variables=None, depths = None, nan=None, top = False, tmean = False, regrid = "bil", max_extrap = 5, **kwargs):
+def match_points(
+    ds=None,
+    df=None,
+    variables=None,
+    depths=None,
+    nan=None,
+    top=False,
+    tmean=False,
+    regrid="bil",
+    max_extrap=5,
+    **kwargs,
+):
     """
     Match netCDF data to a spatiotemporal points dataframe
 
     Parameters
     -------------
     ds: nctoolkit dataset or str/list of file paths
         Dataset or file(s) to match up with
     df: pandas dataframe containing the spatiotemporal points to match with.
-        The column names must be made up of a subset of "lon", "lat", "year", "month", "day" and "depth". 
+        The column names must be made up of a subset of "lon", "lat", "year", "month", "day" and "depth".
         "longitude" and "latitude" will also be accepted for lon/lat. Detection will not be case sensitive
     variables: str or list
         Str or list of variables. All variables are matched up if this is not supplied.
         This can include variables generated by assign using kwargs.
     depths:  nctoolkit dataset or list giving depths
         If each cell has different vertical levels, this must be provided as a dataset.
         If each cell has the same vertical levels, provide it as a list.
@@ -34,33 +44,33 @@
         Only required if values in dataset need changed to missing
     top: bool
         Set to True if you want only the top/surface level of the dataset to be selected for matching.
     regrid: str
         Regridding method. Defaults to "bil". Options available are those in nctoolkit regrid method.
         "nn" for nearest neighbour.
     max_extrap: float
-        Maximum distance for vertical extrapolation of values 
+        Maximum distance for vertical extrapolation of values
     kwargs: kwargs
-        Additional arguments to send to assign 
+        Additional arguments to send to assign
 
     Returns
     ---------------
     matchpoints : pandas.DataFrame
 
     """
 
     mp = open_matchpoint()
 
-    mp.add_data(x = ds, variables = variables, depths = depths, nan = nan, top = top,  **kwargs)
+    mp.add_data(x=ds, variables=variables, depths=depths, nan=nan, top=top, **kwargs)
     mp.add_points(df)
-    mp.matchup(tmean = tmean, regrid = regrid, max_extrap = max_extrap)
+    mp.matchup(tmean=tmean, regrid=regrid, max_extrap=max_extrap)
     return mp.values
 
 
-def add_data(self, x=None, variables=None, depths = None, nan=None, top = False, **kwargs):
+def add_data(self, x=None, variables=None, depths=None, nan=None, top=False, **kwargs):
     """
     Add dataset for matching
 
     Parameters
     -------------
     x: nctoolkit dataset or str/list of file paths
         Dataset or file(s) to match up with
@@ -85,125 +95,127 @@
     except:
         thredds = False
     self.thredds = thredds
 
     if depths is not None:
         self.add_depths(depths)
 
-     ##need to figure out what depths are if they are not provided.
+    ##need to figure out what depths are if they are not provided.
     if depths is None:
-
         if thredds:
-            ds = open_thredds(x, checks = False)
-            ds = open_thredds(ds[0], checks = False)
+            ds = open_thredds(x, checks=False)
+            ds = open_thredds(ds[0], checks=False)
         else:
-            ds = open_data(x, checks = False)
-            ds = open_data(ds[0], checks = False)
+            ds = open_data(x, checks=False)
+            ds = open_data(ds[0], checks=False)
         if len(ds.levels) > 1:
             if "e3t" in ds.variables:
                 ds_depths = ds.copy()
-                ds_depths.subset(time = 0)
-                ds_depths.subset(variable = "e3t")
+                ds_depths.subset(time=0)
+                ds_depths.subset(variable="e3t")
                 ds1 = ds_depths.copy()
                 ds_depths.vertical_cumsum()
                 ds1.run()
                 ds1.divide(2)
                 ds_depths.subtract(ds1)
                 self.depths = ds_depths.copy()
-                self.depths.rename({"e3t":"depth"})
+                self.depths.rename({"e3t": "depth"})
                 print("Depths were derived from e3t variable.")
             else:
                 try:
                     self.depths = ds.levels
                     print(f"Depths assumed to be {self.depths}")
                 except:
-                    raise ValueError("Unable to derive depths from the dataset! Please provide them.")
-
+                    raise ValueError(
+                        "Unable to derive depths from the dataset! Please provide them."
+                    )
 
     if depths is None:
         if self.points is not None:
             if "depth" in self.points:
-                raise ValueError("You cannot match depths without supplying dataset depths")
-
+                raise ValueError(
+                    "You cannot match depths without supplying dataset depths"
+                )
 
     self.top = top
 
     if variables is not None:
         if isinstance(variables, str):
             variables = [variables]
 
     if self.data is not None:
         raise ValueError("You have already added data!")
 
     if thredds:
-        self.data = open_thredds(x, checks = False)
-        #ds_vars = open_thredds(self.data[0], checks = False)
+        self.data = open_thredds(x, checks=False)
+        # ds_vars = open_thredds(self.data[0], checks = False)
     else:
-        self.data = open_data(x, checks = False)
-        #ds_vars = open_data(self.data[0], checks = False)
+        self.data = open_data(x, checks=False)
+        # ds_vars = open_data(self.data[0], checks = False)
 
     if variables is None:
         print("All variables will be used")
 
-
-
     if len(self.data) > 12:
         print("Checking file times. This could take a minute")
 
     self.data_nan = nan
 
     # figure out the time dim
 
     if thredds:
-        ds1 = open_thredds(self.data[0], checks = False)
+        ds1 = open_thredds(self.data[0], checks=False)
     else:
-        ds1 = open_data(self.data[0], checks = False)
+        ds1 = open_data(self.data[0], checks=False)
     pos_times = [
         x
         for x in [
             x for x in list(ds1.to_xarray().dims) if x in list(ds1.to_xarray().coords)
         ]
         if "time" in x
     ]
 
     if len(pos_times) != 1:
-        print("Unable to work out the name of time. Assuming no temporal matchups can occur.")
+        print(
+            "Unable to work out the name of time. Assuming no temporal matchups can occur."
+        )
         self.temporal = False
 
     if self.temporal:
-
         if len(pos_times) == 1:
             time_name = pos_times[0]
 
         df_times = []
 
         for ff in self.data:
             if thredds:
                 ds_ff = open_thredds(ff)
             else:
-                ds_ff = open_data(ff, checks = False)
+                ds_ff = open_data(ff, checks=False)
             ds = ds_ff.to_xarray()
             times = ds[time_name]
             days = [int(x.dt.day) for x in times]
             months = [int(x.dt.month) for x in times]
             years = [int(x.dt.year) for x in times]
             df_times.append(
-                pd.DataFrame({"day": days, "month": months, "year": years}).assign(path=ff)
+                pd.DataFrame({"day": days, "month": months, "year": years}).assign(
+                    path=ff
+                )
             )
         df_times = pd.concat(df_times)
 
         x = list(set(df_times.path))
 
     if len(self.data) > 12:
         print("Finished checking file times.")
 
     if thredds:
-        self.data = open_thredds(x, checks = False)
+        self.data = open_thredds(x, checks=False)
     else:
-        self.data = open_data(x, checks = False)
+        self.data = open_data(x, checks=False)
 
     self.variables = variables
 
     if len(kwargs) > 0:
         self.data.assign(**kwargs)
         self.data.run()
 
@@ -216,16 +228,17 @@
     if self.temporal:
         self.data_times = df_times
     else:
         self.data_times = None
 
     if self.temporal is False:
         if len(self.data) > 1:
-            raise ValueError("You cannot provide more than one dataset without temporal information")
-
+            raise ValueError(
+                "You cannot provide more than one dataset without temporal information"
+            )
 
 
 def add_depths(self, x=None):
     """
     Add depth
 
     Parameters
@@ -264,25 +277,24 @@
 
     """
 
     self.points_temporal = False
 
     df.columns = [x.lower() for x in df.columns]
 
-    df = df.rename(columns = {"longitude":"lon"})
-    df = df.rename(columns = {"latitude":"lat"})
+    df = df.rename(columns={"longitude": "lon"})
+    df = df.rename(columns={"latitude": "lat"})
 
     for x in df.columns:
         if x not in ["lon", "lat", "year", "month", "day", "depth", "pressure"]:
             raise ValueError(f"{x} is not a valid column name")
 
     if "depth" in df.columns and "pressure" in df.columns:
         raise ValueError("You cannot supply depth and pressure")
 
-
     if len([x for x in df.columns if x in ["lon", "lat"]]) < 2:
         raise ValueError("You must provide lon and lat!")
 
     for x in ["year", "month", "day"]:
         if x in df.columns:
             self.points_temporal = True
 
@@ -297,10 +309,10 @@
             raise ImportError("Please install seawater")
         print("Converting pressure to depth")
         self.points["depth"] = sw.dpth(self.points.pressure, self.points.lat)
 
     if self.depths is None and self.data is not None:
         if self.points is not None:
             if "depth" in self.points:
-                raise ValueError("You cannot match depths without supplying dataset depths")
-
-
+                raise ValueError(
+                    "You cannot match depths without supplying dataset depths"
+                )
```

### Comparing `nctoolkit-0.9.2/nctoolkit/mp_matchers.py` & `nctoolkit-0.9.3/nctoolkit/mp_matchers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,22 @@
-import pandas as pd
-from nctoolkit.api import open_data
-import xarray as xr
 from nctoolkit.matchpoint import open_matchpoint
 
-def match_points(self, df = None, variables = None, depths = None, tmean = False, top = False, nan = None, regrid = "bil", max_extrap = 5, **kwargs):
+
+def match_points(
+    self,
+    df=None,
+    variables=None,
+    depths=None,
+    tmean=False,
+    top=False,
+    nan=None,
+    regrid="bil",
+    max_extrap=5,
+    **kwargs,
+):
     """
     Match dataset to a spatiotemporal points dataframe
 
     Parameters
     -------------
     df: pandas DataFrame
         The column names must be made up of a subset of "lon", "lat", "year", "month", "day" and "depth"
@@ -31,17 +40,17 @@
     nan: float or list
         Value or range of values to set to nan. Defaults to 0.
         Only required if values in dataset need changed to missing
     regrid: str
         Regridding method. Defaults to "bil". Options available are those in nctoolkit regrid method.
         "nn" for nearest neighbour.
     max_extrap: float
-        Maximum distance for extrapolation. Defaults to 5. 
+        Maximum distance for extrapolation. Defaults to 5.
     kwargs: kwargs
-        Additional arguments to send to assign 
+        Additional arguments to send to assign
 
     Returns
     ---------------
     matchpoints : pandas.DataFrame
 
     """
     if max_extrap < 0:
@@ -50,16 +59,16 @@
     self.run()
     ds = self.copy()
 
     mp = open_matchpoint()
 
     df.columns = [x.lower() for x in df.columns]
 
-    df = df.rename(columns = {"longitude":"lon"})
-    df = df.rename(columns = {"latitude":"lat"})
+    df = df.rename(columns={"longitude": "lon"})
+    df = df.rename(columns={"latitude": "lat"})
 
     if len([x for x in df.columns if x in ["lon", "lat"]]) == 1:
         raise ValueError("You must provide both lon and lat")
 
     for x in df.columns:
         if x not in ["lon", "lat", "year", "month", "day", "depth", "pressure"]:
             raise ValueError(f"{x} is not a valid column name")
@@ -70,12 +79,11 @@
     if len([x for x in df.columns if x in ["lon", "lat"]]) < 2:
         raise ValueError("You must provide lon and lat!")
 
     for x in ["year", "month", "day"]:
         if x in df.columns:
             self.points_temporal = True
 
-    mp.add_data(x = ds, depths = depths, variables = variables, top = top, nan = nan,  **kwargs)
+    mp.add_data(x=ds, depths=depths, variables=variables, top=top, nan=nan, **kwargs)
     mp.add_points(df)
-    mp.matchup(tmean = tmean, regrid = regrid, max_extrap = max_extrap)
+    mp.matchup(tmean=tmean, regrid=regrid, max_extrap=max_extrap)
     return mp.values
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/mp_matchups.py` & `nctoolkit-0.9.3/nctoolkit/mp_matchups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import pandas as pd
-import re
-import scipy.interpolate as interpolate
 import warnings
 import numpy as np
 from nctoolkit.api import open_data, open_thredds
 from tqdm import tqdm
 
 
 from scipy.interpolate import interp1d
 
-def extrap1d(interpolator, max_extrap = 5):
+
+def extrap1d(interpolator, max_extrap=5):
     xs = interpolator.x
     ys = interpolator.y
 
     def pointwise(x):
-        if x > xs[-1]  and x <= xs[-1] + max_extrap:
+        if x > xs[-1] and x <= xs[-1] + max_extrap:
             return ys[-1]
         elif x > (xs[-1] + max_extrap):
             return np.nan
         elif x >= (xs[0] - max_extrap) and x < xs[0]:
             return ys[0]
         elif x < (xs[0] - max_extrap):
             return np.nan
@@ -26,46 +25,46 @@
             return interpolator(x)
 
     def ufunclike(xs):
         return np.array(list(map(pointwise, np.array(xs))))
 
     return ufunclike
 
-def interp(x,y, levels, max_extrap = 5):
+
+def interp(x, y, levels, max_extrap=5):
     try:
         f_i = interp1d(x, y)
-        f_x = extrap1d(f_i, max_extrap = max_extrap)
-        #f = interpolate.interp1d(x, y, fill_value = "extrapolate")
+        f_x = extrap1d(f_i, max_extrap=max_extrap)
         return f_x(levels)
     except:
-        df = pd.DataFrame({"x":x, "y":y}).dropna()
+        df = pd.DataFrame({"x": x, "y": y}).dropna()
         new = []
         for x in levels:
             if float(np.abs(df.x - x)) < max_extrap:
                 new.append(df.y)
             else:
                 new.append(np.nan)
         return new
 
 
-def matchup(self,  tmean = False, regrid = "bil", max_extrap = 5):
+def matchup(self, tmean=False, regrid="bil", max_extrap=5):
     """
     Matchup gridded model and point observational data
-    
+
     Parameters
     -------------
     tmean: bool
         Set to True or False. Defaults to False. This will calculate a temporal mean for the dataset at the
         resolution given in the point dataset. So, for example, if the point data is monthly, but the dataset
         is daily, it will calculate an appropritate monthly mean.
     regrid: str
         Regridding method. Defaults to "bil". Options available are those in nctoolkit regrid method.
         "nn" for nearest neighbour.
     max_extrap: float
-        Maximum distance for vertical extrapolation of values 
+        Maximum distance for vertical extrapolation of values
 
     """
 
     if max_extrap < 0:
         raise ValueError("max_extrap must be positive")
 
     self.max_extrap = max_extrap
@@ -94,41 +93,47 @@
     if isinstance(on, str):
         on = [on]
 
     if on is not None:
         if isinstance(on, list):
             for x in ["day", "month", "year"]:
                 if x not in on and x in points.columns:
-                    points = points.drop(columns = x)
-
+                    points = points.drop(columns=x)
 
     if self.thredds:
-        ds = open_thredds(self.data[0], checks = False)
+        ds = open_thredds(self.data[0], checks=False)
     else:
-        ds = open_data(self.data[0], checks = False)
+        ds = open_data(self.data[0], checks=False)
 
-    ds.subset(variables = ds.variables[0])
-    ds.subset(time = 0)
+    ds.subset(variables=ds.variables[0])
+    ds.subset(time=0)
     ds.top()
     ds.cdo_command("setmisstoc,1")
-    df = points.loc[:,["lon", "lat"]].drop_duplicates()
-    ds.regrid(df, method = regrid)
-    grid = ds.to_dataframe().reset_index().dropna().loc[:,["lon", "lat"]].drop_duplicates()
+    df = points.loc[:, ["lon", "lat"]].drop_duplicates()
+    ds.regrid(df, method=regrid)
+    grid = (
+        ds.to_dataframe()
+        .reset_index()
+        .dropna()
+        .loc[:, ["lon", "lat"]]
+        .drop_duplicates()
+    )
 
     n_start = len(points)
 
     points = points.merge(grid)
 
     if len(points) == 0:
         raise ValueError("None of the points are contained within the dataset grid")
 
     if len(points) < n_start:
         n_remove = n_start - len(points)
-        print(f"{n_remove} points are outside the dataset grid, and were therefore removed.")
-
+        print(
+            f"{n_remove} points are outside the dataset grid, and were therefore removed."
+        )
 
     n_levels = len(self.data.levels)
 
     if self.points_temporal is False:
         if self.temporal:
             if on is None:
                 on = ["all"]
@@ -140,27 +145,27 @@
 
     acceptable = ["lon", "lat", "year", "month", "day", "depth"]
 
     if self.temporal is False:
         # We need a quick hack
         df_times = []
         for ff in self.data:
-            df_times.append(pd.DataFrame({"year":[None]}))
+            df_times.append(pd.DataFrame({"year": [None]}))
         df_times = pd.concat(df_times)
         self.data_times = df_times
 
-
     if self.temporal:
         if on != ["all"]:
             if tmean is False:
                 df_times = self.data_times
                 point_col = [x for x in df_times.columns if x in points.columns]
-                df_times = self.data_times.merge(points.loc[:,point_col]).drop_duplicates()
+                df_times = self.data_times.merge(
+                    points.loc[:, point_col]
+                ).drop_duplicates()
             else:
-
                 if on == ["day"]:
                     on = ["day", "month"]
                     if "month" not in points.columns:
                         on.remove("month")
                 if not isinstance(on, list):
                     raise ValueError("on must be a list")
                 for x in on:
@@ -175,77 +180,71 @@
                 # This needs to work when there is no time
 
                 if self.points_temporal:
                     df_times = self.data_times.loc[:, on].merge(points.loc[:, on])
                 else:
                     df_times = self.data_times
                 df_times = df_times.drop_duplicates()
-                time_avail = [x for x in ["year", "month", "day"] if x in df_times.columns]
+                time_avail = [
+                    x for x in ["year", "month", "day"] if x in df_times.columns
+                ]
                 df_times = df_times.sort_values(by=time_avail).reset_index(drop=True)
         else:
-            df_times = self.data_times.drop(columns = "path")
+            df_times = self.data_times.drop(columns="path")
 
     if self.temporal is False:
         df_times = self.data_times
 
     df_merged = []
 
-
     # depths only need to be calculated once
     if self.depths is not None:
         if not isinstance(self.depths, list):
             ds_depths = self.depths.copy()
-            obs_locs = points.loc[:,["lon", "lat"]]
-            ds_depths.regrid(obs_locs, method = regrid) 
+            obs_locs = points.loc[:, ["lon", "lat"]]
+            ds_depths.regrid(obs_locs, method=regrid)
             df_depths = (
                 ds_depths.to_dataframe()
                 .reset_index()
                 .loc[:, ["lon", "lat", "depth"]]
                 .drop_duplicates()
             )
         else:
             df_depths = pd.DataFrame({"depth": self.depths})
 
-        all_depths = df_depths
-
     points_merged = False
     if self.points_temporal is False:
         if len(self.data.levels) < 2:
             if self.thredds:
-                ds = open_thredds(self.data, checks = False)
+                ds = open_thredds(self.data, checks=False)
             else:
-                ds = open_data(self.data, checks = False)
+                ds = open_data(self.data, checks=False)
             if self.variables is not None:
-                ds.subset(variables = self.variables)
-            ds.regrid(points.loc[:,["lon", "lat"]], method = regrid) 
+                ds.subset(variables=self.variables)
+            ds.regrid(points.loc[:, ["lon", "lat"]], method=regrid)
             df_merged = [ds.to_dataframe().reset_index()]
             points_merged = True
 
     n_missing = 0
 
-
     if (len(df_times)) == 0:
         raise ValueError("There are no matching times")
 
-
     if points_merged is False:
-
-        df_times = df_times.sample(frac = 1)
+        df_times = df_times.sample(frac=1)
 
         print("Looping through times in ds and df to matchup")
         for i in tqdm(range(0, len(df_times))):
             if self.temporal:
-                i_df = df_times.iloc[
-                    i : (i + 1) :,
-                ]
-                i_df = i_df.reset_index(drop = True)
+                i_df = df_times.iloc[i : (i + 1) :,]
+                i_df = i_df.reset_index(drop=True)
                 if self.points_temporal:
                     i_grid = points.merge(i_df).loc[:, ["lon", "lat"]]
                 else:
-                    i_grid = points.loc[:,["lon", "lat"]]
+                    i_grid = points.loc[:, ["lon", "lat"]]
                 i_year = None
                 i_month = None
                 i_day = None
                 if "year" in on or tmean is False:
                     try:
                         i_year = i_df.year.values[0]
                     except:
@@ -272,49 +271,50 @@
                         i_month = None
                     try:
                         i_day = i_df.day.values[0]
                     except:
                         i_day = None
 
                 if self.thredds:
-                    ds = open_thredds(set(self.data_times.merge(i_df).path), checks=False)
+                    ds = open_thredds(
+                        set(self.data_times.merge(i_df).path), checks=False
+                    )
                 else:
                     ds = open_data(set(self.data_times.merge(i_df).path), checks=False)
             else:
                 if self.thredds:
                     ds = open_thredds(self.data, checks=False)
                 else:
                     ds = open_data(self.data, checks=False)
                 i_grid = points.loc[:, ["lon", "lat"]].drop_duplicates()
 
-
             if self.variables is not None:
                 ds.subset(variables=self.variables)
             if self.top:
                 ds.top()
 
             if self.temporal:
                 for opt in ["day", "year", "month"]:
                     if i_day is not None:
                         ds.subset(day=i_day)
-                    if i_month  is not None:
+                    if i_month is not None:
                         ds.subset(month=i_month)
                     if i_year is not None:
                         ds.subset(year=i_year)
 
                     if self.points_temporal:
                         if len(ds) > 1:
                             ds.merge("time")
             if on is not None and tmean is True:
                 ds.tmean(on)
 
             if self.data_nan is not None:
                 ds.as_missing(self.data_nan)
 
-            ds.regrid(i_grid, method = regrid) 
+            ds.regrid(i_grid, method=regrid)
 
             df_model = ds.to_dataframe().reset_index().drop_duplicates()
 
             # figure out the time dim
 
             if self.temporal:
                 pos_times = [
@@ -329,75 +329,72 @@
 
                 if len(pos_times) != 1:
                     raise ValueError("Unable to work out the name of time")
 
                 if len(pos_times) == 1:
                     time_name = pos_times[0]
 
-            if self.depths is  None:
-
+            if self.depths is None:
                 if self.temporal:
                     locs = [time_name, "lon", "lat"]
                 else:
-                    locs = [ "lon", "lat"]
+                    locs = ["lon", "lat"]
 
                 locs += ds.variables
                 if len(ds.levels) > 1:
                     adict = dict(ds.to_xarray().dims)
 
-                    locs += [k for k in adict.keys() if adict[k]  == n_levels]
-                    acceptable += [k for k in adict.keys() if adict[k]  == n_levels]
+                    locs += [k for k in adict.keys() if adict[k] == n_levels]
+                    acceptable += [k for k in adict.keys() if adict[k] == n_levels]
                     locs = list(set(locs))
 
-                df_model = df_model.loc[
-                    :,  locs
-                ].drop_duplicates()
+                df_model = df_model.loc[:, locs].drop_duplicates()
                 df_merged.append(df_model)
 
             else:
-
                 if "deptht" in df_model.columns:
-
                     if self.temporal:
                         locs = [time_name, "lon", "lat", "deptht"]
                     else:
-                        locs = [ "lon", "lat", "deptht"]
+                        locs = ["lon", "lat", "deptht"]
                     locs += ds.variables
                     df_model = df_model.loc[:, locs].drop_duplicates()
 
                 else:
-                    locs = [ "lon", "lat"]
+                    locs = ["lon", "lat"]
                     locs += ds.variables
-                    drop = [x for x in df_model.columns if "depth" in x and "bnds" not in x]
+                    drop = [
+                        x for x in df_model.columns if "depth" in x and "bnds" not in x
+                    ]
                     locs += drop
-                    df_model = df_model.loc[ :, locs ].drop_duplicates()
-                    df_model = df_model.drop(columns = drop)
-
+                    df_model = df_model.loc[:, locs].drop_duplicates()
+                    df_model = df_model.drop(columns=drop)
 
                 if self.points_temporal:
                     i_obs_df = i_df.merge(points)
                 else:
                     i_obs_df = points
 
                 i_obs_locs = i_obs_df.loc[:, ["lon", "lat"]].drop_duplicates()
-                
 
                 if True:
-
                     for j in range(0, len(i_obs_locs)):
                         if self.depths is not None:
                             df_depths = df_depths
 
-                        j_obs = i_obs_locs.iloc[j : (j + 1), :].merge(i_obs_df).drop_duplicates()
-
-                        j_model = (
-                            df_model.merge(j_obs.loc[:, ["lon", "lat"]].drop_duplicates())
-                            .reset_index(drop=True)
+                        j_obs = (
+                            i_obs_locs.iloc[j : (j + 1), :]
+                            .merge(i_obs_df)
+                            .drop_duplicates()
                         )
-                        j_model = j_model.reset_index(drop = True)
+
+                        j_model = df_model.merge(
+                            j_obs.loc[:, ["lon", "lat"]].drop_duplicates()
+                        ).reset_index(drop=True)
+                        j_model = j_model.reset_index(drop=True)
 
                         if len(j_model) > 0:
                             if not isinstance(self.depths, list):
                                 if self.depths is not None:
                                     j_depths = (
                                         df_depths.merge(j_obs.loc[:, ["lon", "lat"]])
                                         .drop_duplicates()
@@ -412,69 +409,68 @@
                             else:
                                 if self.depths is not None:
                                     locs = ["lon", "lat", "depth"]
                                     locs += ds.variables
                                     j_model = j_model.merge(
                                         df_depths, left_index=True, right_index=True
                                     ).loc[:, locs]
-                                    #j_model = j_model.drop_duplicates()
-
-                            if self.depths is not None:
-                                max_depth = np.max(j_model.depth)
-                                min_depth = np.min(j_model.depth)
 
                             if len(j_obs) > 0:
-
                                 try:
                                     if self.depths is not None:
                                         i_var = 0
                                         for var in ds.variables:
-                                            j_obs[var] = interp(list(j_model.depth), j_model[var], list(j_obs.depth), max_extrap = self.max_extrap)
-        
-                                            i_var +=1
+                                            j_obs[var] = interp(
+                                                list(j_model.depth),
+                                                j_model[var],
+                                                list(j_obs.depth),
+                                                max_extrap=self.max_extrap,
+                                            )
+
+                                            i_var += 1
                                         for x in ["day", "month", "year"]:
                                             if x in i_df.columns:
                                                 j_obs[x] = i_df[x].values[0]
 
                                         df_merged.append(j_obs)
                                     else:
                                         df_merged.append(j_model)
                                 except:
                                     n_missing += 1
 
     if n_missing > 0:
-        warnings.warn(f"{n_missing} points did not have sufficient vertical points in ds for vertical interpolation")
+        warnings.warn(
+            f"{n_missing} points did not have sufficient vertical points in ds for vertical interpolation"
+        )
 
     if len(df_merged) == 0:
         raise ValueError("No data matches were found")
 
     self.values = df_merged
     df_merged = pd.concat(df_merged).drop_duplicates().reset_index(drop=True)
 
     if self.temporal is False:
         acceptable += ds.variables
         acceptable = [x for x in df_merged.columns if x in acceptable]
-        df_merged = df_merged.loc[:,acceptable]
+        df_merged = df_merged.loc[:, acceptable]
 
     if len([x for x in df_merged.columns if x.startswith("time")]) == 1:
         orig_df = df_merged
         try:
             time_name = [x for x in df_merged.columns if x.startswith("time")][0]
             times = df_merged[time_name]
             df_merged["year"] = [x.year for x in times]
             df_merged["month"] = [x.month for x in times]
             df_merged["day"] = [x.day for x in times]
-            df_merged = df_merged.drop(columns = time_name)
+            df_merged = df_merged.drop(columns=time_name)
             # get acceptable variables....
             acceptable += ds.variables
             acceptable = [x for x in df_merged.columns if x in acceptable]
-            df_merged = df_merged.loc[:,acceptable]
+            df_merged = df_merged.loc[:, acceptable]
 
         except:
             df_merged = orig_df
 
     if "path" in df_merged.columns:
-        df_merged = df_merged.drop(columns = "path")
+        df_merged = df_merged.drop(columns="path")
 
     self.values = df_merged
-
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/nco_command.py` & `nctoolkit-0.9.3/nctoolkit/nco_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import copy
 import multiprocessing
+import platform
+import warnings
 
 from nctoolkit.cleanup import cleanup
 from nctoolkit.flatten import str_flatten
 from nctoolkit.runthis import run_nco
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import remove_safe, session_info, append_safe, get_safe
 
@@ -22,14 +24,19 @@
         This is useful for ensemble methods.
     """
 
     self.run()
 
     cores = session_info["cores"]
 
+    if platform.system() != "Linux":
+        if cores > 1:
+            warnings.warn("This cannot run in parallel on macOS")
+            cores = 1
+
     # First, check that the command is valid
     if command is None:
         raise ValueError("Please supply a command")
 
     if not isinstance(command, str):
         raise TypeError("Command supplied is not a str")
 
@@ -50,31 +57,28 @@
         pool = multiprocessing.Pool(cores)
         target_list = []
         results = dict()
     else:
         target_list = []
 
     if (ensemble is False) or (len(self) == 1):
-
         if cores > 1:
             for ff in self:
-
                 target = temp_file(".nc")
 
                 append_safe(target)
 
                 the_command = f"{command} {ff} {target}"
 
                 temp = pool.apply_async(run_nco, [the_command, target])
                 results[ff] = temp
                 new_commands.append(the_command)
 
         else:
             for ff in self:
-
                 target = temp_file(".nc")
                 append_safe(target)
 
                 the_command = f"{command} {ff} {target}"
 
                 target = run_nco(the_command, target=target)
 
@@ -91,23 +95,22 @@
 
         target = run_nco(the_command, target=target)
 
         new_files.append(target)
         new_commands.append(the_command)
 
     if cores == 1 or ensemble:
-
         self.current = new_files
 
         while True:
             removed = 0
             for ff in new_files:
                 if len([x for x in get_safe() if x == ff]) > 1:
                     remove_safe(ff)
-                    removed +=1
+                    removed += 1
             if removed == 0:
                 break
 
         self.history.append(command)
         self._hold_history = copy.deepcopy(self.history)
 
     if cores > 1:
@@ -122,13 +125,13 @@
         self._hold_history = copy.deepcopy(self.history)
 
         while True:
             removed = 0
             for ff in target_list:
                 if len([x for x in get_safe() if x == ff]) > 1:
                     remove_safe(ff)
-                    removed +=1
+                    removed += 1
             if removed == 0:
                 break
 
     self.disk_clean()
     cleanup()
```

### Comparing `nctoolkit-0.9.2/nctoolkit/phenology.py` & `nctoolkit-0.9.3/nctoolkit/phenology.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,20 +54,18 @@
         if var not in nc_variables(ff):
             raise ValueError(f"{var} is not a valid variable!")
 
     if split_files:
         self.split("year")
 
     if metric == "peak":
-
         new_files = []
         new_commands = []
 
         for ff in self:
-
             target = temp_file(".nc")
             command = (
                 f"cdo -timmin -setrtomiss,-10000,0 -expr,'peak=var*ctimestep()' "
                 f"-eq -chname,{var},var -selname,{var} {ff} -timmax -chname,{var},var "
                 f"-selname,{var} {ff} {target}"
             )
 
@@ -85,15 +83,14 @@
         for ff in new_files:
             remove_safe(ff)
 
         cleanup()
         return None
 
     if (metric == "start") or (metric == "end") or (metric == "middle"):
-
         if metric == "middle":
             p = 50.0
 
         if (metric == "start") and (p is None):
             p = 25.0
 
         if (metric == "end") and (p is None):
@@ -106,15 +103,14 @@
             raise TypeError("p is not float")
 
         start = (p) / 100
         new_files = []
         new_commands = []
 
         for ff in self:
-
             target = temp_file(".nc")
             command = (
                 f"cdo -timmin -setrtomiss,-10000,0 -expr,"
                 f"'{metric}=var*ctimestep()' -gt -timcumsum -chname,{var},var "
                 f"-selname,{var} {ff} -mulc,{start} -timsum -chname,{var},var "
                 f"-selname,{var} {ff} {target}"
             )
```

### Comparing `nctoolkit-0.9.2/nctoolkit/plot.py` & `nctoolkit-0.9.3/nctoolkit/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import signal
 from contextlib import contextmanager
 from nctoolkit.session import session_info
 
+
 class TimeoutException(Exception):
     pass
 
+
 @contextmanager
 def time_limit(seconds):
     def signal_handler(signum, frame):
         raise TimeoutException("Timed out. Try plotting fewer variables!")
 
     signal.signal(signal.SIGALRM, signal_handler)
     signal.alarm(seconds)
     try:
         yield
     finally:
         signal.alarm(0)
 
 
-def plot(self, vars=None, autoscale=True, out = None, coast= True, **kwargs):
+def plot(self, vars=None, autoscale=True, out=None, coast=True, **kwargs):
     from ncplot import view
 
     """
     Autoplotting method.
     Automatically plot a dataset.
 
     Parameters
@@ -48,15 +50,14 @@
     If you only want to plot a single variable, do the following. Note, this is often faster if you
     have a large dataset.
 
     >>> ds.plot("var_of_choice")
 
     """
 
-
     if "title" not in kwargs.keys():
         kwargs["title"] = ""
 
     # run any commands
     self.run()
 
     if not session_info["coast"]:
@@ -82,17 +83,16 @@
     if isinstance(vars, list):
         if len(set(self.contents.query("variable in @vars").nlevels)) > 1:
             raise ValueError(
                 "Unable to plot datasets when variables have differing levels"
             )
     if vars is None and len(self.variables) > 1:
         with time_limit(20):
-            return view(self[0], autoscale=autoscale, coast= coast, **kwargs)
+            return view(self[0], autoscale=autoscale, coast=coast, **kwargs)
 
     if isinstance(vars, list) and len(vars) > 1:
         with time_limit(20):
-            return view(self[0], vars=vars, autoscale=autoscale, out = out, coast = coast,  **kwargs)
-
-    return view(self[0], vars=vars, autoscale=autoscale, out = out, coast= coast,   **kwargs)
-
-
+            return view(
+                self[0], vars=vars, autoscale=autoscale, out=out, coast=coast, **kwargs
+            )
 
+    return view(self[0], vars=vars, autoscale=autoscale, out=out, coast=coast, **kwargs)
```

### Comparing `nctoolkit-0.9.2/nctoolkit/reduce.py` & `nctoolkit-0.9.3/nctoolkit/reduce.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/reduce_grid.py` & `nctoolkit-0.9.3/nctoolkit/reduce_grid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/regrid.py` & `nctoolkit-0.9.3/nctoolkit/regrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 from nctoolkit.cleanup import cleanup
 from nctoolkit.generate_grid import generate_grid
 from nctoolkit.runthis import run_this, run_cdo
 from nctoolkit.session import append_safe, remove_safe, get_safe
 from nctoolkit.temp_file import temp_file
 import nctoolkit.api as api
 
+
 def is_iterable(x):
     try:
         iter(x)
         return True
     except:
         return False
 
 
-def regrid(self, grid=None, method="bil", recycle=False, one_grid = False, **kwargs):
+def regrid(self, grid=None, method="bil", recycle=False, one_grid=False, **kwargs):
     """
     Regrid a dataset to a target grid
 
     Parameters
     -------------
     grid : nctoolkit.DataSet, pandas data frame or netCDF file
         The grid to remap to
@@ -34,38 +35,38 @@
         bilinear - "bil";
         nearest neighbour - "nn" - "nearest neighbour"
         bicubic interpolation - "bic"
         Distance-weighted average - "dis"
         First order conservative remapping - "con"
         Second order conservative remapping - "con2"
         Large area fraction remapping - "laf"
-    recycle : bool 
-        Set to True if you want to re-use the remapping weights when you are regridding another dataset. 
-    one_grid : bool 
-        Set to True if all files in multi-file dataset have the same grid, to speed things up. 
-    kwargs : optional method to generate grid 
+    recycle : bool
+        Set to True if you want to re-use the remapping weights when you are regridding another dataset.
+    one_grid : bool
+        Set to True if all files in multi-file dataset have the same grid, to speed things up.
+    kwargs : optional method to generate grid
         Instead of supplying a grid using 'grid', you can supply `lon` and `lat`. These must be equally
         lengthed lists or arrays that will be used to generate the grid. If you want to regrid to a single
         location you can just supply a float to lon and lat.
-        
+
     """
 
     if grid is None and len(kwargs) > 0:
         if "lon" in kwargs and "lat" in kwargs:
             lon = kwargs["lon"]
             lat = kwargs["lat"]
 
             if is_iterable(lon) is False:
                 lon = [lon]
 
             if is_iterable(lat) is False:
                 lat = [lat]
 
             if len(lon) == len(lat):
-                grid = pd.DataFrame({"lon":lon, "lat":lat})
+                grid = pd.DataFrame({"lon": lon, "lat": lat})
 
     if len(self) == 0:
         raise ValueError("Failure due to empty dataset!")
 
     if isinstance(method, str):
         if "nearest" in method:
             method = "nn"
@@ -138,16 +139,15 @@
             if cdo_result in grid_split:
                 grid_split[cdo_result].append(ff)
             else:
                 grid_split[cdo_result] = [ff]
         else:
             grid_split[cdo_result].append(ff)
         if one_grid:
-            i+=1
-
+            i += 1
 
     if grid is not None:
         # first generate the grid
         if grid_type == "df":
             target_grid = generate_grid(grid)
             del_grid = copy.deepcopy(target_grid)
             append_safe(del_grid)
@@ -163,15 +163,15 @@
     else:
         suppress = False
 
     for key in grid_split:
         # first we need to generate the weights for remapping
         # and add this to the files created list and self.weights
         tracker = open_data(
-            grid_split[key], suppress_messages=True, thredds=self._thredds, checks = False
+            grid_split[key], suppress_messages=True, thredds=self._thredds, checks=False
         )
 
         weights_nc = temp_file("nc")
 
         cdo_command = (
             f"cdo -gen{method},{target_grid} {tracker.current[0]} {weights_nc}"
         )
@@ -189,15 +189,15 @@
             self._weights = weights_nc
             self._grid = target_grid
 
         cdo_command = f"cdo -remap,{target_grid},{weights_nc}"
 
         tracker._execute = True
 
-        run_this(cdo_command, tracker, output="ensemble", suppress = suppress)
+        run_this(cdo_command, tracker, output="ensemble", suppress=suppress)
 
         if recycle is False:
             remove_safe(weights_nc)
 
         for ff in tracker:
             append_safe(ff)
```

### Comparing `nctoolkit-0.9.2/nctoolkit/remove.py` & `nctoolkit-0.9.3/nctoolkit/remove.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/rename.py` & `nctoolkit-0.9.3/nctoolkit/rename.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from nctoolkit.runthis import run_this
 from nctoolkit.show import nc_variables
 from nctoolkit.utils import name_check
 import warnings
 
+
 # A custom format for warnings.
 def custom_formatwarning(msg, *args, **kwargs):
     # ignore everything except the message
     return str(msg) + "\n"
 
+
 warnings.formatwarning = custom_formatwarning
 
 
-def rename(self, newnames = None, **kwargs):
+def rename(self, newnames=None, **kwargs):
     """
     Rename variables in a dataset
 
     Parameters
     -------------
     newnames : dict
         Dictionary with key-value pairs being original and new variable names
     * kwargs
-        Alternative method for renaming 
+        Alternative method for renaming
 
     Examples
     ------------
     If you want to rename a variable x to y, do the following:
 
         >>> ds.rename({"x":"y"})
 
@@ -40,29 +42,30 @@
         raise TypeError("a dictionary was not supplied")
 
     if len(self.history) == len(self._hold_history):
         variables = nc_variables(self[0])
         for key in newnames:
             if key not in variables:
                 if len(self) > 1:
-                    warnings.warn(message = f"{key} is not in the first file of the dataset")
+                    warnings.warn(
+                        message=f"{key} is not in the first file of the dataset"
+                    )
                 else:
-                    warnings.warn(message = f"{key} is not in the dataset")
+                    warnings.warn(message=f"{key} is not in the dataset")
 
     # now, we need to loop through the renaming dictionary to get the cdo sub
     cdo_rename = ""
 
     for key, value in newnames.items():
         if name_check(key) is False:
             raise ValueError(f"{key} is not a valid netCDF variable name")
 
         if name_check(value) is False:
             raise ValueError(f"{value} is not a valid netCDF variable name")
 
-
     for key, value in newnames.items():
         if not isinstance(key, str):
             raise TypeError(f"{key} is not a str")
         if not isinstance(value, str):
             raise TypeError(f"{value} is not a str")
         cdo_rename += "," + key
         cdo_rename += "," + value
```

### Comparing `nctoolkit-0.9.2/nctoolkit/resample.py` & `nctoolkit-0.9.3/nctoolkit/resample.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/rollstat.py` & `nctoolkit-0.9.3/nctoolkit/rollstat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from nctoolkit.runthis import run_this
 
-def align(self, align = "right"):
+
+def align(self, align="right"):
     """
-    Method to align output time in temporal methods. 
+    Method to align output time in temporal methods.
 
     Parameters
     -------------
     align = str
         This determines whether the output time is at the left, centre or right hand side of the time window.
         Options are "left", "centre" and "right"
 
     """
-    
+
     if not isinstance(align, str):
         raise TypeError("Alignment must be str type")
 
     if "cen" in align:
         align = "middle"
 
     if "left" in align:
@@ -29,23 +30,24 @@
 
     if "first" in align:
         align = "first"
 
     if "middle" in align:
         align = "midhigh"
 
-    if align not in ["first","middle","last", "midhigh"]:
+    if align not in ["first", "middle", "last", "midhigh"]:
         raise ValueError(f"{align} is not a valid align argument")
 
     new_align = f"--timestat_date {align}"
     if len(self._align) > 0:
         if self._align != new_align:
             self.run()
 
-    self._align = new_align 
+    self._align = new_align
+
 
 def rollstat(self, window=None, stat="mean"):
     """Method to calculate the monthly statistic from a netCDF file"""
 
     # check alignment
 
     # check window supplied is valid
@@ -60,41 +62,41 @@
         raise ValueError(f"{window} is not a valid window!")
 
     # create the cdo call and run it
     cdo_command = f"cdo -run{stat},{str(window)}"
     run_this(cdo_command, self, output="ensemble")
 
 
-def rolling_mean(self, window=None, align = "right"):
+def rolling_mean(self, window=None, align="right"):
     """
     Calculate a rolling mean based on a window
 
     Parameters
     -------------
     window: int
         The size of the window for the calculation of the rolling mean
     align: str
         This determines whether the output time is at the left, centre or right hand side of the time window.
         Options are "left", "centre" and "right"
 
-         
+
 
     Examples
     ------------
 
     If you wanted to calculate a rolling mean with the mean calculated over every 10 time steps, do the following:
 
     >>> ds.rolling_mean(10)
 
     """
     self.align(align)
     rollstat(self, window=window, stat="mean")
 
 
-def rolling_min(self, window=None, align = "right"):
+def rolling_min(self, window=None, align="right"):
     """
     Calculate a rolling minimum based on a window
 
     Parameters
     -------------
     window: int
         The size of the window for the calculation of the rolling minimum
@@ -109,15 +111,15 @@
 
     >>> ds.rolling_min(10)
     """
     self.align(align)
     rollstat(self, window=window, stat="min")
 
 
-def rolling_max(self, window=None, align = "right"):
+def rolling_max(self, window=None, align="right"):
     """
     Calculate a rolling maximum based on a window
 
     Parameters
     -------------
     window: int
         The size of the window for the calculation of the rolling maximum
@@ -131,15 +133,15 @@
 
     >>> ds.rolling_max(10)
     """
     self.align(align)
     rollstat(self, window=window, stat="max")
 
 
-def rolling_range(self, window=None, align = "right"):
+def rolling_range(self, window=None, align="right"):
     """
     Calculate a rolling range based on a window
 
     Parameters
     -------------
     window: int
         The size of the window for the calculation of the rolling range
@@ -154,15 +156,15 @@
 
     >>> ds.rolling_range(10)
     """
     self.align(align)
     rollstat(self, window=window, stat="range")
 
 
-def rolling_sum(self, window=None, align = "right"):
+def rolling_sum(self, window=None, align="right"):
     """
     Calculate a rolling sum based on a window
 
     Parameters
     -------------
     window: int
         The size of the window for the calculation of the rolling sum
@@ -176,15 +178,16 @@
     If you wanted to calculate a rolling sum with the sum calculated over every 10 time steps, do the following:
 
     >>> ds.rolling_sum(10)
     """
     self.align(align)
     rollstat(self, window=window, stat="sum")
 
-def rolling_var(self, window=None, align = "right"):
+
+def rolling_var(self, window=None, align="right"):
     """
     Calculate a rolling variance based on a window
 
     Parameters
     -------------
     window: int
         The size of the window for the calculation of the rolling sum
@@ -198,15 +201,16 @@
     If you wanted to calculate a rolling variance with the variance calculated over every 10 time steps, do the following:
 
     >>> ds.rolling_sum(10)
     """
     self.align(align)
     rollstat(self, window=window, stat="var")
 
-def rolling_stdev(self, window=None, align = "right"):
+
+def rolling_stdev(self, window=None, align="right"):
     """
     Calculate a rolling standard deviation based on a window
 
     Parameters
     -------------
     window: int
         The size of the window for the calculation of the rolling sum
```

### Comparing `nctoolkit-0.9.2/nctoolkit/run.py` & `nctoolkit-0.9.3/nctoolkit/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
 
     # the first step is to set the run status to true
 
     if (self._execute is False) and (
         len(self.history) > len(self._hold_history)
         or self._zip
-        or self._format is not None 
+        or self._format is not None
         or self._precision != "default"
     ):
         self._execute = True
 
         cdo_command = "cdo "
         if self._precision != "default":
             if len(self.history) == len(self._hold_history):
@@ -47,11 +47,11 @@
                 remove_safe(ff)
 
         self._safe = []
 
         cleanup()
 
         self._ncommands = 0
-        self._align= ""
+        self._align = ""
         self.disk_clean()
 
         self._precision = "default"
```

### Comparing `nctoolkit-0.9.2/nctoolkit/runthis.py` & `nctoolkit-0.9.3/nctoolkit/runthis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import copy
 import os
 import re
 import subprocess
 import platform
 import warnings
-import multiprocessing
+if platform.system() == "Linux":
+    import multiprocessing as mp
+else:
+    import multiprocess as mp
+
 import signal
 
 from nctoolkit.cleanup import cleanup
 from nctoolkit.flatten import str_flatten
 from nctoolkit.session import (
     session_info,
     append_safe,
@@ -28,15 +32,14 @@
     """
     if os.path.isfile(file_path):
         file_info = os.stat(file_path)
         return file_info.st_size
 
 
 def tidy_command(command):
-
     if session_info["precision"] is not None:
         command = command.replace("cdo ", "cdo -b " + session_info["precision"] + " ")
 
     command = command.replace("  ", " ")
 
     if " --sortname " in command:
         command = command.replace(" --sortname ", " ")
@@ -147,15 +150,14 @@
     if target != "":
         session_info["latest_size"] = os.path.getsize(target)
 
     return target
 
 
 def run_cdo(command=None, target=None, out_file=None, overwrite=False, precision=None):
-
     warned = False
 
     if not isinstance(precision, str):
         raise ValueError("Precision must be str")
 
     if precision not in ["I8", "I16", "I32", "F32", "F64", "default"]:
         raise ValueError(f"Precision - {precision} - is not valid")
@@ -416,15 +418,14 @@
         errors = text.findall(error)
         if len(errors) > 0:
             error = errors[0]
             raise ValueError(
                 f"None of the days supplied are available. Please check days supplied to nctoolkit methods!"
             )
 
-
         text = re.compile(r"Timestep [0-9]* not found")
         errors = text.findall(error)
         if len(errors) > 0:
             error = errors[0]
             error = [str(int(x) - 1) for x in re.findall(r"\d+", error)]
             error = ",".join(error)
             error = "The following timesteps do not exist: " + error
@@ -607,32 +608,30 @@
     sel_day = []
     sel_month = []
     sel_level = []
     sel_timestep = []
     sel_hour = []
     sel_var = []
 
-
     drop_warnings = []
 
     for x in result.decode("utf-8").lower().split("\n"):
         warned = False
         ignore = False
 
         text = re.compile("delete \(warning\): month >[0-9]*< not found!")
         errors = text.findall(x)
         if len(errors) > 0:
             for y in errors:
-                for z in re.findall(r'\d+', y):
+                for z in re.findall(r"\d+", y):
                     drop_warnings.append(z)
-                    #message= f"Warning: Unable to find month {z}"
-                    #warnings.warn(message)
+                    # message= f"Warning: Unable to find month {z}"
+                    # warnings.warn(message)
                     ignore = True
 
-
         if "selyear" in x:
             text = re.compile("selyear \\(warning\\): year [0-9]* not found")
             all_text = text.findall(x)
             if len(all_text) > 0:
                 for tt in all_text:
                     sel_year.append(int(re.findall(r"\d+", all_text[0])[0]))
                 ignore = True
@@ -759,32 +758,26 @@
                 text_find = text.findall(x)
                 if len(text_find) > 0:
                     message = text_find[0]
                     message = "Warning for grid area calculations: " + message
                     warnings.warn(message)
                     warned = True
 
-                text = re.compile(
-                    "delete \(warning\): timestep .* not found"
-                )
+                text = re.compile("delete \(warning\): timestep .* not found")
                 text_find = text.findall(x)
                 if len(text_find) > 0:
                     message = text_find[0]
                     message = "Warning: attempting to drop non-existent timesteps!"
                     warnings.warn(message)
                     warned = True
 
             ## Unsupported array structure message
             if "unsupported" in x and "skipped variable" in x:
                 text = re.compile("skipped variable .*!")
-                bad_var = (
-                    text.findall(x)[0]
-                    .split(" ")[2]
-                    .replace("!", "")
-                )
+                bad_var = text.findall(x)[0].split(" ")[2].replace("!", "")
                 message = f"This variable's structure is not supported by CDO: {bad_var}. Full CDO warning: {x}"
                 warnings.warn(message)
                 warned = True
 
             if "warning" in x:
                 if "day 29feb not found" in x:
                     warnings.warn("No leap years found in data!")
@@ -935,15 +928,14 @@
         if len(self._hold_history) == len(self.history):
             self.history.append(os_command)
         else:
             self.history[-1] = os_command + " " + self.history[-1].replace("cdo ", " ")
             self.history[-1] = self.history[-1].replace("  ", " ")
     try:
         if self._execute:
-
             if ((output == "ensemble") and (len(self) > 1)) or (
                 (output == "ensemble") and (len(self) == 1)
             ):
                 new_history = copy.deepcopy(self._hold_history)
 
                 if len(self) == 1:
                     cores = 1
@@ -953,15 +945,15 @@
                     os_command = f'{os_command} {self.history[-1].replace("cdo ", " ")}'
                     os_command = os_command.replace("  ", " ")
 
                 if cores > 1:
                     original_sigint_handler = signal.signal(
                         signal.SIGTERM, signal.SIG_IGN
                     )
-                    pool = multiprocessing.Pool(cores)
+                    pool = mp.Pool(cores)
                     signal.signal(signal.SIGTERM, original_sigint_handler)
 
                     target_list = []
                     results = dict()
                 else:
                     target_list = []
 
@@ -1049,25 +1041,23 @@
                     if cores > 1:
                         temp = pool.apply_async(
                             run_cdo,
                             [ff_command, target, out_file, False, self._precision],
                         )
                         results[ff] = temp
                     else:
-
                         target = run_cdo(
                             ff_command, target, out_file, precision=self._precision
                         )
                         target_list.append(target)
                         if progress_bar:
                             if not suppress:
                                 pbar.update(1)
 
                 if cores > 1:
-
                     if progress_bar:
                         if session_info["progress"] == "on":
                             if not suppress:
                                 print("Processing ensemble. In progress:")
                         else:
                             if not suppress:
                                 print("Processing a large ensemble. In progress:")
@@ -1097,15 +1087,14 @@
                 self._ncommands = 0
 
                 self._format = None
 
                 return None
 
             if ((output == "one") and (len(self) > 1)) or self._zip is False:
-
                 new_history = copy.deepcopy(self._hold_history)
 
                 if len(self.history) > len(self._hold_history):
                     os_command = f'{os_command} {self.history[-1].replace("cdo ", " ")}'
                     os_command = os_command.replace("  ", " ")
 
                 # ensure there is sufficient space in /tmp if it is to be used
@@ -1166,28 +1155,26 @@
 
                 if "mergetime" in os_command:
                     try:
                         target = run_cdo(
                             os_command, target, out_file, precision=self._precision
                         )
                     except:
-
                         var_list = []
                         var_com = []
 
                         for ff in self:
                             var_list += nc_variables(ff)
                             var_com.append(nc_variables(ff))
                         new_list = []
 
                         for var in set(var_list):
                             if len(var_com) == len([x for x in var_com if var in x]):
                                 new_list.append(var)
                         if version_below(session_info["cdo"], "1.9.9"):
-
                             target = run_cdo(
                                 os_command, target, out_file, precision=self._precision
                             )
                         else:
                             f_list = ",".join(new_list)
                             os_command = os_command.replace(
                                 "-mergetime ", f'-mergetime -apply,"-selname,{f_list}" '
```

### Comparing `nctoolkit-0.9.2/nctoolkit/session.py` & `nctoolkit-0.9.3/nctoolkit/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 import glob
 import os
-from multiprocessing import Manager
+#from multiprocessing import Manager
+import multiprocessing
+import platform
 
 
 session_info = dict()
-mgr = Manager()
+if platform.system() == "Linux":
+    from multiprocessing import Manager
+    nc_safe_par = Manager().list()
+    temp_dirs_par = Manager().list()
+    nc_protected_par = Manager().list()
+else:
+    import multiprocess
+    from multiprocess import Manager
+    nc_safe_par = Manager().list()
+    temp_dirs_par = Manager().list()
+    nc_protected_par = Manager().list()
+
+#mgr = Manager()
 nc_safe = list()
-nc_safe_par = Manager().list()
+#nc_safe_par = Manager().list()
 
 
 def append_safe(ff):
     """
     Function to add a file to the safe list
     """
     if session_info["parallel"]:
@@ -72,15 +86,14 @@
     else:
         return nc_protected
 
 
 html_files = []
 
 temp_dirs = list()
-temp_dirs_par = Manager().list()
 
 
 def append_tempdirs(ff):
     """
     Function to add a file to the list of temp dirs used
     """
     if session_info["parallel"]:
@@ -98,15 +111,14 @@
     if session_info["parallel"]:
         return temp_dirs_par
     else:
         return temp_dirs
 
 
 nc_protected = list()
-nc_protected_par = Manager().list()
 
 
 def session_files():
     """
     Function to return the session files
     """
     candidates = []
```

### Comparing `nctoolkit-0.9.2/nctoolkit/setters.py` & `nctoolkit-0.9.3/nctoolkit/setters.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/shift.py` & `nctoolkit-0.9.3/nctoolkit/shift.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/show.py` & `nctoolkit-0.9.3/nctoolkit/show.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,33 +110,35 @@
     Function to get the variables available in a netCDF file
     """
 
     cdo_result = subprocess.run(
         f"cdo showname {ff}", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
     )
 
-    new = " ".join([
-    x
-    for x in [
-        x
-        for x in cdo_result.stdout.decode("utf-8").split("\n")
-        if "cdo" not in x and len(x) > 0
-    ]
-        if len(x) > 0
-    ])
+    new = " ".join(
+        [
+            x
+            for x in [
+                x
+                for x in cdo_result.stdout.decode("utf-8").split("\n")
+                if "cdo" not in x and len(x) > 0
+            ]
+            if len(x) > 0
+        ]
+    )
     return [x for x in new.split(" ") if len(x) > 0]
-    #return [
+    # return [
     #    x
     #    for x in [
     #        x
     #        for x in cdo_result.stdout.decode("utf-8").split("\n")
     #        if "cdo" not in x and len(x) > 0
     #    ][0].split(" ")
     #    if len(x) > 0
-    #]
+    # ]
 
 
 def nc_months(ff):
     """
     Function to get the months available in a netCDF file
     """
```

### Comparing `nctoolkit-0.9.2/nctoolkit/split.py` & `nctoolkit-0.9.3/nctoolkit/split.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     new_files = []
 
     commands = []
 
     bases = []
 
     for ff in self:
-
         # We need to split the file by name
         # But, first we need to check if there is space in the output folder
         # If there isn't, we need to switch to the /var/tmp
 
         if platform.system() == "Linux":
             if session_info["temp_dir"] == "/tmp/":
                 result = os.statvfs("/tmp/")
```

### Comparing `nctoolkit-0.9.2/nctoolkit/static_plot.py` & `nctoolkit-0.9.3/nctoolkit/static_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from nctoolkit.session import session_info
 
 try:
     import signal
     from contextlib import contextmanager
-    from nctoolkit.session import session_info
     from mpl_toolkits.axes_grid1 import make_axes_locatable
     import matplotlib as mpl
 
     from mpl_toolkits import axes_grid1
 
     from netCDF4 import Dataset
     import numpy as np
@@ -96,14 +95,15 @@
     if new_x == "(degC)":
         new_x = "(°C)"
     return new_x[1:-1]
 
 
 def pub_plot(
     ds,
+    var=None,
     extent=None,
     title=None,
     legend=None,
     size="auto",
     land="auto",
     colours="auto",
     norm=None,
@@ -120,37 +120,43 @@
 ):
     """
     Static plotting. This requires datasets to have regular latlon grids.
     Plots a static map, and requires only one variable, time step and vertical level
 
     Parameters
     -------------
+    ds: nctoolkit dataset
+        Dataset to plot
+    var: str
+        Variable to plot
     extent: list
-        List with [lon_min, lon_max, lat_min, lat_max] to limit the map extent
+        List with [lon_min, lon_max, lat_min, lat_max] for plotting extent
     title: str
         Character string with plot title
     legend: str
         Character string with legend title
     size: list
         List with [xsize, ysize] for plotting size
     land: str
         Character string with colour required for land. Set to None if you do not want land to show.
     norm: str or matplotlib.colors norm
          Norm to use for colour bar
-    mid_point: float
-        Mid-point to use for colour bar
     projection: cartopy projection
         Cartopy projection to use.
+    mid_point: float
+        Mid-point to use for colour bar
     coast: str
         Set to "coarse", "low", "intermediate", "high" or "full" if you want to use GSHHS coastlines
     scale: str
         "low", "medium" or "high"
     grid: bool
         Set to False if you do not want grid lines.
     legend_position = "auto"
+    robust :    bool
+        Whether to use robust statistics for the colour scale or not
     *kwargs:
         kwargs to allow slight misspelling of arguments
 
     -------------
     """
 
     if legend_position not in ["auto", "right", "bottom"]:
@@ -190,14 +196,19 @@
         "grid",
         "grid_colour",
         "legend_position",
     ]
 
     for kk in kwargs:
         fixed = False
+
+        if var is None:
+            if kk.lower().startswith("var"):
+                var = kwargs[kk]
+                fixed = True
         if kk.lower().startswith("col") and kk.lower().endswith("rs"):
             if colours == "viridis":
                 colours = kwargs[kk]
                 fixed = True
 
         if kk.lower().startswith("trans"):
             if norm == None:
@@ -231,14 +242,17 @@
                 raise ValueError(
                     f"{kk} is not a valid argument. Did you mean one of these? {part2}"
                 )
             else:
                 raise ValueError(f"{kk} is not a valid argument")
 
     ds1 = ds.copy()
+
+    if var is not None:
+        ds1.subset(variables=var)
     ds1.run()
 
     if len(ds1.variables) > 1:
         raise ValueError("Only one variable wanted")
     if len(ds1.times) > 1:
         raise ValueError("Only one timestep wanted")
```

### Comparing `nctoolkit-0.9.2/nctoolkit/strip_vars.py` & `nctoolkit-0.9.3/nctoolkit/strip_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,33 +16,30 @@
         individual or list of variables to select and strip. All variables will be stripped if this is not defined.
 
     """
 
     self.run()
 
     if vars is not None:
-
         if isinstance(vars, str):
             vars = [vars]
 
         for vv in vars:
             if vv not in self.variables:
                 raise ValueError(f"{vv} is not a valid variable!")
 
         command = f"ncks -C -v {str_flatten(vars)}"
 
     else:
-
         command = f"ncks -C -v {str_flatten(self.variables)}"
 
     new_files = []
     new_commands = []
 
     for ff in self:
-
         target = temp_file(".nc")
 
         the_command = f"{command} {ff} {target}"
 
         target = run_nco(the_command, target=target)
 
         new_files.append(target)
```

### Comparing `nctoolkit-0.9.2/nctoolkit/subset.py` & `nctoolkit-0.9.3/nctoolkit/subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 
 def fix_ind(x):
     if int(x) < 0:
         return int(x)
     else:
         return int(x) + 1
 
+
 def is_iterable(x):
-    try: 
+    try:
         y = iter(x)
         return True
     except:
         return False
 
 
 def to_date(x):
@@ -31,14 +32,15 @@
     if len(new) != 3:
         raise ValueError(f"{x} could not be parsed")
     day = int(new[0])
     month = int(new[1])
     year = int(new[2])
     return datetime(year, month, day)
 
+
 def select_levels(self, levels=None):
     """
     Select season from a dataset
 
     Parameters
     -------------
     levels : list
@@ -55,18 +57,18 @@
         try:
             levels[0] = int(np.floor(float(levels[0])))
             levels[1] = int(np.ceil(float(levels[1])))
         except:
             raise ValueError("levels provided are not valid!")
         if levels[0] > levels[1]:
             raise ValueError("levels have the wrong order")
-        levels = f"{levels[0]}/{levels[1]}" 
+        levels = f"{levels[0]}/{levels[1]}"
+
+    cdo_command = f"cdo -sellevel,{levels}"
 
-    cdo_command =  f"cdo -sellevel,{levels}"
-        
     run_this(cdo_command, self, "ensemble")
 
 
 def select_period(self, period=None):
     """
     Select season from a dataset
 
@@ -121,14 +123,15 @@
 
     if season not in ["DJF", "MAM", "JJA", "SON"]:
         raise ValueError("Invalid season supplied")
 
     cdo_command = f"cdo -select,season={season}"
     run_this(cdo_command, self, output="ensemble")
 
+
 def select_hours(self, hours=None):
     """
     Select hours from a dataset
     This method will subset the dataset to only contain hours within the list given.
     A warning message will be provided when there are missing hours.
 
     Parameters
@@ -148,15 +151,14 @@
         hours = [hours]
     # all of the variables in hours need to be converted to ints,
     # just in case floats have been provided
     # coerce to int if numpy float etc.
 
     hours = [int(x) if "int" in str(type(x)) else x for x in hours]
 
-
     for x in hours:
         if not isinstance(x, int):
             raise TypeError(f"{x} is not an int")
         if x not in list(range(1, 32)):
             raise ValueError(f"{x} is not a hour")
 
     hours = str_flatten(hours, ",")
@@ -188,15 +190,14 @@
         days = [days]
     # all of the variables in days need to be converted to ints,
     # just in case floats have been provided
     # coerce to int if numpy float etc.
 
     days = [int(x) if "int" in str(type(x)) else x for x in days]
 
-
     for x in days:
         if not isinstance(x, int):
             raise TypeError(f"{x} is not an int")
         if x not in list(range(1, 32)):
             raise ValueError(f"{x} is not a day")
 
     days = str_flatten(days, ",")
@@ -228,15 +229,14 @@
         months = [months]
     # all of the variables in months need to be converted to ints,
     # just in case floats have been provided
     # coerce to int if numpy float etc.
 
     months = [int(x) if "int" in str(type(x)) else x for x in months]
 
-
     for x in months:
         if not isinstance(x, int):
             raise TypeError(f"{x} is not an int")
         if x not in list(range(1, 13)):
             raise ValueError(f"{x} is not a month")
 
     months = str_flatten(months, ",")
@@ -270,30 +270,27 @@
     years = [int(x) if "int" in str(type(x)) else x for x in years]
 
     for yy in years:
         if not isinstance(yy, int):
             raise TypeError(f"{yy} is not an int")
 
     if self._merged is False:
-
         missing_files = 0
 
         n_removed = 0
 
         # loop through all of the files and remove any that do not have valid years
         new_current = []
 
-
         all_check = []
 
         for ff in self:
-
             all_years = nc_years(ff)
             all_years = list(set(all_years))
-            all_check+=all_years
+            all_check += all_years
             all_years = [int(v) for v in all_years]
             inter = [element for element in all_years if element in years]
 
             if len(inter) > 0:
                 new_current.append(ff)
             if len(inter) == 0:
                 n_removed += 1
@@ -314,27 +311,35 @@
                 + " files did not have valid years, so were removed from the dataset!"
             )
 
         missing_years = [str(x) for x in years if x not in all_years]
         if len(missing_years) > 0:
             len_missing = len(missing_years)
             missing_years = [int(x) for x in missing_years]
-            if set(range(min(missing_years), max(missing_years) + 1)) == set(missing_years):
+            if set(range(min(missing_years), max(missing_years) + 1)) == set(
+                missing_years
+            ):
                 if len(missing_years) > 1:
-                    missing_years = str(min(missing_years)) + "-" + str(max(missing_years))
+                    missing_years = (
+                        str(min(missing_years)) + "-" + str(max(missing_years))
+                    )
                 else:
                     missing_years = str(missing_years[0])
             else:
                 missing_years = [str(x) for x in missing_years]
                 missing_years = str_flatten(missing_years, ",")
             if missing_files == 0:
                 if len_missing == 1:
-                    warnings.warn(f"The following year was not available in the dataset: {missing_years}")
+                    warnings.warn(
+                        f"The following year was not available in the dataset: {missing_years}"
+                    )
                 else:
-                    warnings.warn(f"{len_missing} years were not available in the dataset: {missing_years}")
+                    warnings.warn(
+                        f"{len_missing} years were not available in the dataset: {missing_years}"
+                    )
 
         self.current = new_current
 
         if missing_files > 0:
             years = str_flatten(years, ",")
 
             cdo_command = f"cdo -selyear,{years}"
@@ -397,24 +402,25 @@
 
     if times is None:
         raise ValueError("Please supply times")
 
     if isinstance(times, range):
         times = list(times)
 
-
     if not isinstance(times, list):
         times = [times]
 
     for tt in times:
         if not isinstance(tt, int):
             raise TypeError(f"{tt} is not an int")
         if tt < 0:
             if version_above(cdo_version(), "2.0.0") is False:
-                raise ValueError(f"Please install CDO version 2.0.5 or above for negative timestep selections")
+                raise ValueError(
+                    f"Please install CDO version 2.0.5 or above for negative timestep selections"
+                )
 
     # all of the variables in months need to be converted to ints,
     # just in case floats have been provided
 
     times = [fix_ind(x) for x in times]
     times = [str(x) for x in times]
     times = str_flatten(times)
@@ -502,33 +508,32 @@
         if is_iterable(kwargs[kk]):
             ints = True
             for x in kwargs[kk]:
                 try:
                     y = int(x)
                 except:
                     ints = False
-                
+
                 if ints:
                     kwargs[kk] = kwargs[kk]
 
     non_selected = True
 
     lon = None
     lat = None
     for key in kwargs:
         if "lon" in key.lower():
             lon = kwargs[key]
         if "lat" in key.lower():
             lat = kwargs[key]
     if lon is not None or lat is not None:
-        self.crop(lon = lon, lat = lat)
+        self.crop(lon=lon, lat=lat)
         non_selected = False
 
     for key in kwargs:
-
         if "ran" in key.lower():
             select_period(self, kwargs[key])
             non_selected = False
 
         if "var" in key.lower():
             select_variables(self, kwargs[key])
             non_selected = False
@@ -557,10 +562,9 @@
             select_hours(self, kwargs[key])
             non_selected = False
 
         if "lev" in key.lower() or "depth" in key.lower():
             select_levels(self, kwargs[key])
             non_selected = False
 
-
     if non_selected:
         raise AttributeError(f"{key} is not a valid select method")
```

### Comparing `nctoolkit-0.9.2/nctoolkit/sumall.py` & `nctoolkit-0.9.3/nctoolkit/sumall.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,28 @@
 
     self.run()
 
     contents = self.contents
 
     easy = True
     if len(self) > 1:
-        for x in self.contents.reset_index().loc[:,["file", "variable"]].groupby("variable").size().values:
+        for x in (
+            self.contents.reset_index()
+            .loc[:, ["file", "variable"]]
+            .groupby("variable")
+            .size()
+            .values
+        ):
             if x != len(self):
                 easy = False
 
     if (len(self) > 1 and easy is False) and (self._merged is False):
-        raise TypeError("This currently only works for datasets with files with the same variables")
+        raise TypeError(
+            "This currently only works for datasets with files with the same variables"
+        )
 
     if drop is True:
         self.cdo_command("expr,total=" + "+".join(self.variables))
 
     else:
         if "total" not in self.variables:
             self.cdo_command("aexpr,total=" + "+".join(self.variables))
```

### Comparing `nctoolkit-0.9.2/nctoolkit/temp_file.py` & `nctoolkit-0.9.3/nctoolkit/temp_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
         append_tempdirs(os.path.dirname(target))
 
         return target
 
     # osx approach
     else:
-
         target = tempfile.NamedTemporaryFile().name
 
         if not isinstance(ext, str):
             raise TypeError("Extension supplied is not a str")
         if ext.startswith("."):
             target = target + ext
         else:
```

### Comparing `nctoolkit-0.9.2/nctoolkit/temporal_stat.py` & `nctoolkit-0.9.3/nctoolkit/temporal_stat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import copy
 
 from nctoolkit.cleanup import cleanup
 from nctoolkit.runthis import run_this, run_cdo, tidy_command
 from nctoolkit.temporals import *
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import remove_safe
-import warnings
 
 
 def time_stat(self, stat="mean", over="time"):
     """Method to calculate a stat over all time steps"""
     # create cdo command and run it
 
     if len(self) == 0:
@@ -63,15 +62,15 @@
         return None
 
     if over == ["day", "hour"]:
         run = True
         yhourstat(self, stat=stat)
         return None
 
-    if over == ["day", "hour",  "year"]:
+    if over == ["day", "hour", "year"]:
         run = True
         hourstat(self, stat=stat)
         return None
 
     if over == ["hour"]:
         run = True
         dhourstat(self, stat=stat)
@@ -114,30 +113,29 @@
         run = True
         monstat(self, stat=stat)
         return None
     if run is False:
         raise ValueError(f"Grouping {over} is currently not supported!")
 
 
-
-def tsum(self, over="time", align = "right"):
+def tsum(self, over="time", align="right"):
     """
     Calculate the temporal sum of all variables
 
     Parameters
     -------------
     align = str
         This determines whether the output time is at the left, centre or right hand side of the time window.
         Options are "left", "centre" and "right"
     """
     self.align(align)
     time_stat(self, stat="sum", over=over)
 
 
-def na_count(self, over="time", align = "right"):
+def na_count(self, over="time", align="right"):
     """
     Calculate the number of missing values
 
     Parameters
     -------------
     over: str or list
         Time periods to to the count over over. Options are 'time', 'year', 'month', 'day'.
@@ -152,15 +150,15 @@
 
     for vv in self.variables:
         self.cdo_command(f"-aexpr,'{vv}=isMissval({vv})'")
 
     self.tsum(over=over)
 
 
-def na_frac(self, over="time", align = "right"):
+def na_frac(self, over="time", align="right"):
     """
     Calculate the number of missing values
 
     Parameters
     -------------
     over: str or list
         Time periods to to the count over over. Options are 'time', 'year', 'month', 'day'.
@@ -175,15 +173,15 @@
 
     for vv in self.variables:
         self.cdo_command(f"-aexpr,'{vv}=isMissval({vv})'")
 
     self.tmean(over=over)
 
 
-def tmean(self, over="time", align = "right"):
+def tmean(self, over="time", align="right"):
     """
     Calculate the temporal mean of all variables
 
     Parameters
     -------------
     over: str or list
         Time periods to average over. Options are 'year', 'month', 'day'.
@@ -217,19 +215,19 @@
 
     A daily climatological mean would be the following:
 
         >>> ds.tmean( "day")
 
 
     """
-    self.align(align = align)
+    self.align(align=align)
     time_stat(self, stat="mean", over=over)
 
 
-def tmin(self, over="time", align = "right"):
+def tmin(self, over="time", align="right"):
     """
     Calculate the temporal minimum of all variables
 
     Parameters
     -------------
     over: str or list
         Time periods to average over. Options are 'year', 'month', 'day'.
@@ -262,19 +260,19 @@
         >>> ds.tmin( "month")
 
     A daily climatological minimum would be the following:
 
         >>> ds.tmin( "day")
 
     """
-    self.align(align = align)
+    self.align(align=align)
     time_stat(self, stat="min", over=over)
 
 
-def tmax(self, over="time", align = "right"):
+def tmax(self, over="time", align="right"):
     """
     Calculate the temporal maximum of all variables
 
     Parameters
     -------------
     over: str or list
         Time periods to average over. Options are 'year', 'month', 'day'.
@@ -305,19 +303,19 @@
 
         >>> ds.tmax( "month")
 
     A daily climatological maximum would be the following:
 
         >>> ds.tmax( "day")
     """
-    self.align(align = align)
+    self.align(align=align)
     time_stat(self, stat="max", over=over)
 
 
-def tmedian(self, over="time", align = "right"):
+def tmedian(self, over="time", align="right"):
     """
     Calculate the temporal median of all variables
 
     Parameters
     -------------
     over: str or list
         Time periods to average over. Options are 'year', 'month', 'day'.
@@ -348,19 +346,19 @@
 
         >>> ds.tmedian( "month")
 
     A daily climatological median would be the following:
 
         >>> ds.tmedian( "day")
     """
-    self.align(align = align)
+    self.align(align=align)
     self.tpercentile(p=50, over=over)
 
 
-def trange(self, over="time", align = "right"):
+def trange(self, over="time", align="right"):
     """
     Calculate the temporal range of all variables
 
     Parameters
     -------------
     over: str or list
         Time periods to average over. Options are 'year', 'month', 'day'.
@@ -392,19 +390,19 @@
         >>> ds.trange( "month")
 
     A daily climatological range would be the following:
 
         >>> ds.trange( "day")
 
     """
-    self.align(align = align)
+    self.align(align=align)
     time_stat(self, stat="range", over=over)
 
 
-def tvar(self, over="time", align = "right"):
+def tvar(self, over="time", align="right"):
     """
     Calculate the temporal variance of all variables
 
     Parameters
     -------------
     over: str or list
         Time periods to average over. Options are 'year', 'month', 'day'.
@@ -436,19 +434,19 @@
 
         >>> ds.tvar( "month")
 
     A daily climatological variance would be the following:
 
         >>> ds.tvar( "day")
     """
-    self.align(align = align)
+    self.align(align=align)
     time_stat(self, stat="var", over=over)
 
 
-def tstdev(self, over="time", align = "right"):
+def tstdev(self, over="time", align="right"):
     """
     Calculate the temporal standard deviation of all variables
 
     Parameters
     -------------
     over: str or list
         Time periods to average over. Options are 'year', 'month', 'day'.
@@ -480,19 +478,19 @@
 
         >>> ds.tstdev("month")
 
     A daily climatological standard deviation would be the following:
 
         >>> ds.tstdev("day")
     """
-    self.align(align = align)
+    self.align(align=align)
     time_stat(self, stat="std", over=over)
 
 
-def tcumsum(self, align = "right"):
+def tcumsum(self, align="right"):
     """
     Calculate the temporal cumulative sum of all variables
 
     Parameters
     -------------
     align: str
         This determines whether the output time is at the left, centre or right hand side of the time window.
@@ -506,15 +504,15 @@
 
     """
     self.align(align=align)
     # create cdo command and runit
     time_stat(self, stat="cumsum")
 
 
-def tpercentile(self, p=None, over="time", align = "right"):
+def tpercentile(self, p=None, over="time", align="right"):
     """
     Calculate the temporal percentile of all variables
 
     Parameters
     -------------
     p: float or int
         Percentile to calculate
@@ -621,16 +619,16 @@
 
     new_files = []
     new_commands = []
     for ff in self:
         target = temp_file("nc")
 
         cdo_command = (
-                perc_term
-            #"cdo -timpctl,"
+            perc_term
+            # "cdo -timpctl,"
             + str(p)
             + " "
             + ff
             + min_command
             + ff
             + max_command
             + ff
```

### Comparing `nctoolkit-0.9.2/nctoolkit/temporals.py` & `nctoolkit-0.9.3/nctoolkit/temporals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from nctoolkit.runthis import run_this
 
+
 def hourstat(self, stat="mean"):
     """Method to calculate the hourly statistic from a function"""
 
     cdo_command = f"cdo -hour{stat}"
 
     run_this(cdo_command, self, output="ensemble")
 
+
 def yhourstat(self, stat="mean"):
     """Method to calculate the hourly statistic from a function"""
 
     cdo_command = f"cdo -yhour{stat}"
 
     run_this(cdo_command, self, output="ensemble")
 
+
 def dhourstat(self, stat="mean"):
     """Method to calculate the hourly statistic from a function"""
 
     cdo_command = f"cdo -dhour{stat}"
 
     run_this(cdo_command, self, output="ensemble")
 
+
 def ymonstat(self, stat="mean"):
     """Method to calculate the seasonal statistic from a function"""
 
     cdo_command = f"cdo -ymon{stat}"
 
     run_this(cdo_command, self, output="ensemble")
```

### Comparing `nctoolkit-0.9.2/nctoolkit/thresholds.py` & `nctoolkit-0.9.3/nctoolkit/thresholds.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.gt(x)
         run_code = True
 
     if run_code:
         self.rename({self.variables[0]: "target"})
         self.as_missing([-1, 0.1])
         if old:
-            self.assign( new=lambda x: (x.target == x.target) * (timestep(x.target) + 1), drop=True)
+            self.assign( new=lambda x: (x.target == x.target) * (timestep(x.target) + 1), drop=True,)
         else:
             self.assign( new=lambda x: (x.target == x.target) * (timestep() + 1), drop=True)
         self.as_missing([0, 0.01])
         self.tmin()
         self.assign(first=lambda x: int(x.new) - 1, drop=True)
         self.rename({"first": variable})
         self.run()
@@ -127,15 +127,15 @@
             x.run()
         self.lt(x)
         run_code = True
     if run_code:
         self.rename({self.variables[0]: "target"})
         self.as_missing([-1, 0.1])
         if old:
-            self.assign( new=lambda x: (x.target == x.target) * (timestep(x.target) + 1), drop=True)
+            self.assign( new=lambda x: (x.target == x.target) * (timestep(x.target) + 1), drop=True,)
         else:
             self.assign( new=lambda x: (x.target == x.target) * (timestep() + 1), drop=True)
         self.as_missing([0, 0.01])
         self.tmin()
         self.assign(first=lambda x: int(x.new) - 1, drop=True)
         self.rename({"first": variable})
         self.run()
@@ -201,15 +201,15 @@
         self.gt(x)
         run_code = True
 
     if run_code:
         self.rename({self.variables[0]: "target"})
         self.as_missing([-1, 0.1])
         if old:
-            self.assign( new=lambda x: (x.target == x.target) * (timestep(x.target) + 1), drop=True)
+            self.assign( new=lambda x: (x.target == x.target) * (timestep(x.target) + 1), drop=True,)
         else:
             self.assign( new=lambda x: (x.target == x.target) * (timestep() + 1), drop=True)
         self.as_missing([0, 0.01])
         self.multiply(-1)
         self.tmin()
         self.multiply(-1)
         self.assign(last=lambda x: int(x.new) - 1, drop=True)
@@ -277,15 +277,15 @@
         self.lt(x)
         run_code = True
 
     if run_code:
         self.rename({self.variables[0]: "target"})
         self.as_missing([-1, 0.1])
         if old:
-            self.assign( new=lambda x: (x.target == x.target) * -1 * (timestep(x.target) + 1), drop=True)
+            self.assign( new=lambda x: (x.target == x.target) * -1 * (timestep(x.target) + 1), drop=True,)
         else:
             self.assign( new=lambda x: (x.target == x.target) * -1 * (timestep() + 1), drop=True)
         self.as_missing([0, 0.01])
         self.assign(new=lambda x: int(x.new))
         self.tmin()
         self.multiply(-1)
         self.assign(new=lambda x: int(x.new))
```

### Comparing `nctoolkit-0.9.2/nctoolkit/to_lonlat.py` & `nctoolkit-0.9.3/nctoolkit/to_lonlat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.2/nctoolkit/to_nc.py` & `nctoolkit-0.9.3/nctoolkit/to_nc.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         raise ValueError("You cannot save an empty dataset!")
 
     if os.path.basename(out) != out:
         out_dir = os.path.dirname(out)
         if os.path.exists(out_dir) is False:
             raise ValueError(f"{out_dir} does not exist!")
 
-
     # Figure out if it is possible to write the file, i.e. if a dataset is still an
     # ensemble, you cannot write.
     ff = copy.deepcopy(self.current)
     write = False
 
     if len(self) == 1:
         write = True
@@ -67,47 +66,49 @@
     if write is False:
         raise ValueError("You cannot save multiple files!")
 
     if (os.path.exists(out)) and (overwrite is True):
         if len(self) > 1:
             self.run()
 
-
     # Check if outfile exists and overwrite is set to False
     # This should maybe be a warning, not an error
     if (os.path.exists(out)) and (overwrite is False):
         raise ValueError("The out file exists and overwrite is set to false")
 
-
     if len(kwargs) > 0:
-
         self1 = self.copy()
 
         self1.subset(**kwargs)
 
         self1.run()
         ff = copy.deepcopy(self1.current)
 
-
         if len(self1.history) == len(self1._hold_history):
             if zip:
                 cdo_command = f"cdo -z zip_9 copy {ff[0]} {out}"
                 run_cdo(
-                    cdo_command, target=out, overwrite=overwrite, precision=self._precision
+                    cdo_command,
+                    target=out,
+                    overwrite=overwrite,
+                    precision=self._precision,
                 )
 
                 self1.history.append(cdo_command)
                 self1._hold_history = copy.deepcopy(self1.history)
                 self1.current = out
                 remove_safe(out)
 
             else:
                 cdo_command = f"cdo copy {ff[0]} {out}"
                 run_cdo(
-                    cdo_command, target=out, overwrite=overwrite, precision=self1._precision
+                    cdo_command,
+                    target=out,
+                    overwrite=overwrite,
+                    precision=self1._precision,
                 )
                 self1.history.append(cdo_command)
                 self1._hold_history = copy.deepcopy(self1.history)
 
                 self1.current = out
                 remove_safe(out)
 
@@ -121,33 +122,37 @@
 
             run_this(cdo_command, self1, out_file=out)
             self1._execute = False
 
         if os.path.exists(out) is False:
             raise ValueError("File zipping was not successful")
     else:
-
         ff = copy.deepcopy(self.current)
 
         if len(self.history) == len(self._hold_history):
             if zip:
                 cdo_command = f"cdo -z zip_9 copy {ff[0]} {out}"
                 run_cdo(
-                    cdo_command, target=out, overwrite=overwrite, precision=self._precision
+                    cdo_command,
+                    target=out,
+                    overwrite=overwrite,
+                    precision=self._precision,
                 )
                 self.history.append(cdo_command)
                 self._hold_history = copy.deepcopy(self.history)
                 self.current = out
                 remove_safe(out)
 
-
             else:
                 cdo_command = f"cdo copy {ff[0]} {out}"
                 run_cdo(
-                    cdo_command, target=out, overwrite=overwrite, precision=self._precision
+                    cdo_command,
+                    target=out,
+                    overwrite=overwrite,
+                    precision=self._precision,
                 )
                 self.history.append(cdo_command)
                 self._hold_history = copy.deepcopy(self.history)
 
                 self.current = out
                 remove_safe(out)
 
@@ -161,9 +166,8 @@
             run_this(cdo_command, self, out_file=out)
             self._execute = False
             self.current = out
 
         if os.path.exists(out) is False:
             raise ValueError("File zipping was not successful")
 
-
     cleanup()
```

### Comparing `nctoolkit-0.9.2/nctoolkit/toxarray.py` & `nctoolkit-0.9.3/nctoolkit/toxarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     #   3: decode_times is True, but xarray cannot decodes times - open in xarray,
     #   then use cdo to get the times
 
     # All commands need to be run before opening it xarray
     if len(kwargs) == 0:
         self.run()
 
-
     self1 = self.copy()
 
     if len(kwargs) > 0:
         self1.subset(**kwargs)
         self1.run()
 
     # if you don't want to decode times, this is straight forward. Just open the data
@@ -86,15 +85,14 @@
             data = xr.open_mfdataset(self1.current, decode_times=decode_times)
         return data
 
     # If it does not, then we use cdo to pull out the times,
     # then push those to the xarray object
 
     if len(self1) == 1:
-
         if isinstance(self1.times[0], datetime):
             times = self1.times
         else:
             times = [
                 datetime.strptime(ss.replace("T", " "), "%Y-%m-%d %H:%M:%S")
                 for ss in self1.times
             ]
```

### Comparing `nctoolkit-0.9.2/nctoolkit/tozlev.py` & `nctoolkit-0.9.3/nctoolkit/tozlev.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-import copy
-import subprocess
-import warnings
-import os
-
 from nctoolkit.api import open_data
-from nctoolkit.cleanup import cleanup
-from nctoolkit.flatten import str_flatten
-from nctoolkit.runthis import run_this, run_cdo
+from nctoolkit.runthis import run_cdo
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import append_safe
 from nctoolkit.session import remove_safe
-from nctoolkit.session import get_safe
 import nctoolkit.api as api
 
-def to_zlevels(self, levels = None, thickness = None):
+
+def to_zlevels(self, levels=None, thickness=None):
     """
-    Convert datasets with non z-level verticals to z-levels 
+    Convert datasets with non z-level verticals to z-levels
     Experimental method: Use at your own risk.
 
 
     Parameters
     -------------
     levels: list
         List of new z-levels. Must be positive and in metres.
@@ -72,65 +65,62 @@
             ds_depths.run()
             drop_this = thickness
         else:
             ds_depths = open_data(thickness)
             if len(ds_depths.variables) != 1:
                 raise ValueError("Please provide a thickness file with 1 variable!")
 
-
     thick_var = ds_depths.variables[0]
 
     ds_depths.rename({thick_var: "thickness"})
     ds_depths.cdo_command("setmisstoc,1.0")
     ds_depths.run()
     ds_thick = ds_depths.copy()
     ds_thick.divide(2)
     ds_depths.vertical_cumsum()
     ds_depths.rename({"thickness": "depth"})
     ds_depths.subtract(ds_thick)
-    ds_depths.assign(depth = lambda x: x.depth * (vertical_min(x.depth) < x.depth) * (isnan(x.depth) == False), drop = True)
-    ds_depths.subset(times = 0)
+    ds_depths.assign( depth=lambda x: x.depth * (vertical_min(x.depth) < x.depth) * (isnan(x.depth) == False), drop=True,)
+    ds_depths.subset(times=0)
     ds_depths.cdo_command("setmisstoc,-9999999")
     ds_depths.run()
 
     zaxis = temp_file().replace(".", "")
     append_safe(zaxis)
 
     if not isinstance(levels, list):
         raise TypeError("levels must be a list")
 
     for ll in levels:
         if ll < 0:
             raise ValueError("levels must not have negative values")
 
-
     line3 = "levels = " + " ".join([str(x) for x in levels]) + " \n"
-    with open(zaxis, 'a') as the_file:
-        x = the_file.write('zaxistype = depth_below_sea \n')
-        x = the_file.write(f'size = {len(levels)} \n')
+    with open(zaxis, "a") as the_file:
+        x = the_file.write("zaxistype = depth_below_sea \n")
+        x = the_file.write(f"size = {len(levels)} \n")
         x = the_file.write(line3)
 
     target = ds_depths.copy()
-    target.assign(depth = lambda x: level(x.depth) + 0 * (x.depth == x.depth), drop = True)
+    target.assign(depth=lambda x: level(x.depth) + 0 * (x.depth == x.depth), drop=True)
     target.run()
 
-    target.vertical_interp(levels = levels, fixed = True)
-    target.assign(depth = lambda x: level(x.depth) + 0 * (x.depth == x.depth), drop = True)
+    target.vertical_interp(levels=levels, fixed=True)
+    target.assign(depth=lambda x: level(x.depth) + 0 * (x.depth == x.depth), drop=True)
     target.run()
 
     out = temp_file(".nc")
     append_safe(out)
 
     command = f"cdo intlevel3d,{target[0]} {ds[0]}  {ds_depths[0]} {out}"
 
-    run_cdo(command, target = out, precision = self._precision)
+    run_cdo(command, target=out, precision=self._precision)
 
     test = open_data(out)
     test.cdo_command(f"setzaxis,{zaxis}")
-    test.subset(variables = vars)
+    test.subset(variables=vars)
     test.run()
     self.current = test.current
 
     remove_safe(out)
     remove_safe(out)
     remove_safe(zaxis)
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/unify.py` & `nctoolkit-0.9.3/nctoolkit/unify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import pandas as pd
 import re
 import warnings
 
 
 def is_number(s):
     try:
@@ -43,54 +42,52 @@
     if len(df.loc[:, ["month"]].drop_duplicates()) == len(df):
         return ["month"]
 
     if len(df.loc[:, ["year", "month"]].drop_duplicates()) == len(df):
         return ["year", "month"]
 
 
-
-def unify(x=None, y=None, ignore = None, clim = False, **kwargs):
+def unify(x=None, y=None, ignore=None, clim=False, **kwargs):
     """
-    Unify datasets temporally and spatially 
+    Unify datasets temporally and spatially
     Experimental feature: use at your own risk!
 
     Parameters
     -------------
     x: dataset
         First dataset to use
     y: dataset
         Second dataset to use
     ignore: list
         List, made up of "time" and "grid", "levels" of dimensions to ignore.
     clim: bool
         Set to True if one of the variables is a climatology. Default is False.
-        
+
     """
 
     if not isinstance(x, api.DataSet):
         raise TypeError("Please check x is a dataset")
 
     if not isinstance(y, api.DataSet):
         raise TypeError("Please check y is a dataset")
         # make sure everything has been evaluated
 
     x.run()
     y.run()
 
-    #if len(x) > 1 or len(y) > 1:
+    # if len(x) > 1 or len(y) > 1:
     #    raise TypeError("cor_time only accepts single file datasets!")
 
     a = x.copy()
     b = y.copy()
 
     unify_time = True
     unify_grid = True
     unify_levels = True
 
-
     if ignore is not None:
         if isinstance(ignore, str):
             ignore = [ignore]
 
         if len(ignore) == 0:
             checked = True
         checked = False
@@ -105,19 +102,17 @@
                 checked = True
 
         for ii in ignore:
             if "level" in ii.lower():
                 unify_levels = False
                 checked = True
 
-
             if checked is False:
                 raise ValueError(f"ignore is not valid: {ignore}")
 
-
     if unify_time:
         a_times = a.times
         b_times = b.times
 
         a_times_df = pd.DataFrame(
             {
                 "year": [x.year for x in a_times],
@@ -135,15 +130,14 @@
         )
 
         # If the years do not match, we will need to get them to match...
 
         b_years = list(set(b_times_df["year"]))
         a_years = list(set(a_times_df["year"]))
         if a_years != b_years:
-
             if len(b_years) > 1 and len(b_years) > 1:
                 years = [x for x in b_years if x in a_years]
                 f_years = ",".join([str(y) for y in years])
                 print(f"Selecting matching years {f_years}")
 
                 b.subset(years=years)
                 a.subset(years=years)
@@ -153,71 +147,69 @@
         a_months = list(set(a_times_df["month"]))
         if len(a) > 1:
             a.merge("time")
 
         if len(b) > 1:
             b.merge("time")
 
-
         if a_months != b_months:
-
             if len(b_months) > 1 and len(b_months) > 1:
                 months = [x for x in b_months if x in a_months]
                 f_months = ",".join([str(y) for y in months])
                 print(f"Selecting matching months {f_months}")
                 if b_months != months:
                     b.subset(months=months)
                 if a_months != months:
                     a.subset(months=months)
 
-
     if unify_levels:
         if len(a.levels) >= 1 and len(b.levels) > 1:
             run = False
             try:
-                b.vertical_interp(levels= a.levels)
+                b.vertical_interp(levels=a.levels)
                 run = True
             except:
-                warnings.warn("Unable to interpolate vertically. Original vertical levels are maintained!")
+                warnings.warn(
+                    "Unable to interpolate vertically. Original vertical levels are maintained!"
+                )
             if run:
-                print("Vertically interpolating the second dataset to the first dataset's levels!")
+                print(
+                    "Vertically interpolating the second dataset to the first dataset's levels!"
+                )
         if len(a.levels) > 1 and len(b.levels) == 1:
             print("Only one level in second dataset. Unable to vertically interpolate!")
 
-
     a.run()
 
     # Regrid to the bervational dataset
 
     fix_nemo = False
     for kk in kwargs:
         if kk.lower() == "amm7":
             if kwargs[kk]:
                 fix_nemo = True
 
-
     if fix_nemo:
         a.fix_nemo_ersem_grid()
 
-    #try:
+    # try:
     #    b.fix_nemo_ersem_grid()
-    #except:
+    # except:
     #    whatever = "Not the dev version of nctoolkit"
 
     if unify_grid:
         print("Horizontally regridding the second dataset to the first dataset's grid")
         b.regrid(a)
 
     if unify_time:
         if True:
             mod_ag = get_type(a_times_df)
             b_ag = get_type(b_times_df)
 
             if mod_ag != b_ag:
-
                 ag = [x for x in mod_ag if x in b_ag]
 
                 if ag == []:
                     if "year" in mod_ag or "year" in b_ag:
                         ag = ["year"]
 
                 if ag == []:
@@ -227,15 +219,16 @@
                 if ag == []:
                     raise ValueError("not working")
 
                 if True:
                     if ag == ["month"]:
                         if clim:
                             print("Using a monthly climatology for matchups!")
-                        else: ag = ["year", "month"]
+                        else:
+                            ag = ["year", "month"]
 
                     if ag == ["yearly"]:
                         print("Using an annual climatology for matchups!")
 
                     if ag == ["daily"]:
                         if clim:
                             print("Using a daily climatology for matchups!")
@@ -250,15 +243,14 @@
 
             aggregation = ag
 
             a.run()
             b.run()
 
         if len(a.times) != len(b.times):
-
             if True:
                 if ag == ["year", "month"]:
                     mod_times = (
                         get_timedf(a)
                         .loc[:, ["month", "year"]]
                         .reset_index()
                         .rename(columns={"index": "a_index"})
@@ -321,25 +313,19 @@
                     b_index = [int(x) for x in indices.b_index]
 
                     a.subset(times=mod_index)
                     b.subset(times=b_index)
 
                     print("Only selecting matching days!")
 
-
         a.run()
         b.run()
 
-
         if len(a.times) != len(b.times):
             raise ValueError("Problems matching times")
 
-
     x.current = a.current
     y.current = b.current
     x.history.append(a.history)
     y.history.append(b.history)
     x._hold_history.append(a._hold_history)
     y._hold_history.append(b._hold_history)
-
-
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/utils.py` & `nctoolkit-0.9.3/nctoolkit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import subprocess
 
-def name_check(x):
 
+def name_check(x):
     if len(x) == 0:
         return False
 
     if " " in x:
         return False
 
     text = re.compile(".*[+,/,-,*]")
@@ -24,15 +24,14 @@
 
     if text.match(x):
         return True
     else:
         return False
 
 
-
 def is_curvilinear(ff):
     """
     Function to work out if a file contains a curvilinear grid
     """
     cdo_result = subprocess.run(
         f"cdo sinfo {ff}", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
     )
@@ -67,48 +66,53 @@
     y = int(y[0]) * 1000 + int(y[1]) * 100 + int(y[2])
 
     return x > y
 
 
 # check version of cdo installed
 
+
 def latest_version():
     try:
         import requests
-    
+
         url = "https://anaconda.org/conda-forge/cdo"
         r = requests.get(url)
         import re
+
         text = re.compile("v.*..*..[0-10]")
-    
+
         text = re.compile("v[0-9].[0-9]?[0-9].[0-9]?[0-9]")
         options = []
         for x in [text.findall(x) for x in r.text.split(" ") if "2.0.5" in x]:
             options += x
-    
+
         versions = []
         for x in options:
             versions.append(x.replace("v", ""))
         versions = list(set(versions))
-        if  len(versions) == 1:
+        if len(versions) == 1:
             return versions[0]
         else:
             return None
     except:
         return None
 
+
 def validate_version():
     """
     Function to tell the user whether a valid version of CDO is installed
     """
     bad = False
 
     try:
         version = cdo_version()
-        bad = version_above(cdo_version(), "2.0.0") and version_below(cdo_version(), "2.0.5")
+        bad = version_above(cdo_version(), "2.0.0") and version_below(
+            cdo_version(), "2.0.5"
+        )
         actual_version = version
         if version is None:
             print(
                 "Please install CDO version 1.9.7 or above: https://code.mpimet.mpg.de/projects/cdo/ or https://anaconda.org/conda-forge/cdo"
             )
         sub = "."
         wanted = ""
@@ -122,25 +126,30 @@
         after = after.replace(sub, wanted)
         if version_below(cdo_version(), "1.9.7"):
             print(
                 "Please install CDO version 1.9.7 or above: https://code.mpimet.mpg.de/projects/cdo/ or https://anaconda.org/conda-forge/cdo"
             )
         else:
             ## Ignore check for CDO version
-            #latest = latest_version()
-            latest = None 
+            # latest = latest_version()
+            latest = None
 
             if latest is None:
-                print(f"nctoolkit is using Climate Data Operators version {actual_version}")
+                print(
+                    f"nctoolkit is using Climate Data Operators version {actual_version}"
+                )
             else:
                 if version_below(actual_version, latest):
-                    print(f"nctoolkit is using Climate Data Operators version {actual_version}. v{latest} is available: https://anaconda.org/conda-forge/cdo!")
+                    print(
+                        f"nctoolkit is using Climate Data Operators version {actual_version}. v{latest} is available: https://anaconda.org/conda-forge/cdo!"
+                    )
                 else:
-                    print(f"nctoolkit is using the latest version of Climate Data Operators version: {actual_version}")
-
+                    print(
+                        f"nctoolkit is using the latest version of Climate Data Operators version: {actual_version}"
+                    )
 
     except:
         print(
             "Please install CDO version 1.9.7 or above: https://code.mpimet.mpg.de/projects/cdo/ or https://anaconda.org/conda-forge/cdo"
         )
     if bad:
         raise ValueError(
```

### Comparing `nctoolkit-0.9.2/nctoolkit/validator.py` & `nctoolkit-0.9.3/nctoolkit/validator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,23 @@
-
-
-
 def validator():
-
     val = Validator()
     return val
 
 
-
-
-
 class Validator(object):
     """
     A modifiable ensemble of netCDF files
     """
 
     def __init__(self, start=""):
         """Initialize the starting file name etc"""
         # Attribuates of interest to users
         self.model = None
         self.obs = None
         self.plots = []
 
-
     # Import any methods
 
     from nctoolkit.validator_funs import add_observations
     from nctoolkit.validator_funs import add_model
     from nctoolkit.validator_funs import matchup
     from nctoolkit.validator_funs import validate
```

### Comparing `nctoolkit-0.9.2/nctoolkit/validator_funs.py` & `nctoolkit-0.9.3/nctoolkit/validator_funs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,29 @@
     A model validation object
     """
 
     def __init__(self, start=""):
         """Initialize the starting file name etc"""
         # Attribuates of interest to users
         self.data = None
-        #self.plot = None
+        # self.plot = None
         self.plot_type = None
         self.info = None
+
     def __repr__(self):
         return f"Validation object: {self.info}"
 
     @property
     def plot(self):
         if self.plot_type == "nctoolkit":
-            return self.data.plot(title = self.info)
+            return self.data.plot(title=self.info)
         else:
             return self._ggplot
 
+
 def get_type(ds):
     times = ds.times
 
     df = pd.DataFrame(
         {
             "year": [x.year for x in times],
             "month": [x.month for x in times],
@@ -50,17 +52,15 @@
     if len(df.loc[:, ["month"]].drop_duplicates()) == len(df):
         return ["month"]
 
     if len(df.loc[:, ["year", "month"]].drop_duplicates()) == len(df):
         return ["year", "month"]
 
 
-
-
-def add_model(self, ds = None, map = None, nan = None , precision = None, **kwargs):
+def add_model(self, ds=None, map=None, nan=None, precision=None, **kwargs):
     """
     Add model data
 
     Parameters
     -------------
     ds: Dataset
 
@@ -79,27 +79,26 @@
 
     if not isinstance(map, dict):
         raise ValueError("You must provided a map")
 
     if len(map) != 1:
         raise ValueError("There should only be one variable in the map!")
 
-
     self.model = ds.copy()
     self.model_map = map
     self.model_nan = nan
     self.model_precision = precision
 
     for kk in kwargs:
         if kk == "amm7":
             if kwargs[kk]:
                 self.model.amm7 = True
 
 
-def add_observations(self, ds = None, map = None, nan = None , precision = None):
+def add_observations(self, ds=None, map=None, nan=None, precision=None):
     """
     Add observational data
 
     Parameters
     -------------
     ds: Dataset
     map: dict
@@ -123,15 +122,14 @@
     self.obs = ds.copy()
 
     self.obs_map = map
     self.obs_nan = nan
     self.obs_precision = precision
 
 
-
 import re
 
 
 def is_number(s):
     try:
         float(s)
         return True
@@ -139,48 +137,50 @@
         return False
 
 
 def is_equation(x):
     regexp = re.compile(r"[+,\-,/, \* ]")
     return len(regexp.findall(x)) > 0
 
-def matchup(self, levels = "top", na_match = False, **kwargs):
 
+def matchup(self, levels="top", na_match=False, **kwargs):
     expected_model_vars = []
     for key, value in self.model_map.items():
         expected_model_vars += re.findall(r"\w+", value)
 
     expected_obs_vars = []
     for key, value in self.obs_map.items():
         expected_obs_vars += re.findall(r"\w+", value)
 
     model_vars = self.model.variables
     obs_vars = self.obs.variables
 
     for vv in expected_model_vars:
         if is_number(vv) is False:
             if vv not in model_vars:
-                raise ValueError(f"{vv} does not exist in model data!. Available vars: {model_vars}")
+                raise ValueError(
+                    f"{vv} does not exist in model data!. Available vars: {model_vars}"
+                )
 
     for vv in expected_obs_vars:
         if is_number(vv) is False:
             if vv not in obs_vars:
-                raise ValueError(f"{vv} does not exist in observational data! Available vars: {obs_vars}")
-
+                raise ValueError(
+                    f"{vv} does not exist in observational data! Available vars: {obs_vars}"
+                )
 
     if self.model_map is None or self.model_map is None:
         raise ValueError("You must provide maps for model and observational data!")
 
     if set(self.model_map.keys()) != set(self.obs_map.keys()):
         raise ValueError("Variables in maps should match")
 
     # Step 1. Figure out the levels
 
-
-   # extract some variables....
+    # extract some variables....
 
     keep_these = []
     for key, value in self.model_map.items():
         keep_these += re.findall(r"\w+", value)
 
     self.model.subset(variables=keep_these)
 
@@ -192,15 +192,14 @@
 
     if len(self.model) > 1:
         self.model.merge("time")
 
     if len(self.obs) > 1:
         self.obs.merge("time")
 
-
     self.model.run()
 
     if self.model_nan is not None:
         print("Fixing missing values in model data!")
         self.model.as_missing(self.model_nan)
     if self.obs_nan is not None:
         print("Fixing missing values in observation data!")
@@ -227,66 +226,57 @@
             fixed_value = value.replace("(", "\(")
             fixed_value = fixed_value.replace(")", "\)")
             self.obs.cdo_command(f"aexpr,'{key}={fixed_value}'")
 
     self.model.subset(variables=list(self.model_map.keys()))
     self.obs.subset(variables=list(self.obs_map.keys()))
 
-
     try:
         self.model.amm7
-        unify(self.model, self.obs, amm7 = True)
+        unify(self.model, self.obs, amm7=True)
     except:
         unify(self.model, self.obs)
 
     self.aggregation = get_type(self.model)
 
-
     if na_match:
         print("Matching missing values in model and observation datasets")
 
         mask = self.model.copy()
         mask.rename({list(self.model_map.keys())[0]: "variable"})
-        mask.assign(variable = lambda x: isnan(x.variable) == False)
+        mask.assign(variable=lambda x: isnan(x.variable) == False)
         mask.as_missing(0)
 
         self.model.multiply(mask)
         self.obs.multiply(mask)
 
         mask = self.obs.copy()
         mask.rename({list(self.model_map.keys())[0]: "variable"})
-        mask.assign(variable = lambda x: isnan(x.variable) == False)
+        mask.assign(variable=lambda x: isnan(x.variable) == False)
         mask.as_missing(0)
 
         self.model.multiply(mask)
         self.obs.multiply(mask)
 
         self.model.run()
         self.obs.run()
 
-
     self.matched = True
 
 
-
-
-
-
-
-def validate(self, region = None):
-
+def validate(self, region=None):
     try:
         from plotnine import ggplot
     except:
         raise ValueError("Please install plotnine")
 
     if self.matched is False:
         raise ValueError("Data has not been matched")
 
-    self.results  = []
+    self.results = []
 
     if "month" in self.aggregation or "day" in self.aggregation:
         val = Validation()
         ds_model = self.model.copy()
         ds_obs = self.obs.copy()
 
         if len(self.model.years) > 1:
@@ -302,56 +292,52 @@
         val.plot_type = "nctoolkit"
 
         self.results.append(val)
 
     ## Annual bias
 
     if len(self.model.months) == 12:
-
         val = Validation()
 
         ds_val = open_data()
         ds_model = self.model.copy()
         ds_obs = self.obs.copy()
         ds_model.tmean(["year", "month"])
         ds_obs.tmean(["year", "month"])
         ds_model.tmean(["year"])
         ds_obs.tmean(["year"])
         ds_model.subtract(ds_obs)
         ds_model.tmean()
         ds_model.rename({self.model.variables[0]: "absolute"})
         ds_val.append(ds_model)
 
-
         ds_model = self.model.copy()
         ds_obs = self.obs.copy()
         ds_model.tmean(["year", "month"])
         ds_obs.tmean(["year", "month"])
         ds_model.tmean(["year"])
         ds_obs.tmean(["year"])
         ds_model.tmean()
         ds_model.divide(ds_obs)
         ds_model.subtract(1)
         ds_model.multiply(100)
         ds_model.rename({self.model.variables[0]: "relative"})
-        ds_model.set_longnames({ "relative":"Percentage difference"})
-        ds_model.set_units({ "relative":"%"})
+        ds_model.set_longnames({"relative": "Percentage difference"})
+        ds_model.set_units({"relative": "%"})
         ds_val.append(ds_model)
         ds_val.merge("variable")
 
-        val.info= "Annual climatological bias (model -/ observation)"
+        val.info = "Annual climatological bias (model -/ observation)"
         val.plot_type = "nctoolkit"
         val.data = ds_val.copy()
         self.results.append(val)
 
-
     if "month" in self.aggregation or "day" in self.aggregation:
         # Try to find the units
         if region is None:
-
             ds_model = self.model.copy()
 
             model_vars = ds_model.variables
 
             model_units = dict()
             for vv in model_vars:
                 try:
@@ -424,15 +410,17 @@
 
             all_df = all_df.melt(value_vars=model_vars, id_vars=id_vars)
 
             ylab = model_vars[0]
 
             val = Validation()
 
-            val.info = f"Monthly climatologies of model and observational data for {ylab}"
+            val.info = (
+                f"Monthly climatologies of model and observational data for {ylab}"
+            )
 
             if ylab in model_units.keys():
                 ylab = ylab + "(" + model_units[ylab] + ")"
 
             plot = (
                 ggplot(all_df.dropna())
                 + geom_line(aes("month", "value", colour="source"))
@@ -440,17 +428,15 @@
                 + labs(title=val.info)
             )
 
             val._ggplot = plot
             val.data = all_df
             self.results.append(val)
 
-
         if region is not None:
-
             regions = region.copy()
 
             ds_model = self.model.copy()
 
             model_vars = ds_model.variables
 
             model_units = dict()
@@ -531,15 +517,17 @@
             id_vars = [x for x in all_df.columns if x not in model_vars]
 
             all_df = all_df.melt(value_vars=model_vars, id_vars=id_vars)
 
             ylab = model_vars[0]
             val = Validation()
 
-            val.info =  f"Monthly climatologies of model and observational data for {ylab}"
+            val.info = (
+                f"Monthly climatologies of model and observational data for {ylab}"
+            )
 
             if ylab in model_units.keys():
                 ylab = ylab + "(" + model_units[ylab] + ")"
 
             plot = (
                 ggplot(all_df.dropna())
                 + geom_line(aes("month", "value", colour="source"))
@@ -559,15 +547,15 @@
 
         ds_bias = self.model.copy()
         ds_bias.subtract(self.obs)
         ds_bias.tmean("month")
 
         val.data = ds_bias.copy()
 
-        val.plot_type  = "nctoolkit"
+        val.plot_type = "nctoolkit"
         self.results.append(val)
 
     # Plot the annual time series...
     if "year" in self.aggregation and len(self.model.years) > 1:
         # Try to find the units
 
         if region is not None:
@@ -657,15 +645,15 @@
             id_vars = [x for x in all_df.columns if x not in model_vars]
 
             all_df = all_df.melt(value_vars=model_vars, id_vars=id_vars)
 
             ylab = model_vars[0]
 
             val = Validation()
-            val.info =  f"Annual means of model and observational data for {ylab}"
+            val.info = f"Annual means of model and observational data for {ylab}"
 
             if ylab in model_units.keys():
                 ylab = ylab + "(" + model_units[ylab] + ")"
 
             plot = (
                 ggplot(all_df)
                 + geom_line(aes("year", "value", colour="source"))
@@ -675,15 +663,14 @@
             )
             val._ggplot = plot
             val.plot_type = "plotnine"
 
             self.results.append(val)
 
         if region is None:
-
             ds_model = self.model.copy()
 
             model_vars = ds_model.variables
 
             model_units = dict()
             for vv in model_vars:
                 try:
@@ -769,10 +756,7 @@
                 + labs(y=ylab)
                 + labs(title=val.info)
             )
 
             val._ggplot = plot
             val.data = all_df
             self.results.append(val)
-
-
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/verticals.py` & `nctoolkit-0.9.3/nctoolkit/verticals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-import copy
 import subprocess
 import warnings
-import os
-
-from nctoolkit.api import open_data
+import copy
 from nctoolkit.cleanup import cleanup
-from nctoolkit.flatten import str_flatten
-from nctoolkit.runthis import run_this, run_cdo
+from nctoolkit.api import open_data
 from nctoolkit.temp_file import temp_file
-from nctoolkit.session import append_safe
-from nctoolkit.session import remove_safe
 from nctoolkit.utils import version_above, cdo_version
+from nctoolkit.flatten import str_flatten
+from nctoolkit.runthis import run_this 
 import nctoolkit.api as api
 
 
 def bottom(self):
     """
     Extract the bottom level from a dataset
     This extracts the bottom level from each netCDF file. Please note that for
@@ -72,30 +68,30 @@
     This method is most useful for things like oceanic data, where this method will extract the sea surface.
     """
 
     cdo_command = "cdo -sellevidx,1"
     run_this(cdo_command, self, output="ensemble")
 
 
-def vertical_interp(self, levels=None, fixed = None, thickness = None):
+def vertical_interp(self, levels=None, fixed=None, thickness=None):
     """
     Verticaly interpolate a dataset based on given vertical levels
     This is calculated for each time step and grid cell
     Note: This requires consistent vertical levels in space. For the likes of sigma-coordinates,
     please use to_zlevels.
 
     Parameters
     -------------
     levels : list, int or str
         list of vertical levels, for example depths for an ocean model, to vertically
         interpolate to. These must be floats or ints.
-    fixed : bool 
+    fixed : bool
         Define whether the vertical levels are the same in all spatial locations.
         Set to True if they are, e.g. you have z-levels. If you have the likes of sigma-coordinates,
-        set this to True. 
+        set this to True.
     thickness: str or Dataset
         This must be supplied if fixed is False, otherwise vertical thickness cannot be known.
         Option argument when vertical levels vary in space.
         One of: a variable, in the dataset, which contains the variable thicknesses; a .nc file which contains
         the thicknesses; or a Dataset that contains the thicknesses. Note: the .nc file or Dataset must only contain
         one variable. Thickness should be in metres. Vertical interpolation will take the value from the mid-point of the level.
 
@@ -123,26 +119,26 @@
         if thickness is None:
             raise TypeError("fixed must be a bool")
 
     if thickness is not None:
         fixed = False
 
     if fixed is False:
-        self.to_zlevels(levels = levels, thickness = thickness)
+        self.to_zlevels(levels=levels, thickness=thickness)
         return None
 
     if levels is None:
         raise ValueError("Please supply vertical depths")
 
     # first a quick fix for the case when there is only one vertical depth
 
     if isinstance(levels, (int, float)):
         levels = [levels]
 
-    #levels = [float(x) for x in levels]
+    # levels = [float(x) for x in levels]
 
     for vv in levels:
         if not isinstance(vv, (int, float)):
             raise TypeError(f"{vv} is not a valid depth")
 
     levels = str_flatten(levels, ",")
     cdo_command = f"cdo -intlevel,{levels}"
@@ -152,33 +148,33 @@
 
 def vertstat(self, stat="mean"):
     """Method to calculate the vertical mean from a function"""
     cdo_command = f"cdo -vert{stat}"
     run_this(cdo_command, self, output="ensemble")
 
 
-def vertical_mean(self, thickness=None, depth_range=None, fixed = None):
+def vertical_mean(self, thickness=None, depth_range=None, fixed=None):
     """
     Calculate the depth-averaged mean for each variable
     This is calculated for each time step and grid cell
 
     Optional parameters
     -------------
     thickness: str or Dataset
         This mube be supplied when vertical levels vary in space, i.e. fixed=False.
         One of: a variable, in the dataset, which contains the variable thicknesses; a .nc file which contains
         the thicknesses; or a Dataset that contains the thicknesses. Note: the .nc file or Dataset must only contain
         one variable.
     depth_range: list
         Only use when vertical levels vary in space
         Set a depth range if desired. Should be of the form [min_depth, max_depth].
-    fixed : bool 
+    fixed : bool
         Define whether the vertical levels are the same in all spatial locations.
         Set to True if they are, e.g. you have z-levels. If you have the likes of sigma-coordinates,
-        set this to True. 
+        set this to True.
 
     Examples
     ------------
 
     If you wanted to vertical mean of every variable in a dataset with consistent vertical levels, you would do this:
 
     >>> ds.vertical_mean(fixed = True)
@@ -198,15 +194,14 @@
             raise ValueError("Please provide thickness")
 
     if thickness is None and depth_range is None:
         vertstat(self, stat="mean")
         return None
 
     if isinstance(depth_range, list):
-
         if len(depth_range) != 2:
             raise ValueError("Please provide a 2 variable list for depth range")
         if depth_range[1] <= depth_range[0]:
             raise ValueError("Please provide a correctly ordered depth range")
 
     if depth_range is not None:
         if not isinstance(depth_range, list):
@@ -217,42 +212,43 @@
             raise ValueError("Please provide a thickness variable")
 
     self.run()
 
     self1 = self.copy()
 
     if len(self) > 1:
-        warnings.warn("Vertical structure will be assumed to be the same for all files in the dataset")
+        warnings.warn(
+            "Vertical structure will be assumed to be the same for all files in the dataset"
+        )
 
     # Set up the thickness
 
     sorted = False
 
     if isinstance(thickness, api.DataSet):
         ds_thick = thickness.copy()
         if len(ds_thick.variables) != 1:
             raise ValueError("Please provide a thickness dataset with 1 variable!")
         sorted = True
 
     drop_this = None
     if sorted is False:
         if thickness in self.variables:
-            ds_thick = open_data(self[0]) 
+            ds_thick = open_data(self[0])
             ds_thick.subset(variable=thickness)
             ds_thick.run()
             drop_this = thickness
         else:
             ds_thick = open_data(thickness)
             if len(ds_thick.variables) != 1:
                 raise ValueError("Please provide a thickness file with 1 variable!")
 
     thick_var = ds_thick.variables[0]
     # modify the depth if it is a list
     if isinstance(depth_range, list):
-
         ds_thick.rename({thick_var: "thickness"})
         ds_thick.run()
         ds_depth = ds_thick.copy()
         ds_depth.vertical_cumsum()
         ds_depth.rename({"thickness": "depth"})
         ds_thick.append(ds_depth)
         ds_thick.merge()
@@ -260,33 +256,34 @@
         ds_thick.assign( z_min=lambda x: x.z_min * (x.z_min >= depth_range[0]) + depth_range[0] * (x.z_min < depth_range[0]))
         ds_thick.assign( depth=lambda x: x.depth * (x.depth <= depth_range[1]) + depth_range[1] * (x.depth > depth_range[1]))
         ds_thick.assign(thickness=lambda x: x.depth - x.z_min, drop=True)
         ds_thick.assign(thickness=lambda x: x.thickness * (x.thickness > 0), drop=True)
 
     self1.subset(variables=self.contents.query("nlevels > 1").variable)
     if drop_this is not None:
-        self1.drop(variables = drop_this)
+        self1.drop(variables=drop_this)
 
     ds_thick.run()
     self1.run()
     self1.multiply(ds_thick)
-    warnings.warn(message = "Assuming missing values are in the same grid cells in thickness and variable data. Modify thickness and re-run if they are not.")
+    warnings.warn(
+        message="Assuming missing values are in the same grid cells in thickness and variable data. Modify thickness and re-run if they are not."
+    )
     self1.run()
     self1.vertical_sum()
     self1.run()
 
     ds_thick.vertical_sum()
     self1.divide(ds_thick)
     self1.run()
 
     del ds_thick
     if isinstance(depth_range, list):
         del ds_depth
 
-
     self.current = self1.current
     self.history = self1.history
     self._hold_history = self1._hold_history
 
 
 def vertical_min(self):
     """
@@ -332,32 +329,32 @@
 
     >>> ds.vertical_range()
 
     """
     vertstat(self, stat="range")
 
 
-def vertical_integration(self, thickness=None, depth_range=None, fixed = None):
+def vertical_integration(self, thickness=None, depth_range=None, fixed=None):
     """
     Calculate the vertically integrated sum over the water column
     This calculates the sum of the variable multiplied by the cell thickness
 
     Parameters
     -------------
     thickness: str or Dataset
         This must be supplied when vertical levels vary spatially.
         One of: a variable, in the dataset, which contains the variable thicknesses; a .nc file which contains
         the thicknesses; or a Dataset that contains the thicknesses. Note: the .nc file or Dataset must only contain
         one variable.
     depth_range: list
         Set a depth range if desired. Should be of the form [min_depth, max_depth].
-    fixed : bool 
+    fixed : bool
         Define whether the vertical levels are the same in all spatial locations.
         Set to True if they are, e.g. you have z-levels. If you have the likes of sigma-coordinates,
-        set this to True. 
+        set this to True.
 
     Examples
     ------------
 
     If you wanted to sum of values across all vertical levels of every variable in a dataset that has spatially fixed vertical levels, you would do this:
 
     >>> ds.vertical_sum(fixed = True)
@@ -371,37 +368,38 @@
             raise ValueError("Please install CDO>2.0.0")
         warnings.warn("Extracting vertical thickness from dataset level data")
         var = list(self.contents.query("nlevels > 1").variable)[0]
 
         ff = self[0]
         command = f"cdo zaxisdes {ff}"
         out = subprocess.Popen(
-                 command,
-                 shell=True,
-                 stdin=subprocess.PIPE,
-                 stdout=subprocess.PIPE,
-                 stderr=subprocess.STDOUT,
-             )
+            command,
+            shell=True,
+            stdin=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+        )
         result, ignore = out.communicate()
 
         if "bounds" not in result.decode("utf-8").lower():
-            raise ValueError("Vertical bounds info does not appear to be in the netCDF files, so thicknesses cannot be calculated for vertical integration!")
+            raise ValueError(
+                "Vertical bounds info does not appear to be in the netCDF files, so thicknesses cannot be calculated for vertical integration!"
+            )
 
         thickness = self.copy()
-        thickness.subset(time = 0, variable = var)
-        thickness.rename({var:"thickness"})
-        thickness.assign(thickness = lambda x: (isnan(x.thickness) == False) * level(x.thickness), drop = True)
-        thickness.assign(thickness = lambda x: thickness(x.thickness) + (x.thickness < x.thickness), drop = True)
+        thickness.subset(time=0, variable=var)
+        thickness.rename({var: "thickness"})
+        thickness.assign( thickness=lambda x: (isnan(x.thickness) is False) * level(x.thickness), drop=True,)
+        thickness.assign( thickness=lambda x: thickness(x.thickness) + (x.thickness < x.thickness), drop=True,)
         thickness.run()
-    
+
     if thickness is None:
         raise ValueError("Please specify thickness")
 
     if isinstance(depth_range, list):
-
         if len(depth_range) != 2:
             raise ValueError("Please provide a 2 variable list for depth range")
         if depth_range[1] <= depth_range[0]:
             raise ValueError("Please provide a correctly ordered depth range")
 
     drop_this = None
     if depth_range is not None:
@@ -411,15 +409,17 @@
     if not isinstance(thickness, api.DataSet):
         if thickness is None or isinstance(thickness, str) is False:
             raise ValueError("Please provide a thickness variable")
 
     self.run()
 
     if len(self) > 1:
-        warnings.warn("Vertical integration will assume all files have the same structure")
+        warnings.warn(
+            "Vertical integration will assume all files have the same structure"
+        )
 
     # Set up the thickness
 
     self1 = self.copy()
 
     sorted = False
 
@@ -439,15 +439,14 @@
             ds_thick = open_data(thickness)
             if len(ds_thick.variables) != 1:
                 raise ValueError("Please provide a thickness file with 1 variable!")
 
     thick_var = ds_thick.variables[0]
     # modify the depth if it is a list
     if isinstance(depth_range, list):
-
         if thick_var != "thickness":
             ds_thick.rename({thick_var: "thickness"})
             ds_thick.run()
         ds_depth = ds_thick.copy()
         ds_depth.vertical_cumsum()
         ds_depth.rename({"thickness": "depths"})
         ds_thick.append(ds_depth)
@@ -457,15 +456,15 @@
         ds_thick.assign( z_min=lambda x: x.z_min * (x.z_min >= depth_range[0]) + depth_range[0] * (x.z_min < depth_range[0]))
         ds_thick.assign( depths=lambda x: x.depths * (x.depths <= depth_range[1]) + depth_range[1] * (x.depths > depth_range[1]))
         ds_thick.assign(thickness=lambda x: x.depths - x.z_min, drop=True)
         ds_thick.assign(thickness=lambda x: x.thickness * (x.thickness > 0), drop=True)
 
     self1.subset(variables=self1.contents.query("nlevels > 1").variable)
     if drop_this is not None:
-        self1.drop(variables = drop_this)
+        self1.drop(variables=drop_this)
 
     ds_thick.run()
     self1.run()
     self1.multiply(ds_thick)
     self1.run()
     self1.vertical_sum()
     self1.run()
@@ -566,26 +565,20 @@
     self.current = copy.deepcopy(bottom.current)
 
     self.history = copy.deepcopy(bottom.history)
     self._hold_history = copy.deepcopy(self.history)
 
     cleanup()
 
+
 def surface_mask(self):
     """
     Create a mask identifying the shallowest cell without missing values.
     This converts a dataset to a mask identifying which cell represents top level,
     for example the sea surface. 1 identifies the shallowest cell with non-missing values.
     Everything else is 0, or missing. At present this method only uses the first
     available variable from netCDF files, so it may not be suitable for all data
     """
 
     self.invert_levels()
     self.bottom_mask()
     self.invert_levels()
-
-
-
-
-
-
-
```

### Comparing `nctoolkit-0.9.2/nctoolkit/zonals.py` & `nctoolkit-0.9.3/nctoolkit/zonals.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,41 +10,43 @@
         if is_curvilinear(ff):
             raise TypeError(f"zonal_{stat} cannot be calculated for curvilinear grids.")
 
     cdo_command = f"cdo -zon{stat}"
 
     run_this(cdo_command, self, output="ensemble")
 
-def zonal_sum(self, by_area = False):
+
+def zonal_sum(self, by_area=False):
     """
     Calculate the zonal sum for each year/month combination in files.
     This applies to each file in an ensemble.
 
     Parameters
     -------------
-    by_area : bool 
-        Set to True if you want the cell value to be multiplied by the cell area prior to summing 
+    by_area : bool
+        Set to True if you want the cell value to be multiplied by the cell area prior to summing
 
     Examples
     ------------
     If you want to calculate the zonal sum for a dataset, do the following:
 
     >>> ds.zonal_sum()
 
     """
     if by_area is True:
         if len(self) > 1:
             print("Using first file in the dataset for areas")
         ds_area = open_data(self[0])
-        ds_area.subset(time = 0)
-        ds_area.cell_area(join = False)
+        ds_area.subset(time=0)
+        ds_area.cell_area(join=False)
         self.multiply(ds_area)
 
     zonstat(self, stat="sum")
 
+
 def zonal_mean(self):
     """
     Calculate the zonal mean for each year/month combination in files.
     This applies to each file in an ensemble.
 
     Examples
     ------------
```

### Comparing `nctoolkit-0.9.2/nctoolkit.egg-info/SOURCES.txt` & `nctoolkit-0.9.3/nctoolkit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -78,8 +78,10 @@
 nctoolkit/tozlev.py
 nctoolkit/unify.py
 nctoolkit/utils.py
 nctoolkit/validator.py
 nctoolkit/validator_funs.py
 nctoolkit/verticals.py
 nctoolkit/zip.py
-nctoolkit/zonals.py
+nctoolkit/zonals.py
+testing/test_parallel.py
+testing/test_scripting.py
```

### Comparing `nctoolkit-0.9.2/setup.py` & `nctoolkit-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 extras_require["complete"] = ["geoviews", "rioxarray", "cfchecker", "geocube", "geopandas"]
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(name='nctoolkit',
-      version='0.9.2',
+      version='0.9.3',
       description=DESCRIPTION,
       long_description=LONG_DESCRIPTION,
       python_requires='>=3.6.1',
       classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
```

