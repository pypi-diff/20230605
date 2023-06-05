# Comparing `tmp/ai_transform-0.31.3.tar.gz` & `tmp/ai_transform-0.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.31.3.tar", last modified: Wed May 24 06:05:44 2023, max compression
+gzip compressed data, was "ai_transform-0.32.0.tar", last modified: Mon Jun  5 07:15:37 2023, max compression
```

## Comparing `ai_transform-0.31.3.tar` & `ai_transform-0.32.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.664851 ai_transform-0.31.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-24 06:05:21.000000 ai_transform-0.31.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 06:05:44.664851 ai_transform-0.31.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-24 06:05:21.000000 ai_transform-0.31.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.652850 ai_transform-0.31.3/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.656850 ai_transform-0.31.3/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.656850 ai_transform-0.31.3/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.656850 ai_transform-0.31.3/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.656850 ai_transform-0.31.3/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.656850 ai_transform-0.31.3/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.656850 ai_transform-0.31.3/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.660851 ai_transform-0.31.3/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-24 06:05:21.000000 ai_transform-0.31.3/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.652850 ai_transform-0.31.3/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 06:05:44.000000 ai_transform-0.31.3/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-24 06:05:44.000000 ai_transform-0.31.3/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 06:05:44.000000 ai_transform-0.31.3/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-24 06:05:44.000000 ai_transform-0.31.3/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 06:05:44.000000 ai_transform-0.31.3/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 06:05:21.000000 ai_transform-0.31.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 06:05:44.664851 ai_transform-0.31.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-24 06:05:21.000000 ai_transform-0.31.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.660851 ai_transform-0.31.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.660851 ai_transform-0.31.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.660851 ai_transform-0.31.3/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.660851 ai_transform-0.31.3/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.660851 ai_transform-0.31.3/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.660851 ai_transform-0.31.3/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:44.664851 ai_transform-0.31.3/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-24 06:05:21.000000 ai_transform-0.31.3/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.004160 ai_transform-0.32.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-05 07:15:05.000000 ai_transform-0.32.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 07:15:37.004160 ai_transform-0.32.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-05 07:15:05.000000 ai_transform-0.32.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.992159 ai_transform-0.32.0/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-05 07:15:05.000000 ai_transform-0.32.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:15:37.004160 ai_transform-0.32.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-05 07:15:05.000000 ai_transform-0.32.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.004160 ai_transform-0.32.0/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.004160 ai_transform-0.32.0/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.004160 ai_transform-0.32.0/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.31.3/LICENSE` & `ai_transform-0.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/README.md` & `ai_transform-0.32.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/__init__.py` & `ai_transform-0.32.0/ai_transform/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.31.3"
+__version__ = "0.32.0"
 
 from ai_transform.timer import Timer
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.31.3/ai_transform/api/api.py` & `ai_transform-0.32.0/ai_transform/api/api.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/api/client.py` & `ai_transform-0.32.0/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/api/helpers.py` & `ai_transform-0.32.0/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/api/wrappers.py` & `ai_transform-0.32.0/ai_transform/api/wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/components/components.py` & `ai_transform-0.32.0/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/config.py` & `ai_transform-0.32.0/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/dataset/dataset.py` & `ai_transform-0.32.0/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/dataset/field.py` & `ai_transform-0.32.0/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/engine/abstract_engine.py` & `ai_transform-0.32.0/ai_transform/engine/abstract_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import time
-import logging
 import warnings
 
 from json import JSONDecodeError
 from typing import Any, List, Optional, Sequence, Iterator
 from abc import ABC, abstractmethod
 
 from tqdm.auto import tqdm
 
-from ai_transform.logger import format_logging_info, ic
+from ai_transform.logger import ic
 from ai_transform.types import Filter
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.operator.abstract_operator import AbstractOperator
 
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
 
@@ -103,28 +102,27 @@
             self._operator = None
             self._operators = operators
 
         if filters is None:
             filters = []
         assert isinstance(filters, list), "Filters must be applied as a list of Dictionaries"
 
-        if not refresh:
-            filters += self._get_refresh_filter(select_fields, dataset)
+        self._refresh = refresh
+        self._after_id = after_id
+
+        filters += self._get_refresh_filter()
         filters += self._get_workflow_filter()
 
         self._filters = filters
 
         if self.documents:
             self._size = len(documents)
         else:
             self._size = dataset.len(filters=filters) if self._limit_documents is None else self._limit_documents
 
-        self._refresh = refresh
-        self._after_id = after_id
-
         self._successful_documents = 0
         self._success_ratio = None
 
         self._job_id = None
         self._workflow_name = None
 
     @property
@@ -202,44 +200,44 @@
             # if there is no exception then this block will be executed
             # we only update schema on the first chunk
             # otherwise it breaks down how the backend handles
             # schema updates
             self._successful_documents += len(mini_batch)
             return transformed_batch
 
-    def _get_refresh_filter(self, select_fields: List[str], dataset: Dataset):
+    def _get_refresh_filter(self):
         # initialize the refresh filter container
-        refresh_filters = {"filter_type": "or", "condition_value": []}
+        input_field_filters = {"filter_type": "or", "condition_value": []}
 
         # initialize where the filters are going
-        input_field_filters = []
         output_field_filters = {"filter_type": "or", "condition_value": []}
 
-        # We want documents where all select_fields exists
+        # We want documents where any of the select_fields exists
         # as these are needed for operator ...
-        for field in select_fields:
-            input_field_filters += dataset[field].exists()
-
-        # ... and where any of its output_fields dont exist
-        for operator in self.operators:
-            if operator.output_fields is not None:
-                for output_field in operator.output_fields:
-                    output_field_filters["condition_value"] += dataset[output_field].not_exists()
-
         # We construct this as:
         #
-        #   input_field1 and input_field2 and (not output_field1 or not output_field2)
+        #   (input_field1 or input_field2) and (not output_field1 or not output_field2)
         #
         # This use case here is for two input fields and two output fields
         # tho this extends to arbitrarily many.
-        refresh_filters["condition_value"] = input_field_filters
-        refresh_filters["condition_value"] += [output_field_filters]
+        for field in self._select_fields:
+            input_field_filters["condition_value"] += self.dataset[field].exists()
+
+        # ... and where any of its output_fields dont exist
+        if not self._refresh:
+            for operator in self.operators:
+                if operator.output_fields is not None:
+                    for output_field in operator.output_fields:
+                        output_field_filters["condition_value"] += self.dataset[output_field].not_exists()
+
+            return [input_field_filters, output_field_filters]
 
-        # Wrap in list at end
-        return [refresh_filters]
+        else:
+            # Wrap in list at end
+            return [input_field_filters]
 
     def _get_workflow_filter(self, field: str = "_id"):
         # Get the required workflow filter as an environment variable
         # WORKER_NUMBER is passed into execute function
         # total number of workers must be greater than 1 for data sharding to work
         if self.worker_number is not None and self.total_workers is not None:
             if self.total_workers > 1:
```

### Comparing `ai_transform-0.31.3/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.32.0/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.32.0/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/engine/multipass_engine.py` & `ai_transform-0.32.0/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.32.0/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/engine/stable_engine.py` & `ai_transform-0.32.0/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/errors.py` & `ai_transform-0.32.0/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/logger.py` & `ai_transform-0.32.0/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/operator/abstract_operator.py` & `ai_transform-0.32.0/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/operator/dense_operator.py` & `ai_transform-0.32.0/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/timer.py` & `ai_transform-0.32.0/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/types.py` & `ai_transform-0.32.0/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/utils/document.py` & `ai_transform-0.32.0/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/utils/document_list.py` & `ai_transform-0.32.0/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/utils/example_documents.py` & `ai_transform-0.32.0/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/utils/json_encoder.py` & `ai_transform-0.32.0/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/utils/keyphrase.py` & `ai_transform-0.32.0/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.32.0/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/workflow/context_manager.py` & `ai_transform-0.32.0/ai_transform/workflow/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform/workflow/helpers.py` & `ai_transform-0.32.0/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.32.0/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/setup.py` & `ai_transform-0.32.0/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/conftest.py` & `ai_transform-0.32.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,14 +60,63 @@
     dataset = test_client.Dataset(dataset_id, expire=True)
     dataset.insert_documents(mock_documents(20))
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="class")
+def partial_dataset(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    documents = mock_documents(1000)
+    fields = ["sample_1_label", "sample_2_label", "sample_3_label"]
+    for document in documents:
+        for field in random.sample(fields, k=random.randint(1, 3)):
+            document.pop(field)
+    dataset.insert_documents(documents)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="class")
+def simple_partial_dataset(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    documents = mock_documents(1000)
+    fields = ["sample_1_label"]
+    for document in documents:
+        if random.random() < 0.5:
+            document.pop(fields[0])
+    dataset.insert_documents(documents)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="class")
+def partial_dataset_with_outputs(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    documents = mock_documents(1000)
+    fields = ["sample_1_label", "sample_2_label", "sample_3_label"]
+    for document in documents:
+        for field in random.sample(fields, k=random.randint(1, 3)):
+            document.pop(field)
+    for document in documents:
+        for field in fields:
+            if document.get(field) and random.random() < 0.5:
+                document[field + "_output"] = document[field] + "_output"
+    dataset.insert_documents(documents)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="class")
 def mixed_dataset(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
     dataset = test_client.Dataset(dataset_id, expire=True)
     documents = mock_documents(10)
     stripped = mock_documents(10)
     for document in stripped:
@@ -147,14 +196,34 @@
 
             return documents
 
     return ExampleOperator()
 
 
 @pytest.fixture(scope="function")
+def test_partial_operator() -> AbstractOperator:
+    class PartialOperator(AbstractOperator):
+        def __init__(self, fields):
+            super().__init__(input_fields=fields, output_fields=[field + "_output" for field in fields])
+
+        def transform(self, documents: DocumentList) -> DocumentList:
+            """
+            Main transform function
+            """
+            for input_field, output_field in zip(self.input_fields, self.output_fields):
+                for document in documents:
+                    if document.get(input_field):
+                        document[output_field] = document[input_field] + "_output"
+
+            return documents
+
+    return PartialOperator
+
+
+@pytest.fixture(scope="function")
 def test_paid_operator() -> AbstractOperator:
     class ExampleOperator(AbstractOperator):
         def __init__(self):
             super().__init__()
 
         def transform(self, documents: DocumentList) -> DocumentList:
             """
@@ -239,15 +308,15 @@
     dataset.insert_documents(mock_documents(20))
     time.sleep(1)
     job_id = str(uuid.uuid4())
     config = dict(
         job_id=job_id,
         dataset_id=dataset_id,
         authorizationToken=test_client.credentials.token,
-        text_field="sample_1_description_not_in_dataset",
+        text_field="sample_1_description",
     )
     config_string = json.dumps(config)
     config_bytes = config_string.encode()
     workflow_token = base64.b64encode(config_bytes).decode()
     yield workflow_token
     test_client.delete_dataset(dataset_id)
```

### Comparing `ai_transform-0.31.3/tests/core/test_api/test_client.py` & `ai_transform-0.32.0/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_api/test_endpoints.py` & `ai_transform-0.32.0/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.32.0/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_api/test_wrappers.py` & `ai_transform-0.32.0/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.32.0/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_dataset/test_field.py` & `ai_transform-0.32.0/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.32.0/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.32.0/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_engine/test_engine.py` & `ai_transform-0.32.0/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.32.0/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.32.0/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.32.0/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.32.0/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.32.0/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.3/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.32.0/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

