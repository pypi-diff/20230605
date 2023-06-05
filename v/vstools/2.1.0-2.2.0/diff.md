# Comparing `tmp/vstools-2.1.0.tar.gz` & `tmp/vstools-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstools-2.1.0.tar", last modified: Thu May  4 21:57:25 2023, max compression
+gzip compressed data, was "vstools-2.2.0.tar", last modified: Mon Jun  5 13:57:16 2023, max compression
```

## Comparing `vstools-2.1.0.tar` & `vstools-2.2.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.836536 vstools-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 21:57:03.000000 vstools-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 21:57:25.836536 vstools-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 21:57:03.000000 vstools-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:57:25.836536 vstools-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-04 21:57:03.000000 vstools-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34196 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/enums/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/exceptions/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/timecodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20161 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.836536 vstools-2.1.0/vstools/types/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.836536 vstools-2.1.0/vstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/__file_headers.json
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/clips.py
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/ffprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/mime_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/props.py
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/vs_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    25122 2023-05-04 21:57:03.000000 vstools-2.1.0/vstools/utils/vs_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:25.832536 vstools-2.1.0/vstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 21:57:25.000000 vstools-2.1.0/vstools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.983360 vstools-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 13:56:54.000000 vstools-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 13:57:16.983360 vstools-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 13:56:54.000000 vstools-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 13:57:16.983360 vstools-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-05 13:56:54.000000 vstools-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.975360 vstools-2.2.0/vstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.979360 vstools-2.2.0/vstools/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34510 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/enums/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.979360 vstools-2.2.0/vstools/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/exceptions/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.979360 vstools-2.2.0/vstools/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/timecodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.979360 vstools-2.2.0/vstools/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/types/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.983360 vstools-2.2.0/vstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/__file_headers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/clips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/ffprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/mime_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27233 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/vs_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-06-05 13:56:54.000000 vstools-2.2.0/vstools/utils/vs_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:57:16.975360 vstools-2.2.0/vstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 13:57:16.000000 vstools-2.2.0/vstools.egg-info/top_level.txt
```

### Comparing `vstools-2.1.0/LICENSE` & `vstools-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/PKG-INFO` & `vstools-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstools
-Version: 2.1.0
+Version: 2.2.0
 Summary: Functions and utils related to VapourSynth
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-tools
 Project-URL: Documentation, https://vstools.encoding.moe/en/latest/
```

### Comparing `vstools-2.1.0/README.md` & `vstools-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/setup.cfg` & `vstools-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/setup.py` & `vstools-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/enums/base.py` & `vstools-2.2.0/vstools/enums/base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/enums/color.py` & `vstools-2.2.0/vstools/enums/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,15 +476,21 @@
                 return Transfer.BT470BG
 
             return Transfer.BT601
 
         if width <= 2048 and height <= 1536:
             return Transfer.BT709
 
-        return Transfer.ST2084
+        if fmt.bits_per_sample == 10:
+            return Transfer.BT2020_10bits
+
+        if fmt.bits_per_sample == 12:
+            return Transfer.BT2020_12bits
+
+        return Transfer.BT709
 
     @classmethod
     def from_video(
         cls, src: vs.VideoNode | vs.VideoFrame | vs.FrameProps, strict: bool = False, func: FuncExceptT | None = None
     ) -> Transfer:
         """
         Obtain the transfer of a clip from the frame properties.
@@ -984,14 +990,21 @@
     | RGB clips will always be FULL range!
     """
 
     @classmethod
     def from_res(cls, frame: vs.VideoNode | vs.VideoFrame) -> ColorRange:
         """Guess the color range from the frame resolution."""
 
+        from ..utils import get_var_infos
+
+        fmt, w, h = get_var_infos(frame)
+
+        if fmt.color_family == vs.RGB:
+            return cls.FULL
+
         return cls.LIMITED
 
     @classmethod
     def from_video(
         cls, src: vs.VideoNode | vs.VideoFrame | vs.FrameProps, strict: bool = False, func: FuncExceptT | None = None
     ) -> ColorRange:
         """
```

### Comparing `vstools-2.1.0/vstools/enums/generic.py` & `vstools-2.2.0/vstools/enums/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     def field(self) -> int:
         """
         Check what field the enum signifies.
 
         :raises UnsupportedFieldBasedError:      PROGRESSIVE value is passed.
         """
 
-        if self.PROGRESSIVE:
+        if self == self.PROGRESSIVE:
             raise UnsupportedFieldBasedError(
                 'Progressive video aren\'t field based!',
                 f'{self.__class__.__name__}.field'
             )
 
         return self.value - 1
```

### Comparing `vstools-2.1.0/vstools/enums/other.py` & `vstools-2.2.0/vstools/enums/other.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/enums/stubs.py` & `vstools-2.2.0/vstools/enums/stubs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/exceptions/base.py` & `vstools-2.2.0/vstools/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/exceptions/color.py` & `vstools-2.2.0/vstools/exceptions/color.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/exceptions/enum.py` & `vstools-2.2.0/vstools/exceptions/enum.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/exceptions/file.py` & `vstools-2.2.0/vstools/exceptions/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/exceptions/generic.py` & `vstools-2.2.0/vstools/exceptions/generic.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/exceptions/module.py` & `vstools-2.2.0/vstools/exceptions/module.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/functions/check.py` & `vstools-2.2.0/vstools/functions/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,16 +99,14 @@
         return cast(Callable[[F], F], partial(disallow_variable_resolution, only_first=only_first))
 
     return _check_variable(
         function, 'resolution', VariableResolutionError, only_first, lambda x: not all({x.width, x.height})
     )
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def check_ref_clip(src: vs.VideoNode, ref: vs.VideoNode | None, func: FuncExceptT | None = None) -> None:
     """
     Decorator for ensuring the ref clip's format matches that of the input clip.
 
     If no ref clip can be found, this decorator will simply do nothing.
 
     :param src:     Input clip.
```

### Comparing `vstools-2.1.0/vstools/functions/clip.py` & `vstools-2.2.0/vstools/functions/clip.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/functions/funcs.py` & `vstools-2.2.0/vstools/functions/funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Callable, Concatenate, Iterable, Sequence, overload
 
 import vapoursynth as vs
 
+from ..enums import ColorRange, ColorRangeT, Matrix, MatrixT
 from ..exceptions import CustomRuntimeError, InvalidColorFamilyError
 from ..types import (
     MISSING, ConstantFormatVideoNode, FuncExceptT, HoldsVideoFormatT, KwargsT, MissingT, P, PlanesT, R, T, VideoFormatT,
     cachedproperty
 )
 from .check import check_variable
 from .normalize import normalize_planes, normalize_seq, to_arr
@@ -177,34 +178,41 @@
         - Handy properties for common code paths, and improve code readability.
     """
 
     def __init__(
         self, clip: vs.VideoNode, func: FuncExceptT, planes: PlanesT = None,
         color_family: VideoFormatT | HoldsVideoFormatT | vs.ColorFamily | Iterable[
             VideoFormatT | HoldsVideoFormatT | vs.ColorFamily
-        ] | None = None, bitdepth: int | range | None = None, strict: bool = False
+        ] | None = None, bitdepth: int | range | tuple[int, int] | None = None, strict: bool = False,
+        *, matrix: MatrixT | None = None, range_in: ColorRangeT | None = None
     ) -> None:
         from ..utils import get_color_family
 
         assert check_variable(clip, func)
 
         if color_family is not None:
             color_family = [get_color_family(c) for c in to_arr(color_family)]  # type: ignore
 
             if strict:
                 InvalidColorFamilyError.check(clip, color_family, func)
 
+        if isinstance(bitdepth, tuple):
+            bitdepth = range(*bitdepth)
+
         self.clip = clip
         self.planes = planes
         self.func = func
         self.strict = strict
         self.allowed_cfamilies = color_family
         self.cfamily_converted = False
         self.bitdepth = bitdepth
 
+        self._matrix = matrix
+        self._range_in = range_in
+
         self.norm_planes = normalize_planes(self.norm_clip, planes)
 
         super().__init__(self.norm_planes)
 
         self.num_planes = self.work_clip.format.num_planes
 
     @cachedproperty
@@ -245,14 +253,28 @@
     def chroma_planes(self) -> list[vs.VideoNode]:
         """Get chroma planes if possible."""
 
         if self != [0] or self.norm_clip.format.num_planes == 1:
             return []
         return [plane(self.norm_clip, i) for i in {1, 2}]
 
+    @cachedproperty
+    def matrix(self) -> Matrix:
+        return (
+            Matrix.from_param(self._matrix, self.func)
+            or Matrix.from_video(self.work_clip, self.strict, self.func)
+        )
+
+    @cachedproperty
+    def color_range(self) -> ColorRange:
+        return (
+            ColorRange.from_param(self._range_in, self.func)
+            or ColorRange.from_video(self.work_clip, self.strict, self.func)
+        )
+
     @property
     def is_float(self) -> bool:
         """Whether the clip is of float sample type."""
 
         return self.norm_clip.format.sample_type is vs.FLOAT
 
     @property
```

### Comparing `vstools-2.1.0/vstools/functions/heuristics.py` & `vstools-2.2.0/vstools/functions/heuristics.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/functions/normalize.py` & `vstools-2.2.0/vstools/functions/normalize.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     'normalize_planes',
     'to_arr',
     'flatten', 'flatten_vnodes',
     'normalize_list_to_ranges',
     'normalize_ranges_to_list',
     'normalize_franges',
     'normalize_ranges',
+    'invert_ranges',
     'norm_func_name', 'norm_display_name'
 ]
 
 
 @overload
 def normalize_seq(val: Sequence[T], length: int = 3) -> list[T]:
     ...
@@ -38,18 +39,17 @@
     :param length:  Amount of items in the output. Default: 3.
                     If original sequence length is less that this,
                     the last item will be repeated.
 
     :return:        List of normalized values with a set amount of items.
     """
 
-    if not isinstance(val, Sequence):
-        return [val] * length
+    val = to_arr(val)
 
-    val = list(val) + [val[-1]] * (length - len(val))
+    val += [val[-1]] * (length - len(val))
 
     return val[:length]
 
 
 def normalize_planes(clip: vs.VideoNode, planes: PlanesT = None) -> list[int]:
     """
     Normalize a sequence of planes.
@@ -156,15 +156,15 @@
         step = -1 if stop < start else 1
 
         return range(start, stop + step, step)
 
     return franges
 
 
-def normalize_list_to_ranges(flist: Sequence[int], min_length: int = 0) -> list[tuple[int, int]]:
+def normalize_list_to_ranges(flist: Iterable[int], min_length: int = 0) -> list[tuple[int, int]]:
     flist2 = list[list[int]]()
     flist3 = list[int]()
 
     prev_n = -1
 
     for n in sorted(set(flist)):
         if prev_n + 1 != n:
@@ -206,17 +206,17 @@
     Examples:
 
     .. code-block:: python
 
         >>> clip.num_frames
         1000
         >>> normalize_ranges(clip, (None, None))
-        [(0, 1000)]
+        [(0, 999)]
         >>> normalize_ranges(clip, (24, -24))
-        [(24, 976)]
+        [(24, 975)]
         >>> normalize_ranges(clip, [(24, 100), (80, 150)])
         [(24, 150)]
 
 
     :param clip:        Input clip.
     :param franges:     Frame range or list of frame ranges.
 
@@ -250,14 +250,24 @@
         out.append((start, end))
 
     return normalize_list_to_ranges([
         x for start, end in out for x in range(start, end + 1)
     ])
 
 
+def invert_ranges(
+    clipa: vs.VideoNode, clipb: vs.VideoNode | None, ranges: FrameRangeN | FrameRangesN
+) -> list[tuple[int, int]]:
+    norm_ranges = normalize_ranges(clipb or clipa, ranges)
+
+    b_frames = {*normalize_ranges_to_list(norm_ranges)}
+
+    return normalize_list_to_ranges({*range(clipa.num_frames)} - b_frames)
+
+
 def norm_func_name(func_name: SupportsString | F) -> str:
     """Normalize a class, function, or other object to obtain its name"""
 
     if isinstance(func_name, str):
         return func_name.strip()
 
     if not isinstance(func_name, type) and not callable(func_name):
```

### Comparing `vstools-2.1.0/vstools/functions/progress.py` & `vstools-2.2.0/vstools/functions/progress.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/functions/render.py` & `vstools-2.2.0/vstools/functions/render.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/functions/timecodes.py` & `vstools-2.2.0/vstools/functions/timecodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         major_time, minor_fps = self.accumulate_norm_timecodes(self)
 
         assumed_clip = clip.std.AssumeFPS(None, major_time.numerator, major_time.denominator)
 
         for other_fps, fps_ranges in minor_fps.items():
             assumed_clip = replace_ranges(
                 assumed_clip, clip.std.AssumeFPS(None, other_fps.numerator, other_fps.denominator),
-                fps_ranges, False, False, False
+                fps_ranges, mismatch=True
             )
 
         return assumed_clip
 
     def to_file(self, out: FilePathType, format: int = V2, func: FuncExceptT | None = None) -> None:
         from ..utils import check_perms
```

### Comparing `vstools-2.1.0/vstools/functions/utils.py` & `vstools-2.2.0/vstools/functions/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from weakref import WeakValueDictionary
 
 import vapoursynth as vs
 
 from ..enums import ColorRange, ColorRangeT, CustomStrEnum, Matrix
 from ..exceptions import ClipLengthError, CustomIndexError, CustomValueError, InvalidColorFamilyError
 from ..types import HoldsVideoFormatT, PlanesT, VideoFormatT
-from .check import disallow_variable_format
+from .check import check_variable_format, disallow_variable_format
 
 __all__ = [
     'EXPR_VARS',
 
     'DitherType',
 
     'depth', 'depth_func',
@@ -252,15 +252,14 @@
         blank_clip = _f2c_cache[key]
 
     frame_cp = frame.copy()
 
     return blank_clip.std.ModifyFrame(blank_clip, lambda n, f: frame_cp)
 
 
-@disallow_variable_format
 def get_y(clip: vs.VideoNode, /) -> vs.VideoNode:
     """
     Extract the luma (Y) plane of the given clip.
 
     :param clip:                Input clip.
 
     :return:                    Y plane of the input clip.
@@ -269,15 +268,14 @@
     """
 
     InvalidColorFamilyError.check(clip, [vs.YUV, vs.GRAY], get_y)
 
     return plane(clip, 0)
 
 
-@disallow_variable_format
 def get_u(clip: vs.VideoNode, /) -> vs.VideoNode:
     """
     Extract the first chroma (U) plane of the given clip.
 
     :param clip:                Input clip.
 
     :return:                    Y plane of the input clip.
@@ -286,15 +284,14 @@
     """
 
     InvalidColorFamilyError.check(clip, vs.YUV, get_u)
 
     return plane(clip, 1)
 
 
-@disallow_variable_format
 def get_v(clip: vs.VideoNode, /) -> vs.VideoNode:
     """
     Extract the second chroma (V) plane of the given clip.
 
     :param clip:                Input clip.
 
     :return:                    V plane of the input clip.
@@ -303,15 +300,14 @@
     """
 
     InvalidColorFamilyError.check(clip, vs.YUV, get_v)
 
     return plane(clip, 2)
 
 
-@disallow_variable_format
 def get_r(clip: vs.VideoNode, /) -> vs.VideoNode:
     """
     Extract the red plane of the given clip.
 
     :param clip:                Input clip.
 
     :return:                    R plane of the input clip.
@@ -320,15 +316,14 @@
     """
 
     InvalidColorFamilyError.check(clip, vs.RGB, get_r)
 
     return plane(clip, 0)
 
 
-@disallow_variable_format
 def get_g(clip: vs.VideoNode, /) -> vs.VideoNode:
     """
     Extract the green plane of the given clip.
 
     :param clip:                Input clip.
 
     :return:                    G plane of the input clip.
@@ -337,15 +332,14 @@
     """
 
     InvalidColorFamilyError.check(clip, vs.RGB, get_g)
 
     return plane(clip, 1)
 
 
-@disallow_variable_format
 def get_b(clip: vs.VideoNode, /) -> vs.VideoNode:
     """
     Extract the blue plane of the given clip.
 
     :param clip:                Input clip.
 
     :return:                    B plane of the input clip.
@@ -575,46 +569,44 @@
         return clip
     elif n_clips > 4:
         raise CustomValueError('Too many clips or planes passed!', join)
 
     raise CustomValueError('Not enough clips or planes passed!', join)
 
 
-@disallow_variable_format
 def plane(clip: vs.VideoNode, index: int, /, strict: bool = True) -> vs.VideoNode:
     """
     Extract a plane from the given clip.
 
     :param clip:        Input clip.
     :param index:       Index of the plane to extract.
 
     :return:            Grayscale clip of the clip's plane.
     """
 
-    assert clip.format
+    assert check_variable_format(clip, plane)
 
     if clip.format.num_planes == 1 and index == 0:
         return clip
 
     if not strict:
         if clip.format.color_family is vs.RGB:
             clip = clip.std.RemoveFrameProps('_Matrix')
 
     return vs.core.std.ShufflePlanes(clip, index, vs.GRAY)
 
 
-@disallow_variable_format
 def split(clip: vs.VideoNode, /) -> list[vs.VideoNode]:
     """
     Split a clip into a list of individual planes.
 
     :param clip:    Input clip.
 
     :return:        List of individual planes.
     """
 
-    assert clip.format
+    assert check_variable_format(clip, split)
 
     return [clip] if clip.format.num_planes == 1 else cast(list[vs.VideoNode], clip.std.SplitPlanes())
 
 
 depth_func = depth
```

### Comparing `vstools-2.1.0/vstools/types/builtins.py` & `vstools-2.2.0/vstools/types/builtins.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/types/funcs.py` & `vstools-2.2.0/vstools/types/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/types/generic.py` & `vstools-2.2.0/vstools/types/generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Literal, Protocol, TypeAlias, TypeVar, Union
+from typing import Any, Callable, Literal, Protocol, TypeAlias, TypeVar, Union, TYPE_CHECKING
 from enum import Enum, auto
 import vapoursynth as vs
 
 from .builtins import F, SingleOrArr, SingleOrArrOpt, SupportsString
 
 __all__ = [
     'MissingT', 'MISSING',
@@ -54,16 +54,25 @@
 
 BoundVSMapValue = TypeVar('BoundVSMapValue', bound=VSMapValue)
 """Type variable that can be one of the types in a VSMapValue."""
 
 VSMapValueCallback = Callable[..., VSMapValue]
 """Callback that can be held in a VSMap. It can only return values representable in a VSMap."""
 
-VideoFormatT = Union[vs.PresetFormat, vs.VideoFormat]
-"""Types representing a clear VideoFormat."""
+if TYPE_CHECKING:
+    from ..utils.vs_enums import VSPresetVideoFormat
+    VideoFormatT = Union[VSPresetVideoFormat, vs.VideoFormat]
+    """Types representing a clear VideoFormat."""
+else:
+    if hasattr(vs, 'PresetFormat'):
+        VideoFormatT = Union[vs.PresetFormat, vs.VideoFormat]
+        """Types representing a clear VideoFormat."""
+    else:
+        VideoFormatT = Union[vs.PresetVideoFormat, vs.VideoFormat]
+        """Types representing a clear VideoFormat."""
 
 # TODO change to | when mypy fixes bug upstream
 HoldsVideoFormatT = Union[vs.VideoNode, vs.VideoFrame, vs.VideoFormat]
 """Types from which a clear VideoFormat can be retrieved."""
 
 HoldsPropValueT = Union[vs.FrameProps, vs.VideoFrame, vs.AudioFrame, vs.VideoNode, vs.AudioNode]
 """Types that can hold :py:attr:`vs.FrameProps`."""
```

### Comparing `vstools-2.1.0/vstools/types/utils.py` & `vstools-2.2.0/vstools/types/utils.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/__file_headers.json` & `vstools-2.2.0/vstools/utils/__file_headers.json`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/__init__.py` & `vstools-2.2.0/vstools/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from . import vs_proxy as vapoursynth
+from .cache import *  # noqa: F401, F403
 from .clips import *  # noqa: F401, F403
 from .colors import *  # noqa: F401, F403
 from .ffprobe import *  # noqa: F401, F403
 from .file import *  # noqa: F401, F403
 from .funcs import *  # noqa: F401, F403
 from .info import *  # noqa: F401, F403
 from .math import *  # noqa: F401, F403
```

### Comparing `vstools-2.1.0/vstools/utils/clips.py` & `vstools-2.2.0/vstools/utils/clips.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/colors.py` & `vstools-2.2.0/vstools/utils/colors.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/ffprobe.py` & `vstools-2.2.0/vstools/utils/ffprobe.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/file.py` & `vstools-2.2.0/vstools/utils/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/funcs.py` & `vstools-2.2.0/vstools/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/info.py` & `vstools-2.2.0/vstools/utils/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,21 +39,23 @@
 
 @disallow_variable_format
 def get_video_format(
     value: int | VideoFormatT | HoldsVideoFormatT, /, *, sample_type: int | vs.SampleType | None = None
 ) -> vs.VideoFormat:
     """Get format of a given value."""
 
+    from ..utils.vs_enums import VSPresetVideoFormat
+
     if sample_type is not None:
         sample_type = vs.SampleType(sample_type)
 
     if isinstance(value, vs.VideoFormat):
         return value  # type: ignore
 
-    if isinstance(value, vs.PresetFormat):
+    if isinstance(value, VSPresetVideoFormat):
         return vs.core.get_video_format(value)
 
     if isinstance(value, int):
         if value > 32:
             return vs.core.get_video_format(value)
 
         if sample_type is None:
@@ -266,15 +268,15 @@
     """
 
     if isinstance(ar_or_ref, (vs.VideoNode, vs.VideoFrame)):
         assert (ref := ar_or_ref).format  # type: ignore
         aspect_ratio = ref.height / ref.width  # type: ignore
         mod = fallback(mod, ref.format.subsampling_h and 2 << ref.format.subsampling_h)  # type: ignore
     else:
-        aspect_ratio = ar_or_ref
+        aspect_ratio = 1.0 / ar_or_ref  # type: ignore
 
         if mod is None:
             mod = 0 if width % 2 else 2
 
     height = width * aspect_ratio
 
     if mod:
```

### Comparing `vstools-2.1.0/vstools/utils/math.py` & `vstools-2.2.0/vstools/utils/math.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/mime.py` & `vstools-2.2.0/vstools/utils/mime.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/mime_base.py` & `vstools-2.2.0/vstools/utils/mime_base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/misc.py` & `vstools-2.2.0/vstools/utils/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from fractions import Fraction
 from math import floor
 from typing import Any, Callable, Iterable, TypeVar
 
 import vapoursynth as vs
 
 from ..exceptions import InvalidSubsamplingError
-from ..functions import disallow_variable_format, disallow_variable_resolution
 from .info import get_video_format
 
 __all__ = [
     'change_fps',
 
     'padder',
 
@@ -46,16 +45,14 @@
     new_fps_clip = clip.std.BlankClip(
         length=floor(clip.num_frames * factor), fpsnum=dest_num, fpsden=dest_den
     )
 
     return new_fps_clip.std.FrameEval(lambda n: clip[round(n / factor)])
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def padder(
     clip: vs.VideoNode, left: int = 0, right: int = 0, top: int = 0, bottom: int = 0, reflect: bool = True
 ) -> vs.VideoNode:
     """
     Pad out the pixels on the side by the given amount of pixels.
 
     There are two padding modes:
@@ -74,16 +71,19 @@
     :param left:        Padding added to the left side of the clip.
     :param right:       Padding added to the right side of the clip.
     :param top:         Padding added to the top side of the clip.
     :param bottom:      Padding added to the bottom side of the clip.
     :param reflect:     Whether to reflect the padded pixels.
                         Default: True.
     """
+    from ..functions import check_variable
     from ..utils import core
 
+    assert check_variable(clip, padder)
+
     width = clip.width + left + right
     height = clip.height + top + bottom
 
     fmt = get_video_format(clip)
 
     if (width % (1 << fmt.subsampling_w) != 0) or (height % (1 << fmt.subsampling_h) != 0):
         raise InvalidSubsamplingError(
@@ -104,16 +104,14 @@
     )
 
 
 FINT = TypeVar('FINT', bound=Callable[..., vs.VideoNode])
 FFLOAT = TypeVar('FFLOAT', bound=Callable[..., vs.VideoNode])
 
 
-@disallow_variable_format
-@disallow_variable_resolution
 def pick_func_stype(clip: vs.VideoNode, func_int: FINT, func_float: FFLOAT) -> FINT | FFLOAT:
     """
     Pick the function matching the sample type of the clip's format.
 
     :param clip:        Input clip.
     :param func_int:    Function to run on integer clips.
     :param func_float:  Function to run on float clips.
@@ -124,18 +122,26 @@
     assert clip.format
 
     return func_float if clip.format.sample_type == vs.FLOAT else func_int
 
 
 def set_output(
     node: vs.RawNode | Iterable[vs.RawNode | Iterable[vs.RawNode | Iterable[vs.RawNode]]],
-    name: str | bool = True, **kwargs: Any
+    name: str | bool = True, cache: bool | None = None, **kwargs: Any
 ) -> None:
     """Set output node with optional name, and if available, use vspreview set_output."""
     from ..functions import flatten
+    from ..utils import cache_clip
+
+    if cache is None:
+        try:
+            from vspreview import is_preview
+            cache = is_preview()
+        except Exception:
+            ...
 
     last_index = len(vs.get_outputs())
 
     ref_id = str(id(node))
 
     title = 'Node'
 
@@ -165,18 +171,24 @@
                 name = vname
                 break
 
     try:
         from vspreview import set_output as vsp_set_output
         if isinstance(node, list):
             for idx, n in enumerate(node, 0 if index else last_index):
+                if cache:
+                    n = cache_clip(n)
                 vsp_set_output(n, name and f'{name} {idx}', **kwargs)
         else:
-            vsp_set_output(node, name, **kwargs)
+            vsp_set_output(cache_clip(node) if cache else node, name, **kwargs)
     except ModuleNotFoundError:
         if isinstance(name, str) and isinstance(node, vs.VideoNode):
             if isinstance(node, list):
                 for idx, n in enumerate(node, 0 if index else last_index):
+                    if cache:
+                        n = cache_clip(n)
                     n.std.SetFrameProp('Name', data=f'{name.title()} {idx}').set_output(last_index)
                     last_index += 1
             else:
+                if cache:
+                    n = cache_clip(n)
                 n.std.SetFrameProp('Name', data=name.title()).set_output(last_index)
```

### Comparing `vstools-2.1.0/vstools/utils/other.py` & `vstools-2.2.0/vstools/utils/other.py`

 * *Files identical despite different names*

### Comparing `vstools-2.1.0/vstools/utils/props.py` & `vstools-2.2.0/vstools/utils/props.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, TypeVar, overload
+from typing import Any, Callable, TypeVar, overload
 
 import vapoursynth as vs
 
 from ..enums import PropEnum
 from ..exceptions import FramePropError
 from ..types import MISSING, BoundVSMapValue, FuncExceptT, HoldsPropValueT, MissingT, SupportsString
 
@@ -41,23 +41,23 @@
 ) -> BoundVSMapValue | DT:
     ...
 
 
 @overload
 def get_prop(
     obj: HoldsPropValueT, key: SupportsString | PropEnum, t: type[BoundVSMapValue],
-    cast: type[CT], default: DT | MissingT = MISSING,
+    cast: type[CT] | Callable[[BoundVSMapValue], CT], default: DT | MissingT = MISSING,
     func: FuncExceptT | None = None
 ) -> CT | DT:
     ...
 
 
 def get_prop(
     obj: HoldsPropValueT, key: SupportsString | PropEnum, t: type[BoundVSMapValue],
-    cast: type[CT] | None = None, default: DT | MissingT = MISSING,
+    cast: type[CT] | Callable[[BoundVSMapValue], CT] | None = None, default: DT | MissingT = MISSING,
     func: FuncExceptT | None = None
 ) -> BoundVSMapValue | CT | DT:
     """
     Get FrameProp ``prop`` from frame ``frame`` with expected type ``t`` to satisfy the type checker.
 
     :param frame:               Frame containing props.
     :param key:                 Prop to get.
```

### Comparing `vstools-2.1.0/vstools/utils/ranges.py` & `vstools-2.2.0/vstools/utils/ranges.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import warnings
 from itertools import chain, zip_longest
-from typing import Callable, Iterable, Union, overload
+from typing import Any, Callable, Iterable, Union, overload
 
 import vapoursynth as vs
 
 from ..exceptions import (
     CustomIndexError, CustomValueError, FormatsMismatchError, FramerateMismatchError, LengthMismatchError,
     ResolutionsMismatchError
 )
 from ..functions import check_ref_clip
-from ..types import T0, FrameRangeN, FrameRangesN, T
+from ..types import T0, FrameRangeN, FrameRangesN, T, copy_signature
 
 __all__ = [
     'replace_ranges', 'rfs',
 
     'ranges_product',
 
     'interleave_arr'
@@ -88,57 +88,49 @@
 def replace_ranges(
     clip_a: vs.VideoNode, clip_b: vs.VideoNode,
     ranges: FrameRangeN | FrameRangesN | RangesCallback | None,
     exclusive: bool = False, use_plugin: bool | None = None, mismatch: bool = False,
     *, prop_src: vs.VideoNode | list[vs.VideoNode] | None = None
 ) -> vs.VideoNode:
     """
-    Remaps frame indices in a clip using ints and tuples rather than a string.
-
+    Replaces frames in a clip, either with pre-calculated indices or on-the-fly with a callback.
     Frame ranges are inclusive. This behaviour can be changed by setting `exclusive=True`.
 
-    If you're trying to splice in clips, it's recommended you use :py:func:`insert_clip` instead.
-
-    This function will try to call the `VapourSynth-RemapFrames` plugin before doing any of its own processing.
-    This should come with a speed boost, so it's recommended you install it.
-
     Examples with clips ``black`` and ``white`` of equal length:
         * ``replace_ranges(black, white, [(0, 1)])``: replace frames 0 and 1 with ``white``
         * ``replace_ranges(black, white, [(None, None)])``: replace the entire clip with ``white``
         * ``replace_ranges(black, white, [(0, None)])``: same as previous
         * ``replace_ranges(black, white, [(200, None)])``: replace 200 until the end with ``white``
         * ``replace_ranges(black, white, [(200, -1)])``: replace 200 until the end with ``white``,
                                                          leaving 1 frame of ``black``
 
-    Alias for this function is ``rfs``.
-
     Optional Dependencies:
-        * `use_plugin=True`: Either of the following two plugins:
+        * Either of the following two plugins:
             * `VS Julek Plugin <https://github.com/dnjulek/vapoursynth-julek-plugin>`_
             * `VSRemapFrames <https://github.com/Irrational-Encoding-Wizardry/Vapoursynth-RemapFrames>`_
 
     :param clip_a:      Original clip.
     :param clip_b:      Replacement clip.
     :param ranges:      Ranges to replace clip_a (original clip) with clip_b (replacement clip).
                         Integer values in the list indicate single frames,
                         Tuple values indicate inclusive ranges.
+                        Callbacks must return true to replace a with b.
                         Negative integer values will be wrapped around based on clip_b's length.
                         None values are context dependent:
                             * None provided as sole value to ranges: no-op
                             * Single None value in list: Last frame in clip_b
                             * None as first value of tuple: 0
                             * None as second value of tuple: Last frame in clip_b
     :param exclusive:   Use exclusive ranges (Default: False).
-    :param use_plugin:  Use the ReplaceFramesSimple plugin for the rfs call (Default: True).
     :param mismatch:    Accept format or resolution mismatch between clips.
 
     :return:            Clip with ranges from clip_a replaced with clip_b.
     """
 
-    from ..functions import normalize_ranges, normalize_ranges_to_list
+    from ..functions import invert_ranges, normalize_ranges, normalize_ranges_to_list
 
     if ranges != 0 and not ranges or clip_a is clip_b:
         return clip_a
 
     if not mismatch:
         check_ref_clip(clip_a, clip_b)
 
@@ -158,38 +150,38 @@
                 'For passing f to the callback you must specify the node(s) to grab the frame from via prop_src.'
             )
 
         if 'f' in params and 'n' in params:
             return base_clip.std.FrameEval(lambda n, f: clip_b if callback(n, f) else clip_a, prop_src)  # type: ignore
 
         if 'f' in params:
-            return base_clip.std.FrameEval(lambda f: clip_b if callback(f) else clip_a, prop_src)  # type: ignore
+            return base_clip.std.FrameEval(lambda n, f: clip_b if callback(f) else clip_a, prop_src)  # type: ignore
 
         if 'n' in params:
             return base_clip.std.FrameEval(lambda n: clip_b if callback(n) else clip_a)  # type: ignore
 
         raise CustomValueError('Callback must have signature ((n, f) | (n) | (f)) -> bool!')
 
-    nranges = normalize_ranges(clip_b, ranges)
-    do_splice_trim = len(nranges) <= 5
+    b_ranges = normalize_ranges(clip_b, ranges)
+    do_splice_trim = len(b_ranges) <= 5
 
     if use_plugin is not None:
         warnings.warn('replace_ranges: use_plugin is deprecated!')
 
     if not do_splice_trim:
         try:
             if hasattr(vs.core, 'julek'):
                 return vs.core.julek.RFS(  # type: ignore
-                    clip_a, clip_b, [y for (s, e) in nranges for y in range(s, e + (not exclusive if s != e else 1))],
+                    clip_a, clip_b, [y for (s, e) in b_ranges for y in range(s, e + (not exclusive if s != e else 1))],
                     mismatch=mismatch
                 )
             elif hasattr(vs.core, 'remap'):
                 return vs.core.remap.ReplaceFramesSimple(  # type: ignore
                     clip_a, clip_b, mismatch=mismatch,
-                    mappings=' '.join(f'[{s} {e + (exclusive if s != e else 0)}]' for s, e in nranges)
+                    mappings=' '.join(f'[{s} {e + (exclusive if s != e else 0)}]' for s, e in b_ranges)
                 )
         except vs.Error as e:
             msg = str(e).replace('vapoursynth.Error: ReplaceFramesSimple: ', '')
 
             match msg:
                 case "Clip lengths don't match":
                     raise LengthMismatchError(replace_ranges, (clip_a, clip_b))
@@ -206,36 +198,38 @@
         warnings.warn(
             f"replace_ranges: 'The number of frames of the clips don't match! "
             f"({clip_a.num_frames=}, {clip_b.num_frames=})\n"
             "The function will still work, but you may run into undefined behavior, or a broken output clip!'"
         )
 
     if do_splice_trim:
-        out = clip_a
-        shift = 1 + exclusive
-
-        for start, end in nranges:
-            tmp = clip_b[start:end + shift]
+        shift = 1 - exclusive
 
-            if start != 0:
-                tmp = vs.core.std.Splice([out[: start], tmp], mismatch)
+        a_ranges = invert_ranges(clip_b, clip_a, b_ranges)
 
-            if end < out.num_frames - 1:
-                tmp = vs.core.std.Splice([tmp, out[end + shift:]], mismatch)
+        a_trims = [clip_a[start:end + shift] for start, end in a_ranges]
+        b_trims = [clip_b[start:end + shift] for start, end in b_ranges]
 
-            out = tmp
+        if a_ranges:
+            main, other = (a_trims, b_trims) if (a_ranges[0][0] == 0) else (b_trims, a_trims)
+        else:
+            main, other = (b_trims, a_trims) if (b_ranges[0][0] == 0) else (a_trims, b_trims)
 
-        return out
+        return vs.core.std.Splice(list(interleave_arr(main, other, 1)), mismatch)
 
-    b_frames = set(normalize_ranges_to_list(nranges))
+    b_frames = set(normalize_ranges_to_list(b_ranges))
     return replace_ranges(clip_a, clip_b, lambda n: n in b_frames)
 
 
 # Aliases
-rfs = replace_ranges
+@copy_signature(replace_ranges)
+def rfs(*args: Any, **kwargs: Any) -> Any:
+    import warnings
+    warnings.warn('rfs: This alias is D-E-P-R-E-C-A-T-E-D and BIG EVIL. Use replace_ranges!')
+    return replace_ranges(*args, **kwargs)
 
 
 @overload
 def ranges_product(range0: range | int, range1: range | int, /) -> Iterable[tuple[int, int]]:
     ...
 
 
@@ -284,15 +278,17 @@
     :param arr1:    Second array to be interleaved.
     :param n:       The number of elements from arr0 to include in the interleaved sequence
                     before including an element from arr1.
 
     :yield:         Elements from either arr0 or arr01.
     """
     if n == 1:
-        return [x for x in chain(*zip_longest(arr0, arr1)) if x is not None]
+        yield from (x for x in chain.from_iterable(zip_longest(arr0, arr1)) if x is not None)
+
+        return
 
     arr0_i, arr1_i = iter(arr0), iter(arr1)
     arr1_vals = arr0_vals = True
 
     while arr1_vals or arr0_vals:
         if arr0_vals:
             for _ in range(n):
```

### Comparing `vstools-2.1.0/vstools/utils/scale.py` & `vstools-2.2.0/vstools/utils/scale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Literal, Sequence, overload
 
 import vapoursynth as vs
 
 from ..enums import ColorRange, ColorRangeT
-from ..functions import disallow_variable_format, normalize_seq
+from ..functions import normalize_seq
 from ..types import HoldsVideoFormatT, VideoFormatT
 from .info import get_depth, get_video_format
 
 __all__ = [
     'scale_8bit', 'scale_value',
 
     'get_lowest_value', 'get_neutral_value', 'get_peak_value',
@@ -139,15 +139,14 @@
             out_value += 128 << (out_fmt.bits_per_sample - 8)
         elif range_in.is_full and range_out.is_limited:
             out_value += 16 << (out_fmt.bits_per_sample - 8)
 
     return out_value
 
 
-@disallow_variable_format
 def get_lowest_value(
     clip_or_depth: int | VideoFormatT | HoldsVideoFormatT, chroma: bool = False,
     range_in: ColorRangeT = ColorRange.FULL
 ) -> float:
     """
     Returns the lowest value for the specified bit depth, or bit depth of the clip/format specified.
 
@@ -165,28 +164,27 @@
 
     if chroma and fmt.sample_type == vs.FLOAT:
         return -0.5
 
     return 0.
 
 
-@disallow_variable_format
 def get_lowest_values(
     clip_or_depth: int | VideoFormatT | HoldsVideoFormatT, range_in: ColorRangeT = ColorRange.FULL
 ) -> Sequence[float]:
     """Get all planes lowest values of a format."""
 
     fmt = get_video_format(clip_or_depth)
-    return normalize_seq(
-        [get_lowest_value(fmt, False, range_in),
-         get_lowest_value(fmt, True, range_in)],
-        fmt.num_planes)
+
+    return normalize_seq([
+        get_lowest_value(fmt, False, range_in),
+        get_lowest_value(fmt, True, range_in)
+    ], fmt.num_planes)
 
 
-@disallow_variable_format
 def get_neutral_value(clip_or_depth: int | VideoFormatT | HoldsVideoFormatT, chroma: bool = False) -> float:
     """
     Returns the mid point value for the specified bit depth, or bit depth of the clip/format specified.
 
     :param clip_or_depth:   Input bit depth, or clip, frame, format from where to get it.
     :param chroma:          Whether to get luma (default) or chroma plane value.
 
@@ -197,23 +195,21 @@
 
     if fmt.sample_type == vs.FLOAT:
         return 0. if chroma else 0.5
 
     return float(1 << (get_depth(fmt) - 1))
 
 
-@disallow_variable_format
 def get_neutral_values(clip_or_depth: int | VideoFormatT | HoldsVideoFormatT) -> Sequence[float]:
     """Get all planes neutral values of a format."""
 
     fmt = get_video_format(clip_or_depth)
     return normalize_seq([get_neutral_value(fmt, False), get_neutral_value(fmt, True)], fmt.num_planes)
 
 
-@disallow_variable_format
 def get_peak_value(
     clip_or_depth: int | VideoFormatT | HoldsVideoFormatT, chroma: bool = False,
     range_in: ColorRangeT = ColorRange.FULL
 ) -> float:
     """
     Returns the peak value for the specified bit depth, or bit depth of the clip/format specified.
 
@@ -231,15 +227,14 @@
 
     if fmt.sample_type == vs.FLOAT:
         return 0.5 if chroma else 1.
 
     return (1 << get_depth(fmt)) - 1.
 
 
-@disallow_variable_format
 def get_peak_values(
     clip_or_depth: int | VideoFormatT | HoldsVideoFormatT, range_in: ColorRangeT = ColorRange.FULL
 ) -> Sequence[float]:
     """Get all planes peak values of a format."""
 
     fmt = get_video_format(clip_or_depth)
     return normalize_seq([get_peak_value(fmt, False, range_in), get_peak_value(fmt, True, range_in)], fmt.num_planes)
```

### Comparing `vstools-2.1.0/vstools/utils/vs_enums.py` & `vstools-2.2.0/vstools/utils/vs_enums.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
 from enum import IntEnum
 from typing import TYPE_CHECKING
 
 from vapoursynth import FLOAT, GRAY, INTEGER, RGB, YUV
-from vapoursynth import PresetFormat as VSPresetFormat
+
+try:
+    from vapoursynth import PresetFormat as VSPresetVideoFormat
+except ImportError:
+    from vapoursynth import PresetVideoFormat as VSPresetVideoFormat
 
 from .other import IS_DOCS
 
 __all__ = [
-    'PresetFormat',
+    'PresetVideoFormat', 'PresetVideoFormat', 'VSPresetVideoFormat',
     'GRAY8', 'GRAY9', 'GRAY10', 'GRAY11', 'GRAY12', 'GRAY13', 'GRAY14', 'GRAY15', 'GRAY16', 'GRAY17', 'GRAY18',
     'GRAY19', 'GRAY20', 'GRAY21', 'GRAY22', 'GRAY23', 'GRAY24', 'GRAY25', 'GRAY26', 'GRAY27', 'GRAY28', 'GRAY29',
     'GRAY30', 'GRAY31', 'GRAY32', 'GRAYH', 'GRAYS',
     'YUV420P8', 'YUV420P9', 'YUV420P10', 'YUV420P11', 'YUV420P12', 'YUV420P13', 'YUV420P14', 'YUV420P15', 'YUV420P16',
     'YUV420P17', 'YUV420P18', 'YUV420P19', 'YUV420P20', 'YUV420P21', 'YUV420P22', 'YUV420P23', 'YUV420P24', 'YUV420P25',
     'YUV420P26', 'YUV420P27', 'YUV420P28', 'YUV420P29', 'YUV420P30', 'YUV420P31', 'YUV420P32', 'YUV420PH', 'YUV420PS',
     'YUV444P8', 'YUV444P9', 'YUV444P10', 'YUV444P11', 'YUV444P12', 'YUV444P13', 'YUV444P14', 'YUV444P15', 'YUV444P16',
@@ -40,22 +44,22 @@
 def MAKE_VIDEO_ID(colorFamily: int, sampleType: int, bitsPerSample: int, subSamplingW: int, subSamplingH: int) -> int:
     if IS_DOCS:
         return 0
     return colorFamily << 28 | sampleType << 24 | bitsPerSample << 16 | subSamplingW << 8 | subSamplingH << 0
 
 
 if TYPE_CHECKING:
-    PresetFormatBase = VSPresetFormat
+    PresetVideoFormatBase = VSPresetVideoFormat
 else:
-    PresetFormatBase = IntEnum
+    PresetVideoFormatBase = IntEnum
 
 
 ################################################
 
-class PresetFormat(PresetFormatBase):
+class PresetVideoFormat(PresetVideoFormatBase):
     GRAY8 = MAKE_VIDEO_ID(GRAY, INTEGER, 8, 0, 0)  # type: ignore[misc,assignment]
     GRAY9 = MAKE_VIDEO_ID(GRAY, INTEGER, 9, 0, 0)  # type: ignore[misc,assignment]
     GRAY10 = MAKE_VIDEO_ID(GRAY, INTEGER, 10, 0, 0)  # type: ignore[misc,assignment]
     GRAY11 = MAKE_VIDEO_ID(GRAY, INTEGER, 11, 0, 0)
     GRAY12 = MAKE_VIDEO_ID(GRAY, INTEGER, 12, 0, 0)  # type: ignore[misc,assignment]
     GRAY13 = MAKE_VIDEO_ID(GRAY, INTEGER, 13, 0, 0)
     GRAY14 = MAKE_VIDEO_ID(GRAY, INTEGER, 14, 0, 0)  # type: ignore[misc,assignment]
@@ -295,223 +299,291 @@
     RGB93 = MAKE_VIDEO_ID(RGB, INTEGER, 31, 0, 0)
     RGB96 = MAKE_VIDEO_ID(RGB, INTEGER, 32, 0, 0)
 
     RGBH = MAKE_VIDEO_ID(RGB, FLOAT, 16, 0, 0)  # type: ignore[misc,assignment]
     RGBS = MAKE_VIDEO_ID(RGB, FLOAT, 32, 0, 0)  # type: ignore[misc,assignment]
 
 
-GRAY8 = PresetFormat.GRAY8
-GRAY9 = PresetFormat.GRAY9
-GRAY10 = PresetFormat.GRAY10
-GRAY11 = PresetFormat.GRAY11
-GRAY12 = PresetFormat.GRAY12
-GRAY13 = PresetFormat.GRAY13
-GRAY14 = PresetFormat.GRAY14
-GRAY15 = PresetFormat.GRAY15
-GRAY16 = PresetFormat.GRAY16
-GRAY17 = PresetFormat.GRAY17
-GRAY18 = PresetFormat.GRAY18
-GRAY19 = PresetFormat.GRAY19
-GRAY20 = PresetFormat.GRAY20
-GRAY21 = PresetFormat.GRAY21
-GRAY22 = PresetFormat.GRAY22
-GRAY23 = PresetFormat.GRAY23
-GRAY24 = PresetFormat.GRAY24
-GRAY25 = PresetFormat.GRAY25
-GRAY26 = PresetFormat.GRAY26
-GRAY27 = PresetFormat.GRAY27
-GRAY28 = PresetFormat.GRAY28
-GRAY29 = PresetFormat.GRAY29
-GRAY30 = PresetFormat.GRAY30
-GRAY31 = PresetFormat.GRAY31
-GRAY32 = PresetFormat.GRAY32
-GRAYH = PresetFormat.GRAYH
-GRAYS = PresetFormat.GRAYS
-YUV420P8 = PresetFormat.YUV420P8
-YUV420P9 = PresetFormat.YUV420P9
-YUV420P10 = PresetFormat.YUV420P10
-YUV420P11 = PresetFormat.YUV420P11
-YUV420P12 = PresetFormat.YUV420P12
-YUV420P13 = PresetFormat.YUV420P13
-YUV420P14 = PresetFormat.YUV420P14
-YUV420P15 = PresetFormat.YUV420P15
-YUV420P16 = PresetFormat.YUV420P16
-YUV420P17 = PresetFormat.YUV420P17
-YUV420P18 = PresetFormat.YUV420P18
-YUV420P19 = PresetFormat.YUV420P19
-YUV420P20 = PresetFormat.YUV420P20
-YUV420P21 = PresetFormat.YUV420P21
-YUV420P22 = PresetFormat.YUV420P22
-YUV420P23 = PresetFormat.YUV420P23
-YUV420P24 = PresetFormat.YUV420P24
-YUV420P25 = PresetFormat.YUV420P25
-YUV420P26 = PresetFormat.YUV420P26
-YUV420P27 = PresetFormat.YUV420P27
-YUV420P28 = PresetFormat.YUV420P28
-YUV420P29 = PresetFormat.YUV420P29
-YUV420P30 = PresetFormat.YUV420P30
-YUV420P31 = PresetFormat.YUV420P31
-YUV420P32 = PresetFormat.YUV420P32
-YUV420PH = PresetFormat.YUV420PH
-YUV420PS = PresetFormat.YUV420PS
-YUV444P8 = PresetFormat.YUV444P8
-YUV444P9 = PresetFormat.YUV444P9
-YUV444P10 = PresetFormat.YUV444P10
-YUV444P11 = PresetFormat.YUV444P11
-YUV444P12 = PresetFormat.YUV444P12
-YUV444P13 = PresetFormat.YUV444P13
-YUV444P14 = PresetFormat.YUV444P14
-YUV444P15 = PresetFormat.YUV444P15
-YUV444P16 = PresetFormat.YUV444P16
-YUV444P17 = PresetFormat.YUV444P17
-YUV444P18 = PresetFormat.YUV444P18
-YUV444P19 = PresetFormat.YUV444P19
-YUV444P20 = PresetFormat.YUV444P20
-YUV444P21 = PresetFormat.YUV444P21
-YUV444P22 = PresetFormat.YUV444P22
-YUV444P23 = PresetFormat.YUV444P23
-YUV444P24 = PresetFormat.YUV444P24
-YUV444P25 = PresetFormat.YUV444P25
-YUV444P26 = PresetFormat.YUV444P26
-YUV444P27 = PresetFormat.YUV444P27
-YUV444P28 = PresetFormat.YUV444P28
-YUV444P29 = PresetFormat.YUV444P29
-YUV444P30 = PresetFormat.YUV444P30
-YUV444P31 = PresetFormat.YUV444P31
-YUV444P32 = PresetFormat.YUV444P32
-YUV444PH = PresetFormat.YUV444PH
-YUV444PS = PresetFormat.YUV444PS
-YUV422P8 = PresetFormat.YUV422P8
-YUV422P9 = PresetFormat.YUV422P9
-YUV422P10 = PresetFormat.YUV422P10
-YUV422P11 = PresetFormat.YUV422P11
-YUV422P12 = PresetFormat.YUV422P12
-YUV422P13 = PresetFormat.YUV422P13
-YUV422P14 = PresetFormat.YUV422P14
-YUV422P15 = PresetFormat.YUV422P15
-YUV422P16 = PresetFormat.YUV422P16
-YUV422P17 = PresetFormat.YUV422P17
-YUV422P18 = PresetFormat.YUV422P18
-YUV422P19 = PresetFormat.YUV422P19
-YUV422P20 = PresetFormat.YUV422P20
-YUV422P21 = PresetFormat.YUV422P21
-YUV422P22 = PresetFormat.YUV422P22
-YUV422P23 = PresetFormat.YUV422P23
-YUV422P24 = PresetFormat.YUV422P24
-YUV422P25 = PresetFormat.YUV422P25
-YUV422P26 = PresetFormat.YUV422P26
-YUV422P27 = PresetFormat.YUV422P27
-YUV422P28 = PresetFormat.YUV422P28
-YUV422P29 = PresetFormat.YUV422P29
-YUV422P30 = PresetFormat.YUV422P30
-YUV422P31 = PresetFormat.YUV422P31
-YUV422P32 = PresetFormat.YUV422P32
-YUV422PH = PresetFormat.YUV422PH
-YUV422PS = PresetFormat.YUV422PS
-YUV411P8 = PresetFormat.YUV411P8
-YUV411P9 = PresetFormat.YUV411P9
-YUV411P10 = PresetFormat.YUV411P10
-YUV411P11 = PresetFormat.YUV411P11
-YUV411P12 = PresetFormat.YUV411P12
-YUV411P13 = PresetFormat.YUV411P13
-YUV411P14 = PresetFormat.YUV411P14
-YUV411P15 = PresetFormat.YUV411P15
-YUV411P16 = PresetFormat.YUV411P16
-YUV411P17 = PresetFormat.YUV411P17
-YUV411P18 = PresetFormat.YUV411P18
-YUV411P19 = PresetFormat.YUV411P19
-YUV411P20 = PresetFormat.YUV411P20
-YUV411P21 = PresetFormat.YUV411P21
-YUV411P22 = PresetFormat.YUV411P22
-YUV411P23 = PresetFormat.YUV411P23
-YUV411P24 = PresetFormat.YUV411P24
-YUV411P25 = PresetFormat.YUV411P25
-YUV411P26 = PresetFormat.YUV411P26
-YUV411P27 = PresetFormat.YUV411P27
-YUV411P28 = PresetFormat.YUV411P28
-YUV411P29 = PresetFormat.YUV411P29
-YUV411P30 = PresetFormat.YUV411P30
-YUV411P31 = PresetFormat.YUV411P31
-YUV411P32 = PresetFormat.YUV411P32
-YUV411PH = PresetFormat.YUV411PH
-YUV411PS = PresetFormat.YUV411PS
-YUV440P8 = PresetFormat.YUV440P8
-YUV440P9 = PresetFormat.YUV440P9
-YUV440P10 = PresetFormat.YUV440P10
-YUV440P11 = PresetFormat.YUV440P11
-YUV440P12 = PresetFormat.YUV440P12
-YUV440P13 = PresetFormat.YUV440P13
-YUV440P14 = PresetFormat.YUV440P14
-YUV440P15 = PresetFormat.YUV440P15
-YUV440P16 = PresetFormat.YUV440P16
-YUV440P17 = PresetFormat.YUV440P17
-YUV440P18 = PresetFormat.YUV440P18
-YUV440P19 = PresetFormat.YUV440P19
-YUV440P20 = PresetFormat.YUV440P20
-YUV440P21 = PresetFormat.YUV440P21
-YUV440P22 = PresetFormat.YUV440P22
-YUV440P23 = PresetFormat.YUV440P23
-YUV440P24 = PresetFormat.YUV440P24
-YUV440P25 = PresetFormat.YUV440P25
-YUV440P26 = PresetFormat.YUV440P26
-YUV440P27 = PresetFormat.YUV440P27
-YUV440P28 = PresetFormat.YUV440P28
-YUV440P29 = PresetFormat.YUV440P29
-YUV440P30 = PresetFormat.YUV440P30
-YUV440P31 = PresetFormat.YUV440P31
-YUV440P32 = PresetFormat.YUV440P32
-YUV440PH = PresetFormat.YUV440PH
-YUV440PS = PresetFormat.YUV440PS
-YUV410P8 = PresetFormat.YUV410P8
-YUV410P9 = PresetFormat.YUV410P9
-YUV410P10 = PresetFormat.YUV410P10
-YUV410P11 = PresetFormat.YUV410P11
-YUV410P12 = PresetFormat.YUV410P12
-YUV410P13 = PresetFormat.YUV410P13
-YUV410P14 = PresetFormat.YUV410P14
-YUV410P15 = PresetFormat.YUV410P15
-YUV410P16 = PresetFormat.YUV410P16
-YUV410P17 = PresetFormat.YUV410P17
-YUV410P18 = PresetFormat.YUV410P18
-YUV410P19 = PresetFormat.YUV410P19
-YUV410P20 = PresetFormat.YUV410P20
-YUV410P21 = PresetFormat.YUV410P21
-YUV410P22 = PresetFormat.YUV410P22
-YUV410P23 = PresetFormat.YUV410P23
-YUV410P24 = PresetFormat.YUV410P24
-YUV410P25 = PresetFormat.YUV410P25
-YUV410P26 = PresetFormat.YUV410P26
-YUV410P27 = PresetFormat.YUV410P27
-YUV410P28 = PresetFormat.YUV410P28
-YUV410P29 = PresetFormat.YUV410P29
-YUV410P30 = PresetFormat.YUV410P30
-YUV410P31 = PresetFormat.YUV410P31
-YUV410P32 = PresetFormat.YUV410P32
-YUV410PH = PresetFormat.YUV410PH
-YUV410PS = PresetFormat.YUV410PS
-RGB24 = PresetFormat.RGB24
-RGB27 = PresetFormat.RGB27
-RGB30 = PresetFormat.RGB30
-RGB33 = PresetFormat.RGB33
-RGB36 = PresetFormat.RGB36
-RGB39 = PresetFormat.RGB39
-RGB42 = PresetFormat.RGB42
-RGB45 = PresetFormat.RGB45
-RGB48 = PresetFormat.RGB48
-RGB51 = PresetFormat.RGB51
-RGB54 = PresetFormat.RGB54
-RGB57 = PresetFormat.RGB57
-RGB60 = PresetFormat.RGB60
-RGB63 = PresetFormat.RGB63
-RGB66 = PresetFormat.RGB66
-RGB69 = PresetFormat.RGB69
-RGB72 = PresetFormat.RGB72
-RGB75 = PresetFormat.RGB75
-RGB78 = PresetFormat.RGB78
-RGB81 = PresetFormat.RGB81
-RGB84 = PresetFormat.RGB84
-RGB87 = PresetFormat.RGB87
-RGB90 = PresetFormat.RGB90
-RGB93 = PresetFormat.RGB93
-RGB96 = PresetFormat.RGB96
-RGBH = PresetFormat.RGBH
-RGBS = PresetFormat.RGBS
+class PresetDeprecateProxy(type):
+    @classmethod
+    def _warn(cls) -> None:
+        import warnings
+        warnings.warn('vs.PresetFormat is DEPRECATED! Use PresetVideoFormat from now on!')
+
+    def __bool__(cls):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__bool__()  # type: ignore
+
+    def __call__(  # type: ignore
+        cls, value, names=None, *, module=None, qualname=None, type=None, start=1, boundary=None
+    ):
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__call__(  # type: ignore
+            value, names, module=module, qualname=qualname, type=type, start=start, boundary=boundary
+        )
+
+    def __contains__(cls, member):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__contains__(member)
+
+    def __delattr__(cls, attr):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__delattr__(attr)  # type: ignore
+
+    def __dir__(cls):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__dir__()  # type: ignore
+
+    def __getattr__(cls, name):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__getattr__(name)  # type: ignore
+
+    def __getitem__(cls, name):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__getitem__(name)
+
+    def __iter__(cls):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__iter__()
+
+    def __len__(cls):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__len__()
+
+    @property
+    def __members__(cls):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__members__()
+
+    def __repr__(cls):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__repr__()  # type: ignore
+
+    def __reversed__(cls):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__reversed__()
+
+    def __setattr__(cls, name, value):  # type: ignore
+        PresetDeprecateProxy._warn()
+        return PresetVideoFormat.__setattr__(name, value)  # type: ignore
+
+
+class PresetFormat(metaclass=PresetDeprecateProxy):
+    """Deprecated, use PresetVideoFormat"""
+
+
+GRAY8 = PresetVideoFormat.GRAY8
+GRAY9 = PresetVideoFormat.GRAY9
+GRAY10 = PresetVideoFormat.GRAY10
+GRAY11 = PresetVideoFormat.GRAY11
+GRAY12 = PresetVideoFormat.GRAY12
+GRAY13 = PresetVideoFormat.GRAY13
+GRAY14 = PresetVideoFormat.GRAY14
+GRAY15 = PresetVideoFormat.GRAY15
+GRAY16 = PresetVideoFormat.GRAY16
+GRAY17 = PresetVideoFormat.GRAY17
+GRAY18 = PresetVideoFormat.GRAY18
+GRAY19 = PresetVideoFormat.GRAY19
+GRAY20 = PresetVideoFormat.GRAY20
+GRAY21 = PresetVideoFormat.GRAY21
+GRAY22 = PresetVideoFormat.GRAY22
+GRAY23 = PresetVideoFormat.GRAY23
+GRAY24 = PresetVideoFormat.GRAY24
+GRAY25 = PresetVideoFormat.GRAY25
+GRAY26 = PresetVideoFormat.GRAY26
+GRAY27 = PresetVideoFormat.GRAY27
+GRAY28 = PresetVideoFormat.GRAY28
+GRAY29 = PresetVideoFormat.GRAY29
+GRAY30 = PresetVideoFormat.GRAY30
+GRAY31 = PresetVideoFormat.GRAY31
+GRAY32 = PresetVideoFormat.GRAY32
+GRAYH = PresetVideoFormat.GRAYH
+GRAYS = PresetVideoFormat.GRAYS
+YUV420P8 = PresetVideoFormat.YUV420P8
+YUV420P9 = PresetVideoFormat.YUV420P9
+YUV420P10 = PresetVideoFormat.YUV420P10
+YUV420P11 = PresetVideoFormat.YUV420P11
+YUV420P12 = PresetVideoFormat.YUV420P12
+YUV420P13 = PresetVideoFormat.YUV420P13
+YUV420P14 = PresetVideoFormat.YUV420P14
+YUV420P15 = PresetVideoFormat.YUV420P15
+YUV420P16 = PresetVideoFormat.YUV420P16
+YUV420P17 = PresetVideoFormat.YUV420P17
+YUV420P18 = PresetVideoFormat.YUV420P18
+YUV420P19 = PresetVideoFormat.YUV420P19
+YUV420P20 = PresetVideoFormat.YUV420P20
+YUV420P21 = PresetVideoFormat.YUV420P21
+YUV420P22 = PresetVideoFormat.YUV420P22
+YUV420P23 = PresetVideoFormat.YUV420P23
+YUV420P24 = PresetVideoFormat.YUV420P24
+YUV420P25 = PresetVideoFormat.YUV420P25
+YUV420P26 = PresetVideoFormat.YUV420P26
+YUV420P27 = PresetVideoFormat.YUV420P27
+YUV420P28 = PresetVideoFormat.YUV420P28
+YUV420P29 = PresetVideoFormat.YUV420P29
+YUV420P30 = PresetVideoFormat.YUV420P30
+YUV420P31 = PresetVideoFormat.YUV420P31
+YUV420P32 = PresetVideoFormat.YUV420P32
+YUV420PH = PresetVideoFormat.YUV420PH
+YUV420PS = PresetVideoFormat.YUV420PS
+YUV444P8 = PresetVideoFormat.YUV444P8
+YUV444P9 = PresetVideoFormat.YUV444P9
+YUV444P10 = PresetVideoFormat.YUV444P10
+YUV444P11 = PresetVideoFormat.YUV444P11
+YUV444P12 = PresetVideoFormat.YUV444P12
+YUV444P13 = PresetVideoFormat.YUV444P13
+YUV444P14 = PresetVideoFormat.YUV444P14
+YUV444P15 = PresetVideoFormat.YUV444P15
+YUV444P16 = PresetVideoFormat.YUV444P16
+YUV444P17 = PresetVideoFormat.YUV444P17
+YUV444P18 = PresetVideoFormat.YUV444P18
+YUV444P19 = PresetVideoFormat.YUV444P19
+YUV444P20 = PresetVideoFormat.YUV444P20
+YUV444P21 = PresetVideoFormat.YUV444P21
+YUV444P22 = PresetVideoFormat.YUV444P22
+YUV444P23 = PresetVideoFormat.YUV444P23
+YUV444P24 = PresetVideoFormat.YUV444P24
+YUV444P25 = PresetVideoFormat.YUV444P25
+YUV444P26 = PresetVideoFormat.YUV444P26
+YUV444P27 = PresetVideoFormat.YUV444P27
+YUV444P28 = PresetVideoFormat.YUV444P28
+YUV444P29 = PresetVideoFormat.YUV444P29
+YUV444P30 = PresetVideoFormat.YUV444P30
+YUV444P31 = PresetVideoFormat.YUV444P31
+YUV444P32 = PresetVideoFormat.YUV444P32
+YUV444PH = PresetVideoFormat.YUV444PH
+YUV444PS = PresetVideoFormat.YUV444PS
+YUV422P8 = PresetVideoFormat.YUV422P8
+YUV422P9 = PresetVideoFormat.YUV422P9
+YUV422P10 = PresetVideoFormat.YUV422P10
+YUV422P11 = PresetVideoFormat.YUV422P11
+YUV422P12 = PresetVideoFormat.YUV422P12
+YUV422P13 = PresetVideoFormat.YUV422P13
+YUV422P14 = PresetVideoFormat.YUV422P14
+YUV422P15 = PresetVideoFormat.YUV422P15
+YUV422P16 = PresetVideoFormat.YUV422P16
+YUV422P17 = PresetVideoFormat.YUV422P17
+YUV422P18 = PresetVideoFormat.YUV422P18
+YUV422P19 = PresetVideoFormat.YUV422P19
+YUV422P20 = PresetVideoFormat.YUV422P20
+YUV422P21 = PresetVideoFormat.YUV422P21
+YUV422P22 = PresetVideoFormat.YUV422P22
+YUV422P23 = PresetVideoFormat.YUV422P23
+YUV422P24 = PresetVideoFormat.YUV422P24
+YUV422P25 = PresetVideoFormat.YUV422P25
+YUV422P26 = PresetVideoFormat.YUV422P26
+YUV422P27 = PresetVideoFormat.YUV422P27
+YUV422P28 = PresetVideoFormat.YUV422P28
+YUV422P29 = PresetVideoFormat.YUV422P29
+YUV422P30 = PresetVideoFormat.YUV422P30
+YUV422P31 = PresetVideoFormat.YUV422P31
+YUV422P32 = PresetVideoFormat.YUV422P32
+YUV422PH = PresetVideoFormat.YUV422PH
+YUV422PS = PresetVideoFormat.YUV422PS
+YUV411P8 = PresetVideoFormat.YUV411P8
+YUV411P9 = PresetVideoFormat.YUV411P9
+YUV411P10 = PresetVideoFormat.YUV411P10
+YUV411P11 = PresetVideoFormat.YUV411P11
+YUV411P12 = PresetVideoFormat.YUV411P12
+YUV411P13 = PresetVideoFormat.YUV411P13
+YUV411P14 = PresetVideoFormat.YUV411P14
+YUV411P15 = PresetVideoFormat.YUV411P15
+YUV411P16 = PresetVideoFormat.YUV411P16
+YUV411P17 = PresetVideoFormat.YUV411P17
+YUV411P18 = PresetVideoFormat.YUV411P18
+YUV411P19 = PresetVideoFormat.YUV411P19
+YUV411P20 = PresetVideoFormat.YUV411P20
+YUV411P21 = PresetVideoFormat.YUV411P21
+YUV411P22 = PresetVideoFormat.YUV411P22
+YUV411P23 = PresetVideoFormat.YUV411P23
+YUV411P24 = PresetVideoFormat.YUV411P24
+YUV411P25 = PresetVideoFormat.YUV411P25
+YUV411P26 = PresetVideoFormat.YUV411P26
+YUV411P27 = PresetVideoFormat.YUV411P27
+YUV411P28 = PresetVideoFormat.YUV411P28
+YUV411P29 = PresetVideoFormat.YUV411P29
+YUV411P30 = PresetVideoFormat.YUV411P30
+YUV411P31 = PresetVideoFormat.YUV411P31
+YUV411P32 = PresetVideoFormat.YUV411P32
+YUV411PH = PresetVideoFormat.YUV411PH
+YUV411PS = PresetVideoFormat.YUV411PS
+YUV440P8 = PresetVideoFormat.YUV440P8
+YUV440P9 = PresetVideoFormat.YUV440P9
+YUV440P10 = PresetVideoFormat.YUV440P10
+YUV440P11 = PresetVideoFormat.YUV440P11
+YUV440P12 = PresetVideoFormat.YUV440P12
+YUV440P13 = PresetVideoFormat.YUV440P13
+YUV440P14 = PresetVideoFormat.YUV440P14
+YUV440P15 = PresetVideoFormat.YUV440P15
+YUV440P16 = PresetVideoFormat.YUV440P16
+YUV440P17 = PresetVideoFormat.YUV440P17
+YUV440P18 = PresetVideoFormat.YUV440P18
+YUV440P19 = PresetVideoFormat.YUV440P19
+YUV440P20 = PresetVideoFormat.YUV440P20
+YUV440P21 = PresetVideoFormat.YUV440P21
+YUV440P22 = PresetVideoFormat.YUV440P22
+YUV440P23 = PresetVideoFormat.YUV440P23
+YUV440P24 = PresetVideoFormat.YUV440P24
+YUV440P25 = PresetVideoFormat.YUV440P25
+YUV440P26 = PresetVideoFormat.YUV440P26
+YUV440P27 = PresetVideoFormat.YUV440P27
+YUV440P28 = PresetVideoFormat.YUV440P28
+YUV440P29 = PresetVideoFormat.YUV440P29
+YUV440P30 = PresetVideoFormat.YUV440P30
+YUV440P31 = PresetVideoFormat.YUV440P31
+YUV440P32 = PresetVideoFormat.YUV440P32
+YUV440PH = PresetVideoFormat.YUV440PH
+YUV440PS = PresetVideoFormat.YUV440PS
+YUV410P8 = PresetVideoFormat.YUV410P8
+YUV410P9 = PresetVideoFormat.YUV410P9
+YUV410P10 = PresetVideoFormat.YUV410P10
+YUV410P11 = PresetVideoFormat.YUV410P11
+YUV410P12 = PresetVideoFormat.YUV410P12
+YUV410P13 = PresetVideoFormat.YUV410P13
+YUV410P14 = PresetVideoFormat.YUV410P14
+YUV410P15 = PresetVideoFormat.YUV410P15
+YUV410P16 = PresetVideoFormat.YUV410P16
+YUV410P17 = PresetVideoFormat.YUV410P17
+YUV410P18 = PresetVideoFormat.YUV410P18
+YUV410P19 = PresetVideoFormat.YUV410P19
+YUV410P20 = PresetVideoFormat.YUV410P20
+YUV410P21 = PresetVideoFormat.YUV410P21
+YUV410P22 = PresetVideoFormat.YUV410P22
+YUV410P23 = PresetVideoFormat.YUV410P23
+YUV410P24 = PresetVideoFormat.YUV410P24
+YUV410P25 = PresetVideoFormat.YUV410P25
+YUV410P26 = PresetVideoFormat.YUV410P26
+YUV410P27 = PresetVideoFormat.YUV410P27
+YUV410P28 = PresetVideoFormat.YUV410P28
+YUV410P29 = PresetVideoFormat.YUV410P29
+YUV410P30 = PresetVideoFormat.YUV410P30
+YUV410P31 = PresetVideoFormat.YUV410P31
+YUV410P32 = PresetVideoFormat.YUV410P32
+YUV410PH = PresetVideoFormat.YUV410PH
+YUV410PS = PresetVideoFormat.YUV410PS
+RGB24 = PresetVideoFormat.RGB24
+RGB27 = PresetVideoFormat.RGB27
+RGB30 = PresetVideoFormat.RGB30
+RGB33 = PresetVideoFormat.RGB33
+RGB36 = PresetVideoFormat.RGB36
+RGB39 = PresetVideoFormat.RGB39
+RGB42 = PresetVideoFormat.RGB42
+RGB45 = PresetVideoFormat.RGB45
+RGB48 = PresetVideoFormat.RGB48
+RGB51 = PresetVideoFormat.RGB51
+RGB54 = PresetVideoFormat.RGB54
+RGB57 = PresetVideoFormat.RGB57
+RGB60 = PresetVideoFormat.RGB60
+RGB63 = PresetVideoFormat.RGB63
+RGB66 = PresetVideoFormat.RGB66
+RGB69 = PresetVideoFormat.RGB69
+RGB72 = PresetVideoFormat.RGB72
+RGB75 = PresetVideoFormat.RGB75
+RGB78 = PresetVideoFormat.RGB78
+RGB81 = PresetVideoFormat.RGB81
+RGB84 = PresetVideoFormat.RGB84
+RGB87 = PresetVideoFormat.RGB87
+RGB90 = PresetVideoFormat.RGB90
+RGB93 = PresetVideoFormat.RGB93
+RGB96 = PresetVideoFormat.RGB96
+RGBH = PresetVideoFormat.RGBH
+RGBS = PresetVideoFormat.RGBS
```

### Comparing `vstools-2.1.0/vstools/utils/vs_proxy.py` & `vstools-2.2.0/vstools/utils/vs_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,19 @@
     STEREO_RIGHT, SURROUND_DIRECT_LEFT, SURROUND_DIRECT_RIGHT, TOP_BACK_CENTER, TOP_BACK_LEFT, TOP_BACK_RIGHT,
     TOP_CENTER, TOP_FRONT_CENTER, TOP_FRONT_LEFT, TOP_FRONT_RIGHT, TRANSFER_ARIB_B67, TRANSFER_BT470_BG,
     TRANSFER_BT470_M, TRANSFER_BT601, TRANSFER_BT709, TRANSFER_BT2020_10, TRANSFER_BT2020_12, TRANSFER_IEC_61966_2_1,
     TRANSFER_IEC_61966_2_4, TRANSFER_LINEAR, TRANSFER_LOG_100, TRANSFER_LOG_316, TRANSFER_ST240_M, TRANSFER_ST2084,
     TRANSFER_UNSPECIFIED, UNDEFINED, VIDEO, WIDE_LEFT, WIDE_RIGHT, YUV, AudioChannels, AudioFrame, AudioNode,
     ChromaLocation, ColorFamily, ColorPrimaries, ColorRange, Core, CoreCreationFlags, Environment, EnvironmentData,
     EnvironmentPolicy, EnvironmentPolicyAPI, Error, FieldBased, FilterMode, FrameProps, FramePtr, Func, FuncData,
-    Function, LogHandle, MatrixCoefficients, MediaType, MessageType, Plugin
-)
-from vapoursynth import PresetFormat as VSPresetFormat
-from vapoursynth import (
-    RawFrame, RawNode, SampleType, TransferCharacteristics, VideoFormat, VideoFrame, VideoNode, VideoOutputTuple,
-    __api_version__, __version__, _CoreProxy, ccfDisableAutoLoading, ccfDisableLibraryUnloading,
-    ccfEnableGraphInspection, clear_output, clear_outputs, fmFrameState, fmParallel, fmParallelRequests, fmUnordered,
-    get_current_environment, get_output, get_outputs, has_policy, register_policy
+    Function, LogHandle, MatrixCoefficients, MediaType, MessageType, Plugin, RawFrame, RawNode, SampleType,
+    TransferCharacteristics, VideoFormat, VideoFrame, VideoNode, VideoOutputTuple, __api_version__, __version__,
+    _CoreProxy, ccfDisableAutoLoading, ccfDisableLibraryUnloading, ccfEnableGraphInspection, clear_output,
+    clear_outputs, fmFrameState, fmParallel, fmParallelRequests, fmUnordered, get_current_environment, get_output,
+    get_outputs, has_policy, register_policy
 )
 
 from ..exceptions import CustomRuntimeError
 from .other import IS_DOCS
 from .vs_enums import (
     GRAY8, GRAY9, GRAY10, GRAY11, GRAY12, GRAY13, GRAY14, GRAY15, GRAY16, GRAY17, GRAY18, GRAY19, GRAY20, GRAY21,
     GRAY22, GRAY23, GRAY24, GRAY25, GRAY26, GRAY27, GRAY28, GRAY29, GRAY30, GRAY31, GRAY32, GRAYH, GRAYS, RGB24, RGB27,
@@ -59,15 +56,15 @@
     YUV422P15, YUV422P16, YUV422P17, YUV422P18, YUV422P19, YUV422P20, YUV422P21, YUV422P22, YUV422P23, YUV422P24,
     YUV422P25, YUV422P26, YUV422P27, YUV422P28, YUV422P29, YUV422P30, YUV422P31, YUV422P32, YUV422PH, YUV422PS,
     YUV440P8, YUV440P9, YUV440P10, YUV440P11, YUV440P12, YUV440P13, YUV440P14, YUV440P15, YUV440P16, YUV440P17,
     YUV440P18, YUV440P19, YUV440P20, YUV440P21, YUV440P22, YUV440P23, YUV440P24, YUV440P25, YUV440P26, YUV440P27,
     YUV440P28, YUV440P29, YUV440P30, YUV440P31, YUV440P32, YUV440PH, YUV440PS, YUV444P8, YUV444P9, YUV444P10, YUV444P11,
     YUV444P12, YUV444P13, YUV444P14, YUV444P15, YUV444P16, YUV444P17, YUV444P18, YUV444P19, YUV444P20, YUV444P21,
     YUV444P22, YUV444P23, YUV444P24, YUV444P25, YUV444P26, YUV444P27, YUV444P28, YUV444P29, YUV444P30, YUV444P31,
-    YUV444P32, YUV444PH, YUV444PS, PresetFormat
+    YUV444P32, YUV444PH, YUV444PS, PresetFormat, PresetVideoFormat, VSPresetVideoFormat
 )
 
 __all__ = [
     'AUDIO', 'AudioChannels', 'AudioFrame', 'AudioNode', 'BACK_CENTER', 'BACK_LEFT', 'BACK_RIGHT', 'CHROMA_BOTTOM',
     'CHROMA_BOTTOM_LEFT', 'CHROMA_CENTER', 'CHROMA_LEFT', 'CHROMA_TOP', 'CHROMA_TOP_LEFT', 'CallbackData',
     'ChromaLocation', 'ColorFamily', 'ColorPrimaries', 'ColorRange', 'Core', 'CoreCreationFlags', 'Environment',
     'EnvironmentData', 'EnvironmentPolicy', 'EnvironmentPolicyAPI', 'Error', 'FIELD_BOTTOM', 'FIELD_PROGRESSIVE',
@@ -78,15 +75,16 @@
     'GRAY9', 'GRAYH', 'GRAYS', 'INTEGER', 'LOW_FREQUENCY', 'LOW_FREQUENCY2', 'LogHandle', 'MATRIX_BT2020_CL',
     'MATRIX_BT2020_NCL', 'MATRIX_BT470_BG', 'MATRIX_BT709', 'MATRIX_CHROMATICITY_DERIVED_CL',
     'MATRIX_CHROMATICITY_DERIVED_NCL', 'MATRIX_FCC', 'MATRIX_ICTCP', 'MATRIX_RGB', 'MATRIX_ST170_M',
     'MATRIX_UNSPECIFIED', 'MATRIX_YCGCO', 'MESSAGE_TYPE_CRITICAL', 'MESSAGE_TYPE_DEBUG', 'MESSAGE_TYPE_FATAL',
     'MESSAGE_TYPE_INFORMATION', 'MESSAGE_TYPE_WARNING', 'MatrixCoefficients', 'MediaType', 'MessageType', 'NONE',
     'PRIMARIES_BT2020', 'PRIMARIES_BT470_BG', 'PRIMARIES_BT470_M', 'PRIMARIES_BT709', 'PRIMARIES_EBU3213_E',
     'PRIMARIES_FILM', 'PRIMARIES_ST170_M', 'PRIMARIES_ST240_M', 'PRIMARIES_ST428', 'PRIMARIES_ST431_2',
-    'PRIMARIES_ST432_1', 'PRIMARIES_UNSPECIFIED', 'Plugin', 'PresetFormat', 'PythonVSScriptLoggingBridge', 'RANGE_FULL',
+    'PRIMARIES_ST432_1', 'PRIMARIES_UNSPECIFIED', 'Plugin', 'PresetFormat', 'PresetVideoFormat',
+    'PythonVSScriptLoggingBridge', 'RANGE_FULL',
     'RANGE_LIMITED', 'RGB', 'RGB24', 'RGB27', 'RGB30', 'RGB33', 'RGB36', 'RGB39', 'RGB42', 'RGB45', 'RGB48', 'RGB51',
     'RGB54', 'RGB57', 'RGB60', 'RGB63', 'RGB66', 'RGB69', 'RGB72', 'RGB75', 'RGB78', 'RGB81', 'RGB84', 'RGB87', 'RGB90',
     'RGB93', 'RGB96', 'RGBH', 'RGBS', 'RawFrame', 'RawNode', 'SIDE_LEFT', 'SIDE_RIGHT', 'STEREO_LEFT', 'STEREO_RIGHT',
     'SURROUND_DIRECT_LEFT', 'SURROUND_DIRECT_RIGHT', 'SampleType', 'StandaloneEnvironmentPolicy', 'TOP_BACK_CENTER',
     'TOP_BACK_LEFT', 'TOP_BACK_RIGHT', 'TOP_CENTER', 'TOP_FRONT_CENTER', 'TOP_FRONT_LEFT', 'TOP_FRONT_RIGHT',
     'TRANSFER_ARIB_B67', 'TRANSFER_BT2020_10', 'TRANSFER_BT2020_12', 'TRANSFER_BT470_BG', 'TRANSFER_BT470_M',
     'TRANSFER_BT601', 'TRANSFER_BT709', 'TRANSFER_IEC_61966_2_1', 'TRANSFER_IEC_61966_2_4', 'TRANSFER_LINEAR',
@@ -112,15 +110,15 @@
     'YUV444P22', 'YUV444P23', 'YUV444P24', 'YUV444P25', 'YUV444P26', 'YUV444P27', 'YUV444P28', 'YUV444P29', 'YUV444P30',
     'YUV444P31', 'YUV444P32', 'YUV444P8', 'YUV444P9', 'YUV444PH', 'YUV444PS', '_CoreProxy', '__all__',
     '__api_version__', '__version__', 'ccfDisableAutoLoading', 'ccfDisableLibraryUnloading',
     'ccfEnableGraphInspection', 'clear_output', 'clear_outputs', 'construct_parameter', 'construct_signature',
     'construct_type', 'core', 'fmFrameState', 'fmParallel', 'fmParallelRequests', 'fmUnordered',
     'get_current_environment', 'get_output', 'get_outputs', 'has_policy', 'pyx_capi', 'register_on_creation',
     'register_on_destroy', 'register_policy', 'try_enable_introspection', 'unregister_on_creation',
-    'unregister_on_destroy', 'vs_file'
+    'unregister_on_destroy', 'vs_file', 'clear_cache'
 ]
 
 if IS_DOCS:
     register_on_destroy_poly = True
 else:
     register_on_destroy_poly = __version__.release_major < 61
 
@@ -132,15 +130,20 @@
 
     import __main__
 
     if not hasattr(__main__, '__file__') and '__vapoursynth__' not in sys.modules:
         first_stack = inspect.stack()[-1]
 
         sys.modules['__vapoursynth__'] = ModuleType('__vapoursynth__')
-        sys.modules['__vapoursynth__'].__file__ = str((Path.cwd() / first_stack.filename).resolve())
+
+        cope = (Path.cwd() / first_stack.filename).resolve()
+
+        sys.modules['__vapoursynth__'].__file__ = str(cope)
+
+        sys.path.append(str(cope.parent))
 
 
 if not register_on_destroy_poly:
     from vapoursynth import register_on_destroy, unregister_on_destroy
 else:
     def register_on_destroy(callback: Callable[..., None]) -> None:
         core.register_on_destroy(callback)
@@ -155,14 +158,30 @@
 
 
 def unregister_on_creation(callback: Callable[..., None]) -> None:
     """Unregister this callback from every core creation."""
     core_on_creation_callbacks.pop(id(callback), None)
 
 
+def clear_cache() -> None:
+    try:
+        cache_size = core.max_cache_size
+        core.max_cache_size = 1
+        try:
+            for output in list(get_outputs().values()):
+                if isinstance(output, VideoOutputTuple):
+                    output.clip.get_frame(0)
+                    break
+        except Exception:
+            core.std.BlankClip().get_frame(0)
+        core.max_cache_size = cache_size
+    except Exception:
+        ...
+
+
 if TYPE_CHECKING:
     class FunctionProxyBase(Function):
         ...
 
     class PluginProxyBase(Plugin):
         ...
 
@@ -261,15 +280,18 @@
 
 def vstools_isinstance(
     __obj: object, __class_or_tuple: type | UnionType | tuple[type | UnionType | tuple[Any, ...], ...]
 ) -> bool:
     if __class_or_tuple in (_CoreProxy, Core) and builtins_isinstance(__obj, CoreProxy):
         return True
 
-    if __class_or_tuple is VSPresetFormat and builtins_isinstance(__obj, PresetFormat):
+    if __class_or_tuple is VSPresetVideoFormat and (
+        builtins_isinstance(__obj, PresetVideoFormat)
+        or builtins_isinstance(__obj, PresetFormat)  # LEGACY SUPPORT, PresetFormat is DEPRECATED
+    ):
         return True
 
     return builtins_isinstance(__obj, __class_or_tuple)
 
 
 builtins.isinstance = vstools_isinstance
 
@@ -356,20 +378,23 @@
     return core
 
 
 class VSCoreProxy(CoreProxyBase):
     """Class for wrapping a VapourSynth core."""
 
     def __init__(self, core: Core | None = None) -> None:
-        self._own_core = core is not None
-        self._core = core and weakref.ref(core)
+        object.__setattr__(self, '_own_core', core is not None)
+        object.__setattr__(self, '_core', core and weakref.ref(core))
 
     def __getattr__(self, name: str) -> Plugin:
         return getattr(_get_core_with_cb(self), name)  # type: ignore
 
+    def __setattr__(self, name: str, value: Any) -> None:
+        return setattr(_get_core_with_cb(self), name, value)
+
     @property
     def core(self) -> Core:
         """The underlying VapourSynth Core instance."""
         return _get_core_with_cb(self)
 
     @property
     def proxied(self) -> CoreProxy:
```

### Comparing `vstools-2.1.0/vstools.egg-info/PKG-INFO` & `vstools-2.2.0/vstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstools
-Version: 2.1.0
+Version: 2.2.0
 Summary: Functions and utils related to VapourSynth
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-tools
 Project-URL: Documentation, https://vstools.encoding.moe/en/latest/
```

### Comparing `vstools-2.1.0/vstools.egg-info/SOURCES.txt` & `vstools-2.2.0/vstools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 vstools/types/builtins.py
 vstools/types/file.py
 vstools/types/funcs.py
 vstools/types/generic.py
 vstools/types/utils.py
 vstools/utils/__file_headers.json
 vstools/utils/__init__.py
+vstools/utils/cache.py
 vstools/utils/clips.py
 vstools/utils/colors.py
 vstools/utils/ffprobe.py
 vstools/utils/file.py
 vstools/utils/funcs.py
 vstools/utils/info.py
 vstools/utils/math.py
```

