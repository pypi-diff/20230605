# Comparing `tmp/pymultiMATIC-0.7.0b4.tar.gz` & `tmp/pymultiMATIC-0.7.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultiMATIC-0.7.0b4.tar", last modified: Tue Mar 21 09:33:42 2023, max compression
+gzip compressed data, was "pymultiMATIC-0.7.0b5.tar", last modified: Mon Jun  5 15:13:30 2023, max compression
```

## Comparing `pymultiMATIC-0.7.0b4.tar` & `pymultiMATIC-0.7.0b5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:33:42.735223 pymultiMATIC-0.7.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-03-21 09:33:42.735223 pymultiMATIC-0.7.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:33:42.727223 pymultiMATIC-0.7.0b4/pymultiMATIC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-03-21 09:33:42.000000 pymultiMATIC-0.7.0b4/pymultiMATIC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-21 09:33:42.000000 pymultiMATIC-0.7.0b4/pymultiMATIC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 09:33:42.000000 pymultiMATIC-0.7.0b4/pymultiMATIC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 09:33:42.000000 pymultiMATIC-0.7.0b4/pymultiMATIC.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-21 09:33:42.000000 pymultiMATIC-0.7.0b4/pymultiMATIC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 09:33:42.000000 pymultiMATIC-0.7.0b4/pymultiMATIC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:33:42.727223 pymultiMATIC-0.7.0b4/pymultimatic/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:33:42.731223 pymultiMATIC-0.7.0b4/pymultimatic/api/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/api/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/api/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/api/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/api/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/api/payloads_senso.py
--rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/api/urls_senso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:33:42.731223 pymultiMATIC-0.7.0b4/pymultimatic/model/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/dhw.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/quick_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/syncstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/timeprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/ventilation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/model/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    34200 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/systemmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:33:42.731223 pymultiMATIC-0.7.0b4/pymultimatic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/pymultimatic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-21 09:33:42.735223 pymultiMATIC-0.7.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:33:42.735223 pymultiMATIC-0.7.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_boilerstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_circulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_holidaymode.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_hot_water.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_hvacstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)    26418 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_quickmode.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_quickveto.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_room.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_syncstate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23155 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    38068 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_systemmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_timeprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_ventilation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-03-21 09:33:28.000000 pymultiMATIC-0.7.0b4/tests/test_zone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:30.596942 pymultiMATIC-0.7.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-05 15:13:18.000000 pymultiMATIC-0.7.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-05 15:13:30.596942 pymultiMATIC-0.7.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-05 15:13:18.000000 pymultiMATIC-0.7.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:30.592942 pymultiMATIC-0.7.0b5/pymultiMATIC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-05 15:13:30.000000 pymultiMATIC-0.7.0b5/pymultiMATIC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-05 15:13:30.000000 pymultiMATIC-0.7.0b5/pymultiMATIC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:13:30.000000 pymultiMATIC-0.7.0b5/pymultiMATIC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:13:30.000000 pymultiMATIC-0.7.0b5/pymultiMATIC.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 15:13:30.000000 pymultiMATIC-0.7.0b5/pymultiMATIC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 15:13:30.000000 pymultiMATIC-0.7.0b5/pymultiMATIC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:30.592942 pymultiMATIC-0.7.0b5/pymultimatic/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:30.592942 pymultiMATIC-0.7.0b5/pymultimatic/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/api/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/api/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/api/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/api/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/api/payloads_senso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/api/urls_senso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:30.596942 pymultiMATIC-0.7.0b5/pymultimatic/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/dhw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21716 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/quick_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/syncstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/timeprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/ventilation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/model/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34270 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/systemmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:30.596942 pymultiMATIC-0.7.0b5/pymultimatic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/pymultimatic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 15:13:30.596942 pymultiMATIC-0.7.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:30.596942 pymultiMATIC-0.7.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_boilerstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_circulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_holidaymode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_hot_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_hvacstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26418 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_quickmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_quickveto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_syncstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23155 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38154 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_systemmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_timeprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_ventilation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-05 15:13:19.000000 pymultiMATIC-0.7.0b5/tests/test_zone.py
```

### Comparing `pymultiMATIC-0.7.0b4/LICENSE` & `pymultiMATIC-0.7.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/PKG-INFO` & `pymultiMATIC-0.7.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pymultiMATIC
-Version: 0.7.0b4
+Version: 0.7.0b5
 Summary: Python interface with Vaillant multiMATIC
 Home-page: https://github.com/thomasgermain/pymultiMATIC.git
 Author: Thomas Germain
 Author-email: 12560542+thomasgermain@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymultiMATIC
 ![PyPI - License](https://img.shields.io/github/license/thomasgermain/pymultiMATIC)
 [![codecov](https://codecov.io/gh/thomasgermain/pymultiMATIC/branch/master/graph/badge.svg?token=KKM0BRHJR7)](https://codecov.io/gh/thomasgermain/pymultiMATIC)
```

### Comparing `pymultiMATIC-0.7.0b4/README.md` & `pymultiMATIC-0.7.0b5/README.md`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultiMATIC.egg-info/PKG-INFO` & `pymultiMATIC-0.7.0b5/pymultiMATIC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pymultiMATIC
-Version: 0.7.0b4
+Version: 0.7.0b5
 Summary: Python interface with Vaillant multiMATIC
 Home-page: https://github.com/thomasgermain/pymultiMATIC.git
 Author: Thomas Germain
 Author-email: 12560542+thomasgermain@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymultiMATIC
 ![PyPI - License](https://img.shields.io/github/license/thomasgermain/pymultiMATIC)
 [![codecov](https://codecov.io/gh/thomasgermain/pymultiMATIC/branch/master/graph/badge.svg?token=KKM0BRHJR7)](https://codecov.io/gh/thomasgermain/pymultiMATIC)
```

### Comparing `pymultiMATIC-0.7.0b4/pymultiMATIC.egg-info/SOURCES.txt` & `pymultiMATIC-0.7.0b5/pymultiMATIC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/api/connector.py` & `pymultiMATIC-0.7.0b5/pymultimatic/api/connector.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/api/error.py` & `pymultiMATIC-0.7.0b5/pymultimatic/api/error.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/api/payloads.py` & `pymultiMATIC-0.7.0b5/pymultimatic/api/payloads.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/api/payloads_senso.py` & `pymultiMATIC-0.7.0b5/pymultimatic/api/payloads_senso.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/api/schemas.py` & `pymultiMATIC-0.7.0b5/pymultimatic/api/schemas.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/api/urls.py` & `pymultiMATIC-0.7.0b5/pymultimatic/api/urls.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/api/urls_senso.py` & `pymultiMATIC-0.7.0b5/pymultimatic/api/urls_senso.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/__init__.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/common.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/common.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/dhw.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/dhw.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/info.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/info.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/mapper.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         func = _map_function(raw_heating, "setting", rbr, quick_veto is not None)
         zone_heating = ZoneHeating(func[0], func[1], func[2], func[3])
 
         if raw_cooling:
             func = _map_function(raw_cooling, "setting")
             zone_cooling = ZoneCooling(func[0], func[1], func[2], func[3])
 
-        return Zone(  # type: ignore
+        return Zone(
             id=zone_id,
             name=name,
             temperature=temperature,
             quick_veto=quick_veto,
             active_function=active_function,
             rbr=rbr,
             heating=zone_heating,
```

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/mode.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/mode.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/quick_mode.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/quick_mode.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/report.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/report.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/room.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/room.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/status.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/status.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/syncstate.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/syncstate.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/system.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/system.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/timeprogram.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/timeprogram.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/ventilation.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/ventilation.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/model/zone.py` & `pymultiMATIC-0.7.0b5/pymultimatic/model/zone.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/systemmanager.py` & `pymultiMATIC-0.7.0b5/pymultimatic/systemmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,21 @@
         take some times, it actually does multiples API calls, depending on
         your system configuration.
 
         Returns:
             System: the full system.
         """
 
-        (facilities, full_system, live_report, hvac_state, gateway_json,) = await asyncio.gather(
+        (
+            facilities,
+            full_system,
+            live_report,
+            hvac_state,
+            gateway_json,
+        ) = await asyncio.gather(
             self._call_api(self.urls.facilities_list, schema=schemas.FACILITIES),
             self._call_api(self.urls.system, schema=schemas.SYSTEM),
             self._call_api(self.urls.live_report, schema=schemas.LIVE_REPORTS),
             self._call_api(self.urls.hvac, schema=schemas.HVAC),
             self._call_api(self.urls.gateway_type, schema=schemas.GATEWAY),
         )
```

### Comparing `pymultiMATIC-0.7.0b4/pymultimatic/utils/__init__.py` & `pymultiMATIC-0.7.0b5/pymultimatic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/setup.py` & `pymultiMATIC-0.7.0b5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pymultiMATIC",
-    version="0.7.0b4",
+    version="0.7.0b5",
     description="Python interface with Vaillant multiMATIC",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/thomasgermain/pymultiMATIC.git",
     author="Thomas Germain",
     author_email="12560542+thomasgermain@users.noreply.github.com",
     license="MIT",
@@ -27,10 +27,11 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Home Automation",
     ],
 )
```

### Comparing `pymultiMATIC-0.7.0b4/tests/test_boilerstatus.py` & `pymultiMATIC-0.7.0b5/tests/test_boilerstatus.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_circulation.py` & `pymultiMATIC-0.7.0b5/tests/test_circulation.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_connector.py` & `pymultiMATIC-0.7.0b5/tests/test_connector.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_holidaymode.py` & `pymultiMATIC-0.7.0b5/tests/test_holidaymode.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_hot_water.py` & `pymultiMATIC-0.7.0b5/tests/test_hot_water.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_hvacstatus.py` & `pymultiMATIC-0.7.0b5/tests/test_hvacstatus.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_mapper.py` & `pymultiMATIC-0.7.0b5/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_payloads.py` & `pymultiMATIC-0.7.0b5/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_quickmode.py` & `pymultiMATIC-0.7.0b5/tests/test_quickmode.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_quickveto.py` & `pymultiMATIC-0.7.0b5/tests/test_quickveto.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_room.py` & `pymultiMATIC-0.7.0b5/tests/test_room.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_schema.py` & `pymultiMATIC-0.7.0b5/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_syncstate.py` & `pymultiMATIC-0.7.0b5/tests/test_syncstate.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_system.py` & `pymultiMATIC-0.7.0b5/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_systemmanager.py` & `pymultiMATIC-0.7.0b5/tests/test_systemmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import json
 from datetime import date, timedelta
 from typing import Any, AsyncGenerator, Dict, List, Tuple, Type
 from unittest import mock
 
 import pytest
+import pytest_asyncio
 from aiohttp import ClientSession
 from aioresponses import aioresponses
 
 from pymultimatic.api import (
     ApiError,
     defaults,
     Connector,
@@ -19,45 +20,45 @@
 from pymultimatic.model import OperatingModes, QuickModes, QuickVeto, constants, mapper
 from pymultimatic.systemmanager import SystemManager, retry_async
 from tests.conftest import mock_auth, path
 
 SERIAL = mapper.map_serial_number(json.loads(open(path("files/responses/facilities")).read()))
 
 
-@pytest.fixture(name="resp", autouse=True)
+@pytest_asyncio.fixture(name="resp", autouse=True)
 async def fixture_resp(resp: aioresponses) -> AsyncGenerator[aioresponses, None]:
     with open(path("files/responses/facilities"), "r") as file:
         facilities = json.loads(file.read())
         resp.get(urls.facilities_list(), payload=facilities, status=200)
     yield resp
 
 
-@pytest.fixture(name="manager")
+@pytest_asyncio.fixture(name="manager")
 async def fixture_manager(
     session: ClientSession, connector: Connector
 ) -> AsyncGenerator[SystemManager, None]:
     manager = SystemManager("user", "pass", session, "pymultiMATIC", SERIAL)
     await connector.login()
     with mock.patch.object(connector, "request", wraps=connector.request):
         manager._connector = connector
         yield manager
 
 
-@pytest.fixture(name="senso_manager")
+@pytest_asyncio.fixture(name="senso_manager")
 async def fixture_senso_manager(
     session: ClientSession, senso_connector: Connector
 ) -> AsyncGenerator[SystemManager, None]:
     manager = SystemManager("user", "pass", session, "pymultiMATIC", SERIAL, defaults.SENSO)
     await senso_connector.login()
     with mock.patch.object(senso_connector, "request", wraps=senso_connector.request):
         manager._connector = senso_connector
         yield manager
 
 
-@pytest.fixture(name="managers")
+@pytest_asyncio.fixture(name="managers")
 async def fixture_managers(
     session: ClientSession,
     connector: Connector,
     manager: SystemManager,
     senso_manager: SystemManager,
 ) -> AsyncGenerator[List[SystemManager], None]:
     yield [manager, senso_manager]
@@ -844,15 +845,15 @@
     )
 
     with open(path("files/responses/facilities_multiple"), "r") as file:
         json_raw = json.loads(file.read())
 
     key = None
     for match in resp._matches.items():
-        if match[1].url_or_pattern.path in manager.urls.facilities_list():
+        if match[1].url_or_pattern.path in manager.urls.facilities_list():  # type: ignore
             key = match[0]
     resp._matches.pop(key)
     resp.get(url, status=200, payload=json_raw)
 
     details = await manager.get_facility_detail("888")
     assert details.serial_number == "888"
     _assert_calls(1, manager, [url])
@@ -867,15 +868,15 @@
     )
 
     with open(path("files/responses/facilities_multiple"), "r") as file:
         json_raw = json.loads(file.read())
 
     key = None
     for match in resp._matches.items():
-        if match[1].url_or_pattern.path in senso_manager.urls.facilities_list():
+        if match[1].url_or_pattern.path in senso_manager.urls.facilities_list():  # type: ignore
             key = match[0]
     resp._matches.pop(key)
     resp.get(url, status=200, payload=json_raw)
 
     details = await senso_manager.get_facility_detail("888")
     assert details.serial_number == "888"
     _assert_calls(1, senso_manager, [url])
```

### Comparing `pymultiMATIC-0.7.0b4/tests/test_timeprogram.py` & `pymultiMATIC-0.7.0b5/tests/test_timeprogram.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_urls.py` & `pymultiMATIC-0.7.0b5/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_ventilation.py` & `pymultiMATIC-0.7.0b5/tests/test_ventilation.py`

 * *Files identical despite different names*

### Comparing `pymultiMATIC-0.7.0b4/tests/test_zone.py` & `pymultiMATIC-0.7.0b5/tests/test_zone.py`

 * *Files identical despite different names*

