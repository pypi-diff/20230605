# Comparing `tmp/zigpy-0.55.0.tar.gz` & `tmp/zigpy-0.56.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-0.55.0.tar", last modified: Mon Apr 24 17:30:04 2023, max compression
+gzip compressed data, was "zigpy-0.56.0.tar", last modified: Mon Jun  5 20:35:02 2023, max compression
```

## Comparing `zigpy-0.55.0.tar` & `zigpy-0.56.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 17:30:00.000000 zigpy-0.55.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 17:30:00.000000 zigpy-0.55.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-24 17:30:04.128014 zigpy-0.55.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-24 17:30:00.000000 zigpy-0.55.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-24 17:30:04.132014 zigpy-0.55.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-24 17:30:00.000000 zigpy-0.55.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.120014 zigpy-0.55.0/zigpy/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43034 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/appdb_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v0.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v1.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v10.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v11.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v2.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v4.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v5.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v6.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v8.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v9.sql
--rw-r--r--   0 runner    (1001) docker     (123)    44010 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/backups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/ota/
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/ota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/ota/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/ota/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/ota/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/profiles/zha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/profiles/zll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/quirks/
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/quirks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/quirks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/zigpy/types/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23677 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/types/named.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/zigpy/zcl/
--rw-r--r--   0 runner    (1001) docker     (123)    33587 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/zigpy/zcl/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25260 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/closures.py
--rw-r--r--   0 runner    (1001) docker     (123)    82633 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/hvac.py
--rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/lighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/manufacturer_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/foundation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/zigpy/zdo/
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zdo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.120014 zigpy-0.55.0/zigpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-05 20:34:59.000000 zigpy-0.56.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-05 20:34:59.000000 zigpy-0.56.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-05 20:35:02.334019 zigpy-0.56.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-06-05 20:34:59.000000 zigpy-0.56.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-05 20:35:02.338019 zigpy-0.56.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-05 20:34:59.000000 zigpy-0.56.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.326019 zigpy-0.56.0/zigpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45515 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/appdb_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v0.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v1.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v10.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v12.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v4.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v5.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v6.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v8.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v9.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/backups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/ota/
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/ota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/ota/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/ota/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/ota/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/profiles/zgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/profiles/zha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/profiles/zll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/quirks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/quirks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/quirks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/zigpy/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23899 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/zigpy/zcl/
+-rw-r--r--   0 runner    (1001) docker     (123)    35495 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/zigpy/zcl/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90858 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/manufacturer_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16606 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/foundation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/zigpy/zdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zdo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.326019 zigpy-0.56.0/zigpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/top_level.txt
```

### Comparing `zigpy-0.55.0/COPYING` & `zigpy-0.56.0/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/LICENSE` & `zigpy-0.56.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/PKG-INFO` & `zigpy-0.56.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.55.0
+Version: 0.56.0
 Summary: Library implementing a ZigBee stack
 Home-page: https://github.com/zigpy/zigpy
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zigpy-0.55.0/README.md` & `zigpy-0.56.0/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/setup.cfg` & `zigpy-0.56.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/setup.py` & `zigpy-0.56.0/setup.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb.py` & `zigpy-0.56.0/zigpy/appdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 import zigpy.typing
 import zigpy.util
 from zigpy.zcl.clusters.general import Basic
 from zigpy.zdo import types as zdo_t
 
 LOGGER = logging.getLogger(__name__)
 
-DB_VERSION = 11
+DB_VERSION = 12
 DB_V = f"_v{DB_VERSION}"
 MIN_SQLITE_VERSION = (3, 24, 0)
 
 UNIX_EPOCH = datetime.fromtimestamp(0, tz=timezone.utc)
 DB_V_REGEX = re.compile(r"(?:_v\d+)?$")
 
-MIN_LAST_SEEN_DELTA = timedelta(seconds=30).total_seconds()
+MIN_UPDATE_DELTA = timedelta(seconds=30).total_seconds()
 
 
 def _import_compatible_sqlite3(min_version: tuple[int, int, int]) -> types.ModuleType:
     """Loads an SQLite module with a library version matching the provided constraint."""
 
     import sqlite3
 
@@ -235,21 +235,21 @@
     ) -> None:
         """Device last_seen time is updated."""
         self.enqueue("_save_device_last_seen", device.ieee, last_seen)
 
     async def _save_device_last_seen(self, ieee: t.EUI64, last_seen: datetime) -> None:
         q = f"""UPDATE devices{DB_V}
                     SET last_seen=:ts
-                    WHERE ieee=:ieee AND :ts - last_seen > :min_last_seen_delta"""
+                    WHERE ieee=:ieee AND :ts - last_seen > :min_update_delta"""
         await self.execute(
             q,
             {
                 "ts": last_seen.timestamp(),
                 "ieee": ieee,
-                "min_last_seen_delta": MIN_LAST_SEEN_DELTA,
+                "min_update_delta": MIN_UPDATE_DELTA,
             },
         )
         await self._db.commit()
 
     def device_relays_updated(
         self, device: zigpy.typing.DeviceType, relays: t.Relays | None
     ) -> None:
@@ -264,23 +264,28 @@
                         ON CONFLICT (ieee)
                         DO UPDATE SET relays=excluded.relays WHERE relays != :relays"""
             await self.execute(q, {"ieee": ieee, "relays": relays.serialize()})
 
         await self._db.commit()
 
     def attribute_updated(
-        self, cluster: zigpy.typing.ClusterType, attrid: int, value: Any
+        self,
+        cluster: zigpy.typing.ClusterType,
+        attrid: int,
+        value: Any,
+        timestamp: datetime,
     ) -> None:
         self.enqueue(
             "_save_attribute",
             cluster.endpoint.device.ieee,
             cluster.endpoint.endpoint_id,
             cluster.cluster_id,
             attrid,
             value,
+            timestamp,
         )
 
     def unsupported_attribute_added(
         self, cluster: zigpy.typing.ClusterType, attrid: int
     ) -> None:
         self.enqueue(
             "_unsupported_attribute_added",
@@ -493,21 +498,28 @@
         q = f"""INSERT INTO in_clusters{DB_V} VALUES (?, ?, ?)
                     ON CONFLICT (ieee, endpoint_id, cluster)
                     DO NOTHING"""
         await self._db.executemany(q, clusters)
 
     async def _save_attribute_cache(self, ep: zigpy.typing.EndpointType) -> None:
         clusters = [
-            (ep.device.ieee, ep.endpoint_id, cluster.cluster_id, attrid, value)
+            (
+                ep.device.ieee,
+                ep.endpoint_id,
+                cluster.cluster_id,
+                attrid,
+                value,
+                cluster._attr_last_updated.get(attrid, UNIX_EPOCH).timestamp(),
+            )
             for cluster in ep.in_clusters.values()
             for attrid, value in cluster._attr_cache.items()
         ]
-        q = f"""INSERT INTO attributes_cache{DB_V} VALUES (?, ?, ?, ?, ?)
+        q = f"""INSERT INTO attributes_cache{DB_V} VALUES (?, ?, ?, ?, ?, ?)
                     ON CONFLICT (ieee, endpoint_id, cluster, attrid)
-                    DO UPDATE SET value=excluded.value"""
+                    DO UPDATE SET value=excluded.value, last_updated=excluded.last_updated"""
         await self._db.executemany(q, clusters)
 
     async def _save_unsupported_attributes(self, ep: zigpy.typing.EndpointType) -> None:
         clusters = [
             (ep.device.ieee, ep.endpoint_id, cluster.cluster_id, attr)
             for cluster in ep.in_clusters.values()
             for attr in cluster.unsupported_attributes
@@ -525,21 +537,43 @@
         ]
         q = f"""INSERT INTO out_clusters{DB_V} VALUES (?, ?, ?)
                     ON CONFLICT (ieee, endpoint_id, cluster)
                     DO NOTHING"""
         await self._db.executemany(q, clusters)
 
     async def _save_attribute(
-        self, ieee: t.EUI64, endpoint_id: int, cluster_id: int, attrid: int, value: Any
+        self,
+        ieee: t.EUI64,
+        endpoint_id: int,
+        cluster_id: int,
+        attrid: int,
+        value: Any,
+        timestamp: datetime,
     ) -> None:
-        q = f"""INSERT INTO attributes_cache{DB_V} VALUES (?, ?, ?, ?, ?)
-                    ON CONFLICT (ieee, endpoint_id, cluster, attrid)
-                    DO UPDATE SET
-                        value=excluded.value WHERE value != excluded.value"""
-        await self.execute(q, (ieee, endpoint_id, cluster_id, attrid, value))
+        q = f"""
+            INSERT INTO attributes_cache{DB_V}
+            VALUES (:ieee, :endpoint_id, :cluster_id, :attrid, :value, :timestamp)
+                ON CONFLICT (ieee, endpoint_id, cluster, attrid) DO UPDATE
+                SET value=excluded.value, last_updated=excluded.last_updated
+                WHERE
+                    value != excluded.value
+                    AND :timestamp - last_updated > :min_update_delta
+            """
+        await self.execute(
+            q,
+            {
+                "ieee": ieee,
+                "endpoint_id": endpoint_id,
+                "cluster_id": cluster_id,
+                "attrid": attrid,
+                "value": value,
+                "timestamp": timestamp.timestamp(),
+                "min_update_delta": MIN_UPDATE_DELTA,
+            },
+        )
         await self._db.commit()
 
     def network_backup_created(self, backup: zigpy.backups.NetworkBackup) -> None:
         self.enqueue("_network_backup_created", json.dumps(backup.as_dict()))
 
     async def _network_backup_created(self, backup_json: str) -> None:
         q = f"""INSERT INTO network_backups{DB_V} VALUES (?, ?)
@@ -586,27 +620,37 @@
     async def _load_attributes(self, filter: str = None) -> None:
         if filter:
             query = f"SELECT * FROM attributes_cache{DB_V} WHERE {filter}"
         else:
             query = f"SELECT * FROM attributes_cache{DB_V}"
 
         async with self.execute(query) as cursor:
-            async for (ieee, endpoint_id, cluster, attrid, value) in cursor:
+            async for (
+                ieee,
+                endpoint_id,
+                cluster,
+                attrid,
+                value,
+                last_updated,
+            ) in cursor:
                 dev = self._application.get_device(ieee)
 
                 # Some quirks create endpoints and clusters that do not exist
                 if endpoint_id not in dev.endpoints:
                     continue
 
                 ep = dev.endpoints[endpoint_id]
 
                 if cluster not in ep.in_clusters:
                     continue
 
                 ep.in_clusters[cluster]._attr_cache[attrid] = value
+                ep.in_clusters[cluster]._attr_last_updated[
+                    attrid
+                ] = datetime.fromtimestamp(last_updated, timezone.utc)
 
                 LOGGER.debug(
                     "[0x%04x:%s:0x%04x] Attribute id: %s value: %s",
                     dev.nwk,
                     endpoint_id,
                     cluster,
                     attrid,
@@ -815,14 +859,15 @@
                 (self._migrate_to_v5, 5),
                 (self._migrate_to_v6, 6),
                 (self._migrate_to_v7, 7),
                 (self._migrate_to_v8, 8),
                 (self._migrate_to_v9, 9),
                 (self._migrate_to_v10, 10),
                 (self._migrate_to_v11, 11),
+                (self._migrate_to_v12, 12),
             ]:
                 if db_version >= min(to_db_version, DB_VERSION):
                     continue
 
                 LOGGER.info(
                     "Migrating database from v%d to v%d", db_version, to_db_version
                 )
@@ -1092,7 +1137,36 @@
                 "attributes_cache_v10": "attributes_cache_v11",
                 "neighbors_v10": "neighbors_v11",
                 "node_descriptors_v10": "node_descriptors_v11",
                 "unsupported_attributes_v10": "unsupported_attributes_v11",
                 "network_backups_v10": "network_backups_v11",
             }
         )
+
+    async def _migrate_to_v12(self):
+        """Schema v12 added a `timestamp` column to attribute updates."""
+
+        await self._migrate_tables(
+            {
+                "devices_v11": "devices_v12",
+                "endpoints_v11": "endpoints_v12",
+                "in_clusters_v11": "in_clusters_v12",
+                "neighbors_v11": "neighbors_v12",
+                "routes_v11": "routes_v12",
+                "node_descriptors_v11": "node_descriptors_v12",
+                "out_clusters_v11": "out_clusters_v12",
+                "groups_v11": "groups_v12",
+                "group_members_v11": "group_members_v12",
+                "relays_v11": "relays_v12",
+                "unsupported_attributes_v11": "unsupported_attributes_v12",
+                "network_backups_v11": "network_backups_v12",
+                "attributes_cache_v11": None,
+            }
+        )
+
+        async with self.execute("SELECT * FROM attributes_cache_v11") as cursor:
+            async for (ieee, endpoint_id, cluster_id, attrid, value) in cursor:
+                # Set the default `last_updated` to the unix epoch
+                await self.execute(
+                    "INSERT INTO attributes_cache_v12 VALUES (?, ?, ?, ?, ?, ?)",
+                    (ieee, endpoint_id, cluster_id, attrid, value, 0),
+                )
```

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v0.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v0.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v1.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v1.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v10.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v10.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v11.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v11.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v2.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v2.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v3.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v3.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v4.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v4.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v5.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v5.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v6.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v6.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v7.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v7.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v8.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v8.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/appdb_schemas/schema_v9.sql` & `zigpy-0.56.0/zigpy/appdb_schemas/schema_v9.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/application.py` & `zigpy-0.56.0/zigpy/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,15 +769,14 @@
 
         if dest.relays is None:
             return None
 
         # TODO: utilize topology scanner information
         return dest.relays[::-1]
 
-    @zigpy.util.retryable_request
     async def request(
         self,
         device: zigpy.device.Device,
         profile: t.uint16_t,
         cluster: t.uint16_t,
         src_ep: t.uint8_t,
         dst_ep: t.uint8_t,
```

### Comparing `zigpy-0.55.0/zigpy/backups.py` & `zigpy-0.56.0/zigpy/backups.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/config/__init__.py` & `zigpy-0.56.0/zigpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/config/defaults.py` & `zigpy-0.56.0/zigpy/config/defaults.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/config/validators.py` & `zigpy-0.56.0/zigpy/config/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/const.py` & `zigpy-0.56.0/zigpy/const.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/device.py` & `zigpy-0.56.0/zigpy/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,46 +158,41 @@
         self._initialize_task = asyncio.create_task(self.initialize())
 
         return self._initialize_task
 
     async def get_node_descriptor(self) -> zdo_t.NodeDescriptor:
         self.info("Requesting 'Node Descriptor'")
 
-        status, _, node_desc = await self.zdo.Node_Desc_req(
-            self.nwk, tries=2, delay=0.1
-        )
+        status, _, node_desc = await self.zdo.Node_Desc_req(self.nwk)
 
         if status != zdo_t.Status.SUCCESS:
             raise zigpy.exceptions.InvalidResponse(
                 f"Requesting Node Descriptor failed: {status}"
             )
 
         self.node_desc = node_desc
         self.info("Got Node Descriptor: %s", node_desc)
 
         return node_desc
 
     async def initialize(self) -> None:
         try:
             await self._initialize()
-        except Exception as e:
-            if not isinstance(
-                e, (asyncio.TimeoutError, zigpy.exceptions.ZigbeeException)
-            ):
-                LOGGER.warning(
-                    "Device %r failed to initialize due to unexpected error",
-                    self,
-                    exc_info=True,
-                )
+        except (asyncio.TimeoutError, zigpy.exceptions.ZigbeeException):
+            self.application.listener_event("device_init_failure", self)
+        except Exception:
+            LOGGER.warning(
+                "Device %r failed to initialize due to unexpected error",
+                self,
+                exc_info=True,
+            )
 
             self.application.listener_event("device_init_failure", self)
 
-    @zigpy.util.retryable(
-        (asyncio.TimeoutError, zigpy.exceptions.ZigbeeException), tries=3, delay=0.5
-    )
+    @zigpy.util.retryable_request(tries=5, delay=0.5)
     async def _initialize(self) -> None:
         """Attempts multiple times to discover all basic information about a device: namely
         its node descriptor, all endpoints and clusters, and the model and manufacturer
         attributes from any Basic cluster exposing those attributes.
         """
 
         # Some devices are improperly initialized and are missing a node descriptor
@@ -206,17 +201,15 @@
 
         # Devices should have endpoints other than ZDO
         if self.has_non_zdo_endpoints:
             self.info("Already have endpoints: %s", self.endpoints)
         else:
             self.info("Discovering endpoints")
 
-            status, _, endpoints = await self.zdo.Active_EP_req(
-                self.nwk, tries=3, delay=0.5
-            )
+            status, _, endpoints = await self.zdo.Active_EP_req(self.nwk)
 
             if status != zdo_t.Status.SUCCESS:
                 raise zigpy.exceptions.InvalidResponse(
                     f"Endpoint request failed: {status}"
                 )
 
             self.info("Discovered endpoints: %s", endpoints)
```

### Comparing `zigpy-0.55.0/zigpy/endpoint.py` & `zigpy-0.56.0/zigpy/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import zigpy.exceptions
 import zigpy.profiles
 import zigpy.types as t
 from zigpy.typing import AddressingMode, DeviceType
 import zigpy.util
 import zigpy.zcl
 from zigpy.zcl.foundation import (
+    GENERAL_COMMANDS,
     CommandSchema,
     GeneralCommand,
     Status as ZCLStatus,
     ZCLHeader,
 )
 from zigpy.zdo.types import Status as ZDOStatus
 
@@ -56,15 +57,15 @@
     async def initialize(self) -> None:
         self.info("Discovering endpoint information")
 
         if self.profile_id is not None or self.status == Status.ENDPOINT_INACTIVE:
             self.info("Endpoint descriptor already queried")
         else:
             status, _, sd = await self._device.zdo.Simple_Desc_req(
-                self._device.nwk, self._endpoint_id, tries=3, delay=2
+                self._device.nwk, self._endpoint_id
             )
 
             if status == ZDOStatus.NOT_ACTIVE:
                 # These endpoints are essentially junk but this lets the device join
                 self.status = Status.ENDPOINT_INACTIVE
                 return
             elif status != ZDOStatus.SUCCESS:
@@ -100,18 +101,18 @@
             if cluster_id in self.in_clusters:
                 return self.in_clusters[cluster_id]
 
             cluster = zigpy.zcl.Cluster.from_id(self, cluster_id, is_server=True)
 
         self.in_clusters[cluster_id] = cluster
 
-        if hasattr(cluster, "ep_attribute"):
+        if cluster.ep_attribute is not None:
             self._cluster_attr[cluster.ep_attribute] = cluster
 
-        if hasattr(self._device.application, "_dblistener"):
+        if self._device.application._dblistener is not None:
             listener = zigpy.zcl.ClusterPersistingListener(
                 self._device.application._dblistener, cluster
             )
             cluster.add_listener(listener)
 
         return cluster
 
@@ -160,21 +161,25 @@
         if grp_id in self.device.application.groups:
             self.device.application.groups[grp_id].remove_member(self)
         return res[0]
 
     async def group_membership_scan(self) -> None:
         """Sync up group membership."""
         try:
-            res = await self.groups.get_membership([])
+            res = await self.groups.get_membership(groups=[])
         except AttributeError:
             return
         except (asyncio.TimeoutError, zigpy.exceptions.ZigbeeException):
             self.debug("Failed to sync-up group membership")
             return
 
+        if isinstance(res, GENERAL_COMMANDS[GeneralCommand.Default_Response].schema):
+            self.debug("Device does not support group commands: %s", res)
+            return
+
         groups = set(res[1])
         self.device.application.groups.update_group_membership(self, groups)
 
     async def get_model_info(self) -> tuple[str | None, str | None]:
         if zigpy.zcl.clusters.general.Basic.cluster_id not in self.in_clusters:
             return None, None
```

### Comparing `zigpy-0.55.0/zigpy/exceptions.py` & `zigpy-0.56.0/zigpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/group.py` & `zigpy-0.56.0/zigpy/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     @classmethod
     def from_attr(
         cls, group_endpoint: GroupEndpoint, ep_name: str
     ) -> zigpy.zcl.Cluster:
         """Instantiate by Cluster name."""
 
         for cluster in cls._registry.values():
-            if hasattr(cluster, "ep_attribute") and cluster.ep_attribute == ep_name:
+            if cluster.ep_attribute == ep_name:
                 return cluster(group_endpoint, is_server=True)
         raise AttributeError(f"Unsupported {ep_name} group cluster")
 
 
 class GroupEndpoint(LocalLogMixin):
     """Group request handlers.
```

### Comparing `zigpy-0.55.0/zigpy/listeners.py` & `zigpy-0.56.0/zigpy/listeners.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/ota/__init__.py` & `zigpy-0.56.0/zigpy/ota/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/ota/image.py` & `zigpy-0.56.0/zigpy/ota/image.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/ota/provider.py` & `zigpy-0.56.0/zigpy/ota/provider.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/ota/validators.py` & `zigpy-0.56.0/zigpy/ota/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/profiles/zha.py` & `zigpy-0.56.0/zigpy/profiles/zha.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/profiles/zll.py` & `zigpy-0.56.0/zigpy/profiles/zll.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/quirks/__init__.py` & `zigpy-0.56.0/zigpy/quirks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,14 @@
 
     async def command(
         self,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
         *args,
         manufacturer: int | t.uint16_t | None = None,
         expect_reply: bool = True,
-        tries: int = 1,
         tsn: int | t.uint8_t | None = None,
         **kwargs: typing.Any,
     ) -> typing.Coroutine:
         command = self.server_commands[command_id]
 
         if manufacturer is None and (
             self._is_manuf_specific or command.is_manufacturer_specific
@@ -200,15 +199,14 @@
         return await self.request(
             False,
             command.id,
             command.schema,
             *args,
             manufacturer=manufacturer,
             expect_reply=expect_reply,
-            tries=tries,
             tsn=tsn,
             **kwargs,
         )
 
     async def client_command(
         self,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
```

### Comparing `zigpy-0.55.0/zigpy/quirks/registry.py` & `zigpy-0.56.0/zigpy/quirks/registry.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/serial.py` & `zigpy-0.56.0/zigpy/serial.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/state.py` & `zigpy-0.56.0/zigpy/state.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/topology.py` & `zigpy-0.56.0/zigpy/topology.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/types/basic.py` & `zigpy-0.56.0/zigpy/types/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,18 +356,23 @@
 
 class uint64_t_be(uint_t_be, bits=64):
     pass
 
 
 class _IntEnumMeta(enum.EnumMeta):
     def __call__(cls, value, names=None, *args, **kwargs):
-        if isinstance(value, str) and value.startswith("0x"):
-            value = int(value, base=16)
-        else:
-            value = int(value)
+        if isinstance(value, str):
+            if value.startswith("0x"):
+                value = int(value, base=16)
+            elif value.isnumeric():
+                value = int(value)
+            elif value.startswith(cls.__name__ + "."):
+                value = cls[value[len(cls.__name__) + 1 :]].value
+            else:
+                value = cls[value].value
         return super().__call__(value, names, *args, **kwargs)
 
 
 def bitmap_factory(int_type: CALLABLE_T) -> CALLABLE_T:
     """Mixins are broken by Python 3.8.6 so we must dynamically create the enum with the
     appropriate methods but with only one non-Enum parent class.
     """
```

### Comparing `zigpy-0.55.0/zigpy/types/named.py` & `zigpy-0.56.0/zigpy/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/types/struct.py` & `zigpy-0.56.0/zigpy/types/struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,21 +53,14 @@
         # The "Optional" subclass is dynamically created and breaks types.
         # We have to use a little introspection to find our real class.
         return next(c for c in cls.__mro__ if c.__name__ != "Optional")
 
     def __init_subclass__(cls) -> None:
         super().__init_subclass__()
 
-        # Explicitly check for old-style structs
-        if hasattr(cls, "_fields"):
-            raise TypeError(
-                "Struct subclasses do not use `_fields` anymore."
-                " Use class attributes with type annotations."
-            )
-
         # We generate fields up here to fail early and cache it
         cls.fields = cls._real_cls()._get_fields()
 
         # Check to see if the Struct is also an integer
         cls._int_type = next(
             (
                 c
```

### Comparing `zigpy-0.55.0/zigpy/typing.py` & `zigpy-0.56.0/zigpy/typing.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/util.py` & `zigpy-0.56.0/zigpy/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,40 +136,40 @@
             tries -= 1
             await asyncio.sleep(delay)
 
 
 def retryable(
     retry_exceptions: typing.Iterable[BaseException], tries: int = 1, delay: float = 0.1
 ) -> typing.Callable:
-    """Return a decorator which makes a function able to be retried
-
-    This adds "tries" and "delay" keyword arguments to the function. Only
-    exceptions in `retry_exceptions` will be retried.
+    """Return a decorator which makes a function able to be retried.
+    Only exceptions in `retry_exceptions` will be retried.
     """
 
     def decorator(func: typing.Callable) -> typing.Callable:
         nonlocal tries, delay
 
         @functools.wraps(func)
-        def wrapper(*args, tries=tries, delay=delay, **kwargs):
+        def wrapper(*args, **kwargs):
             if tries <= 1:
                 return func(*args, **kwargs)
             return retry(
                 functools.partial(func, *args, **kwargs),
                 retry_exceptions,
                 tries=tries,
                 delay=delay,
             )
 
         return wrapper
 
     return decorator
 
 
-retryable_request = retryable((ZigbeeException, asyncio.TimeoutError))
+retryable_request = functools.partial(
+    retryable, (ZigbeeException, asyncio.TimeoutError)
+)
 
 
 def aes_mmo_hash_update(length: int, result: bytes, data: bytes) -> tuple[int, bytes]:
     block_size = AES.block_size // 8
 
     while len(data) >= block_size:
         block = bytes(data[:block_size])
```

### Comparing `zigpy-0.55.0/zigpy/zcl/__init__.py` & `zigpy-0.56.0/zigpy/zcl/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from __future__ import annotations
 
+import collections
+from datetime import datetime, timezone
 import enum
 import functools
+import itertools
 import logging
-from typing import TYPE_CHECKING, Any, Sequence
+import types
+from typing import TYPE_CHECKING, Any, Iterable, Sequence
 import warnings
 
 from zigpy import util
 import zigpy.types as t
 from zigpy.typing import AddressingMode, EndpointType
 from zigpy.zcl import foundation
+from zigpy.zcl.foundation import BaseAttributeDefs, BaseCommandDefs
 
 if TYPE_CHECKING:
     from zigpy.appdb import PersistingListener
     from zigpy.endpoint import Endpoint
 
 
 LOGGER = logging.getLogger(__name__)
@@ -47,128 +52,168 @@
     Server = 0
     Client = 1
 
 
 class Cluster(util.ListenableMixin, util.CatchingTaskMixin):
     """A cluster on an endpoint"""
 
+    class AttributeDefs(BaseAttributeDefs):
+        pass
+
+    class ServerCommandDefs(BaseCommandDefs):
+        pass
+
+    class ClientCommandDefs(BaseCommandDefs):
+        pass
+
     # Custom clusters for quirks subclass Cluster but should not be stored in any global
     # registries, since they're device-specific and collide with existing clusters.
     _skip_registry: bool = False
 
     # Most clusters are identified by a single cluster ID
     cluster_id: t.uint16_t = None
 
     # Clusters are accessible by name from their endpoint as an attribute
     ep_attribute: str = None
 
     # Manufacturer specific clusters exist between 0xFC00 and 0xFFFF. This exists solely
     # to remove the need to create 1024 "ManufacturerSpecificCluster" instances.
     cluster_id_range: tuple[t.uint16_t, t.uint16_t] = None
 
-    # Clusters contain attributes and both client and server commands
+    # Deprecated: clusters contain attributes and both client and server commands
     attributes: dict[int, foundation.ZCLAttributeDef] = {}
     client_commands: dict[int, foundation.ZCLCommandDef] = {}
     server_commands: dict[int, foundation.ZCLCommandDef] = {}
+    attributes_by_name: dict[str, foundation.ZCLAttributeDef] = {}
+    commands_by_name: dict[str, foundation.ZCLCommandDef] = {}
 
     # Internal caches and indices
     _registry: dict = {}
     _registry_range: dict = {}
 
-    _server_commands_idx: dict[str, int] = {}
-    _client_commands_idx: dict[str, int] = {}
-
-    attributes_by_name: dict[str, foundation.ZCLAttributeDef] = {}
-    commands_by_name: dict[str, foundation.ZCLCommandDef] = {}
-
     def __init_subclass__(cls) -> None:
-        # Fail on deprecated attribute presence
-        for a in ("attributes", "client_commands", "server_commands"):
-            if not hasattr(cls, f"manufacturer_{a}"):
-                continue
-
-            raise TypeError(
-                f"`manufacturer_{a}` is deprecated. Copy the parent class's `{a}`"
-                f" dictionary and update it with your manufacturer-specific `{a}`. Make"
-                f" sure to specify that it is manufacturer-specific through the "
-                f" appropriate constructor or tuple!"
-            )
-
         if cls.cluster_id is not None:
             cls.cluster_id = t.ClusterId(cls.cluster_id)
 
-        # Clear the caches and lookup tables. Their contents should correspond exactly
-        # to what's in their respective command/attribute dictionaries.
-        cls.attributes_by_name = {}
-        cls.commands_by_name = {}
-        cls._server_commands_idx = {}
-        cls._client_commands_idx = {}
-
-        # Compile command definitions
-        for commands, index in [
-            (cls.server_commands, cls._server_commands_idx),
-            (cls.client_commands, cls._client_commands_idx),
-        ]:
+        # Compile the old command definitions
+        for commands in [cls.server_commands, cls.client_commands]:
             for command_id, command in list(commands.items()):
                 if isinstance(command, tuple):
                     # Backwards compatibility with old command tuples
                     name, schema, direction = command
                     command = foundation.ZCLCommandDef(
                         id=command_id,
                         name=name,
                         schema=convert_list_schema(schema, command_id, direction),
                         direction=direction,
                     )
-                else:
-                    command = command.replace(id=command_id)
-
-                if command.name in cls.commands_by_name:
-                    raise TypeError(
-                        f"Command name {command} is not unique in {cls}: {cls.commands_by_name}"
-                    )
-
-                index[command.name] = command.id
 
-                command = command.with_compiled_schema()
+                command = command.replace(id=command_id).with_compiled_schema()
                 commands[command.id] = command
-                cls.commands_by_name[command.name] = command
 
-        # Compile attributes
+        # Compile the old attribute definitions
         for attr_id, attr in list(cls.attributes.items()):
             if isinstance(attr, tuple):
                 if len(attr) == 2:
                     attr_name, attr_type = attr
                     attr_manuf_specific = False
                 else:
                     attr_name, attr_type, attr_manuf_specific = attr
 
                 attr = foundation.ZCLAttributeDef(
                     id=attr_id,
                     name=attr_name,
                     type=attr_type,
                     is_manufacturer_specific=attr_manuf_specific,
                 )
-            else:
-                attr = attr.replace(id=attr_id)
 
-            cls.attributes[attr.id] = attr
-            cls.attributes_by_name[attr.name] = attr
+            cls.attributes[attr.id] = attr.replace(id=attr_id)
+
+        # Create new definitions from the old-style definitions
+        if cls.attributes and "AttributeDefs" not in cls.__dict__:
+            cls.AttributeDefs = types.new_class(
+                name="AttributeDefs",
+                bases=(BaseAttributeDefs,),
+            )
+
+            for attr in cls.attributes.values():
+                setattr(cls.AttributeDefs, attr.name, attr)
+
+        if cls.server_commands and "ServerCommandDefs" not in cls.__dict__:
+            cls.ServerCommandDefs = types.new_class(
+                name="ServerCommandDefs",
+                bases=(BaseCommandDefs,),
+            )
+
+            for command in cls.server_commands.values():
+                setattr(cls.ServerCommandDefs, command.name, command)
+
+        if cls.client_commands and "ClientCommandDefs" not in cls.__dict__:
+            cls.ClientCommandDefs = types.new_class(
+                name="ClientCommandDefs",
+                bases=(BaseCommandDefs,),
+            )
+
+            for command in cls.client_commands.values():
+                setattr(cls.ClientCommandDefs, command.name, command)
+
+        # Check the old definitions for duplicates
+        for old_defs in [cls.attributes, cls.server_commands, cls.client_commands]:
+            counts = collections.Counter(d.name for d in old_defs.values())
+
+            if len(counts) != sum(counts.values()):
+                duplicates = [n for n, c in counts.items() if c > 1]
+                raise TypeError(f"Duplicate definitions exist for {duplicates}")
+
+        # Populate the `name` attribute of every definition
+        for defs in (cls.ServerCommandDefs, cls.ClientCommandDefs, cls.AttributeDefs):
+            for name in dir(defs):
+                definition = getattr(defs, name)
+
+                if (
+                    isinstance(
+                        definition,
+                        (foundation.ZCLCommandDef, foundation.ZCLAttributeDef),
+                    )
+                    and definition.name is None
+                ):
+                    object.__setattr__(definition, "name", name)
+
+        # Compile the schemas
+        for defs in (cls.ServerCommandDefs, cls.ClientCommandDefs):
+            for name in dir(defs):
+                definition = getattr(defs, name)
+
+                if isinstance(definition, foundation.ZCLCommandDef):
+                    setattr(defs, definition.name, definition.with_compiled_schema())
+
+        # Recreate the old structures using the new-style definitions
+        cls.attributes = {attr.id: attr for attr in cls.AttributeDefs}
+        cls.client_commands = {cmd.id: cmd for cmd in cls.ClientCommandDefs}
+        cls.server_commands = {cmd.id: cmd for cmd in cls.ServerCommandDefs}
+        cls.attributes_by_name = {attr.name: attr for attr in cls.AttributeDefs}
+
+        all_cmds: Iterable[foundation.ZCLCommandDef] = itertools.chain(
+            cls.ClientCommandDefs, cls.ServerCommandDefs
+        )
+        cls.commands_by_name = {cmd.name: cmd for cmd in all_cmds}
 
         if cls._skip_registry:
             return
 
         if cls.cluster_id is not None:
             cls._registry[cls.cluster_id] = cls
 
         if cls.cluster_id_range is not None:
             cls._registry_range[cls.cluster_id_range] = cls
 
     def __init__(self, endpoint: EndpointType, is_server: bool = True) -> None:
         self._endpoint: EndpointType = endpoint
         self._attr_cache: dict[int, Any] = {}
+        self._attr_last_updated: dict[int, datetime] = {}
         self.unsupported_attributes: set[int | str] = set()
         self._listeners = {}
         self._type: ClusterType = (
             ClusterType.Server if is_server else ClusterType.Client
         )
 
     @property
@@ -292,15 +337,14 @@
             manufacturer=manufacturer,
             tsn=tsn,
             command_id=command_id,
         )
 
         return hdr, request
 
-    @util.retryable_request
     async def request(
         self,
         general: bool,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
         schema: dict | t.Struct,
         *args,
         manufacturer: int | t.uint16_t | None = None,
@@ -698,28 +742,26 @@
 
     def command(
         self,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
         *args,
         manufacturer: int | t.uint16_t | None = None,
         expect_reply: bool = True,
-        tries: int = 1,
         tsn: int | t.uint8_t | None = None,
         **kwargs,
     ):
         command = self.server_commands[command_id]
 
         return self.request(
             False,
             command_id,
             command.schema,
             *args,
             manufacturer=manufacturer,
             expect_reply=expect_reply,
-            tries=tries,
             tsn=tsn,
             **kwargs,
         )
 
     def client_command(
         self,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
@@ -756,50 +798,57 @@
 
     @property
     def endpoint(self) -> Endpoint:
         return self._endpoint
 
     @property
     def commands(self):
-        return list(self._server_commands_idx.keys())
+        return list(self.ServerCommandDefs)
 
     def update_attribute(self, attrid: int | t.uint16_t, value: Any) -> None:
         """Update specified attribute with specified value"""
         self._update_attribute(attrid, value)
 
     def _update_attribute(self, attrid: int | t.uint16_t, value: Any) -> None:
+        now = datetime.now(timezone.utc)
+
         self._attr_cache[attrid] = value
-        self.listener_event("attribute_updated", attrid, value)
+        self._attr_last_updated[attrid] = now
+
+        self.listener_event("attribute_updated", attrid, value, now)
 
     def log(self, lvl: int, msg: str, *args, **kwargs) -> None:
         msg = "[%s:%s:0x%04x] " + msg
         args = (
             self._endpoint.device.name,
             self._endpoint.endpoint_id,
             self.cluster_id,
         ) + args
         return LOGGER.log(lvl, msg, *args, **kwargs)
 
     def __getattr__(self, name: str) -> functools.partial:
-        if name in self._client_commands_idx:
-            return functools.partial(
-                self.client_command, self._client_commands_idx[name]
-            )
-        elif name in self._server_commands_idx:
-            return functools.partial(self.command, self._server_commands_idx[name])
+        try:
+            cmd = getattr(self.ClientCommandDefs, name)
+        except AttributeError:
+            pass
         else:
-            raise AttributeError(f"No such command name: {name}")
+            return functools.partial(self.client_command, cmd.id)
 
-    def get(self, key: int | str, default: Any | None = None) -> Any:
-        """Get cached attribute."""
         try:
-            attr_def = self.find_attribute(key)
-        except KeyError:
-            return default
+            cmd = getattr(self.ServerCommandDefs, name)
+        except AttributeError:
+            pass
+        else:
+            return functools.partial(self.command, cmd.id)
+
+        raise AttributeError(f"No such command name: {name}")
 
+    def get(self, key: int | str, default: Any | None = None) -> Any:
+        """Get cached attribute."""
+        attr_def = self.find_attribute(key)
         return self._attr_cache.get(attr_def.id, default)
 
     def __getitem__(self, key: int | str) -> Any:
         """Return cached value of the attr."""
         return self._attr_cache[self.find_attribute(key).id]
 
     def __setitem__(self, key: int | str, value: Any) -> None:
@@ -810,15 +859,14 @@
 
     def general_command(
         self,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
         *args,
         manufacturer: int | t.uint16_t | None = None,
         expect_reply: bool = True,
-        tries: int = 1,
         tsn: int | t.uint8_t | None = None,
         **kwargs,
     ):
         command = foundation.GENERAL_COMMANDS[command_id]
 
         if command.direction == foundation.Direction.Client_to_Server:
             # should reply be retryable?
@@ -835,15 +883,14 @@
         return self.request(
             True,
             command.id,
             command.schema,
             *args,
             manufacturer=manufacturer,
             expect_reply=expect_reply,
-            tries=tries,
             tsn=tsn,
             **kwargs,
         )
 
     _configure_reporting = functools.partialmethod(
         general_command, foundation.GeneralCommand.Configure_Reporting
     )
@@ -935,16 +982,18 @@
 
 
 class ClusterPersistingListener:
     def __init__(self, applistener: PersistingListener, cluster: Cluster) -> None:
         self._applistener = applistener
         self._cluster = cluster
 
-    def attribute_updated(self, attrid: int | t.uint16_t, value: Any) -> None:
-        self._applistener.attribute_updated(self._cluster, attrid, value)
+    def attribute_updated(
+        self, attrid: int | t.uint16_t, value: Any, timestamp: datetime
+    ) -> None:
+        self._applistener.attribute_updated(self._cluster, attrid, value, timestamp)
 
     def cluster_command(self, *args, **kwargs) -> None:
         pass
 
     def general_command(self, *args, **kwargs) -> None:
         pass
```

### Comparing `zigpy-0.55.0/zigpy/zcl/clusters/__init__.py` & `zigpy-0.56.0/zigpy/zcl/clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy/zcl/clusters/general.py` & `zigpy-0.56.0/zigpy/zcl/clusters/general.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,953 +1,1164 @@
 """General Functional Domain"""
 
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Any
+from typing import Any, Final
 
 import zigpy.types as t
 from zigpy.typing import AddressingMode
 from zigpy.zcl import Cluster, foundation
-from zigpy.zcl.foundation import ZCLAttributeDef, ZCLCommandDef
+from zigpy.zcl.foundation import (
+    BaseAttributeDefs,
+    BaseCommandDefs,
+    ZCLAttributeDef,
+    ZCLCommandDef,
+)
+
+
+class PowerSource(t.enum8):
+    """Power source enum."""
+
+    Unknown = 0x00
+    Mains_single_phase = 0x01
+    Mains_three_phase = 0x02
+    Battery = 0x03
+    DC_Source = 0x04
+    Emergency_Mains_Always_On = 0x05
+    Emergency_Mains_Transfer_Switch = 0x06
+
+    def __init__(self, *args, **kwargs):
+        self.battery_backup = False
+
+    @classmethod
+    def deserialize(cls, data: bytes) -> tuple[bytes, bytes]:
+        val, data = t.uint8_t.deserialize(data)
+        r = cls(val & 0x7F)
+        r.battery_backup = bool(val & 0x80)
+        return r, data
+
+
+class PhysicalEnvironment(t.enum8):
+    Unspecified_environment = 0x00
+    # Mirror Capacity Available: for 0x0109 Profile Id only; use 0x71 moving forward
+    # Atrium: defined for legacy devices with non-0x0109 Profile Id; use 0x70 moving
+    #         forward
+
+    # Note: This value is deprecated for Profile Id 0x0104. The value 0x01 is
+    #       maintained for historical purposes and SHOULD only be used for backwards
+    #       compatibility with devices developed before this specification. The 0x01
+    #       value MUST be interpreted using the Profile Id of the endpoint upon
+    #       which it is implemented. For endpoints with the Smart Energy Profile Id
+    #       (0x0109) the value 0x01 has a meaning of Mirror. For endpoints with any
+    #       other profile identifier, the value 0x01 has a meaning of Atrium.
+    Mirror_or_atrium_legacy = 0x01
+    Bar = 0x02
+    Courtyard = 0x03
+    Bathroom = 0x04
+    Bedroom = 0x05
+    Billiard_Room = 0x06
+    Utility_Room = 0x07
+    Cellar = 0x08
+    Storage_Closet = 0x09
+    Theater = 0x0A
+    Office = 0x0B
+    Deck = 0x0C
+    Den = 0x0D
+    Dining_Room = 0x0E
+    Electrical_Room = 0x0F
+    Elevator = 0x10
+    Entry = 0x11
+    Family_Room = 0x12
+    Main_Floor = 0x13
+    Upstairs = 0x14
+    Downstairs = 0x15
+    Basement = 0x16
+    Gallery = 0x17
+    Game_Room = 0x18
+    Garage = 0x19
+    Gym = 0x1A
+    Hallway = 0x1B
+    House = 0x1C
+    Kitchen = 0x1D
+    Laundry_Room = 0x1E
+    Library = 0x1F
+    Master_Bedroom = 0x20
+    Mud_Room_small_room_for_coats_and_boots = 0x21
+    Nursery = 0x22
+    Pantry = 0x23
+    Office_2 = 0x24
+    Outside = 0x25
+    Pool = 0x26
+    Porch = 0x27
+    Sewing_Room = 0x28
+    Sitting_Room = 0x29
+    Stairway = 0x2A
+    Yard = 0x2B
+    Attic = 0x2C
+    Hot_Tub = 0x2D
+    Living_Room = 0x2E
+    Sauna = 0x2F
+    Workshop = 0x30
+    Guest_Bedroom = 0x31
+    Guest_Bath = 0x32
+    Back_Yard = 0x34
+    Front_Yard = 0x35
+    Patio = 0x36
+    Driveway = 0x37
+    Sun_Room = 0x38
+    Grand_Room = 0x39
+    Spa = 0x3A
+    Whirlpool = 0x3B
+    Shed = 0x3C
+    Equipment_Storage = 0x3D
+    Craft_Room = 0x3E
+    Fountain = 0x3F
+    Pond = 0x40
+    Reception_Room = 0x41
+    Breakfast_Room = 0x42
+    Nook = 0x43
+    Garden = 0x44
+    Balcony = 0x45
+    Panic_Room = 0x46
+    Terrace = 0x47
+    Roof = 0x48
+    Toilet = 0x49
+    Toilet_Main = 0x4A
+    Outside_Toilet = 0x4B
+    Shower_room = 0x4C
+    Study = 0x4D
+    Front_Garden = 0x4E
+    Back_Garden = 0x4F
+    Kettle = 0x50
+    Television = 0x51
+    Stove = 0x52
+    Microwave = 0x53
+    Toaster = 0x54
+    Vacuum = 0x55
+    Appliance = 0x56
+    Front_Door = 0x57
+    Back_Door = 0x58
+    Fridge_Door = 0x59
+    Medication_Cabinet_Door = 0x60
+    Wardrobe_Door = 0x61
+    Front_Cupboard_Door = 0x62
+    Other_Door = 0x63
+    Waiting_Room = 0x64
+    Triage_Room = 0x65
+    Doctors_Office = 0x66
+    Patients_Private_Room = 0x67
+    Consultation_Room = 0x68
+    Nurse_Station = 0x69
+    Ward = 0x6A
+    Corridor = 0x6B
+    Operating_Theatre = 0x6C
+    Dental_Surgery_Room = 0x6D
+    Medical_Imaging_Room = 0x6E
+    Decontamination_Room = 0x6F
+    Atrium = 0x70
+    Mirror = 0x71
+    Unknown_environment = 0xFF
+
+
+class AlarmMask(t.bitmap8):
+    General_hardware_fault = 0x01
+    General_software_fault = 0x02
+
+
+class DisableLocalConfig(t.bitmap8):
+    Reset = 0x01
+    Device_Configuration = 0x02
+
+
+class GenericDeviceClass(t.enum8):
+    Lighting = 0x00
+
+
+class GenericLightingDeviceType(t.enum8):
+    Incandescent = 0x00
+    Spotlight_Halogen = 0x01
+    Halogen_bulb = 0x02
+    CFL = 0x03
+    Linear_Fluorescent = 0x04
+    LED_bulb = 0x05
+    Spotlight_LED = 0x06
+    LED_strip = 0x07
+    LED_tube = 0x08
+    Generic_indoor_luminaire = 0x09
+    Generic_outdoor_luminaire = 0x0A
+    Pendant_luminaire = 0x0B
+    Floor_standing_luminaire = 0x0C
+    Generic_Controller = 0xE0
+    Wall_Switch = 0xE1
+    Portable_remote_controller = 0xE2
+    Motion_sensor = 0xE3
+    # 0xe4 to 0xef Reserved
+    Generic_actuator = 0xF0
+    Wall_socket = 0xF1
+    Gateway_Bridge = 0xF2
+    Plug_in_unit = 0xF3
+    Retrofit_actuator = 0xF4
+    Unspecified = 0xFF
 
 
 class Basic(Cluster):
     """Attributes for determining basic information about a
     device, setting user device information such as location,
     and enabling a device.
     """
 
-    class PowerSource(t.enum8):
-        """Power source enum."""
+    PowerSource: Final = PowerSource
+    PhysicalEnvironment: Final = PhysicalEnvironment
+    AlarmMask: Final = AlarmMask
+    DisableLocalConfig: Final = DisableLocalConfig
+    GenericDeviceClass: Final = GenericDeviceClass
+    GenericLightingDeviceType: Final = GenericLightingDeviceType
 
-        Unknown = 0x00
-        Mains_single_phase = 0x01
-        Mains_three_phase = 0x02
-        Battery = 0x03
-        DC_Source = 0x04
-        Emergency_Mains_Always_On = 0x05
-        Emergency_Mains_Transfer_Switch = 0x06
-
-        def __init__(self, *args, **kwargs):
-            self.battery_backup = False
-
-        @classmethod
-        def deserialize(cls, data: bytes) -> tuple[bytes, bytes]:
-            val, data = t.uint8_t.deserialize(data)
-            r = cls(val & 0x7F)
-            r.battery_backup = bool(val & 0x80)
-            return r, data
-
-    class PhysicalEnvironment(t.enum8):
-        Unspecified_environment = 0x00
-        # Mirror Capacity Available: for 0x0109 Profile Id only; use 0x71 moving forward
-        # Atrium: defined for legacy devices with non-0x0109 Profile Id; use 0x70 moving
-        #         forward
-
-        # Note: This value is deprecated for Profile Id 0x0104. The value 0x01 is
-        #       maintained for historical purposes and SHOULD only be used for backwards
-        #       compatibility with devices developed before this specification. The 0x01
-        #       value MUST be interpreted using the Profile Id of the endpoint upon
-        #       which it is implemented. For endpoints with the Smart Energy Profile Id
-        #       (0x0109) the value 0x01 has a meaning of Mirror. For endpoints with any
-        #       other profile identifier, the value 0x01 has a meaning of Atrium.
-        Mirror_or_atrium_legacy = 0x01
-        Bar = 0x02
-        Courtyard = 0x03
-        Bathroom = 0x04
-        Bedroom = 0x05
-        Billiard_Room = 0x06
-        Utility_Room = 0x07
-        Cellar = 0x08
-        Storage_Closet = 0x09
-        Theater = 0x0A
-        Office = 0x0B
-        Deck = 0x0C
-        Den = 0x0D
-        Dining_Room = 0x0E
-        Electrical_Room = 0x0F
-        Elevator = 0x10
-        Entry = 0x11
-        Family_Room = 0x12
-        Main_Floor = 0x13
-        Upstairs = 0x14
-        Downstairs = 0x15
-        Basement = 0x16
-        Gallery = 0x17
-        Game_Room = 0x18
-        Garage = 0x19
-        Gym = 0x1A
-        Hallway = 0x1B
-        House = 0x1C
-        Kitchen = 0x1D
-        Laundry_Room = 0x1E
-        Library = 0x1F
-        Master_Bedroom = 0x20
-        Mud_Room_small_room_for_coats_and_boots = 0x21
-        Nursery = 0x22
-        Pantry = 0x23
-        Office_2 = 0x24
-        Outside = 0x25
-        Pool = 0x26
-        Porch = 0x27
-        Sewing_Room = 0x28
-        Sitting_Room = 0x29
-        Stairway = 0x2A
-        Yard = 0x2B
-        Attic = 0x2C
-        Hot_Tub = 0x2D
-        Living_Room = 0x2E
-        Sauna = 0x2F
-        Workshop = 0x30
-        Guest_Bedroom = 0x31
-        Guest_Bath = 0x32
-        Back_Yard = 0x34
-        Front_Yard = 0x35
-        Patio = 0x36
-        Driveway = 0x37
-        Sun_Room = 0x38
-        Grand_Room = 0x39
-        Spa = 0x3A
-        Whirlpool = 0x3B
-        Shed = 0x3C
-        Equipment_Storage = 0x3D
-        Craft_Room = 0x3E
-        Fountain = 0x3F
-        Pond = 0x40
-        Reception_Room = 0x41
-        Breakfast_Room = 0x42
-        Nook = 0x43
-        Garden = 0x44
-        Balcony = 0x45
-        Panic_Room = 0x46
-        Terrace = 0x47
-        Roof = 0x48
-        Toilet = 0x49
-        Toilet_Main = 0x4A
-        Outside_Toilet = 0x4B
-        Shower_room = 0x4C
-        Study = 0x4D
-        Front_Garden = 0x4E
-        Back_Garden = 0x4F
-        Kettle = 0x50
-        Television = 0x51
-        Stove = 0x52
-        Microwave = 0x53
-        Toaster = 0x54
-        Vacuum = 0x55
-        Appliance = 0x56
-        Front_Door = 0x57
-        Back_Door = 0x58
-        Fridge_Door = 0x59
-        Medication_Cabinet_Door = 0x60
-        Wardrobe_Door = 0x61
-        Front_Cupboard_Door = 0x62
-        Other_Door = 0x63
-        Waiting_Room = 0x64
-        Triage_Room = 0x65
-        Doctors_Office = 0x66
-        Patients_Private_Room = 0x67
-        Consultation_Room = 0x68
-        Nurse_Station = 0x69
-        Ward = 0x6A
-        Corridor = 0x6B
-        Operating_Theatre = 0x6C
-        Dental_Surgery_Room = 0x6D
-        Medical_Imaging_Room = 0x6E
-        Decontamination_Room = 0x6F
-        Atrium = 0x70
-        Mirror = 0x71
-        Unknown_environment = 0xFF
-
-    class AlarmMask(t.bitmap8):
-        General_hardware_fault = 0x01
-        General_software_fault = 0x02
-
-    class DisableLocalConfig(t.bitmap8):
-        Reset = 0x01
-        Device_Configuration = 0x02
-
-    class GenericDeviceClass(t.enum8):
-        Lighting = 0x00
-
-    class GenericLightingDeviceType(t.enum8):
-        Incandescent = 0x00
-        Spotlight_Halogen = 0x01
-        Halogen_bulb = 0x02
-        CFL = 0x03
-        Linear_Fluorescent = 0x04
-        LED_bulb = 0x05
-        Spotlight_LED = 0x06
-        LED_strip = 0x07
-        LED_tube = 0x08
-        Generic_indoor_luminaire = 0x09
-        Generic_outdoor_luminaire = 0x0A
-        Pendant_luminaire = 0x0B
-        Floor_standing_luminaire = 0x0C
-        Generic_Controller = 0xE0
-        Wall_Switch = 0xE1
-        Portable_remote_controller = 0xE2
-        Motion_sensor = 0xE3
-        # 0xe4 to 0xef Reserved
-        Generic_actuator = 0xF0
-        Wall_socket = 0xF1
-        Gateway_Bridge = 0xF2
-        Plug_in_unit = 0xF3
-        Retrofit_actuator = 0xF4
-        Unspecified = 0xFF
-
-    cluster_id = 0x0000
-    ep_attribute = "basic"
-    attributes: dict[int, ZCLAttributeDef] = {
+    cluster_id: Final = 0x0000
+    ep_attribute: Final = "basic"
+
+    class AttributeDefs(BaseAttributeDefs):
         # Basic Device Information
-        0x0000: ZCLAttributeDef(
-            "zcl_version", type=t.uint8_t, access="r", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef("app_version", type=t.uint8_t, access="r"),
-        0x0002: ZCLAttributeDef("stack_version", type=t.uint8_t, access="r"),
-        0x0003: ZCLAttributeDef("hw_version", type=t.uint8_t, access="r"),
-        0x0004: ZCLAttributeDef(
-            "manufacturer", type=t.LimitedCharString(32), access="r"
-        ),
-        0x0005: ZCLAttributeDef("model", type=t.LimitedCharString(32), access="r"),
-        0x0006: ZCLAttributeDef("date_code", type=t.LimitedCharString(16), access="r"),
-        0x0007: ZCLAttributeDef(
-            "power_source", type=PowerSource, access="r", mandatory=True
-        ),
-        0x0008: ZCLAttributeDef(
-            "generic_device_class", type=GenericDeviceClass, access="r"
-        ),
+        zcl_version: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint8_t, access="r", mandatory=True
+        )
+        app_version: Final = ZCLAttributeDef(id=0x0001, type=t.uint8_t, access="r")
+        stack_version: Final = ZCLAttributeDef(id=0x0002, type=t.uint8_t, access="r")
+        hw_version: Final = ZCLAttributeDef(id=0x0003, type=t.uint8_t, access="r")
+        manufacturer: Final = ZCLAttributeDef(
+            id=0x0004, type=t.LimitedCharString(32), access="r"
+        )
+        model: Final = ZCLAttributeDef(
+            id=0x0005, type=t.LimitedCharString(32), access="r"
+        )
+        date_code: Final = ZCLAttributeDef(
+            id=0x0006, type=t.LimitedCharString(16), access="r"
+        )
+        power_source: Final = ZCLAttributeDef(
+            id=0x0007, type=PowerSource, access="r", mandatory=True
+        )
+        generic_device_class: Final = ZCLAttributeDef(
+            id=0x0008, type=GenericDeviceClass, access="r"
+        )
         # Lighting is the only non-reserved device type
-        0x0009: ZCLAttributeDef(
-            "generic_device_type", type=GenericLightingDeviceType, access="r"
-        ),
-        0x000A: ZCLAttributeDef("product_code", type=t.LVBytes, access="r"),
-        0x000B: ZCLAttributeDef("product_url", type=t.CharacterString, access="r"),
-        0x000C: ZCLAttributeDef(
-            "manufacturer_version_details", type=t.CharacterString, access="r"
-        ),
-        0x000D: ZCLAttributeDef("serial_number", type=t.CharacterString, access="r"),
-        0x000E: ZCLAttributeDef("product_label", type=t.CharacterString, access="r"),
+        generic_device_type: Final = ZCLAttributeDef(
+            id=0x0009, type=GenericLightingDeviceType, access="r"
+        )
+        product_code: Final = ZCLAttributeDef(id=0x000A, type=t.LVBytes, access="r")
+        product_url: Final = ZCLAttributeDef(
+            id=0x000B, type=t.CharacterString, access="r"
+        )
+        manufacturer_version_details: Final = ZCLAttributeDef(
+            id=0x000C, type=t.CharacterString, access="r"
+        )
+        serial_number: Final = ZCLAttributeDef(
+            id=0x000D, type=t.CharacterString, access="r"
+        )
+        product_label: Final = ZCLAttributeDef(
+            id=0x000E, type=t.CharacterString, access="r"
+        )
         # Basic Device Settings
-        0x0010: ZCLAttributeDef(
-            "location_desc", type=t.LimitedCharString(16), access="rw"
-        ),
-        0x0011: ZCLAttributeDef("physical_env", type=PhysicalEnvironment, access="rw"),
-        0x0012: ZCLAttributeDef("device_enabled", type=t.Bool, access="rw"),
-        0x0013: ZCLAttributeDef("alarm_mask", type=AlarmMask, access="rw"),
-        0x0014: ZCLAttributeDef(
-            "disable_local_config", type=DisableLocalConfig, access="rw"
-        ),
-        0x4000: ZCLAttributeDef("sw_build_id", type=t.CharacterString, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef("reset_fact_default", {}, False)
-    }
-    client_commands: dict[int, ZCLCommandDef] = {}
+        location_desc: Final = ZCLAttributeDef(
+            id=0x0010, type=t.LimitedCharString(16), access="rw"
+        )
+        physical_env: Final = ZCLAttributeDef(
+            id=0x0011, type=PhysicalEnvironment, access="rw"
+        )
+        device_enabled: Final = ZCLAttributeDef(id=0x0012, type=t.Bool, access="rw")
+        alarm_mask: Final = ZCLAttributeDef(id=0x0013, type=AlarmMask, access="rw")
+        disable_local_config: Final = ZCLAttributeDef(
+            id=0x0014, type=DisableLocalConfig, access="rw"
+        )
+        sw_build_id: Final = ZCLAttributeDef(
+            id=0x4000, type=t.CharacterString, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        reset_fact_default: Final = ZCLCommandDef(id=0x00, schema={}, direction=False)
+
+
+class MainsAlarmMask(t.bitmap8):
+    Voltage_Too_Low = 0b00000001
+    Voltage_Too_High = 0b00000010
+    Power_Supply_Unavailable = 0b00000100
+
+
+class BatterySize(t.enum8):
+    No_battery = 0x00
+    Built_in = 0x01
+    Other = 0x02
+    AA = 0x03
+    AAA = 0x04
+    C = 0x05
+    D = 0x06
+    CR2 = 0x07
+    CR123A = 0x08
+    Unknown = 0xFF
 
 
 class PowerConfiguration(Cluster):
     """Attributes for determining more detailed information
     about a device’s power source(s), and for configuring
     under/over voltage alarms.
     """
 
-    class MainsAlarmMask(t.bitmap8):
-        Voltage_Too_Low = 0b00000001
-        Voltage_Too_High = 0b00000010
-        Power_Supply_Unavailable = 0b00000100
-
-    class BatterySize(t.enum8):
-        No_battery = 0x00
-        Built_in = 0x01
-        Other = 0x02
-        AA = 0x03
-        AAA = 0x04
-        C = 0x05
-        D = 0x06
-        CR2 = 0x07
-        CR123A = 0x08
-        Unknown = 0xFF
-
-    cluster_id = 0x0001
-    name = "Power Configuration"
-    ep_attribute = "power"
-    attributes: dict[int, ZCLAttributeDef] = {
+    MainsAlarmMask: Final = MainsAlarmMask
+    BatterySize: Final = BatterySize
+
+    cluster_id: Final = 0x0001
+    name: Final = "Power Configuration"
+    ep_attribute: Final = "power"
+
+    class AttributeDefs(BaseAttributeDefs):
         # Mains Information
-        0x0000: ZCLAttributeDef("mains_voltage", type=t.uint16_t, access="r"),
-        0x0001: ZCLAttributeDef("mains_frequency", type=t.uint8_t, access="r"),
+        mains_voltage: Final = ZCLAttributeDef(id=0x0000, type=t.uint16_t, access="r")
+        mains_frequency: Final = ZCLAttributeDef(id=0x0001, type=t.uint8_t, access="r")
         # Mains Settings
-        0x0010: ZCLAttributeDef("mains_alarm_mask", type=MainsAlarmMask, access="rw"),
-        0x0011: ZCLAttributeDef("mains_volt_min_thres", type=t.uint16_t, access="rw"),
-        0x0012: ZCLAttributeDef("mains_volt_max_thres", type=t.uint16_t, access="rw"),
-        0x0013: ZCLAttributeDef(
-            "mains_voltage_dwell_trip_point", type=t.uint16_t, access="rw"
-        ),
+        mains_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0010, type=MainsAlarmMask, access="rw"
+        )
+        mains_volt_min_thres: Final = ZCLAttributeDef(
+            id=0x0011, type=t.uint16_t, access="rw"
+        )
+        mains_volt_max_thres: Final = ZCLAttributeDef(
+            id=0x0012, type=t.uint16_t, access="rw"
+        )
+        mains_voltage_dwell_trip_point: Final = ZCLAttributeDef(
+            id=0x0013, type=t.uint16_t, access="rw"
+        )
         # Battery Information
-        0x0020: ZCLAttributeDef("battery_voltage", type=t.uint8_t, access="r"),
-        0x0021: ZCLAttributeDef(
-            "battery_percentage_remaining", type=t.uint8_t, access="rp"
-        ),
+        battery_voltage: Final = ZCLAttributeDef(id=0x0020, type=t.uint8_t, access="r")
+        battery_percentage_remaining: Final = ZCLAttributeDef(
+            id=0x0021, type=t.uint8_t, access="rp"
+        )
         # Battery Settings
-        0x0030: ZCLAttributeDef(
-            "battery_manufacturer", type=t.LimitedCharString(16), access="rw"
-        ),
-        0x0031: ZCLAttributeDef("battery_size", type=BatterySize, access="rw"),
-        0x0032: ZCLAttributeDef(
-            "battery_a_hr_rating", type=t.uint16_t, access="rw"
-        ),  # measured in units of 10mAHr
-        0x0033: ZCLAttributeDef("battery_quantity", type=t.uint8_t, access="rw"),
-        0x0034: ZCLAttributeDef(
-            "battery_rated_voltage", type=t.uint8_t, access="rw"
-        ),  # measured in units of 100mV
-        0x0035: ZCLAttributeDef("battery_alarm_mask", type=t.bitmap8, access="rw"),
-        0x0036: ZCLAttributeDef("battery_volt_min_thres", type=t.uint8_t, access="rw"),
-        0x0037: ZCLAttributeDef("battery_volt_thres1", type=t.uint16_t, access="r*w"),
-        0x0038: ZCLAttributeDef("battery_volt_thres2", type=t.uint16_t, access="r*w"),
-        0x0039: ZCLAttributeDef("battery_volt_thres3", type=t.uint16_t, access="r*w"),
-        0x003A: ZCLAttributeDef(
-            "battery_percent_min_thres", type=t.uint8_t, access="r*w"
-        ),
-        0x003B: ZCLAttributeDef("battery_percent_thres1", type=t.uint8_t, access="r*w"),
-        0x003C: ZCLAttributeDef("battery_percent_thres2", type=t.uint8_t, access="r*w"),
-        0x003D: ZCLAttributeDef("battery_percent_thres3", type=t.uint8_t, access="r*w"),
-        0x003E: ZCLAttributeDef("battery_alarm_state", type=t.bitmap32, access="rp"),
+        battery_manufacturer: Final = ZCLAttributeDef(
+            id=0x0030, type=t.LimitedCharString(16), access="rw"
+        )
+        battery_size: Final = ZCLAttributeDef(id=0x0031, type=BatterySize, access="rw")
+        battery_a_hr_rating: Final = ZCLAttributeDef(
+            id=0x0032, type=t.uint16_t, access="rw"
+        )
+        # measured in units of 10mAHr
+        battery_quantity: Final = ZCLAttributeDef(
+            id=0x0033, type=t.uint8_t, access="rw"
+        )
+        battery_rated_voltage: Final = ZCLAttributeDef(
+            id=0x0034, type=t.uint8_t, access="rw"
+        )
+        # measured in units of 100mV
+        battery_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0035, type=t.bitmap8, access="rw"
+        )
+        battery_volt_min_thres: Final = ZCLAttributeDef(
+            id=0x0036, type=t.uint8_t, access="rw"
+        )
+        battery_volt_thres1: Final = ZCLAttributeDef(
+            id=0x0037, type=t.uint16_t, access="r*w"
+        )
+        battery_volt_thres2: Final = ZCLAttributeDef(
+            id=0x0038, type=t.uint16_t, access="r*w"
+        )
+        battery_volt_thres3: Final = ZCLAttributeDef(
+            id=0x0039, type=t.uint16_t, access="r*w"
+        )
+        battery_percent_min_thres: Final = ZCLAttributeDef(
+            id=0x003A, type=t.uint8_t, access="r*w"
+        )
+        battery_percent_thres1: Final = ZCLAttributeDef(
+            id=0x003B, type=t.uint8_t, access="r*w"
+        )
+        battery_percent_thres2: Final = ZCLAttributeDef(
+            id=0x003C, type=t.uint8_t, access="r*w"
+        )
+        battery_percent_thres3: Final = ZCLAttributeDef(
+            id=0x003D, type=t.uint8_t, access="r*w"
+        )
+        battery_alarm_state: Final = ZCLAttributeDef(
+            id=0x003E, type=t.bitmap32, access="rp"
+        )
         # Battery 2 Information
-        0x0040: ZCLAttributeDef("battery_2_voltage", type=t.uint8_t, access="r"),
-        0x0041: ZCLAttributeDef(
-            "battery_2_percentage_remaining", type=t.uint8_t, access="rp"
-        ),
+        battery_2_voltage: Final = ZCLAttributeDef(
+            id=0x0040, type=t.uint8_t, access="r"
+        )
+        battery_2_percentage_remaining: Final = ZCLAttributeDef(
+            id=0x0041, type=t.uint8_t, access="rp"
+        )
         # Battery 2 Settings
-        0x0050: ZCLAttributeDef(
-            "battery_2_manufacturer", type=t.CharacterString, access="rw"
-        ),
-        0x0051: ZCLAttributeDef("battery_2_size", type=BatterySize, access="rw"),
-        0x0052: ZCLAttributeDef("battery_2_a_hr_rating", type=t.uint16_t, access="rw"),
-        0x0053: ZCLAttributeDef("battery_2_quantity", type=t.uint8_t, access="rw"),
-        0x0054: ZCLAttributeDef("battery_2_rated_voltage", type=t.uint8_t, access="rw"),
-        0x0055: ZCLAttributeDef("battery_2_alarm_mask", type=t.bitmap8, access="rw"),
-        0x0056: ZCLAttributeDef(
-            "battery_2_volt_min_thres", type=t.uint8_t, access="rw"
-        ),
-        0x0057: ZCLAttributeDef("battery_2_volt_thres1", type=t.uint16_t, access="r*w"),
-        0x0058: ZCLAttributeDef("battery_2_volt_thres2", type=t.uint16_t, access="r*w"),
-        0x0059: ZCLAttributeDef("battery_2_volt_thres3", type=t.uint16_t, access="r*w"),
-        0x005A: ZCLAttributeDef(
-            "battery_2_percent_min_thres", type=t.uint8_t, access="r*w"
-        ),
-        0x005B: ZCLAttributeDef(
-            "battery_2_percent_thres1", type=t.uint8_t, access="r*w"
-        ),
-        0x005C: ZCLAttributeDef(
-            "battery_2_percent_thres2", type=t.uint8_t, access="r*w"
-        ),
-        0x005D: ZCLAttributeDef(
-            "battery_2_percent_thres3", type=t.uint8_t, access="r*w"
-        ),
-        0x005E: ZCLAttributeDef("battery_2_alarm_state", type=t.bitmap32, access="rp"),
+        battery_2_manufacturer: Final = ZCLAttributeDef(
+            id=0x0050, type=t.CharacterString, access="rw"
+        )
+        battery_2_size: Final = ZCLAttributeDef(
+            id=0x0051, type=BatterySize, access="rw"
+        )
+        battery_2_a_hr_rating: Final = ZCLAttributeDef(
+            id=0x0052, type=t.uint16_t, access="rw"
+        )
+        battery_2_quantity: Final = ZCLAttributeDef(
+            id=0x0053, type=t.uint8_t, access="rw"
+        )
+        battery_2_rated_voltage: Final = ZCLAttributeDef(
+            id=0x0054, type=t.uint8_t, access="rw"
+        )
+        battery_2_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0055, type=t.bitmap8, access="rw"
+        )
+        battery_2_volt_min_thres: Final = ZCLAttributeDef(
+            id=0x0056, type=t.uint8_t, access="rw"
+        )
+        battery_2_volt_thres1: Final = ZCLAttributeDef(
+            id=0x0057, type=t.uint16_t, access="r*w"
+        )
+        battery_2_volt_thres2: Final = ZCLAttributeDef(
+            id=0x0058, type=t.uint16_t, access="r*w"
+        )
+        battery_2_volt_thres3: Final = ZCLAttributeDef(
+            id=0x0059, type=t.uint16_t, access="r*w"
+        )
+        battery_2_percent_min_thres: Final = ZCLAttributeDef(
+            id=0x005A, type=t.uint8_t, access="r*w"
+        )
+        battery_2_percent_thres1: Final = ZCLAttributeDef(
+            id=0x005B, type=t.uint8_t, access="r*w"
+        )
+        battery_2_percent_thres2: Final = ZCLAttributeDef(
+            id=0x005C, type=t.uint8_t, access="r*w"
+        )
+        battery_2_percent_thres3: Final = ZCLAttributeDef(
+            id=0x005D, type=t.uint8_t, access="r*w"
+        )
+        battery_2_alarm_state: Final = ZCLAttributeDef(
+            id=0x005E, type=t.bitmap32, access="rp"
+        )
         # Battery 3 Information
-        0x0060: ZCLAttributeDef("battery_3_voltage", type=t.uint8_t, access="r"),
-        0x0061: ZCLAttributeDef(
-            "battery_3_percentage_remaining", type=t.uint8_t, access="rp"
-        ),
+        battery_3_voltage: Final = ZCLAttributeDef(
+            id=0x0060, type=t.uint8_t, access="r"
+        )
+        battery_3_percentage_remaining: Final = ZCLAttributeDef(
+            id=0x0061, type=t.uint8_t, access="rp"
+        )
         # Battery 3 Settings
-        0x0070: ZCLAttributeDef(
-            "battery_3_manufacturer", type=t.CharacterString, access="rw"
-        ),
-        0x0071: ZCLAttributeDef("battery_3_size", type=BatterySize, access="rw"),
-        0x0072: ZCLAttributeDef("battery_3_a_hr_rating", type=t.uint16_t, access="rw"),
-        0x0073: ZCLAttributeDef("battery_3_quantity", type=t.uint8_t, access="rw"),
-        0x0074: ZCLAttributeDef("battery_3_rated_voltage", type=t.uint8_t, access="rw"),
-        0x0075: ZCLAttributeDef("battery_3_alarm_mask", type=t.bitmap8, access="rw"),
-        0x0076: ZCLAttributeDef(
-            "battery_3_volt_min_thres", type=t.uint8_t, access="rw"
-        ),
-        0x0077: ZCLAttributeDef("battery_3_volt_thres1", type=t.uint16_t, access="r*w"),
-        0x0078: ZCLAttributeDef("battery_3_volt_thres2", type=t.uint16_t, access="r*w"),
-        0x0079: ZCLAttributeDef("battery_3_volt_thres3", type=t.uint16_t, access="r*w"),
-        0x007A: ZCLAttributeDef(
-            "battery_3_percent_min_thres", type=t.uint8_t, access="r*w"
-        ),
-        0x007B: ZCLAttributeDef(
-            "battery_3_percent_thres1", type=t.uint8_t, access="r*w"
-        ),
-        0x007C: ZCLAttributeDef(
-            "battery_3_percent_thres2", type=t.uint8_t, access="r*w"
-        ),
-        0x007D: ZCLAttributeDef(
-            "battery_3_percent_thres3", type=t.uint8_t, access="r*w"
-        ),
-        0x007E: ZCLAttributeDef("battery_3_alarm_state", type=t.bitmap32, access="rp"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        battery_3_manufacturer: Final = ZCLAttributeDef(
+            id=0x0070, type=t.CharacterString, access="rw"
+        )
+        battery_3_size: Final = ZCLAttributeDef(
+            id=0x0071, type=BatterySize, access="rw"
+        )
+        battery_3_a_hr_rating: Final = ZCLAttributeDef(
+            id=0x0072, type=t.uint16_t, access="rw"
+        )
+        battery_3_quantity: Final = ZCLAttributeDef(
+            id=0x0073, type=t.uint8_t, access="rw"
+        )
+        battery_3_rated_voltage: Final = ZCLAttributeDef(
+            id=0x0074, type=t.uint8_t, access="rw"
+        )
+        battery_3_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0075, type=t.bitmap8, access="rw"
+        )
+        battery_3_volt_min_thres: Final = ZCLAttributeDef(
+            id=0x0076, type=t.uint8_t, access="rw"
+        )
+        battery_3_volt_thres1: Final = ZCLAttributeDef(
+            id=0x0077, type=t.uint16_t, access="r*w"
+        )
+        battery_3_volt_thres2: Final = ZCLAttributeDef(
+            id=0x0078, type=t.uint16_t, access="r*w"
+        )
+        battery_3_volt_thres3: Final = ZCLAttributeDef(
+            id=0x0079, type=t.uint16_t, access="r*w"
+        )
+        battery_3_percent_min_thres: Final = ZCLAttributeDef(
+            id=0x007A, type=t.uint8_t, access="r*w"
+        )
+        battery_3_percent_thres1: Final = ZCLAttributeDef(
+            id=0x007B, type=t.uint8_t, access="r*w"
+        )
+        battery_3_percent_thres2: Final = ZCLAttributeDef(
+            id=0x007C, type=t.uint8_t, access="r*w"
+        )
+        battery_3_percent_thres3: Final = ZCLAttributeDef(
+            id=0x007D, type=t.uint8_t, access="r*w"
+        )
+        battery_3_alarm_state: Final = ZCLAttributeDef(
+            id=0x007E, type=t.bitmap32, access="rp"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+
+class DeviceTempAlarmMask(t.bitmap8):
+    Temp_too_low = 0b00000001
+    Temp_too_high = 0b00000010
 
 
 class DeviceTemperature(Cluster):
     """Attributes for determining information about a device’s
     internal temperature, and for configuring under/over
     temperature alarms.
     """
 
-    class DeviceTempAlarmMask(t.bitmap8):
-        Temp_too_low = 0b00000001
-        Temp_too_high = 0b00000010
-
-    cluster_id = 0x0002
-    name = "Device Temperature"
-    ep_attribute = "device_temperature"
-    attributes: dict[int, ZCLAttributeDef] = {
+    DeviceTempAlarmMask: Final = DeviceTempAlarmMask
+
+    cluster_id: Final = 0x0002
+    name: Final = "Device Temperature"
+    ep_attribute: Final = "device_temperature"
+
+    class AttributeDefs(BaseAttributeDefs):
         # Device Temperature Information
-        0x0000: ZCLAttributeDef(
-            "current_temperature", type=t.int16s, access="r", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef("min_temp_experienced", type=t.int16s, access="r"),
-        0x0002: ZCLAttributeDef("max_temp_experienced", type=t.int16s, access="r"),
-        0x0003: ZCLAttributeDef("over_temp_total_dwell", type=t.uint16_t, access="r"),
+        current_temperature: Final = ZCLAttributeDef(
+            id=0x0000, type=t.int16s, access="r", mandatory=True
+        )
+        min_temp_experienced: Final = ZCLAttributeDef(
+            id=0x0001, type=t.int16s, access="r"
+        )
+        max_temp_experienced: Final = ZCLAttributeDef(
+            id=0x0002, type=t.int16s, access="r"
+        )
+        over_temp_total_dwell: Final = ZCLAttributeDef(
+            id=0x0003, type=t.uint16_t, access="r"
+        )
         # Device Temperature Settings
-        0x0010: ZCLAttributeDef(
-            "dev_temp_alarm_mask", type=DeviceTempAlarmMask, access="rw"
-        ),
-        0x0011: ZCLAttributeDef("low_temp_thres", type=t.int16s, access="rw"),
-        0x0012: ZCLAttributeDef("high_temp_thres", type=t.int16s, access="rw"),
-        0x0013: ZCLAttributeDef(
-            "low_temp_dwell_trip_point", type=t.uint24_t, access="rw"
-        ),
-        0x0014: ZCLAttributeDef(
-            "high_temp_dwell_trip_point", type=t.uint24_t, access="rw"
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        dev_temp_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0010, type=DeviceTempAlarmMask, access="rw"
+        )
+        low_temp_thres: Final = ZCLAttributeDef(id=0x0011, type=t.int16s, access="rw")
+        high_temp_thres: Final = ZCLAttributeDef(id=0x0012, type=t.int16s, access="rw")
+        low_temp_dwell_trip_point: Final = ZCLAttributeDef(
+            id=0x0013, type=t.uint24_t, access="rw"
+        )
+        high_temp_dwell_trip_point: Final = ZCLAttributeDef(
+            id=0x0014, type=t.uint24_t, access="rw"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+
+class EffectIdentifier(t.enum8):
+    Blink = 0x00
+    Breathe = 0x01
+    Okay = 0x02
+    Channel_change = 0x03
+    Finish_effect = 0xFE
+    Stop_effect = 0xFF
+
+
+class EffectVariant(t.enum8):
+    Default = 0x00
 
 
 class Identify(Cluster):
     """Attributes and commands for putting a device into
     Identification mode (e.g. flashing a light)
     """
 
-    class EffectIdentifier(t.enum8):
-        Blink = 0x00
-        Breathe = 0x01
-        Okay = 0x02
-        Channel_change = 0x03
-        Finish_effect = 0xFE
-        Stop_effect = 0xFF
-
-    class EffectVariant(t.enum8):
-        Default = 0x00
-
-    cluster_id = 0x0003
-    ep_attribute = "identify"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "identify_time", type=t.uint16_t, access="rw", mandatory=True
-        ),
-        # 0x0001: ZCLAttributeDef("identify_commission_state", type=t.bitmap8),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef("identify", {"identify_time": t.uint16_t}, False),
-        0x01: ZCLCommandDef("identify_query", {}, False),
+    EffectIdentifier: Final = EffectIdentifier
+    EffectVariant: Final = EffectVariant
+
+    cluster_id: Final = 0x0003
+    ep_attribute: Final = "identify"
+
+    class AttributeDefs(BaseAttributeDefs):
+        identify_time: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint16_t, access="rw", mandatory=True
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        identify: Final = ZCLCommandDef(
+            id=0x00, schema={"identify_time": t.uint16_t}, direction=False
+        )
+        identify_query: Final = ZCLCommandDef(id=0x01, schema={}, direction=False)
         # 0x02: ("ezmode_invoke", (t.bitmap8,), False),
         # 0x03: ("update_commission_state", (t.bitmap8,), False),
-        0x40: ZCLCommandDef(
-            "trigger_effect",
-            {"effect_id": EffectIdentifier, "effect_variant": EffectVariant},
-            False,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef("identify_query_response", {"timeout": t.uint16_t}, True)
-    }
+        trigger_effect: Final = ZCLCommandDef(
+            id=0x40,
+            schema={"effect_id": EffectIdentifier, "effect_variant": EffectVariant},
+            direction=False,
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        identify_query_response: Final = ZCLCommandDef(
+            id=0x00, schema={"timeout": t.uint16_t}, direction=True
+        )
+
+
+class NameSupport(t.bitmap8):
+    Supported = 0b10000000
 
 
 class Groups(Cluster):
     """Attributes and commands for group configuration and
     manipulation.
     """
 
-    class NameSupport(t.bitmap8):
-        Supported = 0b10000000
+    NameSupport: Final = NameSupport
+
+    cluster_id: Final = 0x0004
+    ep_attribute: Final = "groups"
 
-    cluster_id = 0x0004
-    ep_attribute = "groups"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "name_support", type=NameSupport, access="r", mandatory=True
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "add",
-            {"group_id": t.Group, "group_name": t.LimitedCharString(16)},
-            False,
-        ),
-        0x01: ZCLCommandDef("view", {"group_id": t.Group}, False),
-        0x02: ZCLCommandDef("get_membership", {"groups": t.LVList[t.Group]}, False),
-        0x03: ZCLCommandDef("remove", {"group_id": t.Group}, False),
-        0x04: ZCLCommandDef("remove_all", {}, False),
-        0x05: ZCLCommandDef(
-            "add_if_identifying",
-            {"group_id": t.Group, "group_name": t.LimitedCharString(16)},
-            False,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "add_response",
-            {"status": foundation.Status, "group_id": t.Group},
-            True,
-        ),
-        0x01: ZCLCommandDef(
-            "view_response",
-            {
+    class AttributeDefs(BaseAttributeDefs):
+        name_support: Final = ZCLAttributeDef(
+            id=0x0000, type=NameSupport, access="r", mandatory=True
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        add: Final = ZCLCommandDef(
+            id=0x00,
+            schema={"group_id": t.Group, "group_name": t.LimitedCharString(16)},
+            direction=False,
+        )
+        view: Final = ZCLCommandDef(
+            id=0x01, schema={"group_id": t.Group}, direction=False
+        )
+        get_membership: Final = ZCLCommandDef(
+            id=0x02, schema={"groups": t.LVList[t.Group]}, direction=False
+        )
+        remove: Final = ZCLCommandDef(
+            id=0x03, schema={"group_id": t.Group}, direction=False
+        )
+        remove_all: Final = ZCLCommandDef(id=0x04, schema={}, direction=False)
+        add_if_identifying: Final = ZCLCommandDef(
+            id=0x05,
+            schema={"group_id": t.Group, "group_name": t.LimitedCharString(16)},
+            direction=False,
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        add_response: Final = ZCLCommandDef(
+            id=0x00,
+            schema={"status": foundation.Status, "group_id": t.Group},
+            direction=True,
+        )
+        view_response: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "status": foundation.Status,
                 "group_id": t.Group,
                 "group_name": t.LimitedCharString(16),
             },
-            True,
-        ),
-        0x02: ZCLCommandDef(
-            "get_membership_response",
-            {"capacity": t.uint8_t, "groups": t.LVList[t.Group]},
-            True,
-        ),
-        0x03: ZCLCommandDef(
-            "remove_response",
-            {"status": foundation.Status, "group_id": t.Group},
-            True,
-        ),
-    }
+            direction=True,
+        )
+        get_membership_response: Final = ZCLCommandDef(
+            id=0x02,
+            schema={"capacity": t.uint8_t, "groups": t.LVList[t.Group]},
+            direction=True,
+        )
+        remove_response: Final = ZCLCommandDef(
+            id=0x03,
+            schema={"status": foundation.Status, "group_id": t.Group},
+            direction=True,
+        )
 
 
 class Scenes(Cluster):
     """Attributes and commands for scene configuration and
     manipulation.
     """
 
-    class NameSupport(t.bitmap8):
-        Supported = 0b10000000
+    NameSupport: Final = NameSupport
+
+    cluster_id: Final = 0x0005
+    ep_attribute: Final = "scenes"
 
-    cluster_id = 0x0005
-    ep_attribute = "scenes"
-    attributes: dict[int, ZCLAttributeDef] = {
+    class AttributeDefs(BaseAttributeDefs):
         # Scene Management Information
-        0x0000: ZCLAttributeDef("count", type=t.uint8_t, access="r", mandatory=True),
-        0x0001: ZCLAttributeDef(
-            "current_scene", type=t.uint8_t, access="r", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef(
-            "current_group", type=t.uint16_t, access="r", mandatory=True
-        ),
-        0x0003: ZCLAttributeDef("scene_valid", type=t.Bool, access="r", mandatory=True),
-        0x0004: ZCLAttributeDef(
-            "name_support", type=NameSupport, access="r", mandatory=True
-        ),
-        0x0005: ZCLAttributeDef("last_configured_by", type=t.EUI64, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "add",
-            {
+        count: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint8_t, access="r", mandatory=True
+        )
+        current_scene: Final = ZCLAttributeDef(
+            id=0x0001, type=t.uint8_t, access="r", mandatory=True
+        )
+        current_group: Final = ZCLAttributeDef(
+            id=0x0002, type=t.uint16_t, access="r", mandatory=True
+        )
+        scene_valid: Final = ZCLAttributeDef(
+            id=0x0003, type=t.Bool, access="r", mandatory=True
+        )
+        name_support: Final = ZCLAttributeDef(
+            id=0x0004, type=NameSupport, access="r", mandatory=True
+        )
+        last_configured_by: Final = ZCLAttributeDef(id=0x0005, type=t.EUI64, access="r")
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        add: Final = ZCLCommandDef(
+            id=0x00,
+            schema={
                 "group_id": t.Group,
                 "scene_id": t.uint8_t,
                 "transition_time": t.uint16_t,
                 "scene_name": t.LimitedCharString(16),
             },
-            False,
-        ),  # TODO: + extension field sets
-        0x01: ZCLCommandDef(
-            "view", {"group_id": t.Group, "scene_id": t.uint8_t}, False
-        ),
-        0x02: ZCLCommandDef(
-            "remove", {"group_id": t.Group, "scene_id": t.uint8_t}, False
-        ),
-        0x03: ZCLCommandDef("remove_all", {"group_id": t.Group}, False),
-        0x04: ZCLCommandDef(
-            "store", {"group_id": t.Group, "scene_id": t.uint8_t}, False
-        ),
-        0x05: ZCLCommandDef(
-            "recall",
-            {
+            direction=False,
+        )
+        # TODO: + extension field sets
+        view: Final = ZCLCommandDef(
+            id=0x01,
+            schema={"group_id": t.Group, "scene_id": t.uint8_t},
+            direction=False,
+        )
+        remove: Final = ZCLCommandDef(
+            id=0x02,
+            schema={"group_id": t.Group, "scene_id": t.uint8_t},
+            direction=False,
+        )
+        remove_all: Final = ZCLCommandDef(
+            id=0x03, schema={"group_id": t.Group}, direction=False
+        )
+        store: Final = ZCLCommandDef(
+            id=0x04,
+            schema={"group_id": t.Group, "scene_id": t.uint8_t},
+            direction=False,
+        )
+        recall: Final = ZCLCommandDef(
+            id=0x05,
+            schema={
                 "group_id": t.Group,
                 "scene_id": t.uint8_t,
                 "transition_time?": t.uint16_t,
             },
-            False,
-        ),
-        0x06: ZCLCommandDef("get_scene_membership", {"group_id": t.Group}, False),
-        0x40: ZCLCommandDef(
-            "enhanced_add",
-            {
+            direction=False,
+        )
+        get_scene_membership: Final = ZCLCommandDef(
+            id=0x06, schema={"group_id": t.Group}, direction=False
+        )
+        enhanced_add: Final = ZCLCommandDef(
+            id=0x40,
+            schema={
                 "group_id": t.Group,
                 "scene_id": t.uint8_t,
                 "transition_time": t.uint16_t,
                 "scene_name": t.LimitedCharString(16),
             },
-            False,
-        ),
-        0x41: ZCLCommandDef(
-            "enhanced_view", {"group_id": t.Group, "scene_id": t.uint8_t}, False
-        ),
-        0x42: ZCLCommandDef(
-            "copy",
-            {
+            direction=False,
+        )
+        enhanced_view: Final = ZCLCommandDef(
+            id=0x41,
+            schema={"group_id": t.Group, "scene_id": t.uint8_t},
+            direction=False,
+        )
+        copy: Final = ZCLCommandDef(
+            id=0x42,
+            schema={
                 "mode": t.uint8_t,
                 "group_id_from": t.uint16_t,
                 "scene_id_from": t.uint8_t,
                 "group_id_to": t.uint16_t,
                 "scene_id_to": t.uint8_t,
             },
-            False,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "add_scene_response",
-            {"status": foundation.Status, "group_id": t.Group, "scene_id": t.uint8_t},
-            True,
-        ),
-        0x01: ZCLCommandDef(
-            "view_response",
-            {
+            direction=False,
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        add_scene_response: Final = ZCLCommandDef(
+            id=0x00,
+            schema={
+                "status": foundation.Status,
+                "group_id": t.Group,
+                "scene_id": t.uint8_t,
+            },
+            direction=True,
+        )
+        view_response: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "status": foundation.Status,
                 "group_id": t.Group,
                 "scene_id": t.uint8_t,
                 "transition_time?": t.uint16_t,
                 "scene_name?": t.LimitedCharString(16),
             },
-            True,
-        ),  # TODO: + extension field sets
-        0x02: ZCLCommandDef(
-            "remove_scene_response",
-            {"status": foundation.Status, "group_id": t.Group, "scene_id": t.uint8_t},
-            True,
-        ),
-        0x03: ZCLCommandDef(
-            "remove_all_scenes_response",
-            {"status": foundation.Status, "group_id": t.Group},
-            True,
-        ),
-        0x04: ZCLCommandDef(
-            "store_scene_response",
-            {"status": foundation.Status, "group_id": t.Group, "scene_id": t.uint8_t},
-            True,
-        ),
-        0x06: ZCLCommandDef(
-            "get_scene_membership_response",
-            {
+            direction=True,
+        )
+        # TODO: + extension field sets
+        remove_scene_response: Final = ZCLCommandDef(
+            id=0x02,
+            schema={
+                "status": foundation.Status,
+                "group_id": t.Group,
+                "scene_id": t.uint8_t,
+            },
+            direction=True,
+        )
+        remove_all_scenes_response: Final = ZCLCommandDef(
+            id=0x03,
+            schema={"status": foundation.Status, "group_id": t.Group},
+            direction=True,
+        )
+        store_scene_response: Final = ZCLCommandDef(
+            id=0x04,
+            schema={
+                "status": foundation.Status,
+                "group_id": t.Group,
+                "scene_id": t.uint8_t,
+            },
+            direction=True,
+        )
+        get_scene_membership_response: Final = ZCLCommandDef(
+            id=0x06,
+            schema={
                 "status": foundation.Status,
                 "capacity": t.uint8_t,
                 "group_id": t.Group,
                 "scenes?": t.LVList[t.uint8_t],
             },
-            True,
-        ),
-        0x40: ZCLCommandDef(
-            "enhanced_add_response",
-            {"status": foundation.Status, "group_id": t.Group, "scene_id": t.uint8_t},
-            True,
-        ),
-        0x41: ZCLCommandDef(
-            "enhanced_view_response",
-            {
+            direction=True,
+        )
+        enhanced_add_response: Final = ZCLCommandDef(
+            id=0x40,
+            schema={
+                "status": foundation.Status,
+                "group_id": t.Group,
+                "scene_id": t.uint8_t,
+            },
+            direction=True,
+        )
+        enhanced_view_response: Final = ZCLCommandDef(
+            id=0x41,
+            schema={
                 "status": foundation.Status,
                 "group_id": t.Group,
                 "scene_id": t.uint8_t,
                 "transition_time?": t.uint16_t,
                 "scene_name?": t.LimitedCharString(16),
             },
-            True,
-        ),  # TODO: + extension field sets
-        0x42: ZCLCommandDef(
-            "copy_response",
-            {"status": foundation.Status, "group_id": t.Group, "scene_id": t.uint8_t},
-            True,
-        ),
-    }
+            direction=True,
+        )
+        # TODO: + extension field sets
+        copy_response: Final = ZCLCommandDef(
+            id=0x42,
+            schema={
+                "status": foundation.Status,
+                "group_id": t.Group,
+                "scene_id": t.uint8_t,
+            },
+            direction=True,
+        )
+
+
+class StartUpOnOff(t.enum8):
+    Off = 0x00
+    On = 0x01
+    Toggle = 0x02
+    PreviousValue = 0xFF
+
+
+class OffEffectIdentifier(t.enum8):
+    Delayed_All_Off = 0x00
+    Dying_Light = 0x01
+
+
+class OnOffControl(t.bitmap8):
+    Accept_Only_When_On = 0b00000001
 
 
 class OnOff(Cluster):
     """Attributes and commands for switching devices between
     ‘On’ and ‘Off’ states.
     """
 
-    class StartUpOnOff(t.enum8):
-        Off = 0x00
-        On = 0x01
-        Toggle = 0x02
-        PreviousValue = 0xFF
-
-    class OffEffectIdentifier(t.enum8):
-        Delayed_All_Off = 0x00
-        Dying_Light = 0x01
-
-    class OnOffControl(t.bitmap8):
-        Accept_Only_When_On = 0b00000001
+    StartUpOnOff: Final = StartUpOnOff
+    OffEffectIdentifier: Final = OffEffectIdentifier
+    OnOffControl: Final = OnOffControl
 
     DELAYED_ALL_OFF_FADE_TO_OFF = 0x00
     DELAYED_ALL_OFF_NO_FADE = 0x01
     DELAYED_ALL_OFF_DIM_THEN_FADE_TO_OFF = 0x02
 
     DYING_LIGHT_DIM_UP_THEN_FADE_TO_OFF = 0x00
 
-    cluster_id = 0x0006
-    name = "On/Off"
-    ep_attribute = "on_off"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef("on_off", type=t.Bool, access="rps", mandatory=True),
-        0x4000: ZCLAttributeDef("global_scene_control", type=t.Bool, access="r"),
-        0x4001: ZCLAttributeDef("on_time", type=t.uint16_t, access="rw"),
-        0x4002: ZCLAttributeDef("off_wait_time", type=t.uint16_t, access="rw"),
-        0x4003: ZCLAttributeDef("start_up_on_off", type=StartUpOnOff, access="rw"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef("off", {}, False),
-        0x01: ZCLCommandDef("on", {}, False),
-        0x02: ZCLCommandDef("toggle", {}, False),
-        0x40: ZCLCommandDef(
-            "off_with_effect",
-            {"effect_id": OffEffectIdentifier, "effect_variant": t.uint8_t},
-            False,
-        ),
-        0x41: ZCLCommandDef("on_with_recall_global_scene", {}, False),
-        0x42: ZCLCommandDef(
-            "on_with_timed_off",
-            {
+    cluster_id: Final = 0x0006
+    name: Final = "On/Off"
+    ep_attribute: Final = "on_off"
+
+    class AttributeDefs(BaseAttributeDefs):
+        on_off: Final = ZCLAttributeDef(
+            id=0x0000, type=t.Bool, access="rps", mandatory=True
+        )
+        global_scene_control: Final = ZCLAttributeDef(
+            id=0x4000, type=t.Bool, access="r"
+        )
+        on_time: Final = ZCLAttributeDef(id=0x4001, type=t.uint16_t, access="rw")
+        off_wait_time: Final = ZCLAttributeDef(id=0x4002, type=t.uint16_t, access="rw")
+        start_up_on_off: Final = ZCLAttributeDef(
+            id=0x4003, type=StartUpOnOff, access="rw"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        off: Final = ZCLCommandDef(id=0x00, schema={}, direction=False)
+        on: Final = ZCLCommandDef(id=0x01, schema={}, direction=False)
+        toggle: Final = ZCLCommandDef(id=0x02, schema={}, direction=False)
+        off_with_effect: Final = ZCLCommandDef(
+            id=0x40,
+            schema={"effect_id": OffEffectIdentifier, "effect_variant": t.uint8_t},
+            direction=False,
+        )
+        on_with_recall_global_scene: Final = ZCLCommandDef(
+            id=0x41, schema={}, direction=False
+        )
+        on_with_timed_off: Final = ZCLCommandDef(
+            id=0x42,
+            schema={
                 "on_off_control": OnOffControl,
                 "on_time": t.uint16_t,
                 "off_wait_time": t.uint16_t,
             },
-            False,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {}
+            direction=False,
+        )
+
+
+class SwitchType(t.enum8):
+    Toggle = 0x00
+    Momentary = 0x01
+    Multifunction = 0x02
+
+
+class SwitchActions(t.enum8):
+    OnOff = 0x00
+    OffOn = 0x01
+    ToggleToggle = 0x02
 
 
 class OnOffConfiguration(Cluster):
     """Attributes and commands for configuring On/Off switching devices"""
 
-    class SwitchType(t.enum8):
-        Toggle = 0x00
-        Momentary = 0x01
-        Multifunction = 0x02
-
-    class SwitchActions(t.enum8):
-        OnOff = 0x00
-        OffOn = 0x01
-        ToggleToggle = 0x02
-
-    cluster_id = 0x0007
-    name = "On/Off Switch Configuration"
-    ep_attribute = "on_off_config"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "switch_type", type=SwitchType, access="r", mandatory=True
-        ),
-        0x0010: ZCLAttributeDef(
-            "switch_actions", type=SwitchActions, access="rw", mandatory=True
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    SwitchType: Final = SwitchType
+    SwitchActions: Final = SwitchActions
+
+    cluster_id: Final = 0x0007
+    name: Final = "On/Off Switch Configuration"
+    ep_attribute: Final = "on_off_config"
+
+    class AttributeDefs(BaseAttributeDefs):
+        switch_type: Final = ZCLAttributeDef(
+            id=0x0000, type=SwitchType, access="r", mandatory=True
+        )
+        switch_actions: Final = ZCLAttributeDef(
+            id=0x0010, type=SwitchActions, access="rw", mandatory=True
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+
+class MoveMode(t.enum8):
+    Up = 0x00
+    Down = 0x01
+
+
+class StepMode(t.enum8):
+    Up = 0x00
+    Down = 0x01
+
+
+class Options(t.bitmap8):
+    Execute_if_off = 0b00000001
+    Couple_color_temp_to_level = 0b00000010
 
 
 class LevelControl(Cluster):
     """Attributes and commands for controlling devices that
     can be set to a level between fully ‘On’ and fully ‘Off’.
     """
 
-    class MoveMode(t.enum8):
-        Up = 0x00
-        Down = 0x01
-
-    class StepMode(t.enum8):
-        Up = 0x00
-        Down = 0x01
-
-    class Options(t.bitmap8):
-        Execute_if_off = 0b00000001
-        Couple_color_temp_to_level = 0b00000010
-
-    cluster_id = 0x0008
-    name = "Level control"
-    ep_attribute = "level"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "current_level", type=t.uint8_t, access="rps", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef("remaining_time", type=t.uint16_t, access="r"),
-        0x0002: ZCLAttributeDef("min_level", type=t.uint8_t, access="r"),
-        0x0003: ZCLAttributeDef("max_level", type=t.uint8_t, access="r"),
-        0x0004: ZCLAttributeDef("current_frequency", type=t.uint16_t, access="rps"),
-        0x0005: ZCLAttributeDef("min_frequency", type=t.uint16_t, access="r"),
-        0x0006: ZCLAttributeDef("max_frequency", type=t.uint16_t, access="r"),
-        0x000F: ZCLAttributeDef("options", type=t.bitmap8, access="rw"),
-        0x0010: ZCLAttributeDef("on_off_transition_time", type=t.uint16_t, access="rw"),
-        0x0011: ZCLAttributeDef("on_level", type=t.uint8_t, access="rw"),
-        0x0012: ZCLAttributeDef("on_transition_time", type=t.uint16_t, access="rw"),
-        0x0013: ZCLAttributeDef("off_transition_time", type=t.uint16_t, access="rw"),
-        0x0014: ZCLAttributeDef("default_move_rate", type=t.uint8_t, access="rw"),
-        0x4000: ZCLAttributeDef("start_up_current_level", type=t.uint8_t, access="rw"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "move_to_level",
-            {
+    MoveMode: Final = MoveMode
+    StepMode: Final = StepMode
+    Options: Final = Options
+
+    cluster_id: Final = 0x0008
+    name: Final = "Level control"
+    ep_attribute: Final = "level"
+
+    class AttributeDefs(BaseAttributeDefs):
+        current_level: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint8_t, access="rps", mandatory=True
+        )
+        remaining_time: Final = ZCLAttributeDef(id=0x0001, type=t.uint16_t, access="r")
+        min_level: Final = ZCLAttributeDef(id=0x0002, type=t.uint8_t, access="r")
+        max_level: Final = ZCLAttributeDef(id=0x0003, type=t.uint8_t, access="r")
+        current_frequency: Final = ZCLAttributeDef(
+            id=0x0004, type=t.uint16_t, access="rps"
+        )
+        min_frequency: Final = ZCLAttributeDef(id=0x0005, type=t.uint16_t, access="r")
+        max_frequency: Final = ZCLAttributeDef(id=0x0006, type=t.uint16_t, access="r")
+        options: Final = ZCLAttributeDef(id=0x000F, type=t.bitmap8, access="rw")
+        on_off_transition_time: Final = ZCLAttributeDef(
+            id=0x0010, type=t.uint16_t, access="rw"
+        )
+        on_level: Final = ZCLAttributeDef(id=0x0011, type=t.uint8_t, access="rw")
+        on_transition_time: Final = ZCLAttributeDef(
+            id=0x0012, type=t.uint16_t, access="rw"
+        )
+        off_transition_time: Final = ZCLAttributeDef(
+            id=0x0013, type=t.uint16_t, access="rw"
+        )
+        default_move_rate: Final = ZCLAttributeDef(
+            id=0x0014, type=t.uint8_t, access="rw"
+        )
+        start_up_current_level: Final = ZCLAttributeDef(
+            id=0x4000, type=t.uint8_t, access="rw"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        move_to_level: Final = ZCLCommandDef(
+            id=0x00,
+            schema={
                 "level": t.uint8_t,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x01: ZCLCommandDef(
-            "move",
-            {
+            direction=False,
+        )
+        move: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "move_mode": MoveMode,
                 "rate": t.uint8_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x02: ZCLCommandDef(
-            "step",
-            {
+            direction=False,
+        )
+        step: Final = ZCLCommandDef(
+            id=0x02,
+            schema={
                 "step_mode": StepMode,
                 "step_size": t.uint8_t,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x03: ZCLCommandDef(
-            "stop",
-            {
+            direction=False,
+        )
+        stop: Final = ZCLCommandDef(
+            id=0x03,
+            schema={
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x04: ZCLCommandDef(
-            "move_to_level_with_on_off",
-            {"level": t.uint8_t, "transition_time": t.uint16_t},
-            False,
-        ),
-        0x05: ZCLCommandDef(
-            "move_with_on_off", {"move_mode": MoveMode, "rate": t.uint8_t}, False
-        ),
-        0x06: ZCLCommandDef(
-            "step_with_on_off",
-            {
+            direction=False,
+        )
+        move_to_level_with_on_off: Final = ZCLCommandDef(
+            id=0x04,
+            schema={"level": t.uint8_t, "transition_time": t.uint16_t},
+            direction=False,
+        )
+        move_with_on_off: Final = ZCLCommandDef(
+            id=0x05,
+            schema={"move_mode": MoveMode, "rate": t.uint8_t},
+            direction=False,
+        )
+        step_with_on_off: Final = ZCLCommandDef(
+            id=0x06,
+            schema={
                 "step_mode": StepMode,
                 "step_size": t.uint8_t,
                 "transition_time": t.uint16_t,
             },
-            False,
-        ),
-        0x07: ZCLCommandDef("stop_with_on_off", {}, False),
-        0x08: ZCLCommandDef(
-            "move_to_closest_frequency", {"frequency": t.uint16_t}, False
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {}
+            direction=False,
+        )
+        stop_with_on_off: Final = ZCLCommandDef(id=0x07, schema={}, direction=False)
+        move_to_closest_frequency: Final = ZCLCommandDef(
+            id=0x08, schema={"frequency": t.uint16_t}, direction=False
+        )
 
 
 class Alarms(Cluster):
     """Attributes and commands for sending notifications and
     configuring alarm functionality.
     """
 
-    cluster_id = 0x0009
-    ep_attribute = "alarms"
-    attributes: dict[int, ZCLAttributeDef] = {
-        # Alarm Information
-        0x0000: ZCLAttributeDef("alarm_count", type=t.uint16_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "reset_alarm", {"alarm_code": t.uint8_t, "cluster_id": t.uint16_t}, False
-        ),
-        0x01: ZCLCommandDef("reset_all_alarms", {}, False),
-        0x02: ZCLCommandDef("get_alarm", {}, False),
-        0x03: ZCLCommandDef("reset_alarm_log", {}, False),
+    cluster_id: Final = 0x0009
+    ep_attribute: Final = "alarms"
+
+    class AttributeDefs(BaseAttributeDefs):
+        alarm_count: Final = ZCLAttributeDef(id=0x0000, type=t.uint16_t, access="r")
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        reset_alarm: Final = ZCLCommandDef(
+            id=0x00,
+            schema={"alarm_code": t.uint8_t, "cluster_id": t.uint16_t},
+            direction=False,
+        )
+        reset_all_alarms: Final = ZCLCommandDef(id=0x01, schema={}, direction=False)
+        get_alarm: Final = ZCLCommandDef(id=0x02, schema={}, direction=False)
+        reset_alarm_log: Final = ZCLCommandDef(id=0x03, schema={}, direction=False)
         # 0x04: ("publish_event_log", {}, False),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "alarm", {"alarm_code": t.uint8_t, "cluster_id": t.uint16_t}, False
-        ),
-        0x01: ZCLCommandDef(
-            "get_alarm_response",
-            {
+
+    class ClientCommandDefs(BaseCommandDefs):
+        alarm: Final = ZCLCommandDef(
+            id=0x00,
+            schema={"alarm_code": t.uint8_t, "cluster_id": t.uint16_t},
+            direction=False,
+        )
+        get_alarm_response: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "status": foundation.Status,
                 "alarm_code?": t.uint8_t,
                 "cluster_id?": t.uint16_t,
                 "timestamp?": t.uint32_t,
             },
-            True,
-        ),
+            direction=True,
+        )
         # 0x02: ("get_event_log", {}, False),
-    }
+
+
+class TimeStatus(t.bitmap8):
+    Master = 0b00000001
+    Synchronized = 0b00000010
+    Master_for_Zone_and_DST = 0b00000100
+    Superseding = 0b00001000
 
 
 class Time(Cluster):
     """Attributes and commands that provide a basic interface
     to a real-time clock.
     """
 
-    class TimeStatus(t.bitmap8):
-        Master = 0b00000001
-        Synchronized = 0b00000010
-        Master_for_Zone_and_DST = 0b00000100
-        Superseding = 0b00001000
-
-    cluster_id = 0x000A
-    ep_attribute = "time"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef("time", type=t.UTCTime, access="r*w", mandatory=True),
-        0x0001: ZCLAttributeDef(
-            "time_status", type=t.bitmap8, access="r*w", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef("time_zone", type=t.int32s, access="rw"),
-        0x0003: ZCLAttributeDef("dst_start", type=t.uint32_t, access="rw"),
-        0x0004: ZCLAttributeDef("dst_end", type=t.uint32_t, access="rw"),
-        0x0005: ZCLAttributeDef("dst_shift", type=t.int32s, access="rw"),
-        0x0006: ZCLAttributeDef("standard_time", type=t.StandardTime, access="r"),
-        0x0007: ZCLAttributeDef("local_time", type=t.LocalTime, access="r"),
-        0x0008: ZCLAttributeDef("last_set_time", type=t.UTCTime, access="r"),
-        0x0009: ZCLAttributeDef("valid_until_time", type=t.UTCTime, access="rw"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    TimeStatus: Final = TimeStatus
+
+    cluster_id: Final = 0x000A
+    ep_attribute: Final = "time"
+
+    class AttributeDefs(BaseAttributeDefs):
+        time: Final = ZCLAttributeDef(
+            id=0x0000, type=t.UTCTime, access="r*w", mandatory=True
+        )
+        time_status: Final = ZCLAttributeDef(
+            id=0x0001, type=t.bitmap8, access="r*w", mandatory=True
+        )
+        time_zone: Final = ZCLAttributeDef(id=0x0002, type=t.int32s, access="rw")
+        dst_start: Final = ZCLAttributeDef(id=0x0003, type=t.uint32_t, access="rw")
+        dst_end: Final = ZCLAttributeDef(id=0x0004, type=t.uint32_t, access="rw")
+        dst_shift: Final = ZCLAttributeDef(id=0x0005, type=t.int32s, access="rw")
+        standard_time: Final = ZCLAttributeDef(
+            id=0x0006, type=t.StandardTime, access="r"
+        )
+        local_time: Final = ZCLAttributeDef(id=0x0007, type=t.LocalTime, access="r")
+        last_set_time: Final = ZCLAttributeDef(id=0x0008, type=t.UTCTime, access="r")
+        valid_until_time: Final = ZCLAttributeDef(
+            id=0x0009, type=t.UTCTime, access="rw"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
     def handle_cluster_general_request(
         self,
         hdr: foundation.ZCLHeader,
         *args: list[Any],
         dst_addressing: AddressingMode | None = None,
     ):
@@ -970,833 +1181,984 @@
                     diff = datetime.now() - epoch
                     data[attr] = diff.total_seconds()
                 else:
                     data[attr] = None
             self.create_catching_task(self.read_attributes_rsp(data, tsn=hdr.tsn))
 
 
+class LocationMethod(t.enum8):
+    Lateration = 0x00
+    Signposting = 0x01
+    RF_fingerprinting = 0x02
+    Out_of_band = 0x03
+    Centralized = 0x04
+
+
+class NeighborInfo(t.Struct):
+    neighbor: t.EUI64
+    x: t.int16s
+    y: t.int16s
+    z: t.int16s
+    rssi: t.int8s
+    num_measurements: t.uint8_t
+
+
 class RSSILocation(Cluster):
     """Attributes and commands that provide a means for
     exchanging location information and channel parameters
     among devices.
     """
 
-    cluster_id = 0x000B
-    ep_attribute = "rssi_location"
+    LocationMethod: Final = LocationMethod
+    NeighborInfo: Final = NeighborInfo
 
-    class LocationMethod(t.enum8):
-        Lateration = 0x00
-        Signposting = 0x01
-        RF_fingerprinting = 0x02
-        Out_of_band = 0x03
-        Centralized = 0x04
+    cluster_id: Final = 0x000B
+    ep_attribute: Final = "rssi_location"
 
-    attributes: dict[int, ZCLAttributeDef] = {
+    class AttributeDefs(BaseAttributeDefs):
         # Location Information
-        0x0000: ZCLAttributeDef("type", type=t.uint8_t, access="rw", mandatory=True),
-        0x0001: ZCLAttributeDef(
-            "method", type=LocationMethod, access="rw", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef("age", type=t.uint16_t, access="r"),
-        0x0003: ZCLAttributeDef("quality_measure", type=t.uint8_t, access="r"),
-        0x0004: ZCLAttributeDef("num_of_devices", type=t.uint8_t, access="r"),
+        type: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint8_t, access="rw", mandatory=True
+        )
+        method: Final = ZCLAttributeDef(
+            id=0x0001, type=LocationMethod, access="rw", mandatory=True
+        )
+        age: Final = ZCLAttributeDef(id=0x0002, type=t.uint16_t, access="r")
+        quality_measure: Final = ZCLAttributeDef(id=0x0003, type=t.uint8_t, access="r")
+        num_of_devices: Final = ZCLAttributeDef(id=0x0004, type=t.uint8_t, access="r")
         # Location Settings
-        0x0010: ZCLAttributeDef(
-            "coordinate1", type=t.int16s, access="rw", mandatory=True
-        ),
-        0x0011: ZCLAttributeDef(
-            "coordinate2", type=t.int16s, access="rw", mandatory=True
-        ),
-        0x0012: ZCLAttributeDef("coordinate3", type=t.int16s, access="rw"),
-        0x0013: ZCLAttributeDef("power", type=t.int16s, access="rw", mandatory=True),
-        0x0014: ZCLAttributeDef(
-            "path_loss_exponent", type=t.uint16_t, access="rw", mandatory=True
-        ),
-        0x0015: ZCLAttributeDef("reporting_period", type=t.uint16_t, access="rw"),
-        0x0016: ZCLAttributeDef("calculation_period", type=t.uint16_t, access="rw"),
-        0x0017: ZCLAttributeDef(
-            "number_rssi_measurements", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "set_absolute_location",
-            {
+        coordinate1: Final = ZCLAttributeDef(
+            id=0x0010, type=t.int16s, access="rw", mandatory=True
+        )
+        coordinate2: Final = ZCLAttributeDef(
+            id=0x0011, type=t.int16s, access="rw", mandatory=True
+        )
+        coordinate3: Final = ZCLAttributeDef(id=0x0012, type=t.int16s, access="rw")
+        power: Final = ZCLAttributeDef(
+            id=0x0013, type=t.int16s, access="rw", mandatory=True
+        )
+        path_loss_exponent: Final = ZCLAttributeDef(
+            id=0x0014, type=t.uint16_t, access="rw", mandatory=True
+        )
+        reporting_period: Final = ZCLAttributeDef(
+            id=0x0015, type=t.uint16_t, access="rw"
+        )
+        calculation_period: Final = ZCLAttributeDef(
+            id=0x0016, type=t.uint16_t, access="rw"
+        )
+        number_rssi_measurements: Final = ZCLAttributeDef(
+            id=0x0017, type=t.uint8_t, access="rw", mandatory=True
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        set_absolute_location: Final = ZCLCommandDef(
+            id=0x00,
+            schema={
                 "coordinate1": t.int16s,
                 "coordinate2": t.int16s,
                 "coordinate3": t.int16s,
                 "power": t.int16s,
                 "path_loss_exponent": t.uint16_t,
             },
-            False,
-        ),
-        0x01: ZCLCommandDef(
-            "set_dev_config",
-            {
+            direction=False,
+        )
+        set_dev_config: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "power": t.int16s,
                 "path_loss_exponent": t.uint16_t,
                 "calculation_period": t.uint16_t,
                 "num_rssi_measurements": t.uint8_t,
                 "reporting_period": t.uint16_t,
             },
-            False,
-        ),
-        0x02: ZCLCommandDef("get_dev_config", {"target_addr": t.EUI64}, False),
-        0x03: ZCLCommandDef(
-            "get_location_data",
-            {"packed": t.bitmap8, "num_responses": t.uint8_t, "target_addr": t.EUI64},
-            False,
-        ),
-        0x04: ZCLCommandDef(
-            "rssi_response",
-            {
+            direction=False,
+        )
+        get_dev_config: Final = ZCLCommandDef(
+            id=0x02, schema={"target_addr": t.EUI64}, direction=False
+        )
+        get_location_data: Final = ZCLCommandDef(
+            id=0x03,
+            schema={
+                "packed": t.bitmap8,
+                "num_responses": t.uint8_t,
+                "target_addr": t.EUI64,
+            },
+            direction=False,
+        )
+        rssi_response: Final = ZCLCommandDef(
+            id=0x04,
+            schema={
                 "replying_device": t.EUI64,
                 "x": t.int16s,
                 "y": t.int16s,
                 "z": t.int16s,
                 "rssi": t.int8s,
                 "num_rssi_measurements": t.uint8_t,
             },
-            True,
-        ),
-        0x05: ZCLCommandDef(
-            "send_pings",
-            {
+            direction=True,
+        )
+        send_pings: Final = ZCLCommandDef(
+            id=0x05,
+            schema={
                 "target_addr": t.EUI64,
                 "num_rssi_measurements": t.uint8_t,
                 "calculation_period": t.uint16_t,
             },
-            False,
-        ),
-        0x06: ZCLCommandDef(
-            "anchor_node_announce",
-            {
+            direction=False,
+        )
+        anchor_node_announce: Final = ZCLCommandDef(
+            id=0x06,
+            schema={
                 "anchor_node_ieee_addr": t.EUI64,
                 "x": t.int16s,
                 "y": t.int16s,
                 "z": t.int16s,
             },
-            False,
-        ),
-    }
-
-    class NeighborInfo(t.Struct):
-        neighbor: t.EUI64
-        x: t.int16s
-        y: t.int16s
-        z: t.int16s
-        rssi: t.int8s
-        num_measurements: t.uint8_t
-
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "dev_config_response",
-            {
+            direction=False,
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        dev_config_response: Final = ZCLCommandDef(
+            id=0x00,
+            schema={
                 "status": foundation.Status,
                 "power?": t.int16s,
                 "path_loss_exponent?": t.uint16_t,
                 "calculation_period?": t.uint16_t,
                 "num_rssi_measurements?": t.uint8_t,
                 "reporting_period?": t.uint16_t,
             },
-            True,
-        ),
-        0x01: ZCLCommandDef(
-            "location_data_response",
-            {
+            direction=True,
+        )
+        location_data_response: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "status": foundation.Status,
                 "location_type?": t.uint8_t,
                 "coordinate1?": t.int16s,
                 "coordinate2?": t.int16s,
                 "coordinate3?": t.int16s,
                 "power?": t.uint16_t,
                 "path_loss_exponent?": t.uint8_t,
                 "location_method?": t.uint8_t,
                 "quality_measure?": t.uint8_t,
                 "location_age?": t.uint16_t,
             },
-            True,
-        ),
-        0x02: ZCLCommandDef("location_data_notification", {}, False),
-        0x03: ZCLCommandDef("compact_location_data_notification", {}, False),
-        0x04: ZCLCommandDef("rssi_ping", {"location_type": t.uint8_t}, False),  # data8
-        0x05: ZCLCommandDef("rssi_req", {}, False),
-        0x06: ZCLCommandDef(
-            "report_rssi_measurements",
-            {"measuring_device": t.EUI64, "neighbors": t.LVList[NeighborInfo]},
-            False,
-        ),
-        0x07: ZCLCommandDef(
-            "request_own_location", {"ieee_of_blind_node": t.EUI64}, False
-        ),
-    }
+            direction=True,
+        )
+        location_data_notification: Final = ZCLCommandDef(
+            id=0x02, schema={}, direction=False
+        )
+        compact_location_data_notification: Final = ZCLCommandDef(
+            id=0x03, schema={}, direction=False
+        )
+        rssi_ping: Final = ZCLCommandDef(
+            id=0x04, schema={"location_type": t.uint8_t}, direction=False
+        )
+        rssi_req: Final = ZCLCommandDef(id=0x05, schema={}, direction=False)
+        report_rssi_measurements: Final = ZCLCommandDef(
+            id=0x06,
+            schema={
+                "measuring_device": t.EUI64,
+                "neighbors": t.LVList[NeighborInfo],
+            },
+            direction=False,
+        )
+        request_own_location: Final = ZCLCommandDef(
+            id=0x07, schema={"ieee_of_blind_node": t.EUI64}, direction=False
+        )
+
+
+class Reliability(t.enum8):
+    No_fault_detected = 0
+    No_sensor = 1
+    Over_range = 2
+    Under_range = 3
+    Open_loop = 4
+    Shorted_loop = 5
+    No_output = 6
+    Unreliable_other = 7
+    Process_error = 8
+    Multi_state_fault = 9
+    Configuration_error = 10
 
 
 class AnalogInput(Cluster):
-    cluster_id = 0x000C
-    ep_attribute = "analog_input"
+    Reliability: Final = Reliability
+
+    cluster_id: Final = 0x000C
+    ep_attribute: Final = "analog_input"
 
-    class Reliability(t.enum8):
-        No_fault_detected = 0
-        No_sensor = 1
-        Over_range = 2
-        Under_range = 3
-        Open_loop = 4
-        Shorted_loop = 5
-        No_output = 6
-        Unreliable_other = 7
-        Process_error = 8
-        Multi_state_fault = 9
-        Configuration_error = 10
-
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x001C: ZCLAttributeDef("description", type=t.CharacterString, access="r*w"),
-        0x0041: ZCLAttributeDef("max_present_value", type=t.Single, access="r*w"),
-        0x0045: ZCLAttributeDef("min_present_value", type=t.Single, access="r*w"),
-        0x0051: ZCLAttributeDef(
-            "out_of_service", type=t.Bool, access="r*w", mandatory=True
-        ),
-        0x0055: ZCLAttributeDef(
-            "present_value", type=t.Single, access="rwp", mandatory=True
-        ),
-        0x0067: ZCLAttributeDef("reliability", type=Reliability, access="r*w"),
-        0x006A: ZCLAttributeDef("resolution", type=t.Single, access="r*w"),
-        0x006F: ZCLAttributeDef(
-            "status_flags", type=t.bitmap8, access="rp", mandatory=True
-        ),
-        0x0075: ZCLAttributeDef("engineering_units", type=t.enum16, access="r*w"),
-        0x0100: ZCLAttributeDef("application_type", type=t.uint32_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    class AttributeDefs(BaseAttributeDefs):
+        description: Final = ZCLAttributeDef(
+            id=0x001C, type=t.CharacterString, access="r*w"
+        )
+        max_present_value: Final = ZCLAttributeDef(
+            id=0x0041, type=t.Single, access="r*w"
+        )
+        min_present_value: Final = ZCLAttributeDef(
+            id=0x0045, type=t.Single, access="r*w"
+        )
+        out_of_service: Final = ZCLAttributeDef(
+            id=0x0051, type=t.Bool, access="r*w", mandatory=True
+        )
+        present_value: Final = ZCLAttributeDef(
+            id=0x0055, type=t.Single, access="rwp", mandatory=True
+        )
+        reliability: Final = ZCLAttributeDef(id=0x0067, type=Reliability, access="r*w")
+        resolution: Final = ZCLAttributeDef(id=0x006A, type=t.Single, access="r*w")
+        status_flags: Final = ZCLAttributeDef(
+            id=0x006F, type=t.bitmap8, access="rp", mandatory=True
+        )
+        engineering_units: Final = ZCLAttributeDef(
+            id=0x0075, type=t.enum16, access="r*w"
+        )
+        application_type: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint32_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class AnalogOutput(Cluster):
-    cluster_id = 0x000D
-    ep_attribute = "analog_output"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x001C: ZCLAttributeDef("description", type=t.CharacterString, access="r*w"),
-        0x0041: ZCLAttributeDef("max_present_value", type=t.Single, access="r*w"),
-        0x0045: ZCLAttributeDef("min_present_value", type=t.Single, access="r*w"),
-        0x0051: ZCLAttributeDef(
-            "out_of_service", type=t.Bool, access="r*w", mandatory=True
-        ),
-        0x0055: ZCLAttributeDef(
-            "present_value", type=t.Single, access="rwp", mandatory=True
-        ),
+    cluster_id: Final = 0x000D
+    ep_attribute: Final = "analog_output"
+
+    class AttributeDefs(BaseAttributeDefs):
+        description: Final = ZCLAttributeDef(
+            id=0x001C, type=t.CharacterString, access="r*w"
+        )
+        max_present_value: Final = ZCLAttributeDef(
+            id=0x0041, type=t.Single, access="r*w"
+        )
+        min_present_value: Final = ZCLAttributeDef(
+            id=0x0045, type=t.Single, access="r*w"
+        )
+        out_of_service: Final = ZCLAttributeDef(
+            id=0x0051, type=t.Bool, access="r*w", mandatory=True
+        )
+        present_value: Final = ZCLAttributeDef(
+            id=0x0055, type=t.Single, access="rwp", mandatory=True
+        )
         # 0x0057: ZCLAttributeDef('priority_array', type=TODO.array),  # Array of 16 structures of (boolean,
         # single precision)
-        0x0067: ZCLAttributeDef("reliability", type=t.enum8, access="r*w"),
-        0x0068: ZCLAttributeDef("relinquish_default", type=t.Single, access="r*w"),
-        0x006A: ZCLAttributeDef("resolution", type=t.Single, access="r*w"),
-        0x006F: ZCLAttributeDef(
-            "status_flags", type=t.bitmap8, access="rp", mandatory=True
-        ),
-        0x0075: ZCLAttributeDef("engineering_units", type=t.enum16, access="r*w"),
-        0x0100: ZCLAttributeDef("application_type", type=t.uint32_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        reliability: Final = ZCLAttributeDef(id=0x0067, type=t.enum8, access="r*w")
+        relinquish_default: Final = ZCLAttributeDef(
+            id=0x0068, type=t.Single, access="r*w"
+        )
+        resolution: Final = ZCLAttributeDef(id=0x006A, type=t.Single, access="r*w")
+        status_flags: Final = ZCLAttributeDef(
+            id=0x006F, type=t.bitmap8, access="rp", mandatory=True
+        )
+        engineering_units: Final = ZCLAttributeDef(
+            id=0x0075, type=t.enum16, access="r*w"
+        )
+        application_type: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint32_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class AnalogValue(Cluster):
-    cluster_id = 0x000E
-    ep_attribute = "analog_value"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x001C: ZCLAttributeDef("description", type=t.CharacterString, access="r*w"),
-        0x0051: ZCLAttributeDef(
-            "out_of_service", type=t.Bool, access="r*w", mandatory=True
-        ),
-        0x0055: ZCLAttributeDef(
-            "present_value", type=t.Single, access="rw", mandatory=True
-        ),
+    cluster_id: Final = 0x000E
+    ep_attribute: Final = "analog_value"
+
+    class AttributeDefs(BaseAttributeDefs):
+        description: Final = ZCLAttributeDef(
+            id=0x001C, type=t.CharacterString, access="r*w"
+        )
+        out_of_service: Final = ZCLAttributeDef(
+            id=0x0051, type=t.Bool, access="r*w", mandatory=True
+        )
+        present_value: Final = ZCLAttributeDef(
+            id=0x0055, type=t.Single, access="rw", mandatory=True
+        )
         # 0x0057: ('priority_array', TODO.array),  # Array of 16 structures of (boolean,
         # single precision)
-        0x0067: ZCLAttributeDef("reliability", type=t.enum8, access="r*w"),
-        0x0068: ZCLAttributeDef("relinquish_default", type=t.Single, access="r*w"),
-        0x006F: ZCLAttributeDef(
-            "status_flags", type=t.bitmap8, access="r", mandatory=True
-        ),
-        0x0075: ZCLAttributeDef("engineering_units", type=t.enum16, access="r*w"),
-        0x0100: ZCLAttributeDef("application_type", type=t.uint32_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        reliability: Final = ZCLAttributeDef(id=0x0067, type=t.enum8, access="r*w")
+        relinquish_default: Final = ZCLAttributeDef(
+            id=0x0068, type=t.Single, access="r*w"
+        )
+        status_flags: Final = ZCLAttributeDef(
+            id=0x006F, type=t.bitmap8, access="r", mandatory=True
+        )
+        engineering_units: Final = ZCLAttributeDef(
+            id=0x0075, type=t.enum16, access="r*w"
+        )
+        application_type: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint32_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class BinaryInput(Cluster):
-    cluster_id = 0x000F
-    name = "Binary Input (Basic)"
-    ep_attribute = "binary_input"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0004: ZCLAttributeDef("active_text", type=t.CharacterString, access="r*w"),
-        0x001C: ZCLAttributeDef("description", type=t.CharacterString, access="r*w"),
-        0x002E: ZCLAttributeDef("inactive_text", type=t.CharacterString, access="r*w"),
-        0x0051: ZCLAttributeDef(
-            "out_of_service", type=t.Bool, access="r*w", mandatory=True
-        ),
-        0x0054: ZCLAttributeDef("polarity", type=t.enum8, access="r"),
-        0x0055: ZCLAttributeDef(
-            "present_value", type=t.Bool, access="r*w", mandatory=True
-        ),
-        0x0067: ZCLAttributeDef("reliability", type=t.enum8, access="r*w"),
-        0x006F: ZCLAttributeDef(
-            "status_flags", type=t.bitmap8, access="r", mandatory=True
-        ),
-        0x0100: ZCLAttributeDef("application_type", type=t.uint32_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x000F
+    name: Final = "Binary Input (Basic)"
+    ep_attribute: Final = "binary_input"
+
+    class AttributeDefs(BaseAttributeDefs):
+        active_text: Final = ZCLAttributeDef(
+            id=0x0004, type=t.CharacterString, access="r*w"
+        )
+        description: Final = ZCLAttributeDef(
+            id=0x001C, type=t.CharacterString, access="r*w"
+        )
+        inactive_text: Final = ZCLAttributeDef(
+            id=0x002E, type=t.CharacterString, access="r*w"
+        )
+        out_of_service: Final = ZCLAttributeDef(
+            id=0x0051, type=t.Bool, access="r*w", mandatory=True
+        )
+        polarity: Final = ZCLAttributeDef(id=0x0054, type=t.enum8, access="r")
+        present_value: Final = ZCLAttributeDef(
+            id=0x0055, type=t.Bool, access="r*w", mandatory=True
+        )
+        reliability: Final = ZCLAttributeDef(id=0x0067, type=t.enum8, access="r*w")
+        status_flags: Final = ZCLAttributeDef(
+            id=0x006F, type=t.bitmap8, access="r", mandatory=True
+        )
+        application_type: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint32_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class BinaryOutput(Cluster):
-    cluster_id = 0x0010
-    ep_attribute = "binary_output"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0004: ZCLAttributeDef("active_text", type=t.CharacterString, access="r*w"),
-        0x001C: ZCLAttributeDef("description", type=t.CharacterString, access="r*w"),
-        0x002E: ZCLAttributeDef("inactive_text", type=t.CharacterString, access="r*w"),
-        0x0042: ZCLAttributeDef("minimum_off_time", type=t.uint32_t, access="r*w"),
-        0x0043: ZCLAttributeDef("minimum_on_time", type=t.uint32_t, access="r*w"),
-        0x0051: ZCLAttributeDef(
-            "out_of_service", type=t.Bool, access="r*w", mandatory=True
-        ),
-        0x0054: ZCLAttributeDef("polarity", type=t.enum8, access="r"),
-        0x0055: ZCLAttributeDef(
-            "present_value", type=t.Bool, access="r*w", mandatory=True
-        ),
+    cluster_id: Final = 0x0010
+    ep_attribute: Final = "binary_output"
+
+    class AttributeDefs(BaseAttributeDefs):
+        active_text: Final = ZCLAttributeDef(
+            id=0x0004, type=t.CharacterString, access="r*w"
+        )
+        description: Final = ZCLAttributeDef(
+            id=0x001C, type=t.CharacterString, access="r*w"
+        )
+        inactive_text: Final = ZCLAttributeDef(
+            id=0x002E, type=t.CharacterString, access="r*w"
+        )
+        minimum_off_time: Final = ZCLAttributeDef(
+            id=0x0042, type=t.uint32_t, access="r*w"
+        )
+        minimum_on_time: Final = ZCLAttributeDef(
+            id=0x0043, type=t.uint32_t, access="r*w"
+        )
+        out_of_service: Final = ZCLAttributeDef(
+            id=0x0051, type=t.Bool, access="r*w", mandatory=True
+        )
+        polarity: Final = ZCLAttributeDef(id=0x0054, type=t.enum8, access="r")
+        present_value: Final = ZCLAttributeDef(
+            id=0x0055, type=t.Bool, access="r*w", mandatory=True
+        )
         # 0x0057: ('priority_array', TODO.array),  # Array of 16 structures of (boolean,
         # single precision)
-        0x0067: ZCLAttributeDef("reliability", type=t.enum8, access="r*w"),
-        0x0068: ZCLAttributeDef("relinquish_default", type=t.Bool, access="r*w"),
-        0x006A: ZCLAttributeDef(
-            "resolution", type=t.Single, access="r"
-        ),  # Does not seem to be in binary_output
-        0x006F: ZCLAttributeDef(
-            "status_flags", type=t.bitmap8, access="r", mandatory=True
-        ),
-        0x0075: ZCLAttributeDef(
-            "engineering_units", type=t.enum16, access="r"
-        ),  # Does not seem to be in binary_output
-        0x0100: ZCLAttributeDef("application_type", type=t.uint32_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        reliability: Final = ZCLAttributeDef(id=0x0067, type=t.enum8, access="r*w")
+        relinquish_default: Final = ZCLAttributeDef(
+            id=0x0068, type=t.Bool, access="r*w"
+        )
+        resolution: Final = ZCLAttributeDef(
+            id=0x006A, type=t.Single, access="r"
+        )  # Does not seem to be in binary_output
+        status_flags: Final = ZCLAttributeDef(
+            id=0x006F, type=t.bitmap8, access="r", mandatory=True
+        )
+        engineering_units: Final = ZCLAttributeDef(
+            id=0x0075, type=t.enum16, access="r"
+        )  # Does not seem to be in binary_output
+        application_type: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint32_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class BinaryValue(Cluster):
-    cluster_id = 0x0011
-    ep_attribute = "binary_value"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0004: ZCLAttributeDef("active_text", type=t.CharacterString, access="r*w"),
-        0x001C: ZCLAttributeDef("description", type=t.CharacterString, access="r*w"),
-        0x002E: ZCLAttributeDef("inactive_text", type=t.CharacterString, access="r*w"),
-        0x0042: ZCLAttributeDef("minimum_off_time", type=t.uint32_t, access="r*w"),
-        0x0043: ZCLAttributeDef("minimum_on_time", type=t.uint32_t, access="r*w"),
-        0x0051: ZCLAttributeDef(
-            "out_of_service", type=t.Bool, access="r*w", mandatory=True
-        ),
-        0x0055: ZCLAttributeDef(
-            "present_value", type=t.Single, access="r*w", mandatory=True
-        ),
+    cluster_id: Final = 0x0011
+    ep_attribute: Final = "binary_value"
+
+    class AttributeDefs(BaseAttributeDefs):
+        active_text: Final = ZCLAttributeDef(
+            id=0x0004, type=t.CharacterString, access="r*w"
+        )
+        description: Final = ZCLAttributeDef(
+            id=0x001C, type=t.CharacterString, access="r*w"
+        )
+        inactive_text: Final = ZCLAttributeDef(
+            id=0x002E, type=t.CharacterString, access="r*w"
+        )
+        minimum_off_time: Final = ZCLAttributeDef(
+            id=0x0042, type=t.uint32_t, access="r*w"
+        )
+        minimum_on_time: Final = ZCLAttributeDef(
+            id=0x0043, type=t.uint32_t, access="r*w"
+        )
+        out_of_service: Final = ZCLAttributeDef(
+            id=0x0051, type=t.Bool, access="r*w", mandatory=True
+        )
+        present_value: Final = ZCLAttributeDef(
+            id=0x0055, type=t.Single, access="r*w", mandatory=True
+        )
         # 0x0057: ZCLAttributeDef('priority_array', type=TODO.array),  # Array of 16 structures of (boolean,
         # single precision)
-        0x0067: ZCLAttributeDef("reliability", type=t.enum8, access="r*w"),
-        0x0068: ZCLAttributeDef("relinquish_default", type=t.Single, access="r*w"),
-        0x006F: ZCLAttributeDef(
-            "status_flags", type=t.bitmap8, access="r", mandatory=True
-        ),
-        0x0100: ZCLAttributeDef("application_type", type=t.uint32_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        reliability: Final = ZCLAttributeDef(id=0x0067, type=t.enum8, access="r*w")
+        relinquish_default: Final = ZCLAttributeDef(
+            id=0x0068, type=t.Single, access="r*w"
+        )
+        status_flags: Final = ZCLAttributeDef(
+            id=0x006F, type=t.bitmap8, access="r", mandatory=True
+        )
+        application_type: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint32_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class MultistateInput(Cluster):
-    cluster_id = 0x0012
-    ep_attribute = "multistate_input"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x000E: ZCLAttributeDef(
-            "state_text", type=t.List[t.CharacterString], access="r*w"
-        ),
-        0x001C: ZCLAttributeDef("description", type=t.CharacterString, access="r*w"),
-        0x004A: ZCLAttributeDef("number_of_states", type=t.uint16_t, access="r*w"),
-        0x0051: ZCLAttributeDef(
-            "out_of_service", type=t.Bool, access="r*w", mandatory=True
-        ),
-        0x0055: ZCLAttributeDef(
-            "present_value", type=t.Single, access="r*w", mandatory=True
-        ),
+    cluster_id: Final = 0x0012
+    ep_attribute: Final = "multistate_input"
+
+    class AttributeDefs(BaseAttributeDefs):
+        state_text: Final = ZCLAttributeDef(
+            id=0x000E, type=t.List[t.CharacterString], access="r*w"
+        )
+        description: Final = ZCLAttributeDef(
+            id=0x001C, type=t.CharacterString, access="r*w"
+        )
+        number_of_states: Final = ZCLAttributeDef(
+            id=0x004A, type=t.uint16_t, access="r*w"
+        )
+        out_of_service: Final = ZCLAttributeDef(
+            id=0x0051, type=t.Bool, access="r*w", mandatory=True
+        )
+        present_value: Final = ZCLAttributeDef(
+            id=0x0055, type=t.Single, access="r*w", mandatory=True
+        )
         # 0x0057: ('priority_array', TODO.array),  # Array of 16 structures of (boolean,
         # single precision)
-        0x0067: ZCLAttributeDef("reliability", type=t.enum8, access="r*w"),
-        0x006F: ZCLAttributeDef(
-            "status_flags", type=t.bitmap8, access="r", mandatory=True
-        ),
-        0x0100: ZCLAttributeDef("application_type", type=t.uint32_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        reliability: Final = ZCLAttributeDef(id=0x0067, type=t.enum8, access="r*w")
+        status_flags: Final = ZCLAttributeDef(
+            id=0x006F, type=t.bitmap8, access="r", mandatory=True
+        )
+        application_type: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint32_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class MultistateOutput(Cluster):
-    cluster_id = 0x0013
-    ep_attribute = "multistate_output"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x000E: ZCLAttributeDef(
-            "state_text", type=t.List[t.CharacterString], access="r*w"
-        ),
-        0x001C: ZCLAttributeDef("description", type=t.CharacterString, access="r*w"),
-        0x004A: ZCLAttributeDef(
-            "number_of_states", type=t.uint16_t, access="r*w", mandatory=True
-        ),
-        0x0051: ZCLAttributeDef(
-            "out_of_service", type=t.Bool, access="r*w", mandatory=True
-        ),
-        0x0055: ZCLAttributeDef(
-            "present_value", type=t.Single, access="r*w", mandatory=True
-        ),
+    cluster_id: Final = 0x0013
+    ep_attribute: Final = "multistate_output"
+
+    class AttributeDefs(BaseAttributeDefs):
+        state_text: Final = ZCLAttributeDef(
+            id=0x000E, type=t.List[t.CharacterString], access="r*w"
+        )
+        description: Final = ZCLAttributeDef(
+            id=0x001C, type=t.CharacterString, access="r*w"
+        )
+        number_of_states: Final = ZCLAttributeDef(
+            id=0x004A, type=t.uint16_t, access="r*w", mandatory=True
+        )
+        out_of_service: Final = ZCLAttributeDef(
+            id=0x0051, type=t.Bool, access="r*w", mandatory=True
+        )
+        present_value: Final = ZCLAttributeDef(
+            id=0x0055, type=t.Single, access="r*w", mandatory=True
+        )
         # 0x0057: ZCLAttributeDef('priority_array', type=TODO.array),  # Array of 16 structures of (boolean,
         # single precision)
-        0x0067: ZCLAttributeDef("reliability", type=t.enum8, access="r*w"),
-        0x0068: ZCLAttributeDef("relinquish_default", type=t.Single, access="r*w"),
-        0x006F: ZCLAttributeDef(
-            "status_flags", type=t.bitmap8, access="r", mandatory=True
-        ),
-        0x0100: ZCLAttributeDef("application_type", type=t.uint32_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        reliability: Final = ZCLAttributeDef(id=0x0067, type=t.enum8, access="r*w")
+        relinquish_default: Final = ZCLAttributeDef(
+            id=0x0068, type=t.Single, access="r*w"
+        )
+        status_flags: Final = ZCLAttributeDef(
+            id=0x006F, type=t.bitmap8, access="r", mandatory=True
+        )
+        application_type: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint32_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class MultistateValue(Cluster):
-    cluster_id = 0x0014
-    ep_attribute = "multistate_value"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x000E: ZCLAttributeDef("state_text", t.List[t.CharacterString], access="r*w"),
-        0x001C: ZCLAttributeDef("description", t.CharacterString, access="r*w"),
-        0x004A: ZCLAttributeDef(
-            "number_of_states", t.uint16_t, access="r*w", mandatory=True
-        ),
-        0x0051: ZCLAttributeDef("out_of_service", t.Bool, access="r*w", mandatory=True),
-        0x0055: ZCLAttributeDef(
-            "present_value", t.Single, access="r*w", mandatory=True
-        ),
-        # 0x0057: ('priority_array', TODO.array),  # Array of 16 structures of (boolean,
+    cluster_id: Final = 0x0014
+    ep_attribute: Final = "multistate_value"
+
+    class AttributeDefs(BaseAttributeDefs):
+        state_text: Final = ZCLAttributeDef(
+            id=0x000E, type=t.List[t.CharacterString], access="r*w"
+        )
+        description: Final = ZCLAttributeDef(
+            id=0x001C, type=t.CharacterString, access="r*w"
+        )
+        number_of_states: Final = ZCLAttributeDef(
+            id=0x004A, type=t.uint16_t, access="r*w", mandatory=True
+        )
+        out_of_service: Final = ZCLAttributeDef(
+            id=0x0051, type=t.Bool, access="r*w", mandatory=True
+        )
+        present_value: Final = ZCLAttributeDef(
+            id=0x0055, type=t.Single, access="r*w", mandatory=True
+        )
+        # 0x0057: ZCLAttributeDef('priority_array', type=TODO.array),  # Array of 16 structures of (boolean,
         # single precision)
-        0x0067: ZCLAttributeDef("reliability", t.enum8, access="r*w"),
-        0x0068: ZCLAttributeDef("relinquish_default", t.Single, access="r*w"),
-        0x006F: ZCLAttributeDef("status_flags", t.bitmap8, access="r", mandatory=True),
-        0x0100: ZCLAttributeDef("application_type", t.uint32_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        reliability: Final = ZCLAttributeDef(id=0x0067, type=t.enum8, access="r*w")
+        relinquish_default: Final = ZCLAttributeDef(
+            id=0x0068, type=t.Single, access="r*w"
+        )
+        status_flags: Final = ZCLAttributeDef(
+            id=0x006F, type=t.bitmap8, access="r", mandatory=True
+        )
+        application_type: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint32_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+
+class StartupControl(t.enum8):
+    Part_of_network = 0x00
+    Form_network = 0x01
+    Rejoin_network = 0x02
+    Start_from_scratch = 0x03
+
+
+class NetworkKeyType(t.enum8):
+    Standard = 0x01
 
 
 class Commissioning(Cluster):
     """Attributes and commands for commissioning and
     managing a ZigBee device.
     """
 
-    cluster_id = 0x0015
-    ep_attribute = "commissioning"
-
-    class StartupControl(t.enum8):
-        Part_of_network = 0x00
-        Form_network = 0x01
-        Rejoin_network = 0x02
-        Start_from_scratch = 0x03
+    StartupControl: Final = StartupControl
+    NetworkKeyType: Final = NetworkKeyType
 
-    class NetworkKeyType(t.enum8):
-        Standard = 0x01
+    cluster_id: Final = 0x0015
+    ep_attribute: Final = "commissioning"
 
-    attributes: dict[int, ZCLAttributeDef] = {
+    class AttributeDefs(BaseAttributeDefs):
         # Startup Parameters
-        0x0000: ZCLAttributeDef(
-            "short_address", type=t.uint16_t, access="rw", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef(
-            "extended_pan_id", type=t.EUI64, access="rw", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef("pan_id", type=t.uint16_t, access="rw", mandatory=True),
-        0x0003: ZCLAttributeDef(
-            "channel_mask", type=t.Channels, access="rw", mandatory=True
-        ),
-        0x0004: ZCLAttributeDef(
-            "protocol_version", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0005: ZCLAttributeDef(
-            "stack_profile", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0006: ZCLAttributeDef(
-            "startup_control", type=StartupControl, access="rw", mandatory=True
-        ),
-        0x0010: ZCLAttributeDef(
-            "trust_center_address", type=t.EUI64, access="rw", mandatory=True
-        ),
-        0x0011: ZCLAttributeDef("trust_center_master_key", type=t.KeyData, access="rw"),
-        0x0012: ZCLAttributeDef(
-            "network_key", type=t.KeyData, access="rw", mandatory=True
-        ),
-        0x0013: ZCLAttributeDef(
-            "use_insecure_join", type=t.Bool, access="rw", mandatory=True
-        ),
-        0x0014: ZCLAttributeDef(
-            "preconfigured_link_key", type=t.KeyData, access="rw", mandatory=True
-        ),
-        0x0015: ZCLAttributeDef(
-            "network_key_seq_num", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0016: ZCLAttributeDef(
-            "network_key_type", type=NetworkKeyType, access="rw", mandatory=True
-        ),
-        0x0017: ZCLAttributeDef(
-            "network_manager_address", type=t.uint16_t, access="rw", mandatory=True
-        ),
+        short_address: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint16_t, access="rw", mandatory=True
+        )
+        extended_pan_id: Final = ZCLAttributeDef(
+            id=0x0001, type=t.EUI64, access="rw", mandatory=True
+        )
+        pan_id: Final = ZCLAttributeDef(
+            id=0x0002, type=t.uint16_t, access="rw", mandatory=True
+        )
+        channel_mask: Final = ZCLAttributeDef(
+            id=0x0003, type=t.Channels, access="rw", mandatory=True
+        )
+        protocol_version: Final = ZCLAttributeDef(
+            id=0x0004, type=t.uint8_t, access="rw", mandatory=True
+        )
+        stack_profile: Final = ZCLAttributeDef(
+            id=0x0005, type=t.uint8_t, access="rw", mandatory=True
+        )
+        startup_control: Final = ZCLAttributeDef(
+            id=0x0006, type=StartupControl, access="rw", mandatory=True
+        )
+        trust_center_address: Final = ZCLAttributeDef(
+            id=0x0010, type=t.EUI64, access="rw", mandatory=True
+        )
+        trust_center_master_key: Final = ZCLAttributeDef(
+            id=0x0011, type=t.KeyData, access="rw"
+        )
+        network_key: Final = ZCLAttributeDef(
+            id=0x0012, type=t.KeyData, access="rw", mandatory=True
+        )
+        use_insecure_join: Final = ZCLAttributeDef(
+            id=0x0013, type=t.Bool, access="rw", mandatory=True
+        )
+        preconfigured_link_key: Final = ZCLAttributeDef(
+            id=0x0014, type=t.KeyData, access="rw", mandatory=True
+        )
+        network_key_seq_num: Final = ZCLAttributeDef(
+            id=0x0015, type=t.uint8_t, access="rw", mandatory=True
+        )
+        network_key_type: Final = ZCLAttributeDef(
+            id=0x0016, type=NetworkKeyType, access="rw", mandatory=True
+        )
+        network_manager_address: Final = ZCLAttributeDef(
+            id=0x0017, type=t.uint16_t, access="rw", mandatory=True
+        )
         # Join Parameters
-        0x0020: ZCLAttributeDef("scan_attempts", type=t.uint8_t, access="rw"),
-        0x0021: ZCLAttributeDef("time_between_scans", type=t.uint16_t, access="rw"),
-        0x0022: ZCLAttributeDef("rejoin_interval", type=t.uint16_t, access="rw"),
-        0x0023: ZCLAttributeDef("max_rejoin_interval", type=t.uint16_t, access="rw"),
+        scan_attempts: Final = ZCLAttributeDef(id=0x0020, type=t.uint8_t, access="rw")
+        time_between_scans: Final = ZCLAttributeDef(
+            id=0x0021, type=t.uint16_t, access="rw"
+        )
+        rejoin_interval: Final = ZCLAttributeDef(
+            id=0x0022, type=t.uint16_t, access="rw"
+        )
+        max_rejoin_interval: Final = ZCLAttributeDef(
+            id=0x0023, type=t.uint16_t, access="rw"
+        )
         # End Device Parameters
-        0x0030: ZCLAttributeDef("indirect_poll_rate", type=t.uint16_t, access="rw"),
-        0x0031: ZCLAttributeDef("parent_retry_threshold", type=t.uint8_t, access="r"),
+        indirect_poll_rate: Final = ZCLAttributeDef(
+            id=0x0030, type=t.uint16_t, access="rw"
+        )
+        parent_retry_threshold: Final = ZCLAttributeDef(
+            id=0x0031, type=t.uint8_t, access="r"
+        )
         # Concentrator Parameters
-        0x0040: ZCLAttributeDef("concentrator_flag", type=t.Bool, access="rw"),
-        0x0041: ZCLAttributeDef("concentrator_radius", type=t.uint8_t, access="rw"),
-        0x0042: ZCLAttributeDef(
-            "concentrator_discovery_time", type=t.uint8_t, access="rw"
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "restart_device",
-            {"options": t.bitmap8, "delay": t.uint8_t, "jitter": t.uint8_t},
-            False,
-        ),
-        0x01: ZCLCommandDef(
-            "save_startup_parameters", {"options": t.bitmap8, "index": t.uint8_t}, False
-        ),
-        0x02: ZCLCommandDef(
-            "restore_startup_parameters",
-            {"options": t.bitmap8, "index": t.uint8_t},
-            False,
-        ),
-        0x03: ZCLCommandDef(
-            "reset_startup_parameters",
-            {"options": t.bitmap8, "index": t.uint8_t},
-            False,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "restart_device_response", {"status": foundation.Status}, True
-        ),
-        0x01: ZCLCommandDef(
-            "save_startup_params_response", {"status": foundation.Status}, True
-        ),
-        0x02: ZCLCommandDef(
-            "restore_startup_params_response", {"status": foundation.Status}, True
-        ),
-        0x03: ZCLCommandDef(
-            "reset_startup_params_response", {"status": foundation.Status}, True
-        ),
-    }
+        concentrator_flag: Final = ZCLAttributeDef(id=0x0040, type=t.Bool, access="rw")
+        concentrator_radius: Final = ZCLAttributeDef(
+            id=0x0041, type=t.uint8_t, access="rw"
+        )
+        concentrator_discovery_time: Final = ZCLAttributeDef(
+            id=0x0042, type=t.uint8_t, access="rw"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        restart_device: Final = ZCLCommandDef(
+            id=0x00,
+            schema={"options": t.bitmap8, "delay": t.uint8_t, "jitter": t.uint8_t},
+            direction=False,
+        )
+        save_startup_parameters: Final = ZCLCommandDef(
+            id=0x01,
+            schema={"options": t.bitmap8, "index": t.uint8_t},
+            direction=False,
+        )
+        restore_startup_parameters: Final = ZCLCommandDef(
+            id=0x02,
+            schema={"options": t.bitmap8, "index": t.uint8_t},
+            direction=False,
+        )
+        reset_startup_parameters: Final = ZCLCommandDef(
+            id=0x03,
+            schema={"options": t.bitmap8, "index": t.uint8_t},
+            direction=False,
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        restart_device_response: Final = ZCLCommandDef(
+            id=0x00, schema={"status": foundation.Status}, direction=True
+        )
+        save_startup_params_response: Final = ZCLCommandDef(
+            id=0x01, schema={"status": foundation.Status}, direction=True
+        )
+        restore_startup_params_response: Final = ZCLCommandDef(
+            id=0x02, schema={"status": foundation.Status}, direction=True
+        )
+        reset_startup_params_response: Final = ZCLCommandDef(
+            id=0x03, schema={"status": foundation.Status}, direction=True
+        )
 
 
 class Partition(Cluster):
-    cluster_id = 0x0016
-    ep_attribute = "partition"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "maximum_incoming_transfer_size",
+    cluster_id: Final = 0x0016
+    ep_attribute: Final = "partition"
+
+    class AttributeDefs(BaseAttributeDefs):
+        maximum_incoming_transfer_size: Final = ZCLAttributeDef(
+            id=0x0000,
             type=t.uint16_t,
             access="r",
             mandatory=True,
-        ),
-        0x0001: ZCLAttributeDef(
-            "maximum_outgoing_transfer_size",
+        )
+        maximum_outgoing_transfer_size: Final = ZCLAttributeDef(
+            id=0x0001,
             type=t.uint16_t,
             access="r",
             mandatory=True,
-        ),
-        0x0002: ZCLAttributeDef(
-            "partitioned_frame_size", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0003: ZCLAttributeDef(
-            "large_frame_size", type=t.uint16_t, access="rw", mandatory=True
-        ),
-        0x0004: ZCLAttributeDef(
-            "number_of_ack_frame", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0005: ZCLAttributeDef(
-            "nack_timeout", type=t.uint16_t, access="r", mandatory=True
-        ),
-        0x0006: ZCLAttributeDef(
-            "interframe_delay", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0007: ZCLAttributeDef(
-            "number_of_send_retries", type=t.uint8_t, access="r", mandatory=True
-        ),
-        0x0008: ZCLAttributeDef(
-            "sender_timeout", type=t.uint16_t, access="r", mandatory=True
-        ),
-        0x0009: ZCLAttributeDef(
-            "receiver_timeout", type=t.uint16_t, access="r", mandatory=True
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
-
-
-class Ota(Cluster):
-    class ImageUpgradeStatus(t.enum8):
-        Normal = 0x00
-        Download_in_progress = 0x01
-        Download_complete = 0x02
-        Waiting_to_upgrade = 0x03
-        Count_down = 0x04
-        Wait_for_more = 0x05
-        Waiting_to_Upgrade_via_External_Event = 0x06
-
-    class UpgradeActivationPolicy(t.enum8):
-        OTA_server_allowed = 0x00
-        Out_of_band_allowed = 0x01
-
-    class UpgradeTimeoutPolicy(t.enum8):
-        Apply_after_timeout = 0x00
-        Do_not_apply_after_timeout = 0x01
-
-    class ImageNotifyCommand(foundation.CommandSchema):
-        class PayloadType(t.enum8):
-            QueryJitter = 0x00
-            QueryJitter_ManufacturerCode = 0x01
-            QueryJitter_ManufacturerCode_ImageType = 0x02
-            QueryJitter_ManufacturerCode_ImageType_NewFileVersion = 0x03
-
-        payload_type: None = t.StructField(type=PayloadType)
-        query_jitter: t.uint8_t
-        manufacturer_code: t.uint16_t = t.StructField(
-            requires=(
-                lambda s: s.payload_type >= s.PayloadType.QueryJitter_ManufacturerCode
-            )
         )
-        image_type: t.uint16_t = t.StructField(
-            requires=(
-                lambda s: s.payload_type
-                >= s.PayloadType.QueryJitter_ManufacturerCode_ImageType
-            )
+        partitioned_frame_size: Final = ZCLAttributeDef(
+            id=0x0002, type=t.uint8_t, access="rw", mandatory=True
         )
-        new_file_version: t.uint32_t = t.StructField(
-            requires=(
-                lambda s: s.payload_type
-                >= s.PayloadType.QueryJitter_ManufacturerCode_ImageType_NewFileVersion
-            )
+        large_frame_size: Final = ZCLAttributeDef(
+            id=0x0003, type=t.uint16_t, access="rw", mandatory=True
+        )
+        number_of_ack_frame: Final = ZCLAttributeDef(
+            id=0x0004, type=t.uint8_t, access="rw", mandatory=True
         )
+        nack_timeout: Final = ZCLAttributeDef(
+            id=0x0005, type=t.uint16_t, access="r", mandatory=True
+        )
+        interframe_delay: Final = ZCLAttributeDef(
+            id=0x0006, type=t.uint8_t, access="rw", mandatory=True
+        )
+        number_of_send_retries: Final = ZCLAttributeDef(
+            id=0x0007, type=t.uint8_t, access="r", mandatory=True
+        )
+        sender_timeout: Final = ZCLAttributeDef(
+            id=0x0008, type=t.uint16_t, access="r", mandatory=True
+        )
+        receiver_timeout: Final = ZCLAttributeDef(
+            id=0x0009, type=t.uint16_t, access="r", mandatory=True
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+
+class ImageUpgradeStatus(t.enum8):
+    Normal = 0x00
+    Download_in_progress = 0x01
+    Download_complete = 0x02
+    Waiting_to_upgrade = 0x03
+    Count_down = 0x04
+    Wait_for_more = 0x05
+    Waiting_to_Upgrade_via_External_Event = 0x06
+
+
+class UpgradeActivationPolicy(t.enum8):
+    OTA_server_allowed = 0x00
+    Out_of_band_allowed = 0x01
+
+
+class UpgradeTimeoutPolicy(t.enum8):
+    Apply_after_timeout = 0x00
+    Do_not_apply_after_timeout = 0x01
+
+
+class ImageNotifyCommand(foundation.CommandSchema):
+    class PayloadType(t.enum8):
+        QueryJitter = 0x00
+        QueryJitter_ManufacturerCode = 0x01
+        QueryJitter_ManufacturerCode_ImageType = 0x02
+        QueryJitter_ManufacturerCode_ImageType_NewFileVersion = 0x03
+
+    payload_type: None = t.StructField(type=PayloadType)
+    query_jitter: t.uint8_t
+    manufacturer_code: t.uint16_t = t.StructField(
+        requires=(
+            lambda s: s.payload_type >= s.PayloadType.QueryJitter_ManufacturerCode
+        )
+    )
+    image_type: t.uint16_t = t.StructField(
+        requires=(
+            lambda s: s.payload_type
+            >= s.PayloadType.QueryJitter_ManufacturerCode_ImageType
+        )
+    )
+    new_file_version: t.uint32_t = t.StructField(
+        requires=(
+            lambda s: s.payload_type
+            >= s.PayloadType.QueryJitter_ManufacturerCode_ImageType_NewFileVersion
+        )
+    )
+
+
+class QueryNextImageCommand(foundation.CommandSchema):
+    class FieldControl(t.bitmap8):
+        HardwareVersion = 0b00000001
+
+    field_control: None = t.StructField(type=FieldControl)
+    manufacturer_code: t.uint16_t
+    image_type: t.uint16_t
+    current_file_version: t.uint32_t
+    hardware_version: t.uint16_t = t.StructField(
+        requires=(lambda s: s.field_control & s.FieldControl.HardwareVersion)
+    )
+
+
+class ImageBlockCommand(foundation.CommandSchema):
+    class FieldControl(t.bitmap8):
+        RequestNodeAddr = 0b00000001
+        MinimumBlockPeriod = 0b00000010
+
+    field_control: None = t.StructField(type=FieldControl)
+    manufacturer_code: t.uint16_t
+    image_type: t.uint16_t
+    file_version: t.uint32_t
+    file_offset: t.uint32_t
+    maximum_data_size: t.uint8_t
+    request_node_addr: t.EUI64 = t.StructField(
+        requires=(lambda s: s.field_control & s.FieldControl.RequestNodeAddr)
+    )
+    minimum_block_period: t.uint16_t = t.StructField(
+        requires=(lambda s: s.field_control & s.FieldControl.MinimumBlockPeriod)
+    )
+
+
+class ImagePageCommand(foundation.CommandSchema):
+    class FieldControl(t.bitmap8):
+        RequestNodeAddr = 0b00000001
+
+    field_control: None = t.StructField(type=FieldControl)
+    manufacturer_code: t.uint16_t
+    image_type: t.uint16_t
+    file_version: t.uint32_t
+    file_offset: t.uint32_t
+    maximum_data_size: t.uint8_t
+    page_size: t.uint16_t
+    response_spacing: t.uint16_t
+    request_node_addr: t.EUI64 = t.StructField(
+        requires=lambda s: s.field_control & s.FieldControl.RequestNodeAddr
+    )
+
+
+class ImageBlockResponseCommand(foundation.CommandSchema):
+    # All responses contain at least a status
+    status: foundation.Status
+
+    # Payload with `SUCCESS` status
+    manufacturer_code: t.uint16_t = t.StructField(
+        requires=lambda s: s.status == foundation.Status.SUCCESS
+    )
+    image_type: t.uint16_t = t.StructField(
+        requires=lambda s: s.status == foundation.Status.SUCCESS
+    )
+    file_version: t.uint32_t = t.StructField(
+        requires=lambda s: s.status == foundation.Status.SUCCESS
+    )
+    file_offset: t.uint32_t = t.StructField(
+        requires=lambda s: s.status == foundation.Status.SUCCESS
+    )
+    image_data: t.LVBytes = t.StructField(
+        requires=lambda s: s.status == foundation.Status.SUCCESS
+    )
+
+    # Payload with `WAIT_FOR_DATA` status
+    current_time: t.UTCTime = t.StructField(
+        requires=lambda s: s.status == foundation.Status.WAIT_FOR_DATA
+    )
+    request_time: t.UTCTime = t.StructField(
+        requires=lambda s: s.status == foundation.Status.WAIT_FOR_DATA
+    )
+    minimum_block_period: t.uint16_t = t.StructField(
+        requires=lambda s: s.status == foundation.Status.WAIT_FOR_DATA
+    )
+
 
-    class QueryNextImageCommand(foundation.CommandSchema):
-        class FieldControl(t.bitmap8):
-            HardwareVersion = 0b00000001
-
-        field_control: None = t.StructField(type=FieldControl)
-        manufacturer_code: t.uint16_t
-        image_type: t.uint16_t
-        current_file_version: t.uint32_t
-        hardware_version: t.uint16_t = t.StructField(
-            requires=(lambda s: s.field_control & s.FieldControl.HardwareVersion)
-        )
-
-    class ImageBlockCommand(foundation.CommandSchema):
-        class FieldControl(t.bitmap8):
-            RequestNodeAddr = 0b00000001
-            MinimumBlockPeriod = 0b00000010
-
-        field_control: None = t.StructField(type=FieldControl)
-        manufacturer_code: t.uint16_t
-        image_type: t.uint16_t
-        file_version: t.uint32_t
-        file_offset: t.uint32_t
-        maximum_data_size: t.uint8_t
-        request_node_addr: t.EUI64 = t.StructField(
-            requires=(lambda s: s.field_control & s.FieldControl.RequestNodeAddr)
-        )
-        minimum_block_period: t.uint16_t = t.StructField(
-            requires=(lambda s: s.field_control & s.FieldControl.MinimumBlockPeriod)
-        )
-
-    class ImagePageCommand(foundation.CommandSchema):
-        class FieldControl(t.bitmap8):
-            RequestNodeAddr = 0b00000001
-
-        field_control: None = t.StructField(type=FieldControl)
-        manufacturer_code: t.uint16_t
-        image_type: t.uint16_t
-        file_version: t.uint32_t
-        file_offset: t.uint32_t
-        maximum_data_size: t.uint8_t
-        page_size: t.uint16_t
-        response_spacing: t.uint16_t
-        request_node_addr: t.EUI64 = t.StructField(
-            requires=lambda s: s.field_control & s.FieldControl.RequestNodeAddr
-        )
-
-    class ImageBlockResponseCommand(foundation.CommandSchema):
-        # All responses contain at least a status
-        status: foundation.Status
-
-        # Payload with `SUCCESS` status
-        manufacturer_code: t.uint16_t = t.StructField(
-            requires=lambda s: s.status == foundation.Status.SUCCESS
-        )
-        image_type: t.uint16_t = t.StructField(
-            requires=lambda s: s.status == foundation.Status.SUCCESS
-        )
-        file_version: t.uint32_t = t.StructField(
-            requires=lambda s: s.status == foundation.Status.SUCCESS
-        )
-        file_offset: t.uint32_t = t.StructField(
-            requires=lambda s: s.status == foundation.Status.SUCCESS
-        )
-        image_data: t.LVBytes = t.StructField(
-            requires=lambda s: s.status == foundation.Status.SUCCESS
-        )
-
-        # Payload with `WAIT_FOR_DATA` status
-        current_time: t.UTCTime = t.StructField(
-            requires=lambda s: s.status == foundation.Status.WAIT_FOR_DATA
-        )
-        request_time: t.UTCTime = t.StructField(
-            requires=lambda s: s.status == foundation.Status.WAIT_FOR_DATA
-        )
-        minimum_block_period: t.uint16_t = t.StructField(
-            requires=lambda s: s.status == foundation.Status.WAIT_FOR_DATA
-        )
-
-    cluster_id = 0x0019
-    ep_attribute = "ota"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "upgrade_server_id", type=t.EUI64, access="r", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef("file_offset", type=t.uint32_t, access="r"),
-        0x0002: ZCLAttributeDef("current_file_version", type=t.uint32_t, access="r"),
-        0x0003: ZCLAttributeDef(
-            "current_zigbee_stack_version", type=t.uint16_t, access="r"
-        ),
-        0x0004: ZCLAttributeDef("downloaded_file_version", type=t.uint32_t, access="r"),
-        0x0005: ZCLAttributeDef(
-            "downloaded_zigbee_stack_version", type=t.uint16_t, access="r"
-        ),
-        0x0006: ZCLAttributeDef(
-            "image_upgrade_status", type=ImageUpgradeStatus, access="r", mandatory=True
-        ),
-        0x0007: ZCLAttributeDef("manufacturer_id", type=t.uint16_t, access="r"),
-        0x0008: ZCLAttributeDef("image_type_id", type=t.uint16_t, access="r"),
-        0x0009: ZCLAttributeDef("minimum_block_req_delay", type=t.uint16_t, access="r"),
-        0x000A: ZCLAttributeDef("image_stamp", type=t.uint32_t, access="r"),
-        0x000B: ZCLAttributeDef(
-            "upgrade_activation_policy", type=UpgradeActivationPolicy, access="r"
-        ),
-        0x000C: ZCLAttributeDef(
-            "upgrade_timeout_policy", type=UpgradeTimeoutPolicy, access="r"
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x01: ZCLCommandDef("query_next_image", QueryNextImageCommand, False),
-        0x03: ZCLCommandDef("image_block", ImageBlockCommand, False),
-        0x04: ZCLCommandDef("image_page", ImagePageCommand, False),
-        0x06: ZCLCommandDef(
-            "upgrade_end",
-            {
+class Ota(Cluster):
+    ImageUpgradeStatus: Final = ImageUpgradeStatus
+    UpgradeActivationPolicy: Final = UpgradeActivationPolicy
+    UpgradeTimeoutPolicy: Final = UpgradeTimeoutPolicy
+    ImageNotifyCommand: Final = ImageNotifyCommand
+    QueryNextImageCommand: Final = QueryNextImageCommand
+    ImageBlockCommand: Final = ImageBlockCommand
+    ImagePageCommand: Final = ImagePageCommand
+    ImageBlockResponseCommand: Final = ImageBlockResponseCommand
+
+    cluster_id: Final = 0x0019
+    ep_attribute: Final = "ota"
+
+    class AttributeDefs(BaseAttributeDefs):
+        upgrade_server_id: Final = ZCLAttributeDef(
+            id=0x0000, type=t.EUI64, access="r", mandatory=True
+        )
+        file_offset: Final = ZCLAttributeDef(id=0x0001, type=t.uint32_t, access="r")
+        current_file_version: Final = ZCLAttributeDef(
+            id=0x0002, type=t.uint32_t, access="r"
+        )
+        current_zigbee_stack_version: Final = ZCLAttributeDef(
+            id=0x0003, type=t.uint16_t, access="r"
+        )
+        downloaded_file_version: Final = ZCLAttributeDef(
+            id=0x0004, type=t.uint32_t, access="r"
+        )
+        downloaded_zigbee_stack_version: Final = ZCLAttributeDef(
+            id=0x0005, type=t.uint16_t, access="r"
+        )
+        image_upgrade_status: Final = ZCLAttributeDef(
+            id=0x0006, type=ImageUpgradeStatus, access="r", mandatory=True
+        )
+        manufacturer_id: Final = ZCLAttributeDef(id=0x0007, type=t.uint16_t, access="r")
+        image_type_id: Final = ZCLAttributeDef(id=0x0008, type=t.uint16_t, access="r")
+        minimum_block_req_delay: Final = ZCLAttributeDef(
+            id=0x0009, type=t.uint16_t, access="r"
+        )
+        image_stamp: Final = ZCLAttributeDef(id=0x000A, type=t.uint32_t, access="r")
+        upgrade_activation_policy: Final = ZCLAttributeDef(
+            id=0x000B, type=UpgradeActivationPolicy, access="r"
+        )
+        upgrade_timeout_policy: Final = ZCLAttributeDef(
+            id=0x000C, type=UpgradeTimeoutPolicy, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        query_next_image: Final = ZCLCommandDef(
+            id=0x01, schema=QueryNextImageCommand, direction=False
+        )
+        image_block: Final = ZCLCommandDef(
+            id=0x03, schema=ImageBlockCommand, direction=False
+        )
+        image_page: Final = ZCLCommandDef(
+            id=0x04, schema=ImagePageCommand, direction=False
+        )
+        upgrade_end: Final = ZCLCommandDef(
+            id=0x06,
+            schema={
                 "status": foundation.Status,
                 "manufacturer_code": t.uint16_t,
                 "image_type": t.uint16_t,
                 "file_version": t.uint32_t,
             },
-            False,
-        ),
-        0x08: ZCLCommandDef(
-            "query_specific_file",
-            {
+            direction=False,
+        )
+        query_specific_file: Final = ZCLCommandDef(
+            id=0x08,
+            schema={
                 "request_node_addr": t.EUI64,
                 "manufacturer_code": t.uint16_t,
                 "image_type": t.uint16_t,
                 "file_version": t.uint32_t,
                 "current_zigbee_stack_version": t.uint16_t,
             },
-            False,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef("image_notify", ImageNotifyCommand, False),
-        0x02: ZCLCommandDef(
-            "query_next_image_response",
-            {
+            direction=False,
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        image_notify: Final = ZCLCommandDef(
+            id=0x00, schema=ImageNotifyCommand, direction=False
+        )
+        query_next_image_response: Final = ZCLCommandDef(
+            id=0x02,
+            schema={
                 "status": foundation.Status,
                 "manufacturer_code?": t.uint16_t,
                 "image_type?": t.uint16_t,
                 "file_version?": t.uint32_t,
                 "image_size?": t.uint32_t,
             },
-            True,
-        ),
-        0x05: ZCLCommandDef(
-            "image_block_response",
-            ImageBlockResponseCommand,
-            True,
-        ),
-        0x07: ZCLCommandDef(
-            "upgrade_end_response",
-            {
+            direction=True,
+        )
+        image_block_response: Final = ZCLCommandDef(
+            id=0x05,
+            schema=ImageBlockResponseCommand,
+            direction=True,
+        )
+        upgrade_end_response: Final = ZCLCommandDef(
+            id=0x07,
+            schema={
                 "manufacturer_code": t.uint16_t,
                 "image_type": t.uint16_t,
                 "file_version": t.uint32_t,
                 "current_time": t.UTCTime,
                 "upgrade_time": t.UTCTime,
             },
-            True,
-        ),
-        0x09: ZCLCommandDef(
-            "query_specific_file_response",
-            {
+            direction=True,
+        )
+        query_specific_file_response: Final = ZCLCommandDef(
+            id=0x09,
+            schema={
                 "status": foundation.Status,
                 "manufacturer_code?": t.uint16_t,
                 "image_type?": t.uint16_t,
                 "file_version?": t.uint32_t,
                 "image_size?": t.uint32_t,
             },
-            True,
-        ),
-    }
+            direction=True,
+        )
 
     def handle_cluster_request(
         self,
         hdr: foundation.ZCLHeader,
         args: list[Any],
         *,
         dst_addressing: AddressingMode | None = None,
@@ -1973,255 +2335,271 @@
             file_ver,
         )
         await self.upgrade_end_response(
             manufacturer_id, image_type, file_ver, 0x00000000, 0x00000000, tsn=tsn
         )
 
 
+class ScheduleRecord(t.Struct):
+    phase_id: t.uint8_t
+    scheduled_time: t.uint16_t
+
+
+class PowerProfilePhase(t.Struct):
+    energy_phase_id: t.uint8_t
+    macro_phase_id: t.uint8_t
+    expected_duration: t.uint16_t
+    peak_power: t.uint16_t
+    energy: t.uint16_t
+
+
+class PowerProfileType(t.Struct):
+    power_profile_id: t.uint8_t
+    energy_phase_id: t.uint8_t
+    power_profile_remote_control: t.Bool
+    power_profile_state: t.uint8_t
+
+
 class PowerProfile(Cluster):
-    cluster_id = 0x001A
-    ep_attribute = "power_profile"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "total_profile_num", type=t.uint8_t, access="r", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef(
-            "multiple_scheduling", type=t.Bool, access="r", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef(
-            "energy_formatting", type=t.bitmap8, access="r", mandatory=True
-        ),
-        0x0003: ZCLAttributeDef(
-            "energy_remote", type=t.Bool, access="r", mandatory=True
-        ),
-        0x0004: ZCLAttributeDef(
-            "schedule_mode", type=t.bitmap8, access="rwp", mandatory=True
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-
-    class ScheduleRecord(t.Struct):
-        phase_id: t.uint8_t
-        scheduled_time: t.uint16_t
-
-    class PowerProfilePhase(t.Struct):
-        energy_phase_id: t.uint8_t
-        macro_phase_id: t.uint8_t
-        expected_duration: t.uint16_t
-        peak_power: t.uint16_t
-        energy: t.uint16_t
-
-    class PowerProfile(t.Struct):
-        power_profile_id: t.uint8_t
-        energy_phase_id: t.uint8_t
-        power_profile_remote_control: t.Bool
-        power_profile_state: t.uint8_t
-
-    # XXX: are these flipped?
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "power_profile_request", {"power_profile_id": t.uint8_t}, False
-        ),
-        0x01: ZCLCommandDef("power_profile_state_request", {}, False),
-        0x02: ZCLCommandDef(
-            "get_power_profile_price_response",
-            {
+    ScheduleRecord: Final = ScheduleRecord
+    PowerProfilePhase: Final = PowerProfilePhase
+    PowerProfile: Final = PowerProfileType
+
+    cluster_id: Final = 0x001A
+    ep_attribute: Final = "power_profile"
+
+    class AttributeDefs(BaseAttributeDefs):
+        total_profile_num: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint8_t, access="r", mandatory=True
+        )
+        multiple_scheduling: Final = ZCLAttributeDef(
+            id=0x0001, type=t.Bool, access="r", mandatory=True
+        )
+        energy_formatting: Final = ZCLAttributeDef(
+            id=0x0002, type=t.bitmap8, access="r", mandatory=True
+        )
+        energy_remote: Final = ZCLAttributeDef(
+            id=0x0003, type=t.Bool, access="r", mandatory=True
+        )
+        schedule_mode: Final = ZCLAttributeDef(
+            id=0x0004, type=t.bitmap8, access="rwp", mandatory=True
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        power_profile_request: Final = ZCLCommandDef(
+            id=0x00, schema={"power_profile_id": t.uint8_t}, direction=False
+        )
+        power_profile_state_request: Final = ZCLCommandDef(
+            id=0x01, schema={}, direction=False
+        )
+        get_power_profile_price_response: Final = ZCLCommandDef(
+            id=0x02,
+            schema={
                 "power_profile_id": t.uint8_t,
                 "currency": t.uint16_t,
                 "price": t.uint32_t,
                 "price_trailing_digit": t.uint8_t,
             },
-            True,
-        ),
-        0x03: ZCLCommandDef(
-            "get_overall_schedule_price_response",
-            {
+            direction=True,
+        )
+        get_overall_schedule_price_response: Final = ZCLCommandDef(
+            id=0x03,
+            schema={
                 "currency": t.uint16_t,
                 "price": t.uint32_t,
                 "price_trailing_digit": t.uint8_t,
             },
-            True,
-        ),
-        0x04: ZCLCommandDef(
-            "energy_phases_schedule_notification",
-            {
+            direction=True,
+        )
+        energy_phases_schedule_notification: Final = ZCLCommandDef(
+            id=0x04,
+            schema={
                 "power_profile_id": t.uint8_t,
                 "scheduled_phases": t.LVList[ScheduleRecord],
             },
-            False,
-        ),
-        0x05: ZCLCommandDef(
-            "energy_phases_schedule_response",
-            {
+            direction=False,
+        )
+        energy_phases_schedule_response: Final = ZCLCommandDef(
+            id=0x05,
+            schema={
                 "power_profile_id": t.uint8_t,
                 "scheduled_phases": t.LVList[ScheduleRecord],
             },
-            True,
-        ),
-        0x06: ZCLCommandDef(
-            "power_profile_schedule_constraints_request",
-            {"power_profile_id": t.uint8_t},
-            False,
-        ),
-        0x07: ZCLCommandDef(
-            "energy_phases_schedule_state_request",
-            {"power_profile_id": t.uint8_t},
-            False,
-        ),
-        0x08: ZCLCommandDef(
-            "get_power_profile_price_extended_response",
-            {
+            direction=True,
+        )
+        power_profile_schedule_constraints_request: Final = ZCLCommandDef(
+            id=0x06,
+            schema={"power_profile_id": t.uint8_t},
+            direction=False,
+        )
+        energy_phases_schedule_state_request: Final = ZCLCommandDef(
+            id=0x07,
+            schema={"power_profile_id": t.uint8_t},
+            direction=False,
+        )
+        get_power_profile_price_extended_response: Final = ZCLCommandDef(
+            id=0x08,
+            schema={
                 "power_profile_id": t.uint8_t,
                 "currency": t.uint16_t,
                 "price": t.uint32_t,
                 "price_trailing_digit": t.uint8_t,
             },
-            True,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "power_profile_notification",
-            {
+            direction=True,
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        power_profile_notification: Final = ZCLCommandDef(
+            id=0x00,
+            schema={
                 "total_profile_num": t.uint8_t,
                 "power_profile_id": t.uint8_t,
                 "transfer_phases": t.LVList[PowerProfilePhase],
             },
-            False,
-        ),
-        0x01: ZCLCommandDef(
-            "power_profile_response",
-            {
+            direction=False,
+        )
+        power_profile_response: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "total_profile_num": t.uint8_t,
                 "power_profile_id": t.uint8_t,
                 "transfer_phases": t.LVList[PowerProfilePhase],
             },
-            True,
-        ),
-        0x02: ZCLCommandDef(
-            "power_profile_state_response",
-            {"power_profiles": t.LVList[PowerProfile]},
-            True,
-        ),
-        0x03: ZCLCommandDef(
-            "get_power_profile_price", {"power_profile_id": t.uint8_t}, False
-        ),
-        0x04: ZCLCommandDef(
-            "power_profile_state_notification",
-            {"power_profiles": t.LVList[PowerProfile]},
-            False,
-        ),
-        0x05: ZCLCommandDef("get_overall_schedule_price", {}, False),
-        0x06: ZCLCommandDef(
-            "energy_phases_schedule_request",
-            {"power_profile_id": t.uint8_t},
-            False,
-        ),
-        0x07: ZCLCommandDef(
-            "energy_phases_schedule_state_response",
-            {"power_profile_id": t.uint8_t, "num_scheduled_energy_phases": t.uint8_t},
-            True,
-        ),
-        0x08: ZCLCommandDef(
-            "energy_phases_schedule_state_notification",
-            {"power_profile_id": t.uint8_t, "num_scheduled_energy_phases": t.uint8_t},
-            False,
-        ),
-        0x09: ZCLCommandDef(
-            "power_profile_schedule_constraints_notification",
-            {
+            direction=True,
+        )
+        power_profile_state_response: Final = ZCLCommandDef(
+            id=0x02,
+            schema={"power_profiles": t.LVList[PowerProfileType]},
+            direction=True,
+        )
+        get_power_profile_price: Final = ZCLCommandDef(
+            id=0x03, schema={"power_profile_id": t.uint8_t}, direction=False
+        )
+        power_profile_state_notification: Final = ZCLCommandDef(
+            id=0x04,
+            schema={"power_profiles": t.LVList[PowerProfileType]},
+            direction=False,
+        )
+        get_overall_schedule_price: Final = ZCLCommandDef(
+            id=0x05, schema={}, direction=False
+        )
+        energy_phases_schedule_request: Final = ZCLCommandDef(
+            id=0x06,
+            schema={"power_profile_id": t.uint8_t},
+            direction=False,
+        )
+        energy_phases_schedule_state_response: Final = ZCLCommandDef(
+            id=0x07,
+            schema={
+                "power_profile_id": t.uint8_t,
+                "num_scheduled_energy_phases": t.uint8_t,
+            },
+            direction=True,
+        )
+        energy_phases_schedule_state_notification: Final = ZCLCommandDef(
+            id=0x08,
+            schema={
+                "power_profile_id": t.uint8_t,
+                "num_scheduled_energy_phases": t.uint8_t,
+            },
+            direction=False,
+        )
+        power_profile_schedule_constraints_notification: Final = ZCLCommandDef(
+            id=0x09,
+            schema={
                 "power_profile_id": t.uint8_t,
                 "start_after": t.uint16_t,
                 "stop_before": t.uint16_t,
             },
-            False,
-        ),
-        0x0A: ZCLCommandDef(
-            "power_profile_schedule_constraints_response",
-            {
+            direction=False,
+        )
+        power_profile_schedule_constraints_response: Final = ZCLCommandDef(
+            id=0x0A,
+            schema={
                 "power_profile_id": t.uint8_t,
                 "start_after": t.uint16_t,
                 "stop_before": t.uint16_t,
             },
-            True,
-        ),
-        0x0B: ZCLCommandDef(
-            "get_power_profile_price_extended",
-            {
+            direction=True,
+        )
+        get_power_profile_price_extended: Final = ZCLCommandDef(
+            id=0x0B,
+            schema={
                 "options": t.bitmap8,
                 "power_profile_id": t.uint8_t,
                 "power_profile_start_time?": t.uint16_t,
             },
-            False,
-        ),
-    }
+            direction=False,
+        )
 
 
 class ApplianceControl(Cluster):
-    cluster_id = 0x001B
-    ep_attribute = "appliance_control"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "start_time", type=t.uint16_t, access="rp", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef(
-            "finish_time", type=t.uint16_t, access="rp", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef("remaining_time", type=t.uint16_t, access="rp"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x001B
+    ep_attribute: Final = "appliance_control"
+
+    class AttributeDefs(BaseAttributeDefs):
+        start_time: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint16_t, access="rp", mandatory=True
+        )
+        finish_time: Final = ZCLAttributeDef(
+            id=0x0001, type=t.uint16_t, access="rp", mandatory=True
+        )
+        remaining_time: Final = ZCLAttributeDef(id=0x0002, type=t.uint16_t, access="rp")
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class PollControl(Cluster):
-    cluster_id = 0x0020
-    name = "Poll Control"
-    ep_attribute = "poll_control"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "checkin_interval", type=t.uint32_t, access="rw", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef(
-            "long_poll_interval", type=t.uint32_t, access="r", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef(
-            "short_poll_interval", type=t.uint16_t, access="r", mandatory=True
-        ),
-        0x0003: ZCLAttributeDef(
-            "fast_poll_timeout", type=t.uint16_t, access="rw", mandatory=True
-        ),
-        0x0004: ZCLAttributeDef("checkin_interval_min", type=t.uint32_t, access="r"),
-        0x0005: ZCLAttributeDef("long_poll_interval_min", type=t.uint32_t, access="r"),
-        0x0006: ZCLAttributeDef("fast_poll_timeout_max", type=t.uint16_t, access="r"),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "checkin_response",
-            {"start_fast_polling": t.Bool, "fast_poll_timeout": t.uint16_t},
-            True,
-        ),
-        0x01: ZCLCommandDef("fast_poll_stop", {}, False),
-        0x02: ZCLCommandDef(
-            "set_long_poll_interval", {"new_long_poll_interval": t.uint32_t}, False
-        ),
-        0x03: ZCLCommandDef(
-            "set_short_poll_interval",
-            {"new_short_poll_interval": t.uint16_t},
-            False,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x0000: ZCLCommandDef("checkin", {}, False)
-    }
+    cluster_id: Final = 0x0020
+    name: Final = "Poll Control"
+    ep_attribute: Final = "poll_control"
+
+    class AttributeDefs(BaseAttributeDefs):
+        checkin_interval: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint32_t, access="rw", mandatory=True
+        )
+        long_poll_interval: Final = ZCLAttributeDef(
+            id=0x0001, type=t.uint32_t, access="r", mandatory=True
+        )
+        short_poll_interval: Final = ZCLAttributeDef(
+            id=0x0002, type=t.uint16_t, access="r", mandatory=True
+        )
+        fast_poll_timeout: Final = ZCLAttributeDef(
+            id=0x0003, type=t.uint16_t, access="rw", mandatory=True
+        )
+        checkin_interval_min: Final = ZCLAttributeDef(
+            id=0x0004, type=t.uint32_t, access="r"
+        )
+        long_poll_interval_min: Final = ZCLAttributeDef(
+            id=0x0005, type=t.uint32_t, access="r"
+        )
+        fast_poll_timeout_max: Final = ZCLAttributeDef(
+            id=0x0006, type=t.uint16_t, access="r"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        checkin_response: Final = ZCLCommandDef(
+            id=0x00,
+            schema={"start_fast_polling": t.Bool, "fast_poll_timeout": t.uint16_t},
+            direction=True,
+        )
+        fast_poll_stop: Final = ZCLCommandDef(id=0x01, schema={}, direction=False)
+        set_long_poll_interval: Final = ZCLCommandDef(
+            id=0x02, schema={"new_long_poll_interval": t.uint32_t}, direction=False
+        )
+        set_short_poll_interval: Final = ZCLCommandDef(
+            id=0x03,
+            schema={"new_short_poll_interval": t.uint16_t},
+            direction=False,
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        checkin: Final = ZCLCommandDef(id=0x0000, schema={}, direction=False)
 
 
 class GreenPowerProxy(Cluster):
-    cluster_id = 0x0021
-    ep_attribute = "green_power"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0021
+    ep_attribute: Final = "green_power"
```

### Comparing `zigpy-0.55.0/zigpy/zcl/clusters/hvac.py` & `zigpy-0.56.0/zigpy/zcl/clusters/hvac.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,108 +1,130 @@
 """HVAC Functional Domain"""
 
 from __future__ import annotations
 
+from typing import Final
+
 import zigpy.types as t
 from zigpy.zcl import Cluster
-from zigpy.zcl.foundation import ZCLAttributeDef, ZCLCommandDef
+from zigpy.zcl.foundation import (
+    BaseAttributeDefs,
+    BaseCommandDefs,
+    ZCLAttributeDef,
+    ZCLCommandDef,
+)
+
+
+class PumpAlarmMask(t.bitmap16):
+    Supply_voltage_too_low = 0x0001
+    Supply_voltage_too_high = 0x0002
+    Power_missing_phase = 0x0004
+    System_pressure_too_low = 0x0008
+    System_pressure_too_high = 0x0010
+    Dry_running = 0x0020
+    Motor_temperature_too_high = 0x0040
+    Pump_motor_has_fatal_failure = 0x0080
+    Electronic_temperature_too_high = 0x0100
+    Pump_blocked = 0x0200
+    Sensor_failure = 0x0400
+    Electronic_non_fatal_failure = 0x0800
+    Electronic_fatal_failure = 0x1000
+    General_fault = 0x2000
+
+
+class ControlMode(t.enum8):
+    Constant_speed = 0x00
+    Constant_pressure = 0x01
+    Proportional_pressure = 0x02
+    Constant_flow = 0x03
+    Constant_temperature = 0x05
+    Automatic = 0x07
+
+
+class OperationMode(t.enum8):
+    Normal = 0x00
+    Minimum = 0x01
+    Maximum = 0x02
+    Local = 0x03
+
+
+class PumpStatus(t.bitmap16):
+    Device_fault = 0x0001
+    Supply_fault = 0x0002
+    Speed_low = 0x0004
+    Speed_high = 0x0008
+    Local_override = 0x0010
+    Running = 0x0020
+    Remote_Pressure = 0x0040
+    Remote_Flow = 0x0080
+    Remote_Temperature = 0x0100
 
 
 class Pump(Cluster):
     """An interface for configuring and controlling pumps."""
 
-    class AlarmMask(t.bitmap16):
-        Supply_voltage_too_low = 0x0001
-        Supply_voltage_too_high = 0x0002
-        Power_missing_phase = 0x0004
-        System_pressure_too_low = 0x0008
-        System_pressure_too_high = 0x0010
-        Dry_running = 0x0020
-        Motor_temperature_too_high = 0x0040
-        Pump_motor_has_fatal_failure = 0x0080
-        Electronic_temperature_too_high = 0x0100
-        Pump_blocked = 0x0200
-        Sensor_failure = 0x0400
-        Electronic_non_fatal_failure = 0x0800
-        Electronic_fatal_failure = 0x1000
-        General_fault = 0x2000
-
-    class ControlMode(t.enum8):
-        Constant_speed = 0x00
-        Constant_pressure = 0x01
-        Proportional_pressure = 0x02
-        Constant_flow = 0x03
-        Constant_temperature = 0x05
-        Automatic = 0x07
-
-    class OperationMode(t.enum8):
-        Normal = 0x00
-        Minimum = 0x01
-        Maximum = 0x02
-        Local = 0x03
-
-    class PumpStatus(t.bitmap16):
-        Device_fault = 0x0001
-        Supply_fault = 0x0002
-        Speed_low = 0x0004
-        Speed_high = 0x0008
-        Local_override = 0x0010
-        Running = 0x0020
-        Remote_Pressure = 0x0040
-        Remote_Flow = 0x0080
-        Remote_Temperature = 0x0100
-
-    cluster_id = 0x0200
-    name = "Pump Configuration and Control"
-    ep_attribute = "pump"
-    attributes: dict[int, ZCLAttributeDef] = {
+    AlarmMask: Final = PumpAlarmMask
+    ControlMode: Final = ControlMode
+    OperationMode: Final = OperationMode
+    PumpStatus: Final = PumpStatus
+
+    cluster_id: Final = 0x0200
+    name: Final = "Pump Configuration and Control"
+    ep_attribute: Final = "pump"
+
+    class AttributeDefs(BaseAttributeDefs):
         # Pump Information
-        0x0000: ZCLAttributeDef(
-            "max_pressure", type=t.int16s, access="r", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef(
-            "max_speed", type=t.uint16_t, access="r", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef(
-            "max_flow", type=t.uint16_t, access="r", mandatory=True
-        ),
-        0x0003: ZCLAttributeDef("min_const_pressure", type=t.int16s, access="r"),
-        0x0004: ZCLAttributeDef("max_const_pressure", type=t.int16s, access="r"),
-        0x0005: ZCLAttributeDef("min_comp_pressure", type=t.int16s, access="r"),
-        0x0006: ZCLAttributeDef("max_comp_pressure", type=t.int16s, access="r"),
-        0x0007: ZCLAttributeDef("min_const_speed", type=t.uint16_t, access="r"),
-        0x0008: ZCLAttributeDef("max_const_speed", type=t.uint16_t, access="r"),
-        0x0009: ZCLAttributeDef("min_const_flow", type=t.uint16_t, access="r"),
-        0x000A: ZCLAttributeDef("max_const_flow", type=t.uint16_t, access="r"),
-        0x000B: ZCLAttributeDef("min_const_temp", type=t.int16s, access="r"),
-        0x000C: ZCLAttributeDef("max_const_temp", type=t.int16s, access="r"),
+        max_pressure: Final = ZCLAttributeDef(
+            id=0x0000, type=t.int16s, access="r", mandatory=True
+        )
+        max_speed: Final = ZCLAttributeDef(
+            id=0x0001, type=t.uint16_t, access="r", mandatory=True
+        )
+        max_flow: Final = ZCLAttributeDef(
+            id=0x0002, type=t.uint16_t, access="r", mandatory=True
+        )
+        min_const_pressure: Final = ZCLAttributeDef(
+            id=0x0003, type=t.int16s, access="r"
+        )
+        max_const_pressure: Final = ZCLAttributeDef(
+            id=0x0004, type=t.int16s, access="r"
+        )
+        min_comp_pressure: Final = ZCLAttributeDef(id=0x0005, type=t.int16s, access="r")
+        max_comp_pressure: Final = ZCLAttributeDef(id=0x0006, type=t.int16s, access="r")
+        min_const_speed: Final = ZCLAttributeDef(id=0x0007, type=t.uint16_t, access="r")
+        max_const_speed: Final = ZCLAttributeDef(id=0x0008, type=t.uint16_t, access="r")
+        min_const_flow: Final = ZCLAttributeDef(id=0x0009, type=t.uint16_t, access="r")
+        max_const_flow: Final = ZCLAttributeDef(id=0x000A, type=t.uint16_t, access="r")
+        min_const_temp: Final = ZCLAttributeDef(id=0x000B, type=t.int16s, access="r")
+        max_const_temp: Final = ZCLAttributeDef(id=0x000C, type=t.int16s, access="r")
         # Pump Dynamic Information
-        0x0010: ZCLAttributeDef("pump_status", type=PumpStatus, access="rp"),
-        0x0011: ZCLAttributeDef(
-            "effective_operation_mode", type=OperationMode, access="r", mandatory=True
-        ),
-        0x0012: ZCLAttributeDef(
-            "effective_control_mode", type=ControlMode, access="r", mandatory=True
-        ),
-        0x0013: ZCLAttributeDef("capacity", type=t.int16s, access="rp", mandatory=True),
-        0x0014: ZCLAttributeDef("speed", type=t.uint16_t, access="r"),
-        0x0015: ZCLAttributeDef("lifetime_running_hours", type=t.uint24_t, access="rw"),
-        0x0016: ZCLAttributeDef("power", type=t.uint24_t, access="rw"),
-        0x0017: ZCLAttributeDef(
-            "lifetime_energy_consumed", type=t.uint32_t, access="r"
-        ),
+        pump_status: Final = ZCLAttributeDef(id=0x0010, type=PumpStatus, access="rp")
+        effective_operation_mode: Final = ZCLAttributeDef(
+            id=0x0011, type=OperationMode, access="r", mandatory=True
+        )
+        effective_control_mode: Final = ZCLAttributeDef(
+            id=0x0012, type=ControlMode, access="r", mandatory=True
+        )
+        capacity: Final = ZCLAttributeDef(
+            id=0x0013, type=t.int16s, access="rp", mandatory=True
+        )
+        speed: Final = ZCLAttributeDef(id=0x0014, type=t.uint16_t, access="r")
+        lifetime_running_hours: Final = ZCLAttributeDef(
+            id=0x0015, type=t.uint24_t, access="rw"
+        )
+        power: Final = ZCLAttributeDef(id=0x0016, type=t.uint24_t, access="rw")
+        lifetime_energy_consumed: Final = ZCLAttributeDef(
+            id=0x0017, type=t.uint32_t, access="r"
+        )
         # Pump Settings
-        0x0020: ZCLAttributeDef(
-            "operation_mode", type=OperationMode, access="rw", mandatory=True
-        ),
-        0x0021: ZCLAttributeDef("control_mode", type=ControlMode, access="rw"),
-        0x0022: ZCLAttributeDef("alarm_mask", type=AlarmMask, access="r"),
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        operation_mode: Final = ZCLAttributeDef(
+            id=0x0020, type=OperationMode, access="rw", mandatory=True
+        )
+        control_mode: Final = ZCLAttributeDef(id=0x0021, type=ControlMode, access="rw")
+        alarm_mask: Final = ZCLAttributeDef(id=0x0022, type=PumpAlarmMask, access="r")
 
 
 class CoolingSystemStage(t.enum8):
     Cool_Stage_1 = 0x00
     Cool_Stage_2 = 0x01
     Cool_Stage_3 = 0x02
     Reserved = 0x03
@@ -121,448 +143,544 @@
 
 
 class HeatingFuelSource(t.enum8):
     Electric = 0x00
     Gas = 0x01
 
 
+class ACCapacityFormat(t.enum8):
+    BTUh = 0x00
+
+
+class ACCompressorType(t.enum8):
+    Reserved = 0x00
+    T1_max_working_43C = 0x01
+    T2_max_working_35C = 0x02
+    T3_max_working_52C = 0x03
+
+
+class ACType(t.enum8):
+    Reserved = 0x00
+    Cooling_fixed_speed = 0x01
+    Heat_Pump_fixed_speed = 0x02
+    Cooling_Inverter = 0x03
+    Heat_Pump_Inverter = 0x04
+
+
+class ACRefrigerantType(t.enum8):
+    Reserved = 0x00
+    R22 = 0x01
+    R410a = 0x02
+    R407c = 0x03
+
+
+class ACErrorCode(t.bitmap32):
+    No_Errors = 0x00000000
+    Commpressor_Failure = 0x00000001
+    Room_Temperature_Sensor_Failure = 0x00000002
+    Outdoor_Temperature_Sensor_Failure = 0x00000004
+    Indoor_Coil_Temperature_Sensor_Failure = 0x00000008
+    Fan_Failure = 0x00000010
+
+
+class ACLouverPosition(t.enum8):
+    Closed = 0x01
+    Open = 0x02
+    Qurter_Open = 0x03
+    Half_Open = 0x04
+    Three_Quarters_Open = 0x05
+
+
+class AlarmMask(t.bitmap8):
+    No_Alarms = 0x00
+    Initialization_failure = 0x01
+    Hardware_failure = 0x02
+    Self_calibration_failure = 0x04
+
+
+class ControlSequenceOfOperation(t.enum8):
+    Cooling_Only = 0x00
+    Cooling_With_Reheat = 0x01
+    Heating_Only = 0x02
+    Heating_With_Reheat = 0x03
+    Cooling_and_Heating = 0x04
+    Cooling_and_Heating_with_Reheat = 0x05
+
+
+class SeqDayOfWeek(t.bitmap8):
+    Sunday = 0x01
+    Monday = 0x02
+    Tuesday = 0x04
+    Wednesday = 0x08
+    Thursday = 0x10
+    Friday = 0x20
+    Saturday = 0x40
+    Away = 0x80
+
+
+class SeqMode(t.bitmap8):
+    Heat = 0x01
+    Cool = 0x02
+
+
+class Occupancy(t.bitmap8):
+    Unoccupied = 0x00
+    Occupied = 0x01
+
+
+class ProgrammingOperationMode(t.bitmap8):
+    Simple = 0x00
+    Schedule_programming_mode = 0x01
+    Auto_recovery_mode = 0x02
+    Economy_mode = 0x04
+
+
+class RemoteSensing(t.bitmap8):
+    all_local = 0x00
+    local_temperature_sensed_remotely = 0x01
+    outdoor_temperature_sensed_remotely = 0x02
+    occupancy_sensed_remotely = 0x04
+
+
+class SetpointChangeSource(t.enum8):
+    Manual = 0x00
+    Schedule = 0x01
+    External = 0x02
+
+
+class SetpointMode(t.enum8):
+    Heat = 0x00
+    Cool = 0x01
+    Both = 0x02
+
+
+class StartOfWeek(t.enum8):
+    Sunday = 0x00
+    Monday = 0x01
+    Tuesday = 0x02
+    Wednesday = 0x03
+    Thursday = 0x04
+    Friday = 0x05
+    Saturday = 0x06
+
+
+class SystemMode(t.enum8):
+    Off = 0x00
+    Auto = 0x01
+    Cool = 0x03
+    Heat = 0x04
+    Emergency_Heating = 0x05
+    Pre_cooling = 0x06
+    Fan_only = 0x07
+    Dry = 0x08
+    Sleep = 0x09
+
+
+class SystemType(t.bitmap8):
+    Heat_and_or_Cool_Stage_1 = 0x00
+    Cool_Stage_1 = 0x01
+    Cool_Stage_2 = 0x02
+    Heat_Stage_1 = 0x04
+    Heat_Stage_2 = 0x08
+    Heat_Pump = 0x10
+    Gas = 0x20
+
+    @property
+    def cooling_system_stage(self) -> CoolingSystemStage:
+        return CoolingSystemStage(self & 0x03)
+
+    @property
+    def heating_system_stage(self) -> HeatingSystemStage:
+        return HeatingSystemStage((self >> 2) & 0x03)
+
+    @property
+    def heating_system_type(self) -> HeatingSystemType:
+        return HeatingSystemType((self >> 4) & 0x01)
+
+    @property
+    def heating_fuel_source(self) -> HeatingFuelSource:
+        return HeatingFuelSource((self >> 5) & 0x01)
+
+
+class TemperatureSetpointHold(t.enum8):
+    Setpoint_Hold_Off = 0x00
+    Setpoint_Hold_On = 0x01
+
+
+class RunningMode(t.enum8):
+    Off = 0x00
+    Cool = 0x03
+    Heat = 0x04
+
+
+class RunningState(t.bitmap16):
+    Idle = 0x0000
+    Heat_State_On = 0x0001
+    Cool_State_On = 0x0002
+    Fan_State_On = 0x0004
+    Heat_2nd_Stage_On = 0x0008
+    Cool_2nd_Stage_On = 0x0010
+    Fan_2nd_Stage_On = 0x0020
+    Fan_3rd_Stage_On = 0x0040
+
+
 class Thermostat(Cluster):
     """An interface for configuring and controlling the
     functionality of a thermostat.
     """
 
-    class ACCapacityFormat(t.enum8):
-        BTUh = 0x00
+    ACCapacityFormat: Final = ACCapacityFormat
+    ACErrorCode: Final = ACErrorCode
+    ACLouverPosition: Final = ACLouverPosition
+    AlarmMask: Final = AlarmMask
+    ControlSequenceOfOperation: Final = ControlSequenceOfOperation
+    SeqDayOfWeek: Final = SeqDayOfWeek
+    SeqMode: Final = SeqMode
+    Occupancy: Final = Occupancy
+    ProgrammingOperationMode: Final = ProgrammingOperationMode
+    RemoteSensing: Final = RemoteSensing
+    SetpointChangeSource: Final = SetpointChangeSource
+    SetpointMode: Final = SetpointMode
+    StartOfWeek: Final = StartOfWeek
+    SystemMode: Final = SystemMode
+    SystemType: Final = SystemType
+    TemperatureSetpointHold: Final = TemperatureSetpointHold
+    RunningMode: Final = RunningMode
+    RunningState: Final = RunningState
 
-    class ACCompressorType(t.enum8):
-        Reserved = 0x00
-        T1_max_working_43C = 0x01
-        T2_max_working_35C = 0x02
-        T3_max_working_52C = 0x03
-
-    class ACType(t.enum8):
-        Reserved = 0x00
-        Cooling_fixed_speed = 0x01
-        Heat_Pump_fixed_speed = 0x02
-        Cooling_Inverter = 0x03
-        Heat_Pump_Inverter = 0x04
-
-    class ACRefrigerantType(t.enum8):
-        Reserved = 0x00
-        R22 = 0x01
-        R410a = 0x02
-        R407c = 0x03
-
-    class ACErrorCode(t.bitmap32):
-        No_Errors = 0x00000000
-        Commpressor_Failure = 0x00000001
-        Room_Temperature_Sensor_Failure = 0x00000002
-        Outdoor_Temperature_Sensor_Failure = 0x00000004
-        Indoor_Coil_Temperature_Sensor_Failure = 0x00000008
-        Fan_Failure = 0x00000010
-
-    class ACLouverPosition(t.enum8):
-        Closed = 0x01
-        Open = 0x02
-        Qurter_Open = 0x03
-        Half_Open = 0x04
-        Three_Quarters_Open = 0x05
-
-    class AlarmMask(t.bitmap8):
-        No_Alarms = 0x00
-        Initialization_failure = 0x01
-        Hardware_failure = 0x02
-        Self_calibration_failure = 0x04
-
-    class ControlSequenceOfOperation(t.enum8):
-        Cooling_Only = 0x00
-        Cooling_With_Reheat = 0x01
-        Heating_Only = 0x02
-        Heating_With_Reheat = 0x03
-        Cooling_and_Heating = 0x04
-        Cooling_and_Heating_with_Reheat = 0x05
-
-    class SeqDayOfWeek(t.bitmap8):
-        Sunday = 0x01
-        Monday = 0x02
-        Tuesday = 0x04
-        Wednesday = 0x08
-        Thursday = 0x10
-        Friday = 0x20
-        Saturday = 0x40
-        Away = 0x80
-
-    class SeqMode(t.bitmap8):
-        Heat = 0x01
-        Cool = 0x02
-
-    class Occupancy(t.bitmap8):
-        Unoccupied = 0x00
-        Occupied = 0x01
-
-    class ProgrammingOperationMode(t.bitmap8):
-        Simple = 0x00
-        Schedule_programming_mode = 0x01
-        Auto_recovery_mode = 0x02
-        Economy_mode = 0x04
-
-    class RemoteSensing(t.bitmap8):
-        all_local = 0x00
-        local_temperature_sensed_remotely = 0x01
-        outdoor_temperature_sensed_remotely = 0x02
-        occupancy_sensed_remotely = 0x04
-
-    class SetpointChangeSource(t.enum8):
-        Manual = 0x00
-        Schedule = 0x01
-        External = 0x02
-
-    class SetpointMode(t.enum8):
-        Heat = 0x00
-        Cool = 0x01
-        Both = 0x02
-
-    class StartOfWeek(t.enum8):
-        Sunday = 0x00
-        Monday = 0x01
-        Tuesday = 0x02
-        Wednesday = 0x03
-        Thursday = 0x04
-        Friday = 0x05
-        Saturday = 0x06
-
-    class SystemMode(t.enum8):
-        Off = 0x00
-        Auto = 0x01
-        Cool = 0x03
-        Heat = 0x04
-        Emergency_Heating = 0x05
-        Pre_cooling = 0x06
-        Fan_only = 0x07
-        Dry = 0x08
-        Sleep = 0x09
-
-    class SystemType(t.bitmap8):
-        Heat_and_or_Cool_Stage_1 = 0x00
-        Cool_Stage_1 = 0x01
-        Cool_Stage_2 = 0x02
-        Heat_Stage_1 = 0x04
-        Heat_Stage_2 = 0x08
-        Heat_Pump = 0x10
-        Gas = 0x20
-
-        @property
-        def cooling_system_stage(self) -> CoolingSystemStage:
-            return CoolingSystemStage(self & 0x03)
-
-        @property
-        def heating_system_stage(self) -> HeatingSystemStage:
-            return HeatingSystemStage((self >> 2) & 0x03)
-
-        @property
-        def heating_system_type(self) -> HeatingSystemType:
-            return HeatingSystemType((self >> 4) & 0x01)
-
-        @property
-        def heating_fuel_source(self) -> HeatingFuelSource:
-            return HeatingFuelSource((self >> 5) & 0x01)
-
-    class TemperatureSetpointHold(t.enum8):
-        Setpoint_Hold_Off = 0x00
-        Setpoint_Hold_On = 0x01
-
-    class RunningMode(t.enum8):
-        Off = 0x00
-        Cool = 0x03
-        Heat = 0x04
-
-    class RunningState(t.bitmap16):
-        Idle = 0x0000
-        Heat_State_On = 0x0001
-        Cool_State_On = 0x0002
-        Fan_State_On = 0x0004
-        Heat_2nd_Stage_On = 0x0008
-        Cool_2nd_Stage_On = 0x0010
-        Fan_2nd_Stage_On = 0x0020
-        Fan_3rd_Stage_On = 0x0040
-
-    cluster_id = 0x0201
-    ep_attribute = "thermostat"
-    attributes: dict[int, ZCLAttributeDef] = {
+    cluster_id: Final = 0x0201
+    ep_attribute: Final = "thermostat"
+
+    class AttributeDefs(BaseAttributeDefs):
         # Thermostat Information
-        0x0000: ZCLAttributeDef(
-            "local_temperature", type=t.int16s, access="rp", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef("outdoor_temperature", type=t.int16s, access="r"),
-        0x0002: ZCLAttributeDef("occupancy", type=Occupancy, access="r"),
-        0x0003: ZCLAttributeDef(
-            "abs_min_heat_setpoint_limit", type=t.int16s, access="r"
-        ),
-        0x0004: ZCLAttributeDef(
-            "abs_max_heat_setpoint_limit", type=t.int16s, access="r"
-        ),
-        0x0005: ZCLAttributeDef(
-            "abs_min_cool_setpoint_limit", type=t.int16s, access="r"
-        ),
-        0x0006: ZCLAttributeDef(
-            "abs_max_cool_setpoint_limit", type=t.int16s, access="r"
-        ),
-        0x0007: ZCLAttributeDef("pi_cooling_demand", type=t.uint8_t, access="rp"),
-        0x0008: ZCLAttributeDef("pi_heating_demand", type=t.uint8_t, access="rp"),
-        0x0009: ZCLAttributeDef("system_type_config", type=SystemType, access="r*w"),
+        local_temperature: Final = ZCLAttributeDef(
+            id=0x0000, type=t.int16s, access="rp", mandatory=True
+        )
+        outdoor_temperature: Final = ZCLAttributeDef(
+            id=0x0001, type=t.int16s, access="r"
+        )
+        occupancy: Final = ZCLAttributeDef(id=0x0002, type=Occupancy, access="r")
+        abs_min_heat_setpoint_limit: Final = ZCLAttributeDef(
+            id=0x0003, type=t.int16s, access="r"
+        )
+        abs_max_heat_setpoint_limit: Final = ZCLAttributeDef(
+            id=0x0004, type=t.int16s, access="r"
+        )
+        abs_min_cool_setpoint_limit: Final = ZCLAttributeDef(
+            id=0x0005, type=t.int16s, access="r"
+        )
+        abs_max_cool_setpoint_limit: Final = ZCLAttributeDef(
+            id=0x0006, type=t.int16s, access="r"
+        )
+        pi_cooling_demand: Final = ZCLAttributeDef(
+            id=0x0007, type=t.uint8_t, access="rp"
+        )
+        pi_heating_demand: Final = ZCLAttributeDef(
+            id=0x0008, type=t.uint8_t, access="rp"
+        )
+        system_type_config: Final = ZCLAttributeDef(
+            id=0x0009, type=SystemType, access="r*w"
+        )
         # Thermostat Settings
-        0x0010: ZCLAttributeDef(
-            "local_temperature_calibration", type=t.int8s, access="rw"
-        ),
+        local_temperature_calibration: Final = ZCLAttributeDef(
+            id=0x0010, type=t.int8s, access="rw"
+        )
         # At least one of these two attribute sets will be available
-        0x0011: ZCLAttributeDef(
-            "occupied_cooling_setpoint", type=t.int16s, access="rws"
-        ),
-        0x0012: ZCLAttributeDef(
-            "occupied_heating_setpoint", type=t.int16s, access="rws"
-        ),
-        0x0013: ZCLAttributeDef(
-            "unoccupied_cooling_setpoint", type=t.int16s, access="rw"
-        ),
-        0x0014: ZCLAttributeDef(
-            "unoccupied_heating_setpoint", type=t.int16s, access="rw"
-        ),
-        0x0015: ZCLAttributeDef("min_heat_setpoint_limit", type=t.int16s, access="rw"),
-        0x0016: ZCLAttributeDef("max_heat_setpoint_limit", type=t.int16s, access="rw"),
-        0x0017: ZCLAttributeDef("min_cool_setpoint_limit", type=t.int16s, access="rw"),
-        0x0018: ZCLAttributeDef("max_cool_setpoint_limit", type=t.int16s, access="rw"),
-        0x0019: ZCLAttributeDef("min_setpoint_dead_band", type=t.int8s, access="r*w"),
-        0x001A: ZCLAttributeDef("remote_sensing", type=RemoteSensing, access="rw"),
-        0x001B: ZCLAttributeDef(
-            "ctrl_sequence_of_oper",
+        occupied_cooling_setpoint: Final = ZCLAttributeDef(
+            id=0x0011, type=t.int16s, access="rws"
+        )
+        occupied_heating_setpoint: Final = ZCLAttributeDef(
+            id=0x0012, type=t.int16s, access="rws"
+        )
+        unoccupied_cooling_setpoint: Final = ZCLAttributeDef(
+            id=0x0013, type=t.int16s, access="rw"
+        )
+        unoccupied_heating_setpoint: Final = ZCLAttributeDef(
+            id=0x0014, type=t.int16s, access="rw"
+        )
+        min_heat_setpoint_limit: Final = ZCLAttributeDef(
+            id=0x0015, type=t.int16s, access="rw"
+        )
+        max_heat_setpoint_limit: Final = ZCLAttributeDef(
+            id=0x0016, type=t.int16s, access="rw"
+        )
+        min_cool_setpoint_limit: Final = ZCLAttributeDef(
+            id=0x0017, type=t.int16s, access="rw"
+        )
+        max_cool_setpoint_limit: Final = ZCLAttributeDef(
+            id=0x0018, type=t.int16s, access="rw"
+        )
+        min_setpoint_dead_band: Final = ZCLAttributeDef(
+            id=0x0019, type=t.int8s, access="r*w"
+        )
+        remote_sensing: Final = ZCLAttributeDef(
+            id=0x001A, type=RemoteSensing, access="rw"
+        )
+        ctrl_sequence_of_oper: Final = ZCLAttributeDef(
+            id=0x001B,
             type=ControlSequenceOfOperation,
             access="rw",
             mandatory=True,
-        ),
-        0x001C: ZCLAttributeDef(
-            "system_mode", type=SystemMode, access="rws", mandatory=True
-        ),
-        0x001D: ZCLAttributeDef("alarm_mask", type=AlarmMask, access="r"),
-        0x001E: ZCLAttributeDef("running_mode", type=RunningMode, access="r"),
+        )
+        system_mode: Final = ZCLAttributeDef(
+            id=0x001C, type=SystemMode, access="rws", mandatory=True
+        )
+        alarm_mask: Final = ZCLAttributeDef(id=0x001D, type=AlarmMask, access="r")
+        running_mode: Final = ZCLAttributeDef(id=0x001E, type=RunningMode, access="r")
         # Schedule
-        0x0020: ZCLAttributeDef("start_of_week", type=StartOfWeek, access="r"),
-        0x0021: ZCLAttributeDef(
-            "number_of_weekly_transitions", type=t.uint8_t, access="r"
-        ),
-        0x0022: ZCLAttributeDef(
-            "number_of_daily_transitions", type=t.uint8_t, access="r"
-        ),
-        0x0023: ZCLAttributeDef(
-            "temp_setpoint_hold", type=TemperatureSetpointHold, access="rw"
-        ),
-        0x0024: ZCLAttributeDef(
-            "temp_setpoint_hold_duration", type=t.uint16_t, access="rw"
-        ),
-        0x0025: ZCLAttributeDef(
-            "programing_oper_mode", type=ProgrammingOperationMode, access="rwp"
-        ),
+        start_of_week: Final = ZCLAttributeDef(id=0x0020, type=StartOfWeek, access="r")
+        number_of_weekly_transitions: Final = ZCLAttributeDef(
+            id=0x0021, type=t.uint8_t, access="r"
+        )
+        number_of_daily_transitions: Final = ZCLAttributeDef(
+            id=0x0022, type=t.uint8_t, access="r"
+        )
+        temp_setpoint_hold: Final = ZCLAttributeDef(
+            id=0x0023, type=TemperatureSetpointHold, access="rw"
+        )
+        temp_setpoint_hold_duration: Final = ZCLAttributeDef(
+            id=0x0024, type=t.uint16_t, access="rw"
+        )
+        programing_oper_mode: Final = ZCLAttributeDef(
+            id=0x0025, type=ProgrammingOperationMode, access="rwp"
+        )
         # HVAC Relay
-        0x0029: ZCLAttributeDef("running_state", type=RunningState, access="r"),
+        running_state: Final = ZCLAttributeDef(id=0x0029, type=RunningState, access="r")
         # Thermostat Setpoint Change Tracking
-        0x0030: ZCLAttributeDef(
-            "setpoint_change_source", type=SetpointChangeSource, access="r"
-        ),
-        0x0031: ZCLAttributeDef("setpoint_change_amount", type=t.int16s, access="r"),
-        0x0032: ZCLAttributeDef(
-            "setpoint_change_source_timestamp", type=t.UTCTime, access="r"
-        ),
-        0x0034: ZCLAttributeDef("occupied_setback", type=t.uint8_t, access="rw"),
-        0x0035: ZCLAttributeDef("occupied_setback_min", type=t.uint8_t, access="r"),
-        0x0036: ZCLAttributeDef("occupied_setback_max", type=t.uint8_t, access="r"),
-        0x0037: ZCLAttributeDef("unoccupied_setback", type=t.uint8_t, access="rw"),
-        0x0038: ZCLAttributeDef("unoccupied_setback_min", type=t.uint8_t, access="r"),
-        0x0039: ZCLAttributeDef("unoccupied_setback_max", type=t.uint8_t, access="r"),
-        0x003A: ZCLAttributeDef("emergency_heat_delta", type=t.uint8_t, access="rw"),
+        setpoint_change_source: Final = ZCLAttributeDef(
+            id=0x0030, type=SetpointChangeSource, access="r"
+        )
+        setpoint_change_amount: Final = ZCLAttributeDef(
+            id=0x0031, type=t.int16s, access="r"
+        )
+        setpoint_change_source_timestamp: Final = ZCLAttributeDef(
+            id=0x0032, type=t.UTCTime, access="r"
+        )
+        occupied_setback: Final = ZCLAttributeDef(
+            id=0x0034, type=t.uint8_t, access="rw"
+        )
+        occupied_setback_min: Final = ZCLAttributeDef(
+            id=0x0035, type=t.uint8_t, access="r"
+        )
+        occupied_setback_max: Final = ZCLAttributeDef(
+            id=0x0036, type=t.uint8_t, access="r"
+        )
+        unoccupied_setback: Final = ZCLAttributeDef(
+            id=0x0037, type=t.uint8_t, access="rw"
+        )
+        unoccupied_setback_min: Final = ZCLAttributeDef(
+            id=0x0038, type=t.uint8_t, access="r"
+        )
+        unoccupied_setback_max: Final = ZCLAttributeDef(
+            id=0x0039, type=t.uint8_t, access="r"
+        )
+        emergency_heat_delta: Final = ZCLAttributeDef(
+            id=0x003A, type=t.uint8_t, access="rw"
+        )
         # AC Information
-        0x0040: ZCLAttributeDef("ac_type", type=ACType, access="rw"),
-        0x0041: ZCLAttributeDef("ac_capacity", type=t.uint16_t, access="rw"),
-        0x0042: ZCLAttributeDef(
-            "ac_refrigerant_type", type=ACRefrigerantType, access="rw"
-        ),
-        0x0043: ZCLAttributeDef(
-            "ac_compressor_type", type=ACCompressorType, access="rw"
-        ),
-        0x0044: ZCLAttributeDef("ac_error_code", type=ACErrorCode, access="rw"),
-        0x0045: ZCLAttributeDef(
-            "ac_louver_position", type=ACLouverPosition, access="rw"
-        ),
-        0x0046: ZCLAttributeDef("ac_coil_temperature", type=t.int16s, access="r"),
-        0x0047: ZCLAttributeDef(
-            "ac_capacity_format", type=ACCapacityFormat, access="rw"
-        ),
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "setpoint_raise_lower", {"mode": SetpointMode, "amount": t.int8s}, False
-        ),
-        0x01: ZCLCommandDef(
-            "set_weekly_schedule",
-            {
+        ac_type: Final = ZCLAttributeDef(id=0x0040, type=ACType, access="rw")
+        ac_capacity: Final = ZCLAttributeDef(id=0x0041, type=t.uint16_t, access="rw")
+        ac_refrigerant_type: Final = ZCLAttributeDef(
+            id=0x0042, type=ACRefrigerantType, access="rw"
+        )
+        ac_compressor_type: Final = ZCLAttributeDef(
+            id=0x0043, type=ACCompressorType, access="rw"
+        )
+        ac_error_code: Final = ZCLAttributeDef(id=0x0044, type=ACErrorCode, access="rw")
+        ac_louver_position: Final = ZCLAttributeDef(
+            id=0x0045, type=ACLouverPosition, access="rw"
+        )
+        ac_coil_temperature: Final = ZCLAttributeDef(
+            id=0x0046, type=t.int16s, access="r"
+        )
+        ac_capacity_format: Final = ZCLAttributeDef(
+            id=0x0047, type=ACCapacityFormat, access="rw"
+        )
+
+    class ServerCommandDefs(BaseCommandDefs):
+        setpoint_raise_lower: Final = ZCLCommandDef(
+            id=0x00, schema={"mode": SetpointMode, "amount": t.int8s}, direction=False
+        )
+        set_weekly_schedule: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "num_transitions_for_sequence": t.enum8,
                 "day_of_week_for_sequence": SeqDayOfWeek,
                 "mode_for_sequence": SeqMode,
                 "values": t.List[t.int16s],
-            },  # TODO: properly parse values
-            False,
-        ),
-        0x02: ZCLCommandDef(
-            "get_weekly_schedule",
-            {"days_to_return": SeqDayOfWeek, "mode_to_return": SeqMode},
-            False,
-        ),
-        0x03: ZCLCommandDef("clear_weekly_schedule", {}, False),
-        0x04: ZCLCommandDef("get_relay_status_log", {}, False),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "get_weekly_schedule_response",
-            {
+            },
+            direction=False,
+        )
+        get_weekly_schedule: Final = ZCLCommandDef(
+            id=0x02,
+            schema={"days_to_return": SeqDayOfWeek, "mode_to_return": SeqMode},
+            direction=False,
+        )
+        clear_weekly_schedule: Final = ZCLCommandDef(
+            id=0x03, schema={}, direction=False
+        )
+        get_relay_status_log: Final = ZCLCommandDef(id=0x04, schema={}, direction=False)
+
+    class ClientCommandDefs(BaseCommandDefs):
+        get_weekly_schedule_response: Final = ZCLCommandDef(
+            id=0x00,
+            schema={
                 "num_transitions_for_sequence": t.enum8,
                 "day_of_week_for_sequence": SeqDayOfWeek,
                 "mode_for_sequence": SeqMode,
                 "values": t.List[t.int16s],
-            },  # TODO: properly parse values
-            True,
-        ),
-        0x01: ZCLCommandDef(
-            "get_relay_status_log_response",
-            {
+            },
+            direction=True,
+        )
+        get_relay_status_log_response: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "time_of_day": t.uint16_t,
                 "relay_status": t.bitmap8,
                 "local_temperature": t.int16s,
                 "humidity_in_percentage": t.uint8_t,
                 "set_point": t.int16s,
                 "unread_entries": t.uint16_t,
             },
-            True,
-        ),
-    }
+            direction=True,
+        )
+
+
+class FanMode(t.enum8):
+    Off = 0x00
+    Low = 0x01
+    Medium = 0x02
+    High = 0x03
+    On = 0x04
+    Auto = 0x05
+    Smart = 0x06
+
+
+class FanModeSequence(t.enum8):
+    Low_Med_High = 0x00
+    Low_High = 0x01
+    Low_Med_High_Auto = 0x02
+    Low_High_Auto = 0x03
+    On_Auto = 0x04
 
 
 class Fan(Cluster):
     """An interface for controlling a fan in a heating /
     cooling system.
     """
 
-    class FanMode(t.enum8):
-        Off = 0x00
-        Low = 0x01
-        Medium = 0x02
-        High = 0x03
-        On = 0x04
-        Auto = 0x05
-        Smart = 0x06
-
-    class FanModeSequence(t.enum8):
-        Low_Med_High = 0x00
-        Low_High = 0x01
-        Low_Med_High_Auto = 0x02
-        Low_High_Auto = 0x03
-        On_Auto = 0x04
-
-    cluster_id = 0x0202
-    name = "Fan Control"
-    ep_attribute = "fan"
-    attributes: dict[int, ZCLAttributeDef] = {
-        # Fan Control Status
-        0x0000: ZCLAttributeDef("fan_mode", type=FanMode, access=""),
-        0x0001: ZCLAttributeDef("fan_mode_sequence", type=FanModeSequence, access=""),
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    FanMode: Final = FanMode
+    FanModeSequence: Final = FanModeSequence
+
+    cluster_id: Final = 0x0202
+    name: Final = "Fan Control"
+    ep_attribute: Final = "fan"
+
+    class AttributeDefs(BaseAttributeDefs):
+        fan_mode: Final = ZCLAttributeDef(id=0x0000, type=FanMode, access="")
+        fan_mode_sequence: Final = ZCLAttributeDef(
+            id=0x0001, type=FanModeSequence, access=""
+        )
+
+
+class RelativeHumidityMode(t.enum8):
+    RH_measured_locally = 0x00
+    RH_measured_remotely = 0x01
+
+
+class DehumidificationLockout(t.enum8):
+    Dehumidification_not_allowed = 0x00
+    Dehumidification_is_allowed = 0x01
+
+
+class RelativeHumidityDisplay(t.enum8):
+    RH_not_displayed = 0x00
+    RH_is_displayed = 0x01
 
 
 class Dehumidification(Cluster):
     """An interface for controlling dehumidification."""
 
-    class RelativeHumidityMode(t.enum8):
-        RH_measured_locally = 0x00
-        RH_measured_remotely = 0x01
-
-    class DehumidificationLockout(t.enum8):
-        Dehumidification_not_allowed = 0x00
-        Dehumidification_is_allowed = 0x01
-
-    class RelativeHumidityDisplay(t.enum8):
-        RH_not_displayed = 0x00
-        RH_is_displayed = 0x01
-
-    cluster_id = 0x0203
-    ep_attribute = "dehumidification"
-    attributes: dict[int, ZCLAttributeDef] = {
+    RelativeHumidityMode: Final = RelativeHumidityMode
+    DehumidificationLockout: Final = DehumidificationLockout
+    RelativeHumidityDisplay: Final = RelativeHumidityDisplay
+
+    cluster_id: Final = 0x0203
+    ep_attribute: Final = "dehumidification"
+
+    class AttributeDefs(BaseAttributeDefs):
         # Dehumidification Information
-        0x0000: ZCLAttributeDef("relative_humidity", type=t.uint8_t, access="r"),
-        0x0001: ZCLAttributeDef(
-            "dehumidification_cooling", type=t.uint8_t, access="rp", mandatory=True
-        ),
+        relative_humidity: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint8_t, access="r"
+        )
+        dehumidification_cooling: Final = ZCLAttributeDef(
+            id=0x0001, type=t.uint8_t, access="rp", mandatory=True
+        )
         # Dehumidification Settings
-        0x0010: ZCLAttributeDef(
-            "rh_dehumidification_setpoint", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0011: ZCLAttributeDef(
-            "relative_humidity_mode", type=RelativeHumidityMode, access="rw"
-        ),
-        0x0012: ZCLAttributeDef(
-            "dehumidification_lockout", type=DehumidificationLockout, access="rw"
-        ),
-        0x0013: ZCLAttributeDef(
-            "dehumidification_hysteresis", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0014: ZCLAttributeDef(
-            "dehumidification_max_cool", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0015: ZCLAttributeDef(
-            "relative_humidity_display", type=RelativeHumidityDisplay, access="rw"
-        ),
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        rh_dehumidification_setpoint: Final = ZCLAttributeDef(
+            id=0x0010, type=t.uint8_t, access="rw", mandatory=True
+        )
+        relative_humidity_mode: Final = ZCLAttributeDef(
+            id=0x0011, type=RelativeHumidityMode, access="rw"
+        )
+        dehumidification_lockout: Final = ZCLAttributeDef(
+            id=0x0012, type=DehumidificationLockout, access="rw"
+        )
+        dehumidification_hysteresis: Final = ZCLAttributeDef(
+            id=0x0013, type=t.uint8_t, access="rw", mandatory=True
+        )
+        dehumidification_max_cool: Final = ZCLAttributeDef(
+            id=0x0014, type=t.uint8_t, access="rw", mandatory=True
+        )
+        relative_humidity_display: Final = ZCLAttributeDef(
+            id=0x0015, type=RelativeHumidityDisplay, access="rw"
+        )
+
+
+class TemperatureDisplayMode(t.enum8):
+    Metric = 0x00
+    Imperial = 0x01
+
+
+class KeypadLockout(t.enum8):
+    No_lockout = 0x00
+    Level_1_lockout = 0x01
+    Level_2_lockout = 0x02
+    Level_3_lockout = 0x03
+    Level_4_lockout = 0x04
+    Level_5_lockout = 0x05
+
+
+class ScheduleProgrammingVisibility(t.enum8):
+    Enabled = 0x00
+    Disabled = 0x02
 
 
 class UserInterface(Cluster):
     """An interface for configuring the user interface of a
     thermostat (which may be remote from the
     thermostat).
     """
 
-    class TemperatureDisplayMode(t.enum8):
-        Metric = 0x00
-        Imperial = 0x01
-
-    class KeypadLockout(t.enum8):
-        No_lockout = 0x00
-        Level_1_lockout = 0x01
-        Level_2_lockout = 0x02
-        Level_3_lockout = 0x03
-        Level_4_lockout = 0x04
-        Level_5_lockout = 0x05
-
-    class ScheduleProgrammingVisibility(t.enum8):
-        Enabled = 0x00
-        Disabled = 0x02
-
-    cluster_id = 0x0204
-    name = "Thermostat User Interface Configuration"
-    ep_attribute = "thermostat_ui"
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef(
-            "temperature_display_mode",
+    TemperatureDisplayMode: Final = TemperatureDisplayMode
+    KeypadLockout: Final = KeypadLockout
+    ScheduleProgrammingVisibility: Final = ScheduleProgrammingVisibility
+
+    cluster_id: Final = 0x0204
+    name: Final = "Thermostat User Interface Configuration"
+    ep_attribute: Final = "thermostat_ui"
+
+    class AttributeDefs(BaseAttributeDefs):
+        temperature_display_mode: Final = ZCLAttributeDef(
+            id=0x0000,
             type=TemperatureDisplayMode,
             access="rw",
             mandatory=True,
-        ),
-        0x0001: ZCLAttributeDef(
-            "keypad_lockout", type=KeypadLockout, access="rw", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef(
-            "schedule_programming_visibility",
+        )
+        keypad_lockout: Final = ZCLAttributeDef(
+            id=0x0001, type=KeypadLockout, access="rw", mandatory=True
+        )
+        schedule_programming_visibility: Final = ZCLAttributeDef(
+            id=0x0002,
             type=ScheduleProgrammingVisibility,
             access="rw",
-        ),
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        )
```

### Comparing `zigpy-0.55.0/zigpy/zcl/clusters/lighting.py` & `zigpy-0.56.0/zigpy/zcl/clusters/lighting.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,420 +1,498 @@
 """Lighting Functional Domain"""
 
 from __future__ import annotations
 
+from typing import Final
+
 import zigpy.types as t
 from zigpy.zcl import Cluster, foundation
-from zigpy.zcl.foundation import ZCLAttributeDef, ZCLCommandDef
+from zigpy.zcl.foundation import (
+    BaseAttributeDefs,
+    BaseCommandDefs,
+    ZCLAttributeDef,
+    ZCLCommandDef,
+)
+
+
+class ColorMode(t.enum8):
+    Hue_and_saturation = 0x00
+    X_and_Y = 0x01
+    Color_temperature = 0x02
+
+
+class EnhancedColorMode(t.enum8):
+    Hue_and_saturation = 0x00
+    X_and_Y = 0x01
+    Color_temperature = 0x02
+    Enhanced_hue_and_saturation = 0x03
+
+
+class ColorCapabilities(t.bitmap16):
+    Hue_and_saturation = 0b00000000_00000001
+    Enhanced_hue = 0b00000000_00000010
+    Color_loop = 0b00000000_00000100
+    XY_attributes = 0b00000000_00001000
+    Color_temperature = 0b00000000_00010000
+
+
+class Direction(t.enum8):
+    Shortest_distance = 0x00
+    Longest_distance = 0x01
+    Up = 0x02
+    Down = 0x03
+
+
+class MoveMode(t.enum8):
+    Stop = 0x00
+    Up = 0x01
+    Down = 0x03
+
+
+class StepMode(t.enum8):
+    Up = 0x01
+    Down = 0x03
+
+
+class ColorLoopUpdateFlags(t.bitmap8):
+    Action = 0b0000_0001
+    Direction = 0b0000_0010
+    Time = 0b0000_0100
+    Start_Hue = 0b0000_1000
+
+
+class ColorLoopAction(t.enum8):
+    Deactivate = 0x00
+    Activate_from_color_loop_hue = 0x01
+    Activate_from_current_hue = 0x02
+
+
+class ColorLoopDirection(t.enum8):
+    Decrement = 0x00
+    Increment = 0x01
+
+
+class DriftCompensation(t.enum8):
+    NONE = 0x00
+    Other_or_unknown = 0x01
+    Temperature_monitoring = 0x02
+    Luminance_monitoring = 0x03
+    Color_monitoring = 0x03
+
+
+class Options(t.bitmap8):
+    Execute_if_off = 0b00000001
 
 
 class Color(Cluster):
     """Attributes and commands for controlling the color
     properties of a color-capable light
     """
 
-    class ColorMode(t.enum8):
-        Hue_and_saturation = 0x00
-        X_and_Y = 0x01
-        Color_temperature = 0x02
-
-    class EnhancedColorMode(t.enum8):
-        Hue_and_saturation = 0x00
-        X_and_Y = 0x01
-        Color_temperature = 0x02
-        Enhanced_hue_and_saturation = 0x03
-
-    class ColorCapabilities(t.bitmap16):
-        Hue_and_saturation = 0b00000000_00000001
-        Enhanced_hue = 0b00000000_00000010
-        Color_loop = 0b00000000_00000100
-        XY_attributes = 0b00000000_00001000
-        Color_temperature = 0b00000000_00010000
-
-    class Direction(t.enum8):
-        Shortest_distance = 0x00
-        Longest_distance = 0x01
-        Up = 0x02
-        Down = 0x03
-
-    class MoveMode(t.enum8):
-        Stop = 0x00
-        Up = 0x01
-        Down = 0x03
-
-    class StepMode(t.enum8):
-        Up = 0x01
-        Down = 0x03
-
-    class ColorLoopUpdateFlags(t.bitmap8):
-        Action = 0b0000_0001
-        Direction = 0b0000_0010
-        Time = 0b0000_0100
-        Start_Hue = 0b0000_1000
-
-    class ColorLoopAction(t.enum8):
-        Deactivate = 0x00
-        Activate_from_color_loop_hue = 0x01
-        Activate_from_current_hue = 0x02
-
-    class ColorLoopDirection(t.enum8):
-        Decrement = 0x00
-        Increment = 0x01
-
-    class DriftCompensation(t.enum8):
-        NONE = 0x00
-        Other_or_unknown = 0x01
-        Temperature_monitoring = 0x02
-        Luminance_monitoring = 0x03
-        Color_monitoring = 0x03
-
-    class Options(t.bitmap8):
-        Execute_if_off = 0b00000001
-
-    cluster_id = 0x0300
-    name = "Color Control"
-    ep_attribute = "light_color"
-    attributes: dict[int, ZCLAttributeDef] = {
-        # Color Information
-        0x0000: ZCLAttributeDef("current_hue", type=t.uint8_t, access="rp"),
-        0x0001: ZCLAttributeDef("current_saturation", type=t.uint8_t, access="rps"),
-        0x0002: ZCLAttributeDef("remaining_time", type=t.uint16_t, access="r"),
-        0x0003: ZCLAttributeDef("current_x", type=t.uint16_t, access="rps"),
-        0x0004: ZCLAttributeDef("current_y", type=t.uint16_t, access="rps"),
-        0x0005: ZCLAttributeDef(
-            "drift_compensation", type=DriftCompensation, access="r"
-        ),
-        0x0006: ZCLAttributeDef(
-            "compensation_text", type=t.CharacterString, access="r"
-        ),
-        0x0007: ZCLAttributeDef("color_temperature", type=t.uint16_t, access="rps"),
-        0x0008: ZCLAttributeDef(
-            "color_mode", type=ColorMode, access="r", mandatory=True
-        ),
-        0x000F: ZCLAttributeDef("options", type=Options, access="rw", mandatory=True),
+    ColorMode: Final = ColorMode
+    EnhancedColorMode: Final = EnhancedColorMode
+    ColorCapabilities: Final = ColorCapabilities
+    Direction: Final = Direction
+    MoveMode: Final = MoveMode
+    StepMode: Final = StepMode
+    ColorLoopUpdateFlags: Final = ColorLoopUpdateFlags
+    ColorLoopAction: Final = ColorLoopAction
+    ColorLoopDirection: Final = ColorLoopDirection
+    DriftCompensation: Final = DriftCompensation
+    Options: Final = Options
+
+    cluster_id: Final = 0x0300
+    name: Final = "Color Control"
+    ep_attribute: Final = "light_color"
+
+    class AttributeDefs(BaseAttributeDefs):
+        current_hue: Final = ZCLAttributeDef(id=0x0000, type=t.uint8_t, access="rp")
+        current_saturation: Final = ZCLAttributeDef(
+            id=0x0001, type=t.uint8_t, access="rps"
+        )
+        remaining_time: Final = ZCLAttributeDef(id=0x0002, type=t.uint16_t, access="r")
+        current_x: Final = ZCLAttributeDef(id=0x0003, type=t.uint16_t, access="rps")
+        current_y: Final = ZCLAttributeDef(id=0x0004, type=t.uint16_t, access="rps")
+        drift_compensation: Final = ZCLAttributeDef(
+            id=0x0005, type=DriftCompensation, access="r"
+        )
+        compensation_text: Final = ZCLAttributeDef(
+            id=0x0006, type=t.CharacterString, access="r"
+        )
+        color_temperature: Final = ZCLAttributeDef(
+            id=0x0007, type=t.uint16_t, access="rps"
+        )
+        color_mode: Final = ZCLAttributeDef(
+            id=0x0008, type=ColorMode, access="r", mandatory=True
+        )
+        options: Final = ZCLAttributeDef(
+            id=0x000F, type=Options, access="rw", mandatory=True
+        )
         # Defined Primaries Information
-        0x0010: ZCLAttributeDef("num_primaries", type=t.uint8_t, access="r"),
-        0x0011: ZCLAttributeDef("primary1_x", type=t.uint16_t, access="r"),
-        0x0012: ZCLAttributeDef("primary1_y", type=t.uint16_t, access="r"),
-        0x0013: ZCLAttributeDef("primary1_intensity", type=t.uint8_t, access="r"),
-        0x0015: ZCLAttributeDef("primary2_x", type=t.uint16_t, access="r"),
-        0x0016: ZCLAttributeDef("primary2_y", type=t.uint16_t, access="r"),
-        0x0017: ZCLAttributeDef("primary2_intensity", type=t.uint8_t, access="r"),
-        0x0019: ZCLAttributeDef("primary3_x", type=t.uint16_t, access="r"),
-        0x001A: ZCLAttributeDef("primary3_y", type=t.uint16_t, access="r"),
-        0x001B: ZCLAttributeDef("primary3_intensity", type=t.uint8_t, access="r"),
+        num_primaries: Final = ZCLAttributeDef(id=0x0010, type=t.uint8_t, access="r")
+        primary1_x: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t, access="r")
+        primary1_y: Final = ZCLAttributeDef(id=0x0012, type=t.uint16_t, access="r")
+        primary1_intensity: Final = ZCLAttributeDef(
+            id=0x0013, type=t.uint8_t, access="r"
+        )
+        primary2_x: Final = ZCLAttributeDef(id=0x0015, type=t.uint16_t, access="r")
+        primary2_y: Final = ZCLAttributeDef(id=0x0016, type=t.uint16_t, access="r")
+        primary2_intensity: Final = ZCLAttributeDef(
+            id=0x0017, type=t.uint8_t, access="r"
+        )
+        primary3_x: Final = ZCLAttributeDef(id=0x0019, type=t.uint16_t, access="r")
+        primary3_y: Final = ZCLAttributeDef(id=0x001A, type=t.uint16_t, access="r")
+        primary3_intensity: Final = ZCLAttributeDef(
+            id=0x001B, type=t.uint8_t, access="r"
+        )
         # Additional Defined Primaries Information
-        0x0020: ZCLAttributeDef("primary4_x", type=t.uint16_t, access="r"),
-        0x0021: ZCLAttributeDef("primary4_y", type=t.uint16_t, access="r"),
-        0x0022: ZCLAttributeDef("primary4_intensity", type=t.uint8_t, access="r"),
-        0x0024: ZCLAttributeDef("primary5_x", type=t.uint16_t, access="r"),
-        0x0025: ZCLAttributeDef("primary5_y", type=t.uint16_t, access="r"),
-        0x0026: ZCLAttributeDef("primary5_intensity", type=t.uint8_t, access="r"),
-        0x0028: ZCLAttributeDef("primary6_x", type=t.uint16_t, access="r"),
-        0x0029: ZCLAttributeDef("primary6_y", type=t.uint16_t, access="r"),
-        0x002A: ZCLAttributeDef("primary6_intensity", type=t.uint8_t, access="r"),
+        primary4_x: Final = ZCLAttributeDef(id=0x0020, type=t.uint16_t, access="r")
+        primary4_y: Final = ZCLAttributeDef(id=0x0021, type=t.uint16_t, access="r")
+        primary4_intensity: Final = ZCLAttributeDef(
+            id=0x0022, type=t.uint8_t, access="r"
+        )
+        primary5_x: Final = ZCLAttributeDef(id=0x0024, type=t.uint16_t, access="r")
+        primary5_y: Final = ZCLAttributeDef(id=0x0025, type=t.uint16_t, access="r")
+        primary5_intensity: Final = ZCLAttributeDef(
+            id=0x0026, type=t.uint8_t, access="r"
+        )
+        primary6_x: Final = ZCLAttributeDef(id=0x0028, type=t.uint16_t, access="r")
+        primary6_y: Final = ZCLAttributeDef(id=0x0029, type=t.uint16_t, access="r")
+        primary6_intensity: Final = ZCLAttributeDef(
+            id=0x002A, type=t.uint8_t, access="r"
+        )
         # Defined Color Point Settings
-        0x0030: ZCLAttributeDef("white_point_x", type=t.uint16_t, access="r"),
-        0x0031: ZCLAttributeDef("white_point_y", type=t.uint16_t, access="r"),
-        0x0032: ZCLAttributeDef("color_point_r_x", type=t.uint16_t, access="r"),
-        0x0033: ZCLAttributeDef("color_point_r_y", type=t.uint16_t, access="r"),
-        0x0034: ZCLAttributeDef("color_point_r_intensity", type=t.uint8_t, access="r"),
-        0x0036: ZCLAttributeDef("color_point_g_x", type=t.uint16_t, access="r"),
-        0x0037: ZCLAttributeDef("color_point_g_y", type=t.uint16_t, access="r"),
-        0x0038: ZCLAttributeDef("color_point_g_intensity", type=t.uint8_t, access="r"),
-        0x003A: ZCLAttributeDef("color_point_b_x", type=t.uint16_t, access="r"),
-        0x003B: ZCLAttributeDef("color_point_b_y", type=t.uint16_t, access="r"),
-        0x003C: ZCLAttributeDef("color_point_b_intensity", type=t.uint8_t, access="r"),
+        white_point_x: Final = ZCLAttributeDef(id=0x0030, type=t.uint16_t, access="r")
+        white_point_y: Final = ZCLAttributeDef(id=0x0031, type=t.uint16_t, access="r")
+        color_point_r_x: Final = ZCLAttributeDef(id=0x0032, type=t.uint16_t, access="r")
+        color_point_r_y: Final = ZCLAttributeDef(id=0x0033, type=t.uint16_t, access="r")
+        color_point_r_intensity: Final = ZCLAttributeDef(
+            id=0x0034, type=t.uint8_t, access="r"
+        )
+        color_point_g_x: Final = ZCLAttributeDef(id=0x0036, type=t.uint16_t, access="r")
+        color_point_g_y: Final = ZCLAttributeDef(id=0x0037, type=t.uint16_t, access="r")
+        color_point_g_intensity: Final = ZCLAttributeDef(
+            id=0x0038, type=t.uint8_t, access="r"
+        )
+        color_point_b_x: Final = ZCLAttributeDef(id=0x003A, type=t.uint16_t, access="r")
+        color_point_b_y: Final = ZCLAttributeDef(id=0x003B, type=t.uint16_t, access="r")
+        color_point_b_intensity: Final = ZCLAttributeDef(
+            id=0x003C, type=t.uint8_t, access="r"
+        )
         # ...
-        0x4000: ZCLAttributeDef("enhanced_current_hue", type=t.uint16_t, access="rs"),
-        0x4001: ZCLAttributeDef(
-            "enhanced_color_mode", type=EnhancedColorMode, access="r", mandatory=True
-        ),
-        0x4002: ZCLAttributeDef("color_loop_active", type=t.uint8_t, access="rs"),
-        0x4003: ZCLAttributeDef("color_loop_direction", type=t.uint8_t, access="rs"),
-        0x4004: ZCLAttributeDef("color_loop_time", type=t.uint16_t, access="rs"),
-        0x4005: ZCLAttributeDef(
-            "color_loop_start_enhanced_hue", type=t.uint16_t, access="r"
-        ),
-        0x4006: ZCLAttributeDef(
-            "color_loop_stored_enhanced_hue", type=t.uint16_t, access="r"
-        ),
-        0x400A: ZCLAttributeDef(
-            "color_capabilities", type=ColorCapabilities, access="r", mandatory=True
-        ),
-        0x400B: ZCLAttributeDef("color_temp_physical_min", type=t.uint16_t, access="r"),
-        0x400C: ZCLAttributeDef("color_temp_physical_max", type=t.uint16_t, access="r"),
-        0x400D: ZCLAttributeDef(
-            "couple_color_temp_to_level_min", type=t.uint16_t, access="r"
-        ),
-        0x4010: ZCLAttributeDef(
-            "start_up_color_temperature", type=t.uint16_t, access="rw"
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef(
-            "move_to_hue",
-            {
+        enhanced_current_hue: Final = ZCLAttributeDef(
+            id=0x4000, type=t.uint16_t, access="rs"
+        )
+        enhanced_color_mode: Final = ZCLAttributeDef(
+            id=0x4001, type=EnhancedColorMode, access="r", mandatory=True
+        )
+        color_loop_active: Final = ZCLAttributeDef(
+            id=0x4002, type=t.uint8_t, access="rs"
+        )
+        color_loop_direction: Final = ZCLAttributeDef(
+            id=0x4003, type=t.uint8_t, access="rs"
+        )
+        color_loop_time: Final = ZCLAttributeDef(
+            id=0x4004, type=t.uint16_t, access="rs"
+        )
+        color_loop_start_enhanced_hue: Final = ZCLAttributeDef(
+            id=0x4005, type=t.uint16_t, access="r"
+        )
+        color_loop_stored_enhanced_hue: Final = ZCLAttributeDef(
+            id=0x4006, type=t.uint16_t, access="r"
+        )
+        color_capabilities: Final = ZCLAttributeDef(
+            id=0x400A, type=ColorCapabilities, access="r", mandatory=True
+        )
+        color_temp_physical_min: Final = ZCLAttributeDef(
+            id=0x400B, type=t.uint16_t, access="r"
+        )
+        color_temp_physical_max: Final = ZCLAttributeDef(
+            id=0x400C, type=t.uint16_t, access="r"
+        )
+        couple_color_temp_to_level_min: Final = ZCLAttributeDef(
+            id=0x400D, type=t.uint16_t, access="r"
+        )
+        start_up_color_temperature: Final = ZCLAttributeDef(
+            id=0x4010, type=t.uint16_t, access="rw"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
+
+    class ServerCommandDefs(BaseCommandDefs):
+        move_to_hue: Final = ZCLCommandDef(
+            id=0x00,
+            schema={
                 "hue": t.uint8_t,
                 "direction": Direction,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x01: ZCLCommandDef(
-            "move_hue",
-            {
+            direction=False,
+        )
+        move_hue: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "move_mode": MoveMode,
                 "rate": t.uint8_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x02: ZCLCommandDef(
-            "step_hue",
-            {
+            direction=False,
+        )
+        step_hue: Final = ZCLCommandDef(
+            id=0x02,
+            schema={
                 "step_mode": StepMode,
                 "step_size": t.uint8_t,
                 "transition_time": t.uint8_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x03: ZCLCommandDef(
-            "move_to_saturation",
-            {
+            direction=False,
+        )
+        move_to_saturation: Final = ZCLCommandDef(
+            id=0x03,
+            schema={
                 "saturation": t.uint8_t,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x04: ZCLCommandDef(
-            "move_saturation",
-            {
+            direction=False,
+        )
+        move_saturation: Final = ZCLCommandDef(
+            id=0x04,
+            schema={
                 "move_mode": MoveMode,
                 "rate": t.uint8_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x05: ZCLCommandDef(
-            "step_saturation",
-            {
+            direction=False,
+        )
+        step_saturation: Final = ZCLCommandDef(
+            id=0x05,
+            schema={
                 "step_mode": StepMode,
                 "step_size": t.uint8_t,
                 "transition_time": t.uint8_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x06: ZCLCommandDef(
-            "move_to_hue_and_saturation",
-            {
+            direction=False,
+        )
+        move_to_hue_and_saturation: Final = ZCLCommandDef(
+            id=0x06,
+            schema={
                 "hue": t.uint8_t,
                 "saturation": t.uint8_t,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x07: ZCLCommandDef(
-            "move_to_color",
-            {
+            direction=False,
+        )
+        move_to_color: Final = ZCLCommandDef(
+            id=0x07,
+            schema={
                 "color_x": t.uint16_t,
                 "color_y": t.uint16_t,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x08: ZCLCommandDef(
-            "move_color",
-            {
+            direction=False,
+        )
+        move_color: Final = ZCLCommandDef(
+            id=0x08,
+            schema={
                 "rate_x": t.uint16_t,
                 "rate_y": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x09: ZCLCommandDef(
-            "step_color",
-            {
+            direction=False,
+        )
+        step_color: Final = ZCLCommandDef(
+            id=0x09,
+            schema={
                 "step_x": t.uint16_t,
                 "step_y": t.uint16_t,
                 "duration": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x0A: ZCLCommandDef(
-            "move_to_color_temp",
-            {
+            direction=False,
+        )
+        move_to_color_temp: Final = ZCLCommandDef(
+            id=0x0A,
+            schema={
                 "color_temp_mireds": t.uint16_t,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x40: ZCLCommandDef(
-            "enhanced_move_to_hue",
-            {
+            direction=False,
+        )
+        enhanced_move_to_hue: Final = ZCLCommandDef(
+            id=0x40,
+            schema={
                 "enhanced_hue": t.uint16_t,
                 "direction": Direction,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x41: ZCLCommandDef(
-            "enhanced_move_hue",
-            {
+            direction=False,
+        )
+        enhanced_move_hue: Final = ZCLCommandDef(
+            id=0x41,
+            schema={
                 "move_mode": MoveMode,
                 "rate": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x42: ZCLCommandDef(
-            "enhanced_step_hue",
-            {
+            direction=False,
+        )
+        enhanced_step_hue: Final = ZCLCommandDef(
+            id=0x42,
+            schema={
                 "step_mode": StepMode,
                 "step_size": t.uint16_t,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x43: ZCLCommandDef(
-            "enhanced_move_to_hue_and_saturation",
-            {
+            direction=False,
+        )
+        enhanced_move_to_hue_and_saturation: Final = ZCLCommandDef(
+            id=0x43,
+            schema={
                 "enhanced_hue": t.uint16_t,
                 "saturation": t.uint8_t,
                 "transition_time": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x44: ZCLCommandDef(
-            "color_loop_set",
-            {
+            direction=False,
+        )
+        color_loop_set: Final = ZCLCommandDef(
+            id=0x44,
+            schema={
                 "update_flags": ColorLoopUpdateFlags,
                 "action": ColorLoopAction,
                 "direction": ColorLoopDirection,
                 "time": t.uint16_t,
                 "start_hue": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x47: ZCLCommandDef(
-            "stop_move_step",
-            {
+            direction=False,
+        )
+        stop_move_step: Final = ZCLCommandDef(
+            id=0x47,
+            schema={
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x4B: ZCLCommandDef(
-            "move_color_temp",
-            {
+            direction=False,
+        )
+        move_color_temp: Final = ZCLCommandDef(
+            id=0x4B,
+            schema={
                 "move_mode": MoveMode,
                 "rate": t.uint16_t,
                 "color_temp_min_mireds": t.uint16_t,
                 "color_temp_max_mireds": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-        0x4C: ZCLCommandDef(
-            "step_color_temp",
-            {
+            direction=False,
+        )
+        step_color_temp: Final = ZCLCommandDef(
+            id=0x4C,
+            schema={
                 "step_mode": StepMode,
                 "step_size": t.uint16_t,
                 "transition_time": t.uint16_t,
                 "color_temp_min_mireds": t.uint16_t,
                 "color_temp_max_mireds": t.uint16_t,
                 "options_mask?": t.bitmap8,
                 "options_override?": t.bitmap8,
             },
-            False,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {}
+            direction=False,
+        )
+
+
+class BallastStatus(t.bitmap8):
+    Non_operational = 0b00000001
+    Lamp_failure = 0b00000010
+
+
+class LampAlarmMode(t.bitmap8):
+    Lamp_burn_hours = 0b00000001
 
 
 class Ballast(Cluster):
     """Attributes and commands for configuring a lighting
     ballast
     """
 
-    class BallastStatus(t.bitmap8):
-        Non_operational = 0b00000001
-        Lamp_failure = 0b00000010
-
-    class LampAlarmMode(t.bitmap8):
-        Lamp_burn_hours = 0b00000001
-
-    cluster_id = 0x0301
-    ep_attribute = "light_ballast"
-    attributes: dict[int, ZCLAttributeDef] = {
-        # Ballast Information
-        0x0000: ZCLAttributeDef(
-            "physical_min_level", type=t.uint8_t, access="r", mandatory=True
-        ),
-        0x0001: ZCLAttributeDef(
-            "physical_max_level", type=t.uint8_t, access="r", mandatory=True
-        ),
-        0x0002: ZCLAttributeDef("ballast_status", type=BallastStatus, access="r"),
+    BallastStatus: Final = BallastStatus
+    LampAlarmMode: Final = LampAlarmMode
+
+    cluster_id: Final = 0x0301
+    ep_attribute: Final = "light_ballast"
+
+    class AttributeDefs(BaseAttributeDefs):
+        physical_min_level: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint8_t, access="r", mandatory=True
+        )
+        physical_max_level: Final = ZCLAttributeDef(
+            id=0x0001, type=t.uint8_t, access="r", mandatory=True
+        )
+        ballast_status: Final = ZCLAttributeDef(
+            id=0x0002, type=BallastStatus, access="r"
+        )
         # Ballast Settings
-        0x0010: ZCLAttributeDef(
-            "min_level", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0011: ZCLAttributeDef(
-            "max_level", type=t.uint8_t, access="rw", mandatory=True
-        ),
-        0x0012: ZCLAttributeDef("power_on_level", type=t.uint8_t, access="rw"),
-        0x0013: ZCLAttributeDef("power_on_fade_time", type=t.uint16_t, access="rw"),
-        0x0014: ZCLAttributeDef(
-            "intrinsic_ballast_factor", type=t.uint8_t, access="rw"
-        ),
-        0x0015: ZCLAttributeDef(
-            "ballast_factor_adjustment", type=t.uint8_t, access="rw"
-        ),
+        min_level: Final = ZCLAttributeDef(
+            id=0x0010, type=t.uint8_t, access="rw", mandatory=True
+        )
+        max_level: Final = ZCLAttributeDef(
+            id=0x0011, type=t.uint8_t, access="rw", mandatory=True
+        )
+        power_on_level: Final = ZCLAttributeDef(id=0x0012, type=t.uint8_t, access="rw")
+        power_on_fade_time: Final = ZCLAttributeDef(
+            id=0x0013, type=t.uint16_t, access="rw"
+        )
+        intrinsic_ballast_factor: Final = ZCLAttributeDef(
+            id=0x0014, type=t.uint8_t, access="rw"
+        )
+        ballast_factor_adjustment: Final = ZCLAttributeDef(
+            id=0x0015, type=t.uint8_t, access="rw"
+        )
         # Lamp Information
-        0x0020: ZCLAttributeDef("lamp_quantity", type=t.uint8_t, access="r"),
+        lamp_quantity: Final = ZCLAttributeDef(id=0x0020, type=t.uint8_t, access="r")
         # Lamp Settings
-        0x0030: ZCLAttributeDef("lamp_type", type=t.LimitedCharString(16), access="rw"),
-        0x0031: ZCLAttributeDef(
-            "lamp_manufacturer", type=t.LimitedCharString(16), access="rw"
-        ),
-        0x0032: ZCLAttributeDef("lamp_rated_hours", type=t.uint24_t, access="rw"),
-        0x0033: ZCLAttributeDef("lamp_burn_hours", type=t.uint24_t, access="rw"),
-        0x0034: ZCLAttributeDef("lamp_alarm_mode", type=LampAlarmMode, access="rw"),
-        0x0035: ZCLAttributeDef(
-            "lamp_burn_hours_trip_point", type=t.uint24_t, access="rw"
-        ),
-        0xFFFD: foundation.ZCL_CLUSTER_REVISION_ATTR,
-        0xFFFE: foundation.ZCL_REPORTING_STATUS_ATTR,
-    }
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+        lamp_type: Final = ZCLAttributeDef(
+            id=0x0030, type=t.LimitedCharString(16), access="rw"
+        )
+        lamp_manufacturer: Final = ZCLAttributeDef(
+            id=0x0031, type=t.LimitedCharString(16), access="rw"
+        )
+        lamp_rated_hours: Final = ZCLAttributeDef(
+            id=0x0032, type=t.uint24_t, access="rw"
+        )
+        lamp_burn_hours: Final = ZCLAttributeDef(
+            id=0x0033, type=t.uint24_t, access="rw"
+        )
+        lamp_alarm_mode: Final = ZCLAttributeDef(
+            id=0x0034, type=LampAlarmMode, access="rw"
+        )
+        lamp_burn_hours_trip_point: Final = ZCLAttributeDef(
+            id=0x0035, type=t.uint24_t, access="rw"
+        )
+        cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
+        reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
```

### Comparing `zigpy-0.55.0/zigpy/zcl/clusters/lightlink.py` & `zigpy-0.56.0/zigpy/zcl/clusters/lightlink.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
+from typing import Final
+
 import zigpy.types as t
 from zigpy.zcl import Cluster
-from zigpy.zcl.foundation import ZCLAttributeDef, ZCLCommandDef
+from zigpy.zcl.foundation import BaseCommandDefs, ZCLCommandDef
 
 
 class LogicalType(t.enum2):
     Coordinator = 0b00
     Router = 0b01
     EndDevice = 0b10
 
@@ -72,46 +74,48 @@
     endpoint_id: t.uint8_t
     profile_id: t.uint16_t
     device_id: t.uint16_t
     version: t.uint8_t
 
 
 class LightLink(Cluster):
-    cluster_id = 0x1000
-    ep_attribute = "lightlink"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {
-        # Touchlink
-        0x00: ZCLCommandDef(
-            "scan",
-            {
+    cluster_id: Final = 0x1000
+    ep_attribute: Final = "lightlink"
+
+    class ServerCommandDefs(BaseCommandDefs):
+        scan: Final = ZCLCommandDef(
+            id=0x00,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "zigbee_information": ZigbeeInformation,
                 "touchlink_information": ScanRequestInformation,
             },
-            False,
-        ),
-        0x02: ZCLCommandDef(
-            "device_info",
-            {"inter_pan_transaction_id": t.uint32_t, "start_index": t.uint8_t},
-            False,
-        ),
-        0x06: ZCLCommandDef(
-            "identify",
-            {"inter_pan_transaction_id": t.uint32_t, "identify_duration": t.uint16_t},
-            False,
-        ),
-        0x07: ZCLCommandDef(
-            "reset_to_factory_new",
-            {"inter_pan_transaction_id": t.uint32_t},
-            False,
-        ),
-        0x10: ZCLCommandDef(
-            "network_start",
-            {
+            direction=False,
+        )
+        device_info: Final = ZCLCommandDef(
+            id=0x02,
+            schema={"inter_pan_transaction_id": t.uint32_t, "start_index": t.uint8_t},
+            direction=False,
+        )
+        identify: Final = ZCLCommandDef(
+            id=0x06,
+            schema={
+                "inter_pan_transaction_id": t.uint32_t,
+                "identify_duration": t.uint16_t,
+            },
+            direction=False,
+        )
+        reset_to_factory_new: Final = ZCLCommandDef(
+            id=0x07,
+            schema={"inter_pan_transaction_id": t.uint32_t},
+            direction=False,
+        )
+        network_start: Final = ZCLCommandDef(
+            id=0x10,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "epid": t.EUI64,
                 "key_index": t.uint8_t,
                 "encrypted_network_key": t.KeyData,
                 "logical_channel": t.uint8_t,
                 "pan_id": t.PanId,
                 "nwk_addr": t.NWK,
@@ -120,19 +124,19 @@
                 "free_network_addr_range_begin": t.NWK,
                 "free_network_addr_range_end": t.NWK,
                 "free_group_id_range_begin": t.Group,
                 "free_group_id_range_end": t.Group,
                 "initiator_ieee": t.EUI64,
                 "initiator_nwk": t.NWK,
             },
-            False,
-        ),
-        0x12: ZCLCommandDef(
-            "network_join_router",
-            {
+            direction=False,
+        )
+        network_join_router: Final = ZCLCommandDef(
+            id=0x12,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "epid": t.EUI64,
                 "key_index": t.uint8_t,
                 "encrypted_network_key": t.KeyData,
                 "nwk_update_id": t.uint8_t,
                 "logical_channel": t.uint8_t,
                 "pan_id": t.PanId,
@@ -140,19 +144,19 @@
                 "group_identifiers_begin": t.Group,
                 "group_identifiers_end": t.Group,
                 "free_network_addr_range_begin": t.NWK,
                 "free_network_addr_range_end": t.NWK,
                 "free_group_id_range_begin": t.Group,
                 "free_group_id_range_end": t.Group,
             },
-            False,
-        ),
-        0x14: ZCLCommandDef(
-            "network_join_end_device",
-            {
+            direction=False,
+        )
+        network_join_end_device: Final = ZCLCommandDef(
+            id=0x14,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "epid": t.EUI64,
                 "key_index": t.uint8_t,
                 "encrypted_network_key": t.KeyData,
                 "nwk_update_id": t.uint8_t,
                 "logical_channel": t.uint8_t,
                 "pan_id": t.PanId,
@@ -160,49 +164,48 @@
                 "group_identifiers_begin": t.Group,
                 "group_identifiers_end": t.Group,
                 "free_network_addr_range_begin": t.NWK,
                 "free_network_addr_range_end": t.NWK,
                 "free_group_id_range_begin": t.Group,
                 "free_group_id_range_end": t.Group,
             },
-            False,
-        ),
-        0x16: ZCLCommandDef(
-            "network_update",
-            {
+            direction=False,
+        )
+        network_update: Final = ZCLCommandDef(
+            id=0x16,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "epid": t.EUI64,
                 "nwk_update_id": t.uint8_t,
                 "logical_channel": t.uint8_t,
                 "pan_id": t.PanId,
                 "nwk_addr": t.NWK,
             },
-            False,
-        ),
+            direction=False,
+        )
         # Utility
-        0x41: ZCLCommandDef(
-            "get_group_identifiers",
-            {
+        get_group_identifiers: Final = ZCLCommandDef(
+            id=0x41,
+            schema={
                 "start_index": t.uint8_t,
             },
-            False,
-        ),
-        0x42: ZCLCommandDef(
-            "get_endpoint_list",
-            {
+            direction=False,
+        )
+        get_endpoint_list: Final = ZCLCommandDef(
+            id=0x42,
+            schema={
                 "start_index": t.uint8_t,
             },
-            False,
-        ),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        # Touchlink
-        0x01: ZCLCommandDef(
-            "scan_rsp",
-            {
+            direction=False,
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        scan_rsp: Final = ZCLCommandDef(
+            id=0x01,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "rssi_correction": t.uint8_t,
                 "zigbee_info": ZigbeeInformation,
                 "touchlink_info": ScanResponseInformation,
                 "key_bitmask": t.uint16_t,
                 "response_id": t.uint32_t,
                 "epid": t.EUI64,
@@ -214,79 +217,78 @@
                 "total_group_ids": t.uint8_t,
                 "endpoint_id?": t.uint8_t,
                 "profile_id?": t.uint16_t,
                 "device_id?": t.uint16_t,
                 "version?": t.uint8_t,
                 "group_id_count?": t.uint8_t,
             },
-            True,
-        ),
-        0x03: ZCLCommandDef(
-            "device_info_rsp",
-            {
+            direction=True,
+        )
+        device_info_rsp: Final = ZCLCommandDef(
+            id=0x03,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "num_sub_devices": t.uint8_t,
                 "start_index": t.uint8_t,
                 "device_info_records": t.LVList[DeviceInfoRecord],
             },
-            True,
-        ),
-        0x11: ZCLCommandDef(
-            "network_start_rsp",
-            {
+            direction=True,
+        )
+        network_start_rsp: Final = ZCLCommandDef(
+            id=0x11,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "status": Status,
                 "epid": t.EUI64,
                 "nwk_update_id": t.uint8_t,
                 "logical_channel": t.uint8_t,
                 "pan_id": t.PanId,
             },
-            True,
-        ),
-        0x13: ZCLCommandDef(
-            "network_join_router_rsp",
-            {
+            direction=True,
+        )
+        network_join_router_rsp: Final = ZCLCommandDef(
+            id=0x13,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "status": Status,
             },
-            True,
-        ),
-        0x15: ZCLCommandDef(
-            "network_join_end_device_rsp",
-            {
+            direction=True,
+        )
+        network_join_end_device_rsp: Final = ZCLCommandDef(
+            id=0x15,
+            schema={
                 "inter_pan_transaction_id": t.uint32_t,
                 "status": Status,
             },
-            True,
-        ),
+            direction=True,
+        )
         # Utility
-        0x40: ZCLCommandDef(
-            "endpoint_info",
-            {
+        endpoint_info: Final = ZCLCommandDef(
+            id=0x40,
+            schema={
                 "ieee_addr": t.EUI64,
                 "nwk_addr": t.NWK,
                 "endpoint_id": t.uint8_t,
                 "profile_id": t.uint16_t,
                 "device_id": t.uint16_t,
                 "version": t.uint8_t,
             },
-            True,
-        ),
-        0x41: ZCLCommandDef(
-            "get_group_identifiers_rsp",
-            {
+            direction=True,
+        )
+        get_group_identifiers_rsp: Final = ZCLCommandDef(
+            id=0x41,
+            schema={
                 "total": t.uint8_t,
                 "start_index": t.uint8_t,
                 "group_info_records": t.LVList[GroupInfoRecord],
             },
-            True,
-        ),
-        0x42: ZCLCommandDef(
-            "get_endpoint_list_rsp",
-            {
+            direction=True,
+        )
+        get_endpoint_list_rsp: Final = ZCLCommandDef(
+            id=0x42,
+            schema={
                 "total": t.uint8_t,
                 "start_index": t.uint8_t,
                 "endpoint_info_records": t.LVList[EndpointInfoRecord],
             },
-            True,
-        ),
-    }
+            direction=True,
+        )
```

### Comparing `zigpy-0.55.0/zigpy/zcl/clusters/smartenergy.py` & `zigpy-0.56.0/zigpy/zcl/clusters/smartenergy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,440 +1,484 @@
 from __future__ import annotations
 
+from typing import Final
+
 import zigpy.types as t
 from zigpy.zcl import Cluster
-from zigpy.zcl.foundation import ZCLAttributeDef, ZCLCommandDef
+from zigpy.zcl.foundation import (
+    BaseAttributeDefs,
+    BaseCommandDefs,
+    ZCLAttributeDef,
+    ZCLCommandDef,
+)
 
 
 class Price(Cluster):
-    cluster_id = 0x0700
-    ep_attribute = "smartenergy_price"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0700
+    ep_attribute: Final = "smartenergy_price"
 
 
 class Drlc(Cluster):
-    cluster_id = 0x0701
-    ep_attribute = "smartenergy_drlc"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0701
+    ep_attribute: Final = "smartenergy_drlc"
+
+
+class RegisteredTier(t.enum8):
+    No_Tier = 0x00
+    Tier_1 = 0x01
+    Tier_2 = 0x02
+    Tier_3 = 0x03
+    Tier_4 = 0x04
+    Tier_5 = 0x05
+    Tier_6 = 0x06
+    Tier_7 = 0x07
+    Tier_8 = 0x08
+    Tier_9 = 0x09
+    Tier_10 = 0x0A
+    Tier_11 = 0x0B
+    Tier_12 = 0x0C
+    Tier_13 = 0x0D
+    Tier_14 = 0x0E
+    Extended_Tier = 0x0F
 
 
 class Metering(Cluster):
-    cluster_id = 0x0702
-    ep_attribute = "smartenergy_metering"
+    RegisteredTier: Final = RegisteredTier
+
+    cluster_id: Final = 0x0702
+    ep_attribute: Final = "smartenergy_metering"
 
-    class RegisteredTier(t.enum8):
-        No_Tier = 0x00
-        Tier_1 = 0x01
-        Tier_2 = 0x02
-        Tier_3 = 0x03
-        Tier_4 = 0x04
-        Tier_5 = 0x05
-        Tier_6 = 0x06
-        Tier_7 = 0x07
-        Tier_8 = 0x08
-        Tier_9 = 0x09
-        Tier_10 = 0x0A
-        Tier_11 = 0x0B
-        Tier_12 = 0x0C
-        Tier_13 = 0x0D
-        Tier_14 = 0x0E
-        Extended_Tier = 0x0F
-
-    attributes: dict[int, ZCLAttributeDef] = {
-        0x0000: ZCLAttributeDef("current_summ_delivered", type=t.uint48_t, access="r"),
-        0x0001: ZCLAttributeDef("current_summ_received", type=t.uint48_t, access="r"),
-        0x0002: ZCLAttributeDef(
-            "current_max_demand_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0003: ZCLAttributeDef(
-            "current_max_demand_received", type=t.uint48_t, access="r"
-        ),
-        0x0004: ZCLAttributeDef("dft_summ", type=t.uint48_t, access="r"),
-        0x0005: ZCLAttributeDef("daily_freeze_time", type=t.uint16_t, access="r"),
-        0x0006: ZCLAttributeDef("power_factor", type=t.int8s, access="r"),
-        0x0007: ZCLAttributeDef("reading_snapshot_time", type=t.UTCTime, access="r"),
-        0x0008: ZCLAttributeDef(
-            "current_max_demand_delivered_time", type=t.UTCTime, access="r"
-        ),
-        0x0009: ZCLAttributeDef(
-            "current_max_demand_received_time", type=t.UTCTime, access="r"
-        ),
-        0x000A: ZCLAttributeDef("default_update_period", type=t.uint8_t, access="r"),
-        0x000B: ZCLAttributeDef("fast_poll_update_period", type=t.uint8_t, access="r"),
-        0x000C: ZCLAttributeDef(
-            "current_block_period_consump_delivered", type=t.uint48_t, access="r"
-        ),
-        0x000D: ZCLAttributeDef("daily_consump_target", type=t.uint24_t, access="r"),
-        0x000E: ZCLAttributeDef("current_block", type=t.enum8, access="r"),
-        0x000F: ZCLAttributeDef("profile_interval_period", type=t.enum8, access="r"),
-        # 0x0010: ('interval_read_reporting_period', UNKNOWN),  # Deprecated
-        0x0011: ZCLAttributeDef("preset_reading_time", type=t.uint16_t, access="r"),
-        0x0012: ZCLAttributeDef("volume_per_report", type=t.uint16_t, access="r"),
-        0x0013: ZCLAttributeDef("flow_restriction", type=t.uint8_t, access="r"),
-        0x0014: ZCLAttributeDef("supply_status", type=t.enum8, access="r"),
-        0x0015: ZCLAttributeDef(
-            "current_in_energy_carrier_summ", type=t.uint48_t, access="r"
-        ),
-        0x0016: ZCLAttributeDef(
-            "current_out_energy_carrier_summ", type=t.uint48_t, access="r"
-        ),
-        0x0017: ZCLAttributeDef("inlet_temperature", type=t.int24s, access="r"),
-        0x0018: ZCLAttributeDef("outlet_temperature", type=t.int24s, access="r"),
-        0x0019: ZCLAttributeDef("control_temperature", type=t.int24s, access="r"),
-        0x001A: ZCLAttributeDef(
-            "current_in_energy_carrier_demand", type=t.int24s, access="r"
-        ),
-        0x001B: ZCLAttributeDef(
-            "current_out_energy_carrier_demand", type=t.int24s, access="r"
-        ),
-        0x001D: ZCLAttributeDef(
-            "current_block_period_consump_received", type=t.uint48_t, access="r"
-        ),
-        0x001E: ZCLAttributeDef("current_block_received", type=t.uint48_t, access="r"),
-        0x001F: ZCLAttributeDef("dft_summation_received", type=t.uint48_t, access="r"),
-        0x0020: ZCLAttributeDef(
-            "active_register_tier_delivered", type=RegisteredTier, access="r"
-        ),
-        0x0021: ZCLAttributeDef(
-            "active_register_tier_received", type=RegisteredTier, access="r"
-        ),
-        0x0022: ZCLAttributeDef("last_block_switch_time", type=t.UTCTime, access="r"),
+    class AttributeDefs(BaseAttributeDefs):
+        current_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0000, type=t.uint48_t, access="r"
+        )
+        current_summ_received: Final = ZCLAttributeDef(
+            id=0x0001, type=t.uint48_t, access="r"
+        )
+        current_max_demand_delivered: Final = ZCLAttributeDef(
+            id=0x0002, type=t.uint48_t, access="r"
+        )
+        current_max_demand_received: Final = ZCLAttributeDef(
+            id=0x0003, type=t.uint48_t, access="r"
+        )
+        dft_summ: Final = ZCLAttributeDef(id=0x0004, type=t.uint48_t, access="r")
+        daily_freeze_time: Final = ZCLAttributeDef(
+            id=0x0005, type=t.uint16_t, access="r"
+        )
+        power_factor: Final = ZCLAttributeDef(id=0x0006, type=t.int8s, access="r")
+        reading_snapshot_time: Final = ZCLAttributeDef(
+            id=0x0007, type=t.UTCTime, access="r"
+        )
+        current_max_demand_delivered_time: Final = ZCLAttributeDef(
+            id=0x0008, type=t.UTCTime, access="r"
+        )
+        current_max_demand_received_time: Final = ZCLAttributeDef(
+            id=0x0009, type=t.UTCTime, access="r"
+        )
+        default_update_period: Final = ZCLAttributeDef(
+            id=0x000A, type=t.uint8_t, access="r"
+        )
+        fast_poll_update_period: Final = ZCLAttributeDef(
+            id=0x000B, type=t.uint8_t, access="r"
+        )
+        current_block_period_consump_delivered: Final = ZCLAttributeDef(
+            id=0x000C, type=t.uint48_t, access="r"
+        )
+        daily_consump_target: Final = ZCLAttributeDef(
+            id=0x000D, type=t.uint24_t, access="r"
+        )
+        current_block: Final = ZCLAttributeDef(id=0x000E, type=t.enum8, access="r")
+        profile_interval_period: Final = ZCLAttributeDef(
+            id=0x000F, type=t.enum8, access="r"
+        )
+        # 0x0010: ('interval_read_reporting_period', UNKNOWN), # Deprecated
+        preset_reading_time: Final = ZCLAttributeDef(
+            id=0x0011, type=t.uint16_t, access="r"
+        )
+        volume_per_report: Final = ZCLAttributeDef(
+            id=0x0012, type=t.uint16_t, access="r"
+        )
+        flow_restriction: Final = ZCLAttributeDef(id=0x0013, type=t.uint8_t, access="r")
+        supply_status: Final = ZCLAttributeDef(id=0x0014, type=t.enum8, access="r")
+        current_in_energy_carrier_summ: Final = ZCLAttributeDef(
+            id=0x0015, type=t.uint48_t, access="r"
+        )
+        current_out_energy_carrier_summ: Final = ZCLAttributeDef(
+            id=0x0016, type=t.uint48_t, access="r"
+        )
+        inlet_temperature: Final = ZCLAttributeDef(id=0x0017, type=t.int24s, access="r")
+        outlet_temperature: Final = ZCLAttributeDef(
+            id=0x0018, type=t.int24s, access="r"
+        )
+        control_temperature: Final = ZCLAttributeDef(
+            id=0x0019, type=t.int24s, access="r"
+        )
+        current_in_energy_carrier_demand: Final = ZCLAttributeDef(
+            id=0x001A, type=t.int24s, access="r"
+        )
+        current_out_energy_carrier_demand: Final = ZCLAttributeDef(
+            id=0x001B, type=t.int24s, access="r"
+        )
+        current_block_period_consump_received: Final = ZCLAttributeDef(
+            id=0x001D, type=t.uint48_t, access="r"
+        )
+        current_block_received: Final = ZCLAttributeDef(
+            id=0x001E, type=t.uint48_t, access="r"
+        )
+        dft_summation_received: Final = ZCLAttributeDef(
+            id=0x001F, type=t.uint48_t, access="r"
+        )
+        active_register_tier_delivered: Final = ZCLAttributeDef(
+            id=0x0020, type=RegisteredTier, access="r"
+        )
+        active_register_tier_received: Final = ZCLAttributeDef(
+            id=0x0021, type=RegisteredTier, access="r"
+        )
+        last_block_switch_time: Final = ZCLAttributeDef(
+            id=0x0022, type=t.UTCTime, access="r"
+        )
         # 0x0100: ('change_reporting_profile', UNKNOWN),
-        0x0100: ZCLAttributeDef(
-            "current_tier1_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0101: ZCLAttributeDef(
-            "current_tier1_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0102: ZCLAttributeDef(
-            "current_tier2_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0103: ZCLAttributeDef(
-            "current_tier2_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0104: ZCLAttributeDef(
-            "current_tier3_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0105: ZCLAttributeDef(
-            "current_tier3_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0106: ZCLAttributeDef(
-            "current_tier4_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0107: ZCLAttributeDef(
-            "current_tier4_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0108: ZCLAttributeDef(
-            "current_tier5_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0109: ZCLAttributeDef(
-            "current_tier5_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x010A: ZCLAttributeDef(
-            "current_tier6_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x010B: ZCLAttributeDef(
-            "current_tier6_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x010C: ZCLAttributeDef(
-            "current_tier7_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x010D: ZCLAttributeDef(
-            "current_tier7_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x010E: ZCLAttributeDef(
-            "current_tier8_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x010F: ZCLAttributeDef(
-            "current_tier8_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0110: ZCLAttributeDef(
-            "current_tier9_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0111: ZCLAttributeDef(
-            "current_tier9_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0112: ZCLAttributeDef(
-            "current_tier10_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0113: ZCLAttributeDef(
-            "current_tier10_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0114: ZCLAttributeDef(
-            "current_tier11_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0115: ZCLAttributeDef(
-            "current_tier11_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0116: ZCLAttributeDef(
-            "current_tier12_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0117: ZCLAttributeDef(
-            "current_tier12_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0118: ZCLAttributeDef(
-            "current_tier13_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x0119: ZCLAttributeDef(
-            "current_tier13_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x011A: ZCLAttributeDef(
-            "current_tier14_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x011B: ZCLAttributeDef(
-            "current_tier14_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x011C: ZCLAttributeDef(
-            "current_tier15_summ_delivered", type=t.uint48_t, access="r"
-        ),
-        0x011D: ZCLAttributeDef(
-            "current_tier15_summ_received", type=t.uint48_t, access="r"
-        ),
-        0x0200: ZCLAttributeDef("status", type=t.bitmap8, access="r"),
-        0x0201: ZCLAttributeDef("remaining_battery_life", type=t.uint8_t, access="r"),
-        0x0202: ZCLAttributeDef("hours_in_operation", type=t.uint24_t, access="r"),
-        0x0203: ZCLAttributeDef("hours_in_fault", type=t.uint24_t, access="r"),
-        0x0204: ZCLAttributeDef("extended_status", type=t.bitmap64, access="r"),
-        0x0205: ZCLAttributeDef(
-            "remaining_battery_life_days", type=t.uint16_t, access="r"
-        ),
-        0x0206: ZCLAttributeDef("current_meter_id", type=t.LVBytes, access="r"),
-        0x0207: ZCLAttributeDef(
-            "iambient_consumption_indicator", type=t.enum8, access="r"
-        ),
-        0x0300: ZCLAttributeDef("unit_of_measure", type=t.enum8, access="r"),
-        0x0301: ZCLAttributeDef("multiplier", type=t.uint24_t, access="r"),
-        0x0302: ZCLAttributeDef("divisor", type=t.uint24_t, access="r"),
-        0x0303: ZCLAttributeDef("summation_formatting", type=t.bitmap8, access="r"),
-        0x0304: ZCLAttributeDef("demand_formatting", type=t.bitmap8, access="r"),
-        0x0305: ZCLAttributeDef(
-            "historical_consump_formatting", type=t.bitmap8, access="r"
-        ),
-        0x0306: ZCLAttributeDef("metering_device_type", type=t.bitmap8, access="r"),
-        0x0307: ZCLAttributeDef("site_id", type=t.LimitedLVBytes(32), access="r"),
-        0x0308: ZCLAttributeDef(
-            "meter_serial_number", type=t.LimitedLVBytes(24), access="r"
-        ),
-        0x0309: ZCLAttributeDef(
-            "energy_carrier_unit_of_meas", type=t.enum8, access="r"
-        ),
-        0x030A: ZCLAttributeDef(
-            "energy_carrier_summ_formatting", type=t.bitmap8, access="r"
-        ),
-        0x030B: ZCLAttributeDef(
-            "energy_carrier_demand_formatting", type=t.bitmap8, access="r"
-        ),
-        0x030C: ZCLAttributeDef(
-            "temperature_unit_of_measure", type=t.enum8, access="r"
-        ),
-        0x030D: ZCLAttributeDef("temperature_formatting", type=t.bitmap8, access="r"),
-        0x030E: ZCLAttributeDef(
-            "module_serial_number", type=t.LimitedLVBytes(24), access="r"
-        ),
-        0x030F: ZCLAttributeDef(
-            "operating_tariff_label_delivered", type=t.LimitedLVBytes(24), access="r"
-        ),
-        0x0310: ZCLAttributeDef(
-            "operating_tariff_label_received", type=t.LimitedLVBytes(24), access="r"
-        ),
-        0x0311: ZCLAttributeDef(
-            "customer_id_number", type=t.LimitedLVBytes(24), access="r"
-        ),
-        0x0312: ZCLAttributeDef(
-            "alternative_unit_of_measure", type=t.enum8, access="r"
-        ),
-        0x0313: ZCLAttributeDef(
-            "alternative_demand_formatting", type=t.bitmap8, access="r"
-        ),
-        0x0314: ZCLAttributeDef(
-            "alternative_consumption_formatting", type=t.bitmap8, access="r"
-        ),
-        0x0400: ZCLAttributeDef("instantaneous_demand", type=t.int24s, access="r"),
-        0x0401: ZCLAttributeDef(
-            "currentday_consump_delivered", type=t.uint24_t, access="r"
-        ),
-        0x0402: ZCLAttributeDef(
-            "currentday_consump_received", type=t.uint24_t, access="r"
-        ),
-        0x0403: ZCLAttributeDef(
-            "previousday_consump_delivered", type=t.uint24_t, access="r"
-        ),
-        0x0404: ZCLAttributeDef(
-            "previousday_consump_received", type=t.uint24_t, access="r"
-        ),
-        0x0405: ZCLAttributeDef(
-            "cur_part_profile_int_start_time_delivered", type=t.uint32_t, access="r"
-        ),
-        0x0406: ZCLAttributeDef(
-            "cur_part_profile_int_start_time_received", type=t.uint32_t, access="r"
-        ),
-        0x0407: ZCLAttributeDef(
-            "cur_part_profile_int_value_delivered", type=t.uint24_t, access="r"
-        ),
-        0x0408: ZCLAttributeDef(
-            "cur_part_profile_int_value_received", type=t.uint24_t, access="r"
-        ),
-        0x0409: ZCLAttributeDef(
-            "current_day_max_pressure", type=t.uint48_t, access="r"
-        ),
-        0x040A: ZCLAttributeDef(
-            "current_day_min_pressure", type=t.uint48_t, access="r"
-        ),
-        0x040B: ZCLAttributeDef(
-            "previous_day_max_pressure", type=t.uint48_t, access="r"
-        ),
-        0x040C: ZCLAttributeDef(
-            "previous_day_min_pressure", type=t.uint48_t, access="r"
-        ),
-        0x040D: ZCLAttributeDef("current_day_max_demand", type=t.int24s, access="r"),
-        0x040E: ZCLAttributeDef("previous_day_max_demand", type=t.int24s, access="r"),
-        0x040F: ZCLAttributeDef("current_month_max_demand", type=t.int24s, access="r"),
-        0x0410: ZCLAttributeDef("current_year_max_demand", type=t.int24s, access="r"),
-        0x0411: ZCLAttributeDef(
-            "currentday_max_energy_carr_demand", type=t.int24s, access="r"
-        ),
-        0x0412: ZCLAttributeDef(
-            "previousday_max_energy_carr_demand", type=t.int24s, access="r"
-        ),
-        0x0413: ZCLAttributeDef(
-            "cur_month_max_energy_carr_demand", type=t.int24s, access="r"
-        ),
-        0x0414: ZCLAttributeDef(
-            "cur_month_min_energy_carr_demand", type=t.int24s, access="r"
-        ),
-        0x0415: ZCLAttributeDef(
-            "cur_year_max_energy_carr_demand", type=t.int24s, access="r"
-        ),
-        0x0416: ZCLAttributeDef(
-            "cur_year_min_energy_carr_demand", type=t.int24s, access="r"
-        ),
-        0x0500: ZCLAttributeDef(
-            "max_number_of_periods_delivered", type=t.uint8_t, access="r"
-        ),
-        0x0600: ZCLAttributeDef(
-            "current_demand_delivered", type=t.uint24_t, access="r"
-        ),
-        0x0601: ZCLAttributeDef("demand_limit", type=t.uint24_t, access="r"),
-        0x0602: ZCLAttributeDef(
-            "demand_integration_period", type=t.uint8_t, access="r"
-        ),
-        0x0603: ZCLAttributeDef(
-            "number_of_demand_subintervals", type=t.uint8_t, access="r"
-        ),
-        0x0604: ZCLAttributeDef(
-            "demand_limit_arm_duration", type=t.uint16_t, access="r"
-        ),
-        0x0800: ZCLAttributeDef("generic_alarm_mask", type=t.bitmap16, access="r"),
-        0x0801: ZCLAttributeDef("electricity_alarm_mask", type=t.bitmap32, access="r"),
-        0x0802: ZCLAttributeDef(
-            "gen_flow_pressure_alarm_mask", type=t.bitmap16, access="r"
-        ),
-        0x0803: ZCLAttributeDef(
-            "water_specific_alarm_mask", type=t.bitmap16, access="r"
-        ),
-        0x0804: ZCLAttributeDef(
-            "heat_cool_specific_alarm_mask", type=t.bitmap16, access="r"
-        ),
-        0x0805: ZCLAttributeDef("gas_specific_alarm_mask", type=t.bitmap16, access="r"),
-        0x0806: ZCLAttributeDef(
-            "extended_generic_alarm_mask", type=t.bitmap48, access="r"
-        ),
-        0x0807: ZCLAttributeDef("manufacture_alarm_mask", type=t.bitmap16, access="r"),
-        0x0A00: ZCLAttributeDef("bill_to_date", type=t.uint32_t, access="r"),
-        0x0A01: ZCLAttributeDef("bill_to_date_time_stamp", type=t.uint32_t, access="r"),
-        0x0A02: ZCLAttributeDef("projected_bill", type=t.uint32_t, access="r"),
-        0x0A03: ZCLAttributeDef(
-            "projected_bill_time_stamp", type=t.uint32_t, access="r"
-        ),
-    }
-    server_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef("get_profile", {}, False),
-        0x01: ZCLCommandDef("req_mirror", {}, False),
-        0x02: ZCLCommandDef("mirror_rem", {}, False),
-        0x03: ZCLCommandDef("req_fast_poll_mode", {}, False),
-        0x04: ZCLCommandDef("get_snapshot", {}, False),
-        0x05: ZCLCommandDef("take_snapshot", {}, False),
-        0x06: ZCLCommandDef("mirror_report_attr_response", {}, True),
-    }
-    client_commands: dict[int, ZCLCommandDef] = {
-        0x00: ZCLCommandDef("get_profile_response", {}, True),
-        0x01: ZCLCommandDef("req_mirror_response", {}, True),
-        0x02: ZCLCommandDef("mirror_rem_response", {}, True),
-        0x03: ZCLCommandDef("req_fast_poll_mode_response", {}, True),
-        0x04: ZCLCommandDef("get_snapshot_response", {}, True),
-    }
+        current_tier1_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0100, type=t.uint48_t, access="r"
+        )
+        current_tier1_summ_received: Final = ZCLAttributeDef(
+            id=0x0101, type=t.uint48_t, access="r"
+        )
+        current_tier2_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0102, type=t.uint48_t, access="r"
+        )
+        current_tier2_summ_received: Final = ZCLAttributeDef(
+            id=0x0103, type=t.uint48_t, access="r"
+        )
+        current_tier3_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0104, type=t.uint48_t, access="r"
+        )
+        current_tier3_summ_received: Final = ZCLAttributeDef(
+            id=0x0105, type=t.uint48_t, access="r"
+        )
+        current_tier4_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0106, type=t.uint48_t, access="r"
+        )
+        current_tier4_summ_received: Final = ZCLAttributeDef(
+            id=0x0107, type=t.uint48_t, access="r"
+        )
+        current_tier5_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0108, type=t.uint48_t, access="r"
+        )
+        current_tier5_summ_received: Final = ZCLAttributeDef(
+            id=0x0109, type=t.uint48_t, access="r"
+        )
+        current_tier6_summ_delivered: Final = ZCLAttributeDef(
+            id=0x010A, type=t.uint48_t, access="r"
+        )
+        current_tier6_summ_received: Final = ZCLAttributeDef(
+            id=0x010B, type=t.uint48_t, access="r"
+        )
+        current_tier7_summ_delivered: Final = ZCLAttributeDef(
+            id=0x010C, type=t.uint48_t, access="r"
+        )
+        current_tier7_summ_received: Final = ZCLAttributeDef(
+            id=0x010D, type=t.uint48_t, access="r"
+        )
+        current_tier8_summ_delivered: Final = ZCLAttributeDef(
+            id=0x010E, type=t.uint48_t, access="r"
+        )
+        current_tier8_summ_received: Final = ZCLAttributeDef(
+            id=0x010F, type=t.uint48_t, access="r"
+        )
+        current_tier9_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0110, type=t.uint48_t, access="r"
+        )
+        current_tier9_summ_received: Final = ZCLAttributeDef(
+            id=0x0111, type=t.uint48_t, access="r"
+        )
+        current_tier10_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0112, type=t.uint48_t, access="r"
+        )
+        current_tier10_summ_received: Final = ZCLAttributeDef(
+            id=0x0113, type=t.uint48_t, access="r"
+        )
+        current_tier11_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0114, type=t.uint48_t, access="r"
+        )
+        current_tier11_summ_received: Final = ZCLAttributeDef(
+            id=0x0115, type=t.uint48_t, access="r"
+        )
+        current_tier12_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0116, type=t.uint48_t, access="r"
+        )
+        current_tier12_summ_received: Final = ZCLAttributeDef(
+            id=0x0117, type=t.uint48_t, access="r"
+        )
+        current_tier13_summ_delivered: Final = ZCLAttributeDef(
+            id=0x0118, type=t.uint48_t, access="r"
+        )
+        current_tier13_summ_received: Final = ZCLAttributeDef(
+            id=0x0119, type=t.uint48_t, access="r"
+        )
+        current_tier14_summ_delivered: Final = ZCLAttributeDef(
+            id=0x011A, type=t.uint48_t, access="r"
+        )
+        current_tier14_summ_received: Final = ZCLAttributeDef(
+            id=0x011B, type=t.uint48_t, access="r"
+        )
+        current_tier15_summ_delivered: Final = ZCLAttributeDef(
+            id=0x011C, type=t.uint48_t, access="r"
+        )
+        current_tier15_summ_received: Final = ZCLAttributeDef(
+            id=0x011D, type=t.uint48_t, access="r"
+        )
+        status: Final = ZCLAttributeDef(id=0x0200, type=t.bitmap8, access="r")
+        remaining_battery_life: Final = ZCLAttributeDef(
+            id=0x0201, type=t.uint8_t, access="r"
+        )
+        hours_in_operation: Final = ZCLAttributeDef(
+            id=0x0202, type=t.uint24_t, access="r"
+        )
+        hours_in_fault: Final = ZCLAttributeDef(id=0x0203, type=t.uint24_t, access="r")
+        extended_status: Final = ZCLAttributeDef(id=0x0204, type=t.bitmap64, access="r")
+        remaining_battery_life_days: Final = ZCLAttributeDef(
+            id=0x0205, type=t.uint16_t, access="r"
+        )
+        current_meter_id: Final = ZCLAttributeDef(id=0x0206, type=t.LVBytes, access="r")
+        iambient_consumption_indicator: Final = ZCLAttributeDef(
+            id=0x0207, type=t.enum8, access="r"
+        )
+        unit_of_measure: Final = ZCLAttributeDef(id=0x0300, type=t.enum8, access="r")
+        multiplier: Final = ZCLAttributeDef(id=0x0301, type=t.uint24_t, access="r")
+        divisor: Final = ZCLAttributeDef(id=0x0302, type=t.uint24_t, access="r")
+        summation_formatting: Final = ZCLAttributeDef(
+            id=0x0303, type=t.bitmap8, access="r"
+        )
+        demand_formatting: Final = ZCLAttributeDef(
+            id=0x0304, type=t.bitmap8, access="r"
+        )
+        historical_consump_formatting: Final = ZCLAttributeDef(
+            id=0x0305, type=t.bitmap8, access="r"
+        )
+        metering_device_type: Final = ZCLAttributeDef(
+            id=0x0306, type=t.bitmap8, access="r"
+        )
+        site_id: Final = ZCLAttributeDef(
+            id=0x0307, type=t.LimitedLVBytes(32), access="r"
+        )
+        meter_serial_number: Final = ZCLAttributeDef(
+            id=0x0308, type=t.LimitedLVBytes(24), access="r"
+        )
+        energy_carrier_unit_of_meas: Final = ZCLAttributeDef(
+            id=0x0309, type=t.enum8, access="r"
+        )
+        energy_carrier_summ_formatting: Final = ZCLAttributeDef(
+            id=0x030A, type=t.bitmap8, access="r"
+        )
+        energy_carrier_demand_formatting: Final = ZCLAttributeDef(
+            id=0x030B, type=t.bitmap8, access="r"
+        )
+        temperature_unit_of_measure: Final = ZCLAttributeDef(
+            id=0x030C, type=t.enum8, access="r"
+        )
+        temperature_formatting: Final = ZCLAttributeDef(
+            id=0x030D, type=t.bitmap8, access="r"
+        )
+        module_serial_number: Final = ZCLAttributeDef(
+            id=0x030E, type=t.LimitedLVBytes(24), access="r"
+        )
+        operating_tariff_label_delivered: Final = ZCLAttributeDef(
+            id=0x030F, type=t.LimitedLVBytes(24), access="r"
+        )
+        operating_tariff_label_received: Final = ZCLAttributeDef(
+            id=0x0310, type=t.LimitedLVBytes(24), access="r"
+        )
+        customer_id_number: Final = ZCLAttributeDef(
+            id=0x0311, type=t.LimitedLVBytes(24), access="r"
+        )
+        alternative_unit_of_measure: Final = ZCLAttributeDef(
+            id=0x0312, type=t.enum8, access="r"
+        )
+        alternative_demand_formatting: Final = ZCLAttributeDef(
+            id=0x0313, type=t.bitmap8, access="r"
+        )
+        alternative_consumption_formatting: Final = ZCLAttributeDef(
+            id=0x0314, type=t.bitmap8, access="r"
+        )
+        instantaneous_demand: Final = ZCLAttributeDef(
+            id=0x0400, type=t.int24s, access="r"
+        )
+        currentday_consump_delivered: Final = ZCLAttributeDef(
+            id=0x0401, type=t.uint24_t, access="r"
+        )
+        currentday_consump_received: Final = ZCLAttributeDef(
+            id=0x0402, type=t.uint24_t, access="r"
+        )
+        previousday_consump_delivered: Final = ZCLAttributeDef(
+            id=0x0403, type=t.uint24_t, access="r"
+        )
+        previousday_consump_received: Final = ZCLAttributeDef(
+            id=0x0404, type=t.uint24_t, access="r"
+        )
+        cur_part_profile_int_start_time_delivered: Final = ZCLAttributeDef(
+            id=0x0405, type=t.uint32_t, access="r"
+        )
+        cur_part_profile_int_start_time_received: Final = ZCLAttributeDef(
+            id=0x0406, type=t.uint32_t, access="r"
+        )
+        cur_part_profile_int_value_delivered: Final = ZCLAttributeDef(
+            id=0x0407, type=t.uint24_t, access="r"
+        )
+        cur_part_profile_int_value_received: Final = ZCLAttributeDef(
+            id=0x0408, type=t.uint24_t, access="r"
+        )
+        current_day_max_pressure: Final = ZCLAttributeDef(
+            id=0x0409, type=t.uint48_t, access="r"
+        )
+        current_day_min_pressure: Final = ZCLAttributeDef(
+            id=0x040A, type=t.uint48_t, access="r"
+        )
+        previous_day_max_pressure: Final = ZCLAttributeDef(
+            id=0x040B, type=t.uint48_t, access="r"
+        )
+        previous_day_min_pressure: Final = ZCLAttributeDef(
+            id=0x040C, type=t.uint48_t, access="r"
+        )
+        current_day_max_demand: Final = ZCLAttributeDef(
+            id=0x040D, type=t.int24s, access="r"
+        )
+        previous_day_max_demand: Final = ZCLAttributeDef(
+            id=0x040E, type=t.int24s, access="r"
+        )
+        current_month_max_demand: Final = ZCLAttributeDef(
+            id=0x040F, type=t.int24s, access="r"
+        )
+        current_year_max_demand: Final = ZCLAttributeDef(
+            id=0x0410, type=t.int24s, access="r"
+        )
+        currentday_max_energy_carr_demand: Final = ZCLAttributeDef(
+            id=0x0411, type=t.int24s, access="r"
+        )
+        previousday_max_energy_carr_demand: Final = ZCLAttributeDef(
+            id=0x0412, type=t.int24s, access="r"
+        )
+        cur_month_max_energy_carr_demand: Final = ZCLAttributeDef(
+            id=0x0413, type=t.int24s, access="r"
+        )
+        cur_month_min_energy_carr_demand: Final = ZCLAttributeDef(
+            id=0x0414, type=t.int24s, access="r"
+        )
+        cur_year_max_energy_carr_demand: Final = ZCLAttributeDef(
+            id=0x0415, type=t.int24s, access="r"
+        )
+        cur_year_min_energy_carr_demand: Final = ZCLAttributeDef(
+            id=0x0416, type=t.int24s, access="r"
+        )
+        max_number_of_periods_delivered: Final = ZCLAttributeDef(
+            id=0x0500, type=t.uint8_t, access="r"
+        )
+        current_demand_delivered: Final = ZCLAttributeDef(
+            id=0x0600, type=t.uint24_t, access="r"
+        )
+        demand_limit: Final = ZCLAttributeDef(id=0x0601, type=t.uint24_t, access="r")
+        demand_integration_period: Final = ZCLAttributeDef(
+            id=0x0602, type=t.uint8_t, access="r"
+        )
+        number_of_demand_subintervals: Final = ZCLAttributeDef(
+            id=0x0603, type=t.uint8_t, access="r"
+        )
+        demand_limit_arm_duration: Final = ZCLAttributeDef(
+            id=0x0604, type=t.uint16_t, access="r"
+        )
+        generic_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0800, type=t.bitmap16, access="r"
+        )
+        electricity_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0801, type=t.bitmap32, access="r"
+        )
+        gen_flow_pressure_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0802, type=t.bitmap16, access="r"
+        )
+        water_specific_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0803, type=t.bitmap16, access="r"
+        )
+        heat_cool_specific_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0804, type=t.bitmap16, access="r"
+        )
+        gas_specific_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0805, type=t.bitmap16, access="r"
+        )
+        extended_generic_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0806, type=t.bitmap48, access="r"
+        )
+        manufacture_alarm_mask: Final = ZCLAttributeDef(
+            id=0x0807, type=t.bitmap16, access="r"
+        )
+        bill_to_date: Final = ZCLAttributeDef(id=0x0A00, type=t.uint32_t, access="r")
+        bill_to_date_time_stamp: Final = ZCLAttributeDef(
+            id=0x0A01, type=t.uint32_t, access="r"
+        )
+        projected_bill: Final = ZCLAttributeDef(id=0x0A02, type=t.uint32_t, access="r")
+        projected_bill_time_stamp: Final = ZCLAttributeDef(
+            id=0x0A03, type=t.uint32_t, access="r"
+        )
+
+    class ServerCommandDefs(BaseCommandDefs):
+        get_profile: Final = ZCLCommandDef(id=0x00, schema={}, direction=False)
+        req_mirror: Final = ZCLCommandDef(id=0x01, schema={}, direction=False)
+        mirror_rem: Final = ZCLCommandDef(id=0x02, schema={}, direction=False)
+        req_fast_poll_mode: Final = ZCLCommandDef(id=0x03, schema={}, direction=False)
+        get_snapshot: Final = ZCLCommandDef(id=0x04, schema={}, direction=False)
+        take_snapshot: Final = ZCLCommandDef(id=0x05, schema={}, direction=False)
+        mirror_report_attr_response: Final = ZCLCommandDef(
+            id=0x06, schema={}, direction=True
+        )
+
+    class ClientCommandDefs(BaseCommandDefs):
+        get_profile_response: Final = ZCLCommandDef(id=0x00, schema={}, direction=True)
+        req_mirror_response: Final = ZCLCommandDef(id=0x01, schema={}, direction=True)
+        mirror_rem_response: Final = ZCLCommandDef(id=0x02, schema={}, direction=True)
+        req_fast_poll_mode_response: Final = ZCLCommandDef(
+            id=0x03, schema={}, direction=True
+        )
+        get_snapshot_response: Final = ZCLCommandDef(id=0x04, schema={}, direction=True)
 
 
 class Messaging(Cluster):
-    cluster_id = 0x0703
-    ep_attribute = "smartenergy_messaging"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0703
+    ep_attribute: Final = "smartenergy_messaging"
 
 
 class Tunneling(Cluster):
-    cluster_id = 0x0704
-    ep_attribute = "smartenergy_tunneling"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0704
+    ep_attribute: Final = "smartenergy_tunneling"
 
 
 class Prepayment(Cluster):
-    cluster_id = 0x0705
-    ep_attribute = "smartenergy_prepayment"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0705
+    ep_attribute: Final = "smartenergy_prepayment"
 
 
 class EnergyManagement(Cluster):
-    cluster_id = 0x0706
-    ep_attribute = "smartenergy_energy_management"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0706
+    ep_attribute: Final = "smartenergy_energy_management"
 
 
 class Calendar(Cluster):
-    cluster_id = 0x0707
-    ep_attribute = "smartenergy_calendar"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0707
+    ep_attribute: Final = "smartenergy_calendar"
 
 
 class DeviceManagement(Cluster):
-    cluster_id = 0x0708
-    ep_attribute = "smartenergy_device_management"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0708
+    ep_attribute: Final = "smartenergy_device_management"
 
 
 class Events(Cluster):
-    cluster_id = 0x0709
-    ep_attribute = "smartenergy_events"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0709
+    ep_attribute: Final = "smartenergy_events"
 
 
 class MduPairing(Cluster):
-    cluster_id = 0x070A
-    ep_attribute = "smartenergy_mdu_pairing"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x070A
+    ep_attribute: Final = "smartenergy_mdu_pairing"
 
 
 class KeyEstablishment(Cluster):
-    cluster_id = 0x0800
-    ep_attribute = "smartenergy_key_establishment"
-    attributes: dict[int, ZCLAttributeDef] = {}
-    server_commands: dict[int, ZCLCommandDef] = {}
-    client_commands: dict[int, ZCLCommandDef] = {}
+    cluster_id: Final = 0x0800
+    ep_attribute: Final = "smartenergy_key_establishment"
```

### Comparing `zigpy-0.55.0/zigpy/zcl/foundation.py` & `zigpy-0.56.0/zigpy/zcl/foundation.py`

 * *Files 2% similar despite different names*

```diff
@@ -628,21 +628,28 @@
             tsn=tsn,
             command_id=command_id,
         )
 
 
 @dataclasses.dataclass(frozen=True)
 class ZCLCommandDef(t.BaseDataclassMixin):
-    name: str = None
+    id: t.uint8_t = None
     schema: CommandSchema = None
     direction: Direction = None
-    id: t.uint8_t = None
     is_manufacturer_specific: bool = None
 
+    # set later
+    name: str = None
+
     def __post_init__(self) -> None:
+        # Backwards compatibility with positional syntax where the name was first
+        if isinstance(self.id, str):
+            object.__setattr__(self, "name", self.id)
+            object.__setattr__(self, "id", None)
+
         ensure_valid_name(self.name)
 
         if isinstance(self.direction, bool):
             object.__setattr__(
                 self, "direction", Direction._from_is_reply(self.direction)
             )
 
@@ -758,35 +765,39 @@
     ZCLAttributeAccess.Report: "p",
     ZCLAttributeAccess.Scene: "s",
 }
 
 
 @dataclasses.dataclass(frozen=True)
 class ZCLAttributeDef(t.BaseDataclassMixin):
-    name: str = None
+    id: t.uint16_t = None
     type: type = None
     access: ZCLAttributeAccess = dataclasses.field(
         default=(
             ZCLAttributeAccess.Read
             | ZCLAttributeAccess.Write
             | ZCLAttributeAccess.Report
         ),
     )
     mandatory: bool = False
     is_manufacturer_specific: bool = False
 
-    # The ID will be specified later
-    id: t.uint16_t = None
+    # The name will be specified later
+    name: str = None
 
     def __post_init__(self) -> None:
+        # Backwards compatibility with positional syntax where the name was first
+        if isinstance(self.id, str):
+            object.__setattr__(self, "name", self.id)
+            object.__setattr__(self, "id", None)
+
         if self.id is not None and not isinstance(self.id, t.uint16_t):
             object.__setattr__(self, "id", t.uint16_t(self.id))
 
         if isinstance(self.access, str):
-            ZCLAttributeAccess.NONE
             object.__setattr__(self, "access", ZCLAttributeAccess.from_str(self.access))
 
         ensure_valid_name(self.name)
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}("
@@ -796,14 +807,29 @@
             f"access={self.access!r}, "
             f"mandatory={self.mandatory!r}, "
             f"is_manufacturer_specific={self.is_manufacturer_specific}"
             f")"
         )
 
 
+class IterableMemberMeta(type):
+    def __iter__(cls) -> typing.Iterable[typing.Any]:
+        for name in dir(cls):
+            if not name.startswith("_"):
+                yield getattr(cls, name)
+
+
+class BaseCommandDefs(metaclass=IterableMemberMeta):
+    pass
+
+
+class BaseAttributeDefs(metaclass=IterableMemberMeta):
+    pass
+
+
 class GeneralCommand(t.enum8):
     """ZCL Foundation General Command IDs."""
 
     Read_Attributes = 0x00
     Read_Attributes_rsp = 0x01
     Write_Attributes = 0x02
     Write_Attributes_Undivided = 0x03
@@ -919,12 +945,12 @@
 
 for command_id, command_def in list(GENERAL_COMMANDS.items()):
     GENERAL_COMMANDS[command_id] = command_def.replace(
         id=command_id, name=command_id.name
     ).with_compiled_schema()
 
 ZCL_CLUSTER_REVISION_ATTR = ZCLAttributeDef(
-    "cluster_revision", type=t.uint16_t, access="r", mandatory=True
+    id=0xFFFD, type=t.uint16_t, access="r", mandatory=True
 )
 ZCL_REPORTING_STATUS_ATTR = ZCLAttributeDef(
-    "attr_reporting_status", type=AttributeReportingStatus, access="r"
+    id=0xFFFE, type=AttributeReportingStatus, access="r"
 )
```

### Comparing `zigpy-0.55.0/zigpy/zdo/__init__.py` & `zigpy-0.56.0/zigpy/zdo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
         if data:
             # TODO: Seems sane to check, but what should we do?
             self.warning("Data remains after deserializing ZDO frame: %r", data)
 
         return hdr, args
 
-    @zigpy.util.retryable_request
     def request(self, command, *args, use_ieee=False):
         data = self._serialize(command, *args)
         tsn = self.device.application.get_sequence()
         data = t.uint8_t(tsn).serialize() + data
         return self._device.request(0, command, 0, 0, tsn, data, use_ieee=use_ieee)
 
     def reply(self, command, *args, tsn=None, use_ieee=False):
```

### Comparing `zigpy-0.55.0/zigpy/zdo/types.py` & `zigpy-0.56.0/zigpy/zdo/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.55.0/zigpy.egg-info/PKG-INFO` & `zigpy-0.56.0/zigpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.55.0
+Version: 0.56.0
 Summary: Library implementing a ZigBee stack
 Home-page: https://github.com/zigpy/zigpy
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zigpy-0.55.0/zigpy.egg-info/SOURCES.txt` & `zigpy-0.56.0/zigpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 zigpy.egg-info/requires.txt
 zigpy.egg-info/top_level.txt
 zigpy/appdb_schemas/__init__.py
 zigpy/appdb_schemas/schema_v0.sql
 zigpy/appdb_schemas/schema_v1.sql
 zigpy/appdb_schemas/schema_v10.sql
 zigpy/appdb_schemas/schema_v11.sql
+zigpy/appdb_schemas/schema_v12.sql
 zigpy/appdb_schemas/schema_v2.sql
 zigpy/appdb_schemas/schema_v3.sql
 zigpy/appdb_schemas/schema_v4.sql
 zigpy/appdb_schemas/schema_v5.sql
 zigpy/appdb_schemas/schema_v6.sql
 zigpy/appdb_schemas/schema_v7.sql
 zigpy/appdb_schemas/schema_v8.sql
@@ -40,14 +41,15 @@
 zigpy/config/defaults.py
 zigpy/config/validators.py
 zigpy/ota/__init__.py
 zigpy/ota/image.py
 zigpy/ota/provider.py
 zigpy/ota/validators.py
 zigpy/profiles/__init__.py
+zigpy/profiles/zgp.py
 zigpy/profiles/zha.py
 zigpy/profiles/zll.py
 zigpy/quirks/__init__.py
 zigpy/quirks/registry.py
 zigpy/types/__init__.py
 zigpy/types/basic.py
 zigpy/types/named.py
```

