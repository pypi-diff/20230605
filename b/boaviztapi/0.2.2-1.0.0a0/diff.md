# Comparing `tmp/boaviztapi-0.2.2.tar.gz` & `tmp/boaviztapi-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boaviztapi-0.2.2.tar", last modified: Wed Dec 21 13:43:40 2022, max compression
+gzip compressed data, was "boaviztapi-1.0.0a0.tar", max compression
```

## Comparing `boaviztapi-0.2.2.tar` & `boaviztapi-1.0.0a0.tar`

### file list

```diff
@@ -1,120 +1,85 @@
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.580411 boaviztapi-0.2.2/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)    34523 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/LICENSE
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      131 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/MANIFEST.in
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     4793 2022-12-21 13:43:40.580411 boaviztapi-0.2.2/PKG-INFO
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      507 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/Pipfile
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)    64194 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/Pipfile.lock
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     4199 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/README.md
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.560410 boaviztapi-0.2.2/boaviztapi/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       22 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/boaviztapi/__init__.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.556410 boaviztapi-0.2.2/boaviztapi/data/
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.564410 boaviztapi-0.2.2/boaviztapi/data/components/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)    57393 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/data/components/cpu_index.csv
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     7008 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/data/components/cpu_manufacture.csv
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1307 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/boaviztapi/data/components/missing_cpu_manufacture.csv
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      214 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/data/components/ram_manufacture.csv
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       58 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/boaviztapi/data/components/ssd_manufacture.csv
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.556410 boaviztapi-0.2.2/boaviztapi/data/consumption_profile/
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.564410 boaviztapi-0.2.2/boaviztapi/data/consumption_profile/cpu/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      313 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/data/consumption_profile/cpu/cpu_profile.csv
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.556410 boaviztapi-0.2.2/boaviztapi/data/devices/
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.564410 boaviztapi-0.2.2/boaviztapi/data/devices/cloud/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)    86358 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/data/devices/cloud/aws.csv
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      559 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/data/devices/cloud/gcp.csv
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       58 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/boaviztapi/data/devices/cloud/providers.csv
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.564410 boaviztapi-0.2.2/boaviztapi/data/devices/server/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1273 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/data/devices/server/server.csv
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.564410 boaviztapi-0.2.2/boaviztapi/data/electricity/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)    38832 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/data/electricity/electricity_impact_factors.csv
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.564410 boaviztapi-0.2.2/boaviztapi/dto/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       30 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      123 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/base_dto.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.568410 boaviztapi-0.2.2/boaviztapi/dto/component/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      154 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/component/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      209 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/component/component_dto.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     6073 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/component/cpu.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     3192 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/component/disk.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1669 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/component/other.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2808 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/component/ram.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.568410 boaviztapi-0.2.2/boaviztapi/dto/consumption_profile/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       55 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/consumption_profile/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1912 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/consumption_profile/consumption_profile.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.568410 boaviztapi-0.2.2/boaviztapi/dto/device/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       45 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/device/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     4568 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/boaviztapi/dto/device/device.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.568410 boaviztapi-0.2.2/boaviztapi/dto/usage/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       50 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/usage/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     6515 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/dto/usage/usage.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     3012 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/main.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.568410 boaviztapi-0.2.2/boaviztapi/model/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/boaviztapi/model/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2663 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/boattribute.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.568410 boaviztapi-0.2.2/boaviztapi/model/component/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      318 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1381 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/assembly.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     3597 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/case.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2193 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/component.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     5233 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/cpu.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1235 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/hdd.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1051 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/motherboard.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1820 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/power_supply.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     4462 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/ram.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2334 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/component/ssd.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.572410 boaviztapi-0.2.2/boaviztapi/model/consumption_profile/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       88 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/consumption_profile/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     7459 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/consumption_profile/consumption_profile.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.572410 boaviztapi-0.2.2/boaviztapi/model/device/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       81 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/device/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1344 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/device/device.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     8249 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/device/server.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.572410 boaviztapi-0.2.2/boaviztapi/model/usage/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       65 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/usage/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     3511 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/model/usage/usage.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.572410 boaviztapi-0.2.2/boaviztapi/routers/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       73 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/routers/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     4669 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/boaviztapi/routers/cloud_router.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     4865 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/routers/component_router.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      958 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/routers/consumption_profile_router.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.572410 boaviztapi-0.2.2/boaviztapi/routers/openapi_doc/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/boaviztapi/routers/openapi_doc/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     8943 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/boaviztapi/routers/openapi_doc/descriptions.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2693 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/boaviztapi/routers/openapi_doc/examples.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2314 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/boaviztapi/routers/openapi_doc/intro_openapi.md
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2987 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/routers/server_router.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2395 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/routers/utils_router.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.576411 boaviztapi-0.2.2/boaviztapi/service/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       73 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/boaviztapi/service/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      489 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/service/allocation.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2629 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/boaviztapi/service/archetype.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2767 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/service/bottom_up.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     2601 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/service/verbose.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.576411 boaviztapi-0.2.2/boaviztapi/utils/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/boaviztapi/utils/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      652 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/utils/fuzzymatch.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     3141 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/boaviztapi/utils/roundit.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.564410 boaviztapi-0.2.2/boaviztapi.egg-info/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     4793 2022-12-21 13:43:40.000000 boaviztapi-0.2.2/boaviztapi.egg-info/PKG-INFO
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     3051 2022-12-21 13:43:40.000000 boaviztapi-0.2.2/boaviztapi.egg-info/SOURCES.txt
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        1 2022-12-21 13:43:40.000000 boaviztapi-0.2.2/boaviztapi.egg-info/dependency_links.txt
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       78 2022-12-21 13:43:40.000000 boaviztapi-0.2.2/boaviztapi.egg-info/requires.txt
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       17 2022-12-21 13:43:40.000000 boaviztapi-0.2.2/boaviztapi.egg-info/top_level.txt
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       38 2022-12-21 13:43:40.580411 boaviztapi-0.2.2/setup.cfg
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1152 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/setup.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.560410 boaviztapi-0.2.2/tests/
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.576411 boaviztapi-0.2.2/tests/api/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/tests/api/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     8836 2022-12-21 13:16:54.000000 boaviztapi-0.2.2/tests/api/test_cloud.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)    22196 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/api/test_component.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     8577 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/api/test_server.py
-drwxrwxr-x   0 david_ekchajzer  (1000) david_ekchajzer  (1000)        0 2022-12-21 13:43:40.580411 boaviztapi-0.2.2/tests/unit/
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       73 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/tests/unit/__init__.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     9491 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/unit/conftest.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      446 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/unit/test_allocation.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1265 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/unit/test_archetype.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     6236 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/unit/test_bottom_up.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     6644 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/unit/test_consumption_profile.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      714 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/unit/test_fuzzymatch.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)       57 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/unit/test_mapper.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     1340 2022-11-21 16:04:11.000000 boaviztapi-0.2.2/tests/unit/test_roundit.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)      879 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/unit/test_use.py
--rw-rw-r--   0 david_ekchajzer  (1000) david_ekchajzer  (1000)     6617 2022-12-05 16:48:40.000000 boaviztapi-0.2.2/tests/unit/test_verb.py
+-rw-r--r--   0        0        0    34523 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/LICENSE
+-rw-r--r--   0        0        0     4494 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/README.md
+-rw-r--r--   0        0        0      365 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/__init__.py
+-rw-r--r--   0        0        0   114581 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/cloud/aws.csv
+-rw-r--r--   0        0        0      559 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/cloud/gcp.csv
+-rw-r--r--   0        0        0       58 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/cloud/providers.csv
+-rw-r--r--   0        0        0      116 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/components/case.csv
+-rw-r--r--   0        0        0      268 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/components/cpu.csv
+-rw-r--r--   0        0        0       95 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/components/hdd.csv
+-rw-r--r--   0        0        0       97 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/components/power_supply.csv
+-rw-r--r--   0        0        0      162 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/components/ram.csv
+-rw-r--r--   0        0        0      130 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/components/ssd.csv
+-rw-r--r--   0        0        0     1242 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/server.csv
+-rw-r--r--   0        0        0      921 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/archetypes/user_terminal.csv
+-rw-r--r--   0        0        0      819 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/config.yml
+-rw-r--r--   0        0        0      314 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/consumption_profile/cpu/cpu_profile.csv
+-rw-r--r--   0        0        0     3404 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/crowdsourcing/ademe_base_impacts_negaoctet.csv
+-rw-r--r--   0        0        0     4553 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/crowdsourcing/cpu_manufacture.csv
+-rw-r--r--   0        0        0   515038 2023-06-05 08:22:45.049601 boaviztapi-1.0.0a0/boaviztapi/data/crowdsourcing/cpu_specs.csv
+-rw-r--r--   0        0        0    26045 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/data/crowdsourcing/electrical_mix.csv
+-rw-r--r--   0        0        0      113 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/data/crowdsourcing/missing_cpu_manufacture.csv
+-rw-r--r--   0        0        0      214 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/data/crowdsourcing/ram_manufacture.csv
+-rw-r--r--   0        0        0     2274 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/data/crowdsourcing/ssd_manufacture.csv
+-rw-r--r--   0        0        0   425401 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/data/factors.yml
+-rw-r--r--   0        0        0     2259 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/data/utils/jsonifyer.py
+-rw-r--r--   0        0        0       30 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/__init__.py
+-rw-r--r--   0        0        0      123 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/base_dto.py
+-rw-r--r--   0        0        0      154 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/component/__init__.py
+-rw-r--r--   0        0        0      205 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/component/component_dto.py
+-rw-r--r--   0        0        0     2199 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/component/cpu.py
+-rw-r--r--   0        0        0     1814 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/component/disk.py
+-rw-r--r--   0        0        0     1994 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/component/other.py
+-rw-r--r--   0        0        0     1440 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/component/ram.py
+-rw-r--r--   0        0        0       55 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/consumption_profile/__init__.py
+-rw-r--r--   0        0        0     1633 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/consumption_profile/consumption_profile.py
+-rw-r--r--   0        0        0       45 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/device/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/device/device.py
+-rw-r--r--   0        0        0     2629 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/device/user_terminal.py
+-rw-r--r--   0        0        0       50 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/usage/__init__.py
+-rw-r--r--   0        0        0     6577 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/dto/usage/usage.py
+-rw-r--r--   0        0        0     3329 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/main.py
+-rw-r--r--   0        0        0      143 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/__init__.py
+-rw-r--r--   0        0        0     3866 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/boattribute.py
+-rw-r--r--   0        0        0      318 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/__init__.py
+-rw-r--r--   0        0        0     1106 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/assembly.py
+-rw-r--r--   0        0        0     5052 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/case.py
+-rw-r--r--   0        0        0     2150 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/component.py
+-rw-r--r--   0        0        0    14232 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/cpu.py
+-rw-r--r--   0        0        0     1460 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/hdd.py
+-rw-r--r--   0        0        0      941 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/motherboard.py
+-rw-r--r--   0        0        0     2004 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/power_supply.py
+-rw-r--r--   0        0        0     7197 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/ram.py
+-rw-r--r--   0        0        0     4960 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/component/ssd.py
+-rw-r--r--   0        0        0       88 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/consumption_profile/__init__.py
+-rw-r--r--   0        0        0     7244 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/consumption_profile/consumption_profile.py
+-rw-r--r--   0        0        0       81 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/device/__init__.py
+-rw-r--r--   0        0        0     1134 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/device/device.py
+-rw-r--r--   0        0        0     8965 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/device/server.py
+-rw-r--r--   0        0        0     7261 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/device/userTerminal.py
+-rw-r--r--   0        0        0     3983 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/impact.py
+-rw-r--r--   0        0        0       65 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/usage/__init__.py
+-rw-r--r--   0        0        0     8503 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/model/usage/usage.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/routers/__init__.py
+-rw-r--r--   0        0        0     4052 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/routers/cloud_router.py
+-rw-r--r--   0        0        0    17594 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/routers/component_router.py
+-rw-r--r--   0        0        0      958 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/routers/consumption_profile_router.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/routers/openapi_doc/__init__.py
+-rw-r--r--   0        0        0     9638 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/routers/openapi_doc/descriptions.py
+-rw-r--r--   0        0        0     2624 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/routers/openapi_doc/examples.py
+-rw-r--r--   0        0        0     2207 2023-06-05 08:22:45.053602 boaviztapi-1.0.0a0/boaviztapi/routers/openapi_doc/intro_openapi.md
+-rw-r--r--   0        0        0     8625 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/routers/peripheral_router.py
+-rw-r--r--   0        0        0     3612 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/routers/server_router.py
+-rw-r--r--   0        0        0    13529 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/routers/terminal_router.py
+-rw-r--r--   0        0        0     2864 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/routers/utils_router.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/service/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/service/allocation.py
+-rw-r--r--   0        0        0     4276 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/service/archetype.py
+-rw-r--r--   0        0        0     2199 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/service/bottom_up.py
+-rw-r--r--   0        0        0     3280 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/service/factor_provider.py
+-rw-r--r--   0        0        0     2646 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/service/verbose.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/utils/__init__.py
+-rw-r--r--   0        0        0     1405 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/utils/fuzzymatch.py
+-rw-r--r--   0        0        0     3257 2023-06-05 08:22:45.057602 boaviztapi-1.0.0a0/boaviztapi/utils/roundit.py
+-rw-r--r--   0        0        0      699 2023-06-05 08:22:45.073602 boaviztapi-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 boaviztapi-1.0.0a0/PKG-INFO
```

### Comparing `boaviztapi-0.2.2/LICENSE` & `boaviztapi-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `boaviztapi-0.2.2/PKG-INFO` & `boaviztapi-1.0.0a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 Metadata-Version: 2.1
 Name: boaviztapi
-Version: 0.2.2
-Summary: Giving access to BOAVIZTA referenced datas and methodologies trought a RESTful api 
-Home-page: https://github.com/Boavizta/Tools-API
-Keywords: boavizta,api
+Version: 1.0.0a0
+Summary: An API to access Boavizta's methodologies and footprint reference data
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofile (>=3.8,<4.0)
+Requires-Dist: fastapi (>=0.95,<0.96)
+Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
+Requires-Dist: mangum (>=0.17,<0.18)
+Requires-Dist: markdown (>=3.4,<4.0)
+Requires-Dist: numpy (>=1.24,<2.0)
+Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: rapidfuzz (>=3.0,<4.0)
+Requires-Dist: scipy (>=1.9,<2.0)
+Requires-Dist: uvicorn (>=0.22,<0.23)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Boavizta/boaviztapi/dev/boavizta-logo-4.png" width="100">
 </p>
 <h1 align="center">
   Boavizta API
 </h1>
 
 ---
 
-An API to access [Boavizta's](https://boavizta.cmakers.io/) methodologies and footprint [reference data](https://github.com/Boavizta/environmental-footprint-data).
+An API to access [Boavizta's](https://boavizta.cmakers.io/) methodologies and impacts data [reference data](https://github.com/Boavizta/environmental-footprint-data).
 
 See the [documentation](https://doc.api.boavizta.org/) for API usage and methodology.
 
 [![Python tests](https://github.com/Boavizta/boaviztapi/actions/workflows/test.yml/badge.svg)](https://github.com/Boavizta/boaviztapi/actions/workflows/test.yml)
 
 ## :dart: Objective
 
-As part of Boavizta's desire to improve the quality of the measurement of the environmental impacts of ICTs in organizations, this project aims at giving access to the group's work to as many people as possible in an automated and industrialized way.
+Boavizta aims to enhance the assessment of environmental impacts induced by ICTs in organizations by providing widespread access to our work in an automated and efficient manner.
 
-The various data and methodologies integrated by Boavizta are aggregated and made available via an API.
+Boavizta integrates various data and methodologies, which are combined and made accessible through this API.
 
-In the interest of transparency and scientific popularization, the opening of the code, the versioning of the impact factors and the documentation of the project are critical points.
+Transparency and the popularization of scientific knowledge are of utmost importance in this project, and key aspects include open-sourcing the code, versioning the impact factors, and thoroughly documenting the project.
 
-The system is developed in layers according to a bottom-up principle. The first layer implemented is equipment, starting with the servers (MVP). The second layer is the measurement of the impact of digital services or systems. The measurement of the global impact is currently outside the scope.
+In the interest of transparency and scientific popularization, the opening of the code, the versioning of the impact factors and the documentation of the project are critical points. 
+
+The system follows a bottom-up approach in its development, organized into layers. The initial layer focuses on equipment. The second layer focues on the impacts of digital services (e.g. cloud instances) or systems. However, assessing the overall global impact of ICT is currently beyond the project's scope.
 
 ## :fast_forward: Test it yourself (no installation)
 
 * See our pedagogical front-end app (using the API) : <https://datavizta.boavizta.org/serversimpact>
 
 * See the OpenAPI specification: <https://api.boavizta.org/docs>
 
@@ -53,45 +62,50 @@
 
 ## :whale: Run API using docker
 
 ```bash
 $ docker run ghcr.io/boavizta/boaviztapi:latest
 ```
 
-## 📦 Install using pip package
+## Install using pip package
 
 ```bash
 $ pip3 install boaviztapi
 ```
 
+Then you can run the server locally with :
+
+```bash
+$ uvicorn boaviztapi.main:app --host=localhost --port 5000
+```
 
 ## :computer: Development
 
 ### Prerequisite
 
-Python 3, pipenv recommended
+Python 3, poetry recommended
 
-### Setup pipenv
+### Setup poetry
 
-Install pipenv globally
+Install poetry.
 
 ```bash
-$ sudo pip3 install pipenv
+$ pip3 install poetry
 ```
 
 Install dependencies and create a python virtual environment.
 
 ```bash
-$ pipenv install -d
-$ pipenv shell
+$ make install
+$ poetry shell
 ```
 
 ### Launch a development server
 
-**Once in the pipenv environment**
+**Once in the poetry environment**
 
 Development server uses [uvicorn](https://www.uvicorn.org/) and [fastapi](https://fastapi.tiangolo.com/), you can launch development server with the `uvicorn` CLI.
 
 ```bash
 $ uvicorn boaviztapi.main:app --host=localhost --port 5000
 ```
 
@@ -101,15 +115,15 @@
 
 Build application package
 ```sh
 make install
 ```
 Build docker image
 ```sh
-docker build --build-arg VERSION=0.2.0 -t boavizta/boaviztapi:0.2.0 .
+$ make docker-build
 ```
 Run docker image
 ```sh
 docker run -p 5000:5000/tcp boavizta/boaviztapi:0.2.0
 ```
 ### Deploy to AWS as serverless application
 
@@ -132,22 +146,31 @@
 Once API server is launched API swagger is available at [httsp://localhost:5000/docs](https://localhost:5000/docs).
 
 
 ## :woman: Contributing
 
 See [contributing.md](./CONTRIBUTING.md)
 
-You can build a source distribution (installable with pip) with `python setup.py sdist`.
+You can build a source distribution (installable with pip) with `make build`.
 
 ## :one: Versioning
 
 We use [Semantic Versioning 2.0.0](https://semver.org/)
 
 |    Type     | Description                                                          |    Command        |
 | :---        |    :----:                                                            |              ---: |
 | MAJOR       | version when you make incompatible API changes                       | ```make major```  |
 | MINOR       | version when you add functionality in a backwards compatible manner  | ```make minor```  |
 | PATCH       | version when you make backwards compatible bug fixes                 | ```make patch```  |
 
+## :two: Publishing
+
+You can run : 
+
+```shell
+API_TOKEN=<your_token> make distribute 
+```
+
 ## :scroll: License
 
 GNU Affero General Public License v3.0
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `boaviztapi-0.2.2/README.md` & `boaviztapi-1.0.0a0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 </p>
 <h1 align="center">
   Boavizta API
 </h1>
 
 ---
 
-An API to access [Boavizta's](https://boavizta.cmakers.io/) methodologies and footprint [reference data](https://github.com/Boavizta/environmental-footprint-data).
+An API to access [Boavizta's](https://boavizta.cmakers.io/) methodologies and impacts data [reference data](https://github.com/Boavizta/environmental-footprint-data).
 
 See the [documentation](https://doc.api.boavizta.org/) for API usage and methodology.
 
 [![Python tests](https://github.com/Boavizta/boaviztapi/actions/workflows/test.yml/badge.svg)](https://github.com/Boavizta/boaviztapi/actions/workflows/test.yml)
 
 ## :dart: Objective
 
-As part of Boavizta's desire to improve the quality of the measurement of the environmental impacts of ICTs in organizations, this project aims at giving access to the group's work to as many people as possible in an automated and industrialized way.
+Boavizta aims to enhance the assessment of environmental impacts induced by ICTs in organizations by providing widespread access to our work in an automated and efficient manner.
 
-The various data and methodologies integrated by Boavizta are aggregated and made available via an API.
+Boavizta integrates various data and methodologies, which are combined and made accessible through this API.
 
-In the interest of transparency and scientific popularization, the opening of the code, the versioning of the impact factors and the documentation of the project are critical points.
+Transparency and the popularization of scientific knowledge are of utmost importance in this project, and key aspects include open-sourcing the code, versioning the impact factors, and thoroughly documenting the project.
 
-The system is developed in layers according to a bottom-up principle. The first layer implemented is equipment, starting with the servers (MVP). The second layer is the measurement of the impact of digital services or systems. The measurement of the global impact is currently outside the scope.
+In the interest of transparency and scientific popularization, the opening of the code, the versioning of the impact factors and the documentation of the project are critical points. 
+
+The system follows a bottom-up approach in its development, organized into layers. The initial layer focuses on equipment. The second layer focues on the impacts of digital services (e.g. cloud instances) or systems. However, assessing the overall global impact of ICT is currently beyond the project's scope.
 
 ## :fast_forward: Test it yourself (no installation)
 
 * See our pedagogical front-end app (using the API) : <https://datavizta.boavizta.org/serversimpact>
 
 * See the OpenAPI specification: <https://api.boavizta.org/docs>
 
@@ -37,45 +39,50 @@
 
 ## :whale: Run API using docker
 
 ```bash
 $ docker run ghcr.io/boavizta/boaviztapi:latest
 ```
 
-## 📦 Install using pip package
+## Install using pip package
 
 ```bash
 $ pip3 install boaviztapi
 ```
 
+Then you can run the server locally with :
+
+```bash
+$ uvicorn boaviztapi.main:app --host=localhost --port 5000
+```
 
 ## :computer: Development
 
 ### Prerequisite
 
-Python 3, pipenv recommended
+Python 3, poetry recommended
 
-### Setup pipenv
+### Setup poetry
 
-Install pipenv globally
+Install poetry.
 
 ```bash
-$ sudo pip3 install pipenv
+$ pip3 install poetry
 ```
 
 Install dependencies and create a python virtual environment.
 
 ```bash
-$ pipenv install -d
-$ pipenv shell
+$ make install
+$ poetry shell
 ```
 
 ### Launch a development server
 
-**Once in the pipenv environment**
+**Once in the poetry environment**
 
 Development server uses [uvicorn](https://www.uvicorn.org/) and [fastapi](https://fastapi.tiangolo.com/), you can launch development server with the `uvicorn` CLI.
 
 ```bash
 $ uvicorn boaviztapi.main:app --host=localhost --port 5000
 ```
 
@@ -85,15 +92,15 @@
 
 Build application package
 ```sh
 make install
 ```
 Build docker image
 ```sh
-docker build --build-arg VERSION=0.2.0 -t boavizta/boaviztapi:0.2.0 .
+$ make docker-build
 ```
 Run docker image
 ```sh
 docker run -p 5000:5000/tcp boavizta/boaviztapi:0.2.0
 ```
 ### Deploy to AWS as serverless application
 
@@ -116,22 +123,30 @@
 Once API server is launched API swagger is available at [httsp://localhost:5000/docs](https://localhost:5000/docs).
 
 
 ## :woman: Contributing
 
 See [contributing.md](./CONTRIBUTING.md)
 
-You can build a source distribution (installable with pip) with `python setup.py sdist`.
+You can build a source distribution (installable with pip) with `make build`.
 
 ## :one: Versioning
 
 We use [Semantic Versioning 2.0.0](https://semver.org/)
 
 |    Type     | Description                                                          |    Command        |
 | :---        |    :----:                                                            |              ---: |
 | MAJOR       | version when you make incompatible API changes                       | ```make major```  |
 | MINOR       | version when you add functionality in a backwards compatible manner  | ```make minor```  |
 | PATCH       | version when you make backwards compatible bug fixes                 | ```make patch```  |
 
+## :two: Publishing
+
+You can run : 
+
+```shell
+API_TOKEN=<your_token> make distribute 
+```
+
 ## :scroll: License
 
 GNU Affero General Public License v3.0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `boaviztapi-0.2.2/boaviztapi/data/devices/cloud/gcp.csv` & `boaviztapi-1.0.0a0/boaviztapi/data/archetypes/cloud/gcp.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-0.2.2/boaviztapi/dto/component/other.py` & `boaviztapi-1.0.0a0/boaviztapi/dto/component/other.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 from typing import Optional
 
+from boaviztapi import config
 from boaviztapi.dto.component import ComponentDTO
-from boaviztapi.dto.usage.usage import smart_mapper_usage, Usage
-from boaviztapi.model.boattribute import Status
+from boaviztapi.dto.usage.usage import mapper_usage, Usage
 from boaviztapi.model.component import ComponentPowerSupply, ComponentMotherboard, ComponentCase
+from boaviztapi.service.archetype import get_component_archetype
 
 
 class PowerSupply(ComponentDTO):
     unit_weight: Optional[float] = None
 
 
 class Motherboard(ComponentDTO):
     pass
 
 
 class Case(ComponentDTO):
     case_type: str = None
 
 
-def mapper_power_supply(power_supply_dto: PowerSupply) -> ComponentPowerSupply:
-    power_supply_component = ComponentPowerSupply()
+def mapper_power_supply(power_supply_dto: PowerSupply, archetype=get_component_archetype(config["default_power_supply"], "power_supply")) -> ComponentPowerSupply:
+    power_supply_component = ComponentPowerSupply(archetype=archetype)
+    power_supply_component.usage = mapper_usage(power_supply_dto.usage or Usage(), archetype=archetype.get("USAGE"))
+
+    if power_supply_dto.units is not None:
+        power_supply_component.units.set_input(power_supply_dto.units)
 
-    power_supply_component.usage = smart_mapper_usage(power_supply_dto.usage or Usage())
-    power_supply_component.units = power_supply_dto.units
     if power_supply_dto.unit_weight is not None:
-        power_supply_component.unit_weight.value = power_supply_dto.unit_weight
-        power_supply_component.unit_weight.status = Status.INPUT
+        power_supply_component.unit_weight.set_input(power_supply_dto.unit_weight)
 
     return power_supply_component
 
 
 def mapper_motherboard(motherboard_dto: Motherboard) -> ComponentMotherboard:
     motherboard_component = ComponentMotherboard()
+    motherboard_component.usage = mapper_usage(motherboard_dto.usage or Usage())
 
-    motherboard_component.usage = smart_mapper_usage(motherboard_dto.usage or Usage())
-    motherboard_component.units = motherboard_dto.units
+    if motherboard_dto.units is not None:
+        motherboard_component.units.set_input(motherboard_dto.units)
 
     return motherboard_component
 
 
-def mapper_case(case_dto: Case) -> ComponentCase:
-    case_component = ComponentCase()
-    case_component.units = case_dto.units
+def mapper_case(case_dto: Case, archetype=get_component_archetype(config["default_case"], "case")) -> ComponentCase:
+    case_component = ComponentCase(archetype=archetype)
+    case_component.usage = mapper_usage(case_dto.usage or Usage(), archetype=archetype.get("USAGE"))
 
-    if case_dto.case_type is not None:
-        case_component.case_type.value = case_dto.case_type
-        case_component.case_type.status = Status.INPUT
+    if case_dto.units is not None:
+        case_component.units.set_input(case_dto.units)
 
-    case_component.usage = smart_mapper_usage(case_dto.usage or Usage())
+    if case_dto.case_type is not None:
+        case_component.case_type.set_input(case_dto.case_type)
 
     return case_component
```

### Comparing `boaviztapi-0.2.2/boaviztapi/dto/usage/usage.py` & `boaviztapi-1.0.0a0/boaviztapi/dto/usage/usage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-import os
 from typing import Optional, List, Union
 
-import pandas as pd
-
+from boaviztapi import config
 from boaviztapi.dto import BaseDTO
 from boaviztapi.model.boattribute import Status
 from boaviztapi.model.usage import ModelUsage, ModelUsageServer, ModelUsageCloud
-
-_electricity_emission_factors_df = pd.read_csv(os.path.join(os.path.dirname(__file__),
-                                                            '../../data/electricity/electricity_impact_factors.csv'))
-
+from boaviztapi.service.archetype import get_cloud_instance_archetype, get_server_archetype
+from boaviztapi.service.factor_provider import get_available_countries
 
 class WorkloadTime(BaseDTO):
     time_percentage: float = None
     load_percentage: float = None
 
+class ElecFactors(BaseDTO):
+    gwp: Optional[float] = None
+    adp: Optional[float] = None
+    pe: Optional[float] = None
+    gwppb: Optional[float] = None
+    gwppf: Optional[float] = None
+    gwpplu: Optional[float] = None
+    ir: Optional[float] = None
+    lu: Optional[float] = None
+    odp: Optional[float] = None
+    pm: Optional[float] = None
+    pocp: Optional[float] = None
+    wu: Optional[float] = None
+    mips: Optional[float] = None
+    adpe: Optional[float] = None
+    adpf: Optional[float] = None
+    ap: Optional[float] = None
+    ctue: Optional[float] = None
+    ctuh_c: Optional[float] = None
+    ctuh_nc: Optional[float] = None
+    epf: Optional[float] = None
+    epm: Optional[float] = None
+    ept: Optional[float] = None
+
 
 class Usage(BaseDTO):
-    years_use_time: Optional[float] = None
-    days_use_time: Optional[float] = None
-    hours_use_time: Optional[float] = None
+    use_time_ratio: Optional[float] = None
 
-    years_life_time: Optional[float] = None
+    hours_life_time: Optional[float] = None
 
-    hours_electrical_consumption: Optional[float] = None
+    avg_power: Optional[float] = None
     time_workload: Optional[Union[float, List[WorkloadTime]]] = None
 
     usage_location: Optional[str] = None
-    gwp_factor: Optional[float] = None
-    pe_factor: Optional[float] = None
-    adp_factor: Optional[float] = None
+    elec_factors: Optional[ElecFactors] = ElecFactors()
 
 
 class UsageServer(Usage):
     other_consumption_ratio: Optional[float] = None
 
 
 class UsageCloud(UsageServer):
     instance_per_server: Optional[int] = None
 
 
-def smart_mapper_usage(usage_dto: Usage) -> ModelUsage:
-    usage_model = ModelUsage()
+def mapper_usage(usage_dto: Usage, archetype=None) -> ModelUsage:
+    usage_model = ModelUsage(archetype=archetype)
+
+    for elec_factor in usage_dto.elec_factors.__dict__.keys():
+        if usage_dto.elec_factors.__dict__[elec_factor] is not None:
+            usage_model.elec_factors.get(elec_factor).set_input(usage_dto.elec_factors.__dict__[elec_factor])
 
     if usage_dto.time_workload is not None:
         usage_model.time_workload.value = usage_dto.time_workload
+        usage_model.time_workload.min = usage_dto.time_workload
+        usage_model.time_workload.max = usage_dto.time_workload
+
         if type(usage_dto.time_workload) == float:
             usage_model.time_workload.unit = "%"
         else:
             usage_model.time_workload.unit = "(time_percentage:%, load_percentage: %)"
-
         usage_model.time_workload.status = Status.INPUT
 
-    if usage_dto.hours_electrical_consumption is not None:
-        usage_model.hours_electrical_consumption.value = usage_dto.hours_electrical_consumption
-        usage_model.hours_electrical_consumption.status = Status.INPUT
-
-    if usage_dto.years_life_time is not None:
-        usage_model.life_time.value = usage_dto.years_life_time * 24 * 365
-        usage_model.life_time.status = Status.INPUT
-
-    if usage_dto.hours_use_time is not None or usage_dto.days_use_time is not None or usage_dto.years_use_time is not None:
-        usage_model.use_time.value = (usage_dto.hours_use_time or 0) + \
-                                     (usage_dto.days_use_time or 0) * 24 + \
-                                     (usage_dto.years_use_time or 0) * 24 * 365
+    if usage_dto.avg_power is not None:
+        usage_model.avg_power.set_input(usage_dto.avg_power)
 
-        usage_model.use_time.status = Status.INPUT
+    if usage_dto.hours_life_time is not None:
+        usage_model.hours_life_time.set_input(usage_dto.hours_life_time)
+
+    if usage_dto.use_time_ratio is not None:
+        usage_model.use_time_ratio.set_input(usage_dto.use_time_ratio)
 
     if usage_dto.usage_location is not None:
-        sub = _electricity_emission_factors_df
-        sub = sub[sub['code'] == usage_dto.usage_location]
-        if len(sub) == 0:
-            pass
+        if usage_dto.usage_location in get_available_countries(reverse=True):
+            usage_model.usage_location.set_input(usage_dto.usage_location)
         else:
+            usage_model.usage_location.set_changed(usage_model.usage_location.default)
+            usage_model.usage_location.add_warning("Location not found. Default value used.")
 
-            usage_model.usage_location.value = usage_dto.usage_location
-            usage_model.usage_location.status = Status.INPUT
     return usage_model
 
 
-def smart_mapper_usage_server(usage_dto: UsageServer) -> ModelUsageServer:
-    usage_model_server = ModelUsageServer()
+def mapper_usage_server(usage_dto: UsageServer, archetype=get_server_archetype(config["default_server"]).get("USAGE")) -> ModelUsageServer:
+    usage_model_server = ModelUsageServer(archetype=archetype)
+
+    for elec_factor in usage_dto.elec_factors.__dict__.keys():
+        if usage_dto.elec_factors.__dict__[elec_factor] is not None:
+            usage_model_server.elec_factors.get(elec_factor).set_input(usage_dto.elec_factors.__dict__[elec_factor])
+
+    if usage_dto.avg_power is not None:
+        usage_model_server.avg_power.set_input(usage_dto.avg_power)
 
-    if usage_dto.hours_electrical_consumption is not None:
-        usage_model_server.hours_electrical_consumption.value = usage_dto.hours_electrical_consumption
-        usage_model_server.hours_electrical_consumption.status = Status.INPUT
-
-    if usage_dto.years_life_time is not None:
-        usage_model_server.life_time.value = usage_dto.years_life_time * 24 * 365
-        usage_model_server.life_time.status = Status.INPUT
-
-    if usage_dto.hours_use_time is not None or usage_dto.days_use_time is not None or usage_dto.years_use_time is not None:
-        usage_model_server.use_time.value = (usage_dto.hours_use_time or 0) + \
-                                     (usage_dto.days_use_time or 0) * 24 + \
-                                     (usage_dto.years_use_time or 0) * 24 * 365
+    if usage_dto.hours_life_time is not None:
+        usage_model_server.hours_life_time.set_input(usage_dto.hours_life_time)
 
-        usage_model_server.use_time.status = Status.INPUT
+    if usage_dto.use_time_ratio is not None:
+        usage_model_server.use_time_ratio.set_input(usage_dto.use_time_ratio)
 
     if usage_dto.time_workload is not None:
-        usage_model_server.time_workload.value = usage_dto.time_workload
-        usage_model_server.time_workload.status = Status.INPUT
+        usage_model_server.time_workload.set_input(usage_dto.time_workload)
 
     if usage_dto.usage_location is not None:
-        sub = _electricity_emission_factors_df
-        sub = sub[sub['code'] == usage_dto.usage_location]
-        if len(sub) == 0:
-            pass
+        if usage_dto.usage_location in get_available_countries(reverse=True):
+            usage_model_server.usage_location.set_input(usage_dto.usage_location)
         else:
-            usage_model_server.usage_location.value = usage_dto.usage_location
-            usage_model_server.usage_location.status = Status.INPUT
-
+            usage_model_server.usage_location.set_changed(usage_model_server.usage_location.default)
+            usage_model_server.usage_location.add_warning("Location not found. Default value used.")
     if usage_dto.other_consumption_ratio is not None:
-        usage_model_server.other_consumption_ratio.value = usage_dto.other_consumption_ratio
-        usage_model_server.other_consumption_ratio.status = Status.INPUT
+        usage_model_server.other_consumption_ratio.set_input(usage_dto.other_consumption_ratio)
 
     return usage_model_server
 
 
-def smart_mapper_usage_cloud(usage_dto: UsageCloud):
-    usage_model_cloud = ModelUsageCloud()
+def mapper_usage_cloud(usage_dto: UsageCloud, archetype=get_cloud_instance_archetype(config["default_cloud"], config["default_cloud_provider"]).get("USAGE")) -> ModelUsageCloud:
+    usage_model_cloud = ModelUsageCloud(archetype=archetype)
+
+    for elec_factor in usage_dto.elec_factors.__dict__.keys():
+        if usage_dto.elec_factors.__dict__[elec_factor] is not None:
+            usage_model_cloud.elec_factors.get(elec_factor).set_input(usage_dto.elec_factors.__dict__[elec_factor])
+
+    if usage_dto.avg_power is not None:
+        usage_model_cloud.avg_power.set_input(usage_dto.avg_power)
 
-    if usage_dto.hours_electrical_consumption is not None:
-        usage_model_cloud.hours_electrical_consumption.value = usage_dto.hours_electrical_consumption
-        usage_model_cloud.hours_electrical_consumption.status = Status.INPUT
-
-    if usage_dto.years_life_time is not None:
-        usage_model_cloud.life_time.value = usage_dto.years_life_time * 24 * 365
-        usage_model_cloud.life_time.status = Status.INPUT
-
-    if usage_dto.hours_use_time is not None or usage_dto.days_use_time is not None or usage_dto.years_use_time is not None:
-        usage_model_cloud.use_time.value = (usage_dto.hours_use_time or 0) + \
-                                            (usage_dto.days_use_time or 0) * 24 + \
-                                            (usage_dto.years_use_time or 0) * 24 * 365
+    if usage_dto.hours_life_time is not None:
+        usage_model_cloud.hours_life_time.set_input(usage_dto.hours_life_time)
 
-        usage_model_cloud.use_time.status = Status.INPUT
+    if usage_dto.use_time_ratio is not None:
+        usage_model_cloud.use_time_ratio.set_input(usage_dto.use_time_ratio)
 
     if usage_dto.time_workload is not None:
-        usage_model_cloud.time_workload.value = usage_dto.time_workload
-        usage_model_cloud.time_workload.status = Status.INPUT
+        usage_model_cloud.time_workload.set_input(usage_dto.time_workload)
 
     if usage_dto.usage_location is not None:
-        sub = _electricity_emission_factors_df
-        sub = sub[sub['code'] == usage_dto.usage_location]
-        if len(sub) == 0:
-            pass
+        if usage_dto.usage_location in get_available_countries(reverse=True):
+            usage_model_cloud.usage_location.set_input(usage_dto.usage_location)
         else:
-            usage_model_cloud.usage_location.value = usage_dto.usage_location
-            usage_model_cloud.usage_location.status = Status.INPUT
+            usage_model_cloud.usage_location.set_changed(usage_model_cloud.usage_location.default)
+            usage_model_cloud.usage_location.add_warning("Location not found. Default value used.")
 
     if usage_dto.other_consumption_ratio is not None:
-        usage_model_cloud.other_consumption_ratio.value = usage_dto.other_consumption_ratio
-        usage_model_cloud.other_consumption_ratio.status = Status.INPUT
+        usage_model_cloud.other_consumption_ratio.set_input(usage_dto.other_consumption_ratio)
 
     if usage_dto.instance_per_server is not None:
-        usage_model_cloud.instance_per_server.value = usage_dto.instance_per_server
-        usage_model_cloud.instance_per_server.status = Status.INPUT
+        usage_model_cloud.instance_per_server.set_input(usage_dto.instance_per_server)
 
     return usage_model_cloud
```

### Comparing `boaviztapi-0.2.2/boaviztapi/main.py` & `boaviztapi-1.0.0a0/boaviztapi/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 import json
 
 import markdown
 from fastapi.middleware.cors import CORSMiddleware
 import os
-
+import pkg_resources
 from fastapi import FastAPI
 from fastapi.openapi.utils import get_openapi
 from mangum import Mangum
 
-from boaviztapi import __version__
-
 from boaviztapi.routers.component_router import component_router
 from boaviztapi.routers.consumption_profile_router import consumption_profile
+from boaviztapi.routers.peripheral_router import peripheral_router
 from boaviztapi.routers.server_router import server_router
 from boaviztapi.routers.cloud_router import cloud_router
+from boaviztapi.routers.terminal_router import terminal_router
 from boaviztapi.routers.utils_router import utils_router
 
 from fastapi.responses import HTMLResponse
 
 # Serverless frameworks adds a 'stage' prefix to the route used to serve applications
 # We have to manage it to expose openapi doc on aws and generate proper links.
 stage = os.environ.get('STAGE', None)
 openapi_prefix = f"/{stage}" if stage else "/"
 app = FastAPI(root_path=openapi_prefix)  # Here is the magic
+version = pkg_resources.get_distribution('boaviztapi').version
 
 origins = json.loads(os.getenv("ALLOWED_ORIGINS", '["*"]'))
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 app.include_router(server_router)
 app.include_router(cloud_router)
+app.include_router(terminal_router)
+app.include_router(peripheral_router)
 app.include_router(component_router)
 app.include_router(utils_router)
 app.include_router(consumption_profile)
 
 if __name__ == '__main__':
     import uvicorn
 
     uvicorn.run('main:app', host='localhost', port=5000, reload=True, debug=True)
 
 
 @app.on_event("startup")
 def my_schema():
-    intro = open(os.path.join(os.path.dirname(__file__), 'routers/openapi_doc/intro_openapi.md'), 'r')
+    intro = open(os.path.join(os.path.dirname(__file__), 'routers/openapi_doc/intro_openapi.md'), 'r', encoding='utf-8')
     openapi_schema = get_openapi(
         title="BOAVIZTAPI - DEMO",
-        version=__version__,
+        version=version,
         description=markdown.markdown(intro.read()),
         routes=app.routes,
         servers=app.servers,
     )
     app.openapi_schema = openapi_schema
 
     return app.openapi_schema
 
 
 # Wrapper for aws/lambda serverless app
 handler = Mangum(app)
 
 
 @app.get("/", response_class=HTMLResponse)
-async def welcom_page():
-    html_content = """
+async def welcome_page():
+    html_content = f"""
     <html>
         <head>
             <title>BOAVIZTAPI</title>
         </head>
         <body>
             <p align="center">
                 <img src="https://boavizta.org/media/site/d84925bc94-1642413712/boavizta-logo-4.png" width="100">
@@ -82,11 +85,12 @@
               Multicriteria & multistep impacts evaluations for digital assets
             </h2>
             </br>
             <h3 align="center">See our github repository : <a href="https://github.com/Boavizta/boaviztapi">LINK</a></h2>
             <h3 align="center">See OpenAPI specs (swagger) : <a href="docs">LINK</a></h2>
             <h3 align="center">See our complete documentation : <a href="https://doc.api.boavizta.org/">LINK</a></h2>
             <h3 align="center">See the other resources of Boavizta : <a href="https://boavizta.org/">LINK</a> </h2>
+            %s
         </body>
     </html>
-    """
+    """ % os.getenv('SPECIAL_MESSAGE', '')
     return HTMLResponse(content=html_content, status_code=200)
```

### Comparing `boaviztapi-0.2.2/boaviztapi/model/component/ssd.py` & `boaviztapi-1.0.0a0/boaviztapi/model/component/power_supply.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,43 @@
-from typing import Tuple
-
 import boaviztapi.utils.roundit as rd
-from boaviztapi.model.boattribute import Boattribute, Status
-from boaviztapi.model.component.component import Component, NumberSignificantFigures
-
-
-class ComponentSSD(Component):
-    NAME = "SSD"
-
-    __DISK_TYPE = 'ssd'
-
-    DEFAULT_SSD_CAPACITY = 1000
-    DEFAULT_SSD_DENSITY = 48.5
-
-    IMPACT_FACTOR = {
-        'gwp': {
-            'die_impact': 2.20,
-            'impact': 6.34
-        },
-        'pe': {
-            'die_impact': 27.30,
-            'impact': 76.90
-        },
-        'adp': {
-            'die_impact': 6.30E-05,
-            'impact': 5.63E-04
-        }
-    }
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-        self.manufacturer = Boattribute(unit="none")
-        self.capacity = Boattribute(
-            unit="GB",
-            default=self.DEFAULT_SSD_CAPACITY
-        )
-        self.density = Boattribute(
-            unit="GB/cm2",
-            default=self.DEFAULT_SSD_DENSITY
+from boaviztapi import config
+from boaviztapi.model.boattribute import Boattribute
+from boaviztapi.model.component.component import Component, ComputedImpacts
+from boaviztapi.model.impact import ImpactFactor
+from boaviztapi.service.archetype import get_component_archetype, get_arch_value
+from boaviztapi.service.factor_provider import get_impact_factor
+
+
+class ComponentPowerSupply(Component):
+    NAME = "POWER_SUPPLY"
+
+    def __init__(self, archetype=get_component_archetype(config["default_power_supply"], "power_supply"), **kwargs):
+        super().__init__(archetype=archetype, **kwargs)
+
+        self.unit_weight = Boattribute(
+            unit="kg",
+            default=get_arch_value(archetype, 'unit_weight', 'default'),
+            min=get_arch_value(archetype, 'unit_weight', 'min'),
+            max=get_arch_value(archetype, 'unit_weight', 'max')
         )
 
-    def impact_manufacture_gwp(self) -> NumberSignificantFigures:
-        return self.__impact_manufacture('gwp')
+    def impact_embedded(self, impact_type: str) -> ComputedImpacts:
+        impact_factor = ImpactFactor(
+            value=get_impact_factor(item='power_supply', impact_type=impact_type)['impact'],
+            min=get_impact_factor(item='power_supply', impact_type=impact_type)['impact'],
+            max=get_impact_factor(item='power_supply', impact_type=impact_type)['impact']
+        )
 
-    def __impact_manufacture(self, impact_type: str) -> NumberSignificantFigures:
-        ssd_die_impact, ssd_impact = self.__get_impact_constants(impact_type)
-        sign_figures = self.__compute_significant_numbers(ssd_die_impact, ssd_impact)
-        impact = self.__compute_impact_manufacture(ssd_die_impact, ssd_impact)
-        return impact, sign_figures
-
-    def __get_impact_constants(self, impact_type: str) -> Tuple[float, float]:
-        ssd_die_impact = self.IMPACT_FACTOR[impact_type]['die_impact']
-        ssd_impact = self.IMPACT_FACTOR[impact_type]['impact']
-        return ssd_die_impact, ssd_impact
-
-    def __compute_significant_numbers(self, ssd_die_impact: float, ssd_impact: float) -> int:
-        return rd.min_significant_figures(self.density.value, ssd_die_impact, ssd_impact)
+        impact = self.__compute_impact_manufacture(impact_factor)
+        sign_figures = rd.min_significant_figures(impact_factor.value)
 
-    def __compute_impact_manufacture(self, ssd_die_impact: float, ssd_impact: float) -> float:
-        return (self.capacity.value / self.density.value) * ssd_die_impact + ssd_impact
+        return impact.value, sign_figures, impact.min, impact.max, ["End of life is not included in the calculation"]
 
-    def impact_manufacture_pe(self) -> NumberSignificantFigures:
-        return self.__impact_manufacture('pe')
+    def __compute_impact_manufacture(self, power_supply_impact: ImpactFactor) -> ImpactFactor:
+        return ImpactFactor(
+            value=self.unit_weight.value * power_supply_impact.value,
+            min=self.unit_weight.min * power_supply_impact.min,
+            max=self.unit_weight.max * power_supply_impact.max
+        )
 
-    def impact_manufacture_adp(self) -> NumberSignificantFigures:
-        return self.__impact_manufacture('adp')
+    def impact_use(self, impact_type: str, duration: float) -> ComputedImpacts:
+        raise NotImplementedError
```

### Comparing `boaviztapi-0.2.2/boaviztapi/model/consumption_profile/consumption_profile.py` & `boaviztapi-1.0.0a0/boaviztapi/model/consumption_profile/consumption_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,88 +4,74 @@
 from typing import Dict, Optional, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import curve_fit
 
 import boaviztapi.utils.fuzzymatch as fuzzymatch
+from boaviztapi import config, data_dir
 from boaviztapi.dto.usage.usage import WorkloadTime
 from boaviztapi.model.boattribute import Boattribute, Status
+from boaviztapi.service.archetype import get_component_archetype, get_arch_value
 
 fuzzymatch.pandas()
 
-_cpu_profile_consumption_df = pd.read_csv(os.path.join(os.path.dirname(__file__),
-                                                       '../../data/consumption_profile/cpu/cpu_profile.csv'))
-
+_cpu_profile_consumption_df = pd.read_csv(os.path.join(data_dir, 'consumption_profile/cpu/cpu_profile.csv'))
 
 class ConsumptionProfileModel:
     def __iter__(self):
         for attr, value in self.__dict__.items():
             yield attr, value
 
 
 class RAMConsumptionProfileModel(ConsumptionProfileModel):
-    DEFAULT_RAM_CAPACITY = 15
-    DEFAULT_WORKLOADS = None
-    RAM_ELECTRICAL_FACTOR_PER_GO = 0.284
-
-    _DEFAULT_MODEL_PARAMS = {
-        'a': DEFAULT_RAM_CAPACITY * RAM_ELECTRICAL_FACTOR_PER_GO
-    }
+    ram_electrical_factor_per_go = 0.284
 
-    def __init__(self):
+    def __init__(self, archetype=get_component_archetype(config["default_ram"], "ram").get("consumption_profile")):
         self.workloads = Boattribute(
-            default=self.DEFAULT_WORKLOADS,
             unit="workload_rate:W"
         )
-        self.params = Boattribute(default=self._DEFAULT_MODEL_PARAMS)
+        self.params = Boattribute()
 
-    def compute_consumption_profile_model(self, ram_capacity: int = DEFAULT_RAM_CAPACITY) -> int:
-        self.params.value = {'a': self.RAM_ELECTRICAL_FACTOR_PER_GO * ram_capacity}
+    def compute_consumption_profile_model(self, ram_capacity) -> int:
+        self.params.value = {'a': self.ram_electrical_factor_per_go * ram_capacity}
         self.params.status = Status.COMPLETED
-        self.params.source = f"(ram_electrical_factor_per_go : {self.RAM_ELECTRICAL_FACTOR_PER_GO}) * (" \
+        self.params.source = f"(ram_electrical_factor_per_go : {self.ram_electrical_factor_per_go}) * (" \
                              f"ram_capacity: {ram_capacity}) "
         return self.params.value
 
     def apply_consumption_profile(self, load_percentage: float) -> float:
         return self.params.value['a']
 
     def apply_multiple_workloads(self, time_workload: List[WorkloadTime]) -> float:
         total = 0
         for workload in time_workload:
             total += (workload.time_percentage / 100) * self.apply_consumption_profile(workload.load_percentage)
         return total
 
 
 class CPUConsumptionProfileModel(ConsumptionProfileModel):
-    DEFAULT_CPU_MODEL_RANGE = 'Xeon Platinum'
-    DEFAULT_WORKLOADS = None
-
-    _DEFAULT_MODEL_PARAMS = {
-        'a': 171.2,
-        'b': 0.0354,
-        'c': 36.89,
-        'd': -10.13
-    }
-
     _TDP_RATIOS_WORKLOAD = [0, 10, 50, 100]
     _TDP_RATIOS = [0.12, 0.32, 0.75, 1.02]
 
     _DEFAULT_MODEL_BOUNDS = (
         [0, 0, 0, -math.inf],
         [math.inf, math.inf, math.inf, math.inf]
     )
     _MODEL_PARAM_NAME = ['a', 'b', 'c', 'd']
 
-    def __init__(self):
+    def __init__(self, archetype=get_component_archetype(config["default_cpu"], "cpu").get("CONSUMPTION_PROFILE")):
         self.workloads = Boattribute(
-            default=self.DEFAULT_WORKLOADS,
             unit="workload_rate:W"
         )
-        self.params = Boattribute(default=self._DEFAULT_MODEL_PARAMS)
+        self.params = Boattribute(
+            default=get_arch_value(archetype, 'params', 'default'),
+            min=get_arch_value(archetype, 'params', 'min'),
+            max=get_arch_value(archetype, 'params', 'max')
+        )
 
     @property
     def list_workloads(self) -> Tuple[List[float], List[float]]:
         load = [item.load_percentage for item in self.workloads.value]
         power = [item.power_watt for item in self.workloads.value]
         return load, power
 
@@ -106,30 +92,27 @@
 
     def compute_consumption_profile_model(self,
                                           cpu_manufacturer: str = None,
                                           cpu_model_range: str = None,
                                           cpu_tdp: int = None) -> Union[Dict[str, float], None]:
         model = self.lookup_consumption_profile(cpu_manufacturer, cpu_model_range)
         if self.workloads.is_set():
-            model = self.__compute_model_adaptation(base_model=model or self._DEFAULT_MODEL_PARAMS)
+            model = self.__compute_model_adaptation(base_model=model or self.params.default)
             self.params.set_completed(model, source="From workload")
 
         elif cpu_tdp is not None:
             model = self.__compute_model_adaptation_with_tdp(
-                base_model=model or self._DEFAULT_MODEL_PARAMS,
+                base_model=model or self.params.default,
                 cpu_tdp=cpu_tdp
             )
             self.params.set_completed(model, source="From TDP")
 
         elif cpu_model_range is not None:
             self.params.set_completed(model, source="From CPU model range")
 
-        else:
-            self.params.set_default(self._DEFAULT_MODEL_PARAMS)
-
         return self.params.value
 
     def __compute_model_adaptation_with_tdp(self, base_model: Dict[str, float], cpu_tdp: float) -> Dict[str, float]:
         @dataclasses.dataclass
         class _TDPWorkloadPower:
             load_percentage: float = None
             power_watt: float = None
```

### Comparing `boaviztapi-0.2.2/boaviztapi/model/device/device.py` & `boaviztapi-1.0.0a0/boaviztapi/model/device/device.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from abc import abstractmethod
 from typing import Tuple, List
 
+from boaviztapi.model.boattribute import Boattribute
 from boaviztapi.model.component import Component
 from boaviztapi.model.usage import ModelUsage
 
-NumberSignificantFigures = Tuple[float, int]
+ComputedImpacts = Tuple[float, int]
 
 
 class Device:
 
-    def __init__(self, **kwargs):
+    def __init__(self, archetype=None, **kwargs):
+        self.impact_factor = {}
+        self.archetype = archetype
+        self.units = Boattribute(
+            default=1,
+            min=1,
+            max=1
+        )
         self._usage = None
         pass
 
     @property
     def usage(self) -> ModelUsage:
         return self._usage
 
@@ -22,34 +30,18 @@
         self._usage = value
 
     @property
     def components(self) -> List[Component]:
         return []
 
     @abstractmethod
-    def impact_manufacture_gwp(self) -> NumberSignificantFigures:
+    def impact_embedded(self, impact_type: str) -> ComputedImpacts:
         raise NotImplementedError
 
     @abstractmethod
-    def impact_manufacture_pe(self) -> NumberSignificantFigures:
-        raise NotImplementedError
-
-    @abstractmethod
-    def impact_manufacture_adp(self) -> NumberSignificantFigures:
-        raise NotImplementedError
-
-    @abstractmethod
-    def impact_use_gwp(self) -> NumberSignificantFigures:
-        raise NotImplementedError
-
-    @abstractmethod
-    def impact_use_pe(self) -> NumberSignificantFigures:
-        raise NotImplementedError
-
-    @abstractmethod
-    def impact_use_adp(self) -> NumberSignificantFigures:
+    def  impact_use(self, impact_type: str, duration: float) -> ComputedImpacts:
         raise NotImplementedError
 
     def __iter__(self):
         for attr, value in self.__dict__.items():
             yield attr, value
```

### Comparing `boaviztapi-0.2.2/boaviztapi/model/device/server.py` & `boaviztapi-1.0.0a0/boaviztapi/model/device/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-import copy
 from abc import ABC
 from typing import List, Union
 
-from boaviztapi.model.boattribute import Status
+from boaviztapi import config
+from boaviztapi.model import ComputedImpacts
 from boaviztapi.model.component import Component, ComponentCPU, ComponentRAM, ComponentSSD, ComponentHDD, \
     ComponentPowerSupply, ComponentCase, ComponentMotherboard, ComponentAssembly
-from boaviztapi.model.device.device import Device, NumberSignificantFigures
+from boaviztapi.model.device.device import Device
+from boaviztapi.model.impact import ImpactFactor
 from boaviztapi.model.usage import ModelUsageServer, ModelUsageCloud
 import boaviztapi.utils.roundit as rd
+from boaviztapi.service.archetype import get_server_archetype, get_arch_component, get_cloud_instance_archetype
+from boaviztapi.service.factor_provider import get_impact_factor
 
 
 class DeviceServer(Device):
-    DEFAULT_COMPONENT_CPU = ComponentCPU()
-    DEFAULT_NUMBER_CPU = 2
-
-    DEFAULT_COMPONENT_RAM = ComponentRAM()
-    DEFAULT_NUMBER_RAM = 24
-
-    DEFAULT_COMPONENT_DISK = ComponentSSD()
-    DEFAULT_NUMBER_DISK = 1
-
-    DEFAULT_COMPONENT_POWER_SUPPLY = ComponentPowerSupply()
-    DEFAULT_NUMBER_POWER_SUPPLY = 2
-
-    DEFAULT_COMPONENT_CASE = ComponentCase()
-    DEFAULT_COMPONENT_MOTHERBOARD = ComponentMotherboard()
-    DEFAULT_COMPONENT_ASSEMBLY = ComponentAssembly()
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    NAME = "SERVER"
+    def __init__(self, archetype=get_server_archetype(config["default_server"]), **kwargs):
+        super().__init__(archetype=archetype, **kwargs)
         self._cpu = None
         self._ram_list = None
         self._disk_list = None
         self._power_supply = None
         self._case = None
         self._motherboard = None
         self._assembly = None
@@ -41,59 +29,55 @@
         for attr, val in kwargs.items():
             if val is not None:
                 self.__setattr__(attr, val)
 
     @property
     def cpu(self) -> ComponentCPU:
         if self._cpu is None:
-            self._cpu = copy.deepcopy(self.DEFAULT_COMPONENT_CPU)
-            self._cpu.units = self.DEFAULT_NUMBER_CPU
+            self._cpu = ComponentCPU(archetype=get_arch_component(self.archetype,"CPU"))
         return self._cpu
 
     @cpu.setter
     def cpu(self, value: List[ComponentCPU]) -> None:
         self._cpu = value
 
     @property
     def ram(self) -> List[ComponentRAM]:
         if self._ram_list is None:
-            self.DEFAULT_COMPONENT_RAM.units = copy.deepcopy(self.DEFAULT_NUMBER_RAM)
-            self._ram_list = [self.DEFAULT_COMPONENT_RAM]
+            self._ram_list = [ComponentRAM(archetype=get_arch_component(self.archetype,"RAM"))]
         return self._ram_list
 
     @ram.setter
     def ram(self, value: List[ComponentRAM]) -> None:
         self._ram_list = value
 
     @property
     def disk(self) -> List[Union[ComponentSSD, ComponentHDD]]:
         if self._disk_list is None:
-            self.DEFAULT_COMPONENT_DISK.units = self.DEFAULT_NUMBER_DISK
-            self._disk_list = [copy.deepcopy(self.DEFAULT_COMPONENT_DISK)]
+            self._disk_list = [ComponentSSD(archetype=get_arch_component(self.archetype,"SSD"))]
         return self._disk_list
 
     @disk.setter
     def disk(self, value: List[Union[ComponentSSD, ComponentHDD]]) -> None:
         self._disk_list = value
 
     @property
     def power_supply(self) -> ComponentPowerSupply:
         if self._power_supply is None:
-            self._power_supply = copy.deepcopy(self.DEFAULT_COMPONENT_POWER_SUPPLY)
-            self._power_supply.units = self.DEFAULT_NUMBER_POWER_SUPPLY
+            self._power_supply = ComponentPowerSupply(archetype=get_arch_component(self.archetype,"POWER_SUPPLY"))
         return self._power_supply
 
     @power_supply.setter
     def power_supply(self, value: List[ComponentPowerSupply]) -> None:
         self._power_supply = value
 
     @property
     def case(self) -> ComponentCase:
         if self._case is None:
-            self._case = copy.deepcopy(self.DEFAULT_COMPONENT_CASE)
+            self._case = ComponentCase(archetype=get_arch_component(self.archetype,"CASE"))
         return self._case
 
     @case.setter
     def case(self, value: ComponentCase) -> None:
         self._case = value
 
     @property
@@ -103,125 +87,134 @@
     @case_type.setter
     def case_type(self, value: str) -> None:
         self.case.case_type = value
 
     @property
     def motherboard(self) -> ComponentMotherboard:
         if self._motherboard is None:
-            self._motherboard = copy.deepcopy(self.DEFAULT_COMPONENT_MOTHERBOARD)
+            self._motherboard = ComponentMotherboard(archetype=get_arch_component(self.archetype,"MOTHERBOARD"))
         return self._motherboard
 
     @motherboard.setter
     def motherboard(self, value: ComponentMotherboard) -> None:
         self._motherboard = value
 
     @property
     def assembly(self) -> ComponentAssembly:
         if self._assembly is None:
-            self._assembly = copy.deepcopy(self.DEFAULT_COMPONENT_ASSEMBLY)
+            self._assembly = ComponentAssembly(archetype=get_arch_component(self.archetype,"ASSEMBLY"))
         return self._assembly
 
     @assembly.setter
     def assembly(self, value: ComponentAssembly) -> None:
         self._assembly = value
 
     @property
     def usage(self) -> ModelUsageServer:
         if self._usage is None:
-            self._usage = ModelUsageServer()
+            self._usage = ModelUsageServer(archetype=get_arch_component(self.archetype,"USAGE"))
         return self._usage
 
     @usage.setter
     def usage(self, value: ModelUsageServer) -> None:
         self._usage = value
 
     @property
     def components(self) -> List[Component]:
         return [self.assembly] + [self.cpu] + self.ram + self.disk + [self.power_supply] + [self.case] + [
             self.motherboard]
 
-    def __impact_manufacture(self, impact_type: str) -> NumberSignificantFigures:
+    def impact_embedded(self, impact_type: str) -> ComputedImpacts:
         impacts = []
+        min_impacts = []
+        max_impacts = []
         significant_figures = []
-        for component in self.components:
-            impact, sign_fig = getattr(component, f'impact_manufacture_{impact_type}')()
-            impacts.append(impact*component.units)
-            significant_figures.append(sign_fig)
-        return sum(impacts), min(significant_figures)
-
-    def __impact_usage(self, impact_type: str) -> NumberSignificantFigures:
-        impact_factor = getattr(self.usage, f'{impact_type}_factor')
-        if not self.usage.hours_electrical_consumption.is_set():
-            self.usage.hours_electrical_consumption.value = self.model_power_consumption()
-            self.usage.hours_electrical_consumption.status = Status.COMPLETED
+        warnings = []
+
+        try:
+            for component in self.components:
+                impact, sign_fig, min_impact, max_impact, c_warning = getattr(component, f'impact_embedded')(impact_type)
+
+                impacts.append(impact*component.units.value)
+                min_impacts.append(min_impact*component.units.min)
+                max_impacts.append(max_impact*component.units.max)
+
+                significant_figures.append(sign_fig)
+                warnings = warnings + c_warning
+            return sum(impacts), min(significant_figures), sum(min_impacts), sum(max_impacts), warnings
+
+        except NotImplementedError:
+            impact = get_impact_factor(item='SERVER', impact_type=impact_type)["impact"]
+            min_impacts = get_impact_factor(item='SERVER', impact_type=impact_type)["impact"]
+            max_impacts = get_impact_factor(item='SERVER', impact_type=impact_type)["impact"]
+            significant_figures = rd.significant_number(impact)
+
+            warnings = ["Generic data used for impact calculation."]
+
+            return impact, significant_figures, min_impacts, max_impacts, warnings
+
+    def impact_use(self, impact_type: str, duration: float) -> ComputedImpacts:
+        impact_factor = self.usage.elec_factors[impact_type]
+
+        if not self.usage.avg_power.is_set():
+            modeled_consumption = self.model_power_consumption()
+            self.usage.avg_power.set_completed(
+                modeled_consumption.value,
+                min=modeled_consumption.min,
+                max=modeled_consumption.max
+            )
+
+        impact = impact_factor.value * (self.usage.avg_power.value / 1000) * self.usage.use_time_ratio.value * duration
+        min_impact = impact_factor.min * (self.usage.avg_power.min / 1000) * self.usage.use_time_ratio.min * duration
+        max_impact = impact_factor.max * (self.usage.avg_power.max / 1000) * self.usage.use_time_ratio.max * duration
 
-        impacts = impact_factor.value * (self.usage.hours_electrical_consumption.value / 1000) * self.usage.use_time.value
         sig_fig = self.__compute_significant_numbers(impact_factor.value)
-        return impacts, sig_fig
+        return impact, sig_fig, min_impact, max_impact, []
 
     def model_power_consumption(self):
-        conso_cpu = self.cpu.model_power_consumption()*self.cpu.units
-        conso_ram = 0
+        conso_cpu = ImpactFactor(
+            value=self.cpu.model_power_consumption().value*self.cpu.units.value,
+            min=self.cpu.model_power_consumption().min*self.cpu.units.min,
+            max=self.cpu.model_power_consumption().max * self.cpu.units.max,
+        )
+        conso_ram = ImpactFactor(
+            value=0,
+            min=0,
+            max=0
+        )
         for ram_unit in self.ram:
-            conso_ram += ram_unit.model_power_consumption()*ram_unit.units
-        return (conso_cpu + conso_ram) * (1 + self.usage.other_consumption_ratio.value)
+            conso_ram.value = conso_ram.value + ram_unit.model_power_consumption().value * ram_unit.units.value
+            conso_ram.min = conso_ram.min + ram_unit.model_power_consumption().min * ram_unit.units.min
+            conso_ram.max = conso_ram.max + ram_unit.model_power_consumption().max * ram_unit.units.max
+
+        return ImpactFactor(
+                value=(conso_cpu.value + conso_ram.value) * (1 + self.usage.other_consumption_ratio.value),
+                min=(conso_cpu.min + conso_ram.min) * (1 + self.usage.other_consumption_ratio.min),
+                max=(conso_cpu.max + conso_ram.max) * (1 + self.usage.other_consumption_ratio.max)
+        )
 
     def __compute_significant_numbers(self, impact_factor: float) -> int:
-        return rd.min_significant_figures(self.usage.hours_electrical_consumption.value, self.usage.use_time.value, impact_factor)
-
-    def impact_manufacture_gwp(self) -> NumberSignificantFigures:
-        return self.__impact_manufacture('gwp')
-
-    def impact_manufacture_pe(self) -> NumberSignificantFigures:
-        return self.__impact_manufacture('pe')
-
-    def impact_manufacture_adp(self) -> NumberSignificantFigures:
-        return self.__impact_manufacture('adp')
-
-    def impact_use_gwp(self) -> NumberSignificantFigures:
-        return self.__impact_usage('gwp')
-
-    def impact_use_pe(self) -> NumberSignificantFigures:
-        return self.__impact_usage('pe')
-
-    def impact_use_adp(self) -> NumberSignificantFigures:
-        return self.__impact_usage('adp')
+        return rd.min_significant_figures(self.usage.avg_power.value, impact_factor)
 
 
 class DeviceCloudInstance(DeviceServer, ABC):
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, archetype=get_cloud_instance_archetype(config["default_cloud"], config["default_cloud_provider"]), **kwargs):
+        super().__init__(**kwargs, archetype=archetype)
 
     @property
     def usage(self) -> ModelUsageCloud:
         if self._usage is None:
-            self._usage = ModelUsageCloud()
+            self._usage = ModelUsageCloud(archetype=get_arch_component(self.archetype,"USAGE"))
         return self._usage
 
     @usage.setter
     def usage(self, value: ModelUsageCloud) -> None:
         self._usage = value
 
-    def impact_manufacture_gwp(self) -> NumberSignificantFigures:
-        impact, sign_fig = super().impact_manufacture_gwp()
-        return (impact / self.usage.instance_per_server.value), sign_fig
-
-    def impact_manufacture_pe(self) -> NumberSignificantFigures:
-        impact, sign_fig = super().impact_manufacture_pe()
-        return (impact / self.usage.instance_per_server.value), sign_fig
-
-    def impact_manufacture_adp(self) -> NumberSignificantFigures:
-        impact, sign_fig = super().impact_manufacture_adp()
-        return (impact / self.usage.instance_per_server.value), sign_fig
-
-    def impact_use_gwp(self) -> NumberSignificantFigures:
-        impact, sign_fig = super().impact_use_gwp()
-        return (impact / self.usage.instance_per_server.value), sign_fig
-
-    def impact_use_pe(self) -> NumberSignificantFigures:
-        impact, sign_fig = super().impact_use_pe()
-        return (impact / self.usage.instance_per_server.value), sign_fig
-
-    def impact_use_adp(self) -> NumberSignificantFigures:
-        impact, sign_fig = super().impact_use_adp()
-        return (impact / self.usage.instance_per_server.value), sign_fig
+    def impact_embedded(self, impact_type: str) -> ComputedImpacts:
+        impact, sign_fig, min_impact, max_impact, c_warning = super().impact_embedded(impact_type)
+        return (impact / self.usage.instance_per_server.value), sign_fig, min_impact, max_impact, c_warning
+
+    def impact_use(self, impact_type: str, duration: int) -> ComputedImpacts:
+        impact, sign_fig, min_impact, max_impact, c_warning = super().impact_use(impact_type, duration)
+        return (impact / self.usage.instance_per_server.value), sign_fig, min_impact, max_impact, c_warning
```

### Comparing `boaviztapi-0.2.2/boaviztapi/routers/consumption_profile_router.py` & `boaviztapi-1.0.0a0/boaviztapi/routers/consumption_profile_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-0.2.2/boaviztapi/routers/openapi_doc/descriptions.py` & `boaviztapi-1.0.0a0/boaviztapi/routers/openapi_doc/descriptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,152 +1,168 @@
 server_impact_by_model_description = "# ✔ ️Server impacts from model name\n" \
-                                     "Retrieve the impacts of a given server name (archetype).\n" \
+                                     "Retrieve the impacts of a given server archetype.\n" \
                                      "### Features\n\n" \
                                      "👄 Verbose\n\n" \
                                      "🔃 Auto-complete\n\n" \
-                                     "🔨 Manufacture\n\n" \
+                                     "🔨 Embedded\n\n" \
                                      "🔌 Usage\n\n" \
                                      "📋 Archetype: " \
-                                     "Uses the [classic server impacts router]with a pre-registered archetype \n\n" \
+                                     "Uses the classic server impacts router with a pre-registered archetype \n\n" \
                                      "⏬ Allocation"
 
 server_impact_by_config_description = "# ✔️ Server impacts from configuration\n" \
                                       "Retrieve the impacts of a given server configuration.\n" \
                                       "### Features\n\n" \
                                       "👄 Verbose\n\n" \
                                       "🔃 Auto-complete\n\n" \
-                                      "🔨 Manufacture\n\n" \
+                                      "🔨 Embedded\n\n" \
                                       "🔌 Usage\n\n" \
                                       "* ⏺️  Given\n\n" \
                                       "* 📈 Modeled\n\n" \
                                       "📋 Archetype\n\n" \
                                       "⏬ Allocation"
 
-all_default_model_description = "# ✔️ Get all the available server models\n" \
-                                "📜 Return the name of all pre-registered server models"
+all_archetype_servers = "# ✔️ Get all the available server archetype\n"
+all_archetype_components = "# ✔️ Get all the available component archetype for a given component name\n"
+all_archetype_user_terminals = "# ✔️ Get all the available user terminal archetype for a given user terminal name\n"
+all_terminal_categories = "# ✔️ Get all the available user terminal router\n"
+all_peripheral_categories = "# ✔️ Get all the available user peripheral router\n"
+all_user_terminal_subcategories = "# ✔️ Get all the available user terminal subcategories\n"
+all_default_usage_values = "# ✔️ Get all default usage values for a given user terminal category and subcategory\n"
+
+get_archetype_config_desc = "# ✔️ Get the configuration of a given archetype\n"
+get_instance_config = "# ✔️ Get the configuration of a given instance\n"
 
 cpu_description = "# ✔ ️CPU impacts from configuration\n" \
                   "### Features\n\n" \
                   "👄 Verbose\n\n" \
                   "🔃 Auto-complete\n\n" \
-                  "🔨 Manufacture\n\n" \
+                  "🔨 Embedded\n\n" \
                   "<h3>cpu<sub>manuf<sub><em>criteria</em></sub></sub> = ( " \
                   "cpu<sub>core<sub>units</sub></sub> x cpu<sub>diesize</sub> + 0," \
                   "491 ) x cpu<sub>manuf_die<sub><em>criteria</em></sub></sub> + " \
                   "cpu<sub>manuf_base<sub><em>criteria</em></sub></sub></h3> " \
                   "🔌 Usage\n\n" \
                   "* ⏺️  Given\n\n" \
                   "* 📈 Modeled\n\n" \
                   "⏬ Allocation"
 
 ssd_description = "# ✔ ️SSD impacts from configuration\n" \
                   "### Features\n\n" \
                   "👄 Verbose\n\n" \
                   "🔃 Auto-complete\n\n" \
-                  "🔨 Manufacture\n\n" \
+                  "🔨 Embedded\n\n" \
                   "<h3>ssd<sub>manuf<sub><em>criteria</em></sub></sub> =  ( ssd<sub>size</sub> " \
                   "ssd<sub>density</sub> ) x ssd<sub>manuf_die<sub><em>criteria</em></sub></sub> + " \
                   "ssd<sub>manuf_base<sub><em>criteria</em></sub></sub></h3>" \
                   "🔌 Usage\n\n" \
                   "* ⏺️  Given\n\n" \
                   "⏬ Allocation"
 
 hdd_description = "# ✔ ️HDD impacts from configuration\n" \
                   "### Features\n\n" \
                   "👄 Verbose\n\n" \
                   "🔃 Auto-complete\n\n" \
-                  "🔨 Manufacture\n\n" \
+                  "🔨 Embedded\n\n" \
                   "The impacts values are set by default" \
                   "🔌 Usage\n\n" \
                   "* ⏺️  Given\n\n" \
                   "⏬ Allocation"
 
 ram_description = "# ✔️ RAM impacts from configuration\n" \
                   "### Features\n\n" \
                   "👄 Verbose\n\n" \
                   "🔃 Auto-complete\n\n" \
-                  "🔨 Manufacture\n\n" \
+                  "🔨 Embedded\n\n" \
                   "<h3>ram<sub>manuf<sub><em>criteria</em></sub></sub> =( ram<sub>size</sub> " \
                   "/ ram<sub>density</sub> ) x ram<sub>manuf_die<sub><em>criteria</em></sub></sub> + " \
                   "ram<sub>manuf_base<sub><em>criteria</em></sub></sub> </h3> " \
                   "🔌 Usage\n\n" \
                   "* ⏺️  Given\n\n" \
                   "* 📈 Modeled\n\n" \
                   "⏬ Allocation"
 
 motherboard_description = "# ✔ ️Motherboard impacts from configuration\n" \
                           "### Features\n\n" \
                           "👄 Verbose\n\n" \
                           "🔃 Auto-complete\n\n" \
-                          "🔨 Manufacture\n\n" \
+                          "🔨 Embedded\n\n" \
                           "The impacts values are set by default" \
                           "🔌 Usage\n\n" \
                           "* ⏺️  Given\n\n" \
                           "⏬ Allocation"
 
 power_supply_description = "# ✔ ️Power supply impacts from configuration\n" + \
                            "### Features\n\n" \
                            "👄 Verbose\n\n" \
                            "🔃 Auto-complete\n\n" \
-                           "🔨 Manufacture\n\n" \
+                           "🔨 Embedded\n\n" \
                            "<h3>psu<sub>manuf<sub><em>criteria</em></sub></sub> = psu<sub>unit<sub>weight</sub></sub>" \
                            " x psu<sub>manuf_weight<sub><em>criteria</em></sub></sub></h3> " \
                            "🔌 Usage\n\n" \
                            "* ⏺️  Given : shouldn't be used\n\n" \
                            "⏬ Allocation"
 
 case_description = "# ✔ ️Case impacts from configuration\n" \
                    "### Features\n\n" \
                    "👄 Verbose\n\n" \
                    "🔃 Auto-complete\n\n" \
-                   "🔨 Manufacture\n\n" \
-                   "<h3>psu<sub>manuf<sub><em>criteria</em></sub></sub> = psu<sub>unit<sub>weight</sub></sub>" \
-                   " x psu<sub>manuf_weight<sub><em>criteria</em></sub></sub></h3> " \
+                   "🔨 Embedded\n\n" \
                    "🔌 Usage\n\n" \
                    "* ⏺️  Given : when the enclosure consumes energy \n\n" \
                    "⏬ Allocation"
 
 cloud_provider_description = "# ✔ ️Cloud instance impacts from provider, instance type and usage \n" \
-                        "Retrieve the impacts of a given Cloud instance and usage.\n\n" \
-                        "### Features\n\n" \
-                        "📋 Provider \n\n" \
-                        "Name of the cloud provider. You can retrieve the [list here](" \
-                        "#/cloud_instance/server_get_all_cloud_providers).\n\n" \
-                        "📋 Instance type \n\n" \
-                        "Name of the chosen instance. You can retrieve the [list here](" \
-                        "#/cloud/server_get_archetype_name_v1_cloud_all_aws_instances_get).\n\n" \
-                        "👄 Verbose\n\n" \
-                        "🔨 Manufacture\n\n" \
-                        "🔌 Usage \n\n" \
-                        "* 📈 Modeled\n\n" \
-                        "📋 Archetype : The configuration is set by the API, only usage is given by the user\n\n" \
-                        "⏬ Allocation"
-
-cloud_aws_description = "# ✔ (LEGACY) ️AWS instance impacts from instance type and usage \n" \
-                        "Retrieve the impacts of a given AWS instance and usage.\n\n" \
-                        "### Features\n\n" \
-                        "📋 Instance type \n\n" \
-                        "AWS name of the chosen instance. You can retrieve the [list here](" \
-                        "#/cloud/server_get_all_archetype_name_v1_cloud_all_aws_instances_get).\n\n" \
-                        "👄 Verbose\n\n" \
-                        "🔨 Manufacture\n\n" \
-                        "🔌 Usage \n\n" \
-                        "* 📈 Modeled\n\n" \
-                        "📋 Archetype : The configuration is set by the API, only usage is given by the user\n\n" \
-                        "⏬ Allocation"
-
-all_default_aws_instances = "# ✔ (LEGACY)️ Get all the available aws instances\n" \
-                            "📜 Return the name of all pre-registered aws instances"
-            
+                             "Retrieve the impacts of a given Cloud instance and usage.\n\n" \
+                             "### Features\n\n" \
+                             "📋 Provider \n\n" \
+                             "Name of the cloud provider. You can retrieve the [list here](" \
+                             "#/cloud_instance/server_get_all_cloud_providers).\n\n" \
+                             "📋 Instance type \n\n" \
+                             "Name of the chosen instance. You can retrieve the [list here](" \
+                             "#/cloud/server_get_archetype_name_v1_cloud_all_aws_instances_get).\n\n" \
+                             "👄 Verbose\n\n" \
+                             "🔨 Embedded\n\n" \
+                             "🔌 Usage \n\n" \
+                             "* 📈 Modeled\n\n" \
+                             "📋 Archetype : The configuration is set by the API, only usage is given by the user\n\n" \
+                             "⏬ Allocation"
+
 all_default_cloud_instances = "# ✔ ️Get all the available instances for a given Cloud provider\n" \
-                            "📜 Return the name of all pre-registered instances for the Cloud provider"
+                              "📜 Return the name of all pre-registered instances for the Cloud provider"
 
 all_default_cloud_providers = "# ✔ ️Get all the available Cloud providers\n" \
-                            "📜 Return the names of all pre-registered Cloud providers"
+                              "📜 Return the names of all pre-registered Cloud providers"
 
 country_code = "# ✔ ️Get all the available countries with their trigram code (*usage:{usage_location: 'FRA'}*)\n"
 cpu_family = "# ✔ ️Get all the available cpu family in the API (*cpu:{family:'skylake'}*)\n"
 cpu_model_range = "# ✔ ️Get all the available cpu family in the API (*cpu:{model_range:'xeon platinum'}*)\n"
 ssd_manufacturer = "# ✔ ️Get all the available ssd manufacturer in the API (*ssd:{manufacturer:'samsung'}*)\n"
 ram_manufacturer = "# ✔ ️Get all the available ram manufacturer in the API (*ram:{manufacturer:'samsung'}*)\n"
 case_type = "# ✔ ️Get all the available case type in the API (*model:{case:'blade'}*)\n"
 name_to_cpu = "# ✔ ️Complete a cpu attributes from a cpu name\n"
+cpu_names = "# ✔ ️Get all the available cpu name in the API (*cpu:{name:'intel xeon platinum 8175m'}*)\n"
+impacts_criteria = "# ✔ ️Get all the available criteria for the impacts calculation\n"
+
+
+terminal_description = "# ✔ Terminal impacts\n" \
+                          "### Features\n\n" \
+                          "👄 Verbose\n\n" \
+                          "🔃 Auto-complete\n\n" \
+                          "🔨 Embedded\n\n" \
+                          "The impacts values are fix" \
+                          "🔌 Usage\n\n" \
+                          "* ⏺️  Given\n\n" \
+                          "* 📋 Archetype\n\n" \
+                          "⏬ Allocation"
+
+
+peripheral_description = "# ✔ Peripheral impacts\n" \
+                          "### Features\n\n" \
+                          "👄 Verbose\n\n" \
+                          "🔃 Auto-complete\n\n" \
+                          "🔨 Embedded\n\n" \
+                          "The impacts values are fix" \
+                          "🔌 Usage\n\n" \
+                          "* ⏺️  Given\n\n" \
+                          "* 📋 Archetype\n\n" \
+                          "⏬ Allocation"
```

### Comparing `boaviztapi-0.2.2/boaviztapi/routers/openapi_doc/examples.py` & `boaviztapi-1.0.0a0/boaviztapi/routers/openapi_doc/examples.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,18 +26,15 @@
                             "type": "ssd",
                             "capacity": 400,
                             "density": 50.6
                         }
                     ]
             },
         "usage": {
-            "years_use_time": 1,
-            "days_use_time": 1,
-            "hours_use_time": 1,
-            "hours_electrical_consumption": 300,
+            "avg_power": 300,
             "usage_location": "FRA"
         }
     }}
 
 components_examples = {
     "cpu": {
         "name": "intel xeon gold 6134",
@@ -56,29 +53,27 @@
     "power_supply": {
         "unit_weight": 10
     },
     "case": {"case_type": "rack"},
 }
 
 cloud_usage_example = {
-        "hours_use_time": 2,
         "usage_location": "FRA",
         "time_workload": [
             {"time_percentage": 50, "load_percentage": 0},
             {"time_percentage": 25, "load_percentage": 60},
             {"time_percentage": 25, "load_percentage": 100}
         ]
 }
 
 cloud_example = {
     "provider": "aws",
     "instance_type": "a1.4xlarge",
     "usage":
             {
-            "hours_use_time": 2,
             "usage_location": "FRA",
             "time_workload": [
                 {"time_percentage": 50, "load_percentage": 0},
                 {"time_percentage": 25, "load_percentage": 60},
                 {"time_percentage": 25, "load_percentage": 100}
             ]}
 }
@@ -100,8 +95,15 @@
                 "power_watt": 180
             },
             {
                 "load_percentage": 100,
                 "power_watt": 245
             }
         ],
+}
+
+end_user_terminal = {
+    "usage": {
+        "use_time_ratio": 0.3,
+        "usage_location": "FRA",
+    }
 }
```

### Comparing `boaviztapi-0.2.2/boaviztapi/routers/openapi_doc/intro_openapi.md` & `boaviztapi-1.0.0a0/boaviztapi/routers/openapi_doc/intro_openapi.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 🎯 Retrieving the impacts of digital elements.
 
 This is a quick demo, to see full documentation [click here](https://doc.api.boavizta.org)
 
 ## Features
 
-Bellow a list of all available features. Implemented features are specified in each route.
+Bellow a list of all available features.
 
 ### 👄 Verbose
 
 Verbose is an HTTP parameter. If set at true :
 
 * Shows the impacts of each component
-* Shows the value used for each attributes
+* Shows the value used for each attribute
 
-*"attribute": {"value": "value", "unit": "unit", "status": "Status", "source": "Source"}*
+*"attribute": {"value": "value", "unit": "unit", "status": "Status", "source": "Source", "min":"min", "max":"max", "significant_figures":"significant_figures"}*
 
-### 🔨 Manufacture
+### 🔨 Embedded
  
-* Manufacture impacts of devices are the sum of the impacts of its components
-* Manufacture impacts equations of components are given for each component
+* Embedded impacts are the impacts occurring during raw material extraction, manufacture, distribution and end of life
+* When end of life is not taken into account, we specified it in the ```warnings```
 
 ### 🔌  Usage
 
-Usage impacts are measured by multiplying :
+Usage impacts are assessed by multiplying :
 
  * a **duration**
 
  * an **impact factor** 
 
  * an **electrical consumption** 
 
 #### ⏲ Duration
 
-Usage impacts are given for a specific time duration. Duration can be given in :
+Usage impacts can be given as a router parameter, in hours.
 
-* HOURS : *usage:{hours_use_time: 1}*
-* DAYS : *usage:{days_use_time: 1}*
-* YEARS : *usage:{years_use_time: 1}* 
+If no duration is given, **the impact is assess for the all life duration of the asset**.
 
-If no duration is given, **the impact is measured for a year**.
-
-*Note* : units are cumulative
 
 #### ✖️ Impact factors
 
-* Impact factors can be given : *usage:{[criterion]_factors: 0.38}*
-* Impact factors can be retrieved from : *usage:{usage_location: "FRA"}*. 
+* Impact factors can be given : *"usage":{"elec_factors":{[criterion]_factors: 0.38}}*
+* Impact factors can be retrieved from : *"usage":{"usage_location": "FRA"}*. 
 
-*See the list of locations : [/v1/utils/country_code](/v1/utils/country_code)*
+* See the list of locations : [/v1/utils/country_code](/v1/utils/country_code)*
 
 #### ⚡ Electrical consumption
 
 ##### ⏺️ Given
-* Electrical consumption can be given for one hour (average) *usage:{hours_electrical_consumption: 1}*.
+* Electrical consumption can be given for one hour (average) *"usage":{"avg_power": 1}*.
 
 ##### 📈 Modeled
-* Electrical consumption can be retrieved from consumption profile using *usage:{time_workload: 50}*. 
+* Electrical consumption can be retrieved from consumption profile using *usage:{time_workload: 50}*.
 
-### 🔃 Auto-complete
+##### 📋 Archetype
 
-The API will complete the missing attributes in a request. Components have different completion strategies.
-Devices have minimal required components. If not given in the request a component with default characteristics is used.
+* In some cases, default electrical consumption can be taken from the archetype
 
-### 📋 Archetype
+### 🔃 Auto-complete & 📋 Archetype
 
-If an archetype is given, the missing attributes will be complete with the archetypes attributes instead of default attributes
+The API will complete the missing attributes in a request with a completion function or with values
+taken from the ```archetype``` specified in the route parameter.
 
 ### ⏬ Allocation
 
-Allocation is an HTTP parameter. 
+* Usage impacts are assessed on the duration given in route parameter
+* Embedded impacts are allocated linearly on the duration given in parameter
+```embedded_impact = impact * (duration/life_duration)```
 
-* If set at TOTAL, the total manufacture impact is returned.
-* If set at LINEAR the manufacture impact is allocated linearly hover a specific lifespan given or set by default : *{"usage":{"years_life_time":1}}*
+If no duration is given, the life_duration (```hours_life_time``) of the asset is used.
```

### Comparing `boaviztapi-0.2.2/boaviztapi/routers/utils_router.py` & `boaviztapi-1.0.0a0/boaviztapi/routers/utils_router.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import os
+import os
 
 import pandas as pd
-from fastapi import APIRouter
+from fastapi import APIRouter, Query
 
-from boaviztapi.dto.component.cpu import attributes_from_cpu_name, CPU
-from boaviztapi.model.component import ComponentCase, ComponentCPU
+from boaviztapi.dto.component.cpu import CPU
+from boaviztapi.model import impact
+from boaviztapi.model.component import ComponentCase
+from boaviztapi.model.component.cpu import attributes_from_cpu_name
 from boaviztapi.routers.openapi_doc.descriptions import country_code, cpu_family, cpu_model_range, ssd_manufacturer, \
-    ram_manufacturer, case_type, name_to_cpu
+    ram_manufacturer, case_type, name_to_cpu, cpu_names, impacts_criteria
+from boaviztapi.service.factor_provider import get_available_countries
 
 utils_router = APIRouter(
     prefix='/v1/utils',
     tags=['utils']
 )
 
 data_dir = os.path.join(os.path.dirname(__file__), '../data')
-_countries_df = pd.read_csv(os.path.join(data_dir, 'electricity/electricity_impact_factors.csv'))
-_cpu_index = pd.read_csv(os.path.join(data_dir, 'components/cpu_index.csv'))
-_cpu_manuf = pd.read_csv(os.path.join(data_dir, 'components/cpu_manufacture.csv'))
-_ssd_manuf = pd.read_csv(os.path.join(data_dir, 'components/ssd_manufacture.csv'))
-_ram_manuf = pd.read_csv(os.path.join(data_dir, 'components/ram_manufacture.csv'))
+_cpu_specs = pd.read_csv(os.path.join(data_dir, 'crowdsourcing/cpu_specs.csv'))
+_cpu_manuf = pd.read_csv(os.path.join(data_dir, 'crowdsourcing/cpu_manufacture.csv'))
+_ssd_manuf = pd.read_csv(os.path.join(data_dir, 'crowdsourcing/ssd_manufacture.csv'))
+_ram_manuf = pd.read_csv(os.path.join(data_dir, 'crowdsourcing/ram_manufacture.csv'))
 
 
 @utils_router.get('/country_code', description=country_code)
 async def utils_get_all_countries():
-    res = {}
-    for ind in _countries_df.index:
-        res[_countries_df["country"][ind]] = _countries_df["code"][ind]
-
-    return res
+    return get_available_countries()
 
 
 @utils_router.get('/cpu_family', description=cpu_family)
 async def utils_get_all_cpu_family():
     df = _cpu_manuf[_cpu_manuf["family"].notna()]
     return [*df["family"].unique()]
 
 
 @utils_router.get('/cpu_model_range', description=cpu_model_range)
 async def utils_get_all_cpu_model_range():
-    df = _cpu_index[_cpu_index["model_range"].notna()]
+    df = _cpu_specs[_cpu_specs["model_range"].notna()]
     return [*df["model_range"].unique()]
 
 
 @utils_router.get('/ssd_manufacturer', description=ssd_manufacturer)
 async def utils_get_all_ssd_manufacturer():
     df = _ssd_manuf[_ssd_manuf["manufacturer"].notna()]
 
@@ -58,11 +57,19 @@
 
 @utils_router.get('/case_type', description=case_type)
 async def utils_get_all_case_type():
     return ComponentCase.AVAILABLE_CASE_TYPE
 
 
 @utils_router.get('/name_to_cpu', description=name_to_cpu)
-async def name_to_cpu(cpu_name: str = None):
-    manufacturer, model_range, family = attributes_from_cpu_name(cpu_name)
-    cpu = CPU(manufacturer=manufacturer, model_range=model_range, family=family)
-    return cpu
+async def name_to_cpu(cpu_name: str = Query(example="Intel Core i7-9700K")):
+    name, manufacturer, code_name, model_range, tdp, cores, total_die_size, total_die_size_source, source  = attributes_from_cpu_name(cpu_name)
+    return CPU(family=code_name, name=name, tdp=tdp, core_units=cores, die_size=total_die_size, model_range=model_range, manufacturer=manufacturer)
+
+@utils_router.get('/cpu_name', description=cpu_names)
+async def utils_get_all_cpu_name():
+    df = _cpu_specs[_cpu_specs["name"].notna()]
+    return [*df["name"].unique()]
+
+@utils_router.get('/impact_criteria', description=impacts_criteria)
+async def utils_get_all_impacts_criteria():
+    return impact.IMPACT_CRITERIAS
```

### Comparing `boaviztapi-0.2.2/boaviztapi/utils/roundit.py` & `boaviztapi-1.0.0a0/boaviztapi/utils/roundit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import math
 from decimal import Decimal
 
+from boaviztapi import config
+
 DEFAULT_SIG_FIGURES = 3
 
 
 def significant_number(x):
     """
     Determine the number of significant figures for x
     """
@@ -21,15 +23,15 @@
     Returns the minimum of significant figures for a tuple of values
     """
     sigfig = significant_number(inputs[0])
     for input in inputs:
         p = significant_number(input)
         if (p <= sigfig):
             sigfig = p
-    return sigfig
+    return sigfig if sigfig > config['min_significant_figures'] else config['min_significant_figures']
 
 
 def round_to_sigfig(x, significant_figures):
     """
    returns a float rounded to significant figures
    """
     return float(to_precision(x, significant_figures))
```

