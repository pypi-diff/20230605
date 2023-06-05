# Comparing `tmp/chime_frb_api-3.2.0.tar.gz` & `tmp/chime_frb_api-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chime_frb_api-3.2.0.tar", max compression
+gzip compressed data, was "chime_frb_api-3.2.1.tar", max compression
```

## Comparing `chime_frb_api-3.2.0.tar` & `chime_frb_api-3.2.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     1080 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/LICENSE
--rw-r--r--   0        0        0     1386 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/README.md
--rw-r--r--   0        0        0      277 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/backends/__init__.py
--rw-r--r--   0        0        0      352 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/backends/bucket.py
--rw-r--r--   0        0        0      392 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/backends/distributor.py
--rw-r--r--   0        0        0     1932 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/backends/frb_master.py
--rw-r--r--   0        0        0      784 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/cli.py
--rw-r--r--   0        0        0      368 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/configs/__init__.py
--rw-r--r--   0        0        0      136 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/configs/test_workflow.yaml
--rw-r--r--   0        0        0     1185 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/configs/workflow.yaml
--rw-r--r--   0        0        0       48 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/core/__init__.py
--rw-r--r--   0        0        0    18785 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/core/core.py
--rw-r--r--   0        0        0      289 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/core/exceptions.py
--rw-r--r--   0        0        0      144 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/core/json_type.py
--rw-r--r--   0        0        0     2569 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/core/logger.py
--rw-r--r--   0        0        0      265 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/__init__.py
--rw-r--r--   0        0        0     4193 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/bucket.py
--rw-r--r--   0        0        0     8685 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/buckets.py
--rw-r--r--   0        0        0     4548 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/calibration.py
--rw-r--r--   0        0        0      570 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/candidates.py
--rw-r--r--   0        0        0      810 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/catalog.py
--rw-r--r--   0        0        0     4839 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/distributor.py
--rw-r--r--   0        0        0    11217 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/events.py
--rw-r--r--   0        0        0     5521 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/metrics.py
--rw-r--r--   0        0        0     2013 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/mimic.py
--rw-r--r--   0        0        0     4000 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/parameters.py
--rw-r--r--   0        0        0     4882 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/results.py
--rw-r--r--   0        0        0     1875 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/sources.py
--rw-r--r--   0        0        0    11581 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/swarm.py
--rw-r--r--   0        0        0    12551 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/tns.py
--rw-r--r--   0        0        0     1879 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/verification.py
--rw-r--r--   0        0        0    12214 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/voe.py
--rw-r--r--   0        0        0     4234 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/voe_subscribers.py
--rw-r--r--   0        0        0        0 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/stations/__init__.py
--rw-r--r--   0        0        0       22 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/stations/aro.py
--rw-r--r--   0        0        0      706 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/stations/drao.py
--rw-r--r--   0        0        0       22 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/stations/gbo.py
--rw-r--r--   0        0        0     2876 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/docker-compose.yml
--rw-r--r--   0        0        0     9065 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_archive.py
--rw-r--r--   0        0        0     3423 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_audit_daemon.py
--rw-r--r--   0        0        0     1830 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_bucket.py
--rw-r--r--   0        0        0     4282 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_buckets.py
--rw-r--r--   0        0        0     1764 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_calibration.py
--rw-r--r--   0        0        0      262 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_candidates.py
--rw-r--r--   0        0        0      610 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_catalog.py
--rw-r--r--   0        0        0     3413 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_core.py
--rw-r--r--   0        0        0     2066 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_distributor.py
--rw-r--r--   0        0        0     5823 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_events.py
--rw-r--r--   0        0        0     3335 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_metrics.py
--rw-r--r--   0        0        0      960 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_mimic.py
--rw-r--r--   0        0        0      849 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_parameters.py
--rw-r--r--   0        0        0     2134 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_results.py
--rw-r--r--   0        0        0      384 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_sources.py
--rw-r--r--   0        0        0      256 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_stations.py
--rw-r--r--   0        0        0     1454 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_swarm.py
--rw-r--r--   0        0        0     7035 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_tns.py
--rw-r--r--   0        0        0     5367 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_transfer_daemon.py
--rw-r--r--   0        0        0      467 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_verification.py
--rw-r--r--   0        0        0     8503 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_voe.py
--rw-r--r--   0        0        0     2780 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_voe_subscribers.py
--rw-r--r--   0        0        0     5167 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_work.py
--rw-r--r--   0        0        0     1208 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_work_http_operations.py
--rw-r--r--   0        0        0     6650 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/__init__.py
--rw-r--r--   0        0        0     2642 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/copy.py
--rw-r--r--   0        0        0      859 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/github.py
--rw-r--r--   0        0        0     1263 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/loki.py
--rw-r--r--   0        0        0     2642 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/move.py
--rw-r--r--   0        0        0       76 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/__init__.py
--rw-r--r--   0        0        0     3899 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/buckets.py
--rw-r--r--   0        0        0     5239 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/pipelines.py
--rw-r--r--   0        0        0    10180 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/run.py
--rw-r--r--   0        0        0      789 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/sample.py
--rw-r--r--   0        0        0      671 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/sample.yaml
--rw-r--r--   0        0        0        0 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/__init__.py
--rw-r--r--   0        0        0      980 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/audit.py
--rw-r--r--   0        0        0     6787 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/transfer.py
--rw-r--r--   0        0        0       32 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/__init__.py
--rw-r--r--   0        0        0     5166 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/archive.py
--rw-r--r--   0        0        0       33 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/attempt.py
--rw-r--r--   0        0        0      523 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/container.py
--rw-r--r--   0        0        0     4323 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/execute.py
--rw-r--r--   0        0        0     1418 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/validate.py
--rwxr-xr-x   0        0        0      408 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/runner.py
--rw-r--r--   0        0        0    18365 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/work.py
--rw-r--r--   0        0        0     1798 2023-05-25 15:09:33.437735 chime_frb_api-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     2990 1970-01-01 00:00:00.000000 chime_frb_api-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/LICENSE
+-rw-r--r--   0        0        0     1386 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/README.md
+-rw-r--r--   0        0        0      277 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/backends/__init__.py
+-rw-r--r--   0        0        0      352 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/backends/bucket.py
+-rw-r--r--   0        0        0      392 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/backends/distributor.py
+-rw-r--r--   0        0        0     1932 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/backends/frb_master.py
+-rw-r--r--   0        0        0      784 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/cli.py
+-rw-r--r--   0        0        0      368 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/configs/__init__.py
+-rw-r--r--   0        0        0      136 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/configs/test_workflow.yaml
+-rw-r--r--   0        0        0     1185 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/configs/workflow.yaml
+-rw-r--r--   0        0        0       48 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/core/__init__.py
+-rw-r--r--   0        0        0    18785 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/core/core.py
+-rw-r--r--   0        0        0      289 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/core/exceptions.py
+-rw-r--r--   0        0        0      144 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/core/json_type.py
+-rw-r--r--   0        0        0     2569 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/core/logger.py
+-rw-r--r--   0        0        0      265 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/__init__.py
+-rw-r--r--   0        0        0     4193 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/bucket.py
+-rw-r--r--   0        0        0     8685 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/buckets.py
+-rw-r--r--   0        0        0     4548 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/calibration.py
+-rw-r--r--   0        0        0      570 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/candidates.py
+-rw-r--r--   0        0        0      810 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/catalog.py
+-rw-r--r--   0        0        0     4839 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/distributor.py
+-rw-r--r--   0        0        0    11217 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/events.py
+-rw-r--r--   0        0        0     5521 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/metrics.py
+-rw-r--r--   0        0        0     2013 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/mimic.py
+-rw-r--r--   0        0        0     4000 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/parameters.py
+-rw-r--r--   0        0        0     4882 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/results.py
+-rw-r--r--   0        0        0     1875 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/sources.py
+-rw-r--r--   0        0        0    11581 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/swarm.py
+-rw-r--r--   0        0        0    12551 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/tns.py
+-rw-r--r--   0        0        0     1879 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/verification.py
+-rw-r--r--   0        0        0    12214 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/voe.py
+-rw-r--r--   0        0        0     4234 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/modules/voe_subscribers.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/stations/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/stations/aro.py
+-rw-r--r--   0        0        0      706 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/stations/drao.py
+-rw-r--r--   0        0        0       22 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/stations/gbo.py
+-rw-r--r--   0        0        0     2876 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/docker-compose.yml
+-rw-r--r--   0        0        0     9065 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_archive.py
+-rw-r--r--   0        0        0     3423 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_audit_daemon.py
+-rw-r--r--   0        0        0     1830 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_bucket.py
+-rw-r--r--   0        0        0     4282 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_buckets.py
+-rw-r--r--   0        0        0     1764 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_calibration.py
+-rw-r--r--   0        0        0      262 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_candidates.py
+-rw-r--r--   0        0        0      610 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_catalog.py
+-rw-r--r--   0        0        0     3413 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_core.py
+-rw-r--r--   0        0        0     2066 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_distributor.py
+-rw-r--r--   0        0        0     5823 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_events.py
+-rw-r--r--   0        0        0     3335 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_metrics.py
+-rw-r--r--   0        0        0      960 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_mimic.py
+-rw-r--r--   0        0        0      849 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_parameters.py
+-rw-r--r--   0        0        0     2134 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_results.py
+-rw-r--r--   0        0        0      384 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_sources.py
+-rw-r--r--   0        0        0      256 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_stations.py
+-rw-r--r--   0        0        0     1454 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_swarm.py
+-rw-r--r--   0        0        0     7035 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_tns.py
+-rw-r--r--   0        0        0     5367 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_transfer_daemon.py
+-rw-r--r--   0        0        0      467 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_verification.py
+-rw-r--r--   0        0        0     8503 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_voe.py
+-rw-r--r--   0        0        0     2780 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_voe_subscribers.py
+-rw-r--r--   0        0        0     5167 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_work.py
+-rw-r--r--   0        0        0     1208 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_work_http_operations.py
+-rw-r--r--   0        0        0     6650 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/utils/__init__.py
+-rw-r--r--   0        0        0     2642 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/utils/copy.py
+-rw-r--r--   0        0        0      859 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/utils/github.py
+-rw-r--r--   0        0        0     1263 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/utils/loki.py
+-rw-r--r--   0        0        0     2642 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/utils/move.py
+-rw-r--r--   0        0        0       76 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/workflow/cli/__init__.py
+-rw-r--r--   0        0        0     3899 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/workflow/cli/buckets.py
+-rw-r--r--   0        0        0     5239 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/workflow/cli/pipelines.py
+-rw-r--r--   0        0        0    10180 2023-06-05 19:07:12.691029 chime_frb_api-3.2.1/chime_frb_api/workflow/cli/run.py
+-rw-r--r--   0        0        0      789 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/cli/sample.py
+-rw-r--r--   0        0        0      671 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/cli/sample.yaml
+-rw-r--r--   0        0        0        0 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/daemons/__init__.py
+-rw-r--r--   0        0        0      980 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/daemons/audit.py
+-rw-r--r--   0        0        0     6787 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/daemons/transfer.py
+-rw-r--r--   0        0        0       32 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/__init__.py
+-rw-r--r--   0        0        0     5166 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/archive.py
+-rw-r--r--   0        0        0       33 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/attempt.py
+-rw-r--r--   0        0        0      523 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/container.py
+-rw-r--r--   0        0        0     4323 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/execute.py
+-rw-r--r--   0        0        0     1418 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/validate.py
+-rwxr-xr-x   0        0        0      408 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/runner.py
+-rw-r--r--   0        0        0    18365 2023-06-05 19:07:12.695029 chime_frb_api-3.2.1/chime_frb_api/workflow/work.py
+-rw-r--r--   0        0        0     1815 2023-06-05 19:07:12.707028 chime_frb_api-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 chime_frb_api-3.2.1/PKG-INFO
```

### Comparing `chime_frb_api-3.2.0/LICENSE` & `chime_frb_api-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/README.md` & `chime_frb_api-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/backends/frb_master.py` & `chime_frb_api-3.2.1/chime_frb_api/backends/frb_master.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/cli.py` & `chime_frb_api-3.2.1/chime_frb_api/cli.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/configs/workflow.yaml` & `chime_frb_api-3.2.1/chime_frb_api/configs/workflow.yaml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/core/core.py` & `chime_frb_api-3.2.1/chime_frb_api/core/core.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/core/logger.py` & `chime_frb_api-3.2.1/chime_frb_api/core/logger.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/bucket.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/bucket.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/buckets.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/calibration.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/calibration.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/candidates.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/candidates.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/catalog.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/catalog.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/distributor.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/distributor.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/events.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/events.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/metrics.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/metrics.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/mimic.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/mimic.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/parameters.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/parameters.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/results.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/results.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/sources.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/sources.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/swarm.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/swarm.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/tns.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/tns.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/verification.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/verification.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/voe.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/voe.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/modules/voe_subscribers.py` & `chime_frb_api-3.2.1/chime_frb_api/modules/voe_subscribers.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/stations/drao.py` & `chime_frb_api-3.2.1/chime_frb_api/stations/drao.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/docker-compose.yml` & `chime_frb_api-3.2.1/chime_frb_api/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_archive.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_audit_daemon.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_audit_daemon.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_bucket.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_buckets.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_calibration.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_catalog.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_core.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_distributor.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_distributor.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_events.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_metrics.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_mimic.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_mimic.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_parameters.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_results.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_swarm.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_swarm.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_tns.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_tns.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_transfer_daemon.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_transfer_daemon.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_voe.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_voe.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_voe_subscribers.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_voe_subscribers.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_work.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_work.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_work_http_operations.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_work_http_operations.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/tests/test_workflow.py` & `chime_frb_api-3.2.1/chime_frb_api/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/utils/copy.py` & `chime_frb_api-3.2.1/chime_frb_api/utils/copy.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/utils/github.py` & `chime_frb_api-3.2.1/chime_frb_api/utils/github.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/utils/loki.py` & `chime_frb_api-3.2.1/chime_frb_api/utils/loki.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/utils/move.py` & `chime_frb_api-3.2.1/chime_frb_api/utils/move.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/buckets.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/cli/buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/pipelines.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/run.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/cli/run.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/sample.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/cli/sample.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/sample.yaml` & `chime_frb_api-3.2.1/chime_frb_api/workflow/cli/sample.yaml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/audit.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/daemons/audit.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/transfer.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/daemons/transfer.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/archive.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/archive.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/container.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/container.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/execute.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/execute.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/validate.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/lifecycle/validate.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/chime_frb_api/workflow/work.py` & `chime_frb_api-3.2.1/chime_frb_api/workflow/work.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.2.0/pyproject.toml` & `chime_frb_api-3.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chime-frb-api"
-version = "3.2.0"
+version = "3.2.1"
 description = "CHIME/FRB API"
 authors = ["Shiny Brar <charanjotbrar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CHIMEFRB/frb-api"
 documentation = "https://github.com/CHIMEFRB/frb-api"
 classifiers = [
@@ -31,14 +31,15 @@
 tenacity = "^8.1"
 rich = "^13.1"
 mkdocs-material = { version = ">=8", optional = true }
 pytkdocs = { version = ">=0.10", optional = true, extras = ["numpy-style"] }
 mkdocstrings-python = { version = "^0.8.3", optional = true }
 python-logging-loki = "^0.3.1"
 mergedeep = "^1.3.4"
+pyyaml = "^6.0"
 
 [tool.poetry.extras]
 docs = ["mkdocs-material", "mkdocstrings-python", "pytkdocs"]
 
 [tool.poetry.scripts]
 frb-api = "chime_frb_api.cli:cli"
 workflow = "chime_frb_api.workflow.runner:cli"
```

### Comparing `chime_frb_api-3.2.0/PKG-INFO` & `chime_frb_api-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chime-frb-api
-Version: 3.2.0
+Version: 3.2.1
 Summary: CHIME/FRB API
 Home-page: https://github.com/CHIMEFRB/frb-api
 License: MIT
 Author: Shiny Brar
 Author-email: charanjotbrar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,14 +26,15 @@
 Requires-Dist: mkdocs-material (>=8) ; extra == "docs"
 Requires-Dist: mkdocstrings-python (>=0.8.3,<0.9.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyjwt (>=2,<3)
 Requires-Dist: python-dateutil (>=2,<3)
 Requires-Dist: python-logging-loki (>=0.3.1,<0.4.0)
 Requires-Dist: pytkdocs[numpy-style] (>=0.10) ; extra == "docs"
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: rich (>=13.1,<14.0)
 Requires-Dist: tenacity (>=8.1,<9.0)
 Project-URL: Documentation, https://github.com/CHIMEFRB/frb-api
 Project-URL: Repository, https://github.com/CHIMEFRB/frb-api
 Description-Content-Type: text/markdown
```

