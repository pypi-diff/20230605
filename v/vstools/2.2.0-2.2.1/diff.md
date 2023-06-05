# Comparing `tmp/vstools-2.2.0.tar.gz` & `tmp/vstools-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstools-2.2.0.tar", last modified: Mon Jun  5 13:57:16 2023, max compression
+gzip compressed data, was "vstools-2.2.1.tar", last modified: Mon Jun  5 20:27:15 2023, max compression
```

## Comparing `vstools-2.2.0.tar` & `vstools-2.2.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.983360 vstools-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 13:56:54.000000 vstools-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 13:57:16.983360 vstools-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 13:56:54.000000 vstools-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 13:57:16.983360 vstools-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-05 13:56:54.000000 vstools-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.975360 vstools-2.2.0/vstools/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.979360 vstools-2.2.0/vstools/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34510 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.979360 vstools-2.2.0/vstools/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.979360 vstools-2.2.0/vstools/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/timecodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.979360 vstools-2.2.0/vstools/types/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.983360 vstools-2.2.0/vstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/__file_headers.json
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/clips.py
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/ffprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/mime_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/props.py
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)    27233 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/vs_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/vs_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.975360 vstools-2.2.0/vstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.397402 vstools-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 20:26:47.000000 vstools-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 20:27:15.397402 vstools-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 20:26:47.000000 vstools-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 20:27:15.397402 vstools-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-05 20:26:47.000000 vstools-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.377401 vstools-2.2.1/vstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.381401 vstools-2.2.1/vstools/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34595 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.385401 vstools-2.2.1/vstools/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.389402 vstools-2.2.1/vstools/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/timecodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.389402 vstools-2.2.1/vstools/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.397402 vstools-2.2.1/vstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/__file_headers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/clips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/ffprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/mime_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27233 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/vs_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/vs_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.381401 vstools-2.2.1/vstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/top_level.txt
```

### Comparing `vstools-2.2.0/LICENSE` & `vstools-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/PKG-INFO` & `vstools-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstools
-Version: 2.2.0
+Version: 2.2.1
 Summary: Functions and utils related to VapourSynth
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-tools
 Project-URL: Documentation, https://vstools.encoding.moe/en/latest/
```

### Comparing `vstools-2.2.0/README.md` & `vstools-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/setup.cfg` & `vstools-2.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/setup.py` & `vstools-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/enums/base.py` & `vstools-2.2.1/vstools/enums/base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/enums/color.py` & `vstools-2.2.1/vstools/enums/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import vapoursynth as vs
 
 from ..exceptions import (
     ReservedMatrixError, ReservedPrimariesError, ReservedTransferError, UndefinedMatrixError, UndefinedPrimariesError,
     UndefinedTransferError, UnsupportedColorRangeError, UnsupportedMatrixError, UnsupportedPrimariesError,
     UnsupportedTransferError
 )
-from ..types import FuncExceptT, classproperty
+from ..types import FuncExceptT, HoldsPropValueT, classproperty
 from .stubs import PropEnum, _base_from_video, _ColorRangeMeta, _MatrixMeta, _PrimariesMeta, _TransferMeta
 
 __all__ = [
     'PropEnum',
 
     'Matrix', 'Transfer', 'Primaries',
     'MatrixT', 'TransferT', 'PrimariesT',
@@ -1206,18 +1206,18 @@
     Primaries.ST428: 'ST 428 (XYZ)',
     Primaries.ST431_2: 'DCI-P3, DCI white point',
     Primaries.ST432_1: 'DCI-P3 D65 white point',
     Primaries.EBU3213E: '0JEDEC P22 (EBU3213)'
 }
 
 
-MatrixT: TypeAlias = Union[int, vs.MatrixCoefficients, Matrix]
+MatrixT: TypeAlias = Union[int, vs.MatrixCoefficients, Matrix, HoldsPropValueT]
 """Type alias for values that can be used to initialize a :py:attr:`Matrix`."""
 
-TransferT: TypeAlias = Union[int, vs.TransferCharacteristics, Transfer]
+TransferT: TypeAlias = Union[int, vs.TransferCharacteristics, Transfer, HoldsPropValueT]
 """Type alias for values that can be used to initialize a :py:attr:`Transfer`."""
 
-PrimariesT: TypeAlias = Union[int, vs.ColorPrimaries, Primaries]
+PrimariesT: TypeAlias = Union[int, vs.ColorPrimaries, Primaries, HoldsPropValueT]
 """Type alias for values that can be used to initialize a :py:attr:`Primaries`."""
 
-ColorRangeT: TypeAlias = Union[int, vs.ColorRange, ColorRange]
+ColorRangeT: TypeAlias = Union[int, vs.ColorRange, ColorRange, HoldsPropValueT]
 """Type alias for values that can be used to initialize a :py:attr:`ColorRange`."""
```

### Comparing `vstools-2.2.0/vstools/enums/generic.py` & `vstools-2.2.1/vstools/enums/generic.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/enums/other.py` & `vstools-2.2.1/vstools/enums/other.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/enums/stubs.py` & `vstools-2.2.1/vstools/enums/stubs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/exceptions/base.py` & `vstools-2.2.1/vstools/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/exceptions/color.py` & `vstools-2.2.1/vstools/exceptions/color.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/exceptions/enum.py` & `vstools-2.2.1/vstools/exceptions/enum.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/exceptions/file.py` & `vstools-2.2.1/vstools/exceptions/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/exceptions/generic.py` & `vstools-2.2.1/vstools/exceptions/generic.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/exceptions/module.py` & `vstools-2.2.1/vstools/exceptions/module.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/functions/check.py` & `vstools-2.2.1/vstools/functions/check.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/functions/clip.py` & `vstools-2.2.1/vstools/functions/clip.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/functions/funcs.py` & `vstools-2.2.1/vstools/functions/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/functions/heuristics.py` & `vstools-2.2.1/vstools/functions/heuristics.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/functions/normalize.py` & `vstools-2.2.1/vstools/functions/normalize.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/functions/progress.py` & `vstools-2.2.1/vstools/functions/progress.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/functions/render.py` & `vstools-2.2.1/vstools/functions/render.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/functions/timecodes.py` & `vstools-2.2.1/vstools/functions/timecodes.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/functions/utils.py` & `vstools-2.2.1/vstools/functions/utils.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/types/builtins.py` & `vstools-2.2.1/vstools/types/builtins.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/types/file.py` & `vstools-2.2.1/vstools/types/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/types/funcs.py` & `vstools-2.2.1/vstools/types/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/types/generic.py` & `vstools-2.2.1/vstools/types/generic.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/types/utils.py` & `vstools-2.2.1/vstools/types/utils.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/__file_headers.json` & `vstools-2.2.1/vstools/utils/__file_headers.json`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/__init__.py` & `vstools-2.2.1/vstools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/cache.py` & `vstools-2.2.1/vstools/utils/cache.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/clips.py` & `vstools-2.2.1/vstools/utils/clips.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/colors.py` & `vstools-2.2.1/vstools/utils/colors.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/ffprobe.py` & `vstools-2.2.1/vstools/utils/ffprobe.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/file.py` & `vstools-2.2.1/vstools/utils/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/funcs.py` & `vstools-2.2.1/vstools/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/info.py` & `vstools-2.2.1/vstools/utils/info.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/math.py` & `vstools-2.2.1/vstools/utils/math.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/mime.py` & `vstools-2.2.1/vstools/utils/mime.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/mime_base.py` & `vstools-2.2.1/vstools/utils/mime_base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/misc.py` & `vstools-2.2.1/vstools/utils/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from ..exceptions import InvalidSubsamplingError
 from .info import get_video_format
 
 __all__ = [
     'change_fps',
 
+    'match_clip',
+
     'padder',
 
     'pick_func_stype',
 
     'set_output'
 ]
 
@@ -45,14 +47,41 @@
     new_fps_clip = clip.std.BlankClip(
         length=floor(clip.num_frames * factor), fpsnum=dest_num, fpsden=dest_den
     )
 
     return new_fps_clip.std.FrameEval(lambda n: clip[round(n / factor)])
 
 
+def match_clip(
+    clip: vs.VideoNode, ref: vs.VideoNode, dimensions: bool = True,
+    vformat: bool = True, matrices: bool = True, length: bool = False
+) -> vs.VideoNode:
+    from ..enums import Matrix, Primaries, Transfer
+    from ..functions import check_variable
+
+    assert check_variable(clip, match_clip)
+    assert check_variable(ref, match_clip)
+
+    clip = clip * ref.num_frames if length else clip
+    clip = clip.resize.Bicubic(ref.width, ref.height) if dimensions else clip
+
+    if vformat:
+        assert ref.format
+        clip = clip.resize.Bicubic(format=ref.format, matrix=Matrix.from_video(ref))
+
+    if matrices:
+        ref_frame = ref.get_frame(0)
+        clip = clip.std.SetFrameProps(
+            _Matrix=Matrix(ref_frame), _Transfer=Transfer(ref_frame), _Primaries=Primaries(ref_frame)
+        )
+
+    return clip.std.AssumeFPS(fpsnum=ref.fps.numerator, fpsden=ref.fps.denominator)
+
+
+
 def padder(
     clip: vs.VideoNode, left: int = 0, right: int = 0, top: int = 0, bottom: int = 0, reflect: bool = True
 ) -> vs.VideoNode:
     """
     Pad out the pixels on the side by the given amount of pixels.
 
     There are two padding modes:
```

### Comparing `vstools-2.2.0/vstools/utils/other.py` & `vstools-2.2.1/vstools/utils/other.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/props.py` & `vstools-2.2.1/vstools/utils/props.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/ranges.py` & `vstools-2.2.1/vstools/utils/ranges.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/scale.py` & `vstools-2.2.1/vstools/utils/scale.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/vs_enums.py` & `vstools-2.2.1/vstools/utils/vs_enums.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools/utils/vs_proxy.py` & `vstools-2.2.1/vstools/utils/vs_proxy.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.0/vstools.egg-info/PKG-INFO` & `vstools-2.2.1/vstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstools
-Version: 2.2.0
+Version: 2.2.1
 Summary: Functions and utils related to VapourSynth
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-tools
 Project-URL: Documentation, https://vstools.encoding.moe/en/latest/
```

### Comparing `vstools-2.2.0/vstools.egg-info/SOURCES.txt` & `vstools-2.2.1/vstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

