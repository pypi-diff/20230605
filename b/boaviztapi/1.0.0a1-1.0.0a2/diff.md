# Comparing `tmp/boaviztapi-1.0.0a1.tar.gz` & `tmp/boaviztapi-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boaviztapi-1.0.0a1.tar", max compression
+gzip compressed data, was "boaviztapi-1.0.0a2.tar", max compression
```

## Comparing `boaviztapi-1.0.0a1.tar` & `boaviztapi-1.0.0a2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    34523 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/LICENSE
--rw-r--r--   0        0        0     4494 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/README.md
--rw-r--r--   0        0        0      365 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/__init__.py
--rw-r--r--   0        0        0   114581 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/cloud/aws.csv
--rw-r--r--   0        0        0      559 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/cloud/gcp.csv
--rw-r--r--   0        0        0       58 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/cloud/providers.csv
--rw-r--r--   0        0        0      116 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/components/case.csv
--rw-r--r--   0        0        0      268 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/components/cpu.csv
--rw-r--r--   0        0        0       95 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/components/hdd.csv
--rw-r--r--   0        0        0       97 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/components/power_supply.csv
--rw-r--r--   0        0        0      162 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/components/ram.csv
--rw-r--r--   0        0        0      130 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/components/ssd.csv
--rw-r--r--   0        0        0     1242 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/server.csv
--rw-r--r--   0        0        0      921 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/archetypes/user_terminal.csv
--rw-r--r--   0        0        0      819 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/config.yml
--rw-r--r--   0        0        0      314 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/consumption_profile/cpu/cpu_profile.csv
--rw-r--r--   0        0        0     3404 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/ademe_base_impacts_negaoctet.csv
--rw-r--r--   0        0        0     4553 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/cpu_manufacture.csv
--rw-r--r--   0        0        0   515038 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/cpu_specs.csv
--rw-r--r--   0        0        0    26045 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/electrical_mix.csv
--rw-r--r--   0        0        0      113 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/missing_cpu_manufacture.csv
--rw-r--r--   0        0        0      214 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/ram_manufacture.csv
--rw-r--r--   0        0        0     2274 2023-06-05 09:39:11.414964 boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/ssd_manufacture.csv
--rw-r--r--   0        0        0   425401 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/data/factors.yml
--rw-r--r--   0        0        0     2259 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/data/utils/jsonifyer.py
--rw-r--r--   0        0        0       30 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/__init__.py
--rw-r--r--   0        0        0      123 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/base_dto.py
--rw-r--r--   0        0        0      154 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/component/__init__.py
--rw-r--r--   0        0        0      205 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/component/component_dto.py
--rw-r--r--   0        0        0     2199 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/component/cpu.py
--rw-r--r--   0        0        0     1814 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/component/disk.py
--rw-r--r--   0        0        0     1994 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/component/other.py
--rw-r--r--   0        0        0     1440 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/component/ram.py
--rw-r--r--   0        0        0       55 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/consumption_profile/__init__.py
--rw-r--r--   0        0        0     1633 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/consumption_profile/consumption_profile.py
--rw-r--r--   0        0        0       45 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/device/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/device/device.py
--rw-r--r--   0        0        0     2629 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/device/user_terminal.py
--rw-r--r--   0        0        0       50 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/usage/__init__.py
--rw-r--r--   0        0        0     6577 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/dto/usage/usage.py
--rw-r--r--   0        0        0     3329 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/main.py
--rw-r--r--   0        0        0      143 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/__init__.py
--rw-r--r--   0        0        0     3866 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/boattribute.py
--rw-r--r--   0        0        0      318 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/__init__.py
--rw-r--r--   0        0        0     1106 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/assembly.py
--rw-r--r--   0        0        0     5052 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/case.py
--rw-r--r--   0        0        0     2150 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/component.py
--rw-r--r--   0        0        0    14232 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/cpu.py
--rw-r--r--   0        0        0     1460 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/hdd.py
--rw-r--r--   0        0        0      941 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/motherboard.py
--rw-r--r--   0        0        0     2004 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/power_supply.py
--rw-r--r--   0        0        0     7197 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/ram.py
--rw-r--r--   0        0        0     4960 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/component/ssd.py
--rw-r--r--   0        0        0       88 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/consumption_profile/__init__.py
--rw-r--r--   0        0        0     7244 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/consumption_profile/consumption_profile.py
--rw-r--r--   0        0        0       81 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/device/__init__.py
--rw-r--r--   0        0        0     1134 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/device/device.py
--rw-r--r--   0        0        0     8965 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/device/server.py
--rw-r--r--   0        0        0     7261 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/device/userTerminal.py
--rw-r--r--   0        0        0     3983 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/impact.py
--rw-r--r--   0        0        0       65 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/usage/__init__.py
--rw-r--r--   0        0        0     8503 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/model/usage/usage.py
--rw-r--r--   0        0        0        0 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/__init__.py
--rw-r--r--   0        0        0     4052 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/cloud_router.py
--rw-r--r--   0        0        0    17594 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/component_router.py
--rw-r--r--   0        0        0      958 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/consumption_profile_router.py
--rw-r--r--   0        0        0        0 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/openapi_doc/__init__.py
--rw-r--r--   0        0        0     9638 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/openapi_doc/descriptions.py
--rw-r--r--   0        0        0     2624 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/openapi_doc/examples.py
--rw-r--r--   0        0        0     2207 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/openapi_doc/intro_openapi.md
--rw-r--r--   0        0        0     8625 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/peripheral_router.py
--rw-r--r--   0        0        0     3612 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/server_router.py
--rw-r--r--   0        0        0    13529 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/terminal_router.py
--rw-r--r--   0        0        0     2864 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/routers/utils_router.py
--rw-r--r--   0        0        0        0 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/service/__init__.py
--rw-r--r--   0        0        0      602 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/service/allocation.py
--rw-r--r--   0        0        0     4276 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/service/archetype.py
--rw-r--r--   0        0        0     2199 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/service/bottom_up.py
--rw-r--r--   0        0        0     3280 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/service/factor_provider.py
--rw-r--r--   0        0        0     2646 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/service/verbose.py
--rw-r--r--   0        0        0        0 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/utils/__init__.py
--rw-r--r--   0        0        0     1405 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/utils/fuzzymatch.py
--rw-r--r--   0        0        0     3257 2023-06-05 09:39:11.418964 boaviztapi-1.0.0a1/boaviztapi/utils/roundit.py
--rw-r--r--   0        0        0      695 2023-06-05 09:39:11.438964 boaviztapi-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 boaviztapi-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0     4494 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/README.md
+-rw-r--r--   0        0        0      365 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/__init__.py
+-rw-r--r--   0        0        0   114581 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/cloud/aws.csv
+-rw-r--r--   0        0        0      559 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/cloud/gcp.csv
+-rw-r--r--   0        0        0       58 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/cloud/providers.csv
+-rw-r--r--   0        0        0      116 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/components/case.csv
+-rw-r--r--   0        0        0      268 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/components/cpu.csv
+-rw-r--r--   0        0        0       95 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/components/hdd.csv
+-rw-r--r--   0        0        0       97 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/components/power_supply.csv
+-rw-r--r--   0        0        0      162 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/components/ram.csv
+-rw-r--r--   0        0        0      130 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/components/ssd.csv
+-rw-r--r--   0        0        0     1242 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/server.csv
+-rw-r--r--   0        0        0      921 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/archetypes/user_terminal.csv
+-rw-r--r--   0        0        0      819 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/config.yml
+-rw-r--r--   0        0        0      314 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/consumption_profile/cpu/cpu_profile.csv
+-rw-r--r--   0        0        0     3404 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/ademe_base_impacts_negaoctet.csv
+-rw-r--r--   0        0        0     4553 2023-06-05 09:47:21.722076 boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/cpu_manufacture.csv
+-rw-r--r--   0        0        0   515038 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/cpu_specs.csv
+-rw-r--r--   0        0        0    26045 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/electrical_mix.csv
+-rw-r--r--   0        0        0      113 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/missing_cpu_manufacture.csv
+-rw-r--r--   0        0        0      214 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/ram_manufacture.csv
+-rw-r--r--   0        0        0     2274 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/ssd_manufacture.csv
+-rw-r--r--   0        0        0   425401 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/data/factors.yml
+-rw-r--r--   0        0        0     2259 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/data/utils/jsonifyer.py
+-rw-r--r--   0        0        0       30 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/__init__.py
+-rw-r--r--   0        0        0      123 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/base_dto.py
+-rw-r--r--   0        0        0      154 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/component/__init__.py
+-rw-r--r--   0        0        0      205 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/component/component_dto.py
+-rw-r--r--   0        0        0     2199 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/component/cpu.py
+-rw-r--r--   0        0        0     1814 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/component/disk.py
+-rw-r--r--   0        0        0     1994 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/component/other.py
+-rw-r--r--   0        0        0     1440 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/component/ram.py
+-rw-r--r--   0        0        0       55 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/consumption_profile/__init__.py
+-rw-r--r--   0        0        0     1633 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/consumption_profile/consumption_profile.py
+-rw-r--r--   0        0        0       45 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/device/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/device/device.py
+-rw-r--r--   0        0        0     2629 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/device/user_terminal.py
+-rw-r--r--   0        0        0       50 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/usage/__init__.py
+-rw-r--r--   0        0        0     6577 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/dto/usage/usage.py
+-rw-r--r--   0        0        0     3329 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/main.py
+-rw-r--r--   0        0        0      143 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/__init__.py
+-rw-r--r--   0        0        0     3866 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/boattribute.py
+-rw-r--r--   0        0        0      318 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/__init__.py
+-rw-r--r--   0        0        0     1106 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/assembly.py
+-rw-r--r--   0        0        0     5052 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/case.py
+-rw-r--r--   0        0        0     2150 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/component.py
+-rw-r--r--   0        0        0    14232 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/cpu.py
+-rw-r--r--   0        0        0     1460 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/hdd.py
+-rw-r--r--   0        0        0      941 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/motherboard.py
+-rw-r--r--   0        0        0     2004 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/power_supply.py
+-rw-r--r--   0        0        0     7197 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/ram.py
+-rw-r--r--   0        0        0     4960 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/component/ssd.py
+-rw-r--r--   0        0        0       88 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/consumption_profile/__init__.py
+-rw-r--r--   0        0        0     7244 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/consumption_profile/consumption_profile.py
+-rw-r--r--   0        0        0       81 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/device/__init__.py
+-rw-r--r--   0        0        0     1134 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/device/device.py
+-rw-r--r--   0        0        0     8965 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/device/server.py
+-rw-r--r--   0        0        0     7261 2023-06-05 09:47:21.726076 boaviztapi-1.0.0a2/boaviztapi/model/device/userTerminal.py
+-rw-r--r--   0        0        0     3983 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/model/impact.py
+-rw-r--r--   0        0        0       65 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/model/usage/__init__.py
+-rw-r--r--   0        0        0     8503 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/model/usage/usage.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/__init__.py
+-rw-r--r--   0        0        0     4052 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/cloud_router.py
+-rw-r--r--   0        0        0    17594 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/component_router.py
+-rw-r--r--   0        0        0      958 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/consumption_profile_router.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/openapi_doc/__init__.py
+-rw-r--r--   0        0        0     9638 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/openapi_doc/descriptions.py
+-rw-r--r--   0        0        0     2624 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/openapi_doc/examples.py
+-rw-r--r--   0        0        0     2207 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/openapi_doc/intro_openapi.md
+-rw-r--r--   0        0        0     8625 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/peripheral_router.py
+-rw-r--r--   0        0        0     3612 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/server_router.py
+-rw-r--r--   0        0        0    13529 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/terminal_router.py
+-rw-r--r--   0        0        0     2864 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/routers/utils_router.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/service/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/service/allocation.py
+-rw-r--r--   0        0        0     4276 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/service/archetype.py
+-rw-r--r--   0        0        0     2199 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/service/bottom_up.py
+-rw-r--r--   0        0        0     3280 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/service/factor_provider.py
+-rw-r--r--   0        0        0     2646 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/service/verbose.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/utils/__init__.py
+-rw-r--r--   0        0        0     1405 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/utils/fuzzymatch.py
+-rw-r--r--   0        0        0     3257 2023-06-05 09:47:21.730076 boaviztapi-1.0.0a2/boaviztapi/utils/roundit.py
+-rw-r--r--   0        0        0      695 2023-06-05 09:47:21.746077 boaviztapi-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 boaviztapi-1.0.0a2/PKG-INFO
```

### Comparing `boaviztapi-1.0.0a1/LICENSE` & `boaviztapi-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/README.md` & `boaviztapi-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/archetypes/cloud/aws.csv` & `boaviztapi-1.0.0a2/boaviztapi/data/archetypes/cloud/aws.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/archetypes/cloud/gcp.csv` & `boaviztapi-1.0.0a2/boaviztapi/data/archetypes/cloud/gcp.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/archetypes/server.csv` & `boaviztapi-1.0.0a2/boaviztapi/data/archetypes/server.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/archetypes/user_terminal.csv` & `boaviztapi-1.0.0a2/boaviztapi/data/archetypes/user_terminal.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/config.yml` & `boaviztapi-1.0.0a2/boaviztapi/data/config.yml`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/ademe_base_impacts_negaoctet.csv` & `boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/ademe_base_impacts_negaoctet.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/cpu_manufacture.csv` & `boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/cpu_manufacture.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/cpu_specs.csv` & `boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/cpu_specs.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/electrical_mix.csv` & `boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/electrical_mix.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/crowdsourcing/ssd_manufacture.csv` & `boaviztapi-1.0.0a2/boaviztapi/data/crowdsourcing/ssd_manufacture.csv`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/factors.yml` & `boaviztapi-1.0.0a2/boaviztapi/data/factors.yml`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/data/utils/jsonifyer.py` & `boaviztapi-1.0.0a2/boaviztapi/data/utils/jsonifyer.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/dto/component/cpu.py` & `boaviztapi-1.0.0a2/boaviztapi/dto/component/cpu.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/dto/component/disk.py` & `boaviztapi-1.0.0a2/boaviztapi/dto/component/disk.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/dto/component/other.py` & `boaviztapi-1.0.0a2/boaviztapi/dto/component/other.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/dto/component/ram.py` & `boaviztapi-1.0.0a2/boaviztapi/dto/component/ram.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/dto/consumption_profile/consumption_profile.py` & `boaviztapi-1.0.0a2/boaviztapi/dto/consumption_profile/consumption_profile.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/dto/device/device.py` & `boaviztapi-1.0.0a2/boaviztapi/dto/device/device.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/dto/device/user_terminal.py` & `boaviztapi-1.0.0a2/boaviztapi/dto/device/user_terminal.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/dto/usage/usage.py` & `boaviztapi-1.0.0a2/boaviztapi/dto/usage/usage.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/main.py` & `boaviztapi-1.0.0a2/boaviztapi/main.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/boattribute.py` & `boaviztapi-1.0.0a2/boaviztapi/model/boattribute.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/component/assembly.py` & `boaviztapi-1.0.0a2/boaviztapi/model/component/assembly.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/component/case.py` & `boaviztapi-1.0.0a2/boaviztapi/model/component/case.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/component/component.py` & `boaviztapi-1.0.0a2/boaviztapi/model/component/component.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/component/cpu.py` & `boaviztapi-1.0.0a2/boaviztapi/model/component/cpu.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/component/hdd.py` & `boaviztapi-1.0.0a2/boaviztapi/model/component/hdd.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/component/motherboard.py` & `boaviztapi-1.0.0a2/boaviztapi/model/component/motherboard.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/component/power_supply.py` & `boaviztapi-1.0.0a2/boaviztapi/model/component/power_supply.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/component/ram.py` & `boaviztapi-1.0.0a2/boaviztapi/model/component/ram.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/component/ssd.py` & `boaviztapi-1.0.0a2/boaviztapi/model/component/ssd.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/consumption_profile/consumption_profile.py` & `boaviztapi-1.0.0a2/boaviztapi/model/consumption_profile/consumption_profile.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/device/device.py` & `boaviztapi-1.0.0a2/boaviztapi/model/device/device.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/device/server.py` & `boaviztapi-1.0.0a2/boaviztapi/model/device/server.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/device/userTerminal.py` & `boaviztapi-1.0.0a2/boaviztapi/model/device/userTerminal.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/impact.py` & `boaviztapi-1.0.0a2/boaviztapi/model/impact.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/model/usage/usage.py` & `boaviztapi-1.0.0a2/boaviztapi/model/usage/usage.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/cloud_router.py` & `boaviztapi-1.0.0a2/boaviztapi/routers/cloud_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/component_router.py` & `boaviztapi-1.0.0a2/boaviztapi/routers/component_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/consumption_profile_router.py` & `boaviztapi-1.0.0a2/boaviztapi/routers/consumption_profile_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/openapi_doc/descriptions.py` & `boaviztapi-1.0.0a2/boaviztapi/routers/openapi_doc/descriptions.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/openapi_doc/examples.py` & `boaviztapi-1.0.0a2/boaviztapi/routers/openapi_doc/examples.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/openapi_doc/intro_openapi.md` & `boaviztapi-1.0.0a2/boaviztapi/routers/openapi_doc/intro_openapi.md`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/peripheral_router.py` & `boaviztapi-1.0.0a2/boaviztapi/routers/peripheral_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/server_router.py` & `boaviztapi-1.0.0a2/boaviztapi/routers/server_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/terminal_router.py` & `boaviztapi-1.0.0a2/boaviztapi/routers/terminal_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/routers/utils_router.py` & `boaviztapi-1.0.0a2/boaviztapi/routers/utils_router.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/service/allocation.py` & `boaviztapi-1.0.0a2/boaviztapi/service/allocation.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/service/archetype.py` & `boaviztapi-1.0.0a2/boaviztapi/service/archetype.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/service/bottom_up.py` & `boaviztapi-1.0.0a2/boaviztapi/service/bottom_up.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/service/factor_provider.py` & `boaviztapi-1.0.0a2/boaviztapi/service/factor_provider.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/service/verbose.py` & `boaviztapi-1.0.0a2/boaviztapi/service/verbose.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/utils/fuzzymatch.py` & `boaviztapi-1.0.0a2/boaviztapi/utils/fuzzymatch.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/boaviztapi/utils/roundit.py` & `boaviztapi-1.0.0a2/boaviztapi/utils/roundit.py`

 * *Files identical despite different names*

### Comparing `boaviztapi-1.0.0a1/pyproject.toml` & `boaviztapi-1.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boaviztapi"
-version = "1.0.0a1"
+version = "1.0.0a2"
 description = "An API to access Boavizta's methodologies and footprint reference data"
 authors = []
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = '^1.10'
```

### Comparing `boaviztapi-1.0.0a1/PKG-INFO` & `boaviztapi-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boaviztapi
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: An API to access Boavizta's methodologies and footprint reference data
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

