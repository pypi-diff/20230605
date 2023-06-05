# Comparing `tmp/codecarbon-2.2.2.tar.gz` & `tmp/codecarbon-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecarbon-2.2.2.tar", last modified: Thu May 25 09:25:54 2023, max compression
+gzip compressed data, was "codecarbon-2.2.3.tar", last modified: Mon Jun  5 05:26:02 2023, max compression
```

## Comparing `codecarbon-2.2.2.tar` & `codecarbon-2.2.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.938085 codecarbon-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 09:25:41.000000 codecarbon-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-25 09:25:54.938085 codecarbon-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-25 09:25:41.000000 codecarbon-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.926085 codecarbon-2.2.2/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.926085 codecarbon-2.2.2/carbonserver/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.926085 codecarbon-2.2.2/carbonserver/carbonserver/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/carbonserver/carbonserver/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/codecarbon/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/codecarbon/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/rapl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.926085 codecarbon-2.2.2/codecarbon/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/data/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/cloud/impact.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/data/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)    49423 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/hardware/cpu_power.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/data/private_infra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/data/private_infra/2016/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0 runner    (1001) docker     (123)   124501 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)    37361 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/emissions_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/geography.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/viz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.938085 codecarbon-2.2.2/codecarbon/viz/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/carbonboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/codecarbon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:25:54.938085 codecarbon-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-25 09:25:41.000000 codecarbon-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.938085 codecarbon-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_api_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_core_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_emissions_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_emissions_tracker_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_emissions_tracker_flush.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_geography.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_logging_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_ram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.112112 codecarbon-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-05 05:25:49.000000 codecarbon-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-05 05:26:02.112112 codecarbon-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-05 05:25:49.000000 codecarbon-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.100112 codecarbon-2.2.3/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/domain/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/carbonserver/carbonserver/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/carbonserver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-05 05:25:49.000000 codecarbon-2.2.3/carbonserver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.104112 codecarbon-2.2.3/codecarbon/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/rapl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.100112 codecarbon-2.2.3/codecarbon/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/data/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/cloud/impact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/data/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    49423 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/hardware/cpu_power.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/data/private_infra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/data/private_infra/2016/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)   124501 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38065 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/emissions_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/external/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.112112 codecarbon-2.2.3/codecarbon/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.112112 codecarbon-2.2.3/codecarbon/viz/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/carbonboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-06-05 05:25:49.000000 codecarbon-2.2.3/codecarbon/viz/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.108112 codecarbon-2.2.3/codecarbon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 05:26:02.000000 codecarbon-2.2.3/codecarbon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 05:26:02.112112 codecarbon-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-05 05:25:49.000000 codecarbon-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:26:02.112112 codecarbon-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_core_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_emissions_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_emissions_tracker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_emissions_tracker_flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_logging_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/test_ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-05 05:25:49.000000 codecarbon-2.2.3/tests/testutils.py
```

### Comparing `codecarbon-2.2.2/LICENSE` & `codecarbon-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/PKG-INFO` & `codecarbon-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.2
+Version: 2.2.3
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.2/README.md` & `codecarbon-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/dependencies.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/domain/experiments.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/domain/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/errors.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/errors.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/authenticate.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/authenticate.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/emissions.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/experiments.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/organizations.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/organizations.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/projects.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/projects.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/runs.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/runs.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/teams.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/teams.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/users.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/api/schemas.py` & `codecarbon-2.2.3/carbonserver/carbonserver/api/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/carbonserver/database/database.py` & `codecarbon-2.2.3/carbonserver/carbonserver/database/database.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/container.py` & `codecarbon-2.2.3/carbonserver/container.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/main.py` & `codecarbon-2.2.3/carbonserver/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/carbonserver/setup.py` & `codecarbon-2.2.3/carbonserver/setup.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/cli/cli_utils.py` & `codecarbon-2.2.3/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/cli/main.py` & `codecarbon-2.2.3/codecarbon/cli/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/api_client.py` & `codecarbon-2.2.3/codecarbon/core/api_client.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/cloud.py` & `codecarbon-2.2.3/codecarbon/core/cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/co2_signal.py` & `codecarbon-2.2.3/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/config.py` & `codecarbon-2.2.3/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/cpu.py` & `codecarbon-2.2.3/codecarbon/core/cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/emissions.py` & `codecarbon-2.2.3/codecarbon/core/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/gpu.py` & `codecarbon-2.2.3/codecarbon/core/gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/rapl.py` & `codecarbon-2.2.3/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/schemas.py` & `codecarbon-2.2.3/codecarbon/core/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/core/units.py` & `codecarbon-2.2.3/codecarbon/core/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 
     def __sub__(self, other: "Energy") -> "Energy":
         return Energy(self.kWh - other.kWh)
 
     def __add__(self, other: "Energy") -> "Energy":
         return Energy(self.kWh + other.kWh)
 
+    def __mul__(self, factor: float) -> "Energy":
+        return Energy(self.kWh * factor)
+
     def __float__(self) -> float:
         return float(self.kWh)
 
 
 @dataclass
 class Power:
     """
```

### Comparing `codecarbon-2.2.2/codecarbon/core/util.py` & `codecarbon-2.2.3/codecarbon/core/util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/data/cloud/impact.csv` & `codecarbon-2.2.3/codecarbon/data/cloud/impact.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/data/hardware/cpu_power.csv` & `codecarbon-2.2.3/codecarbon/data/hardware/cpu_power.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.2.3/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.2.3/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.2.3/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/data/private_infra/global_energy_mix.json` & `codecarbon-2.2.3/codecarbon/data/private_infra/global_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/emissions_tracker.py` & `codecarbon-2.2.3/codecarbon/emissions_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         experiment_id: Optional[str] = _sentinel,
         co2_signal_api_token: Optional[str] = _sentinel,
         tracking_mode: Optional[str] = _sentinel,
         log_level: Optional[Union[int, str]] = _sentinel,
         on_csv_write: Optional[str] = _sentinel,
         logger_preamble: Optional[str] = _sentinel,
         default_cpu_power: Optional[int] = _sentinel,
+        pue: Optional[int] = _sentinel,
     ):
         """
         :param project_name: Project name for current experiment run, default name
                              is "codecarbon".
         :param measure_power_secs: Interval (in seconds) to measure hardware power
                                    usage, defaults to 15.
         :param api_call_interval: Occurrence to wait before calling API :
@@ -193,15 +194,16 @@
                           Defaults to "info".
         :param on_csv_write: "append" or "update". Whether to always append a new line
                              to the csv when writing or to update the existing `run_id`
                              row (useful when calling`tracker.flush()` manually).
                              Accepts one of "append" or "update". Default is "append".
         :param logger_preamble: String to systematically include in the logger.
                                 messages. Defaults to "".
-        :param default_cpu_power: cpu power to be used as default if the cpu is not known
+        :param default_cpu_power: cpu power to be used as default if the cpu is not known.
+        :param pue: PUE (Power Usage Effectiveness) of the datacenter.
         """
 
         # logger.info("base tracker init")
         self._external_conf = get_hierarchical_config()
 
         self._set_from_conf(api_call_interval, "api_call_interval", 8, int)
         self._set_from_conf(api_endpoint, "api_endpoint", "https://api.codecarbon.io")
@@ -217,14 +219,15 @@
         self._set_from_conf(save_to_file, "save_to_file", True, bool)
         self._set_from_conf(save_to_logger, "save_to_logger", False, bool)
         self._set_from_conf(logging_logger, "logging_logger")
         self._set_from_conf(tracking_mode, "tracking_mode", "machine")
         self._set_from_conf(on_csv_write, "on_csv_write", "append")
         self._set_from_conf(logger_preamble, "logger_preamble", "")
         self._set_from_conf(default_cpu_power, "default_cpu_power")
+        self._set_from_conf(pue, "pue", 1.0, float)
 
         assert self._tracking_mode in ["machine", "process"]
         set_logger_level(self._log_level)
         set_logger_format(self._logger_preamble)
 
         self._start_time: Optional[float] = None
         self._last_measured_time: float = time.time()
@@ -498,14 +501,15 @@
             gpu_model=self._conf.get("gpu_model"),
             cpu_count=self._conf.get("cpu_count"),
             cpu_model=self._conf.get("cpu_model"),
             longitude=self._conf.get("longitude"),
             latitude=self._conf.get("latitude"),
             ram_total_size=self._conf.get("ram_total_size"),
             tracking_mode=self._conf.get("tracking_mode"),
+            pue=self._pue,
         )
         if delta:
             if self._previous_emissions is None:
                 self._previous_emissions = total_emissions
             else:
                 # Create a copy
                 delta_emissions = dataclasses.replace(total_emissions)
@@ -551,14 +555,16 @@
         for hardware in self._hardware:
             h_time = time.time()
             # Compute last_duration again for more accuracy
             last_duration = time.time() - self._last_measured_time
             power, energy = hardware.measure_power_and_energy(
                 last_duration=last_duration
             )
+            # Apply the PUE of the datacenter to the consumed energy
+            energy *= self._pue
             self._total_energy += energy
             if isinstance(hardware, CPU):
                 self._total_cpu_energy += energy
                 self._cpu_power = power
                 logger.info(
                     f"Energy consumed for all CPUs : {self._total_cpu_energy.kWh:.6f} kWh"
                     + f". Total CPU Power : {self._cpu_power.W} W"
@@ -747,14 +753,16 @@
     country_iso_code: Optional[str] = _sentinel,
     region: Optional[str] = _sentinel,
     cloud_provider: Optional[str] = _sentinel,
     cloud_region: Optional[str] = _sentinel,
     gpu_ids: Optional[List] = _sentinel,
     co2_signal_api_token: Optional[str] = _sentinel,
     log_level: Optional[Union[int, str]] = _sentinel,
+    default_cpu_power: Optional[int] = _sentinel,
+    pue: Optional[int] = _sentinel,
 ):
     """
     Decorator that supports both `EmissionsTracker` and `OfflineEmissionsTracker`
     :param fn: Function to be decorated
     :param project_name: Project name for current experiment run,
                          default name is "codecarbon".
     :param measure_power_secs: Interval (in seconds) to measure hardware power usage,
@@ -785,14 +793,16 @@
                          See https://github.com/mlco2/codecarbon/
                                             blob/master/codecarbon/data/cloud/impact.csv
                          for a list of cloud regions.
     :param gpu_ids: User-specified known gpu ids to track, defaults to None
     :param log_level: Global codecarbon log level. Accepts one of:
                         {"debug", "info", "warning", "error", "critical"}.
                       Defaults to "info".
+    :param default_cpu_power: cpu power to be used as default if the cpu is not known.
+    :param pue: PUE (Power Usage Effectiveness) of the datacenter.
 
     :return: The decorated function
     """
 
     def _decorate(fn: Callable):
         @wraps(fn)
         def wrapped_fn(*args, **kwargs):
@@ -813,14 +823,16 @@
                     country_iso_code=country_iso_code,
                     region=region,
                     cloud_provider=cloud_provider,
                     cloud_region=cloud_region,
                     gpu_ids=gpu_ids,
                     log_level=log_level,
                     co2_signal_api_token=co2_signal_api_token,
+                    default_cpu_power=default_cpu_power,
+                    pue=pue,
                 )
             else:
                 tracker = EmissionsTracker(
                     project_name=project_name,
                     measure_power_secs=measure_power_secs,
                     output_dir=output_dir,
                     output_file=output_file,
@@ -832,14 +844,16 @@
                     emissions_endpoint=emissions_endpoint,
                     experiment_id=experiment_id,
                     api_call_interval=api_call_interval,
                     api_key=api_key,
                     api_endpoint=api_endpoint,
                     save_to_api=save_to_api,
                     co2_signal_api_token=co2_signal_api_token,
+                    default_cpu_power=default_cpu_power,
+                    pue=pue,
                 )
             tracker.start()
             try:
                 fn_result = fn(*args, **kwargs)
             finally:
                 logger.info(
                     "\nGraceful stopping: collecting and writing information.\n"
```

### Comparing `codecarbon-2.2.2/codecarbon/external/geography.py` & `codecarbon-2.2.3/codecarbon/external/geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/external/hardware.py` & `codecarbon-2.2.3/codecarbon/external/hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/external/logger.py` & `codecarbon-2.2.3/codecarbon/external/logger.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/external/scheduler.py` & `codecarbon-2.2.3/codecarbon/external/scheduler.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/input.py` & `codecarbon-2.2.3/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/output.py` & `codecarbon-2.2.3/codecarbon/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     gpu_count: float
     gpu_model: str
     longitude: float
     latitude: float
     ram_total_size: float
     tracking_mode: str
     on_cloud: str = "N"
+    pue: float = 1
 
     @property
     def values(self) -> OrderedDict:
         return OrderedDict(self.__dict__.items())
 
     def compute_delta_emission(self, previous_emission):
         delta_duration = self.duration - previous_emission.duration
```

### Comparing `codecarbon-2.2.2/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.2.3/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.2.3/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.2.3/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/viz/carbonboard.py` & `codecarbon-2.2.3/codecarbon/viz/carbonboard.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.2.3/codecarbon/viz/carbonboard_on_api.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/viz/components.py` & `codecarbon-2.2.3/codecarbon/viz/components.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon/viz/data.py` & `codecarbon-2.2.3/codecarbon/viz/data.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/codecarbon.egg-info/PKG-INFO` & `codecarbon-2.2.3/codecarbon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.2
+Version: 2.2.3
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.2/codecarbon.egg-info/SOURCES.txt` & `codecarbon-2.2.3/codecarbon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/setup.py` & `codecarbon-2.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 
 TEST_DEPENDENCIES = ["mock", "pytest", "responses", "tox", "numpy", "requests-mock"]
 
 
 setuptools.setup(
     name="codecarbon",
-    version="2.2.2",
+    version="2.2.3",
     author="Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files=("LICENSE",),
     packages=setuptools.find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]
     ),
```

### Comparing `codecarbon-2.2.2/tests/test_api_call.py` & `codecarbon-2.2.3/tests/test_api_call.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_cloud.py` & `codecarbon-2.2.3/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_co2_signal.py` & `codecarbon-2.2.3/tests/test_co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_config.py` & `codecarbon-2.2.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_core_util.py` & `codecarbon-2.2.3/tests/test_core_util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_cpu.py` & `codecarbon-2.2.3/tests/test_cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_emissions.py` & `codecarbon-2.2.3/tests/test_emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_emissions_tracker.py` & `codecarbon-2.2.3/tests/test_emissions_tracker.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_emissions_tracker_constant.py` & `codecarbon-2.2.3/tests/test_emissions_tracker_constant.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_emissions_tracker_flush.py` & `codecarbon-2.2.3/tests/test_emissions_tracker_flush.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_energy.py` & `codecarbon-2.2.3/tests/test_energy.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_geography.py` & `codecarbon-2.2.3/tests/test_geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_gpu.py` & `codecarbon-2.2.3/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_hardware.py` & `codecarbon-2.2.3/tests/test_hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_logging_output.py` & `codecarbon-2.2.3/tests/test_logging_output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/test_ram.py` & `codecarbon-2.2.3/tests/test_ram.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/testdata.py` & `codecarbon-2.2.3/tests/testdata.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.2/tests/testutils.py` & `codecarbon-2.2.3/tests/testutils.py`

 * *Files identical despite different names*

