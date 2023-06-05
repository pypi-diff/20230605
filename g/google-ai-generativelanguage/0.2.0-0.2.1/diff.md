# Comparing `tmp/google-ai-generativelanguage-0.2.0.tar.gz` & `tmp/google-ai-generativelanguage-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-ai-generativelanguage-0.2.0.tar", last modified: Fri May  5 19:20:54 2023, max compression
+gzip compressed data, was "google-ai-generativelanguage-0.2.1.tar", last modified: Mon Jun  5 13:59:54 2023, max compression
```

## Comparing `google-ai-generativelanguage-0.2.0.tar` & `google-ai-generativelanguage-0.2.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.367656 google-ai-generativelanguage-0.2.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4628 2023-05-05 19:20:54.367656 google-ai-generativelanguage-0.2.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3704 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.355657 google-ai-generativelanguage-0.2.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.355657 google-ai-generativelanguage-0.2.0/google/ai/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.355657 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage/
--rw-rw-r--   0 root         (0)     1003     3100 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.359657 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/
--rw-rw-r--   0 root         (0)     1003     2426 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     3627 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.359657 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.359657 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    22262 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    31346 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.359657 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6599 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13308 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13535 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18539 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.359657 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    18648 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27717 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003     5792 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.363656 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6411 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12800 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13054 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    16273 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.363656 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    22608 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    31700 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.363656 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6481 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13056 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13294 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17619 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.363656 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     1847 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2905 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/citation.py
--rw-rw-r--   0 root         (0)     1003    11871 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003     4669 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/model.py
--rw-rw-r--   0 root         (0)     1003     3158 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     7969 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/safety.py
--rw-rw-r--   0 root         (0)     1003    10979 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.367656 google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/
--rw-r--r--   0 root         (0)     1003     4628 2023-05-05 19:20:54.000000 google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3473 2023-05-05 19:20:54.000000 google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-05 19:20:54.000000 google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       17 2023-05-05 19:20:54.000000 google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-05 19:20:54.000000 google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-05-05 19:20:54.000000 google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-05 19:20:54.000000 google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-05-05 19:20:54.367656 google-ai-generativelanguage-0.2.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2953 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.367656 google-ai-generativelanguage-0.2.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.367656 google-ai-generativelanguage-0.2.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.367656 google-ai-generativelanguage-0.2.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-05 19:20:54.367656 google-ai-generativelanguage-0.2.0/tests/unit/gapic/generativelanguage_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/tests/unit/gapic/generativelanguage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003    92212 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003    92796 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py
--rw-rw-r--   0 root         (0)     1003    89656 2023-05-05 19:18:21.000000 google-ai-generativelanguage-0.2.0/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.726774 google-ai-generativelanguage-0.2.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4611 2023-06-05 13:59:54.726774 google-ai-generativelanguage-0.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3687 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.710774 google-ai-generativelanguage-0.2.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.710774 google-ai-generativelanguage-0.2.1/google/ai/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.714774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage/
+-rw-rw-r--   0 root         (0)     1003     3100 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage/__init__.py
+-rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.714774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     2426 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3627 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.714774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.714774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22262 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    31346 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.718774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6599 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13308 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13535 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18539 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.718774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18648 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27717 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5792 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.718774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6411 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12800 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13054 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    16273 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.718774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22608 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    31700 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.722774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6481 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13056 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13294 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17619 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.722774 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     1847 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2905 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    11871 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003     4669 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/model.py
+-rw-rw-r--   0 root         (0)     1003     3158 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     7969 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    10979 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.722774 google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/
+-rw-r--r--   0 root         (0)     1003     4611 2023-06-05 13:59:54.000000 google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3473 2023-06-05 13:59:54.000000 google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-05 13:59:54.000000 google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       17 2023-06-05 13:59:54.000000 google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-05 13:59:54.000000 google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-06-05 13:59:54.000000 google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-05 13:59:54.000000 google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-06-05 13:59:54.726774 google-ai-generativelanguage-0.2.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2953 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.722774 google-ai-generativelanguage-0.2.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.722774 google-ai-generativelanguage-0.2.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.722774 google-ai-generativelanguage-0.2.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:54.726774 google-ai-generativelanguage-0.2.1/tests/unit/gapic/generativelanguage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/tests/unit/gapic/generativelanguage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    92212 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003    92796 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003    89656 2023-06-05 13:56:51.000000 google-ai-generativelanguage-0.2.1/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py
```

### Comparing `google-ai-generativelanguage-0.2.0/LICENSE` & `google-ai-generativelanguage-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/MANIFEST.in` & `google-ai-generativelanguage-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/PKG-INFO` & `google-ai-generativelanguage-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-generativelanguage
-Version: 0.2.0
+Version: 0.2.1
 Summary: Google Ai Generativelanguage API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -35,15 +35,15 @@
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
 .. _Generative Language API: https://developers.generativeai.google/
-.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/generativelanguage/latest
+.. _Client Library Documentation: https://googleapis.dev/python/generativelanguage/latest
 .. _Product Documentation:  https://developers.generativeai.google/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
```

### Comparing `google-ai-generativelanguage-0.2.0/README.rst` & `google-ai-generativelanguage-0.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
 .. _Generative Language API: https://developers.generativeai.google/
-.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/generativelanguage/latest
+.. _Client Library Documentation: https://googleapis.dev/python/generativelanguage/latest
 .. _Product Documentation:  https://developers.generativeai.google/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
```

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage/gapic_version.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.2.1"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/gapic_metadata.json` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/gapic_version.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.2.1"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/client.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/client.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/__init__.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/citation.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/citation.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/discuss_service.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/model.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/model.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/model_service.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/safety.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/safety.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google/ai/generativelanguage_v1beta2/types/text_service.py` & `google-ai-generativelanguage-0.2.1/google/ai/generativelanguage_v1beta2/types/text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/PKG-INFO` & `google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-generativelanguage
-Version: 0.2.0
+Version: 0.2.1
 Summary: Google Ai Generativelanguage API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -35,15 +35,15 @@
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
 .. _Generative Language API: https://developers.generativeai.google/
-.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/generativelanguage/latest
+.. _Client Library Documentation: https://googleapis.dev/python/generativelanguage/latest
 .. _Product Documentation:  https://developers.generativeai.google/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
```

### Comparing `google-ai-generativelanguage-0.2.0/google_ai_generativelanguage.egg-info/SOURCES.txt` & `google-ai-generativelanguage-0.2.1/google_ai_generativelanguage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/setup.py` & `google-ai-generativelanguage-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/tests/__init__.py` & `google-ai-generativelanguage-0.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/tests/unit/__init__.py` & `google-ai-generativelanguage-0.2.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/tests/unit/gapic/__init__.py` & `google-ai-generativelanguage-0.2.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/tests/unit/gapic/generativelanguage_v1beta2/__init__.py` & `google-ai-generativelanguage-0.2.1/tests/unit/gapic/generativelanguage_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py` & `google-ai-generativelanguage-0.2.1/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py` & `google-ai-generativelanguage-0.2.1/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.2.0/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py` & `google-ai-generativelanguage-0.2.1/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py`

 * *Files identical despite different names*

