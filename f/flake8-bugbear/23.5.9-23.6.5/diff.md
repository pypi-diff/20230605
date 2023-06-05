# Comparing `tmp/flake8-bugbear-23.5.9.tar.gz` & `tmp/flake8-bugbear-23.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-bugbear-23.5.9.tar", last modified: Tue May  9 23:58:06 2023, max compression
+gzip compressed data, was "flake8-bugbear-23.6.5.tar", last modified: Mon Jun  5 16:20:50 2023, max compression
```

## Comparing `flake8-bugbear-23.5.9.tar` & `flake8-bugbear-23.6.5.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:58:06.916914 flake8-bugbear-23.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-05-09 23:58:06.916914 flake8-bugbear-23.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25062 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    65897 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/bugbear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:58:06.912913 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-09 23:58:06.916914 flake8-bugbear-23.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:58:06.916914 flake8-bugbear-23.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b001.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b002.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b003.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b004.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b005.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b006_b008.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b007.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b008_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b009_b010.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b011.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b012.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b013.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b014.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b015.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b016.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b017.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b018_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b018_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b018_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b019.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b020.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b021.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b022.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b023.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b024.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b025.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b026.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b027.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b028.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b029.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b030.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b031.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b032.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b033.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b901.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b902.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b902_py38.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b903.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b904.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b905_py310.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b906.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b907.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b908.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b950.py
--rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/test_bugbear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:20:50.367162 flake8-bugbear-23.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26492 2023-06-05 16:20:50.367162 flake8-bugbear-23.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25173 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    65990 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/bugbear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:20:50.363162 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26492 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-05 16:20:50.367162 flake8-bugbear-23.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:20:50.367162 flake8-bugbear-23.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b001.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b006_b008.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b008_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b009_b010.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b012.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b014.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b018_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b018_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b018_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b020.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b025.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b026.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b027.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b028.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b029.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b030.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b031.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b032.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b033.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b901.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b902.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b902_py38.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b903.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b904.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b905_py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b906.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b907.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b908.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b950.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29309 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/test_bugbear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tox.ini
```

### Comparing `flake8-bugbear-23.5.9/LICENSE` & `flake8-bugbear-23.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/PKG-INFO` & `flake8-bugbear-23.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-bugbear
-Version: 23.5.9
+Version: 23.6.5
 Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
 Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
 Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
 Classifier: Development Status :: 5 - Production/Stable
@@ -354,14 +354,20 @@
 
 MIT
 
 
 Change Log
 ----------
 
+23.6.5
+~~~~~~
+
+* Include tox.ini in MANIFEST.in for sdist. (#389)
+* Improve B033 (duplicate set items) (#385)
+
 23.5.9
 ~~~~~~
 
 * Add B033: Detect duplicate items in sets
 * Add B908: Detect assertRauses like contexts only has top level statements that could throw
 * Add B028: Allow stacklevel to be explicitly assigned as a positional argument
 * Remove more < 3.8 checks / assertions
```

### Comparing `flake8-bugbear-23.5.9/README.rst` & `flake8-bugbear-23.6.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -325,14 +325,20 @@
 
 MIT
 
 
 Change Log
 ----------
 
+23.6.5
+~~~~~~
+
+* Include tox.ini in MANIFEST.in for sdist. (#389)
+* Improve B033 (duplicate set items) (#385)
+
 23.5.9
 ~~~~~~
 
 * Add B033: Detect duplicate items in sets
 * Add B908: Detect assertRauses like contexts only has top level statements that could throw
 * Add B028: Allow stacklevel to be explicitly assigned as a positional argument
 * Remove more < 3.8 checks / assertions
```

### Comparing `flake8-bugbear-23.5.9/bugbear.py` & `flake8-bugbear-23.6.5/bugbear.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from contextlib import suppress
 from functools import lru_cache, partial
 from keyword import iskeyword
 
 import attr
 import pycodestyle
 
-__version__ = "23.5.9"
+__version__ = "23.6.5"
 
 LOG = logging.getLogger("flake8.bugbear")
 CONTEXTFUL_NODES = (
     ast.Module,
     ast.ClassDef,
     ast.AsyncFunctionDef,
     ast.FunctionDef,
@@ -1347,20 +1347,24 @@
                     and node.target.value.id != "self"
                 )
             )
         ):
             self.errors.append(B032(node.lineno, node.col_offset))
 
     def check_for_b033(self, node):
-        constants = [
-            item.value
-            for item in filter(lambda x: isinstance(x, ast.Constant), node.elts)
-        ]
-        if len(constants) != len(set(constants)):
-            self.errors.append(B033(node.lineno, node.col_offset))
+        seen = set()
+        for elt in node.elts:
+            if not isinstance(elt, ast.Constant):
+                continue
+            if elt.value in seen:
+                self.errors.append(
+                    B033(elt.lineno, elt.col_offset, vars=(repr(elt.value),))
+                )
+            else:
+                seen.add(elt.value)
 
 
 def compose_call_path(node):
     if isinstance(node, ast.Attribute):
         yield from compose_call_path(node.value)
         yield node.attr
     elif isinstance(node, ast.Call):
@@ -1753,16 +1757,16 @@
         "B032 Possible unintentional type annotation (using `:`). Did you mean to"
         " assign (using `=`)?"
     )
 )
 
 B033 = Error(
     message=(
-        "B033 Sets should not contain duplicate items. Duplicate items will be replaced"
-        " with a single item at runtime."
+        "B033 Set should not contain duplicate item {}. Duplicate items will be"
+        " replaced with a single item at runtime."
     )
 )
 
 # Warnings disabled by default.
 B901 = Error(
     message=(
         "B901 Using `yield` together with `return x`. Use native "
@@ -1813,14 +1817,14 @@
     message=(
         "B907 {!r} is manually surrounded by quotes, consider using the `!r` conversion"
         " flag."
     )
 )
 B908 = Error(
     message=(
-        "B908 assertRaises-type context should not contains more than one top-level"
+        "B908 assertRaises-type context should not contain more than one top-level"
         " statement."
     )
 )
 B950 = Error(message="B950 line too long ({} > {} characters)")
 
 disabled_by_default = ["B901", "B902", "B903", "B904", "B905", "B906", "B908", "B950"]
```

### Comparing `flake8-bugbear-23.5.9/flake8_bugbear.egg-info/PKG-INFO` & `flake8-bugbear-23.6.5/flake8_bugbear.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-bugbear
-Version: 23.5.9
+Version: 23.6.5
 Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
 Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
 Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
 Classifier: Development Status :: 5 - Production/Stable
@@ -354,14 +354,20 @@
 
 MIT
 
 
 Change Log
 ----------
 
+23.6.5
+~~~~~~
+
+* Include tox.ini in MANIFEST.in for sdist. (#389)
+* Improve B033 (duplicate set items) (#385)
+
 23.5.9
 ~~~~~~
 
 * Add B033: Detect duplicate items in sets
 * Add B908: Detect assertRauses like contexts only has top level statements that could throw
 * Add B028: Allow stacklevel to be explicitly assigned as a positional argument
 * Remove more < 3.8 checks / assertions
```

### Comparing `flake8-bugbear-23.5.9/flake8_bugbear.egg-info/SOURCES.txt` & `flake8-bugbear-23.6.5/flake8_bugbear.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 bugbear.py
 pyproject.toml
 setup.cfg
 setup.py
+tox.ini
 flake8_bugbear.egg-info/PKG-INFO
 flake8_bugbear.egg-info/SOURCES.txt
 flake8_bugbear.egg-info/dependency_links.txt
 flake8_bugbear.egg-info/entry_points.txt
 flake8_bugbear.egg-info/not-zip-safe
 flake8_bugbear.egg-info/requires.txt
 flake8_bugbear.egg-info/top_level.txt
```

### Comparing `flake8-bugbear-23.5.9/pyproject.toml` & `flake8-bugbear-23.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b001.py` & `flake8-bugbear-23.6.5/tests/b001.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b005.py` & `flake8-bugbear-23.6.5/tests/b005.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b006_b008.py` & `flake8-bugbear-23.6.5/tests/b006_b008.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b007.py` & `flake8-bugbear-23.6.5/tests/b007.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b009_b010.py` & `flake8-bugbear-23.6.5/tests/b009_b010.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b012.py` & `flake8-bugbear-23.6.5/tests/b012.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b013.py` & `flake8-bugbear-23.6.5/tests/b013.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b014.py` & `flake8-bugbear-23.6.5/tests/b014.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b017.py` & `flake8-bugbear-23.6.5/tests/b017.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b019.py` & `flake8-bugbear-23.6.5/tests/b019.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b020.py` & `flake8-bugbear-23.6.5/tests/b020.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b021.py` & `flake8-bugbear-23.6.5/tests/b021.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b023.py` & `flake8-bugbear-23.6.5/tests/b023.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b024.py` & `flake8-bugbear-23.6.5/tests/b024.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b027.py` & `flake8-bugbear-23.6.5/tests/b027.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b030.py` & `flake8-bugbear-23.6.5/tests/b030.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b031.py` & `flake8-bugbear-23.6.5/tests/b031.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b901.py` & `flake8-bugbear-23.6.5/tests/b901.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b902.py` & `flake8-bugbear-23.6.5/tests/b902.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b902_py38.py` & `flake8-bugbear-23.6.5/tests/b902_py38.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b903.py` & `flake8-bugbear-23.6.5/tests/b903.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b904.py` & `flake8-bugbear-23.6.5/tests/b904.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b906.py` & `flake8-bugbear-23.6.5/tests/b906.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b907.py` & `flake8-bugbear-23.6.5/tests/b907.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b908.py` & `flake8-bugbear-23.6.5/tests/b908.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/b950.py` & `flake8-bugbear-23.6.5/tests/b950.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.5.9/tests/test_bugbear.py` & `flake8-bugbear-23.6.5/tests/test_bugbear.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,21 +489,23 @@
         self.assertEqual(errors, expected)
 
     def test_b033(self):
         filename = Path(__file__).absolute().parent / "b033.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
         expected = self.errors(
-            B033(6, 7),
-            B033(7, 7),
-            B033(8, 7),
-            B033(9, 7),
-            B033(10, 7),
-            B033(11, 7),
-            B033(12, 7),
+            B033(6, 17, vars=("3",)),
+            B033(7, 23, vars=("'c'",)),
+            B033(8, 21, vars=("True",)),
+            B033(9, 20, vars=("None",)),
+            B033(10, 11, vars=("3.0",)),
+            B033(11, 11, vars=("True",)),
+            B033(12, 11, vars=("False",)),
+            B033(16, 4, vars=("True",)),
+            B033(18, 4, vars=("False",)),
         )
         self.assertEqual(errors, expected)
 
     def test_b908(self):
         filename = Path(__file__).absolute().parent / "b908.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
```

