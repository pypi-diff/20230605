# Comparing `tmp/vspreview-0.4.4.tar.gz` & `tmp/vspreview-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vspreview-0.4.4.tar", last modified: Fri May  5 14:43:20 2023, max compression
+gzip compressed data, was "vspreview-0.5.0.tar", last modified: Mon Jun  5 20:45:46 2023, max compression
```

## Comparing `vspreview-0.4.4.tar` & `vspreview-0.5.0.tar`

### file list

```diff
@@ -1,101 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 14:42:57.000000 vspreview-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-05 14:43:20.431944 vspreview-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 14:42:57.000000 vspreview-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 14:43:20.435944 vspreview-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-05 14:42:57.000000 vspreview-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.423944 vspreview-0.4.4/vspreview/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/api/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/timecodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/core/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/core/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/combobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/dragnavigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/edits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/graphicsview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/notch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    21321 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/vsenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/main/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/generalmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/picture_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/scening.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/benchmark/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9279 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/benchmark/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/comp/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/comp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/comp/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20360 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/comp/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/debug/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/debug/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/debug/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/main/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/main/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/main/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/misc/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/misc/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/pipette/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/pipette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/pipette/colorview.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/pipette/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/pipette/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/playback/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/playback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/playback/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    24853 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/playback/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/scening/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/scening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/scening/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/scening/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    35883 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/scening/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.423944 vspreview-0.4.4/vspreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:43:12.000000 vspreview-0.4.4/vspreview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 20:45:25.000000 vspreview-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-05 20:45:46.920426 vspreview-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-05 20:45:25.000000 vspreview-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-05 20:45:46.920426 vspreview-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-05 20:45:25.000000 vspreview-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.912425 vspreview-0.5.0/vspreview/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.912425 vspreview-0.5.0/vspreview/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/timecodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.912425 vspreview-0.5.0/vspreview/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/core/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/combobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/dragnavigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/edits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/graphicsview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/notch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20976 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/vsenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31704 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/models/generalmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/models/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/models/scening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/plugins/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/plugins/frame_props.ppy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/toolbars/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/benchmark/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/benchmark/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/toolbars/comp/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/comp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/comp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30642 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/comp/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/debug/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/debug/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/main/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/misc/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/misc/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/pipette/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/pipette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/pipette/colorview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/pipette/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/pipette/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/playback/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/playback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/playback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24853 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/playback/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/scening/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/scening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/scening/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/scening/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35998 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/scening/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.912425 vspreview-0.5.0/vspreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:45:39.000000 vspreview-0.5.0/vspreview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/top_level.txt
```

### Comparing `vspreview-0.4.4/LICENSE` & `vspreview-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/PKG-INFO` & `vspreview-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.4.4
+Version: 0.5.0
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
@@ -27,15 +27,15 @@
 
 This program is meant to be paired with a code editor with integrated terminal like Visual Studio Code.
 
 # Prerequisites
 
 1. [Python](https://www.Python.org/downloads) (3.10+ required)
     * Make sure to install Python to your `PATH`.
-1. [Vapoursynth](https://github.com/vapoursynth/vapoursynth/releases) (R59+ required)
+1. [VapourSynth](https://github.com/vapoursynth/vapoursynth/releases) (R60+ required)
 
 # Installation
 
 Install latest stable via pypi:
 ```bash
 pip install vspreview
 ```
@@ -46,15 +46,16 @@
 pip install -U git+https://github.com/Irrational-Encoding-Wizardry/vs-preview.git
 ```
 
 # Usage
 
 It can be used by running `vspreview script.vpy` or your preferred way in [your IDE](#ide-integration).
 
-[Keyboard Shortcuts](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/shortcuts.md)
+[Keyboard Shortcuts](https://github.com/Irrational-Encoding-Wizardry/vs-preview/blob/master/docs/accessibility/keybinds.rst)
 
 [Saved Frame Filename Variables](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/save_frame_placeholders.md)
 
 # IDE Integration
 
-* [VSCode](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/vscode_install.md)
-* [Vim](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/vim_install.md)
+* [Visual Studio Code](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/installation/install_vscode.rst)
+* [Vim](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/installation/install_vim.rst)
+* [Notepad++](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/installation/install_notepad++.rst)
```

### Comparing `vspreview-0.4.4/README.md` & `vspreview-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This program is meant to be paired with a code editor with integrated terminal like Visual Studio Code.
 
 # Prerequisites
 
 1. [Python](https://www.Python.org/downloads) (3.10+ required)
     * Make sure to install Python to your `PATH`.
-1. [Vapoursynth](https://github.com/vapoursynth/vapoursynth/releases) (R59+ required)
+1. [VapourSynth](https://github.com/vapoursynth/vapoursynth/releases) (R60+ required)
 
 # Installation
 
 Install latest stable via pypi:
 ```bash
 pip install vspreview
 ```
@@ -23,15 +23,16 @@
 pip install -U git+https://github.com/Irrational-Encoding-Wizardry/vs-preview.git
 ```
 
 # Usage
 
 It can be used by running `vspreview script.vpy` or your preferred way in [your IDE](#ide-integration).
 
-[Keyboard Shortcuts](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/shortcuts.md)
+[Keyboard Shortcuts](https://github.com/Irrational-Encoding-Wizardry/vs-preview/blob/master/docs/accessibility/keybinds.rst)
 
 [Saved Frame Filename Variables](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/save_frame_placeholders.md)
 
 # IDE Integration
 
-* [VSCode](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/vscode_install.md)
-* [Vim](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/vim_install.md)
+* [Visual Studio Code](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/installation/install_vscode.rst)
+* [Vim](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/installation/install_vim.rst)
+* [Notepad++](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/installation/install_notepad++.rst)
```

### Comparing `vspreview-0.4.4/setup.cfg` & `vspreview-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/setup.py` & `vspreview-0.5.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,24 +28,35 @@
         'Tracker': 'https://github.com/Irrational-Encoding-Wizardry/vs-preview/issues',
         'Contact': 'https://discord.gg/qxTxVJGtst'
     },
     install_requires=requirements,
     python_requires='>=3.10',
     packages=setuptools.find_packages('.', ('docs', 'stubs')),
     package_data={
-        package_name: ['py.typed']
+        package_name: ['py.typed'],
+        f'{package_name}.plugins': [
+            file.name for file in (Path(package_name) / 'plugins').glob('*.ppy')
+        ]
     },
     classifiers=[
         'Topic :: Multimedia :: Graphics',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
     entry_points={
         'console_scripts': [
             'vspreview = vspreview.init:main'
         ]
+    },
+    command_options={
+        "build_sphinx": {
+            "project": ("setup.py", package_name),
+            "version": ("setup.py", meta['__version__']),
+            "release": ("setup.py", meta['__version__']),
+            "source_dir": ("setup.py", "docs")
+        }
     }
 )
```

### Comparing `vspreview-0.4.4/vspreview/api/other.py` & `vspreview-0.5.0/vspreview/api/other.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         with open(launch, 'w') as f:
             json.dump(current_settings, f, indent=4)
         return
 
     if mode != 'append':
         return _write()
 
-    with open(launch, 'r+') as f:
+    with open(launch, 'r+', encoding='utf-8') as f:
         try:
             current_settings = json.loads(f.read())
         except json.JSONDecodeError:
             current_settings = {}
 
     if 'configurations' not in current_settings or len(current_settings['configurations']) == 0:
         current_settings['configurations'] = settings['configurations']
```

### Comparing `vspreview-0.4.4/vspreview/api/output.py` & `vspreview-0.5.0/vspreview/api/output.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/abstracts.py` & `vspreview-0.5.0/vspreview/core/abstracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 __all__ = [
     'HBoxLayout', 'VBoxLayout',
 
     'SpinBox', 'PushButton', 'LineEdit', 'CheckBox', 'Timer', 'ProgressBar', 'DoubleSpinBox',
 
     'AbstractQItem', 'AbstractYAMLObject',
 
-    'ExtendedWidget', 'ExtendedDialog', 'ExtendedTableView',
+    'ExtendedWidgetBase', 'ExtendedWidget', 'ExtendedDialog', 'ExtendedTableView',
 
-    'AbstractToolbar', 'AbstractToolbarSettings',
+    'NotchProvider', 'AbstractToolbar', 'AbstractToolbarSettings',
 
     'main_window', 'storage_err_msg', 'try_load',
 ]
 
 
 class ExtendedLayout(QBoxLayout):
     @overload
@@ -286,15 +286,15 @@
 
 class AbstractYAMLObject(AbstractQItem):
     @abstractmethod
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         raise NotImplementedError
 
 
-class ExtendedWidget(AbstractQItem, QWidget):
+class ExtendedWidgetBase(AbstractQItem):
     vlayout: VBoxLayout
     hlayout: HBoxLayout
 
     def setup_ui(self) -> None:
         self.vlayout = VBoxLayout(self)
         self.hlayout = HBoxLayout(self.vlayout)
 
@@ -304,31 +304,40 @@
     def get_separator(self) -> QFrame:
         separator = QFrame(self)
         separator.setFrameShape(QFrame.Shape.VLine)
         separator.setFrameShadow(QFrame.Shadow.Sunken)
         return separator
 
 
+class ExtendedWidget(ExtendedWidgetBase, QWidget):
+    ...
+
+
 class ExtendedDialog(AbstractQItem, QDialog):
     ...
 
 
 class ExtendedTableView(AbstractQItem, QTableView):
     ...
 
 
 class AbstractToolbarSettings(ExtendedWidget, QYAMLObjectSingleton):
     __slots__ = ()
 
+    _add_to_tab = True
+
     def __init__(self, parent: type[AbstractToolbar] | AbstractToolbar) -> None:
         super().__init__()
 
         self.parent_toolbar_type = parent if isinstance(parent, type) else parent.__class__
 
         self.setup_ui()
+
+        self.vlayout.addStretch(1)
+
         self.set_defaults()
 
         self.set_qobject_names()
 
     def set_defaults(self) -> None:
         pass
 
@@ -344,27 +353,41 @@
 
             try:
                 super().__setstate__(state)  # type: ignore
             except AttributeError:
                 ...
 
 
-class AbstractToolbar(ExtendedWidget, QWidget, QABC):
+class NotchProvider(QABC):
+    notches_changed = pyqtSignal(ExtendedWidget)
+
+    def init_notches(self, main: MainWindow = ...) -> None:
+        self.notches_changed.connect(main.timeline.update_notches)
+
+    def get_notches(self) -> Notches:
+        from .custom import Notches
+        return Notches()
+
+    @property
+    @abstractmethod
+    def is_notches_visible(self) -> bool:
+        ...
+
+
+class AbstractToolbar(ExtendedWidget, NotchProvider):
     _no_visibility_choice = False
     storable_attrs = tuple[str, ...]()
     class_storable_attrs = tuple[str, ...](('settings', 'visibility'))
     num_keys = [
         Qt.Key.Key_1, Qt.Key.Key_2, Qt.Key.Key_3, Qt.Key.Key_4, Qt.Key.Key_5, Qt.Key.Key_6,
         Qt.Key.Key_7, Qt.Key.Key_8, Qt.Key.Key_9, Qt.Key.Key_0
     ]
 
     __slots__ = ('main', 'toggle_button', *class_storable_attrs)
 
-    notches_changed = pyqtSignal(ExtendedWidget)
-
     main: MainWindow
     name: str
 
     def __init__(self, main: MainWindow, settings: QWidget | None = None) -> None:
         super().__init__(main.central_widget)
 
         if settings is None:
@@ -372,27 +395,28 @@
 
             raise CustomValueError('Missing settings widget!')
 
         self.main = main
         self.settings = settings
         self.name = self.__class__.__name__[:-7]
 
-        self.main.app_settings.addTab(settings, self.name)
+        if settings._add_to_tab:
+            self.main.app_settings.addTab(settings, self.name)
         self.setFocusPolicy(Qt.FocusPolicy.ClickFocus)
 
-        self.notches_changed.connect(self.main.timeline.update_notches)
-
         self.toggle_button = PushButton(
             self.name, self, checkable=True, clicked=self.on_toggle
         )
         self.toggle_button.setVisible(not self._no_visibility_choice)
 
         self.setVisible(False)
         self.visibility = False
 
+        self.init_notches(self.main)
+
     def setup_ui(self) -> None:
         self.hlayout = HBoxLayout(self)
         self.vlayout = VBoxLayout(self.hlayout)
 
         self.hlayout.setContentsMargins(0, 0, 0, 0)
 
     def on_toggle(self, new_state: bool) -> None:
@@ -407,20 +431,17 @@
 
     def on_current_frame_changed(self, frame: Frame) -> None:
         pass
 
     def on_current_output_changed(self, index: int, prev_index: int) -> None:
         pass
 
-    def get_notches(self) -> Notches:
-        from .custom import Notches
-        return Notches()
-
+    @property
     def is_notches_visible(self) -> bool:
-        return self.isVisible()
+        return self.visibility
 
     def resize_main_window(self, expanding: bool) -> None:
         if self.main.windowState() in {Qt.WindowState.WindowMaximized, Qt.WindowState.WindowFullScreen}:
             return
 
         if expanding:
             self.main.resize(self.main.width(), self.main.height() + self.height() + round(6 * self.main.display_scale))
```

### Comparing `vspreview-0.4.4/vspreview/core/bases.py` & `vspreview-0.5.0/vspreview/core/bases.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/custom/combobox.py` & `vspreview-0.5.0/vspreview/core/custom/combobox.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/custom/dragnavigator.py` & `vspreview-0.5.0/vspreview/core/custom/dragnavigator.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,19 +90,16 @@
         self.repaint()
 
     def repaint_timeout(self) -> None:
         self.hide()
         self.repaint_timer.stop()
 
     def paintEvent(self, event: QPaintEvent) -> None:
-        if (
-            (self.contentsW == 0) or (self.contentsH == 0)
-            or (self.viewportW == 0) or (self.viewportH == 0)
-            or (self.viewportX >= self.contentsW) or (self.viewportY >= self.contentsH)
-        ):
+        if (self.contentsW == 0) or (self.contentsH == 0) or (self.viewportW == 0) or \
+                (self.viewportH == 0) or (self.viewportX >= self.contentsW) or (self.viewportY >= self.contentsH):
             event.ignore()
             return
 
         norm = 100.0 / max(self.contentsW, self.contentsH, self.viewportW, self.viewportH)
 
         normContentsWidth, normContentsHeight = round(self.contentsW * norm), round(self.contentsH * norm)
         normViewportWidth, normViewportHeight = round(self.viewportW * norm), round(self.viewportH * norm)
```

### Comparing `vspreview-0.4.4/vspreview/core/custom/edits.py` & `vspreview-0.5.0/vspreview/core/custom/edits.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/custom/graphicsview.py` & `vspreview-0.5.0/vspreview/core/custom/graphicsview.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/custom/misc.py` & `vspreview-0.5.0/vspreview/core/custom/misc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 from typing import Any, Sequence, cast
 
-from PyQt6.QtCore import QRect, Qt
+from PyQt6.QtCore import QAbstractTableModel, QModelIndex, QRect, Qt
 from PyQt6.QtGui import QBrush, QColor, QPainter, QPaintEvent, QPen
 from PyQt6.QtWidgets import QLabel, QStatusBar, QWidget
 
 from ..abstracts import PushButton
 
 __all__ = [
     'StatusBar',
-    'Switch'
+    'Switch',
+    'TableModel'
 ]
 
 
 class StatusBar(QStatusBar):
     label_names = (
         'total_frames_label', 'duration_label', 'resolution_label',
         'pixel_format_label', 'fps_label', 'frame_props_label', 'label'
@@ -98,7 +99,39 @@
         painter.drawRoundedRect(switch_rect, self.radius, self.radius)
 
         textpen = QPen(self.text_color)
         textpen.setWidth(self.state_texts[2])
 
         painter.setPen(textpen)
         painter.drawText(switch_rect, Qt.AlignmentFlag.AlignCenter, cast(str, self.state_texts[int(self.isChecked())]))
+
+
+class TableModel(QAbstractTableModel):
+    def __init__(self, data: list[list[Any]] = [], columns: list[Any] | bool = True, rows: bool = True) -> None:
+        super().__init__()
+
+        self._data = data
+        self._columns = columns
+        self._rows = rows
+
+    def data(self, index: QModelIndex, role: int) -> Any:
+        if role == Qt.ItemDataRole.DisplayRole:
+            return self._data[index.row()][index.column()]
+
+    def rowCount(self, index: QModelIndex) -> int:
+        return len(self._data)
+
+    def columnCount(self, index: QModelIndex) -> int:
+        return len(self._data) and len(self._data[0])
+
+    def headerData(self, section, orientation, role):
+        if role == Qt.DisplayRole:
+            if orientation == Qt.Horizontal:
+                if isinstance(self._columns, bool):
+                    if self._columns:
+                        return super().headerData(section, orientation, role)
+                else:
+                    return str(self._columns[section])
+
+            if orientation == Qt.Vertical:
+                if self._rows:
+                    return super().headerData(section, orientation, role)
```

### Comparing `vspreview-0.4.4/vspreview/core/logger.py` & `vspreview-0.5.0/vspreview/core/logger.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/types/audio.py` & `vspreview-0.5.0/vspreview/core/types/audio.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/types/scene.py` & `vspreview-0.5.0/vspreview/core/types/scene.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/types/units.py` & `vspreview-0.5.0/vspreview/core/types/units.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/types/video.py` & `vspreview-0.5.0/vspreview/core/types/video.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 
 from fractions import Fraction
 from itertools import count as iter_count
-from typing import Any, Mapping, cast
+from typing import TYPE_CHECKING, Any, Mapping, cast
 
 import vapoursynth as vs
 from PyQt6 import sip
 from PyQt6.QtCore import Qt
 from PyQt6.QtGui import QColorSpace, QImage, QPainter, QPixmap
 
 from ..abstracts import AbstractYAMLObject, main_window, try_load
 from .misc import CroppingInfo, VideoOutputNode
 from .units import Frame, Time
 
+if TYPE_CHECKING:
+    from vstools import VideoFormatT
+
 __all__ = [
     'VideoOutput'
 ]
 
 
 class PackingTypeInfo:
     _getid = iter_count()
 
     def __init__(
-        self, vs_format: vs.PresetFormat | vs.VideoFormat, qt_format: QImage.Format, shuffle: bool,
+        self, vs_format: VideoFormatT, qt_format: QImage.Format, shuffle: bool,
         can_playback: bool = True
     ):
         self.id = next(self._getid)
         self.vs_format = vs.core.get_video_format(vs_format)
         self.qt_format = qt_format
         self.shuffle = shuffle
         self.can_playback = can_playback
@@ -235,25 +238,14 @@
         else:
             try:
                 import numpy  # noqa: F401
                 PACKING_TYPE = PackingType.numpy_10bit if _default_10bits else PackingType.numpy_8bit
             except ModuleNotFoundError:
                 PACKING_TYPE = PackingType.none_10bit if _default_10bits else PackingType.none_8bit
 
-                print(ImportWarning(
-                    "\n"
-                    "  One of LibP2P, Akarin, cupy, numpy is required to pack RGB data efficiently for previewing!\n"
-                    "  Now falling back to pure python. You won't be able to playback.\n"
-                    "  You can download one of them from here: \n"
-                    "      https://github.com/DJATOM/LibP2P-Vapoursynth\n"
-                    "      https://github.com/AkarinVS/vapoursynth-plugin\n"
-                    "      https://docs.cupy.dev/en/stable/install.html#installing-cupy\n"
-                    "      pip install numpy\n"
-                ))
-
         self.set_fmt_values()
 
     @property
     def name(self) -> str:
         placeholder = 'Video Node %d' % self.index
         if not hasattr(self, 'title') or self.title in {None, placeholder}:
             if 'Name' in self.props:
@@ -408,21 +400,31 @@
         )
 
         return QImage(pointer, width, height, stride, qt_format).copy()  # type: ignore
 
     def update_graphic_item(
         self, pixmap: QPixmap | None = None, crop_values: CroppingInfo | None | bool = None
     ) -> QPixmap | None:
+        from vstools import complex_hash
+
+        old_crop = complex_hash.hash(self.crop_values)
+
         if isinstance(crop_values, bool):
             self.crop_values.active = crop_values
         elif crop_values is not None:
             self.crop_values = crop_values
 
+        new_crop = complex_hash.hash(self.crop_values)
+
         if hasattr(self, 'graphics_scene_item'):
             self.graphics_scene_item.setPixmap(pixmap, self.crop_values)
+
+        if old_crop != new_crop:
+            self.main.cropValuesChanged.emit(self.crop_values)
+
         return pixmap
 
     def render_frame(
         self, frame: Frame | None, vs_frame: vs.VideoFrame | None = None,
         vs_alpha_frame: vs.VideoFrame | None = None, do_painting: bool = True,
         output_colorspace: QColorSpace | None = None
     ) -> QPixmap:
```

### Comparing `vspreview-0.4.4/vspreview/core/types/yaml.py` & `vspreview-0.5.0/vspreview/core/types/yaml.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/core/vsenv.py` & `vspreview-0.5.0/vspreview/core/vsenv.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/init.py` & `vspreview-0.5.0/vspreview/init.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/main/dialog.py` & `vspreview-0.5.0/vspreview/main/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class ScriptErrorDialog(ExtendedDialog):
     __slots__ = ('main', 'label', 'reload_button', 'exit_button')
 
     def __init__(self, main_window: MainWindow) -> None:
         super().__init__(main_window, Qt.WindowType.Dialog)
         self.main = main_window
 
-        self.setWindowTitle('Script Loading Error')
+        self.setWindowTitle('There was an error')
         self.setModal(True)
 
         self.setup_ui()
         self.setup_shortcuts()
 
         self.set_qobject_names()
```

### Comparing `vspreview-0.4.4/vspreview/main/settings.py` & `vspreview-0.5.0/vspreview/main/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import sys
 from functools import partial
 from multiprocessing import cpu_count
-from typing import Any, Mapping
+from typing import Any, Mapping, cast
 
 from PyQt6.QtCore import QKeyCombination, Qt
 from PyQt6.QtGui import QShortcut
 from PyQt6.QtWidgets import QComboBox, QLabel
 
 from ..core import (
     AbstractToolbarSettings, CheckBox, ComboBox, HBoxLayout, PushButton, QYAMLObjectSingleton, SpinBox, Time, TimeEdit,
@@ -311,28 +311,41 @@
         try_load(state, 'zoom_default_index', int, self.zoom_level_default_combobox.setCurrentIndex)
         try_load(state, 'dragnavigator_timeout', int, self.dragnavigator_timeout_spinbox.setValue)
         try_load(state, 'color_management', bool, self.color_management_checkbox.setChecked)
 
 
 class WindowSettings(QYAMLObjectSingleton):
     __slots__ = (
-        'timeline_mode', 'window_geometry', 'window_state'
+        'timeline_mode', 'window_geometry', 'window_state', 'zoom_index', 'x_pos', 'y_pos'
     )
 
-    def __init__(self, timeline_mode: str, window_geometry: bytes, window_state: bytes) -> None:
-        self.timeline_mode = timeline_mode
-        self.window_geometry = window_geometry
-        self.window_state = window_state
-
-        super().__init__()
-
     def __getstate__(self) -> Mapping[str, Any]:
+        main = main_window()
+
         return {
-            'timeline_mode': self.timeline_mode,
-            'window_geometry': self.window_geometry,
-            'window_state': self.window_state
+            'timeline_mode': main.timeline.mode,
+            'window_geometry': bytes(cast(bytearray, main.saveGeometry())),
+            'window_state': bytes(cast(bytearray, main.saveState())),
+            'zoom_index': main.toolbars.main.zoom_combobox.currentIndex(),
+            'x_pos': main.graphics_view.horizontalScrollBar().value(),
+            'y_pos': main.graphics_view.verticalScrollBar().value(),
         }
 
     def __setstate__(self, state: Mapping[str, Any]) -> None:
         try_load(state, 'timeline_mode', str, self.__setattr__)
         try_load(state, 'window_geometry', bytes, self.__setattr__)
         try_load(state, 'window_state', bytes, self.__setattr__)
+        try_load(state, 'zoom_index', int, self.__setattr__)
+        try_load(state, 'x_pos', int, self.__setattr__)
+        try_load(state, 'y_pos', int, self.__setattr__)
+
+        main = main_window()
+
+        main.timeline.mode = self.timeline_mode
+
+        main.toolbars.main.zoom_combobox.setCurrentIndex(self.zoom_index)
+
+        main.graphics_view.horizontalScrollBar().setValue(self.x_pos)
+        main.graphics_view.verticalScrollBar().setValue(self.y_pos)
+
+        main.restoreState(self.window_state)
+        main.restoreGeometry(self.window_geometry)
```

### Comparing `vspreview-0.4.4/vspreview/main/timeline.py` & `vspreview-0.5.0/vspreview/main/timeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from copy import deepcopy
 from typing import Any, cast
 
 from PyQt6.QtCore import QEvent, QLineF, QRectF, Qt, pyqtSignal
 from PyQt6.QtGui import QMouseEvent, QMoveEvent, QPainter, QPaintEvent, QPalette, QPen, QResizeEvent
 from PyQt6.QtWidgets import QApplication, QToolTip, QWidget
 
-from ..core import AbstractToolbar, AbstractYAMLObject, Frame, Notch, Notches, Time, VideoOutput, main_window
+from ..core import NotchProvider, AbstractYAMLObject, Frame, Notch, Notches, Time, VideoOutput, main_window
 from ..utils import strfdelta
 
 __all__ = [
     'Timeline'
 ]
 
 
@@ -64,15 +64,15 @@
         self.cursor_x = 0
         # used as a fallback when self.rectF.width() is 0,
         # so cursorX is incorrect
         self.cursor_ftx: Frame | Time | int | None = None
         # False means that only cursor position'll be recalculated
         self.need_full_repaint = True
 
-        self.toolbars_notches = dict[AbstractToolbar, Notches]()
+        self.notches = dict[NotchProvider, Notches]()
 
         self.setAttribute(Qt.WidgetAttribute.WA_OpaquePaintEvent)
         self.setMouseTracking(True)
 
     def paintEvent(self, event: QPaintEvent) -> None:
         super().paintEvent(event)
         self.rect_f = QRectF(event.rect())
@@ -117,16 +117,16 @@
 
             self.scroll_rect = QRectF(
                 self.rect_f.left(),
                 label_notch_bottom + self.notch_scroll_interval,
                 self.rect_f.width(), self.scroll_height
             )
 
-            for toolbar, notches in self.toolbars_notches.items():
-                if not toolbar.is_notches_visible():
+            for provider, notches in self.notches.items():
+                if not provider.is_notches_visible:
                     continue
 
                 for notch in notches:
                     if isinstance(notch.data, Frame):
                         x = self.f_to_x(notch.data)
                     elif isinstance(notch.data, Time):
                         x = self.t_to_x(notch.data)
@@ -178,16 +178,16 @@
                         anchor_rect, Qt.AlignmentFlag.AlignBottom | Qt.AlignmentFlag.AlignHCenter, label
                     )
                 painter.drawText(rect, label)
 
         painter.setRenderHint(QPainter.RenderHint.Antialiasing, False)
         painter.fillRect(self.scroll_rect, Qt.GlobalColor.gray)
 
-        for toolbar, notches in self.toolbars_notches.items():
-            if not toolbar.is_notches_visible():
+        for provider, notches in self.notches.items():
+            if not provider.is_notches_visible:
                 continue
 
             for notch in notches:
                 painter.setPen(notch.color)
                 painter.drawLine(notch.line)
 
         painter.setPen(Qt.GlobalColor.black)
@@ -208,16 +208,16 @@
         pos = event.pos().toPointF()
         if self.scroll_rect.contains(pos):
             self.set_position(int(pos.x()))
             self.clicked.emit(self.x_to_f(self.cursor_x, Frame), self.x_to_t(self.cursor_x, Time))
 
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
         super().mouseMoveEvent(event)
-        for toolbar, notches in self.toolbars_notches.items():
-            if not toolbar.is_notches_visible():
+        for provider, notches in self.notches.items():
+            if not provider.is_notches_visible:
                 continue
             for notch in notches:
                 line = notch.line
                 if line.x1() - 0.5 <= event.pos().x() <= line.x1() + 0.5:
                     QToolTip.showText(event.globalPosition().toPoint(), notch.label)
                     return
 
@@ -229,20 +229,22 @@
         if event.type() in {QEvent.Type.Polish, QEvent.Type.ApplicationPaletteChange}:
             self.setPalette(self.main.palette())
             self.full_repaint()
             return True
 
         return super().event(event)
 
-    def update_notches(self, toolbar: AbstractToolbar | None = None) -> None:
-        if toolbar is not None:
-            self.toolbars_notches[toolbar] = toolbar.get_notches()
-        if toolbar is None:
+    def update_notches(self, provider: NotchProvider | None = None) -> None:
+        if provider is not None:
+            self.notches[provider] = provider.get_notches()
+        else:
             for t in self.main.toolbars:
-                self.toolbars_notches[t] = t.get_notches()
+                self.notches[t] = t.get_notches()
+            for t in self.main.plugins:
+                self.notches[t] = t.get_notches()
         self.full_repaint()
 
     @property
     def mode(self) -> str:
         return self._mode
 
     @mode.setter
```

### Comparing `vspreview-0.4.4/vspreview/main/window.py` & `vspreview-0.5.0/vspreview/main/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 
 import io
 import logging
 import sys
 from fractions import Fraction
 from importlib import reload as reload_module
 from pathlib import Path
-from pkgutil import iter_modules
 from time import time
 from typing import Any, Iterable, Mapping, cast
 
 import vapoursynth as vs
-from PyQt6.QtCore import QByteArray, QEvent, QRectF, pyqtSignal
+from PyQt6 import QtCore
+from PyQt6.QtCore import QEvent, QRectF, pyqtSignal
 from PyQt6.QtGui import QCloseEvent, QColorSpace, QMoveEvent, QPalette, QPixmap, QShowEvent
 from PyQt6.QtOpenGLWidgets import QOpenGLWidget
-from PyQt6.QtWidgets import QApplication, QGraphicsScene, QGraphicsView, QLabel, QMainWindow, QSizePolicy
+from PyQt6.QtWidgets import (
+    QApplication, QGraphicsScene, QGraphicsView, QLabel, QMainWindow, QSizePolicy, QSplitter, QTabWidget
+)
 from vsengine import vpy  # type: ignore
 
 from ..core import (
-    PRELOADED_MODULES, AbstractQItem, DragNavigator, ExtendedWidget, Frame, GraphicsImageItem, GraphicsView,
-    QAbstractYAMLObjectSingleton, StatusBar, Time, Timer, VBoxLayout, VideoOutput, ViewMode, _monkey_runpy_dicts,
-    get_current_environment, make_environment, try_load
+    PRELOADED_MODULES, AbstractQItem, CroppingInfo, DragNavigator, ExtendedWidget, Frame, GraphicsImageItem,
+    GraphicsView, HBoxLayout, QAbstractYAMLObjectSingleton, StatusBar, Time, Timer, VBoxLayout, VideoOutput, ViewMode,
+    _monkey_runpy_dicts, get_current_environment, make_environment
 )
 from ..models import VideoOutputs
+from ..plugins import Plugins
 from ..toolbars import Toolbars
 from ..utils import fire_and_forget, set_status_label
 from .dialog import ScriptErrorDialog, SettingsDialog
 from .settings import MainSettings, WindowSettings
 from .timeline import Timeline
 
 if sys.platform == 'win32':
@@ -50,24 +53,45 @@
 from yaml import MarkedYAMLError, YAMLError
 
 __all__ = [
     'MainWindow'
 ]
 
 
+class CentralSplitter(QSplitter):
+    def __init__(self, main_window: MainWindow, orientation: QtCore.Qt.Orientation) -> None:
+        super().__init__(orientation)
+
+        self.main_window = main_window
+
+        self.splitterMoved.connect(self.on_splitter_moved)
+
+        self.previous_position = 0
+
+    @property
+    def current_position(self) -> int:
+        return self.sizes()[-1]
+
+    def on_splitter_moved(self) -> None:
+        if self.previous_position == 0 and self.current_position:
+            self.main_window.plugins.update()
+
+        self.previous_position = self.current_position
+
+
 class MainWindow(AbstractQItem, QMainWindow, QAbstractYAMLObjectSingleton):
     current_viewmode: ViewMode
 
     VSP_DIR_NAME = '.vspreview'
     VSP_GLOBAL_DIR_NAME = Path(
         expandvars('%APPDATA%') if sys.platform == "win32" else expanduser('~/.config')  # type: ignore
     )
 
-    VSP_VERSION = 3.1
-    BREAKING_CHANGES_VERSIONS = list[str](['3.0'])
+    VSP_VERSION = 3.2
+    BREAKING_CHANGES_VERSIONS = list[str](['3.0', '3.1'])
 
     # status bar
     def STATUS_FRAME_PROP(self, prop: Any) -> str:
         return 'Type: %s' % (prop['_PictType'].decode('utf-8') if '_PictType' in prop else '?')
 
     EVENT_POLICY = QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
 
@@ -81,45 +105,53 @@
         'current_storage_path', 'opengl_widget', 'drag_navigator'
     )
 
     # emit when about to reload a script: clear all existing references to existing clips.
     reload_signal = pyqtSignal()
     reload_before_signal = pyqtSignal()
     reload_after_signal = pyqtSignal()
+    cropValuesChanged = pyqtSignal(CroppingInfo)
 
     toolbars: Toolbars
+    plugins: Plugins
     app_settings: SettingsDialog
-    window_settings: WindowSettings
+    window_settings = WindowSettings()
 
     autosave_timer: Timer
 
     def __init__(self, config_dir: Path) -> None:
         from ..toolbars import MainToolbar
 
         super().__init__()
 
         self.settings = MainSettings(MainToolbar)
 
         self.current_config_dir = config_dir / self.VSP_DIR_NAME
         self.global_config_dir = self.VSP_GLOBAL_DIR_NAME / self.VSP_DIR_NAME
         self.global_storage_path = self.global_config_dir / '.global.yml'
+        self.global_plugins_dir = self.global_config_dir / 'plugins'
+        self.global_plugins_dir.mkdir(parents=True, exist_ok=True)
 
         self.app = cast(QApplication, QApplication.instance())
         assert self.app
 
         self.last_reload_time = time()
 
         if self.settings.dark_theme_enabled:
+            from ..core import apply_plotting_style
+
             try:
                 from qdarkstyle import _load_stylesheet  # type: ignore[import]
             except ImportError:
                 self.settings.dark_theme_enabled = False
             else:
+                apply_plotting_style()
                 self.app.setStyleSheet(self.patch_dark_stylesheet(_load_stylesheet(qt_api='pyqt6')))
-                self.ensurePolished()
+
+        self.ensurePolished()
 
         self.display_scale = self.app.primaryScreen().logicalDotsPerInch() / self.settings.base_ppi
         self.setWindowTitle('VSPreview')
 
         desktop_size = self.app.primaryScreen().size()
 
         self.move(int(desktop_size.width() * 0.15), int(desktop_size.height() * 0.075))
@@ -168,14 +200,16 @@
 
         Toolbars(self)
 
         for toolbar in self.toolbars:
             self.main_layout.addWidget(toolbar)
             self.toolbars.main.layout().addWidget(toolbar.toggle_button)
 
+        Plugins(self)
+
         self.app_settings.tab_widget.setUsesScrollButtons(False)
         self.app_settings.setMinimumWidth(
             int(len(self.toolbars) * 1.05 * self.app_settings.tab_widget.geometry().width() / 2)
         )
 
         self.current_viewmode = ViewMode.NORMAL
 
@@ -194,15 +228,26 @@
         self.graphics_view.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
         self.graphics_view.setDragMode(QGraphicsView.DragMode.ScrollHandDrag)
 
         self.drag_navigator = DragNavigator(self, self.graphics_view)
 
         self.timeline = Timeline(self.central_widget)
 
-        self.main_layout.addWidgets([self.graphics_view, self.timeline])
+        self.plugins_tab = QTabWidget(self.central_widget)
+        self.plugins_tab.currentChanged.connect(lambda x: self.plugins.update())
+
+        self.main_split = CentralSplitter(self, QtCore.Qt.Orientation.Horizontal)
+        self.main_split.addWidget(self.graphics_view)
+        self.main_split.addWidget(self.plugins_tab)
+        self.main_split.setSizePolicy(
+            QSizePolicy.Policy.Expanding, QSizePolicy.Policy.MinimumExpanding
+        )
+
+        HBoxLayout(self.main_layout, [self.main_split])
+        self.main_layout.addWidget(self.timeline)
 
         # status bar
         self.statusbar = StatusBar(self.central_widget)
 
         for name in self.statusbar.label_names:
             self.statusbar.__setattr__(name, QLabel(self.central_widget))
 
@@ -248,56 +293,59 @@
             pass
 
         try:
             if reloading:
                 std_path_lib = Path(logging.__file__).parent.parent
                 std_path_dlls = std_path_lib.parent / 'DLLs'
 
+                check_reloaded = set[str]()
+
                 for module in set(sys.modules.values()) - PRELOADED_MODULES:
                     if not hasattr(module, '__file__') or module.__file__ is None:
                         continue
 
+                    main_mod = module.__name__.split('.')[0]
+
+                    if main_mod in check_reloaded:
+                        continue
+
                     mod_file = Path(module.__file__)
 
                     if 'vspreview' in mod_file.parts:
                         continue
 
                     if std_path_lib in mod_file.parents or std_path_dlls in mod_file.parents:
                         continue
 
                     if not mod_file.exists() or not mod_file.is_file():
                         continue
 
-                    parent = Path(module.__file__)
+                    check_reloaded.add(main_mod)
 
-                    def _traverse(path: Path) -> Iterable[bool]:
-                        for module in iter_modules([path]):
-                            newpath = Path(module.module_finder) / module.name
+                for module in check_reloaded:
+                    all_submodules = sorted([
+                        k for k in sys.modules.keys()
+                        if k == module or k.startswith(f'{module}.')
+                    ])
 
-                            if module.ispkg:
-                                if _traverse([newpath]):
-                                    return True
-
-                                continue
-
-                            newpath = newpath.with_suffix('.py')
-
-                            try:
-                                stats = newpath.stat()
-                            except FileNotFoundError:
-                                return False
-
-                            return stats.st_mtime > self.last_reload_time
-
-                    if _traverse(parent):
+                    for mod_name in all_submodules:
                         try:
-                            logging.debug(f'Hot reloaded Python Package: "{module.__name__}"')
-                            reload_module(module)
-                        except Exception as e:
-                            logging.error(e)
+                            if Path(sys.modules[mod_name].__file__).stat().st_mtime > self.last_reload_time:
+                                break
+                        except Exception:
+                            ...
+                    else:
+                        continue
+
+                    try:
+                        logging.info(f'Hot reloaded Python Package: "{module}"')
+                        for mod_name in reversed(all_submodules):
+                            sys.modules[mod_name] = reload_module(sys.modules[mod_name])
+                    except Exception as e:
+                        logging.error(e)
 
             self.env = vpy.variables(
                 dict(self.external_args),
                 environment=vs.get_current_environment(),
                 module_name="__vspreview__"
             ).result()
             self.env.module.__dict__['_monkey_runpy'] = random()
@@ -310,34 +358,34 @@
             te = TracebackException.from_exception(e.parent_error)
             logging.error(''.join(te.format()))
 
             self.script_exec_failed = True
             return self.handle_script_error(
                 '\n'.join([
                     str(e), 'See console output for details.'
-                ])
+                ]), True
             )
         finally:
             if argv_orig is not None:
                 sys.argv = argv_orig
             sys.path.pop()
             self.last_reload_time = time()
 
         if len(vs.get_outputs()) == 0:
             logging.error('Script has no outputs set.')
             self.script_exec_failed = True
-            self.handle_script_error('Script has no outputs set.')
+            self.handle_script_error('Script has no outputs set.', True)
             return
 
         reload_from_error = self.script_exec_failed and reloading
         self.script_exec_failed = False
         self.current_storage_path = (self.current_config_dir / self.script_path.stem).with_suffix('.yml')
 
         self.storage_not_found = not (
-            self.current_storage_path.exists() and self.current_storage_path.read_text().strip()
+            self.current_storage_path.exists() and self.current_storage_path.read_text('utf8').strip()
         )
 
         load_error = None
 
         try:
             if self.storage_not_found or reload_from_error:
                 self.load_storage()
@@ -367,15 +415,15 @@
             error_string = "There was an error while loading the script!\n"
 
             logging.error(error_string + vpy.textwrap.indent(vpy.ExecutionFailed.extract_traceback(load_error), '| '))
 
             self.script_exec_failed = True
 
             return self.handle_script_error(
-                f'{error_string}{vpy.textwrap.indent(str(load_error), " | ")}\nSee console output for details.'
+                f'{error_string}{vpy.textwrap.indent(str(load_error), " | ")}\nSee console output for details.', False
             )
 
     @set_status_label('Loading...')
     def load_storage(self) -> None:
         storage_paths = [self.global_storage_path, self.current_storage_path]
 
         if self.storage_not_found:
@@ -482,16 +530,16 @@
                 '\n'.join([version, '# Global VSPreview storage for settings'] + storage_dump[:idx])
             )
 
         with io.open(self.current_storage_path, 'w', encoding='utf-8') as current_file:
             current_file.writelines(
                 '\n'.join([
                     version,
-                    f'# VSPreview script storage for: {self.script_path}',
-                    f'# Global setting saved at path: {self.global_storage_path}'
+                    f'# VSPreview local storage for script: {self.script_path}',
+                    f'# Global setting (storage/plugins) saved at path: {self.global_config_dir}'
                 ] + storage_dump[idx:])
             )
 
         if manually:
             self.show_message('Saved successfully')
 
     def _serialize_data(self) -> Any:
@@ -546,18 +594,26 @@
         for output in self.outputs:
             raw_frame_item = self.graphics_scene.addPixmap(QPixmap())
             raw_frame_item.hide()
 
             output.graphics_scene_item = GraphicsImageItem(raw_frame_item)
 
     def reload_script(self) -> None:
+        from vstools.utils.vs_proxy import clear_cache
+
         self.reload_before_signal.emit()
 
         self.dump_storage()
 
+        try:
+            with self.env:
+                clear_cache()
+        except Exception:
+            ...
+
         vs.clear_outputs()
         self.graphics_scene.clear()
 
         self.timecodes.clear()
         self.norm_timecodes.clear()
         for v in self.user_output_names.values():
             v.clear()
@@ -622,14 +678,16 @@
         self.current_output.last_showed_frame = frame
 
         self.timeline.set_position(frame)
 
         for toolbar in self.toolbars:
             toolbar.on_current_frame_changed(frame)
 
+        self.plugins.on_current_frame_changed(frame)
+
         self.statusbar.frame_props_label.setText(self.STATUS_FRAME_PROP(self.current_output.props))
 
     def switch_output(self, value: int | VideoOutput) -> None:
         if not self.outputs or len(self.outputs) == 0:
             return
 
         if isinstance(value, VideoOutput):
@@ -659,14 +717,16 @@
         self.current_output.graphics_scene_item.show()
         self.graphics_scene.setSceneRect(QRectF(self.current_output.graphics_scene_item.pixmap().rect()))
         self.timeline.update_notches()
 
         for toolbar in self.toolbars[1:]:
             toolbar.on_current_output_changed(index, prev_index)
 
+        self.plugins.on_current_output_changed(index, prev_index)
+
         self.update_statusbar_output_info()
 
     @property
     def current_output(self) -> VideoOutput:
         return cast(VideoOutput, self.toolbars.main.outputs_combobox.currentData())
 
     @current_output.setter
@@ -676,17 +736,18 @@
 
         self.switch_output(self.outputs.index_of(value))
 
     @property
     def outputs(self) -> VideoOutputs | None:
         return self.toolbars.main.outputs
 
-    def handle_script_error(self, message: str) -> None:
+    def handle_script_error(self, message: str, script: bool = False) -> None:
         self.clear_monkey_runpy()
         self.script_error_dialog.label.setText(message)
+        self.script_error_dialog.setWindowTitle('Script Loading Error' if script else 'Program Error')
         self.script_error_dialog.open()
 
     def on_wheel_scrolled(self, steps: int) -> None:
         new_index = self.toolbars.main.zoom_combobox.currentIndex() + steps
         if new_index < 0:
             new_index = 0
         elif new_index >= len(self.settings.zoom_levels):
@@ -699,34 +760,27 @@
             self.switch_frame(start)
             self.toolbars.playback.play()
         else:
             self.switch_frame(start)
 
     def update_display_profile(self) -> None:
         if sys.platform == 'win32':
-            if _imagingcms is None:
-                print(ImportWarning(
-                    'You\'re missing packages for the image csm!\n'
-                    'You can install it with "pip install pywin32 Pillow"!'
-                ))
-                return
-
-            assert self.app
+            assert self.app and _imagingcms
 
             screen_name = self.current_screen.name()
 
-            dc = win32gui.CreateDC(screen_name, None, None)
+            dc = win32gui.CreateDC('DISPLAY', screen_name, None)
 
             logging.info(f'Changed screen: {screen_name}')
 
             icc_path = _imagingcms.get_display_profile_win32(dc, 1)
 
             if icc_path is not None:
                 with open(icc_path, 'rb') as icc:
-                    self.display_profile = QColorSpace.fromIccProfile(QByteArray(len(x := icc.read()), x))
+                    self.display_profile = QColorSpace.fromIccProfile(icc.read())
 
         if hasattr(self, 'current_output') and self.current_output is not None and self.display_profile is not None:
             self.switch_frame(self.current_output.last_showed_frame)
 
     def show_message(self, message: str) -> None:
         self.statusbar.showMessage(
             message, round(float(self.settings.statusbar_message_timeout) * 1000)
@@ -836,28 +890,9 @@
         self.switch_output(self.toolbars.main.outputs_combobox.currentIndex())
 
         if playback_active:
             self.toolbars.playback.play()
 
     def __getstate__(self) -> Mapping[str, Any]:
         return super().__getstate__() | {
-            'window_settings': WindowSettings(
-                self.timeline.mode,
-                bytes(cast(bytearray, self.saveGeometry())),
-                bytes(cast(bytearray, self.saveState()))
-            )
+            'window_settings': self.window_settings
         }
-
-    def __setstate__(self, state: Mapping[str, Any]) -> None:
-        # toolbars is singleton, so it initialize itself right in its __setstate__()
-        self.window_settings = {}  # type: ignore
-
-        try:
-            try_load(state, 'window_settings', dict, self)
-        except BaseException:
-            try_load(state, 'timeline_mode', str, self.window_settings)
-            try_load(state, 'window_geometry', bytes, self.window_settings)
-            try_load(state, 'window_state', bytes, self.window_settings)
-
-        self.timeline.mode = self.window_settings.timeline_mode
-        self.restoreGeometry(QByteArray(len(x := self.window_settings.window_geometry), x))
-        self.restoreState(QByteArray(len(x := self.window_settings.window_state), x))
```

### Comparing `vspreview-0.4.4/vspreview/models/generalmodel.py` & `vspreview-0.5.0/vspreview/models/generalmodel.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/models/outputs.py` & `vspreview-0.5.0/vspreview/models/outputs.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/models/scening.py` & `vspreview-0.5.0/vspreview/models/scening.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/toolbars/__init__.py` & `vspreview-0.5.0/vspreview/toolbars/__init__.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/toolbars/benchmark/settings.py` & `vspreview-0.5.0/vspreview/toolbars/benchmark/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/toolbars/benchmark/toolbar.py` & `vspreview-0.5.0/vspreview/toolbars/benchmark/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import vapoursynth as vs
 from PyQt6.QtCore import QMetaObject, Qt
 from PyQt6.QtWidgets import QLabel
 
 from ...core import AbstractToolbar, CheckBox, Frame, PushButton, Time, Timer
 from ...core.custom import FrameEdit
-from ...utils import qt_silent_call, strfdelta, vs_clear_cache
+from ...utils import qt_silent_call, strfdelta
 from .settings import BenchmarkSettings
 
 
 if TYPE_CHECKING:
     from ...main import MainWindow
     from vapoursynth import _Future as Future
 else:
@@ -101,15 +101,16 @@
     def on_current_output_changed(self, index: int, prev_index: int) -> None:
         self.start_frame_control.setMaximum(self.main.current_output.total_frames - 1)
         self.end_frame_control.setMaximum(self.main.current_output.total_frames - 1)
         self.total_frames_control.setMaximum(self.main.current_output.total_frames - Frame(1))
 
     def run(self) -> None:
         if self.settings.clear_cache_enabled:
-            vs_clear_cache()
+            from vstools.utils.vs_proxy import clear_cache
+            clear_cache()
 
         if self.settings.frame_data_sharing_fix_enabled:
             self.main.current_output.update_graphic_item(
                 self.main.current_output.graphics_scene_item.pixmap().copy()
             )
 
         self.start_frame = self.start_frame_control.value()
```

### Comparing `vspreview-0.4.4/vspreview/toolbars/debug/toolbar.py` & `vspreview-0.5.0/vspreview/toolbars/debug/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
             self.exec_lineedit,
             PushButton('Exec', self, clicked=self.exec_button_clicked)
         ])
 
         self.hlayout.addStretch()
 
     def test_button_clicked(self, checked: bool | None = None) -> None:
-        from ...utils import vs_clear_cache
-        vs_clear_cache()
+        from vstools.utils.vs_proxy import clear_cache
+        clear_cache()
 
     def exec_button_clicked(self, checked: bool | None = None) -> None:
         try:
             exec(self.exec_lineedit.text())
         except BaseException as e:
             import logging
```

### Comparing `vspreview-0.4.4/vspreview/toolbars/main/dialog.py` & `vspreview-0.5.0/vspreview/core/custom/plotting.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,176 +1,212 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from math import exp, log
+from pathlib import Path
+from typing import Sequence
+
+import matplotlib.pyplot as plt  # type: ignore
+from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg  # type: ignore
+from matplotlib.figure import Figure  # type: ignore
+from matplotlib.layout_engine import ConstrainedLayoutEngine  # type: ignore
+from matplotlib.rcsetup import cycler  # type: ignore
+from PyQt6.QtCore import QEvent, QPointF, Qt, pyqtSignal
+from PyQt6.QtGui import QMouseEvent, QNativeGestureEvent, QWheelEvent
 
-from PyQt6.QtCore import QPointF, Qt
-from PyQt6.QtGui import QColor, QMouseEvent, QPainter, QPaintEvent
-from PyQt6.QtWidgets import QLabel
-from vapoursynth import FrameProps
+STYLE_DIR = Path(__file__).parent / 'plotting.mplstyle'
 
-from ...core import ExtendedWidget, HBoxLayout, PushButton, Stretch, VBoxLayout
 
-if TYPE_CHECKING:
-    from vstools import PropEnum
+__all__ = [
+    'apply_plotting_style',
 
-    from ...main import MainWindow
+    'PlottingCanvas'
+]
 
 
-__all__ = [
-    'FramePropsDialog'
-]
+def apply_plotting_style() -> None:
+    plt.style.use({
+        'axes.edgecolor': '#FFFFFF3D',
+        'axes.facecolor': '#FFFFFF07',
+        'axes.labelcolor': '#FFFFFFD9',
+        'axes.prop_cycle': cycler('color', [
+            '#FF6200', '#696969', '#525199', '#60A6DA', '#D0D93C', '#A8A8A9', '#FF0000', '#349651', '#AB0066'
+        ]),
+        'figure.facecolor': '#19232D',
+        'legend.edgecolor': '#FFFFFFD9',
+        'legend.facecolor': 'inherit',
+        'legend.framealpha': 0.12,
+        'markers.fillstyle': 'full',
+        'savefig.facecolor': '#19232D',
+        'text.color': 'white',
+        'xtick.color': '#FFFFFFD9',
+        'ytick.color': '#FFFFFFD9'
+    })
+
+
+class PlottingCanvas(FigureCanvasQTAgg):
+    WHEEL_STEP = 15 * 8  # degrees
+
+    mouseMoved = pyqtSignal(QMouseEvent)
+    wheelScrolled = pyqtSignal(int)
+
+    def __init__(self, ylog: bool = False, xlog: bool = False) -> None:
+        self.ylog, self.xlog = ylog, xlog
+
+        self.figure = Figure((5, 4), 100)
 
+        self.axes = self.figure.add_subplot(111)
 
-_frame_props_excluded_keys = {
-    # vs internals
-    '_AbsoluteTime', '_DurationNum', '_DurationDen', '_PictType', '_Alpha',
-    # Handled separately
-    '_SARNum', '_SARDen',
-    # source filters
-    '_FrameNumber',
-    # vstools set_output
-    'Name'
-}
-
-
-def _create_enum_props_lut(enum: type[PropEnum], pretty_name: str) -> tuple[str, dict[str, dict[int, str]]]:
-    return enum.prop_key, {
-        pretty_name: {
-            idx: enum.from_param(idx).pretty_string if enum.is_valid(idx) else 'Invalid'
-            for idx in range(min(enum.__members__.values()) - 1, max(enum.__members__.values()) + 1)
-        }
-    }
-
-
-class FramePropsDialog(ExtendedWidget):
-    __slots__ = (
-        'main_window', 'clicked', 'old_pos', 'header', 'framePropsVLayout'
-    )
-
-    def __init__(self, main_window: MainWindow) -> None:
-        from vstools import ChromaLocation, ColorRange, FieldBased, Matrix, Primaries, Transfer, PropEnum
-
-        super().__init__(main_window)
-
-        self.main_window = main_window
-        self.setWindowFlags(Qt.WindowType.FramelessWindowHint)
-        self.setAttribute(Qt.WidgetAttribute.WA_NoSystemBackground, True)
-        self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground, True)
-        self.clicked = False
-        self.old_pos = QPointF(0.0, 0.0)
-        self.setGeometry(100, 100, 300, 450)
-        self.setStyleSheet('.QLabel { font-size: 12px; background-color: none }')
+        self.figure.set_layout_engine(ConstrainedLayoutEngine())
 
-        self.setup_ui()
+        super().__init__(self.figure)
 
-        self.set_qobject_names()
-        self.hide()
+        self.angleRemainder = 0
+        self.zoomValue = 0.0
 
-        self._frame_props_lut = {
-            '_Combed': {
-                'Is Combed': [
-                    'No',
-                    'Yes'
-                ]
-            },
-            '_Field': {
-                'Frame Field Type': [
-                    'Bottom Field',
-                    'Top Field'
-                ]
-            },
-            '_SceneChangeNext': {
-                'Scene Cut': [
-                    'Current Scene',
-                    'End of Scene'
-                ]
-            },
-            '_SceneChangePrev': {
-                'Scene Change': [
-                    'Current Scene',
-                    'Start of Scene'
-                ]
-            }
-        } | dict([
-            _create_enum_props_lut(enum, name)
-            for enum, name in list[tuple[type[PropEnum], str]]([
-                (FieldBased, 'Field Type'),
-                (Matrix, 'Matrix'),
-                (Transfer, 'Transfer'),
-                (Primaries, 'Primaries'),
-                (ChromaLocation, 'Chroma Location'),
-                (ColorRange, 'Color Range')
-            ])
-        ])
-
-    def setup_ui(self) -> None:
-        self.framePropsVLayout = VBoxLayout()
-        self.header = QLabel()
-        font = self.header.font()
-        font.setPixelSize(15)
-        self.header.setFont(font)
-        VBoxLayout(self, [
-            HBoxLayout([
-                Stretch(), self.header, Stretch(), PushButton(' X ', clicked=self.hide)
-            ]),
-            self.framePropsVLayout,
-            Stretch()
-        ])
-
-    def showDialog(self, props: FrameProps | None) -> None:
-        if props is not None:
-            self.update_frame_props(props)
-
-        super().show()
-
-    def update_frame_props(self, props: FrameProps) -> None:
-        node_idx = self.main_window.toolbars.main.outputs_combobox.currentIndex()
-        self.header.setText(
-            f'Frame Props - Node {node_idx} / Frame {self.main_window.current_output.last_showed_frame}'
-        )
-        self.framePropsVLayout.clear()
+        self.clicked = False
+        self.old_pos = QPointF(0.0, 0.0)
 
-        def _add_prop_row(key: str, value: str) -> None:
-            self.framePropsVLayout.addLayout(
-                HBoxLayout([QLabel(key), QLabel(value)], spacing=5)
+    @classmethod
+    def limits_to_range(cls, lim: tuple[int, int]) -> int:
+        return lim[1] - lim[0]
+
+    @property
+    def cur_lims(self) -> tuple[tuple[float, float], tuple[float, float]]:
+
+        try:
+            return (
+                tuple[float, float](log(x) if self.xlog else x for x in self.axes.get_xlim()),
+                tuple[float, float](log(x) if self.ylog else x for x in self.axes.get_ylim())
             )
+        except ValueError:
+            return (self.axes.get_xlim(), self.axes.get_ylim())
 
-        for key in sorted(props.keys()):
-            if key in _frame_props_excluded_keys:
-                continue
-
-            if key in self._frame_props_lut:
-                title = list(self._frame_props_lut[key].keys())[0]
-                value_str = self._frame_props_lut[key][title][props[key]]  # type: ignore
-            else:
-                title = key[1:] if key.startswith('_') else key
-                value_str = str(props[key])
-
-            if value_str is not None:
-                _add_prop_row(title, value_str)
+    @cur_lims.setter
+    def cur_lims(self, new_lims: tuple[Sequence[float], Sequence[float]]) -> None:
+        new_xlim, new_ylim = new_lims
+
+        try:
+            self.axes.set_xlim(tuple[float, float](exp(x) if self.xlog else x for x in new_xlim))
+            self.axes.set_ylim(tuple[float, float](exp(x) if self.ylog else x for x in new_ylim))
+
+            self.figure.canvas.draw_idle()
+        except OverflowError:
+            # zooming/panning too much
+            ...
+
+    def event(self, event: QEvent) -> bool:
+        if isinstance(event, QNativeGestureEvent):
+            typ = event.gestureType()
+
+            if typ == Qt.NativeGestureType.BeginNativeGesture:
+                self.zoomValue = 0.0
+            elif typ == Qt.NativeGestureType.ZoomNativeGesture:
+                self.zoomValue += event.value()
 
-        if '_SARNum' in props and '_SARDen' in props:
-            _add_prop_row('Pixel aspect ratio', f"{props['_SARNum']}/{props['_SARDen']}")
+            if typ == Qt.NativeGestureType.EndNativeGesture:
+                self.zoom_function(event, -1 if self.zoomValue < 0 else 1)
 
-    def paintEvent(self, event: QPaintEvent) -> None:
-        QPainter(self).fillRect(self.rect(), QColor(45, 55, 65, 168))
-        self.main_window.timeline.full_repaint()
+        return super().event(event)
 
     def mousePressEvent(self, event: QMouseEvent) -> None:
-        self.clicked = True
+        if event.button() == Qt.MouseButton.LeftButton:
+            self.clicked = True
 
     def mouseReleaseEvent(self, event: QMouseEvent) -> None:
         self.clicked = False
 
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
+        self.mouseMoved.emit(event)
+
         if self.clicked:
-            new_x = int(self.pos().x() - (self.old_pos.x() - event.globalPosition().x()))
-            new_y = int(self.pos().y() - (self.old_pos.y() - event.globalPosition().y()))
+            cur_xlim, cur_ylim = self.cur_lims
 
-            if 0 < new_x < self.main_window.width() and 0 < new_y < self.main_window.height():
-                self.move(new_x, new_y)
-            else:
-                return
+            curr_pos = event.globalPosition()
+
+            rel_x = self.old_pos.x() - curr_pos.x()
+            rel_y = self.old_pos.y() - curr_pos.y()
+
+            width, height = self.get_width_height()
+            v_width, v_height = cur_xlim[1] - cur_xlim[0], cur_ylim[1] - cur_ylim[0]
+
+            xrate = rel_x * v_width / width
+            yrate = rel_y * v_height / height
+
+            self.cur_lims = (
+                (x + xrate for x in cur_xlim),
+                (x - yrate for x in cur_ylim)
+            )
 
         self.old_pos = event.globalPosition()
 
-        return super().mouseMoveEvent(event)
+        try:
+            super().mouseMoveEvent(event)
+        except Exception:
+            event.ignore()
+
+    def wheelEvent(self, event: QWheelEvent) -> None:
+        modifier = event.modifiers()
+        mouse = event.buttons()
+
+        if modifier == Qt.KeyboardModifier.ControlModifier or mouse in {
+            Qt.MouseButton.RightButton, Qt.MouseButton.MiddleButton
+        }:
+            angleDelta = event.angleDelta().y()
+
+            if self.angleRemainder * angleDelta < 0:
+                self.angleRemainder = 0
+
+            self.angleRemainder += angleDelta
+
+            if abs(self.angleRemainder) >= self.WHEEL_STEP:
+                steps = self.angleRemainder // self.WHEEL_STEP
+                self.zoomValue += steps
+                self.zoom_function(event, steps)
+
+                self.angleRemainder %= self.WHEEL_STEP
+
+        event.ignore()
+
+    def zoom_function(self, event: QWheelEvent, steps: int) -> None:
+        if not steps:
+            return
+
+        scale_factor = 1
+        base_scale = 1.1
+
+        for _ in range(abs(steps)):
+            if steps > 0:
+                scale_factor *= base_scale
+            else:
+                scale_factor /= base_scale
+
+        cur_xlim, cur_ylim = self.cur_lims
+
+        pos = event.position()
+        xdata, ydata = pos.x(), pos.y()
+        width, height = self.get_width_height()
+
+        xrate, yrate = xdata / width, ydata / height
+
+        xabs = cur_xlim[1] * xrate + cur_xlim[0] * (1 - xrate)
+        yabs = cur_ylim[0] * yrate + cur_ylim[1] * (1 - yrate)
+
+        new_width = abs(cur_xlim[1] - cur_xlim[0]) / scale_factor
+        new_height = abs(cur_ylim[1] - cur_ylim[0]) / scale_factor
+
+        self.cur_lims = (
+            (xabs - new_width * xrate, xabs + new_width * (1 - xrate)),
+            (yabs - new_height * (1 - yrate), yabs + new_height * yrate)
+        )
+
+    def clear(self) -> None:
+        self.axes.clear()
+
+        if self.ylog:
+            self.axes.set_yscale("log")
+
+        if self.xlog:
+            self.axes.set_xscale("log")
+
+    def draw(self) -> None:
+        if 0 not in self.figure.get_size_inches():
+            super().draw()
```

### Comparing `vspreview-0.4.4/vspreview/toolbars/main/toolbar.py` & `vspreview-0.5.0/vspreview/toolbars/main/toolbar.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from PyQt6.QtWidgets import QComboBox
 
 from ...core import (
     AbstractToolbar, CheckBox, ComboBox, Frame, FrameEdit, PushButton, Time, TimeEdit, VideoOutput, try_load
 )
 from ...models import GeneralModel, VideoOutputs
 from ...utils import qt_silent_call
-from .dialog import FramePropsDialog
 
 if TYPE_CHECKING:
     from ...main import MainSettings, MainWindow
 
 
 __all__ = [
     'MainToolbar'
@@ -23,15 +22,15 @@
 
 
 class MainToolbar(AbstractToolbar):
     _no_visibility_choice = True
     storable_attrs = ('outputs', )
 
     __slots__ = (
-        *storable_attrs, 'frame_props_dialog',
+        *storable_attrs,
         'outputs_combobox', 'frame_control', 'copy_frame_button',
         'time_control', 'copy_timestamp_button', 'zoom_combobox',
         'switch_timeline_mode_button', 'settings_button'
     )
 
     outputs: VideoOutputs | None
     zoom_combobox: ComboBox[float]
@@ -52,16 +51,14 @@
         self.set_qobject_names()
 
     def setup_ui(self) -> None:
         super().setup_ui()
 
         self.setVisible(True)
 
-        self.frame_props_dialog = FramePropsDialog(self.main)
-
         self.outputs_combobox = ComboBox[VideoOutput](
             self, editable=True, insertPolicy=QComboBox.InsertPolicy.InsertAtCurrent,
             duplicatesEnabled=True, sizeAdjustPolicy=QComboBox.SizeAdjustPolicy.AdjustToContents
         )
         self.outputs_combobox.currentIndexChanged.connect(self.main.switch_output)
         self.outputs_combobox.view().setMinimumWidth(
             self.outputs_combobox.minimumSizeHint().width()
@@ -86,29 +83,24 @@
         self.zoom_combobox = ComboBox[float](self, minimumContentsLength=4)
         self.zoom_combobox.currentTextChanged.connect(self.on_zoom_changed)
 
         self.switch_timeline_mode_button = PushButton(
             'Switch Timeline Mode', self, clicked=self.on_switch_timeline_mode_clicked
         )
 
-        self.frame_props_tab_button = PushButton(
-            'Frame Props', self, clicked=lambda: self.frame_props_dialog.showDialog(self.main.current_output.props)
-        )
-
         self.settings_button = PushButton('Settings', self, clicked=self.main.app_settings.show)
 
         self.hlayout.addWidgets([
             self.outputs_combobox,
             self.frame_control, self.copy_frame_button,
             self.time_control, self.copy_timestamp_button,
             self.sync_outputs_checkbox,
             self.get_separator(),
             self.auto_fit_button, self.zoom_combobox,
             self.switch_timeline_mode_button,
-            self.frame_props_tab_button,
             self.settings_button
         ])
 
         self.hlayout.addStretch()
 
     def add_shortcuts(self) -> None:
         self.main.add_shortcut(
@@ -156,17 +148,14 @@
     def on_current_frame_changed(self, frame: Frame) -> None:
         qt_silent_call(self.frame_control.setValue, frame)
         qt_silent_call(self.time_control.setValue, Time(frame))
 
         if self.outputs and len(self.outputs) > 1 and self.sync_outputs_checkbox.isChecked():
             self.on_sync_outputs_clicked(True, force_frame=frame)
 
-        if not self.frame_props_dialog.isHidden():
-            self.frame_props_dialog.update_frame_props(self.main.current_output.props)
-
     def on_current_output_changed(self, index: int, prev_index: int) -> None:
         qt_silent_call(self.outputs_combobox.setCurrentIndex, index)
         qt_silent_call(self.frame_control.setMaximum, self.main.current_output.total_frames - 1)
         qt_silent_call(self.time_control.setMaximum, self.main.current_output.total_time - Frame(1))
 
         if self.main.graphics_view.autofit:
             self.main.graphics_view.setZoom(None)
@@ -192,16 +181,14 @@
 
     def on_zoom_changed(self, text: str | None = None) -> None:
         self.main.graphics_view.setZoom(self.zoom_combobox.currentData())
 
     def __getstate__(self) -> Mapping[str, Any]:
         return super().__getstate__() | {
             'current_output_index': self.outputs_combobox.currentIndex(),
-            'current_zoom_index': self.zoom_combobox.currentIndex(),
             'sync_outputs': self.sync_outputs_checkbox.isChecked()
         }
 
     def __setstate__(self, state: Mapping[str, Any]) -> None:
         try_load(state, 'outputs', VideoOutputs, self.rescan_outputs)
-        try_load(state, 'current_zoom_index', int, self.zoom_combobox.setCurrentIndex)
         try_load(state, 'current_output_index', int, self.main.switch_output)
         try_load(state, 'sync_outputs', bool, self.sync_outputs_checkbox.setChecked)
```

### Comparing `vspreview-0.4.4/vspreview/toolbars/misc/toolbar.py` & `vspreview-0.5.0/vspreview/toolbars/misc/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/toolbars/pipette/colorview.py` & `vspreview-0.5.0/vspreview/toolbars/pipette/colorview.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/toolbars/pipette/toolbar.py` & `vspreview-0.5.0/vspreview/toolbars/pipette/toolbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
+from colorsys import rgb_to_hls, rgb_to_hsv
 from math import ceil, floor, log
 from typing import TYPE_CHECKING, Generator, cast
 from weakref import WeakKeyDictionary
 
 import vapoursynth as vs
 from PyQt6.QtCore import QPoint, Qt
 from PyQt6.QtGui import QFont, QMouseEvent
-from PyQt6.QtWidgets import QGraphicsView, QLabel
+from PyQt6.QtWidgets import QFrame, QGraphicsView, QLabel
 
 from ...core import AbstractToolbar, Frame, PushButton, VideoOutput
 from .colorview import ColorView
 from .settings import PipetteSettings
 
 if TYPE_CHECKING:
     from ...main import MainWindow
@@ -91,28 +92,36 @@
 
         self.src_label = QLabel(self)
 
         self.src_hex = QLabel(self)
         self.src_dec = QLabel(self)
         self.src_norm = QLabel(self)
 
+        self.rgb_hls = QLabel(self)
+        self.rgb_hsv = QLabel(self)
+
         for label in [
             self.position,
             self.rgb_hex, self.rgb_dec, self.rgb_norm,
             self.src_hex, self.src_dec, self.src_norm
         ]:
             label.setFont(font)
             label.setTextInteractionFlags(Qt.TextInteractionFlag.TextSelectableByMouse)
 
         self.copy_position_button = PushButton('⎘', self, clicked=self.on_copy_position_clicked)
 
         self.hlayout.addWidgets([
+            QFrame(),
             self.color_view, self.position, self.copy_position_button,
+            self.get_separator(),
             self.rgb_label, self.rgb_hex, self.rgb_dec, self.rgb_norm,
-            self.src_label, self.src_hex, self.src_dec, self.src_norm
+            self.get_separator(),
+            self.src_label, self.src_hex, self.src_dec, self.src_norm,
+            self.get_separator(),
+            QLabel('HLS:'), self.rgb_hls, QLabel('HSV:'), self.rgb_hsv,
         ])
 
         self.hlayout.addStretch()
 
     def on_current_frame_changed(self, frame: Frame) -> None:
         if self.last_pos and self.last_pos[0] is self.main.current_output:
             self.update_labels(self.last_pos[1])
@@ -189,21 +198,25 @@
         pos_f = self.main.graphics_view.mapToScene(local_pos)
 
         if not self.main.current_output.graphics_scene_item.contains(pos_f):
             return
 
         pos = QPoint(floor(pos_f.x()), floor(pos_f.y()))
         color = self.main.current_output.graphics_scene_item.pixmap().toImage().pixelColor(pos)
-        red, green, blue = color.red(), color.green(), color.blue()
+        components = color.red(), color.green(), color.blue()
+        components_float = tuple[float, ...](x / 255 for x in components)
 
         self.color_view.color = color
         self.position.setText('{:4d},{:4d}'.format(pos.x(), pos.y()))
-        self.rgb_hex.setText('{:2X},{:2X},{:2X}'.format(red, green, blue))
-        self.rgb_dec.setText('{:3d},{:3d},{:3d}'.format(red, green, blue))
-        self.rgb_norm.setText('{:0.5f},{:0.5f},{:0.5f}'.format(red / 255, green / 255, blue / 255))
+
+        self.rgb_hex.setText('{:2X},{:2X},{:2X}'.format(*components))
+        self.rgb_dec.setText('{:3d},{:3d},{:3d}'.format(*components))
+        self.rgb_norm.setText('{:0.5f},{:0.5f},{:0.5f}'.format(*components_float))
+        self.rgb_hls.setText('{}%,{}%,{}%'.format(*(int(x * 255) for x in rgb_to_hls(*components_float))))
+        self.rgb_hsv.setText('{}%,{}%,{}%'.format(*(int(x * 255) for x in rgb_to_hsv(*components_float))))
 
         if not self.src_label.isVisible():
             return
 
         fmt = self.current_source_frame.format
 
         src_vals = list(self.extract_value(self.current_source_frame, pos))
@@ -228,15 +241,15 @@
         if self.main.current_output not in self.outputs:
             self.outputs[self.main.current_output] = self.prepare_vs_output(self.main.current_output.source.clip)
 
         assert (src_fmt := self.outputs[self.main.current_output].format)
 
         has_alpha = bool(self.main.current_output.source.alpha)
 
-        self.src_label.setText(f"Raw ({str(src_fmt.color_family)[12:]}{' + Alpha' if has_alpha else ''}):")
+        self.src_label.setText(f"Raw ({src_fmt.color_family.name}{' + Alpha' if has_alpha else ''}):")
         self.src_hex.setVisible(src_fmt.sample_type == vs.INTEGER)
 
         if src_fmt.sample_type == vs.INTEGER:
             self.src_max_val = 2**src_fmt.bits_per_sample - 1
         elif src_fmt.sample_type == vs.FLOAT:
             self.src_max_val = 1.0
```

### Comparing `vspreview-0.4.4/vspreview/toolbars/playback/settings.py` & `vspreview-0.5.0/vspreview/toolbars/playback/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/toolbars/playback/toolbar.py` & `vspreview-0.5.0/vspreview/toolbars/playback/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/toolbars/scening/dialog.py` & `vspreview-0.5.0/vspreview/toolbars/scening/dialog.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/toolbars/scening/settings.py` & `vspreview-0.5.0/vspreview/toolbars/scening/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/toolbars/scening/toolbar.py` & `vspreview-0.5.0/vspreview/toolbars/scening/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,16 @@
         )
 
     def on_toggle(self, new_state: bool) -> None:
         if new_state is True:
             self.check_add_to_list_possibility()
             self.check_remove_export_possibility()
 
-        self.status_label.setVisible(self.is_notches_visible())
+        self.status_label.setVisible(self.is_notches_visible)
+
         super().on_toggle(new_state)
 
     def on_current_output_changed(self, index: int, prev_index: int) -> None:
         self.scening_list_dialog.on_current_output_changed(index, prev_index)
 
     def on_current_frame_changed(self, frame: Frame) -> None:
         self.check_remove_export_possibility()
@@ -250,14 +251,15 @@
 
     @current_list_index.setter
     def current_list_index(self, index: int) -> None:
         if (0 <= index < len(self.lists)):
             return self.items_combobox.setCurrentIndex(index)
         raise IndexError
 
+    @property
     def is_notches_visible(self) -> bool:
         return self.always_show_scene_marks_checkbox.isChecked() or self.toggle_button.isChecked()
 
     # list management
     def on_add_list_clicked(self, checked: bool | None = None) -> None:
         _, self.current_list_index = self.lists.add()
 
@@ -324,15 +326,15 @@
         self.main.switch_frame(new_pos)
 
     # scene management
     def on_add_single_frame_clicked(self, checked: bool | None = None) -> None:
         if self.current_list is None:
             self.on_add_list_clicked()
 
-        assert self.current_list
+        assert self.current_list is not None
 
         self.current_list.add(self.main.current_output.last_showed_frame, label=self.label_lineedit.text())
 
         self.check_remove_export_possibility()
 
     def on_add_to_list_clicked(self, checked: bool | None = None) -> None:
         self.current_list.add(self.first_frame, self.second_frame, self.label_lineedit.text())  # type: ignore
@@ -445,15 +447,15 @@
                 out_of_range_count += 1
 
     def import_celltimes(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
         Imports cell times as single-frame scenes
         '''
 
-        for line in path.read_text().splitlines():
+        for line in path.read_text('utf8').splitlines():
             try:
                 scening_list.add(Frame(int(line)))
             except ValueError:
                 out_of_range_count += 1
 
     def import_cue(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
@@ -472,15 +474,15 @@
             match = pattern.match(offset)
             if match is None:
                 return None
             return Time(minutes=int(match[1]), seconds=int(match[2]), milliseconds=int(match[3]) / 75 * 1000)
 
         cue_sheet = CueSheet()
         cue_sheet.setOutputFormat('')
-        cue_sheet.setData(path.read_text())
+        cue_sheet.setData(path.read_text('utf8'))
         cue_sheet.parse()
 
         for track in cue_sheet.tracks:
             if track.offset is None:
                 continue
             offset = offset_to_time(track.offset)
             if offset is None:
@@ -502,15 +504,15 @@
                 out_of_range_count += 1
 
     def import_dgi(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
         Imports IDR frames as single-frame scenes.
         '''
         pattern = re.compile(r'IDR\s\d+\n(\d+):FRM', re.RegexFlag.MULTILINE)
-        for match in pattern.findall(path.read_text()):
+        for match in pattern.findall(path.read_text('utf8')):
             try:
                 scening_list.add(Frame(match))
             except ValueError:
                 out_of_range_count += 1
 
     def import_lwi(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
@@ -522,15 +524,15 @@
         IS_KEY = 1
 
         pattern = re.compile(r'Index={}.*?Codec=(\d+).*?\n.*?Key=(\d)'.format(
             STREAM_INDEX
         ))
 
         frame = Frame(0)
-        for match in pattern.finditer(path.read_text(), re.RegexFlag.MULTILINE):
+        for match in pattern.finditer(path.read_text('utf8'), re.RegexFlag.MULTILINE):
             if int(match[1]) >= AV_CODEC_ID_FIRST_AUDIO:
                 frame += Frame(1)
                 continue
 
             if not int(match[2]) == IS_KEY:
                 frame += Frame(1)
                 continue
@@ -588,27 +590,27 @@
         Imports chapters as signle-frame scenes.
         Uses NAME for scene label.
         '''
         pattern = re.compile(
             r'(CHAPTER\d+)=(\d{2}):(\d{2}):(\d{2}(?:\.\d{3})?)\n\1NAME=(.*)',
             re.RegexFlag.MULTILINE
         )
-        for match in pattern.finditer(path.read_text()):
+        for match in pattern.finditer(path.read_text('utf8')):
             time = Time(hours=int(match[2]), minutes=int(match[3]), seconds=float(match[4]))
             try:
                 scening_list.add(Frame(time), label=match[5])
             except ValueError:
                 out_of_range_count += 1
 
     def import_qp(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
         Imports I- and K-frames as single-frame scenes.
         '''
         pattern = re.compile(r'(\d+)\sI|K')
-        for match in pattern.findall(path.read_text()):
+        for match in pattern.findall(path.read_text('utf8')):
             try:
                 scening_list.add(Frame(int(match)))
             except ValueError:
                 out_of_range_count += 1
 
     def import_ses(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
@@ -634,29 +636,29 @@
     def import_matroska_timestamps_v1(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
         Imports listed scenes.
         Uses FPS for scene label.
         '''
         pattern = re.compile(r'(\d+),(\d+),(\d+(?:\.\d+)?)')
 
-        for match in pattern.finditer(path.read_text()):
+        for match in pattern.finditer(path.read_text('utf8')):
             try:
                 scening_list.add(
                     Frame(int(match[1])), Frame(int(match[2])), '{:.3f} fps'.format(float(match[3]))
                 )
             except ValueError:
                 out_of_range_count += 1
 
     def import_matroska_timestamps_v2(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
         Imports intervals of constant FPS as scenes.
         Uses FPS for scene label.
         '''
         timestamps = list[Time]()
-        for line in path.read_text().splitlines():
+        for line in path.read_text('utf8').splitlines():
             try:
                 timestamps.append(Time(milliseconds=float(line)))
             except ValueError:
                 continue
 
         if len(timestamps) < 2:
             logging.warning(
@@ -700,22 +702,22 @@
         '''
         pattern = re.compile(
             r'^((?:\d+(?:\.\d+)?)|gap)(?:,\s?(\d+(?:\.\d+)?))?',
             re.RegexFlag.MULTILINE
         )
 
         assume_pattern = re.compile(r'assume (\d+(?:\.\d+))')
-        if len(mmatch := assume_pattern.findall(path.read_text())) > 0:
+        if len(mmatch := assume_pattern.findall(path.read_text('utf8'))) > 0:
             default_fps = float(mmatch[0])
         else:
             logging.warning('Scening import: "assume" entry not found.')
             return
 
         pos = Time()
-        for match in pattern.finditer(path.read_text()):
+        for match in pattern.finditer(path.read_text('utf8')):
             if match[1] == 'gap':
                 pos += Time(seconds=float(match[2]))
                 continue
 
             interval = Time(seconds=float(match[1]))
             fps = float(match[2]) if (match.lastindex or 0) >= 2 else default_fps
 
@@ -735,15 +737,15 @@
         '''
         class TFMFrame(Frame):
             mic: int | None
 
         tfm_frame_pattern = re.compile(r'(\d+)\s\((\d+)\)')
         tfm_group_pattern = re.compile(r'(\d+),(\d+)\s\((\d+(?:\.\d+)%)\)')
 
-        log = path.read_text()
+        log = path.read_text('utf8')
 
         start_pos = log.find('OVR HELP INFORMATION')
         if start_pos == -1:
             logging.warning("Scening import: TFM log doesn't contain OVR Help Information.")
             return
         log = log[start_pos:]
 
@@ -771,15 +773,15 @@
     def import_vsedit(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
         Imports bookmarks as single-frame scenes
         '''
 
         frames = []
 
-        for bookmark in path.read_text().split(', '):
+        for bookmark in path.read_text('utf8').split(', '):
             try:
                 frames.append(int(bookmark))
             except ValueError:
                 out_of_range_count += 1
 
         ranges = list[list[int]]()
         prev_x: int
@@ -799,38 +801,38 @@
             )
 
     def import_x264_2pass_log(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
         Imports I- and K-frames as single-frame scenes.
         '''
         pattern = re.compile(r'in:(\d+).*type:I|K')
-        for match in pattern.findall(path.read_text()):
+        for match in pattern.findall(path.read_text('utf8')):
             try:
                 scening_list.add(Frame(int(match)))
             except ValueError:
                 out_of_range_count += 1
 
     def import_xvid(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
         Imports I-frames as single-frame scenes.
         '''
-        for i, line in enumerate(path.read_text().splitlines()):
+        for i, line in enumerate(path.read_text('utf8').splitlines()):
             if not line.startswith('i'):
                 continue
             try:
                 scening_list.add(Frame(i - 3))
             except ValueError:
                 out_of_range_count += 1
 
     def import_generic(self, path: Path, scening_list: SceningList, out_of_range_count: int) -> None:
         '''
         Import generic (rfs style) frame mappings: {start end}
 
         '''
-        for line in path.read_text().splitlines():
+        for line in path.read_text('utf8').splitlines():
             try:
                 fnumbers = [int(n) for n in line.split()]
                 scening_list.add(Frame(fnumbers[0]), Frame(fnumbers[1]))
             except ValueError:
                 out_of_range_count += 1
 
     # export
```

### Comparing `vspreview-0.4.4/vspreview/utils/debug.py` & `vspreview-0.5.0/vspreview/utils/debug.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.4/vspreview/utils/utils.py` & `vspreview-0.5.0/vspreview/utils/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from __future__ import annotations
 
 from functools import partial, wraps
 from string import Template
 from typing import TYPE_CHECKING, Any, Callable
 
-import vapoursynth as vs
 from PyQt6.QtCore import QSignalBlocker
 
 if TYPE_CHECKING:
     from vstools import F, P, R, T
 
-from ..core import Frame, Time, main_window
+from ..core import Time, main_window
 
 __all__ = [
     'qt_silent_call',
     'strfdelta',
     'fire_and_forget',
-    'set_status_label',
-    'vs_clear_cache',
+    'set_status_label'
 ]
 
 
 # it is a BuiltinMethodType at the same time
 def qt_silent_call(qt_method: Callable[P, R], *args: P.args, **kwargs: P.kwargs) -> R:
     block = QSignalBlocker(qt_method.__self__)  # type: ignore
     ret = qt_method(*args, **kwargs)
@@ -81,17 +79,7 @@
 
             main.statusbar.label.setText('Ready')
 
             return ret
         return _wrapped
 
     return _decorator
-
-
-def vs_clear_cache() -> None:
-    cache_size = vs.core.max_cache_size
-    vs.core.max_cache_size = 1
-    for output in list(vs.get_outputs().values()):
-        if isinstance(output, vs.VideoOutputTuple):
-            output.clip.get_frame(int(main_window().current_output.last_showed_frame or Frame(0)))
-            break
-    vs.core.max_cache_size = cache_size
```

### Comparing `vspreview-0.4.4/vspreview.egg-info/PKG-INFO` & `vspreview-0.5.0/vspreview.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.4.4
+Version: 0.5.0
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
@@ -27,15 +27,15 @@
 
 This program is meant to be paired with a code editor with integrated terminal like Visual Studio Code.
 
 # Prerequisites
 
 1. [Python](https://www.Python.org/downloads) (3.10+ required)
     * Make sure to install Python to your `PATH`.
-1. [Vapoursynth](https://github.com/vapoursynth/vapoursynth/releases) (R59+ required)
+1. [VapourSynth](https://github.com/vapoursynth/vapoursynth/releases) (R60+ required)
 
 # Installation
 
 Install latest stable via pypi:
 ```bash
 pip install vspreview
 ```
@@ -46,15 +46,16 @@
 pip install -U git+https://github.com/Irrational-Encoding-Wizardry/vs-preview.git
 ```
 
 # Usage
 
 It can be used by running `vspreview script.vpy` or your preferred way in [your IDE](#ide-integration).
 
-[Keyboard Shortcuts](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/shortcuts.md)
+[Keyboard Shortcuts](https://github.com/Irrational-Encoding-Wizardry/vs-preview/blob/master/docs/accessibility/keybinds.rst)
 
 [Saved Frame Filename Variables](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/save_frame_placeholders.md)
 
 # IDE Integration
 
-* [VSCode](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/vscode_install.md)
-* [Vim](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/vim_install.md)
+* [Visual Studio Code](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/installation/install_vscode.rst)
+* [Vim](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/installation/install_vim.rst)
+* [Notepad++](https://github.com/Irrational-Encoding-Wizardry/vs-preview/tree/master/docs/installation/install_notepad++.rst)
```

### Comparing `vspreview-0.4.4/vspreview.egg-info/SOURCES.txt` & `vspreview-0.5.0/vspreview.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 vspreview/core/custom/__init__.py
 vspreview/core/custom/combobox.py
 vspreview/core/custom/dragnavigator.py
 vspreview/core/custom/edits.py
 vspreview/core/custom/graphicsview.py
 vspreview/core/custom/misc.py
 vspreview/core/custom/notch.py
+vspreview/core/custom/plotting.py
 vspreview/core/types/__init__.py
 vspreview/core/types/audio.py
 vspreview/core/types/misc.py
 vspreview/core/types/scene.py
 vspreview/core/types/units.py
 vspreview/core/types/video.py
 vspreview/core/types/yaml.py
@@ -43,28 +44,29 @@
 vspreview/main/dialog.py
 vspreview/main/settings.py
 vspreview/main/timeline.py
 vspreview/main/window.py
 vspreview/models/__init__.py
 vspreview/models/generalmodel.py
 vspreview/models/outputs.py
-vspreview/models/picture_types.py
 vspreview/models/scening.py
+vspreview/plugins/__init__.py
+vspreview/plugins/abstract.py
+vspreview/plugins/frame_props.ppy
 vspreview/toolbars/__init__.py
 vspreview/toolbars/benchmark/__init__.py
 vspreview/toolbars/benchmark/settings.py
 vspreview/toolbars/benchmark/toolbar.py
 vspreview/toolbars/comp/__init__.py
 vspreview/toolbars/comp/settings.py
 vspreview/toolbars/comp/toolbar.py
 vspreview/toolbars/debug/__init__.py
 vspreview/toolbars/debug/settings.py
 vspreview/toolbars/debug/toolbar.py
 vspreview/toolbars/main/__init__.py
-vspreview/toolbars/main/dialog.py
 vspreview/toolbars/main/toolbar.py
 vspreview/toolbars/misc/__init__.py
 vspreview/toolbars/misc/settings.py
 vspreview/toolbars/misc/toolbar.py
 vspreview/toolbars/pipette/__init__.py
 vspreview/toolbars/pipette/colorview.py
 vspreview/toolbars/pipette/settings.py
```

