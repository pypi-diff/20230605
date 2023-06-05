# Comparing `tmp/giskard-1.9.1.tar.gz` & `tmp/giskard-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-1.9.1.tar", max compression
+gzip compressed data, was "giskard-2.0.0b1.tar", last modified: Mon Jun  5 15:46:48 2023, max compression
```

## Comparing `giskard-1.9.1.tar` & `giskard-2.0.0b1.tar`

### file list

```diff
@@ -1,48 +1,220 @@
--rw-r--r--   0        0        0    12124 2023-01-23 17:24:47.551223 giskard-1.9.1/README.md
--rw-r--r--   0        0        0      859 2023-03-17 16:15:32.290842 giskard-1.9.1/giskard/__init__.py
--rw-r--r--   0        0        0     6745 2023-03-17 16:15:32.291169 giskard-1.9.1/giskard/cli.py
--rw-r--r--   0        0        0     2067 2023-03-17 16:15:32.291532 giskard-1.9.1/giskard/cli_utils.py
--rw-r--r--   0        0        0        0 2023-03-17 16:15:32.292058 giskard-1.9.1/giskard/client/__init__.py
--rw-r--r--   0        0        0     2342 2023-03-17 16:15:32.292524 giskard-1.9.1/giskard/client/analytics_collector.py
--rw-r--r--   0        0        0     5109 2023-03-17 16:15:32.292989 giskard-1.9.1/giskard/client/giskard_client.py
--rw-r--r--   0        0        0     2102 2023-02-20 18:05:11.279579 giskard-1.9.1/giskard/client/io_utils.py
--rw-r--r--   0        0        0      874 2023-03-17 16:15:32.293094 giskard-1.9.1/giskard/client/model.py
--rw-r--r--   0        0        0    31739 2023-03-17 16:15:32.293668 giskard-1.9.1/giskard/client/project.py
--rw-r--r--   0        0        0        0 2023-01-23 17:24:47.553209 giskard-1.9.1/giskard/client/py.typed
--rw-r--r--   0        0        0      673 2023-02-20 23:26:58.213126 giskard-1.9.1/giskard/client/python_utils.py
--rw-r--r--   0        0        0        0 2023-01-23 17:24:47.553300 giskard-1.9.1/giskard/ml_worker/__init__.py
--rw-r--r--   0        0        0       42 2023-01-23 17:24:47.553370 giskard-1.9.1/giskard/ml_worker/bridge/error.py
--rw-r--r--   0        0        0     7239 2023-03-17 16:15:32.294001 giskard-1.9.1/giskard/ml_worker/bridge/ml_worker_bridge.py
--rw-r--r--   0        0        0       50 2023-03-17 16:15:32.294293 giskard-1.9.1/giskard/ml_worker/bridge/service_messages.py
--rw-r--r--   0        0        0        0 2023-03-17 16:15:32.294343 giskard-1.9.1/giskard/ml_worker/core/__init__.py
--rw-r--r--   0        0        0      814 2023-03-17 16:15:32.294580 giskard-1.9.1/giskard/ml_worker/core/giskard_dataset.py
--rw-r--r--   0        0        0     4080 2023-03-17 16:15:32.294790 giskard-1.9.1/giskard/ml_worker/core/model.py
--rw-r--r--   0        0        0     6158 2023-03-17 16:15:32.295096 giskard-1.9.1/giskard/ml_worker/core/model_explanation.py
--rw-r--r--   0        0        0      375 2023-01-23 17:24:47.554312 giskard-1.9.1/giskard/ml_worker/exceptions/IllegalArgumentError.py
--rw-r--r--   0        0        0        0 2023-01-23 17:24:47.554336 giskard-1.9.1/giskard/ml_worker/exceptions/__init__.py
--rw-r--r--   0        0        0      114 2023-01-23 17:24:47.554390 giskard-1.9.1/giskard/ml_worker/exceptions/giskard_exception.py
--rw-r--r--   0        0        0    41119 2023-03-17 16:28:21.739680 giskard-1.9.1/giskard/ml_worker/generated/ml_worker_pb2.py
--rw-r--r--   0        0        0    48891 2023-03-17 16:28:21.708849 giskard-1.9.1/giskard/ml_worker/generated/ml_worker_pb2.pyi
--rw-r--r--   0        0        0    17884 2023-03-17 16:28:21.739367 giskard-1.9.1/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
--rw-r--r--   0        0        0     4119 2023-03-17 16:28:21.709144 giskard-1.9.1/giskard/ml_worker/generated/ml_worker_pb2_grpc.pyi
--rw-r--r--   0        0        0     1776 2023-03-17 16:15:32.295288 giskard-1.9.1/giskard/ml_worker/ml_worker.py
--rw-r--r--   0        0        0        0 2023-01-23 17:24:47.554476 giskard-1.9.1/giskard/ml_worker/server/__init__.py
--rw-r--r--   0        0        0    13845 2023-03-17 16:15:32.295772 giskard-1.9.1/giskard/ml_worker/server/ml_worker_service.py
--rw-r--r--   0        0        0        0 2023-01-23 17:24:47.555156 giskard-1.9.1/giskard/ml_worker/testing/__init__.py
--rw-r--r--   0        0        0     1029 2023-03-17 16:15:32.295918 giskard-1.9.1/giskard/ml_worker/testing/abstract_test_collection.py
--rw-r--r--   0        0        0    31525 2023-03-17 16:15:32.296398 giskard-1.9.1/giskard/ml_worker/testing/drift_tests.py
--rw-r--r--   0        0        0      935 2023-03-16 09:52:13.159685 giskard-1.9.1/giskard/ml_worker/testing/functions.py
--rw-r--r--   0        0        0    30966 2023-03-17 16:15:32.298162 giskard-1.9.1/giskard/ml_worker/testing/metamorphic_tests.py
--rw-r--r--   0        0        0    23410 2023-03-17 16:15:32.298400 giskard-1.9.1/giskard/ml_worker/testing/performance_tests.py
--rw-r--r--   0        0        0     4719 2023-03-17 16:15:32.298567 giskard-1.9.1/giskard/ml_worker/testing/stat_utils.py
--rw-r--r--   0        0        0    10438 2023-03-17 16:15:32.298771 giskard-1.9.1/giskard/ml_worker/testing/statistical_tests.py
--rw-r--r--   0        0        0     1770 2023-03-05 23:31:01.264436 giskard-1.9.1/giskard/ml_worker/testing/utils.py
--rw-r--r--   0        0        0        0 2023-01-23 17:24:47.556028 giskard-1.9.1/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0        0        0     2449 2023-03-17 16:15:32.298981 giskard-1.9.1/giskard/ml_worker/utils/error_interceptor.py
--rw-r--r--   0        0        0     1832 2023-03-17 16:15:32.299121 giskard-1.9.1/giskard/ml_worker/utils/grpc_mapper.py
--rw-r--r--   0        0        0     2181 2023-03-17 16:15:32.299483 giskard-1.9.1/giskard/ml_worker/utils/logging.py
--rw-r--r--   0        0        0      498 2023-02-21 09:29:33.873588 giskard-1.9.1/giskard/ml_worker/utils/network.py
--rw-r--r--   0        0        0      393 2023-03-17 16:15:32.299622 giskard-1.9.1/giskard/path_utils.py
--rw-r--r--   0        0        0      843 2023-03-17 16:15:32.299742 giskard-1.9.1/giskard/settings.py
--rw-r--r--   0        0        0     4699 2023-03-17 16:31:38.690560 giskard-1.9.1/pyproject.toml
--rw-r--r--   0        0        0    14437 1970-01-01 00:00:00.000000 giskard-1.9.1/PKG-INFO
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.296171 giskard-2.0.0b1/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13101 2023-06-05 15:46:48.296287 giskard-2.0.0b1/PKG-INFO
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12124 2023-04-12 00:50:05.000000 giskard-2.0.0b1/README.md
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.245336 giskard-2.0.0b1/giskard/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1681 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/cli.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/cli_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.248245 giskard-2.0.0b1/giskard/client/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/client/dtos.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/client/giskard_client.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/client/io_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/client/project.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-04-12 00:50:05.000000 giskard-2.0.0b1/giskard/client/python_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.250599 giskard-2.0.0b1/giskard/commands/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14555 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/commands/cli_server.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7042 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/commands/cli_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.256664 giskard-2.0.0b1/giskard/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/core/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11273 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/core/core.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/core/dataset_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/core/errors.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13200 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/core/model_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-05 15:04:55.000000 giskard-2.0.0b1/giskard/core/suite.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/core/validation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.256944 giskard-2.0.0b1/giskard/datasets/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/datasets/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.257133 giskard-2.0.0b1/giskard/datasets/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26419 2023-06-05 15:04:55.000000 giskard-2.0.0b1/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.263799 giskard-2.0.0b1/giskard/datasets/metadata/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.264133 giskard-2.0.0b1/giskard/demo/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2931 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/demo/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/demo/titanic.csv
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.264526 giskard-2.0.0b1/giskard/ml_worker/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b1/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.265446 giskard-2.0.0b1/giskard/ml_worker/bridge/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b1/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/ml_worker/bridge/ml_worker_bridge.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/bridge/service_messages.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.265862 giskard-2.0.0b1/giskard/ml_worker/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/core/log_listener.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5951 2023-06-05 15:04:55.000000 giskard-2.0.0b1/giskard/ml_worker/core/savable.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.266414 giskard-2.0.0b1/giskard/ml_worker/exceptions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b1/giskard/ml_worker/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b1/giskard/ml_worker/exceptions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b1/giskard/ml_worker/exceptions/giskard_exception.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.266771 giskard-2.0.0b1/giskard/ml_worker/generated/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-05 15:46:48.000000 giskard-2.0.0b1/giskard/ml_worker/generated/ml_worker_pb2.py
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-05 15:46:48.000000 giskard-2.0.0b1/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.267013 giskard-2.0.0b1/giskard/ml_worker/server/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b1/giskard/ml_worker/server/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26370 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/ml_worker/server/ml_worker_service.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.268110 giskard-2.0.0b1/giskard/ml_worker/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b1/giskard/ml_worker/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.268809 giskard-2.0.0b1/giskard/ml_worker/testing/functions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/testing/functions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3851 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/testing/functions/slicing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6431 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/ml_worker/testing/functions/transformation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.270545 giskard-2.0.0b1/giskard/ml_worker/testing/registry/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/testing/registry/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/testing/registry/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/testing/registry/decorators_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/ml_worker/testing/registry/giskard_test.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/ml_worker/testing/registry/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-05 15:04:55.000000 giskard-2.0.0b1/giskard/ml_worker/testing/registry/slicing_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-05 15:04:55.000000 giskard-2.0.0b1/giskard/ml_worker/testing/registry/transformation_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/testing/registry/udf_repository.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/testing/stat_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/testing/test_result.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1598 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/testing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.271827 giskard-2.0.0b1/giskard/ml_worker/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b1/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/utils/file_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/ml_worker/utils/logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      498 2023-04-12 00:50:05.000000 giskard-2.0.0b1/giskard/ml_worker/utils/network.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/ml_worker/utils/request_interceptor.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.272857 giskard-2.0.0b1/giskard/models/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/models/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/models/_precooked.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.273029 giskard-2.0.0b1/giskard/models/automodel/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9112 2023-06-05 15:04:55.000000 giskard-2.0.0b1/giskard/models/automodel/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.273325 giskard-2.0.0b1/giskard/models/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34146 2023-06-05 15:04:55.000000 giskard-2.0.0b1/giskard/models/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.274179 giskard-2.0.0b1/giskard/models/cache/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/models/cache/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2701 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/models/cache/cache.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.274370 giskard-2.0.0b1/giskard/models/catboost/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/models/catboost/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.274654 giskard-2.0.0b1/giskard/models/function/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/models/function/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.274949 giskard-2.0.0b1/giskard/models/huggingface/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5880 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/models/huggingface/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.275144 giskard-2.0.0b1/giskard/models/langchain/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2617 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/models/langchain/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6701 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/models/model_explanation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.275328 giskard-2.0.0b1/giskard/models/pytorch/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7213 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/models/pytorch/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.275519 giskard-2.0.0b1/giskard/models/sklearn/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4329 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/models/sklearn/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.275685 giskard-2.0.0b1/giskard/models/tensorflow/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1664 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/models/tensorflow/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/models/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/path_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.277421 giskard-2.0.0b1/giskard/scanner/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/scanner/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.278244 giskard-2.0.0b1/giskard/scanner/calibration/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/calibration/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.278701 giskard-2.0.0b1/giskard/scanner/common/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/common/examples.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/common/loss_based_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.278948 giskard-2.0.0b1/giskard/scanner/data_leakage/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/issues.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.279390 giskard-2.0.0b1/giskard/scanner/llm/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5910 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/scanner/llm/toxicity_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/scanner/llm/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/logger.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.280182 giskard-2.0.0b1/giskard/scanner/performance/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4126 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/performance/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/result.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.282902 giskard-2.0.0b1/giskard/scanner/robustness/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6078 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      934 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3246 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/scanner/robustness/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      987 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7982 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/scanner/scanner.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.283090 giskard-2.0.0b1/giskard/scanner/stochasticity/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.284614 giskard-2.0.0b1/giskard/scanner/templates/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      783 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/_code_snippet.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.286026 giskard-2.0.0b1/giskard/scanner/templates/_issues/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/_issues/data_leakage.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/_issues/default.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/scanner/templates/_issues/llm_toxicity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/_issues/overconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/_issues/performance.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/_issues/robustness.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/_issues/stochasticity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/_issues/underconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/scanner/templates/_issues_table.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/scanner/templates/_main_content.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-02 09:24:08.000000 giskard-2.0.0b1/giskard/scanner/templates/_tab_header.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      187 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/base.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      550 2023-06-04 23:03:53.000000 giskard-2.0.0b1/giskard/scanner/templates/scan_results.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.286673 giskard-2.0.0b1/giskard/scanner/templates/static/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-02 09:24:08.000000 giskard-2.0.0b1/giskard/scanner/templates/static/style.css
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.287111 giskard-2.0.0b1/giskard/scanner/visualization/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/scanner/visualization/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/scanner/visualization/custom_jinja.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/settings.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.289264 giskard-2.0.0b1/giskard/slicing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/base.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/category_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/slicing/slice.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/stop_words.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/text_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/slicing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.289408 giskard-2.0.0b1/giskard/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.291030 giskard-2.0.0b1/giskard/testing/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/testing/tests/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33261 2023-06-05 15:37:25.000000 giskard-2.0.0b1/giskard/testing/tests/drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30180 2023-06-05 15:04:55.000000 giskard-2.0.0b1/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    24509 2023-06-05 15:37:17.000000 giskard-2.0.0b1/giskard/testing/tests/performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10315 2023-06-05 15:04:55.000000 giskard-2.0.0b1/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.291853 giskard-2.0.0b1/giskard/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-02 00:09:24.000000 giskard-2.0.0b1/giskard/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5502 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/utils/analytics_collector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-04 21:20:31.000000 giskard-2.0.0b1/giskard/utils/display.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-05 15:02:01.000000 giskard-2.0.0b1/giskard/utils/environment_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.246582 giskard-2.0.0b1/giskard.egg-info/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    13101 2023-06-05 15:46:48.000000 giskard-2.0.0b1/giskard.egg-info/PKG-INFO
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-05 15:46:48.000000 giskard-2.0.0b1/giskard.egg-info/SOURCES.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-05 15:46:48.000000 giskard-2.0.0b1/giskard.egg-info/dependency_links.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-05 15:46:48.000000 giskard-2.0.0b1/giskard.egg-info/entry_points.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      591 2023-06-05 15:46:48.000000 giskard-2.0.0b1/giskard.egg-info/requires.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        8 2023-06-05 15:46:48.000000 giskard-2.0.0b1/giskard.egg-info/top_level.txt
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6637 2023-06-05 15:04:55.000000 giskard-2.0.0b1/pyproject.toml
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-05 15:46:48.296617 giskard-2.0.0b1/setup.cfg
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-02 00:09:24.000000 giskard-2.0.0b1/setup.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-05 15:46:48.295987 giskard-2.0.0b1/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1521 2023-06-04 23:03:53.000000 giskard-2.0.0b1/tests/test_custom_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_data_drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_dataset.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b1/tests/test_logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_metamorphic_direction.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2800 2023-06-04 23:03:53.000000 giskard-2.0.0b1/tests/test_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_model_auto_inference.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_model_explanation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_model_postprocess.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13505 2023-06-04 21:20:31.000000 giskard-2.0.0b1/tests/test_performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-04 23:03:53.000000 giskard-2.0.0b1/tests/test_programmatic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_project_uploads.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_statistical.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_upload.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-02 00:09:24.000000 giskard-2.0.0b1/tests/test_utils.py
```

### Comparing `giskard-1.9.1/README.md` & `giskard-2.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `giskard-1.9.1/giskard/cli.py` & `giskard-2.0.0b1/giskard/commands/cli_worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,220 +1,220 @@
 import asyncio
+import functools
 import logging
 import os
 import platform
 import sys
+from typing import Optional
 
 import click
 import lockfile
 import psutil
 from click import INT, STRING
 from lockfile.pidlockfile import PIDLockFile, read_pid_from_pidfile, remove_existing_pidfile
+from pydantic import AnyHttpUrl
 
-import giskard
+from giskard.cli_utils import common_options
 from giskard.cli_utils import (
     create_pid_file_path,
     remove_stale_pid_file,
     run_daemon,
     get_log_path,
     tail,
-    follow_file,
+    follow_file, validate_url,
 )
-from giskard.client.analytics_collector import GiskardAnalyticsCollector, anonymize
-from giskard.ml_worker.ml_worker import start_ml_worker
 from giskard.path_utils import run_dir
 from giskard.settings import settings
-
-run_dir.mkdir(parents=True, exist_ok=True)
+from giskard.utils.analytics_collector import anonymize, analytics
 
 logger = logging.getLogger(__name__)
-analytics = GiskardAnalyticsCollector()
-
-
-def set_verbose(_ctx, _param, value):
-    if value:
-        logging.getLogger().setLevel(logging.DEBUG)
-
-
-@click.group("cli")
-@click.version_option(f"{giskard.__version__} (Python {platform.python_version()})")
-def cli():
-    """
-    Giskard Command Line
-    """
 
 
-@cli.group("worker", help="ML Worker management", context_settings={"show_default": True})
+@click.group("worker", help="ML Worker management", context_settings={"show_default": True})
 def worker() -> None:
     """
     ML Worker management
     """
 
 
-def start_stop_options(fn):
-    fn = click.option(
-        "--host",
-        "-h",
+def start_stop_options(func):
+    @click.option(
+        "--url",
+        "-u",
         type=STRING,
-        default="localhost",
-        help="Remote Giskard host address to connect to",
-    )(fn)
-
-    fn = click.option(
+        default="http://localhost:19000",
+        help="Remote Giskard server url",
+        callback=validate_url,
+    )
+    @click.option(
         "--server",
         "-s",
         "is_server",
         is_flag=True,
         default=False,
         help="Server mode. Used by Giskard embedded ML Worker",
-    )(fn)
-    fn = click.option(
-        "--port",
-        "-p",
-        type=INT,
-        default=40051,
-        help="Remote Giskard port accepting external ML Worker connections",
-    )(fn)
-    fn = click.option(
-        "--verbose",
-        "-v",
-        is_flag=True,
-        callback=set_verbose,
-        default=False,
-        expose_value=False,
-        is_eager=True,
-        help="Enable verbose logging",
-    )(fn)
-    return fn
+    )
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
+
+    return wrapper
 
 
 @worker.command("start")
+@common_options
 @start_stop_options
 @click.option(
+    "--key",
+    "-k",
+    "api_key",
+    envvar="GSK_API_KEY",
+    help="Giskard server API key",
+)
+@click.option(
     "--daemon",
     "-d",
     "is_daemon",
     is_flag=True,
     default=False,
     help="Should ML Worker be started as a Daemon in a background",
 )
-def start_command(host, port, is_server, is_daemon):
+def start_command(url: AnyHttpUrl, is_server, api_key, is_daemon):
     """\b
     Start ML Worker.
 
     ML Worker can be started in 2 modes:
 
     - server: used by default by an ML Worker shipped by Giskard. ML Worker acts as a server that Giskard connects to.
 
     - client: ML Worker acts as a client and should connect to a running Giskard instance
         by specifying this instance's host and port.
     """
+    api_key = initialize_api_key(api_key, is_server)
+    _start_command(is_server, url, api_key, is_daemon)
+
 
-    _start_command(is_server, host, port, is_daemon)
+def initialize_api_key(api_key, is_server):
+    if is_server:
+        return None
+    if not api_key:
+        api_key = click.prompt("Enter Giskard server API key", type=str)
+    if "GSK_API_KEY" in os.environ:
+        # delete API key environment variable so that it doesn't get leaked when the test code is executed
+        del os.environ["GSK_API_KEY"]
+    return api_key
 
 
-def _start_command(is_server, host, port, is_daemon):
+def _start_command(is_server, url: AnyHttpUrl, api_key, is_daemon):
+    from giskard.ml_worker.ml_worker import MLWorker
+
     analytics.track(
-        "Start ML Worker",
-        {
-            "is_server": is_server,
-            "host": anonymize(host),
-            "port": anonymize(port),
-            "is_daemon": is_daemon,
-        },
-        force=True,
+        "Start ML Worker", {"is_server": is_server, "url": anonymize(url), "is_daemon": is_daemon}, force=True
     )
+
     start_msg = "Starting ML Worker"
     start_msg += " server" if is_server else " client"
     if is_daemon:
         start_msg += " daemon"
     logger.info(start_msg)
     logger.info(f"Python: {sys.executable} ({platform.python_version()})")
     logger.info(f"Giskard Home: {settings.home_dir}")
-    pid_file_path = create_pid_file_path(is_server, host, port)
+    pid_file_path = create_pid_file_path(is_server, url)
     pid_file = PIDLockFile(pid_file_path)
     remove_stale_pid_file(pid_file)
+
+    ml_worker: Optional[MLWorker] = None
     try:
         pid_file.acquire()
         if is_daemon:
             # Releasing the lock because it will be re-acquired by a daemon process
             pid_file.release()
-            run_daemon(is_server, host, port)
+            # If on windows, throw error and exit
+            if sys.platform == "win32":
+                logger.error("Daemon mode is not supported on Windows.")
+                return
+
+            run_daemon(is_server, url, api_key)
         else:
-            loop = asyncio.new_event_loop()
-            loop.create_task(start_ml_worker(is_server, host, port))
-            loop.run_forever()
+            ml_worker = MLWorker(is_server, url, api_key)
+            asyncio.get_event_loop().run_until_complete(ml_worker.start())
     except KeyboardInterrupt:
         logger.info("Exiting")
+        if ml_worker:
+            asyncio.get_event_loop().run_until_complete(ml_worker.stop())
     except lockfile.AlreadyLocked:
         existing_pid = read_pid_from_pidfile(pid_file_path)
         logger.warning(
-            f"Another ML Worker {_ml_worker_description(is_server, host, port)} "
+            f"Another ML Worker {_ml_worker_description(is_server, url)} "
             f"is already running with PID: {existing_pid}. "
             f"Not starting a new one."
         )
     finally:
         if pid_file.i_am_locking():
             pid_file.release()
 
 
-def _ml_worker_description(is_server, host, port):
-    return "server" if is_server else f"client for {host or 'localhost'}:{port or ''}"
+def _ml_worker_description(is_server, url):
+    return "server" if is_server else f"client for {url}"
 
 
 @worker.command("stop", help="Stop running ML Workers")
+@common_options
 @start_stop_options
-@click.option(
-    "--all", "-a", "stop_all", is_flag=True, default=False, help="Stop all running ML Workers"
-)
-def stop_command(is_server, host, port, stop_all):
+@click.option("--all", "-a", "stop_all", is_flag=True, default=False, help="Stop all running ML Workers")
+def stop_command(is_server, url, stop_all):
     import re
 
     if stop_all:
         for pid_fname in os.listdir(run_dir):
             if not re.match(r"^ml-worker-.*\.pid$", pid_fname):
                 continue
             _stop_pid_fname(pid_fname)
     else:
-        _find_and_stop(is_server, host, port)
+        _find_and_stop(is_server, url)
 
 
 @worker.command("restart", help="Restart ML Worker")
+@common_options
 @start_stop_options
-def restart_command(is_server, host, port):
-    _find_and_stop(is_server, host, port)
-    _start_command(is_server, host, port, is_daemon=True)
+@click.option("--api-key", "-k", "api_key", help="Giskard server API key")
+def restart_command(is_server, url, api_key):
+    api_key = initialize_api_key(api_key, is_server)
+
+    _find_and_stop(is_server, url)
+    _start_command(is_server, url, api_key, is_daemon=True)
 
 
 def _stop_pid_fname(pid_fname):
     pid_file_path = str(run_dir / pid_fname)
     remove_stale_pid_file(PIDLockFile(pid_file_path))
     pid = read_pid_from_pidfile(pid_file_path)
     if pid:
         worker_process = psutil.Process(pid)
         worker_process.terminate()
         logger.info(f"Stopped ML Worker Daemon by PID: {pid}")
     remove_existing_pidfile(pid_file_path)
 
 
-def _find_and_stop(is_server, host, port):
-    pid_file_path = str(create_pid_file_path(is_server, host, port))
+def _find_and_stop(is_server, url):
+    pid_file_path = str(create_pid_file_path(is_server, url))
     remove_stale_pid_file(PIDLockFile(pid_file_path))
     pid = read_pid_from_pidfile(pid_file_path)
     logger.info("Stopping ML Worker Daemon")
     if pid:
         worker_process = psutil.Process(pid)
         worker_process.terminate()
-        logger.info(f"Stopped ML Worker {_ml_worker_description(is_server, host, port)}")
+        logger.info(f"Stopped ML Worker {_ml_worker_description(is_server, url)}")
     else:
-        logger.info(f"ML Worker {_ml_worker_description(is_server, host, port)} is not running")
+        logger.info(f"ML Worker {_ml_worker_description(is_server, url)} is not running")
     remove_existing_pidfile(pid_file_path)
 
 
 @worker.command("logs")
+@common_options
 @click.option(
     "--lines",
     "-n",
     type=INT,
     default=10,
     help="Output the last N lines of the log file, 10 lines are displayed by default",
 )
@@ -234,11 +234,7 @@
         exit(-1)
 
     for line in tail(log_path, lines):
         print(line, end="")
 
     if is_follow:
         follow_file(log_path)
-
-
-if __name__ == "__main__":
-    cli()
```

### Comparing `giskard-1.9.1/giskard/cli_utils.py` & `giskard-2.0.0b1/giskard/cli_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,105 @@
 import asyncio
 import collections
+import functools
 import hashlib
 import logging
 import os
 import sys
 from time import sleep
 
-from daemon import DaemonContext
-from daemon.daemon import change_working_directory
-from daemon.runner import is_pidfile_stale
+import click
 from lockfile.pidlockfile import PIDLockFile
+from pydantic import AnyHttpUrl, parse_obj_as
 
-from giskard.ml_worker.ml_worker import start_ml_worker
 from giskard.path_utils import run_dir
 from giskard.settings import settings
 
 logger = logging.getLogger(__name__)
+logging.getLogger().setLevel(logging.INFO)
+logging.getLogger("giskard").setLevel(logging.INFO)
+
+
+def common_options(func):
+    @click.option(
+        "--verbose",
+        "-v",
+        is_flag=True,
+        callback=set_verbose,
+        default=False,
+        expose_value=False,
+        is_eager=True,
+        help="Enable verbose logging",
+    )
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+def set_verbose(_ctx, _param, value):
+    if value:
+        logging.getLogger("giskard").setLevel(logging.DEBUG)
 
 
 def remove_stale_pid_file(pid_file):
-    if is_pidfile_stale(pid_file):
+    pid = pid_file.read_pid()
+    if pid is not None and is_pid_stale(pid):
         logger.debug("Stale PID file found, removing it")
         pid_file.break_lock()
 
 
-def create_pid_file_path(is_server, host, port):
+def is_pid_stale(pid):
+    try:
+        os.kill(pid, 0)  # NOSONAR
+    except (OSError, TypeError):
+        return True
+    else:
+        return False
+
+
+def create_pid_file_path(is_server, url):
+    hash_value = ml_worker_id(is_server, url)
+    return run_dir / f"ml-worker-{hash_value}.pid"
+
+
+def ml_worker_id(is_server, url):
     key = f"{sys.executable}"
     if not is_server:
-        key += f"{host}{port}"
+        key += url
     hash_value = hashlib.sha1(key.encode()).hexdigest()
-    return run_dir / f"ml-worker-{hash_value}.pid"
+    return hash_value
+
 
+def validate_url(_ctx, _param, value) -> AnyHttpUrl:
+    return parse_obj_as(AnyHttpUrl, value)
+
+
+def run_daemon(is_server, url, api_key):
+    from giskard.ml_worker.ml_worker import MLWorker
+    from daemon import DaemonContext
+    from daemon.daemon import change_working_directory
 
-def run_daemon(is_server, host, port):
     log_path = get_log_path()
     logger.info(f"Writing logs to {log_path}")
-    pid_file = PIDLockFile(create_pid_file_path(is_server, host, port))
+    pid_file = PIDLockFile(create_pid_file_path(is_server, url))
 
     with DaemonContext(pidfile=pid_file, stdout=open(log_path, "w+t")):
+        # For some reason requests.utils.should_bypass_proxies that's called inside every request made by requests
+        # hangs when the process runs as a daemon. A dirty temporary fix is to disable proxies for daemon mode.
+        # True reasons for this to happen to be investigated
+        os.environ['no_proxy'] = '*'
+
         workdir = settings.home_dir / "tmp" / f"daemon-run-{os.getpid()}"
         workdir.mkdir(exist_ok=True, parents=True)
         change_working_directory(workdir)
 
         logger.info(f"Daemon PID: {os.getpid()}")
-        asyncio.get_event_loop().run_until_complete(start_ml_worker(is_server, host, port))
+        asyncio.get_event_loop().run_until_complete(MLWorker(is_server, url, api_key).start())
 
 
 def get_log_path():
     return run_dir / "ml-worker.log"
 
 
 def tail(filename, n=100):
```

### Comparing `giskard-1.9.1/giskard/client/io_utils.py` & `giskard-2.0.0b1/giskard/client/io_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 
 def save_df(df: pd.DataFrame, format: str = "csv") -> bytes:
     pandas_version: int = int(re.sub(r"\D", "", pd.__version__))
     if format == "csv":
         csv_buffer = BytesIO()
         if pandas_version >= 120:
-            df.to_csv(csv_buffer, index=False, na_rep="_GSK_NA_")
+            df.to_csv(csv_buffer, index=False, na_rep="_GSK_NA_", escapechar="\\")
         else:
-            csv_buffer.write(df.to_csv(index=False, na_rep="_GSK_NA_").encode("utf-8"))
+            csv_buffer.write(df.to_csv(index=False, na_rep="_GSK_NA_", escapechar="\\").encode("utf-8"))
             csv_buffer.seek(0)
         return csv_buffer.getvalue()
     else:
         raise ValueError("Invalid method: {method}. Choose 'csv'.")
 
 
 def compress(data: bytes, method: Optional[str] = "zstd") -> bytes:
```

### Comparing `giskard-1.9.1/giskard/client/project.py` & `giskard-2.0.0b1/giskard/datasets/base/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,723 +1,612 @@
-import json
-from typing import Callable, Dict, Iterable, List, Optional, Union
+import inspect
+import logging
+import posixpath
+import tempfile
+import uuid
+from functools import cached_property
+from pathlib import Path
+from typing import Dict, Optional, List, Union
 
-import cloudpickle
 import numpy as np
+import pandas
 import pandas as pd
-import requests
+import yaml
+from pandas.api.types import is_list_like
 from pandas.api.types import is_numeric_dtype
-from pandas.api.types import is_string_dtype
-from requests_toolbelt.sessions import BaseUrlSession
+from xxhash import xxh3_128_hexdigest
+from zstandard import ZstdDecompressor
 
-from giskard.client.analytics_collector import GiskardAnalyticsCollector, anonymize
-from giskard.client.io_utils import compress, pickle_dumps, save_df
-from giskard.client.model import SupportedColumnType, SupportedModelTypes
-from giskard.client.python_utils import get_python_requirements, get_python_version, warning
+from giskard.client.giskard_client import GiskardClient
+from giskard.client.io_utils import save_df, compress
+from giskard.client.python_utils import warning
+from giskard.core.core import DatasetMeta, SupportedColumnTypes
+from giskard.core.validation import configured_validate_arguments
+from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction, SlicingFunctionType
+from giskard.ml_worker.testing.registry.transformation_function import (
+    TransformationFunction,
+    TransformationFunctionType,
+)
+from giskard.settings import settings
+from ..metadata.indexing import ColumnMetadataMixin
+from ...ml_worker.utils.file_utils import get_file_name
+
+SAMPLE_SIZE = 1000
+
+logger = logging.getLogger(__name__)
+
+
+class DataProcessor:
+    """
+    A class for processing tabular data using a pipeline of functions.
+
+    The pipeline consists of slicing functions that extract subsets of the data and transformation functions that modify it.
+    Slicing functions should take a pandas DataFrame as input and return a DataFrame, while transformation functions
+    should take a DataFrame and return a modified version of it.
+
+    Attributes:
+        pipeline (List[Union[SlicingFunction, TransformationFunction]]): a list of functions to be applied to the data,
+            in the order in which they were added.
+
+    Methods:
+        add_step(processor: Union[SlicingFunction, TransformationFunction]) -> DataProcessor:
+            Add a function to the processing pipeline, if it is not already the last step in the pipeline. Return self.
+
+        apply(dataset: Dataset, apply_only_last=False) -> Dataset:
+            Apply the processing pipeline to the given dataset. If apply_only_last is True, apply only the last function
+            in the pipeline. Return a new Dataset object containing the processed data.
+
+        __repr__() -> str:
+            Return a string representation of the DataProcessor object, showing the number of steps in its pipeline.
+    """
+
+    pipeline: List[Union[SlicingFunction, TransformationFunction]]
+
+    def __init__(self):
+        self.pipeline = []
+
+    @configured_validate_arguments
+    def add_step(self, processor: Union[SlicingFunction, TransformationFunction]):
+        if not len(self.pipeline) or self.pipeline[-1] != processor:
+            self.pipeline.append(processor)
+        return self
+
+    def apply(self, dataset: "Dataset", apply_only_last=False):
+        ds = dataset.copy()
+        is_slicing_only = True
+
+        while len(self.pipeline):
+            step = self.pipeline.pop(-1 if apply_only_last else 0)
+            is_slicing_only = is_slicing_only and isinstance(step, SlicingFunction)
+            df = step.execute(ds) if getattr(step, "needs_dataset", False) else step.execute(ds.df)
+            ds = Dataset(
+                df=df,
+                name=ds.name,
+                target=ds.target,
+                cat_columns=ds.cat_columns,
+                column_types=ds.column_types,
+                validation=False,
+            )
+
+            if apply_only_last:
+                break
+
+        if len(self.pipeline):
+            ds.data_processor = self
+
+        # If dataset had metadata, copy it to the new dataset
+        if is_slicing_only and hasattr(dataset, "column_meta"):
+            ds.load_metadata_from_instance(dataset.column_meta)
 
+        return ds
 
-class GiskardProject:
+    def __repr__(self) -> str:
+        return f"<DataProcessor ({len(self.pipeline)} steps)>"
+
+
+class Dataset(ColumnMetadataMixin):
+    """
+    A class for constructing and processing datasets.
+
+    Attributes:
+        df (pandas.DataFrame):
+            A `pandas.DataFrame` that contains the raw data (before all the pre-processing steps) and the actual
+            ground truth variable (target). `df` can contain more columns than the features of the model, such as the sample_id,
+            metadata, etc.
+        name (Optional[str]):
+            A string representing the name of the dataset (default None).
+        target (Optional[str]):
+            The column name in df corresponding to the actual target variable (ground truth).
+        cat_columns (Optional[List[str]]):
+            A list of strings representing the names of categorical columns (default None). If not provided,
+            the categorical columns will be automatically inferred.
+        column_types (Optional[Dict[str, str]]):
+            A dictionary of column names and their types (numeric, category or text) for all columns of df. If not provided,
+            the categorical columns will be automatically inferred.
+        data_processor (DataProcessor):
+            An instance of the `DataProcessor` class used for data processing.
+    """
+
+    name: Optional[str]
+    target: Optional[str]
+    column_types: Dict[str, str]
+    df: pd.DataFrame
+    id: uuid.UUID
+    data_processor: DataProcessor
+
+    @configured_validate_arguments
     def __init__(
-            self,
-            session: BaseUrlSession,
-            project_key: str,
-            project_id: int,
-            analytics: GiskardAnalyticsCollector = None,
+        self,
+        df: pd.DataFrame,
+        name: Optional[str] = None,
+        target: Optional[str] = None,
+        cat_columns: Optional[List[str]] = None,
+        column_types: Optional[Dict[str, str]] = None,
+        id: Optional[uuid.UUID] = None,
+        validation=True,
     ) -> None:
-        self.project_key = project_key
-        self._session = session
-        self.url = self._session.base_url.replace("/api/v2/", "")
-        self.analytics = analytics or GiskardAnalyticsCollector()
-        self.project_id = project_id
-
-    @staticmethod
-    def _serialize(
-            prediction_function: Callable[
-                [pd.DataFrame],
-                Iterable[Union[str, float, int]],
-            ]
-    ) -> bytes:
-        compressed_pickle: bytes = compress(pickle_dumps(prediction_function))
-        return compressed_pickle
-
-    def upload_model(
-            self,
-            prediction_function: Callable[[pd.DataFrame], Iterable[Union[str, float, int]]],
-            model_type: str,
-            feature_names: List[str] = None,
-            name: str = None,
-            validate_df: pd.DataFrame = None,
-            target: Optional[List[str]] = None,
-            classification_threshold: Optional[float] = None,
-            classification_labels: Optional[List[str]] = None,
-    ):
         """
-        Function to upload the Model to Giskard
+        Initializes a Dataset object.
+
         Args:
-            prediction_function:
-                The model you want to predict. It could be any Python function with the signature of
-                predict_proba for classification: It returns the classification probabilities for all
-                the classification labels
-                predict for regression : It returns the predicted values for regression models.
-            model_type:
-                "classification" for classification model
-                "regression" for regression model
-            feature_names:
-                 A list of the feature names of prediction_function. If provided, this list will be used to filter
-                 the dataframe's columns before applying the model. By default, the dataframe is used as-is, meaning
-                 that all of its columns are passed to the model.
-                 Some important remarks:
-                    - Make sure these features are contained in df
-                    - Make sure that prediction_function(df[feature_names]) does not return an error message
-                    - Make sure these features have the same order as the ones used in the
-                      pipeline of prediction_function.
-            name:
-                The name of the model you want to upload
-            validate_df:
-                Dataset used to validate the model
-            target:
-                The column name in validate_df corresponding to the actual target variable (ground truth).
-            classification_threshold:
-                The probability threshold in the case of a binary classification model
-            classification_labels:
-                The classification labels of your prediction when prediction_task="classification".
-                 Some important remarks:
-                    - If classification_labels is a list of n elements, make sure prediction_function is
-                     also returning probabilities
-                    - Make sure the labels have the same order as the output of prediction_function
-                    - Prefer using categorical values instead of numeric values in classification_labels
-        """
-        classification_labels, model = self._validate_model(
-            classification_labels,
-            classification_threshold,
-            feature_names,
-            model_type,
-            prediction_function,
-            target,
-            validate_df,
-        )
-        return self._post_model(
-            classification_labels, classification_threshold, feature_names, model, model_type, name
-        )
+            df (pd.DataFrame): The input dataset as a pandas DataFrame.
+            name (Optional[str]): The name of the dataset.
+            target (Optional[str]): The column name in df corresponding to the actual target variable (ground truth).
+            cat_columns (Optional[List[str]]): A list of column names that are categorical.
+            column_types (Optional[Dict[str, str]]): A dictionary mapping column names to their types.
+            id (Optional[uuid.UUID]): A UUID that uniquely identifies this dataset.
+
+        Notes:
+            if neither of cat_columns or column_types are provided. We infer heuristically the types of the columns.
+            See the _infer_column_types method.
+        """
+        if id is None:
+            self.id = uuid.uuid4()
+        else:
+            self.id = id
+        self.name = name
+        self.df = pd.DataFrame(df)
+        self.target = target
+
+        if validation:
+            from giskard.core.dataset_validation import validate_dtypes, validate_target
+
+            validate_dtypes(self)
+            validate_target(self)
+
+        self.column_dtypes = self.extract_column_dtypes(self.df)
+
+        # used in the inference of category columns
+        self.category_threshold = round(np.log10(len(self.df))) if len(self.df) >= 100 else 2
+        self.column_types = self._infer_column_types(column_types, cat_columns, validation)
+        if validation:
+            from giskard.core.dataset_validation import validate_column_types
+
+            validate_column_types(self)
+
+        if validation:
+            from giskard.core.dataset_validation import validate_column_categorization, validate_numeric_columns
+
+            validate_column_categorization(self)
+            validate_numeric_columns(self)
+
+        self.number_of_rows = len(self.df.index)
+        self.category_features = {
+            column: list(map(lambda x: str(x), self.df[column].dropna().unique()))
+            for column, column_type in self.column_types.items()
+            if column_type == 'category'
+        }
 
-    def _update_test_suite_params(
-            self, actual_ds_id, reference_ds_id, model_id, test_id=None, test_suite_id=None
-    ):
-        assert (
-                test_id is not None or test_suite_id is not None
-        ), "Either test_id or test_suite_id should be specified"
-        res = self._session.put(
-            "testing/suites/update_params",
-            json={
-                "testSuiteId": test_suite_id,
-                "testId": test_id,
-                "referenceDatasetId": reference_ds_id,
-                "actualDatasetId": actual_ds_id,
-                "modelId": model_id,
-            },
-        )
-        assert res.status_code == 200, "Failed to update test suite"
+        self.data_processor = DataProcessor()
 
-    def list_tests_in_suite(self, suite_id):
-        assert suite_id is not None, "suite_id should be specified"
-        res = self._session.get("testing/tests", params={"suiteId": suite_id}).json()
-        return [{"id": t["id"], "name": t["name"]} for t in res]
-
-    def list_test_suites(self):
-        res = self._session.get(f"testing/suites/{self.project_id}").json()
-        return [{"id": t["id"], "name": t["name"]} for t in res]
-
-    def _execution_dto_filter(self, answer_json):
-        res = {
-            "id": answer_json["testId"],
-            "name": answer_json["testName"],
-            "status": answer_json["status"],
-            "executionDate": answer_json["executionDate"],
-            "message": answer_json["message"],
-        }
-        if answer_json["status"] != "ERROR":
-            res["metric"] = answer_json["result"][0]["result"]["metric"]
-        return res
-
-    def execute_test(self, test_id, actual_ds_id=None, reference_ds_id=None, model_id=None):
-        self.analytics.track(
-            "execute_test",
-            {
-                "test_id": anonymize(test_id),
-                "actual_ds_id": anonymize(actual_ds_id),
-                "reference_ds_id": anonymize(reference_ds_id),
-                "model_id": anonymize(model_id),
-            },
-        )
-        assert test_id is not None, "test_id should be specified"
+        logger.info("Your 'pandas.DataFrame' is successfully wrapped by Giskard's 'Dataset' wrapper class.")
 
-        self._update_test_suite_params(actual_ds_id, reference_ds_id, model_id, test_id=test_id)
-        answer_json = self._session.post(f"testing/tests/{test_id}/run").json()
-        return self._execution_dto_filter(answer_json)
+    def add_slicing_function(self, slicing_function: SlicingFunction):
+        """
+        Adds a slicing function to the data processor's list of steps.
 
-    def execute_test_suite(
-            self, test_suite_id, actual_ds_id=None, reference_ds_id=None, model_id=None
-    ):
-        self.analytics.track(
-            "execute_test_suite",
-            {
-                "test_suite_id": anonymize(test_suite_id),
-                "actual_ds_id": anonymize(actual_ds_id),
-                "reference_ds_id": anonymize(reference_ds_id),
-                "model_id": anonymize(model_id),
-            },
-        )
-        assert test_suite_id is not None, "test_suite_id should be specified"
-        self._update_test_suite_params(
-            actual_ds_id,
-            reference_ds_id,
-            model_id,
-            test_suite_id=test_suite_id,
-        )
-        answer_json = self._session.post("testing/suites/execute", json={"suiteId": test_suite_id}).json()
-        return [self._execution_dto_filter(test) for test in answer_json]
+        Args:
+            slicing_function (SlicingFunction): A slicing function to add to the data processor.
+        """
+        self.data_processor.add_step(slicing_function)
+        return self
 
-    def _post_model(
-            self,
-            classification_labels,
-            classification_threshold,
-            feature_names,
-            model,
-            model_type,
-            name,
-    ):
-        requirements = get_python_requirements()
-        params = {
-            "name": name,
-            "projectKey": self.project_key,
-            "languageVersion": get_python_version(),
-            "modelType": model_type,
-            "threshold": classification_threshold,
-            "featureNames": feature_names,
-            "language": "PYTHON",
-            "classificationLabels": classification_labels,
-        }
-        files = [
-            ("metadata", (None, json.dumps(params), "application/json")),
-            ("modelFile", model),
-            ("requirementsFile", requirements),
-        ]
-        model_res = self._session.post("project/models/upload", data={}, files=files)
-        self.analytics.track(
-            "Upload Model",
-            {
-                "name": anonymize(name),
-                "projectKey": anonymize(self.project_key),
-                "languageVersion": get_python_version(),
-                "modelType": model_type,
-                "threshold": classification_threshold,
-                "featureNames": anonymize(feature_names),
-                "language": "PYTHON",
-                "classificationLabels": anonymize(classification_labels),
-            },
-        )
+    def add_transformation_function(self, transformation_function: TransformationFunction):
+        """
+        Add a transformation function to the data processor's list of steps.
 
-        model_id = model_res.json().get("id")
-        print(
-            f"Model successfully uploaded to project key '{self.project_key}' with ID = {model_id}. It is available at {self.url} "
-        )
-        return model_id
+        Args:
+            transformation_function (TransformationFunction): A transformation function to add to the data processor.
+        """
+        self.data_processor.add_step(transformation_function)
+        return self
 
-    def _validate_model(
-            self,
-            classification_labels,
-            classification_threshold,
-            feature_names,
-            model_type,
-            prediction_function,
-            target,
-            validate_df,
+    @cached_property
+    def row_hashes(self):
+        return pandas.Series(
+            map(
+                lambda row: xxh3_128_hexdigest(f"{', '.join(map(lambda x: repr(x), row))}".encode('utf-8')),
+                self.df.values,
+            ),
+            index=self.df.index,
+        )
+
+    @configured_validate_arguments
+    def slice(
+        self,
+        slicing_function: Union[SlicingFunction, SlicingFunctionType],
+        row_level: bool = True,
+        cell_level=False,
+        column_name: Optional[str] = None,
     ):
-        prediction_function = self._validate_model_is_pickleable(prediction_function)
-        transformed_pred_func = self.transform_prediction_function(
-            prediction_function, feature_names
-        )
-
-        self._validate_prediction_function(prediction_function)
-        self._validate_model_type(model_type)
-        classification_labels = self._validate_classification_labels(
-            classification_labels, model_type
-        )
+        """
+        Slice the dataset using the specified `slicing_function`.
 
-        if model_type == SupportedModelTypes.CLASSIFICATION.value:
-            self._validate_classification_threshold_label(
-                classification_labels, classification_threshold
-            )
+        Args:
+            slicing_function (Union[SlicingFunction, SlicingFunctionType]): A slicing function to apply.
+                If `slicing_function` is a callable, it will be wrapped in a `SlicingFunction` object
+                with `row_level` and `cell_level` as its arguments. The `SlicingFunction` object will be
+                used to slice the DataFrame. If `slicing_function` is a `SlicingFunction` object, it
+                will be used directly to slice the DataFrame.
+            row_level (bool): Whether the `slicing_function` should be applied to the rows (True) or
+                the whole dataframe (False). Defaults to True.
+            cell_level (bool): Whether the `slicing_function` should be applied to the cells (True) or
+                the whole dataframe (False). Defaults to False.
 
-        assert feature_names is None or isinstance(
-            feature_names, list
-        ), "Invalid feature_names parameter. Please provide the feature names as a list."
-
-        if validate_df is not None:
-            self._validate_is_pandasdataframe(validate_df)
-            self._validate_features(feature_names=feature_names, validate_df=validate_df)
-
-            if model_type == SupportedModelTypes.REGRESSION.value:
-                self._validate_model_execution(
-                    transformed_pred_func, validate_df, model_type, target=target
-                )
-            elif target is not None and model_type == SupportedModelTypes.CLASSIFICATION.value:
-                self._validate_target(target, validate_df.keys())
-                target_values = validate_df[target].unique()
-                self._validate_label_with_target(classification_labels, target_values, target)
-                self._validate_model_execution(
-                    transformed_pred_func,
-                    validate_df,
-                    model_type,
-                    classification_labels,
-                    target=target,
-                )
-            else:  # Classification with target = None
-                self._validate_model_execution(
-                    transformed_pred_func,
-                    validate_df,
-                    model_type,
-                    classification_labels,
-                    target=target,
-                )
+        Returns:
+            Dataset:
+                The sliced dataset as a `Dataset` object.
 
-        model = self._serialize(transformed_pred_func)
-        return classification_labels, model
+        Notes:
+            Raises TypeError: If `slicing_function` is not a callable or a `SlicingFunction` object.
+        """
+        if inspect.isfunction(slicing_function):
+            slicing_function = SlicingFunction(slicing_function, row_level=row_level, cell_level=cell_level)
 
-    def upload_df(
-            self,
-            df: pd.DataFrame,
-            column_types: Dict[str, str],
-            target: str = None,
-            name: str = None,
-    ) -> requests.Response:
+        if slicing_function.cell_level and column_name is not None:
+            slicing_function = slicing_function(column_name=column_name,
+                                                **{key: value for key, value in slicing_function.params.items() if
+                                                   key != 'column_name'})
+
+        return self.data_processor.add_step(slicing_function).apply(self, apply_only_last=True)
+
+    @configured_validate_arguments
+    def transform(
+        self,
+        transformation_function: Union[TransformationFunction, TransformationFunctionType],
+        row_level: bool = True,
+        cell_level=False,
+        column_name: Optional[str] = None,
+    ):
         """
-        Function to upload Dataset to Giskard
+        Transform the data in the current Dataset by applying a transformation function.
+
         Args:
-            df:
-                Dataset you want to upload
-            column_types:
-                A dictionary of column names and their types (numeric, category or text) for all columns of df.
-            target:
-                The column name in df corresponding to the actual target variable (ground truth).
-            name:
-                The name of the dataset you want to upload
+            transformation_function (Union[TransformationFunction, TransformationFunctionType]):
+                A transformation function to apply. If `transformation_function` is a callable, it will
+                be wrapped in a `TransformationFunction` object with `row_level` and `cell_level` as its
+                arguments. If `transformation_function` is a `TransformationFunction` object, it will be used
+                directly to transform the DataFrame.
+            row_level (bool): Whether the `transformation_function` should be applied to the rows (True) or
+                the whole dataframe (False). Defaults to True.
+            cell_level (bool): Whether the `slicing_function` should be applied to the cells (True) or
+                the whole dataframe (False). Defaults to False.
+
         Returns:
-                Response of the upload
-        """
-        data, raw_column_types = self._validate_and_compress_data(column_types, df, target)
-        result = self._post_data(column_types, data, name, raw_column_types, target)
-        return result
-
-    def _post_data(self, column_types, data, name, raw_column_types, target):
-        params = {
-            "projectKey": self.project_key,
-            "name": name,
-            "featureTypes": column_types,
-            "columnTypes": raw_column_types,
-            "target": target,
-        }
-        files = [("metadata", (None, json.dumps(params), "application/json")), ("file", data)]
-        result = self._session.post("project/data/upload", data={}, files=files)
-        ds_id = result.json().get("id")
-        print(
-            f"Dataset successfully uploaded to project key '{self.project_key}' with ID = {ds_id}. It is available at {self.url} "
-        )
-        self.analytics.track(
-            "Upload dataset",
-            {
-                "projectKey": anonymize(self.project_key),
-                "name": anonymize(name),
-                "featureTypes": anonymize(column_types),
-                "target": anonymize(target),
-            },
-        )
-        return ds_id
+            Dataset: A new Dataset object containing the transformed data.
 
-    def _validate_and_compress_data(self, column_types, df, target):
-        self._validate_is_pandasdataframe(df)
-        if target is not None:
-            self._validate_target(target, df.keys())
-        self.validate_columns_columntypes(df, column_types, target)
-        self._validate_column_types(column_types)
-        self._validate_column_categorization(df, column_types, target)
-        raw_column_types = df.dtypes.apply(lambda x: x.name).to_dict()
-        data = compress(save_df(df))
-        return data, raw_column_types
-
-    def upload_model_and_df(
-            self,
-            prediction_function: Callable[[pd.DataFrame], Iterable[Union[str, float, int]]],
-            model_type: str,
-            df: pd.DataFrame,
-            column_types: Dict[str, str],
-            feature_names: List[str] = None,
-            target: str = None,
-            model_name: str = None,
-            dataset_name: str = None,
-            classification_threshold: Optional[float] = None,
-            classification_labels: Optional[List[str]] = None,
-    ):
+        Notes:
+            Raises TypeError: If `transformation_function` is not a callable or a `TransformationFunction` object.
         """
-        Function to upload Dataset and model to Giskard
-        Args:
-            prediction_function:
-                The model you want to predict. It could be any Python function with the signature of
-                predict_proba for classification: It returns the classification probabilities for all
-                the classification labels
-                predict for regression : It returns the predicted values for regression models.
-            model_type:
-                "classification" for classification model
-                "regression" for regression model
-            df:
-                Dataset you want to upload
-            column_types:
-                A dictionary of column names and their types (numeric, category or text) for all columns of df.
-            feature_names:
-                 A list of the feature names of prediction_function. If provided, this list will be used to filter
-                 the dataframe's columns before applying the model. By default, the dataframe is used as-is, meaning
-                 that all of its columns are passed to the model.
-                 Some important remarks:
-                    - Make sure these features are contained in df
-                    - Make sure that prediction_function(df[feature_names]) does not return an error message
-                    - Make sure these features have the same order as the ones used
-                      in the pipeline of prediction_function.
-            target:
-                The column name in df corresponding to the actual target variable (ground truth).
-            model_name:
-                The name of the model you want to upload
-            dataset_name:
-                The name of the dataset you want to upload
-            classification_threshold:
-                The probability threshold in the case of a binary classification model
-            classification_labels:
-                The classification labels of your prediction when prediction_task="classification".
-                 Some important remarks:
-                    - If classification_labels is a list of n elements, make sure prediction_function is
-                     also returning probabilities
-                    - Make sure the labels have the same order as the output of prediction_function
-                    - Prefer using categorical values instead of numeric values in classification_labels
-        """
-        self.analytics.track("Upload model and dataset")
-        data, raw_column_types = self._validate_and_compress_data(column_types, df, target)
-        classification_labels, model = self._validate_model(
-            classification_labels,
-            classification_threshold,
-            feature_names,
-            model_type,
-            prediction_function,
-            target,
-            df,
-        )
-        data_res = self._post_data(column_types, data, dataset_name, raw_column_types, target)
-        model_res = self._post_model(
-            classification_labels,
-            classification_threshold,
-            feature_names,
-            model,
-            model_type,
-            model_name,
-        )
-        return model_res, data_res
 
-    @staticmethod
-    def _validate_model_type(model_type):
-        if model_type not in {task.value for task in SupportedModelTypes}:
-            raise ValueError(
-                f"Invalid model_type parameter: {model_type}. "
-                + f"Please choose one of {[task.value for task in SupportedModelTypes]}."
+        if inspect.isfunction(transformation_function):
+            transformation_function = TransformationFunction(
+                transformation_function, row_level=row_level, cell_level=cell_level
             )
 
-    @staticmethod
-    def _validate_column_types(column_types):
-        if column_types and isinstance(column_types, dict):
-            if not set(column_types.values()).issubset(
-                    set(column_type.value for column_type in SupportedColumnType)
-            ):
-                raise ValueError(
-                    "Invalid column_types parameter: "
-                    + f"Please choose types among {[column_type.value for column_type in SupportedColumnType]}."
-                )
-        else:
-            raise ValueError(
-                f"Invalid column_types parameter: {column_types}. Please specify non-empty dictionary."
-            )
+        if transformation_function.cell_level and column_name is not None:
+            transformation_function = transformation_function(column_name=column_name,
+                                                              **{key: value for key, value in
+                                                                 transformation_function.params.items() if
+                                                                 key != 'column_name'})
 
-    @staticmethod
-    def transform_prediction_function(prediction_function, feature_names=None):
-        if feature_names:
-            return lambda df: prediction_function(df[feature_names])
-        else:
-            return prediction_function
+        assert (
+            not transformation_function.cell_level or 'column_name' in transformation_function.params
+        ), "column_name should be provided for TransformationFunction at cell level"
+        return self.data_processor.add_step(transformation_function).apply(self, apply_only_last=True)
 
-    @staticmethod
-    def _validate_prediction_function(prediction_function):
-        if not callable(prediction_function):
-            raise ValueError(
-                f"Invalid prediction_function parameter: {prediction_function}. Please specify Python function."
-            )
+    def process(self):
+        """
+        Process the dataset by applying all the transformation and slicing functions in the defined order.
 
-    @staticmethod
-    def _validate_target(target, dataframe_keys):
-        if target not in dataframe_keys:
-            raise ValueError(
-                f"Invalid target parameter:"
-                f" {target} column is not present in the dataset with columns: {dataframe_keys}"
-            )
+        Returns:
+            The processed dataset after applying all the transformation and slicing functions.
+        """
+        return self.data_processor.apply(self)
 
-    @staticmethod
-    def _validate_features(feature_names=None, validate_df=None):
-        if (
-                feature_names is not None
-                and validate_df is not None
-                and not set(feature_names).issubset(set(validate_df.columns))
-        ):
-            missing_feature_names = set(feature_names) - set(validate_df.columns)
-            raise ValueError(
-                f"Value mentioned in  feature_names is  not available in validate_df: {missing_feature_names} "
-            )
+    def _infer_column_types(self, column_types: Optional[Dict[str, str]], cat_columns: Optional[List[str]],
+                            validation: bool = True):
+        """
+       This function infers the column types of a given DataFrame based on the number of unique values and column data types. It takes into account the provided column types and categorical columns. The inferred types can be 'text', 'numeric', or 'category'. The function also applies a logarithmic rule to determine the category threshold.
 
-    @staticmethod
-    def _validate_classification_threshold_label(
-            classification_labels, classification_threshold=None
-    ):
-        if classification_labels is None:
-            raise ValueError("Missing classification_labels parameter for classification model.")
-        if classification_threshold is not None and not isinstance(
-                classification_threshold, (int, float)
-        ):
-            raise ValueError(
-                f"Invalid classification_threshold parameter: {classification_threshold}. Please specify valid number."
-            )
+       Here's a summary of the function's logic:
 
-        if classification_threshold is not None:
-            if classification_threshold != 0.5:
-                if len(classification_labels) != 2:
-                    raise ValueError(
-                        f"Invalid classification_threshold parameter: {classification_threshold} value is applicable "
-                        f"only for binary classification. "
-                    )
+       1. If no column types are provided, initialize an empty dictionary.
+       2. Determine the columns in the DataFrame, excluding the target column if it exists.
+       3. If categorical columns are specified, prioritize them over the provided column types and mark them as 'category'.
+       4. Check for any unknown columns in the provided column types and remove them from the dictionary.
+       5. If there are no missing columns, remove the target column (if present) from the column types dictionary.
+       6. Calculate the number of unique values in each missing column.
+       7. For each missing column:
 
-    @staticmethod
-    def _validate_label_with_target(classification_labels, target_values=None, target_name=None):
-        if target_values is not None:
-            if not is_string_dtype(target_values):
-                print(
-                    'Hint: "Your target variable values are numeric. '
-                    "It is recommended to have Human readable string as your target values "
-                    'to make results more understandable in Giskard."'
-                )
+          - If the number of unique values is less than or equal to the category threshold, categorize it as 'category'.
+          - Otherwise, attempt to convert the column to numeric using `pd.to_numeric` and categorize it as 'numeric'.
+          - If the column does not have the expected numeric data type and validation is enabled, issue a warning message.
+          - If conversion to numeric raises a ValueError, categorize the column as 'text'.
+       8. Return the column types dictionary.
 
-            target_values = (
-                target_values
-                if is_string_dtype(target_values)
-                else [str(label) for label in target_values]
-            )
-            if not set(target_values).issubset(set(classification_labels)):
-                invalid_target_values = set(target_values) - set(classification_labels)
+       The logarithmic rule is used to calculate the category threshold. The formula is: `category_threshold = round(np.log10(len(self.df))) if len(self.df) >= 100 else 2`. This means that if the length of the DataFrame is greater than or equal to 100, the category threshold is set to the rounded value of the base-10 logarithm of the DataFrame length. Otherwise, the category threshold is set to 2. The logarithmic rule helps in dynamically adjusting the category threshold based on the size of the DataFrame.
+
+       Returns:
+          dict: A dictionary that maps column names to their inferred types, one of 'text', 'numeric', or 'category'.
+        """
+        if not column_types:
+            column_types = {}
+        df_columns = set([col for col in self.columns if col != self.target]) if self.target else set(self.columns)
+
+        # priority of cat_columns over column_types (for categorical columns)
+        if cat_columns:
+            if not set(cat_columns).issubset(df_columns):
                 raise ValueError(
-                    f"Values in {target_name} column are not declared in "
-                    f"classification_labels parameter: {invalid_target_values}"
+                    "The provided 'cat_columns' are not all part of your dataset 'columns'. "
+                    "Please make sure that `cat_columns` refers to existing columns in your dataset."
                 )
+            for cat_col in cat_columns:
+                if cat_col != self.target:
+                    column_types[cat_col] = SupportedColumnTypes.CATEGORY.value
+
+        given_columns = set(column_types.keys())
+        unknown_columns = given_columns - df_columns
+        missing_columns = df_columns - given_columns
 
-    @staticmethod
-    def _validate_classification_labels(classification_labels, model_type):
-        res = None
-        if model_type == SupportedModelTypes.CLASSIFICATION.value:
-            if classification_labels is not None and isinstance(classification_labels, Iterable):  # type: ignore
-                if len(classification_labels) > 1:
-                    res: Optional[List[str]] = [str(label) for label in classification_labels]
-                else:
-                    raise ValueError(
-                        f"Invalid classification_labels parameter: {classification_labels}. "
-                        f"Please specify more than 1 label."
+        if unknown_columns:
+            warning(
+                f"The provided keys {list(unknown_columns)} in 'column_types' are not part of your dataset "
+                "'columns'. Please make sure that the column names in `column_types` refers to existing "
+                "columns in your dataset."
+            )
+            [column_types.pop(i) for i in unknown_columns]
+
+        if not missing_columns:
+            column_types.pop(self.target, None)  # no need for target type
+            return column_types
+
+        nuniques = self.df.nunique()
+        for col in missing_columns:
+            if col == self.target:
+                continue
+            if nuniques[col] <= self.category_threshold:
+                column_types[col] = SupportedColumnTypes.CATEGORY.value
+                continue
+            # inference of text and numeric columns
+            try:
+                pd.to_numeric(self.df[col])
+                column_types[col] = SupportedColumnTypes.NUMERIC.value
+                if not is_numeric_dtype(self.df[col]) and validation:
+                    warning(
+                        f"The column {col} is declared as numeric but has '{str(self.df[col].dtype)}' as data type. "
+                        "To avoid potential future issues, make sure to cast this column to the correct data type."
                     )
-            else:
-                raise ValueError(
-                    f"Invalid classification_labels parameter: {classification_labels}. "
-                    f"Please specify valid list of strings."
-                )
-        if model_type == SupportedModelTypes.REGRESSION.value and classification_labels is not None:
-            warning("'classification_labels' parameter is ignored for regression model")
-            res = None
-        return res
-
-    def _validate_model_execution(
-            self,
-            prediction_function,
-            df: pd.DataFrame,
-            model_type,
-            classification_labels=None,
-            target=None,
-    ) -> None:
-        if target is not None and target in df.columns:
-            df = df.drop(target, axis=1)
-        try:
-            prediction_function(df.head(1))
-        except Exception:
-            raise ValueError(
-                "Invalid prediction_function input.\n"
-                "Please make sure that prediction_function(df.head(1)) does not return an error "
-                "message before uploading in Giskard"
-            )
-        try:
-            prediction = prediction_function(df)
-        except Exception:
-            raise ValueError(
-                "Invalid prediction_function input.\n"
-                "Please make sure that prediction_function(df[feature_names]) does not return an error "
-                "message before uploading in Giskard"
-            )
-        min_num_rows = min(len(df), 5)
-        GiskardProject._validate_deterministic_model(
-            df.head(min_num_rows), prediction[:min_num_rows], prediction_function
-        )
-        GiskardProject._validate_prediction_output(df, model_type, prediction)
-        if model_type == SupportedModelTypes.CLASSIFICATION.value:
-            GiskardProject._validate_classification_prediction(classification_labels, prediction)
 
-    @staticmethod
-    def _validate_prediction_output(df: pd.DataFrame, model_type, prediction):
-        assert len(df) == len(prediction), (
-            f"Number of rows ({len(df)}) of dataset provided does not match with the "
-            f"number of rows ({len(prediction)}) of prediction_function output"
-        )
-        if isinstance(prediction, np.ndarray) or isinstance(prediction, list):
-            if model_type == SupportedModelTypes.CLASSIFICATION.value:
-                if not any(isinstance(y, (np.floating, float)) for x in prediction for y in x):
-                    raise ValueError("Model prediction should return float values ")
-            if model_type == SupportedModelTypes.REGRESSION.value:
-                if not any(isinstance(x, (np.floating, float)) for x in prediction):
-                    raise ValueError("Model prediction should return float values ")
-        else:
-            raise ValueError("Model should return numpy array or a list")
+            except ValueError:
+                column_types[col] = SupportedColumnTypes.TEXT.value
 
-    @staticmethod
-    def _validate_classification_prediction(classification_labels, prediction):
-        if not np.all(np.logical_and(prediction >= 0, prediction <= 1)):
-            warning(
-                "Output of the prediction_function returns values out of range [0,1]. "
-                "The output of Multiclass and Binary classifications should be within the range [0,1]"
-            )
-        if not np.all(np.isclose(np.sum(prediction, axis=1), 1, atol=0.0000001)):
-            warning(
-                "Sum of output values of prediction_function is not equal to 1."
-                " For Multiclass and Binary classifications, the sum of probabilities should be 1"
-            )
-        if prediction.shape[1] != len(classification_labels):
-            raise ValueError(
-                "Prediction output label shape and classification_labels shape do not match"
-            )
+        return column_types
 
     @staticmethod
-    def validate_columns_columntypes(df: pd.DataFrame, feature_types, target) -> pd.DataFrame:
-        columns_with_types = set(feature_types.keys())
+    def extract_column_dtypes(df):
+        """
+        Extracts the column data types from a pandas DataFrame.
+
+        Args:
+            df (pandas.DataFrame): The input DataFrame.
 
-        if target in df.columns:
-            df = df.drop(target, axis=1)
+        Returns:
+            dict: A dictionary where the keys are the column names and the values are the corresponding data types as strings.
+        """
+        return df.dtypes.apply(lambda x: x.name).to_dict()
 
-        df_columns = set(df.columns)
-        columns_with_types.discard(target)
+    def upload(self, client: GiskardClient, project_key: str):
+        """
+        Uploads the dataset to the specified Giskard project.
 
-        if not columns_with_types.issubset(df_columns):
-            missing_columns = columns_with_types - df_columns
-            raise ValueError(
-                f"Missing columns in dataframe according to column_types: {missing_columns}"
-            )
-        elif not df_columns.issubset(columns_with_types):
-            missing_columns = df_columns - columns_with_types
-            if missing_columns:
-                raise ValueError(
-                    f"Invalid column_types parameter: Please declare the type for "
-                    f"{missing_columns} columns"
-                )
+        Args:
+            client: A GiskardClient instance for connecting to the Giskard API.
+            project_key (str): The key of the project to upload the dataset to.
 
-        pandas_inferred_column_types = df.dtypes.to_dict()
-        for column, dtype in pandas_inferred_column_types.items():
-            if feature_types.get(column) == SupportedColumnType.NUMERIC.value and dtype == "object":
-                try:
-                    df[column] = df[column].astype(float)
-                except Exception as e:
-                    raise ValueError(f"Failed to convert column '{column}' to float") from e
-            return df
+        Returns:
+            str: The ID of the uploaded dataset.
+        """
+        dataset_id = str(self.id)
+
+        with tempfile.TemporaryDirectory(prefix="giskard-dataset-") as local_path:
+            original_size_bytes, compressed_size_bytes = self.save(Path(local_path), dataset_id)
+            client.log_artifacts(local_path, posixpath.join(project_key, "datasets", dataset_id))
+            client.save_dataset_meta(
+                project_key,
+                dataset_id,
+                self.meta,
+                original_size_bytes=original_size_bytes,
+                compressed_size_bytes=compressed_size_bytes,
+            )
+        return dataset_id
+
+    @property
+    def meta(self):
+        return DatasetMeta(
+            name=self.name,
+            target=self.target,
+            column_types=self.column_types,
+            column_dtypes=self.column_dtypes,
+            number_of_rows=self.number_of_rows,
+            category_features=self.category_features,
+        )
 
     @staticmethod
-    def _validate_column_categorization(df: pd.DataFrame, feature_types, target=None):
+    def cast_column_to_dtypes(df, column_dtypes):
+        current_types = df.dtypes.apply(lambda x: x.name).to_dict()
+        logger.info(f"Casting dataframe columns from {current_types} to {column_dtypes}")
+        if column_dtypes:
+            try:
+                df = df.astype(column_dtypes, errors='ignore')
+            except Exception as e:
+                raise ValueError("Failed to apply column types to dataset") from e
+        return df
+
+    @classmethod
+    def load(cls, local_path: str):
+        with open(local_path, "rb") as ds_stream:
+            return pd.read_csv(
+                ZstdDecompressor().stream_reader(ds_stream),
+                keep_default_na=False,
+                na_values=["_GSK_NA_"],
+            )
+
+    @classmethod
+    def download(cls, client: GiskardClient, project_key, dataset_id, sample: bool = False):
         """
-        Validates if features_types is declared accurately by verifying the number of unique values for each column
-        in feature_types
+        Downloads a dataset from a Giskard project and returns a Dataset object.
+        If the client is None, then the function assumes that it is running in an internal worker and looks for the dataset locally.
+
+        Args:
+            client (GiskardClient):
+                The GiskardClient instance to use for downloading the dataset.
+                If None, the function looks for the dataset locally.
+            project_key (str): The key of the Giskard project that the dataset belongs to.
+            dataset_id (str): The ID of the dataset to download.
+            sample (bool): Only open a sample of 1000 rows if True
+
+        Returns:
+            Dataset: A Dataset object that represents the downloaded dataset.
         """
-        nuniques = df.nunique()
-        nuniques_category = 2
-        nuniques_numeric = 100
-        nuniques_text = 1000
-        df = (
-            df.drop(target, axis=1)
-            if target is not None and target not in feature_types.keys()
-            else df
-        )
+        local_dir = settings.home_dir / settings.cache_dir / project_key / "datasets" / dataset_id
 
-        for column in df.columns:
-            if nuniques[column] <= nuniques_category and (
-                    feature_types[column] == SupportedColumnType.NUMERIC.value
-                    or feature_types[column] == SupportedColumnType.TEXT.value
-            ):
-                warning(
-                    f"Feature '{column}' is declared as '{feature_types[column]}' but has {nuniques[column]} (<= nuniques_category={nuniques_category}) distinct values. Are "
-                    f"you sure it is not a 'category' feature?"
-                )
-            elif (
-                    nuniques[column] > nuniques_text
-                    and is_string_dtype(df[column])
-                    and (
-                            feature_types[column] == SupportedColumnType.CATEGORY.value
-                            or feature_types[column] == SupportedColumnType.NUMERIC.value
-                    )
-            ):
-                warning(
-                    f"Feature '{column}' is declared as '{feature_types[column]}' but has {nuniques[column]} (> nuniques_text={nuniques_text}) distinct values. Are "
-                    f"you sure it is not a 'text' feature?"
-                )
-            elif (
-                    nuniques[column] > nuniques_numeric
-                    and is_numeric_dtype(df[column])
-                    and (
-                            feature_types[column] == SupportedColumnType.CATEGORY.value
-                            or feature_types[column] == SupportedColumnType.TEXT.value
-                    )
-            ):
-                warning(
-                    f"Feature '{column}' is declared as '{feature_types[column]}' but has {nuniques[column]} (> nuniques_numeric={nuniques_numeric}) distinct values. Are "
-                    f"you sure it is not a 'numeric' feature?"
+        if client is None:
+            # internal worker case, no token based http client
+            assert local_dir.exists(), f"Cannot find existing dataset {project_key}.{dataset_id}"
+            with open(Path(local_dir) / "giskard-dataset-meta.yaml") as f:
+                saved_meta = yaml.load(f, Loader=yaml.Loader)
+                meta = DatasetMeta(
+                    name=saved_meta["name"],
+                    target=saved_meta["target"],
+                    column_types=saved_meta["column_types"],
+                    column_dtypes=saved_meta["column_dtypes"],
+                    number_of_rows=saved_meta["number_of_rows"],
+                    category_features=saved_meta["category_features"],
                 )
+        else:
+            client.load_artifact(local_dir, posixpath.join(project_key, "datasets", dataset_id))
+            meta: DatasetMeta = client.load_dataset_meta(project_key, dataset_id)
 
-    @staticmethod
-    def _validate_is_pandasdataframe(df):
-        assert isinstance(df, pd.DataFrame), "Dataset provided is not a pandas dataframe"
+        df = cls.load(local_dir / get_file_name("data", "csv.zst", sample))
+        df = cls.cast_column_to_dtypes(df, meta.column_dtypes)
+        return cls(
+            df=df,
+            name=meta.name,
+            target=meta.target,
+            column_types=meta.column_types,
+            id=uuid.uuid4() if sample else uuid.UUID(dataset_id),
+        )
+
+    @staticmethod
+    def _cat_columns(meta):
+        return (
+            [fname for (fname, ftype) in meta.column_types.items() if ftype == SupportedColumnTypes.CATEGORY]
+            if meta.column_types
+            else None
+        )
+
+    @property
+    def cat_columns(self):
+        return self._cat_columns(self.meta)
+
+    def save(self, local_path: Path, dataset_id):
+        with open(local_path / "data.csv.zst", "wb") as f, open(local_path / "data.sample.csv.zst", "wb") as f_sample:
+            uncompressed_bytes = save_df(self.df)
+            compressed_bytes = compress(uncompressed_bytes)
+            f.write(compressed_bytes)
+            original_size_bytes, compressed_size_bytes = len(uncompressed_bytes), len(compressed_bytes)
+
+            uncompressed_bytes = save_df(self.df.sample(min(SAMPLE_SIZE, len(self.df.index))))
+            compressed_bytes = compress(uncompressed_bytes)
+            f_sample.write(compressed_bytes)
+
+            with open(Path(local_path) / "giskard-dataset-meta.yaml", "w") as meta_f:
+                yaml.dump(
+                    {
+                        "id": dataset_id,
+                        "name": self.meta.name,
+                        "target": self.meta.target,
+                        "column_types": self.meta.column_types,
+                        "column_dtypes": self.meta.column_dtypes,
+                        "original_size_bytes": original_size_bytes,
+                        "compressed_size_bytes": compressed_size_bytes,
+                        "number_of_rows": self.meta.number_of_rows,
+                        "category_features": self.meta.category_features,
+                    },
+                    meta_f,
+                    default_flow_style=False,
+                )
+            return original_size_bytes, compressed_size_bytes
+
+    @property
+    def columns(self):
+        return self.df.columns
+
+    def __len__(self):
+        return len(self.df)
+
+    def select_columns(self, columns=None, col_type=None):
+        columns = _cast_to_list_like(columns) if columns is not None else None
+        col_type = _cast_to_list_like(col_type) if col_type is not None else None
+
+        df = self.df.copy()
+
+        if columns is None and col_type is None:
+            # TODO: should probably copy
+            return self
+
+        # Filter by columns
+        if columns is not None:
+            df = df.loc[:, columns]
+
+        # Filter by type
+        if col_type is not None:
+            if not is_list_like(col_type):
+                col_type = [col_type]
+
+            columns = [col for col in df.columns if self.column_types[col] in col_type]
+            df = df.loc[:, columns]
+
+        return Dataset(
+            df=df,
+            target=self.target if self.target in df.columns else None,
+            column_types={key: val for key, val in self.column_types.items() if key in df.columns},
+            validation=False,
+        )
+
+    def copy(self):
+        dataset = Dataset(
+            df=self.df.copy(),
+            target=self.target,
+            column_types=self.column_types.copy(),
+            validation=False,
+        )
 
-    @staticmethod
-    def _validate_deterministic_model(sample_df, prev_prediction, prediction_function):
-        """
-        Asserts if the model is deterministic by asserting previous and current prediction on same data
-        """
-        new_prediction = prediction_function(sample_df)
+        if hasattr(self, "column_meta"):
+            dataset.load_metadata_from_instance(self.column_meta)
 
-        if not np.allclose(prev_prediction, new_prediction):
-            warning(
-                "Model is stochastic and not deterministic. Prediction function returns different results"
-                "after being invoked for the same data multiple times."
-            )
+        return dataset
 
-    @staticmethod
-    def _validate_model_is_pickleable(prediction_function):
-        """
-        Validates if the model can be pickled and un-pickled using cloud pickle
-        """
-        try:
-            pickled_model = cloudpickle.dumps(prediction_function)
-            unpickled_model = cloudpickle.loads(pickled_model)
-        except Exception:
-            raise ValueError("Unable to pickle or unpickle model on Giskard")
-        return unpickled_model
 
-    def __repr__(self) -> str:
-        return f"GiskardProject(project_key='{self.project_key}')"
+def _cast_to_list_like(object):
+    return object if is_list_like(object) else (object,)
```

### Comparing `giskard-1.9.1/giskard/client/python_utils.py` & `giskard-2.0.0b1/giskard/client/python_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-1.9.1/giskard/ml_worker/core/model_explanation.py` & `giskard-2.0.0b1/giskard/models/model_explanation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,94 @@
 import logging
-from itertools import groupby
-from typing import Callable, Dict, List, Any
-
-import eli5
 import numpy as np
 import pandas as pd
-import shap
-from eli5.lime import TextExplainer
+import warnings
+from itertools import groupby
+from typing import Callable, Dict, List, Any
 
-from giskard.ml_worker.core.giskard_dataset import GiskardDataset
-from giskard.ml_worker.core.model import GiskardModel
+from giskard.datasets.base import Dataset
 from giskard.ml_worker.utils.logging import timer
+from giskard.models.base import BaseModel
+
+warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
+import shap  # noqa
 
 logger = logging.getLogger(__name__)
 
 
 @timer()
-def explain(model: GiskardModel, dataset: GiskardDataset, input_data: Dict):
+def explain(model: BaseModel, dataset: Dataset, input_data: Dict):
     def prepare_df(df):
+        df = model.prepare_dataframe(df, column_dtypes=dataset.column_dtypes, target=dataset.target)
+        if dataset.target in df.columns:
+            prepared_ds = Dataset(df=df, target=dataset.target, column_types=dataset.column_types)
+        else:
+            prepared_ds = Dataset(df=df, column_types=dataset.column_types)
         prepared_df = model.prepare_dataframe(
-            GiskardDataset(
-                df=df,
-                target=dataset.target,
-                feature_types=dataset.feature_types,
-                column_types=dataset.column_types,
-            )
+            prepared_ds.df, column_dtypes=prepared_ds.column_dtypes, target=prepared_ds.target
         )
         columns_in_original_order = (
-            model.feature_names
-            if model.feature_names
+            model.meta.feature_names
+            if model.meta.feature_names
             else [c for c in dataset.df.columns if c in prepared_df.columns]
         )
         # Make sure column order is the same as in df
         return prepared_df[columns_in_original_order]
 
-    df = model.prepare_dataframe(dataset)
+    df = model.prepare_dataframe(dataset.df, column_dtypes=dataset.column_dtypes, target=dataset.target)
     feature_names = list(df.columns)
 
     input_df = prepare_df(pd.DataFrame([input_data]))
 
     def predict_array(array):
-        return model.prediction_function(prepare_df(pd.DataFrame(array, columns=list(df.columns))))
+        arr_df = pd.DataFrame(array, columns=list(df.columns))
+        return model.predict_df(prepare_df(arr_df))
 
-    example = background_example(df, dataset.feature_types)
+    example = background_example(df, dataset.column_types)
     kernel = shap.KernelExplainer(predict_array, example)
     shap_values = kernel.shap_values(input_df, silent=True)
 
-    if model.model_type == "regression":
-        explanation_chart_data = summary_shap_regression(
-            shap_values=shap_values, feature_names=feature_names
-        )
-    elif model.model_type == "classification":
+    if model.is_regression:
+        explanation_chart_data = summary_shap_regression(shap_values=shap_values, feature_names=feature_names)
+    elif model.is_classification:
         explanation_chart_data = summary_shap_classification(
             shap_values=shap_values,
             feature_names=feature_names,
-            class_names=model.classification_labels,
+            class_names=model.meta.classification_labels,
         )
     else:
-        raise ValueError(f"Prediction task is not supported: {model.model_type}")
+        raise ValueError(f"Prediction task is not supported: {model.meta.model_type}")
     return explanation_chart_data
 
 
 @timer()
-def explain_text(
-        model: GiskardModel,
-        input_df: pd.DataFrame,
-        text_column: str,
-        text_document: str,
-        n_samples: int,
-):
-    text_explainer = TextExplainer(random_state=42, n_samples=n_samples)
-    prediction_function = text_explanation_prediction_wrapper(
-        model.prediction_function, input_df, text_column
-    )
-    text_explain_attempts = 10
+def explain_text(model: BaseModel, input_df: pd.DataFrame, text_column: str, text_document: str, n_samples: int):
     try:
+        # eli5 doesn't work with scipy>=1.9: cannot import name 'itemfreq' from 'scipy.stats'
+        # In principle we should have the following dependency in pyproject.toml:
+        # "scipy>=1.7.3,<1.9"
+        # But in order to let people use the rest of Giskard features we let giskard be installed with more modern scipy
+        # and let it fail here
+
+        import eli5
+        from eli5.lime import TextExplainer
+        text_explainer = TextExplainer(random_state=42, n_samples=n_samples)
+        prediction_function = text_explanation_prediction_wrapper(model.predict_df, input_df, text_column)
+        text_explain_attempts = 10
         for i in range(text_explain_attempts):
             try:
                 text_explainer.fit(text_document, prediction_function)
                 break
             except ZeroDivisionError:
                 logger.warning(f"Failed to fit text explainer {i}")
 
-        text_explainer.show_prediction(target_names=model.classification_labels)
-        exp = text_explainer.explain_prediction(target_names=model.classification_labels)
+        text_explainer.show_prediction(target_names=model.meta.classification_labels)
+        exp = text_explainer.explain_prediction(target_names=model.meta.classification_labels)
         exp = eli5.formatters.html.prepare_weighted_spans(exp.targets)
         return get_list_words_weights(exp)
-
     except Exception as e:
         logger.exception(f"Failed to explain text: {text_document}", e)
         raise Exception("Failed to create text explanation") from e
 
 
 def get_list_words_weights(exp):
     list_words = []
@@ -108,67 +106,61 @@
             i += len(word)
         list_weights.append(current_weights)
     return (list_words, list_weights)
 
 
 def background_example(df: pd.DataFrame, input_types: Dict[str, str]) -> pd.DataFrame:
     example = df.mode(dropna=False).head(1)  # si plusieurs modes, on prend le premier
-    example.fillna("", inplace=True)
+    # example.fillna("", inplace=True)
     median = df.median()
     num_columns = [key for key in list(df.columns) if input_types.get(key) == "numeric"]
     for column in num_columns:
         example[column] = median[column]
     return example.astype(df.dtypes)
 
 
 def summary_shap_classification(
-        shap_values: List[np.ndarray],
-        feature_names: List[str],
-        class_names: List[str],
-        max_display: int = 5,
+    shap_values: List[np.ndarray],
+    feature_names: List[str],
+    class_names: List[str],
+    max_display: int = 5,
 ) -> Dict[str, Dict[str, Dict[str, float]]]:
     feature_order = np.argsort(np.sum(np.mean(np.abs(shap_values), axis=1), axis=0))
-    feature_order = feature_order[-min(max_display, len(feature_order)):]
+    feature_order = feature_order[-min(max_display, len(feature_order)) :]
     feature_inds = feature_order[:max_display]
     chart_data: Dict[str, Dict[Any, Any]] = {"explanations": {}}
     for i in range(len(shap_values)):
         global_shap_values = np.abs(shap_values[i]).mean(0)
         chart_data["explanations"][class_names[i]] = {
-            feature_names[feature_ind]: global_shap_values[feature_ind]
-            for feature_ind in feature_inds
+            feature_names[feature_ind]: global_shap_values[feature_ind] for feature_ind in feature_inds
         }
     return chart_data
 
 
 def summary_shap_regression(
-        shap_values: np.ndarray, feature_names: List[str], max_display: int = 5
+    shap_values: np.ndarray, feature_names: List[str], max_display: int = 5
 ) -> Dict[str, Dict[str, Dict[str, float]]]:
     max_display = min(max_display, shap_values.shape[1])
     feature_order = np.argsort(np.mean(np.abs(shap_values), axis=0))
     feature_order = feature_order[-max_display:]
     feature_inds = feature_order[:max_display]
     global_shap_values = np.abs(shap_values).mean(0)
 
     chart_data = {
         "explanations": {
-            "default": {
-                feature_names[feature_ind]: global_shap_values[feature_ind]
-                for feature_ind in feature_inds
-            }
+            "default": {feature_names[feature_ind]: global_shap_values[feature_ind] for feature_ind in feature_inds}
         }
     }
     return chart_data
 
 
 def text_explanation_prediction_wrapper(
-        prediction_function: Callable, input_example: pd.DataFrame, text_column: str
+    prediction_function: Callable, input_example: pd.DataFrame, text_column: str
 ) -> Callable:
     def text_predict(text_documents: List[str]):
         num_documents = len(text_documents)
 
-        df_with_text_documents = input_example.append(
-            [input_example] * (num_documents - 1), ignore_index=True
-        )
+        df_with_text_documents = input_example.append([input_example] * (num_documents - 1), ignore_index=True)
         df_with_text_documents[text_column] = pd.DataFrame(text_documents)
         return prediction_function(df_with_text_documents)
 
     return text_predict
```

### Comparing `giskard-1.9.1/giskard/ml_worker/generated/ml_worker_pb2.py` & `giskard-2.0.0b1/giskard/ml_worker/generated/ml_worker_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,87 +14,111 @@
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fml-worker.proto\x12\x06worker\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1bgoogle/protobuf/empty.proto\",\n\x13MLWorkerInfoRequest\x12\x15\n\rlist_packages\x18\x01 \x01(\x08\"\xe3\x02\n\x0cMLWorkerInfo\x12&\n\x08platform\x18\x01 \x01(\x0b\x32\x14.worker.PlatformInfo\x12\x13\n\x0binterpreter\x18\x02 \x01(\t\x12\x1b\n\x13interpreter_version\x18\x03 \x01(\t\x12G\n\x12installed_packages\x18\x04 \x03(\x0b\x32+.worker.MLWorkerInfo.InstalledPackagesEntry\x12\x1a\n\x12internal_grpc_port\x18\x05 \x01(\r\x12\x11\n\tis_remote\x18\x06 \x01(\x08\x12\x0b\n\x03pid\x18\x07 \x01(\r\x12\x1a\n\x12process_start_time\x18\x08 \x01(\x04\x12\x1e\n\x16giskard_client_version\x18\t \x01(\t\x1a\x38\n\x16InstalledPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x0cPlatformInfo\x12\x0f\n\x07machine\x18\x01 \x01(\t\x12\x0c\n\x04node\x18\x02 \x01(\t\x12\x11\n\tprocessor\x18\x03 \x01(\t\x12\x0f\n\x07release\x18\x04 \x01(\t\x12\x0e\n\x06system\x18\x05 \x01(\t\x12\x0f\n\x07version\x18\x06 \x01(\t\"n\n\x11\x46ileUploadRequest\x12.\n\x08metadata\x18\x01 \x01(\x0b\x32\x1a.worker.FileUploadMetadataH\x00\x12\x1e\n\x05\x63hunk\x18\x02 \x01(\x0b\x32\r.worker.ChunkH\x00\x42\t\n\x07request\"h\n\x12\x46ileUploadMetadata\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\tfile_type\x18\x02 \x01(\x0e\x32\x10.worker.FileType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0bproject_key\x18\x04 \x01(\t\"\x16\n\x07\x45\x63hoMsg\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\xd8\x01\n\x0e\x45xplainRequest\x12-\n\x05model\x18\x01 \x01(\x0b\x32\x1e.worker.SerializedGiskardModel\x12\x31\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32 .worker.SerializedGiskardDataset\x12\x34\n\x07\x63olumns\x18\x03 \x03(\x0b\x32#.worker.ExplainRequest.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xd0\x02\n\x12\x45xplainTextRequest\x12-\n\x05model\x18\x01 \x01(\x0b\x32\x1e.worker.SerializedGiskardModel\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\x12\x38\n\x07\x63olumns\x18\x03 \x03(\x0b\x32\'.worker.ExplainTextRequest.ColumnsEntry\x12\x43\n\rfeature_types\x18\x04 \x03(\x0b\x32,.worker.ExplainTextRequest.FeatureTypesEntry\x12\x11\n\tn_samples\x18\x05 \x01(\r\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x33\n\x11\x46\x65\x61tureTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb9\x02\n\x0f\x45xplainResponse\x12?\n\x0c\x65xplanations\x18\x01 \x03(\x0b\x32).worker.ExplainResponse.ExplanationsEntry\x1a\x8a\x01\n\x0b\x45xplanation\x12H\n\x0bper_feature\x18\x01 \x03(\x0b\x32\x33.worker.ExplainResponse.Explanation.PerFeatureEntry\x1a\x31\n\x0fPerFeatureEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1aX\n\x11\x45xplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.worker.ExplainResponse.Explanation:\x02\x38\x01\"\xe4\x01\n\x13\x45xplainTextResponse\x12\r\n\x05words\x18\x01 \x03(\t\x12\x39\n\x07weights\x18\x02 \x03(\x0b\x32(.worker.ExplainTextResponse.WeightsEntry\x1a$\n\x11WeightsPerFeature\x12\x0f\n\x07weights\x18\x01 \x03(\x02\x1a]\n\x0cWeightsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12<\n\x05value\x18\x02 \x01(\x0b\x32-.worker.ExplainTextResponse.WeightsPerFeature:\x02\x38\x01\"\x8d\x01\n\x1cRunModelForDataFrameResponse\x12*\n\x0f\x61ll_predictions\x18\x01 \x01(\x0b\x32\x11.worker.DataFrame\x12\x12\n\nprediction\x18\x02 \x03(\t\x12\x15\n\rprobabilities\x18\x03 \x03(\x02\x12\x16\n\x0eraw_prediction\x18\x04 \x03(\x02\"h\n\x07\x44\x61taRow\x12-\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x1c.worker.DataRow.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"*\n\tDataFrame\x12\x1d\n\x04rows\x18\x01 \x03(\x0b\x32\x0f.worker.DataRow\"\x85\x03\n\x1bRunModelForDataFrameRequest\x12-\n\x05model\x18\x01 \x01(\x0b\x32\x1e.worker.SerializedGiskardModel\x12$\n\tdataframe\x18\x02 \x01(\x0b\x32\x11.worker.DataFrame\x12\x0e\n\x06target\x18\x03 \x01(\t\x12L\n\rfeature_types\x18\x04 \x03(\x0b\x32\x35.worker.RunModelForDataFrameRequest.FeatureTypesEntry\x12J\n\x0c\x63olumn_types\x18\x05 \x03(\x0b\x32\x34.worker.RunModelForDataFrameRequest.ColumnTypesEntry\x1a\x33\n\x11\x46\x65\x61tureTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x32\n\x10\x43olumnTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"s\n\x0fRunModelRequest\x12-\n\x05model\x18\x01 \x01(\x0b\x32\x1e.worker.SerializedGiskardModel\x12\x31\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32 .worker.SerializedGiskardDataset\"?\n\x10RunModelResponse\x12\x13\n\x0bresults_csv\x18\x01 \x01(\t\x12\x16\n\x0e\x63\x61lculated_csv\x18\x02 \x01(\t\"N\n\x13RunAdHocTestRequest\x12\x0e\n\x06testId\x18\x01 \x01(\t\x12\'\n\targuments\x18\x02 \x03(\x0b\x32\x14.worker.TestArgument\"\xb1\x01\n\x0cTestArgument\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x05model\x18\x02 \x01(\x0b\x32\x1e.worker.SerializedGiskardModelH\x00\x12\x33\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32 .worker.SerializedGiskardDatasetH\x00\x12\x0f\n\x05\x66loat\x18\x04 \x01(\x02H\x00\x12\x10\n\x06string\x18\x05 \x01(\tH\x00\x42\n\n\x08\x61rgument\"\xba\x01\n\x0eRunTestRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12-\n\x05model\x18\x02 \x01(\x0b\x32\x1e.worker.SerializedGiskardModel\x12\x33\n\tactual_ds\x18\x03 \x01(\x0b\x32 .worker.SerializedGiskardDataset\x12\x36\n\x0creference_ds\x18\x04 \x01(\x0b\x32 .worker.SerializedGiskardDataset\"\xcf\x02\n\x18SerializedGiskardDataset\x12\x13\n\x0bproject_key\x18\x01 \x01(\t\x12\x11\n\tfile_name\x18\x02 \x01(\t\x12\x0e\n\x06target\x18\x03 \x01(\t\x12I\n\rfeature_types\x18\x04 \x03(\x0b\x32\x32.worker.SerializedGiskardDataset.FeatureTypesEntry\x12G\n\x0c\x63olumn_types\x18\x05 \x03(\x0b\x32\x31.worker.SerializedGiskardDataset.ColumnTypesEntry\x1a\x33\n\x11\x46\x65\x61tureTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x32\n\x10\x43olumnTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x1f\n\x0fRunTestResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\"9\n\x19Partial_unexpected_counts\x12\r\n\x05value\x18\x01 \x03(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"O\n\x15NamedSingleTestResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12(\n\x06result\x18\x02 \x01(\x0b\x32\x18.worker.SingleTestResult\"B\n\x0bTestMessage\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.worker.TestMessageType\x12\x0c\n\x04text\x18\x02 \x01(\t\"\x98\x06\n\x10SingleTestResult\x12\x0e\n\x06passed\x18\r \x01(\x08\x12%\n\x08messages\x18\x10 \x03(\x0b\x32\x13.worker.TestMessage\x12\x32\n\x05props\x18\x0e \x03(\x0b\x32#.worker.SingleTestResult.PropsEntry\x12\x0e\n\x06metric\x18\x0f \x01(\x02\x12\x32\n\rmissing_count\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x35\n\x0fmissing_percent\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x10unexpected_count\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x38\n\x12unexpected_percent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12>\n\x18unexpected_percent_total\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x43\n\x1dunexpected_percent_nonmissing\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12%\n\x1dpartial_unexpected_index_list\x18\t \x03(\r\x12\x44\n\x19partial_unexpected_counts\x18\n \x03(\x0b\x32!.worker.Partial_unexpected_counts\x12\x1d\n\x15unexpected_index_list\x18\x0c \x03(\r\x12\x11\n\toutput_df\x18\x12 \x01(\x0c\x12 \n\x18number_of_perturbed_rows\x18\x14 \x01(\r\x12\x1a\n\x12\x61\x63tual_slices_size\x18\x15 \x03(\r\x12\x1d\n\x15reference_slices_size\x18\x16 \x03(\r\x1a,\n\nPropsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"C\n\x11TestResultMessage\x12.\n\x07results\x18\x01 \x03(\x0b\x32\x1d.worker.NamedSingleTestResult\"\xbb\x01\n\x16SerializedGiskardModel\x12\x12\n\nmodel_type\x18\x02 \x01(\t\x12/\n\tthreshold\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x15\n\rfeature_names\x18\x04 \x03(\t\x12\x1d\n\x15\x63lassification_labels\x18\x05 \x03(\t\x12\x13\n\x0bproject_key\x18\x06 \x01(\t\x12\x11\n\tfile_name\x18\x07 \x01(\t\"\x18\n\x05\x43hunk\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\x0c\"0\n\x0cUploadStatus\x12 \n\x04\x63ode\x18\x01 \x01(\x0e\x32\x12.worker.StatusCode\"U\n\x14TestFunctionArgument\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08optional\x18\x03 \x01(\x08\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x04 \x01(\t\"\xef\x01\n\x0cTestFunction\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06module\x18\x03 \x01(\t\x12\x0b\n\x03\x64oc\x18\x04 \x01(\t\x12\x12\n\nmodule_doc\x18\x05 \x01(\t\x12\x36\n\targuments\x18\x06 \x03(\x0b\x32#.worker.TestFunction.ArgumentsEntry\x12\x0c\n\x04tags\x18\x07 \x03(\t\x1aN\n\x0e\x41rgumentsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.worker.TestFunctionArgument:\x02\x38\x01\"?\n\x14TestRegistryResponse\x12\'\n\tfunctions\x18\x01 \x03(\x0b\x32\x14.worker.TestFunction\"1\n\x11MLWorkerErrorInfo\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\r\n\x05stack\x18\x02 \x01(\t\"m\n\x14\x46ilterDatasetRequest\x12+\n\x04meta\x18\x01 \x01(\x0b\x32\x1d.worker.FilterDatasetMetadata\x12\x1b\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\r.worker.Chunk\x12\x0b\n\x03idx\x18\x03 \x01(\r\"\xb4\x01\n\x15\x46ilterDatasetMetadata\x12\x10\n\x08\x66unction\x18\x01 \x01(\t\x12\x0f\n\x07headers\x18\x02 \x01(\t\x12\x44\n\x0c\x63olumn_types\x18\x03 \x03(\x0b\x32..worker.FilterDatasetMetadata.ColumnTypesEntry\x1a\x32\n\x10\x43olumnTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"k\n\x15\x46ilterDatasetResponse\x12 \n\x04\x63ode\x18\x01 \x01(\x0e\x32\x12.worker.StatusCode\x12\x0b\n\x03idx\x18\x02 \x01(\r\x12\x0c\n\x04rows\x18\x03 \x03(\r\x12\x15\n\rerror_message\x18\x04 \x01(\t*\"\n\x08\x46ileType\x12\t\n\x05MODEL\x10\x00\x12\x0b\n\x07\x44\x41TASET\x10\x01*&\n\x0fTestMessageType\x12\t\n\x05\x45RROR\x10\x00\x12\x08\n\x04INFO\x10\x01*Q\n\nStatusCode\x12\x0b\n\x07Unknown\x10\x00\x12\x06\n\x02Ok\x10\x01\x12\n\n\x06\x46\x61iled\x10\x02\x12\r\n\tCacheMiss\x10\x03\x12\t\n\x05Ready\x10\x04\x12\x08\n\x04Next\x10\x05\x32\x8e\x06\n\x08MLWorker\x12>\n\x07getInfo\x12\x1b.worker.MLWorkerInfoRequest\x1a\x14.worker.MLWorkerInfo\"\x00\x12>\n\x07runTest\x12\x16.worker.RunTestRequest\x1a\x19.worker.TestResultMessage\"\x00\x12H\n\x0crunAdHocTest\x12\x1b.worker.RunAdHocTestRequest\x1a\x19.worker.TestResultMessage\"\x00\x12?\n\x08runModel\x12\x17.worker.RunModelRequest\x1a\x18.worker.RunModelResponse\"\x00\x12\x63\n\x14runModelForDataFrame\x12#.worker.RunModelForDataFrameRequest\x1a$.worker.RunModelForDataFrameResponse\"\x00\x12<\n\x07\x65xplain\x12\x16.worker.ExplainRequest\x1a\x17.worker.ExplainResponse\"\x00\x12H\n\x0b\x65xplainText\x12\x1a.worker.ExplainTextRequest\x1a\x1b.worker.ExplainTextResponse\"\x00\x12*\n\x04\x65\x63ho\x12\x0f.worker.EchoMsg\x1a\x0f.worker.EchoMsg\"\x00\x12?\n\x06upload\x12\x19.worker.FileUploadRequest\x1a\x14.worker.UploadStatus\"\x00(\x01\x30\x01\x12I\n\x0fgetTestRegistry\x12\x16.google.protobuf.Empty\x1a\x1c.worker.TestRegistryResponse\"\x00\x12R\n\rfilterDataset\x12\x1c.worker.FilterDatasetRequest\x1a\x1d.worker.FilterDatasetResponse\"\x00(\x01\x30\x01\x42(\n\x11\x61i.giskard.workerB\x0bWorkerProtoP\x01\xa2\x02\x03WRKb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fml-worker.proto\x12\x06worker\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1bgoogle/protobuf/empty.proto\",\n\x13MLWorkerInfoRequest\x12\x15\n\rlist_packages\x18\x01 \x01(\x08\"\xe6\x02\n\x0cMLWorkerInfo\x12&\n\x08platform\x18\x01 \x01(\x0b\x32\x14.worker.PlatformInfo\x12\x13\n\x0binterpreter\x18\x02 \x01(\t\x12\x1b\n\x13interpreter_version\x18\x03 \x01(\t\x12G\n\x12installed_packages\x18\x04 \x03(\x0b\x32+.worker.MLWorkerInfo.InstalledPackagesEntry\x12\x1d\n\x15internal_grpc_address\x18\x05 \x01(\t\x12\x11\n\tis_remote\x18\x06 \x01(\x08\x12\x0b\n\x03pid\x18\x07 \x01(\r\x12\x1a\n\x12process_start_time\x18\x08 \x01(\x04\x12\x1e\n\x16giskard_client_version\x18\t \x01(\t\x1a\x38\n\x16InstalledPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x0cPlatformInfo\x12\x0f\n\x07machine\x18\x01 \x01(\t\x12\x0c\n\x04node\x18\x02 \x01(\t\x12\x11\n\tprocessor\x18\x03 \x01(\t\x12\x0f\n\x07release\x18\x04 \x01(\t\x12\x0e\n\x06system\x18\x05 \x01(\t\x12\x0f\n\x07version\x18\x06 \x01(\t\"n\n\x11\x46ileUploadRequest\x12.\n\x08metadata\x18\x01 \x01(\x0b\x32\x1a.worker.FileUploadMetadataH\x00\x12\x1e\n\x05\x63hunk\x18\x02 \x01(\x0b\x32\r.worker.ChunkH\x00\x42\t\n\x07request\"h\n\x12\x46ileUploadMetadata\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\tfile_type\x18\x02 \x01(\x0e\x32\x10.worker.FileType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0bproject_key\x18\x04 \x01(\t\"\x16\n\x07\x45\x63hoMsg\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\xc0\x01\n\x0e\x45xplainRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12$\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x34\n\x07\x63olumns\x18\x03 \x03(\x0b\x32#.worker.ExplainRequest.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc2\x02\n\x12\x45xplainTextRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\x12\x38\n\x07\x63olumns\x18\x03 \x03(\x0b\x32\'.worker.ExplainTextRequest.ColumnsEntry\x12\x41\n\x0c\x63olumn_types\x18\x04 \x03(\x0b\x32+.worker.ExplainTextRequest.ColumnTypesEntry\x12\x11\n\tn_samples\x18\x05 \x01(\r\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x32\n\x10\x43olumnTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb9\x02\n\x0f\x45xplainResponse\x12?\n\x0c\x65xplanations\x18\x01 \x03(\x0b\x32).worker.ExplainResponse.ExplanationsEntry\x1a\x8a\x01\n\x0b\x45xplanation\x12H\n\x0bper_feature\x18\x01 \x03(\x0b\x32\x33.worker.ExplainResponse.Explanation.PerFeatureEntry\x1a\x31\n\x0fPerFeatureEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1aX\n\x11\x45xplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.worker.ExplainResponse.Explanation:\x02\x38\x01\"\xe4\x01\n\x13\x45xplainTextResponse\x12\r\n\x05words\x18\x01 \x03(\t\x12\x39\n\x07weights\x18\x02 \x03(\x0b\x32(.worker.ExplainTextResponse.WeightsEntry\x1a$\n\x11WeightsPerFeature\x12\x0f\n\x07weights\x18\x01 \x03(\x02\x1a]\n\x0cWeightsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12<\n\x05value\x18\x02 \x01(\x0b\x32-.worker.ExplainTextResponse.WeightsPerFeature:\x02\x38\x01\"\x8d\x01\n\x1cRunModelForDataFrameResponse\x12*\n\x0f\x61ll_predictions\x18\x01 \x01(\x0b\x32\x11.worker.DataFrame\x12\x12\n\nprediction\x18\x02 \x03(\t\x12\x15\n\rprobabilities\x18\x03 \x03(\x02\x12\x16\n\x0eraw_prediction\x18\x04 \x03(\x02\"h\n\x07\x44\x61taRow\x12-\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x1c.worker.DataRow.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"*\n\tDataFrame\x12\x1d\n\x04rows\x18\x01 \x03(\x0b\x32\x0f.worker.DataRow\"\xfa\x02\n\x1bRunModelForDataFrameRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12$\n\tdataframe\x18\x02 \x01(\x0b\x32\x11.worker.DataFrame\x12\x0e\n\x06target\x18\x03 \x01(\t\x12J\n\x0c\x63olumn_types\x18\x04 \x03(\x0b\x32\x34.worker.RunModelForDataFrameRequest.ColumnTypesEntry\x12L\n\rcolumn_dtypes\x18\x05 \x03(\x0b\x32\x35.worker.RunModelForDataFrameRequest.ColumnDtypesEntry\x1a\x32\n\x10\x43olumnTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x33\n\x11\x43olumnDtypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x86\x01\n\x0fRunModelRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12$\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x14\n\x0cinspectionId\x18\x03 \x01(\x04\x12\x13\n\x0bproject_key\x18\x04 \x01(\t\"?\n\x10RunModelResponse\x12\x13\n\x0bresults_csv\x18\x01 \x01(\t\x12\x16\n\x0e\x63\x61lculated_csv\x18\x02 \x01(\t\"P\n\x13RunAdHocTestRequest\x12\x10\n\x08testUuid\x18\x01 \x01(\t\x12\'\n\targuments\x18\x02 \x03(\x0b\x32\x14.worker.FuncArgument\"v\n\x18\x44\x61tasetProcessingRequest\x12$\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x34\n\tfunctions\x18\x02 \x03(\x0b\x32!.worker.DatasetProcessingFunction\"\xb7\x01\n\x19\x44\x61tasetProcessingFunction\x12.\n\x0fslicingFunction\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x35\n\x16transformationFunction\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\'\n\targuments\x18\x03 \x03(\x0b\x32\x14.worker.FuncArgumentB\n\n\x08\x66unction\"Z\n\x11SuiteTestArgument\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08testUuid\x18\x02 \x01(\t\x12\'\n\targuments\x18\x03 \x03(\x0b\x32\x14.worker.FuncArgument\"n\n\x13RunTestSuiteRequest\x12(\n\x05tests\x18\x01 \x03(\x0b\x32\x19.worker.SuiteTestArgument\x12-\n\x0fglobalArguments\x18\x02 \x03(\x0b\x32\x14.worker.FuncArgument\"\xe0\x02\n\x0c\x46uncArgument\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x05model\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12&\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x0f\n\x05\x66loat\x18\x04 \x01(\x02H\x00\x12\r\n\x03int\x18\x05 \x01(\x05H\x00\x12\r\n\x03str\x18\x06 \x01(\tH\x00\x12\x0e\n\x04\x62ool\x18\x07 \x01(\x08H\x00\x12.\n\x0fslicingFunction\x18\x08 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x35\n\x16transformationFunction\x18\t \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x10\n\x06kwargs\x18\n \x01(\tH\x00\x12\"\n\x04\x61rgs\x18\x0b \x03(\x0b\x32\x14.worker.FuncArgument\x12\x0c\n\x04none\x18\x0c \x01(\x08\x42\n\n\x08\x61rgument\"\x1f\n\x0fRunTestResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\"9\n\x19Partial_unexpected_counts\x12\r\n\x05value\x18\x01 \x03(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"S\n\x15NamedSingleTestResult\x12\x10\n\x08testUuid\x18\x01 \x01(\t\x12(\n\x06result\x18\x02 \x01(\x0b\x32\x18.worker.SingleTestResult\"R\n\x1aIdentifierSingleTestResult\x12\n\n\x02id\x18\x01 \x01(\x03\x12(\n\x06result\x18\x02 \x01(\x0b\x32\x18.worker.SingleTestResult\"B\n\x0bTestMessage\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.worker.TestMessageType\x12\x0c\n\x04text\x18\x02 \x01(\t\"\xe6\x04\n\x10SingleTestResult\x12\x0e\n\x06passed\x18\r \x01(\x08\x12%\n\x08messages\x18\x10 \x03(\x0b\x32\x13.worker.TestMessage\x12\x32\n\x05props\x18\x0e \x03(\x0b\x32#.worker.SingleTestResult.PropsEntry\x12\x0e\n\x06metric\x18\x0f \x01(\x02\x12\x15\n\rmissing_count\x18\x02 \x01(\x05\x12\x17\n\x0fmissing_percent\x18\x03 \x01(\x01\x12\x18\n\x10unexpected_count\x18\x04 \x01(\x05\x12\x1a\n\x12unexpected_percent\x18\x05 \x01(\x01\x12 \n\x18unexpected_percent_total\x18\x06 \x01(\x01\x12%\n\x1dunexpected_percent_nonmissing\x18\x07 \x01(\x01\x12%\n\x1dpartial_unexpected_index_list\x18\t \x03(\r\x12\x44\n\x19partial_unexpected_counts\x18\n \x03(\x0b\x32!.worker.Partial_unexpected_counts\x12\x1d\n\x15unexpected_index_list\x18\x0c \x03(\r\x12\x11\n\toutput_df\x18\x12 \x01(\x0c\x12 \n\x18number_of_perturbed_rows\x18\x14 \x01(\r\x12\x1a\n\x12\x61\x63tual_slices_size\x18\x15 \x03(\r\x12\x1d\n\x15reference_slices_size\x18\x16 \x03(\r\x1a,\n\nPropsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"C\n\x11TestResultMessage\x12.\n\x07results\x18\x01 \x03(\x0b\x32\x1d.worker.NamedSingleTestResult\"\x99\x01\n\x1e\x44\x61tasetProcessingResultMessage\x12\x11\n\tdatasetId\x18\x01 \x01(\t\x12\x11\n\ttotalRows\x18\x02 \x01(\r\x12\x14\n\x0c\x66ilteredRows\x18\x03 \x03(\r\x12;\n\rmodifications\x18\x04 \x03(\x0b\x32$.worker.DatasetRowModificationResult\"\xb3\x01\n\x1c\x44\x61tasetRowModificationResult\x12\r\n\x05rowId\x18\x01 \x01(\r\x12N\n\rmodifications\x18\x02 \x03(\x0b\x32\x37.worker.DatasetRowModificationResult.ModificationsEntry\x1a\x34\n\x12ModificationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"~\n\x16TestSuiteResultMessage\x12\x10\n\x08is_error\x18\x01 \x01(\x08\x12\x0f\n\x07is_pass\x18\x02 \x01(\x08\x12\x33\n\x07results\x18\x03 \x03(\x0b\x32\".worker.IdentifierSingleTestResult\x12\x0c\n\x04logs\x18\x04 \x01(\t\"N\n\x0b\x41rtifactRef\x12\x13\n\x0bproject_key\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\x12\x13\n\x06sample\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\t\n\x07_sample\"\x18\n\x05\x43hunk\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\x0c\"0\n\x0cUploadStatus\x12 \n\x04\x63ode\x18\x01 \x01(\x0e\x32\x12.worker.StatusCode\"1\n\x11MLWorkerErrorInfo\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\r\n\x05stack\x18\x02 \x01(\t\"\xa4\x01\n\nSuiteInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12*\n\nmodel_meta\x18\x03 \x01(\x0b\x32\x11.worker.ModelMetaH\x00\x88\x01\x01\x12.\n\x0c\x64\x61taset_meta\x18\x04 \x01(\x0b\x32\x13.worker.DatasetMetaH\x01\x88\x01\x01\x42\r\n\x0b_model_metaB\x0f\n\r_dataset_meta\"3\n\tModelMeta\x12\x17\n\nmodel_type\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_model_type\"-\n\x0b\x44\x61tasetMeta\x12\x13\n\x06target\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\t\n\x07_target\"S\n\x18GenerateTestSuiteRequest\x12\x13\n\x0bproject_key\x18\x01 \x01(\t\x12\"\n\x06inputs\x18\x02 \x03(\x0b\x32\x12.worker.SuiteInput\"A\n\x19GenerateTestSuiteResponse\x12$\n\x05tests\x18\x01 \x03(\x0b\x32\x15.worker.GeneratedTest\"N\n\rGeneratedTest\x12\x11\n\ttest_uuid\x18\x01 \x01(\t\x12*\n\x06inputs\x18\x02 \x03(\x0b\x32\x1a.worker.GeneratedTestInput\"C\n\x12GeneratedTestInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x10\n\x08is_alias\x18\x03 \x01(\x08\"\xb3\x03\n\x0f\x43\x61talogResponse\x12\x31\n\x05tests\x18\x01 \x03(\x0b\x32\".worker.CatalogResponse.TestsEntry\x12\x33\n\x06slices\x18\x02 \x03(\x0b\x32#.worker.CatalogResponse.SlicesEntry\x12\x45\n\x0ftransformations\x18\x03 \x03(\x0b\x32,.worker.CatalogResponse.TransformationsEntry\x1a\x42\n\nTestsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.worker.FunctionMeta:\x02\x38\x01\x1aQ\n\x0bSlicesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".worker.DatasetProcessFunctionMeta:\x02\x38\x01\x1aZ\n\x14TransformationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".worker.DatasetProcessFunctionMeta:\x02\x38\x01\"\xd6\x01\n\x0c\x46unctionMeta\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x0e\n\x06module\x18\x05 \x01(\t\x12\x0b\n\x03\x64oc\x18\x06 \x01(\t\x12\x11\n\tmoduleDoc\x18\x07 \x01(\t\x12*\n\x04\x61rgs\x18\x08 \x03(\x0b\x32\x1c.worker.TestFunctionArgument\x12\x0c\n\x04tags\x18\t \x03(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\"\xb4\x02\n\x1a\x44\x61tasetProcessFunctionMeta\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x0e\n\x06module\x18\x05 \x01(\t\x12\x0b\n\x03\x64oc\x18\x06 \x01(\t\x12\x11\n\tmoduleDoc\x18\x07 \x01(\t\x12*\n\x04\x61rgs\x18\x08 \x03(\x0b\x32\x1c.worker.TestFunctionArgument\x12\x0c\n\x04tags\x18\t \x03(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x11\n\tcellLevel\x18\x0c \x01(\x08\x12\x17\n\ncolumnType\x18\r \x01(\tH\x00\x88\x01\x01\x12\x13\n\x0bprocessType\x18\x0e \x01(\tB\r\n\x0b_columnType\"g\n\x14TestFunctionArgument\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08optional\x18\x03 \x01(\x08\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x04 \x01(\t\x12\x10\n\x08\x61rgOrder\x18\x05 \x01(\r\"\x8c\x01\n\x10\x43omparisonClause\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12/\n\x0f\x63omparison_type\x18\x02 \x01(\x0e\x32\x16.worker.ComparisonType\x12\x14\n\x0c\x63olumn_dtype\x18\x03 \x01(\t\x12\x12\n\x05value\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_value\"V\n\x1eGenerateQueryBasedSliceRequest\x12\x34\n\x12\x63omparison_clauses\x18\x01 \x03(\x0b\x32\x18.worker.ComparisonClause\"-\n\x1fGenerateQueryBasedSliceResponse\x12\n\n\x02id\x18\x01 \x01(\t*\"\n\x08\x46ileType\x12\t\n\x05MODEL\x10\x00\x12\x0b\n\x07\x44\x41TASET\x10\x01*&\n\x0fTestMessageType\x12\t\n\x05\x45RROR\x10\x00\x12\x08\n\x04INFO\x10\x01*Q\n\nStatusCode\x12\x0b\n\x07Unknown\x10\x00\x12\x06\n\x02Ok\x10\x01\x12\n\n\x06\x46\x61iled\x10\x02\x12\r\n\tCacheMiss\x10\x03\x12\t\n\x05Ready\x10\x04\x12\x08\n\x04Next\x10\x05*\x89\x01\n\x0e\x43omparisonType\x12\x06\n\x02IS\x10\x00\x12\n\n\x06IS_NOT\x10\x01\x12\x0c\n\x08\x43ONTAINS\x10\x02\x12\x15\n\x11\x44OES_NOT_CONTAINS\x10\x03\x12\x0f\n\x0bSTARTS_WITH\x10\x04\x12\r\n\tENDS_WITH\x10\x05\x12\x0c\n\x08IS_EMPTY\x10\x06\x12\x10\n\x0cIS_NOT_EMPTY\x10\x07\x32\xf1\x07\n\x08MLWorker\x12>\n\x07getInfo\x12\x1b.worker.MLWorkerInfoRequest\x1a\x14.worker.MLWorkerInfo\"\x00\x12H\n\x0crunAdHocTest\x12\x1b.worker.RunAdHocTestRequest\x1a\x19.worker.TestResultMessage\"\x00\x12_\n\x11\x64\x61tasetProcessing\x12 .worker.DatasetProcessingRequest\x1a&.worker.DatasetProcessingResultMessage\"\x00\x12M\n\x0crunTestSuite\x12\x1b.worker.RunTestSuiteRequest\x1a\x1e.worker.TestSuiteResultMessage\"\x00\x12=\n\x08runModel\x12\x17.worker.RunModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x63\n\x14runModelForDataFrame\x12#.worker.RunModelForDataFrameRequest\x1a$.worker.RunModelForDataFrameResponse\"\x00\x12<\n\x07\x65xplain\x12\x16.worker.ExplainRequest\x1a\x17.worker.ExplainResponse\"\x00\x12H\n\x0b\x65xplainText\x12\x1a.worker.ExplainTextRequest\x1a\x1b.worker.ExplainTextResponse\"\x00\x12*\n\x04\x65\x63ho\x12\x0f.worker.EchoMsg\x1a\x0f.worker.EchoMsg\"\x00\x12Z\n\x11generateTestSuite\x12 .worker.GenerateTestSuiteRequest\x1a!.worker.GenerateTestSuiteResponse\"\x00\x12>\n\nstopWorker\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\ngetCatalog\x12\x16.google.protobuf.Empty\x1a\x17.worker.CatalogResponse\"\x00\x12v\n!generateQueryBasedSlicingFunction\x12&.worker.GenerateQueryBasedSliceRequest\x1a\'.worker.GenerateQueryBasedSliceResponse\"\x00\x42(\n\x11\x61i.giskard.workerB\x0bWorkerProtoP\x01\xa2\x02\x03WRKb\x06proto3')
 
 _FILETYPE = DESCRIPTOR.enum_types_by_name['FileType']
 FileType = enum_type_wrapper.EnumTypeWrapper(_FILETYPE)
 _TESTMESSAGETYPE = DESCRIPTOR.enum_types_by_name['TestMessageType']
 TestMessageType = enum_type_wrapper.EnumTypeWrapper(_TESTMESSAGETYPE)
 _STATUSCODE = DESCRIPTOR.enum_types_by_name['StatusCode']
 StatusCode = enum_type_wrapper.EnumTypeWrapper(_STATUSCODE)
+_COMPARISONTYPE = DESCRIPTOR.enum_types_by_name['ComparisonType']
+ComparisonType = enum_type_wrapper.EnumTypeWrapper(_COMPARISONTYPE)
 MODEL = 0
 DATASET = 1
 ERROR = 0
 INFO = 1
 Unknown = 0
 Ok = 1
 Failed = 2
 CacheMiss = 3
 Ready = 4
 Next = 5
+IS = 0
+IS_NOT = 1
+CONTAINS = 2
+DOES_NOT_CONTAINS = 3
+STARTS_WITH = 4
+ENDS_WITH = 5
+IS_EMPTY = 6
+IS_NOT_EMPTY = 7
 
 
 _MLWORKERINFOREQUEST = DESCRIPTOR.message_types_by_name['MLWorkerInfoRequest']
 _MLWORKERINFO = DESCRIPTOR.message_types_by_name['MLWorkerInfo']
 _MLWORKERINFO_INSTALLEDPACKAGESENTRY = _MLWORKERINFO.nested_types_by_name['InstalledPackagesEntry']
 _PLATFORMINFO = DESCRIPTOR.message_types_by_name['PlatformInfo']
 _FILEUPLOADREQUEST = DESCRIPTOR.message_types_by_name['FileUploadRequest']
 _FILEUPLOADMETADATA = DESCRIPTOR.message_types_by_name['FileUploadMetadata']
 _ECHOMSG = DESCRIPTOR.message_types_by_name['EchoMsg']
 _EXPLAINREQUEST = DESCRIPTOR.message_types_by_name['ExplainRequest']
 _EXPLAINREQUEST_COLUMNSENTRY = _EXPLAINREQUEST.nested_types_by_name['ColumnsEntry']
 _EXPLAINTEXTREQUEST = DESCRIPTOR.message_types_by_name['ExplainTextRequest']
 _EXPLAINTEXTREQUEST_COLUMNSENTRY = _EXPLAINTEXTREQUEST.nested_types_by_name['ColumnsEntry']
-_EXPLAINTEXTREQUEST_FEATURETYPESENTRY = _EXPLAINTEXTREQUEST.nested_types_by_name['FeatureTypesEntry']
+_EXPLAINTEXTREQUEST_COLUMNTYPESENTRY = _EXPLAINTEXTREQUEST.nested_types_by_name['ColumnTypesEntry']
 _EXPLAINRESPONSE = DESCRIPTOR.message_types_by_name['ExplainResponse']
 _EXPLAINRESPONSE_EXPLANATION = _EXPLAINRESPONSE.nested_types_by_name['Explanation']
 _EXPLAINRESPONSE_EXPLANATION_PERFEATUREENTRY = _EXPLAINRESPONSE_EXPLANATION.nested_types_by_name['PerFeatureEntry']
 _EXPLAINRESPONSE_EXPLANATIONSENTRY = _EXPLAINRESPONSE.nested_types_by_name['ExplanationsEntry']
 _EXPLAINTEXTRESPONSE = DESCRIPTOR.message_types_by_name['ExplainTextResponse']
 _EXPLAINTEXTRESPONSE_WEIGHTSPERFEATURE = _EXPLAINTEXTRESPONSE.nested_types_by_name['WeightsPerFeature']
 _EXPLAINTEXTRESPONSE_WEIGHTSENTRY = _EXPLAINTEXTRESPONSE.nested_types_by_name['WeightsEntry']
 _RUNMODELFORDATAFRAMERESPONSE = DESCRIPTOR.message_types_by_name['RunModelForDataFrameResponse']
 _DATAROW = DESCRIPTOR.message_types_by_name['DataRow']
 _DATAROW_COLUMNSENTRY = _DATAROW.nested_types_by_name['ColumnsEntry']
 _DATAFRAME = DESCRIPTOR.message_types_by_name['DataFrame']
 _RUNMODELFORDATAFRAMEREQUEST = DESCRIPTOR.message_types_by_name['RunModelForDataFrameRequest']
-_RUNMODELFORDATAFRAMEREQUEST_FEATURETYPESENTRY = _RUNMODELFORDATAFRAMEREQUEST.nested_types_by_name['FeatureTypesEntry']
 _RUNMODELFORDATAFRAMEREQUEST_COLUMNTYPESENTRY = _RUNMODELFORDATAFRAMEREQUEST.nested_types_by_name['ColumnTypesEntry']
+_RUNMODELFORDATAFRAMEREQUEST_COLUMNDTYPESENTRY = _RUNMODELFORDATAFRAMEREQUEST.nested_types_by_name['ColumnDtypesEntry']
 _RUNMODELREQUEST = DESCRIPTOR.message_types_by_name['RunModelRequest']
 _RUNMODELRESPONSE = DESCRIPTOR.message_types_by_name['RunModelResponse']
 _RUNADHOCTESTREQUEST = DESCRIPTOR.message_types_by_name['RunAdHocTestRequest']
-_TESTARGUMENT = DESCRIPTOR.message_types_by_name['TestArgument']
-_RUNTESTREQUEST = DESCRIPTOR.message_types_by_name['RunTestRequest']
-_SERIALIZEDGISKARDDATASET = DESCRIPTOR.message_types_by_name['SerializedGiskardDataset']
-_SERIALIZEDGISKARDDATASET_FEATURETYPESENTRY = _SERIALIZEDGISKARDDATASET.nested_types_by_name['FeatureTypesEntry']
-_SERIALIZEDGISKARDDATASET_COLUMNTYPESENTRY = _SERIALIZEDGISKARDDATASET.nested_types_by_name['ColumnTypesEntry']
+_DATASETPROCESSINGREQUEST = DESCRIPTOR.message_types_by_name['DatasetProcessingRequest']
+_DATASETPROCESSINGFUNCTION = DESCRIPTOR.message_types_by_name['DatasetProcessingFunction']
+_SUITETESTARGUMENT = DESCRIPTOR.message_types_by_name['SuiteTestArgument']
+_RUNTESTSUITEREQUEST = DESCRIPTOR.message_types_by_name['RunTestSuiteRequest']
+_FUNCARGUMENT = DESCRIPTOR.message_types_by_name['FuncArgument']
 _RUNTESTRESPONSE = DESCRIPTOR.message_types_by_name['RunTestResponse']
 _PARTIAL_UNEXPECTED_COUNTS = DESCRIPTOR.message_types_by_name['Partial_unexpected_counts']
 _NAMEDSINGLETESTRESULT = DESCRIPTOR.message_types_by_name['NamedSingleTestResult']
+_IDENTIFIERSINGLETESTRESULT = DESCRIPTOR.message_types_by_name['IdentifierSingleTestResult']
 _TESTMESSAGE = DESCRIPTOR.message_types_by_name['TestMessage']
 _SINGLETESTRESULT = DESCRIPTOR.message_types_by_name['SingleTestResult']
 _SINGLETESTRESULT_PROPSENTRY = _SINGLETESTRESULT.nested_types_by_name['PropsEntry']
 _TESTRESULTMESSAGE = DESCRIPTOR.message_types_by_name['TestResultMessage']
-_SERIALIZEDGISKARDMODEL = DESCRIPTOR.message_types_by_name['SerializedGiskardModel']
+_DATASETPROCESSINGRESULTMESSAGE = DESCRIPTOR.message_types_by_name['DatasetProcessingResultMessage']
+_DATASETROWMODIFICATIONRESULT = DESCRIPTOR.message_types_by_name['DatasetRowModificationResult']
+_DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY = _DATASETROWMODIFICATIONRESULT.nested_types_by_name['ModificationsEntry']
+_TESTSUITERESULTMESSAGE = DESCRIPTOR.message_types_by_name['TestSuiteResultMessage']
+_ARTIFACTREF = DESCRIPTOR.message_types_by_name['ArtifactRef']
 _CHUNK = DESCRIPTOR.message_types_by_name['Chunk']
 _UPLOADSTATUS = DESCRIPTOR.message_types_by_name['UploadStatus']
-_TESTFUNCTIONARGUMENT = DESCRIPTOR.message_types_by_name['TestFunctionArgument']
-_TESTFUNCTION = DESCRIPTOR.message_types_by_name['TestFunction']
-_TESTFUNCTION_ARGUMENTSENTRY = _TESTFUNCTION.nested_types_by_name['ArgumentsEntry']
-_TESTREGISTRYRESPONSE = DESCRIPTOR.message_types_by_name['TestRegistryResponse']
 _MLWORKERERRORINFO = DESCRIPTOR.message_types_by_name['MLWorkerErrorInfo']
-_FILTERDATASETREQUEST = DESCRIPTOR.message_types_by_name['FilterDatasetRequest']
-_FILTERDATASETMETADATA = DESCRIPTOR.message_types_by_name['FilterDatasetMetadata']
-_FILTERDATASETMETADATA_COLUMNTYPESENTRY = _FILTERDATASETMETADATA.nested_types_by_name['ColumnTypesEntry']
-_FILTERDATASETRESPONSE = DESCRIPTOR.message_types_by_name['FilterDatasetResponse']
+_SUITEINPUT = DESCRIPTOR.message_types_by_name['SuiteInput']
+_MODELMETA = DESCRIPTOR.message_types_by_name['ModelMeta']
+_DATASETMETA = DESCRIPTOR.message_types_by_name['DatasetMeta']
+_GENERATETESTSUITEREQUEST = DESCRIPTOR.message_types_by_name['GenerateTestSuiteRequest']
+_GENERATETESTSUITERESPONSE = DESCRIPTOR.message_types_by_name['GenerateTestSuiteResponse']
+_GENERATEDTEST = DESCRIPTOR.message_types_by_name['GeneratedTest']
+_GENERATEDTESTINPUT = DESCRIPTOR.message_types_by_name['GeneratedTestInput']
+_CATALOGRESPONSE = DESCRIPTOR.message_types_by_name['CatalogResponse']
+_CATALOGRESPONSE_TESTSENTRY = _CATALOGRESPONSE.nested_types_by_name['TestsEntry']
+_CATALOGRESPONSE_SLICESENTRY = _CATALOGRESPONSE.nested_types_by_name['SlicesEntry']
+_CATALOGRESPONSE_TRANSFORMATIONSENTRY = _CATALOGRESPONSE.nested_types_by_name['TransformationsEntry']
+_FUNCTIONMETA = DESCRIPTOR.message_types_by_name['FunctionMeta']
+_DATASETPROCESSFUNCTIONMETA = DESCRIPTOR.message_types_by_name['DatasetProcessFunctionMeta']
+_TESTFUNCTIONARGUMENT = DESCRIPTOR.message_types_by_name['TestFunctionArgument']
+_COMPARISONCLAUSE = DESCRIPTOR.message_types_by_name['ComparisonClause']
+_GENERATEQUERYBASEDSLICEREQUEST = DESCRIPTOR.message_types_by_name['GenerateQueryBasedSliceRequest']
+_GENERATEQUERYBASEDSLICERESPONSE = DESCRIPTOR.message_types_by_name['GenerateQueryBasedSliceResponse']
 MLWorkerInfoRequest = _reflection.GeneratedProtocolMessageType('MLWorkerInfoRequest', (_message.Message,), {
   'DESCRIPTOR' : _MLWORKERINFOREQUEST,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.MLWorkerInfoRequest)
   })
 _sym_db.RegisterMessage(MLWorkerInfoRequest)
 
@@ -161,27 +185,27 @@
   'ColumnsEntry' : _reflection.GeneratedProtocolMessageType('ColumnsEntry', (_message.Message,), {
     'DESCRIPTOR' : _EXPLAINTEXTREQUEST_COLUMNSENTRY,
     '__module__' : 'ml_worker_pb2'
     # @@protoc_insertion_point(class_scope:worker.ExplainTextRequest.ColumnsEntry)
     })
   ,
 
-  'FeatureTypesEntry' : _reflection.GeneratedProtocolMessageType('FeatureTypesEntry', (_message.Message,), {
-    'DESCRIPTOR' : _EXPLAINTEXTREQUEST_FEATURETYPESENTRY,
+  'ColumnTypesEntry' : _reflection.GeneratedProtocolMessageType('ColumnTypesEntry', (_message.Message,), {
+    'DESCRIPTOR' : _EXPLAINTEXTREQUEST_COLUMNTYPESENTRY,
     '__module__' : 'ml_worker_pb2'
-    # @@protoc_insertion_point(class_scope:worker.ExplainTextRequest.FeatureTypesEntry)
+    # @@protoc_insertion_point(class_scope:worker.ExplainTextRequest.ColumnTypesEntry)
     })
   ,
   'DESCRIPTOR' : _EXPLAINTEXTREQUEST,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.ExplainTextRequest)
   })
 _sym_db.RegisterMessage(ExplainTextRequest)
 _sym_db.RegisterMessage(ExplainTextRequest.ColumnsEntry)
-_sym_db.RegisterMessage(ExplainTextRequest.FeatureTypesEntry)
+_sym_db.RegisterMessage(ExplainTextRequest.ColumnTypesEntry)
 
 ExplainResponse = _reflection.GeneratedProtocolMessageType('ExplainResponse', (_message.Message,), {
 
   'Explanation' : _reflection.GeneratedProtocolMessageType('Explanation', (_message.Message,), {
 
     'PerFeatureEntry' : _reflection.GeneratedProtocolMessageType('PerFeatureEntry', (_message.Message,), {
       'DESCRIPTOR' : _EXPLAINRESPONSE_EXPLANATION_PERFEATUREENTRY,
@@ -260,34 +284,34 @@
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.DataFrame)
   })
 _sym_db.RegisterMessage(DataFrame)
 
 RunModelForDataFrameRequest = _reflection.GeneratedProtocolMessageType('RunModelForDataFrameRequest', (_message.Message,), {
 
-  'FeatureTypesEntry' : _reflection.GeneratedProtocolMessageType('FeatureTypesEntry', (_message.Message,), {
-    'DESCRIPTOR' : _RUNMODELFORDATAFRAMEREQUEST_FEATURETYPESENTRY,
+  'ColumnTypesEntry' : _reflection.GeneratedProtocolMessageType('ColumnTypesEntry', (_message.Message,), {
+    'DESCRIPTOR' : _RUNMODELFORDATAFRAMEREQUEST_COLUMNTYPESENTRY,
     '__module__' : 'ml_worker_pb2'
-    # @@protoc_insertion_point(class_scope:worker.RunModelForDataFrameRequest.FeatureTypesEntry)
+    # @@protoc_insertion_point(class_scope:worker.RunModelForDataFrameRequest.ColumnTypesEntry)
     })
   ,
 
-  'ColumnTypesEntry' : _reflection.GeneratedProtocolMessageType('ColumnTypesEntry', (_message.Message,), {
-    'DESCRIPTOR' : _RUNMODELFORDATAFRAMEREQUEST_COLUMNTYPESENTRY,
+  'ColumnDtypesEntry' : _reflection.GeneratedProtocolMessageType('ColumnDtypesEntry', (_message.Message,), {
+    'DESCRIPTOR' : _RUNMODELFORDATAFRAMEREQUEST_COLUMNDTYPESENTRY,
     '__module__' : 'ml_worker_pb2'
-    # @@protoc_insertion_point(class_scope:worker.RunModelForDataFrameRequest.ColumnTypesEntry)
+    # @@protoc_insertion_point(class_scope:worker.RunModelForDataFrameRequest.ColumnDtypesEntry)
     })
   ,
   'DESCRIPTOR' : _RUNMODELFORDATAFRAMEREQUEST,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.RunModelForDataFrameRequest)
   })
 _sym_db.RegisterMessage(RunModelForDataFrameRequest)
-_sym_db.RegisterMessage(RunModelForDataFrameRequest.FeatureTypesEntry)
 _sym_db.RegisterMessage(RunModelForDataFrameRequest.ColumnTypesEntry)
+_sym_db.RegisterMessage(RunModelForDataFrameRequest.ColumnDtypesEntry)
 
 RunModelRequest = _reflection.GeneratedProtocolMessageType('RunModelRequest', (_message.Message,), {
   'DESCRIPTOR' : _RUNMODELREQUEST,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.RunModelRequest)
   })
 _sym_db.RegisterMessage(RunModelRequest)
@@ -302,50 +326,48 @@
 RunAdHocTestRequest = _reflection.GeneratedProtocolMessageType('RunAdHocTestRequest', (_message.Message,), {
   'DESCRIPTOR' : _RUNADHOCTESTREQUEST,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.RunAdHocTestRequest)
   })
 _sym_db.RegisterMessage(RunAdHocTestRequest)
 
-TestArgument = _reflection.GeneratedProtocolMessageType('TestArgument', (_message.Message,), {
-  'DESCRIPTOR' : _TESTARGUMENT,
+DatasetProcessingRequest = _reflection.GeneratedProtocolMessageType('DatasetProcessingRequest', (_message.Message,), {
+  'DESCRIPTOR' : _DATASETPROCESSINGREQUEST,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.TestArgument)
+  # @@protoc_insertion_point(class_scope:worker.DatasetProcessingRequest)
   })
-_sym_db.RegisterMessage(TestArgument)
+_sym_db.RegisterMessage(DatasetProcessingRequest)
 
-RunTestRequest = _reflection.GeneratedProtocolMessageType('RunTestRequest', (_message.Message,), {
-  'DESCRIPTOR' : _RUNTESTREQUEST,
+DatasetProcessingFunction = _reflection.GeneratedProtocolMessageType('DatasetProcessingFunction', (_message.Message,), {
+  'DESCRIPTOR' : _DATASETPROCESSINGFUNCTION,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.RunTestRequest)
+  # @@protoc_insertion_point(class_scope:worker.DatasetProcessingFunction)
   })
-_sym_db.RegisterMessage(RunTestRequest)
+_sym_db.RegisterMessage(DatasetProcessingFunction)
 
-SerializedGiskardDataset = _reflection.GeneratedProtocolMessageType('SerializedGiskardDataset', (_message.Message,), {
+SuiteTestArgument = _reflection.GeneratedProtocolMessageType('SuiteTestArgument', (_message.Message,), {
+  'DESCRIPTOR' : _SUITETESTARGUMENT,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.SuiteTestArgument)
+  })
+_sym_db.RegisterMessage(SuiteTestArgument)
 
-  'FeatureTypesEntry' : _reflection.GeneratedProtocolMessageType('FeatureTypesEntry', (_message.Message,), {
-    'DESCRIPTOR' : _SERIALIZEDGISKARDDATASET_FEATURETYPESENTRY,
-    '__module__' : 'ml_worker_pb2'
-    # @@protoc_insertion_point(class_scope:worker.SerializedGiskardDataset.FeatureTypesEntry)
-    })
-  ,
+RunTestSuiteRequest = _reflection.GeneratedProtocolMessageType('RunTestSuiteRequest', (_message.Message,), {
+  'DESCRIPTOR' : _RUNTESTSUITEREQUEST,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.RunTestSuiteRequest)
+  })
+_sym_db.RegisterMessage(RunTestSuiteRequest)
 
-  'ColumnTypesEntry' : _reflection.GeneratedProtocolMessageType('ColumnTypesEntry', (_message.Message,), {
-    'DESCRIPTOR' : _SERIALIZEDGISKARDDATASET_COLUMNTYPESENTRY,
-    '__module__' : 'ml_worker_pb2'
-    # @@protoc_insertion_point(class_scope:worker.SerializedGiskardDataset.ColumnTypesEntry)
-    })
-  ,
-  'DESCRIPTOR' : _SERIALIZEDGISKARDDATASET,
+FuncArgument = _reflection.GeneratedProtocolMessageType('FuncArgument', (_message.Message,), {
+  'DESCRIPTOR' : _FUNCARGUMENT,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.SerializedGiskardDataset)
+  # @@protoc_insertion_point(class_scope:worker.FuncArgument)
   })
-_sym_db.RegisterMessage(SerializedGiskardDataset)
-_sym_db.RegisterMessage(SerializedGiskardDataset.FeatureTypesEntry)
-_sym_db.RegisterMessage(SerializedGiskardDataset.ColumnTypesEntry)
+_sym_db.RegisterMessage(FuncArgument)
 
 RunTestResponse = _reflection.GeneratedProtocolMessageType('RunTestResponse', (_message.Message,), {
   'DESCRIPTOR' : _RUNTESTRESPONSE,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.RunTestResponse)
   })
 _sym_db.RegisterMessage(RunTestResponse)
@@ -360,14 +382,21 @@
 NamedSingleTestResult = _reflection.GeneratedProtocolMessageType('NamedSingleTestResult', (_message.Message,), {
   'DESCRIPTOR' : _NAMEDSINGLETESTRESULT,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.NamedSingleTestResult)
   })
 _sym_db.RegisterMessage(NamedSingleTestResult)
 
+IdentifierSingleTestResult = _reflection.GeneratedProtocolMessageType('IdentifierSingleTestResult', (_message.Message,), {
+  'DESCRIPTOR' : _IDENTIFIERSINGLETESTRESULT,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.IdentifierSingleTestResult)
+  })
+_sym_db.RegisterMessage(IdentifierSingleTestResult)
+
 TestMessage = _reflection.GeneratedProtocolMessageType('TestMessage', (_message.Message,), {
   'DESCRIPTOR' : _TESTMESSAGE,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.TestMessage)
   })
 _sym_db.RegisterMessage(TestMessage)
 
@@ -389,20 +418,49 @@
 TestResultMessage = _reflection.GeneratedProtocolMessageType('TestResultMessage', (_message.Message,), {
   'DESCRIPTOR' : _TESTRESULTMESSAGE,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.TestResultMessage)
   })
 _sym_db.RegisterMessage(TestResultMessage)
 
-SerializedGiskardModel = _reflection.GeneratedProtocolMessageType('SerializedGiskardModel', (_message.Message,), {
-  'DESCRIPTOR' : _SERIALIZEDGISKARDMODEL,
+DatasetProcessingResultMessage = _reflection.GeneratedProtocolMessageType('DatasetProcessingResultMessage', (_message.Message,), {
+  'DESCRIPTOR' : _DATASETPROCESSINGRESULTMESSAGE,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.DatasetProcessingResultMessage)
+  })
+_sym_db.RegisterMessage(DatasetProcessingResultMessage)
+
+DatasetRowModificationResult = _reflection.GeneratedProtocolMessageType('DatasetRowModificationResult', (_message.Message,), {
+
+  'ModificationsEntry' : _reflection.GeneratedProtocolMessageType('ModificationsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY,
+    '__module__' : 'ml_worker_pb2'
+    # @@protoc_insertion_point(class_scope:worker.DatasetRowModificationResult.ModificationsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _DATASETROWMODIFICATIONRESULT,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.DatasetRowModificationResult)
+  })
+_sym_db.RegisterMessage(DatasetRowModificationResult)
+_sym_db.RegisterMessage(DatasetRowModificationResult.ModificationsEntry)
+
+TestSuiteResultMessage = _reflection.GeneratedProtocolMessageType('TestSuiteResultMessage', (_message.Message,), {
+  'DESCRIPTOR' : _TESTSUITERESULTMESSAGE,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.SerializedGiskardModel)
+  # @@protoc_insertion_point(class_scope:worker.TestSuiteResultMessage)
   })
-_sym_db.RegisterMessage(SerializedGiskardModel)
+_sym_db.RegisterMessage(TestSuiteResultMessage)
+
+ArtifactRef = _reflection.GeneratedProtocolMessageType('ArtifactRef', (_message.Message,), {
+  'DESCRIPTOR' : _ARTIFACTREF,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.ArtifactRef)
+  })
+_sym_db.RegisterMessage(ArtifactRef)
 
 Chunk = _reflection.GeneratedProtocolMessageType('Chunk', (_message.Message,), {
   'DESCRIPTOR' : _CHUNK,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.Chunk)
   })
 _sym_db.RegisterMessage(Chunk)
@@ -410,222 +468,316 @@
 UploadStatus = _reflection.GeneratedProtocolMessageType('UploadStatus', (_message.Message,), {
   'DESCRIPTOR' : _UPLOADSTATUS,
   '__module__' : 'ml_worker_pb2'
   # @@protoc_insertion_point(class_scope:worker.UploadStatus)
   })
 _sym_db.RegisterMessage(UploadStatus)
 
-TestFunctionArgument = _reflection.GeneratedProtocolMessageType('TestFunctionArgument', (_message.Message,), {
-  'DESCRIPTOR' : _TESTFUNCTIONARGUMENT,
+MLWorkerErrorInfo = _reflection.GeneratedProtocolMessageType('MLWorkerErrorInfo', (_message.Message,), {
+  'DESCRIPTOR' : _MLWORKERERRORINFO,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.TestFunctionArgument)
+  # @@protoc_insertion_point(class_scope:worker.MLWorkerErrorInfo)
   })
-_sym_db.RegisterMessage(TestFunctionArgument)
+_sym_db.RegisterMessage(MLWorkerErrorInfo)
 
-TestFunction = _reflection.GeneratedProtocolMessageType('TestFunction', (_message.Message,), {
+SuiteInput = _reflection.GeneratedProtocolMessageType('SuiteInput', (_message.Message,), {
+  'DESCRIPTOR' : _SUITEINPUT,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.SuiteInput)
+  })
+_sym_db.RegisterMessage(SuiteInput)
 
-  'ArgumentsEntry' : _reflection.GeneratedProtocolMessageType('ArgumentsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _TESTFUNCTION_ARGUMENTSENTRY,
-    '__module__' : 'ml_worker_pb2'
-    # @@protoc_insertion_point(class_scope:worker.TestFunction.ArgumentsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _TESTFUNCTION,
+ModelMeta = _reflection.GeneratedProtocolMessageType('ModelMeta', (_message.Message,), {
+  'DESCRIPTOR' : _MODELMETA,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.TestFunction)
+  # @@protoc_insertion_point(class_scope:worker.ModelMeta)
   })
-_sym_db.RegisterMessage(TestFunction)
-_sym_db.RegisterMessage(TestFunction.ArgumentsEntry)
+_sym_db.RegisterMessage(ModelMeta)
 
-TestRegistryResponse = _reflection.GeneratedProtocolMessageType('TestRegistryResponse', (_message.Message,), {
-  'DESCRIPTOR' : _TESTREGISTRYRESPONSE,
+DatasetMeta = _reflection.GeneratedProtocolMessageType('DatasetMeta', (_message.Message,), {
+  'DESCRIPTOR' : _DATASETMETA,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.TestRegistryResponse)
+  # @@protoc_insertion_point(class_scope:worker.DatasetMeta)
   })
-_sym_db.RegisterMessage(TestRegistryResponse)
+_sym_db.RegisterMessage(DatasetMeta)
 
-MLWorkerErrorInfo = _reflection.GeneratedProtocolMessageType('MLWorkerErrorInfo', (_message.Message,), {
-  'DESCRIPTOR' : _MLWORKERERRORINFO,
+GenerateTestSuiteRequest = _reflection.GeneratedProtocolMessageType('GenerateTestSuiteRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GENERATETESTSUITEREQUEST,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.MLWorkerErrorInfo)
+  # @@protoc_insertion_point(class_scope:worker.GenerateTestSuiteRequest)
   })
-_sym_db.RegisterMessage(MLWorkerErrorInfo)
+_sym_db.RegisterMessage(GenerateTestSuiteRequest)
+
+GenerateTestSuiteResponse = _reflection.GeneratedProtocolMessageType('GenerateTestSuiteResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GENERATETESTSUITERESPONSE,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.GenerateTestSuiteResponse)
+  })
+_sym_db.RegisterMessage(GenerateTestSuiteResponse)
+
+GeneratedTest = _reflection.GeneratedProtocolMessageType('GeneratedTest', (_message.Message,), {
+  'DESCRIPTOR' : _GENERATEDTEST,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.GeneratedTest)
+  })
+_sym_db.RegisterMessage(GeneratedTest)
 
-FilterDatasetRequest = _reflection.GeneratedProtocolMessageType('FilterDatasetRequest', (_message.Message,), {
-  'DESCRIPTOR' : _FILTERDATASETREQUEST,
+GeneratedTestInput = _reflection.GeneratedProtocolMessageType('GeneratedTestInput', (_message.Message,), {
+  'DESCRIPTOR' : _GENERATEDTESTINPUT,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.FilterDatasetRequest)
+  # @@protoc_insertion_point(class_scope:worker.GeneratedTestInput)
   })
-_sym_db.RegisterMessage(FilterDatasetRequest)
+_sym_db.RegisterMessage(GeneratedTestInput)
 
-FilterDatasetMetadata = _reflection.GeneratedProtocolMessageType('FilterDatasetMetadata', (_message.Message,), {
+CatalogResponse = _reflection.GeneratedProtocolMessageType('CatalogResponse', (_message.Message,), {
 
-  'ColumnTypesEntry' : _reflection.GeneratedProtocolMessageType('ColumnTypesEntry', (_message.Message,), {
-    'DESCRIPTOR' : _FILTERDATASETMETADATA_COLUMNTYPESENTRY,
+  'TestsEntry' : _reflection.GeneratedProtocolMessageType('TestsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _CATALOGRESPONSE_TESTSENTRY,
     '__module__' : 'ml_worker_pb2'
-    # @@protoc_insertion_point(class_scope:worker.FilterDatasetMetadata.ColumnTypesEntry)
+    # @@protoc_insertion_point(class_scope:worker.CatalogResponse.TestsEntry)
     })
   ,
-  'DESCRIPTOR' : _FILTERDATASETMETADATA,
+
+  'SlicesEntry' : _reflection.GeneratedProtocolMessageType('SlicesEntry', (_message.Message,), {
+    'DESCRIPTOR' : _CATALOGRESPONSE_SLICESENTRY,
+    '__module__' : 'ml_worker_pb2'
+    # @@protoc_insertion_point(class_scope:worker.CatalogResponse.SlicesEntry)
+    })
+  ,
+
+  'TransformationsEntry' : _reflection.GeneratedProtocolMessageType('TransformationsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _CATALOGRESPONSE_TRANSFORMATIONSENTRY,
+    '__module__' : 'ml_worker_pb2'
+    # @@protoc_insertion_point(class_scope:worker.CatalogResponse.TransformationsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _CATALOGRESPONSE,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.CatalogResponse)
+  })
+_sym_db.RegisterMessage(CatalogResponse)
+_sym_db.RegisterMessage(CatalogResponse.TestsEntry)
+_sym_db.RegisterMessage(CatalogResponse.SlicesEntry)
+_sym_db.RegisterMessage(CatalogResponse.TransformationsEntry)
+
+FunctionMeta = _reflection.GeneratedProtocolMessageType('FunctionMeta', (_message.Message,), {
+  'DESCRIPTOR' : _FUNCTIONMETA,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.FunctionMeta)
+  })
+_sym_db.RegisterMessage(FunctionMeta)
+
+DatasetProcessFunctionMeta = _reflection.GeneratedProtocolMessageType('DatasetProcessFunctionMeta', (_message.Message,), {
+  'DESCRIPTOR' : _DATASETPROCESSFUNCTIONMETA,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.DatasetProcessFunctionMeta)
+  })
+_sym_db.RegisterMessage(DatasetProcessFunctionMeta)
+
+TestFunctionArgument = _reflection.GeneratedProtocolMessageType('TestFunctionArgument', (_message.Message,), {
+  'DESCRIPTOR' : _TESTFUNCTIONARGUMENT,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.TestFunctionArgument)
+  })
+_sym_db.RegisterMessage(TestFunctionArgument)
+
+ComparisonClause = _reflection.GeneratedProtocolMessageType('ComparisonClause', (_message.Message,), {
+  'DESCRIPTOR' : _COMPARISONCLAUSE,
+  '__module__' : 'ml_worker_pb2'
+  # @@protoc_insertion_point(class_scope:worker.ComparisonClause)
+  })
+_sym_db.RegisterMessage(ComparisonClause)
+
+GenerateQueryBasedSliceRequest = _reflection.GeneratedProtocolMessageType('GenerateQueryBasedSliceRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GENERATEQUERYBASEDSLICEREQUEST,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.FilterDatasetMetadata)
+  # @@protoc_insertion_point(class_scope:worker.GenerateQueryBasedSliceRequest)
   })
-_sym_db.RegisterMessage(FilterDatasetMetadata)
-_sym_db.RegisterMessage(FilterDatasetMetadata.ColumnTypesEntry)
+_sym_db.RegisterMessage(GenerateQueryBasedSliceRequest)
 
-FilterDatasetResponse = _reflection.GeneratedProtocolMessageType('FilterDatasetResponse', (_message.Message,), {
-  'DESCRIPTOR' : _FILTERDATASETRESPONSE,
+GenerateQueryBasedSliceResponse = _reflection.GeneratedProtocolMessageType('GenerateQueryBasedSliceResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GENERATEQUERYBASEDSLICERESPONSE,
   '__module__' : 'ml_worker_pb2'
-  # @@protoc_insertion_point(class_scope:worker.FilterDatasetResponse)
+  # @@protoc_insertion_point(class_scope:worker.GenerateQueryBasedSliceResponse)
   })
-_sym_db.RegisterMessage(FilterDatasetResponse)
+_sym_db.RegisterMessage(GenerateQueryBasedSliceResponse)
 
 _MLWORKER = DESCRIPTOR.services_by_name['MLWorker']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021ai.giskard.workerB\013WorkerProtoP\001\242\002\003WRK'
   _MLWORKERINFO_INSTALLEDPACKAGESENTRY._options = None
   _MLWORKERINFO_INSTALLEDPACKAGESENTRY._serialized_options = b'8\001'
   _EXPLAINREQUEST_COLUMNSENTRY._options = None
   _EXPLAINREQUEST_COLUMNSENTRY._serialized_options = b'8\001'
   _EXPLAINTEXTREQUEST_COLUMNSENTRY._options = None
   _EXPLAINTEXTREQUEST_COLUMNSENTRY._serialized_options = b'8\001'
-  _EXPLAINTEXTREQUEST_FEATURETYPESENTRY._options = None
-  _EXPLAINTEXTREQUEST_FEATURETYPESENTRY._serialized_options = b'8\001'
+  _EXPLAINTEXTREQUEST_COLUMNTYPESENTRY._options = None
+  _EXPLAINTEXTREQUEST_COLUMNTYPESENTRY._serialized_options = b'8\001'
   _EXPLAINRESPONSE_EXPLANATION_PERFEATUREENTRY._options = None
   _EXPLAINRESPONSE_EXPLANATION_PERFEATUREENTRY._serialized_options = b'8\001'
   _EXPLAINRESPONSE_EXPLANATIONSENTRY._options = None
   _EXPLAINRESPONSE_EXPLANATIONSENTRY._serialized_options = b'8\001'
   _EXPLAINTEXTRESPONSE_WEIGHTSENTRY._options = None
   _EXPLAINTEXTRESPONSE_WEIGHTSENTRY._serialized_options = b'8\001'
   _DATAROW_COLUMNSENTRY._options = None
   _DATAROW_COLUMNSENTRY._serialized_options = b'8\001'
-  _RUNMODELFORDATAFRAMEREQUEST_FEATURETYPESENTRY._options = None
-  _RUNMODELFORDATAFRAMEREQUEST_FEATURETYPESENTRY._serialized_options = b'8\001'
   _RUNMODELFORDATAFRAMEREQUEST_COLUMNTYPESENTRY._options = None
   _RUNMODELFORDATAFRAMEREQUEST_COLUMNTYPESENTRY._serialized_options = b'8\001'
-  _SERIALIZEDGISKARDDATASET_FEATURETYPESENTRY._options = None
-  _SERIALIZEDGISKARDDATASET_FEATURETYPESENTRY._serialized_options = b'8\001'
-  _SERIALIZEDGISKARDDATASET_COLUMNTYPESENTRY._options = None
-  _SERIALIZEDGISKARDDATASET_COLUMNTYPESENTRY._serialized_options = b'8\001'
+  _RUNMODELFORDATAFRAMEREQUEST_COLUMNDTYPESENTRY._options = None
+  _RUNMODELFORDATAFRAMEREQUEST_COLUMNDTYPESENTRY._serialized_options = b'8\001'
   _SINGLETESTRESULT_PROPSENTRY._options = None
   _SINGLETESTRESULT_PROPSENTRY._serialized_options = b'8\001'
-  _TESTFUNCTION_ARGUMENTSENTRY._options = None
-  _TESTFUNCTION_ARGUMENTSENTRY._serialized_options = b'8\001'
-  _FILTERDATASETMETADATA_COLUMNTYPESENTRY._options = None
-  _FILTERDATASETMETADATA_COLUMNTYPESENTRY._serialized_options = b'8\001'
-  _FILETYPE._serialized_start=5856
-  _FILETYPE._serialized_end=5890
-  _TESTMESSAGETYPE._serialized_start=5892
-  _TESTMESSAGETYPE._serialized_end=5930
-  _STATUSCODE._serialized_start=5932
-  _STATUSCODE._serialized_end=6013
+  _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY._options = None
+  _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY._serialized_options = b'8\001'
+  _CATALOGRESPONSE_TESTSENTRY._options = None
+  _CATALOGRESPONSE_TESTSENTRY._serialized_options = b'8\001'
+  _CATALOGRESPONSE_SLICESENTRY._options = None
+  _CATALOGRESPONSE_SLICESENTRY._serialized_options = b'8\001'
+  _CATALOGRESPONSE_TRANSFORMATIONSENTRY._options = None
+  _CATALOGRESPONSE_TRANSFORMATIONSENTRY._serialized_options = b'8\001'
+  _FILETYPE._serialized_start=7376
+  _FILETYPE._serialized_end=7410
+  _TESTMESSAGETYPE._serialized_start=7412
+  _TESTMESSAGETYPE._serialized_end=7450
+  _STATUSCODE._serialized_start=7452
+  _STATUSCODE._serialized_end=7533
+  _COMPARISONTYPE._serialized_start=7536
+  _COMPARISONTYPE._serialized_end=7673
   _MLWORKERINFOREQUEST._serialized_start=115
   _MLWORKERINFOREQUEST._serialized_end=159
   _MLWORKERINFO._serialized_start=162
-  _MLWORKERINFO._serialized_end=517
-  _MLWORKERINFO_INSTALLEDPACKAGESENTRY._serialized_start=461
-  _MLWORKERINFO_INSTALLEDPACKAGESENTRY._serialized_end=517
-  _PLATFORMINFO._serialized_start=519
-  _PLATFORMINFO._serialized_end=633
-  _FILEUPLOADREQUEST._serialized_start=635
-  _FILEUPLOADREQUEST._serialized_end=745
-  _FILEUPLOADMETADATA._serialized_start=747
-  _FILEUPLOADMETADATA._serialized_end=851
-  _ECHOMSG._serialized_start=853
-  _ECHOMSG._serialized_end=875
-  _EXPLAINREQUEST._serialized_start=878
-  _EXPLAINREQUEST._serialized_end=1094
-  _EXPLAINREQUEST_COLUMNSENTRY._serialized_start=1048
-  _EXPLAINREQUEST_COLUMNSENTRY._serialized_end=1094
-  _EXPLAINTEXTREQUEST._serialized_start=1097
-  _EXPLAINTEXTREQUEST._serialized_end=1433
-  _EXPLAINTEXTREQUEST_COLUMNSENTRY._serialized_start=1048
-  _EXPLAINTEXTREQUEST_COLUMNSENTRY._serialized_end=1094
-  _EXPLAINTEXTREQUEST_FEATURETYPESENTRY._serialized_start=1382
-  _EXPLAINTEXTREQUEST_FEATURETYPESENTRY._serialized_end=1433
-  _EXPLAINRESPONSE._serialized_start=1436
-  _EXPLAINRESPONSE._serialized_end=1749
-  _EXPLAINRESPONSE_EXPLANATION._serialized_start=1521
-  _EXPLAINRESPONSE_EXPLANATION._serialized_end=1659
-  _EXPLAINRESPONSE_EXPLANATION_PERFEATUREENTRY._serialized_start=1610
-  _EXPLAINRESPONSE_EXPLANATION_PERFEATUREENTRY._serialized_end=1659
-  _EXPLAINRESPONSE_EXPLANATIONSENTRY._serialized_start=1661
-  _EXPLAINRESPONSE_EXPLANATIONSENTRY._serialized_end=1749
-  _EXPLAINTEXTRESPONSE._serialized_start=1752
-  _EXPLAINTEXTRESPONSE._serialized_end=1980
-  _EXPLAINTEXTRESPONSE_WEIGHTSPERFEATURE._serialized_start=1849
-  _EXPLAINTEXTRESPONSE_WEIGHTSPERFEATURE._serialized_end=1885
-  _EXPLAINTEXTRESPONSE_WEIGHTSENTRY._serialized_start=1887
-  _EXPLAINTEXTRESPONSE_WEIGHTSENTRY._serialized_end=1980
-  _RUNMODELFORDATAFRAMERESPONSE._serialized_start=1983
-  _RUNMODELFORDATAFRAMERESPONSE._serialized_end=2124
-  _DATAROW._serialized_start=2126
-  _DATAROW._serialized_end=2230
-  _DATAROW_COLUMNSENTRY._serialized_start=1048
-  _DATAROW_COLUMNSENTRY._serialized_end=1094
-  _DATAFRAME._serialized_start=2232
-  _DATAFRAME._serialized_end=2274
-  _RUNMODELFORDATAFRAMEREQUEST._serialized_start=2277
-  _RUNMODELFORDATAFRAMEREQUEST._serialized_end=2666
-  _RUNMODELFORDATAFRAMEREQUEST_FEATURETYPESENTRY._serialized_start=1382
-  _RUNMODELFORDATAFRAMEREQUEST_FEATURETYPESENTRY._serialized_end=1433
-  _RUNMODELFORDATAFRAMEREQUEST_COLUMNTYPESENTRY._serialized_start=2616
-  _RUNMODELFORDATAFRAMEREQUEST_COLUMNTYPESENTRY._serialized_end=2666
-  _RUNMODELREQUEST._serialized_start=2668
-  _RUNMODELREQUEST._serialized_end=2783
-  _RUNMODELRESPONSE._serialized_start=2785
-  _RUNMODELRESPONSE._serialized_end=2848
-  _RUNADHOCTESTREQUEST._serialized_start=2850
-  _RUNADHOCTESTREQUEST._serialized_end=2928
-  _TESTARGUMENT._serialized_start=2931
-  _TESTARGUMENT._serialized_end=3108
-  _RUNTESTREQUEST._serialized_start=3111
-  _RUNTESTREQUEST._serialized_end=3297
-  _SERIALIZEDGISKARDDATASET._serialized_start=3300
-  _SERIALIZEDGISKARDDATASET._serialized_end=3635
-  _SERIALIZEDGISKARDDATASET_FEATURETYPESENTRY._serialized_start=1382
-  _SERIALIZEDGISKARDDATASET_FEATURETYPESENTRY._serialized_end=1433
-  _SERIALIZEDGISKARDDATASET_COLUMNTYPESENTRY._serialized_start=2616
-  _SERIALIZEDGISKARDDATASET_COLUMNTYPESENTRY._serialized_end=2666
-  _RUNTESTRESPONSE._serialized_start=3637
-  _RUNTESTRESPONSE._serialized_end=3668
-  _PARTIAL_UNEXPECTED_COUNTS._serialized_start=3670
-  _PARTIAL_UNEXPECTED_COUNTS._serialized_end=3727
-  _NAMEDSINGLETESTRESULT._serialized_start=3729
-  _NAMEDSINGLETESTRESULT._serialized_end=3808
-  _TESTMESSAGE._serialized_start=3810
-  _TESTMESSAGE._serialized_end=3876
-  _SINGLETESTRESULT._serialized_start=3879
-  _SINGLETESTRESULT._serialized_end=4671
-  _SINGLETESTRESULT_PROPSENTRY._serialized_start=4627
-  _SINGLETESTRESULT_PROPSENTRY._serialized_end=4671
-  _TESTRESULTMESSAGE._serialized_start=4673
-  _TESTRESULTMESSAGE._serialized_end=4740
-  _SERIALIZEDGISKARDMODEL._serialized_start=4743
-  _SERIALIZEDGISKARDMODEL._serialized_end=4930
-  _CHUNK._serialized_start=4932
-  _CHUNK._serialized_end=4956
-  _UPLOADSTATUS._serialized_start=4958
-  _UPLOADSTATUS._serialized_end=5006
-  _TESTFUNCTIONARGUMENT._serialized_start=5008
-  _TESTFUNCTIONARGUMENT._serialized_end=5093
-  _TESTFUNCTION._serialized_start=5096
-  _TESTFUNCTION._serialized_end=5335
-  _TESTFUNCTION_ARGUMENTSENTRY._serialized_start=5257
-  _TESTFUNCTION_ARGUMENTSENTRY._serialized_end=5335
-  _TESTREGISTRYRESPONSE._serialized_start=5337
-  _TESTREGISTRYRESPONSE._serialized_end=5400
-  _MLWORKERERRORINFO._serialized_start=5402
-  _MLWORKERERRORINFO._serialized_end=5451
-  _FILTERDATASETREQUEST._serialized_start=5453
-  _FILTERDATASETREQUEST._serialized_end=5562
-  _FILTERDATASETMETADATA._serialized_start=5565
-  _FILTERDATASETMETADATA._serialized_end=5745
-  _FILTERDATASETMETADATA_COLUMNTYPESENTRY._serialized_start=2616
-  _FILTERDATASETMETADATA_COLUMNTYPESENTRY._serialized_end=2666
-  _FILTERDATASETRESPONSE._serialized_start=5747
-  _FILTERDATASETRESPONSE._serialized_end=5854
-  _MLWORKER._serialized_start=6016
-  _MLWORKER._serialized_end=6798
+  _MLWORKERINFO._serialized_end=520
+  _MLWORKERINFO_INSTALLEDPACKAGESENTRY._serialized_start=464
+  _MLWORKERINFO_INSTALLEDPACKAGESENTRY._serialized_end=520
+  _PLATFORMINFO._serialized_start=522
+  _PLATFORMINFO._serialized_end=636
+  _FILEUPLOADREQUEST._serialized_start=638
+  _FILEUPLOADREQUEST._serialized_end=748
+  _FILEUPLOADMETADATA._serialized_start=750
+  _FILEUPLOADMETADATA._serialized_end=854
+  _ECHOMSG._serialized_start=856
+  _ECHOMSG._serialized_end=878
+  _EXPLAINREQUEST._serialized_start=881
+  _EXPLAINREQUEST._serialized_end=1073
+  _EXPLAINREQUEST_COLUMNSENTRY._serialized_start=1027
+  _EXPLAINREQUEST_COLUMNSENTRY._serialized_end=1073
+  _EXPLAINTEXTREQUEST._serialized_start=1076
+  _EXPLAINTEXTREQUEST._serialized_end=1398
+  _EXPLAINTEXTREQUEST_COLUMNSENTRY._serialized_start=1027
+  _EXPLAINTEXTREQUEST_COLUMNSENTRY._serialized_end=1073
+  _EXPLAINTEXTREQUEST_COLUMNTYPESENTRY._serialized_start=1348
+  _EXPLAINTEXTREQUEST_COLUMNTYPESENTRY._serialized_end=1398
+  _EXPLAINRESPONSE._serialized_start=1401
+  _EXPLAINRESPONSE._serialized_end=1714
+  _EXPLAINRESPONSE_EXPLANATION._serialized_start=1486
+  _EXPLAINRESPONSE_EXPLANATION._serialized_end=1624
+  _EXPLAINRESPONSE_EXPLANATION_PERFEATUREENTRY._serialized_start=1575
+  _EXPLAINRESPONSE_EXPLANATION_PERFEATUREENTRY._serialized_end=1624
+  _EXPLAINRESPONSE_EXPLANATIONSENTRY._serialized_start=1626
+  _EXPLAINRESPONSE_EXPLANATIONSENTRY._serialized_end=1714
+  _EXPLAINTEXTRESPONSE._serialized_start=1717
+  _EXPLAINTEXTRESPONSE._serialized_end=1945
+  _EXPLAINTEXTRESPONSE_WEIGHTSPERFEATURE._serialized_start=1814
+  _EXPLAINTEXTRESPONSE_WEIGHTSPERFEATURE._serialized_end=1850
+  _EXPLAINTEXTRESPONSE_WEIGHTSENTRY._serialized_start=1852
+  _EXPLAINTEXTRESPONSE_WEIGHTSENTRY._serialized_end=1945
+  _RUNMODELFORDATAFRAMERESPONSE._serialized_start=1948
+  _RUNMODELFORDATAFRAMERESPONSE._serialized_end=2089
+  _DATAROW._serialized_start=2091
+  _DATAROW._serialized_end=2195
+  _DATAROW_COLUMNSENTRY._serialized_start=1027
+  _DATAROW_COLUMNSENTRY._serialized_end=1073
+  _DATAFRAME._serialized_start=2197
+  _DATAFRAME._serialized_end=2239
+  _RUNMODELFORDATAFRAMEREQUEST._serialized_start=2242
+  _RUNMODELFORDATAFRAMEREQUEST._serialized_end=2620
+  _RUNMODELFORDATAFRAMEREQUEST_COLUMNTYPESENTRY._serialized_start=1348
+  _RUNMODELFORDATAFRAMEREQUEST_COLUMNTYPESENTRY._serialized_end=1398
+  _RUNMODELFORDATAFRAMEREQUEST_COLUMNDTYPESENTRY._serialized_start=2569
+  _RUNMODELFORDATAFRAMEREQUEST_COLUMNDTYPESENTRY._serialized_end=2620
+  _RUNMODELREQUEST._serialized_start=2623
+  _RUNMODELREQUEST._serialized_end=2757
+  _RUNMODELRESPONSE._serialized_start=2759
+  _RUNMODELRESPONSE._serialized_end=2822
+  _RUNADHOCTESTREQUEST._serialized_start=2824
+  _RUNADHOCTESTREQUEST._serialized_end=2904
+  _DATASETPROCESSINGREQUEST._serialized_start=2906
+  _DATASETPROCESSINGREQUEST._serialized_end=3024
+  _DATASETPROCESSINGFUNCTION._serialized_start=3027
+  _DATASETPROCESSINGFUNCTION._serialized_end=3210
+  _SUITETESTARGUMENT._serialized_start=3212
+  _SUITETESTARGUMENT._serialized_end=3302
+  _RUNTESTSUITEREQUEST._serialized_start=3304
+  _RUNTESTSUITEREQUEST._serialized_end=3414
+  _FUNCARGUMENT._serialized_start=3417
+  _FUNCARGUMENT._serialized_end=3769
+  _RUNTESTRESPONSE._serialized_start=3771
+  _RUNTESTRESPONSE._serialized_end=3802
+  _PARTIAL_UNEXPECTED_COUNTS._serialized_start=3804
+  _PARTIAL_UNEXPECTED_COUNTS._serialized_end=3861
+  _NAMEDSINGLETESTRESULT._serialized_start=3863
+  _NAMEDSINGLETESTRESULT._serialized_end=3946
+  _IDENTIFIERSINGLETESTRESULT._serialized_start=3948
+  _IDENTIFIERSINGLETESTRESULT._serialized_end=4030
+  _TESTMESSAGE._serialized_start=4032
+  _TESTMESSAGE._serialized_end=4098
+  _SINGLETESTRESULT._serialized_start=4101
+  _SINGLETESTRESULT._serialized_end=4715
+  _SINGLETESTRESULT_PROPSENTRY._serialized_start=4671
+  _SINGLETESTRESULT_PROPSENTRY._serialized_end=4715
+  _TESTRESULTMESSAGE._serialized_start=4717
+  _TESTRESULTMESSAGE._serialized_end=4784
+  _DATASETPROCESSINGRESULTMESSAGE._serialized_start=4787
+  _DATASETPROCESSINGRESULTMESSAGE._serialized_end=4940
+  _DATASETROWMODIFICATIONRESULT._serialized_start=4943
+  _DATASETROWMODIFICATIONRESULT._serialized_end=5122
+  _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY._serialized_start=5070
+  _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY._serialized_end=5122
+  _TESTSUITERESULTMESSAGE._serialized_start=5124
+  _TESTSUITERESULTMESSAGE._serialized_end=5250
+  _ARTIFACTREF._serialized_start=5252
+  _ARTIFACTREF._serialized_end=5330
+  _CHUNK._serialized_start=5332
+  _CHUNK._serialized_end=5356
+  _UPLOADSTATUS._serialized_start=5358
+  _UPLOADSTATUS._serialized_end=5406
+  _MLWORKERERRORINFO._serialized_start=5408
+  _MLWORKERERRORINFO._serialized_end=5457
+  _SUITEINPUT._serialized_start=5460
+  _SUITEINPUT._serialized_end=5624
+  _MODELMETA._serialized_start=5626
+  _MODELMETA._serialized_end=5677
+  _DATASETMETA._serialized_start=5679
+  _DATASETMETA._serialized_end=5724
+  _GENERATETESTSUITEREQUEST._serialized_start=5726
+  _GENERATETESTSUITEREQUEST._serialized_end=5809
+  _GENERATETESTSUITERESPONSE._serialized_start=5811
+  _GENERATETESTSUITERESPONSE._serialized_end=5876
+  _GENERATEDTEST._serialized_start=5878
+  _GENERATEDTEST._serialized_end=5956
+  _GENERATEDTESTINPUT._serialized_start=5958
+  _GENERATEDTESTINPUT._serialized_end=6025
+  _CATALOGRESPONSE._serialized_start=6028
+  _CATALOGRESPONSE._serialized_end=6463
+  _CATALOGRESPONSE_TESTSENTRY._serialized_start=6222
+  _CATALOGRESPONSE_TESTSENTRY._serialized_end=6288
+  _CATALOGRESPONSE_SLICESENTRY._serialized_start=6290
+  _CATALOGRESPONSE_SLICESENTRY._serialized_end=6371
+  _CATALOGRESPONSE_TRANSFORMATIONSENTRY._serialized_start=6373
+  _CATALOGRESPONSE_TRANSFORMATIONSENTRY._serialized_end=6463
+  _FUNCTIONMETA._serialized_start=6466
+  _FUNCTIONMETA._serialized_end=6680
+  _DATASETPROCESSFUNCTIONMETA._serialized_start=6683
+  _DATASETPROCESSFUNCTIONMETA._serialized_end=6991
+  _TESTFUNCTIONARGUMENT._serialized_start=6993
+  _TESTFUNCTIONARGUMENT._serialized_end=7096
+  _COMPARISONCLAUSE._serialized_start=7099
+  _COMPARISONCLAUSE._serialized_end=7239
+  _GENERATEQUERYBASEDSLICEREQUEST._serialized_start=7241
+  _GENERATEQUERYBASEDSLICEREQUEST._serialized_end=7327
+  _GENERATEQUERYBASEDSLICERESPONSE._serialized_start=7329
+  _GENERATEQUERYBASEDSLICERESPONSE._serialized_end=7374
+  _MLWORKER._serialized_start=7676
+  _MLWORKER._serialized_end=8685
 # @@protoc_insertion_point(module_scope)
```

### Comparing `giskard-1.9.1/giskard/ml_worker/generated/ml_worker_pb2_grpc.py` & `giskard-2.0.0b1/giskard/ml_worker/generated/ml_worker_pb2_grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,28 +16,33 @@
             channel: A grpc.Channel.
         """
         self.getInfo = channel.unary_unary(
                 '/worker.MLWorker/getInfo',
                 request_serializer=ml__worker__pb2.MLWorkerInfoRequest.SerializeToString,
                 response_deserializer=ml__worker__pb2.MLWorkerInfo.FromString,
                 )
-        self.runTest = channel.unary_unary(
-                '/worker.MLWorker/runTest',
-                request_serializer=ml__worker__pb2.RunTestRequest.SerializeToString,
-                response_deserializer=ml__worker__pb2.TestResultMessage.FromString,
-                )
         self.runAdHocTest = channel.unary_unary(
                 '/worker.MLWorker/runAdHocTest',
                 request_serializer=ml__worker__pb2.RunAdHocTestRequest.SerializeToString,
                 response_deserializer=ml__worker__pb2.TestResultMessage.FromString,
                 )
+        self.datasetProcessing = channel.unary_unary(
+                '/worker.MLWorker/datasetProcessing',
+                request_serializer=ml__worker__pb2.DatasetProcessingRequest.SerializeToString,
+                response_deserializer=ml__worker__pb2.DatasetProcessingResultMessage.FromString,
+                )
+        self.runTestSuite = channel.unary_unary(
+                '/worker.MLWorker/runTestSuite',
+                request_serializer=ml__worker__pb2.RunTestSuiteRequest.SerializeToString,
+                response_deserializer=ml__worker__pb2.TestSuiteResultMessage.FromString,
+                )
         self.runModel = channel.unary_unary(
                 '/worker.MLWorker/runModel',
                 request_serializer=ml__worker__pb2.RunModelRequest.SerializeToString,
-                response_deserializer=ml__worker__pb2.RunModelResponse.FromString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.runModelForDataFrame = channel.unary_unary(
                 '/worker.MLWorker/runModelForDataFrame',
                 request_serializer=ml__worker__pb2.RunModelForDataFrameRequest.SerializeToString,
                 response_deserializer=ml__worker__pb2.RunModelForDataFrameResponse.FromString,
                 )
         self.explain = channel.unary_unary(
@@ -51,47 +56,58 @@
                 response_deserializer=ml__worker__pb2.ExplainTextResponse.FromString,
                 )
         self.echo = channel.unary_unary(
                 '/worker.MLWorker/echo',
                 request_serializer=ml__worker__pb2.EchoMsg.SerializeToString,
                 response_deserializer=ml__worker__pb2.EchoMsg.FromString,
                 )
-        self.upload = channel.stream_stream(
-                '/worker.MLWorker/upload',
-                request_serializer=ml__worker__pb2.FileUploadRequest.SerializeToString,
-                response_deserializer=ml__worker__pb2.UploadStatus.FromString,
+        self.generateTestSuite = channel.unary_unary(
+                '/worker.MLWorker/generateTestSuite',
+                request_serializer=ml__worker__pb2.GenerateTestSuiteRequest.SerializeToString,
+                response_deserializer=ml__worker__pb2.GenerateTestSuiteResponse.FromString,
                 )
-        self.getTestRegistry = channel.unary_unary(
-                '/worker.MLWorker/getTestRegistry',
+        self.stopWorker = channel.unary_unary(
+                '/worker.MLWorker/stopWorker',
                 request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=ml__worker__pb2.TestRegistryResponse.FromString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
-        self.filterDataset = channel.stream_stream(
-                '/worker.MLWorker/filterDataset',
-                request_serializer=ml__worker__pb2.FilterDatasetRequest.SerializeToString,
-                response_deserializer=ml__worker__pb2.FilterDatasetResponse.FromString,
+        self.getCatalog = channel.unary_unary(
+                '/worker.MLWorker/getCatalog',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=ml__worker__pb2.CatalogResponse.FromString,
+                )
+        self.generateQueryBasedSlicingFunction = channel.unary_unary(
+                '/worker.MLWorker/generateQueryBasedSlicingFunction',
+                request_serializer=ml__worker__pb2.GenerateQueryBasedSliceRequest.SerializeToString,
+                response_deserializer=ml__worker__pb2.GenerateQueryBasedSliceResponse.FromString,
                 )
 
 
 class MLWorkerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def getInfo(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def runTest(self, request, context):
+    def runAdHocTest(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def runAdHocTest(self, request, context):
+    def datasetProcessing(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def runTestSuite(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def runModel(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -119,54 +135,65 @@
 
     def echo(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def upload(self, request_iterator, context):
+    def generateTestSuite(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def stopWorker(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def getTestRegistry(self, request, context):
+    def getCatalog(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def filterDataset(self, request_iterator, context):
+    def generateQueryBasedSlicingFunction(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_MLWorkerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'getInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.getInfo,
                     request_deserializer=ml__worker__pb2.MLWorkerInfoRequest.FromString,
                     response_serializer=ml__worker__pb2.MLWorkerInfo.SerializeToString,
             ),
-            'runTest': grpc.unary_unary_rpc_method_handler(
-                    servicer.runTest,
-                    request_deserializer=ml__worker__pb2.RunTestRequest.FromString,
-                    response_serializer=ml__worker__pb2.TestResultMessage.SerializeToString,
-            ),
             'runAdHocTest': grpc.unary_unary_rpc_method_handler(
                     servicer.runAdHocTest,
                     request_deserializer=ml__worker__pb2.RunAdHocTestRequest.FromString,
                     response_serializer=ml__worker__pb2.TestResultMessage.SerializeToString,
             ),
+            'datasetProcessing': grpc.unary_unary_rpc_method_handler(
+                    servicer.datasetProcessing,
+                    request_deserializer=ml__worker__pb2.DatasetProcessingRequest.FromString,
+                    response_serializer=ml__worker__pb2.DatasetProcessingResultMessage.SerializeToString,
+            ),
+            'runTestSuite': grpc.unary_unary_rpc_method_handler(
+                    servicer.runTestSuite,
+                    request_deserializer=ml__worker__pb2.RunTestSuiteRequest.FromString,
+                    response_serializer=ml__worker__pb2.TestSuiteResultMessage.SerializeToString,
+            ),
             'runModel': grpc.unary_unary_rpc_method_handler(
                     servicer.runModel,
                     request_deserializer=ml__worker__pb2.RunModelRequest.FromString,
-                    response_serializer=ml__worker__pb2.RunModelResponse.SerializeToString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'runModelForDataFrame': grpc.unary_unary_rpc_method_handler(
                     servicer.runModelForDataFrame,
                     request_deserializer=ml__worker__pb2.RunModelForDataFrameRequest.FromString,
                     response_serializer=ml__worker__pb2.RunModelForDataFrameResponse.SerializeToString,
             ),
             'explain': grpc.unary_unary_rpc_method_handler(
@@ -180,28 +207,33 @@
                     response_serializer=ml__worker__pb2.ExplainTextResponse.SerializeToString,
             ),
             'echo': grpc.unary_unary_rpc_method_handler(
                     servicer.echo,
                     request_deserializer=ml__worker__pb2.EchoMsg.FromString,
                     response_serializer=ml__worker__pb2.EchoMsg.SerializeToString,
             ),
-            'upload': grpc.stream_stream_rpc_method_handler(
-                    servicer.upload,
-                    request_deserializer=ml__worker__pb2.FileUploadRequest.FromString,
-                    response_serializer=ml__worker__pb2.UploadStatus.SerializeToString,
+            'generateTestSuite': grpc.unary_unary_rpc_method_handler(
+                    servicer.generateTestSuite,
+                    request_deserializer=ml__worker__pb2.GenerateTestSuiteRequest.FromString,
+                    response_serializer=ml__worker__pb2.GenerateTestSuiteResponse.SerializeToString,
+            ),
+            'stopWorker': grpc.unary_unary_rpc_method_handler(
+                    servicer.stopWorker,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
-            'getTestRegistry': grpc.unary_unary_rpc_method_handler(
-                    servicer.getTestRegistry,
+            'getCatalog': grpc.unary_unary_rpc_method_handler(
+                    servicer.getCatalog,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=ml__worker__pb2.TestRegistryResponse.SerializeToString,
+                    response_serializer=ml__worker__pb2.CatalogResponse.SerializeToString,
             ),
-            'filterDataset': grpc.stream_stream_rpc_method_handler(
-                    servicer.filterDataset,
-                    request_deserializer=ml__worker__pb2.FilterDatasetRequest.FromString,
-                    response_serializer=ml__worker__pb2.FilterDatasetResponse.SerializeToString,
+            'generateQueryBasedSlicingFunction': grpc.unary_unary_rpc_method_handler(
+                    servicer.generateQueryBasedSlicingFunction,
+                    request_deserializer=ml__worker__pb2.GenerateQueryBasedSliceRequest.FromString,
+                    response_serializer=ml__worker__pb2.GenerateQueryBasedSliceResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'worker.MLWorker', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -223,44 +255,61 @@
         return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/getInfo',
             ml__worker__pb2.MLWorkerInfoRequest.SerializeToString,
             ml__worker__pb2.MLWorkerInfo.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def runTest(request,
+    def runAdHocTest(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/runTest',
-            ml__worker__pb2.RunTestRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/runAdHocTest',
+            ml__worker__pb2.RunAdHocTestRequest.SerializeToString,
             ml__worker__pb2.TestResultMessage.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def runAdHocTest(request,
+    def datasetProcessing(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/runAdHocTest',
-            ml__worker__pb2.RunAdHocTestRequest.SerializeToString,
-            ml__worker__pb2.TestResultMessage.FromString,
+        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/datasetProcessing',
+            ml__worker__pb2.DatasetProcessingRequest.SerializeToString,
+            ml__worker__pb2.DatasetProcessingResultMessage.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def runTestSuite(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/runTestSuite',
+            ml__worker__pb2.RunTestSuiteRequest.SerializeToString,
+            ml__worker__pb2.TestSuiteResultMessage.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def runModel(request,
             target,
             options=(),
@@ -269,15 +318,15 @@
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/runModel',
             ml__worker__pb2.RunModelRequest.SerializeToString,
-            ml__worker__pb2.RunModelResponse.FromString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def runModelForDataFrame(request,
             target,
             options=(),
@@ -342,56 +391,73 @@
         return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/echo',
             ml__worker__pb2.EchoMsg.SerializeToString,
             ml__worker__pb2.EchoMsg.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def upload(request_iterator,
+    def generateTestSuite(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/worker.MLWorker/upload',
-            ml__worker__pb2.FileUploadRequest.SerializeToString,
-            ml__worker__pb2.UploadStatus.FromString,
+        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/generateTestSuite',
+            ml__worker__pb2.GenerateTestSuiteRequest.SerializeToString,
+            ml__worker__pb2.GenerateTestSuiteResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def stopWorker(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/stopWorker',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def getTestRegistry(request,
+    def getCatalog(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/getTestRegistry',
+        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/getCatalog',
             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ml__worker__pb2.TestRegistryResponse.FromString,
+            ml__worker__pb2.CatalogResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def filterDataset(request_iterator,
+    def generateQueryBasedSlicingFunction(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/worker.MLWorker/filterDataset',
-            ml__worker__pb2.FilterDatasetRequest.SerializeToString,
-            ml__worker__pb2.FilterDatasetResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/worker.MLWorker/generateQueryBasedSlicingFunction',
+            ml__worker__pb2.GenerateQueryBasedSliceRequest.SerializeToString,
+            ml__worker__pb2.GenerateQueryBasedSliceResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `giskard-1.9.1/giskard/ml_worker/testing/drift_tests.py` & `giskard-2.0.0b1/giskard/testing/tests/drift.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,788 +1,776 @@
-import typing
-from typing import Union
-
 import re
+import typing
 import uuid
 from collections import Counter
+from typing import Optional, List
 
 import numpy as np
 import pandas as pd
 from scipy.stats import chi2, ks_2samp
 from scipy.stats.stats import Ks_2sampResult, wasserstein_distance
 
-from giskard.ml_worker.core.giskard_dataset import GiskardDataset
-from giskard.ml_worker.core.model import GiskardModel
-from giskard.ml_worker.generated.ml_worker_pb2 import SingleTestResult, TestMessage, TestMessageType
-from giskard.ml_worker.testing.abstract_test_collection import AbstractTestCollection
-
-
-class DriftTests(AbstractTestCollection):
-    # Class Variable
-    other_modalities_pattern = "^other_modalities_[a-z0-9]{32}$"
-
-    @staticmethod
-    def _calculate_psi(category, actual_distribution, expected_distribution):
-        # To use log and avoid zero distribution probability,
-        # we bound distribution probability by min_distribution_probability
-        min_distribution_probability = 0.0001
-
-        expected_distribution_bounded = max(
-            expected_distribution[category], min_distribution_probability
-        )
-        actual_distribution_bounded = max(
-            actual_distribution[category], min_distribution_probability
-        )
-        modality_psi = (expected_distribution_bounded - actual_distribution_bounded) * np.log(
-            expected_distribution_bounded / actual_distribution_bounded
+from giskard.datasets.base import Dataset
+from giskard.ml_worker.testing.registry.decorators import test
+from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction
+from giskard.ml_worker.testing.test_result import TestResult, TestMessage, TestMessageLevel
+from giskard.ml_worker.testing.utils import check_slice_not_empty
+from giskard.ml_worker.testing.utils import validate_classification_label
+from giskard.models.base import BaseModel
+
+other_modalities_pattern = "^other_modalities_[a-z0-9]{32}$"
+
+
+def _calculate_psi(category, actual_distribution, expected_distribution):
+    # To use log and avoid zero distribution probability,
+    # we bound distribution probability by min_distribution_probability
+    min_distribution_probability = 0.0001
+
+    expected_distribution_bounded = max(expected_distribution[category], min_distribution_probability)
+    actual_distribution_bounded = max(actual_distribution[category], min_distribution_probability)
+    modality_psi = (expected_distribution_bounded - actual_distribution_bounded) * np.log(
+        expected_distribution_bounded / actual_distribution_bounded
+    )
+    return modality_psi
+
+
+def _calculate_frequencies(actual_series, reference_series, max_categories=None):
+    all_modalities = list(set(reference_series).union(set(actual_series)))
+    if max_categories is not None and len(all_modalities) > max_categories:
+        var_count_expected = dict(Counter(reference_series).most_common(max_categories))
+        other_modalities_key = "other_modalities_" + uuid.uuid1().hex
+        var_count_expected[other_modalities_key] = len(reference_series) - sum(var_count_expected.values())
+        categories_list = list(var_count_expected.keys())
+
+        var_count_actual = Counter(actual_series)
+        # For test data, we take the same category names as expected_data
+        var_count_actual = {i: var_count_actual[i] for i in categories_list}
+        var_count_actual[other_modalities_key] = len(actual_series) - sum(var_count_actual.values())
+
+        all_modalities = categories_list
+    else:
+        var_count_expected = Counter(reference_series)
+        var_count_actual = Counter(actual_series)
+    expected_frequencies = np.array([var_count_expected[i] for i in all_modalities])
+    actual_frequencies = np.array([var_count_actual[i] for i in all_modalities])
+    return all_modalities, actual_frequencies, expected_frequencies
+
+
+def _calculate_drift_psi(actual_series, reference_series, max_categories):
+    (
+        all_modalities,
+        actual_frequencies,
+        expected_frequencies,
+    ) = _calculate_frequencies(actual_series, reference_series, max_categories)
+    expected_distribution = expected_frequencies / len(reference_series)
+    actual_distribution = actual_frequencies / len(actual_series)
+    total_psi = 0
+    output_data = pd.DataFrame(columns=["Modality", "Reference_distribution", "Actual_distribution", "Psi"])
+    for category in range(len(all_modalities)):
+        modality_psi = _calculate_psi(category, actual_distribution, expected_distribution)
+
+        total_psi += modality_psi
+        row = {
+            "Modality": all_modalities[category],
+            "Reference_distribution": expected_distribution[category],
+            "Actual_distribution": expected_distribution[category],
+            "Psi": modality_psi,
+        }
+
+        output_data = output_data.append(pd.Series(row), ignore_index=True)
+    return total_psi, output_data
+
+
+def _calculate_ks(actual_series, reference_series) -> Ks_2sampResult:
+    return ks_2samp(reference_series, actual_series)
+
+
+def _calculate_earth_movers_distance(actual_series, reference_series):
+    unique_reference = np.unique(reference_series)
+    unique_actual = np.unique(actual_series)
+    sample_space = list(set(unique_reference).union(set(unique_actual)))
+    val_max = max(sample_space)
+    val_min = min(sample_space)
+    if val_max == val_min:
+        metric = 0
+    else:
+        # Normalizing reference_series and actual_series for comparison purposes
+        reference_series = (reference_series - val_min) / (val_max - val_min)
+        actual_series = (actual_series - val_min) / (val_max - val_min)
+
+        metric = wasserstein_distance(reference_series, actual_series)
+    return metric
+
+
+def _calculate_chi_square(actual_series, reference_series, max_categories):
+    (
+        all_modalities,
+        actual_frequencies,
+        expected_frequencies,
+    ) = _calculate_frequencies(actual_series, reference_series, max_categories)
+    chi_square = 0
+    # it's necessary for comparison purposes to normalize expected_frequencies
+    # so that reference and actual has the same size
+    # See https://github.com/scipy/scipy/blob/v1.8.0/scipy/stats/_stats_py.py#L6787
+    k_norm = actual_series.shape[0] / reference_series.shape[0]
+    output_data = pd.DataFrame(columns=["Modality", "Reference_frequencies", "Actual_frequencies", "Chi_square"])
+    for i in range(len(all_modalities)):
+        chi_square_value = (actual_frequencies[i] - expected_frequencies[i] * k_norm) ** 2 / (
+                expected_frequencies[i] * k_norm
         )
-        return modality_psi
-
-    @staticmethod
-    def _calculate_frequencies(actual_series, reference_series, max_categories=None):
-        all_modalities = list(set(reference_series).union(set(actual_series)))
-        if max_categories is not None and len(all_modalities) > max_categories:
-            var_count_expected = dict(Counter(reference_series).most_common(max_categories))
-            other_modalities_key = "other_modalities_" + uuid.uuid1().hex
-            var_count_expected[other_modalities_key] = len(reference_series) - sum(
-                var_count_expected.values()
-            )
-            categories_list = list(var_count_expected.keys())
-
-            var_count_actual = Counter(actual_series)
-            # For test data, we take the same category names as expected_data
-            var_count_actual = {i: var_count_actual[i] for i in categories_list}
-            var_count_actual[other_modalities_key] = len(actual_series) - sum(
-                var_count_actual.values()
-            )
+        chi_square += chi_square_value
 
-            all_modalities = categories_list
-        else:
-            var_count_expected = Counter(reference_series)
-            var_count_actual = Counter(actual_series)
-        expected_frequencies = np.array([var_count_expected[i] for i in all_modalities])
-        actual_frequencies = np.array([var_count_actual[i] for i in all_modalities])
-        return all_modalities, actual_frequencies, expected_frequencies
-
-    @staticmethod
-    def _calculate_drift_psi(actual_series, reference_series, max_categories):
-        (
-            all_modalities,
-            actual_frequencies,
-            expected_frequencies,
-        ) = DriftTests._calculate_frequencies(actual_series, reference_series, max_categories)
-        expected_distribution = expected_frequencies / len(reference_series)
-        actual_distribution = actual_frequencies / len(actual_series)
-        total_psi = 0
-        output_data = pd.DataFrame(
-            columns=["Modality", "Reference_distribution", "Actual_distribution", "Psi"]
-        )
-        for category in range(len(all_modalities)):
-            modality_psi = DriftTests._calculate_psi(
-                category, actual_distribution, expected_distribution
-            )
+        row = {
+            "Modality": all_modalities[i],
+            "Reference_frequencies": expected_frequencies[i],
+            "Actual_frequencies": actual_frequencies[i],
+            "Chi_square": chi_square_value,
+        }
+
+        output_data = output_data.append(pd.Series(row), ignore_index=True)
+    # if reference_series and actual_series has only one modality it turns nan (len(all_modalities)=1)
+    if len(all_modalities) > 1:
+        chi_cdf = chi2.cdf(chi_square, len(all_modalities) - 1)
+        p_value = 1 - chi_cdf if chi_cdf != 0 else 0
+    else:
+        p_value = 0
+    return chi_square, p_value, output_data
+
+
+def _validate_feature_type(gsk_dataset, column_name, feature_type):
+    assert (
+            gsk_dataset.column_types[column_name] == feature_type
+    ), f'Column "{column_name}" is not of type "{feature_type}"'
 
-            total_psi += modality_psi
-            row = {
-                "Modality": all_modalities[category],
-                "Reference_distribution": expected_distribution[category],
-                "Actual_distribution": expected_distribution[category],
-                "Psi": modality_psi,
-            }
-
-            output_data = output_data.append(pd.Series(row), ignore_index=True)
-        return total_psi, output_data
-
-    @staticmethod
-    def _calculate_ks(actual_series, reference_series) -> Ks_2sampResult:
-        return ks_2samp(reference_series, actual_series)
-
-    @staticmethod
-    def _calculate_earth_movers_distance(actual_series, reference_series):
-        unique_reference = np.unique(reference_series)
-        unique_actual = np.unique(actual_series)
-        sample_space = list(set(unique_reference).union(set(unique_actual)))
-        val_max = max(sample_space)
-        val_min = min(sample_space)
-        if val_max == val_min:
-            metric = 0
-        else:
-            # Normalizing reference_series and actual_series for comparison purposes
-            reference_series = (reference_series - val_min) / (val_max - val_min)
-            actual_series = (actual_series - val_min) / (val_max - val_min)
-
-            metric = wasserstein_distance(reference_series, actual_series)
-        return metric
-
-    @staticmethod
-    def _calculate_chi_square(actual_series, reference_series, max_categories):
-        (
-            all_modalities,
-            actual_frequencies,
-            expected_frequencies,
-        ) = DriftTests._calculate_frequencies(actual_series, reference_series, max_categories)
-        chi_square = 0
-        # it's necessary for comparison purposes to normalize expected_frequencies
-        # so that reference and actual has the same size
-        # See https://github.com/scipy/scipy/blob/v1.8.0/scipy/stats/_stats_py.py#L6787
-        k_norm = actual_series.shape[0] / reference_series.shape[0]
-        output_data = pd.DataFrame(
-            columns=["Modality", "Reference_frequencies", "Actual_frequencies", "Chi_square"]
-        )
-        for i in range(len(all_modalities)):
-            chi_square_value = (actual_frequencies[i] - expected_frequencies[i] * k_norm) ** 2 / (
-                expected_frequencies[i] * k_norm
-            )
-            chi_square += chi_square_value
 
-            row = {
-                "Modality": all_modalities[i],
-                "Reference_frequencies": expected_frequencies[i],
-                "Actual_frequencies": actual_frequencies[i],
-                "Chi_square": chi_square_value,
-            }
-
-            output_data = output_data.append(pd.Series(row), ignore_index=True)
-        # if reference_series and actual_series has only one modality it turns nan (len(all_modalities)=1)
-        if len(all_modalities) > 1:
-            chi_cdf = chi2.cdf(chi_square, len(all_modalities) - 1)
-            p_value = 1 - chi_cdf if chi_cdf != 0 else 0
-        else:
-            p_value = 0
-        return chi_square, p_value, output_data
-
-    @staticmethod
-    def _validate_column_type(gsk_dataset, column_name, column_type):
-        assert (
-            gsk_dataset.feature_types[column_name] == column_type
-        ), f'Column "{column_name}" is not of type "{column_type}"'
-
-    @staticmethod
-    def _validate_column_name(actual_ds, reference_ds, column_name):
-        assert (
+def _validate_column_name(actual_ds, reference_ds, column_name):
+    assert (
             column_name in actual_ds.columns
-        ), f'"{column_name}" is not a column of Actual Dataset Columns: {", ".join(actual_ds.columns)}'
-        assert (
+    ), f'"{column_name}" is not a column of Actual Dataset Columns: {", ".join(actual_ds.columns)}'
+    assert (
             column_name in reference_ds.columns
-        ), f'"{column_name}" is not a column of Reference Dataset Columns: {", ".join(reference_ds.columns)}'
-
-    @staticmethod
-    def _validate_series_notempty(actual_series, reference_series):
-        if actual_series.empty:
-            raise ValueError("Actual Series computed from the column is empty")
-        if reference_series.empty:
-            raise ValueError("Reference Series computed from the column is empty")
-
-    def _extract_series(self, actual_ds, reference_ds, column_name, column_type):
-        actual_ds.df.reset_index(drop=True, inplace=True)
-        reference_ds.df.reset_index(drop=True, inplace=True)
-        self._validate_column_name(actual_ds, reference_ds, column_name)
-        self._validate_column_type(actual_ds, column_name, column_type)
-        self._validate_column_type(reference_ds, column_name, column_type)
-        actual_series = actual_ds.df[column_name]
-        reference_series = reference_ds.df[column_name]
-        self._validate_series_notempty(actual_series, reference_series)
-        return actual_series, reference_series
-
-    def test_drift_psi(
-        self,
-        reference_ds: GiskardDataset,
-        actual_ds: GiskardDataset,
-        column_name: str,
-        threshold=0.2,
-        max_categories: int = 20,
-        psi_contribution_percent: float = 0.2,
-    ) -> SingleTestResult:
-        """
-        Test if the PSI score between the actual and reference datasets is below the threshold for
-        a given categorical feature
-
-        Example : The test is passed when the  PSI score of gender between reference and actual sets is below 0.2
-
-        Args:
-            actual_ds(GiskardDataset):
-                Actual dataset to compute the test
-            reference_ds(GiskardDataset):
-                Reference dataset to compute the test
-            column_name(str):
-                Name of column with categorical feature
-            threshold(float:
-                Threshold value for PSI
-            max_categories:
-                the maximum categories to compute the PSI score
-            psi_contribution_percent:
-                the ratio between the PSI score of a given category over the total PSI score
-                of the categorical variable. If there is a drift, the test provides all the
-                categories that have a PSI contribution over than this ratio.
-
-        Returns:
-            actual_slices_size:
-                Length of rows with given categorical feature in actual slice
-            reference_slices_size:
-                Length of rows with given categorical feature in reference slice
-            metric:
-                The total psi score between the actual and reference datasets
-            passed:
-                TRUE if total_psi <= threshold
-        """
-        actual_series, reference_series = self._extract_series(
-            actual_ds, reference_ds, column_name, "category"
-        )
-
-        messages, passed, total_psi = self._test_series_drift_psi(
-            actual_series,
-            reference_series,
-            "data",
-            max_categories,
-            psi_contribution_percent,
-            threshold,
-        )
-
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_series)],
-                reference_slices_size=[len(reference_series)],
-                passed=passed,
-                metric=total_psi,
-                messages=messages,
-            )
-        )
-
-    def test_drift_chi_square(
-        self,
-        reference_ds: GiskardDataset,
-        actual_ds: GiskardDataset,
-        column_name: str,
-        threshold=0.05,
-        max_categories: int = 20,
-        chi_square_contribution_percent: float = 0.2,
-    ) -> SingleTestResult:
-        """
-        Test if the p-value of the chi square test between the actual and reference datasets is
-        above the threshold for a given categorical feature
-
-        Example : The test is passed when the pvalue of the chi square test of the categorical variable between
-         reference and actual sets is higher than 0.05. It means that chi square test cannot be rejected at 5% level
-         and that we cannot assume drift for this variable.
-
-        Args:
-            actual_ds(GiskardDataset):
-                Actual dataset to compute the test
-            reference_ds(GiskardDataset):
-                Reference dataset to compute the test
-            column_name(str):
-                Name of column with categorical feature
-            threshold(float):
-                Threshold for p-value of chi-square
-            max_categories:
-                the maximum categories to compute the chi square
-            chi_square_contribution_percent:
-                the ratio between the Chi-Square value of a given category over the total Chi-Square
-                value of the categorical variable. If there is a drift, the test provides all the
-                categories that have a PSI contribution over than this ratio.
-
-        Returns:
-            actual_slices_size:
-                Length of rows with given categorical feature in actual slice
-            reference_slices_size:
-                Length of rows with given categorical feature in reference slice
-            metric:
-                The pvalue of chi square test
-            passed:
-                TRUE if metric > threshold
-        """
-        actual_series, reference_series = self._extract_series(
-            actual_ds, reference_ds, column_name, "category"
-        )
-
-        messages, p_value, passed = self._test_series_drift_chi(
-            actual_series,
-            reference_series,
-            "data",
-            chi_square_contribution_percent,
-            max_categories,
-            threshold,
-        )
-
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_series)],
-                reference_slices_size=[len(reference_series)],
-                passed=passed,
-                metric=p_value,
-                messages=messages,
-            )
-        )
-
-    def test_drift_ks(
-        self,
-        reference_ds: GiskardDataset,
-        actual_ds: GiskardDataset,
-        column_name: str,
-        threshold=0.05,
-    ) -> SingleTestResult:
-        """
-        Test if the pvalue of the KS test between the actual and reference datasets is above
-        the threshold for a given numerical feature
-
-        Example : The test is passed when the pvalue of the KS test of the numerical variable
-        between the actual and reference datasets is higher than 0.05. It means that the KS test
-        cannot be rejected at 5% level and that we cannot assume drift for this variable.
-
-        Args:
-            actual_ds(GiskardDataset):
-               Actual dataset to compute the test
-            reference_ds(GiskardDataset):
-                Reference dataset to compute the test
-            column_name(str):
-                Name of column with numerical feature
-            threshold:
-                Threshold for p-value of KS test
-
-        Returns:
-            actual_slices_size:
-                Length of rows with given numerical feature in actual slice
-            reference_slices_size:
-                Length of rows with given numerical feature in reference slice
-            metric:
-                The pvalue of KS test
-            passed:
-                TRUE if metric >= threshold
-        """
-        actual_series, reference_series = self._extract_series(
-            actual_ds, reference_ds, column_name, "numeric"
-        )
-
-        result = self._calculate_ks(actual_series, reference_series)
+    ), f'"{column_name}" is not a column of Reference Dataset Columns: {", ".join(reference_ds.columns)}'
 
-        passed = result.pvalue >= threshold
 
-        messages = self._generate_message_ks(passed, result, threshold, "data")
+def _validate_series_notempty(actual_series, reference_series):
+    if actual_series.empty:
+        raise ValueError("Actual Series computed from the column is empty")
+    if reference_series.empty:
+        raise ValueError("Reference Series computed from the column is empty")
+
+
+def _extract_series(actual_ds, reference_ds, column_name, feature_type):
+    _validate_column_name(actual_ds, reference_ds, column_name)
+    _validate_feature_type(actual_ds, column_name, feature_type)
+    _validate_feature_type(reference_ds, column_name, feature_type)
+    actual_series = actual_ds.df[column_name]
+    reference_series = reference_ds.df[column_name]
+    _validate_series_notempty(actual_series, reference_series)
+    return actual_series, reference_series
+
+
+@test(name='Categorical drift (PSI)')
+def test_drift_psi(actual_dataset: Dataset, reference_dataset: Dataset, column_name: str,
+                   slicing_function: SlicingFunction = None,
+                   threshold: float = 0.2, max_categories: int = 20,
+                   psi_contribution_percent: float = 0.2) -> TestResult:
+    """
+    Test if the PSI score between the actual and reference datasets is below the threshold for
+    a given categorical feature
+
+    Example : The test is passed when the  PSI score of gender between reference and actual sets is below 0.2
+
+    Args:
+        actual_dataset(Dataset):
+            Actual dataset used to compute the test
+        reference_dataset(Dataset):
+            Reference dataset used to compute the test
+        column_name(str):
+            Name of column with categorical feature
+        slicing_function(Optional[SlicingFunction]):
+          Slicing function to be applied on both actual and reference datasets
+        threshold(Optional[float]):
+            Threshold value for PSI
+        max_categories:
+            the maximum categories to compute the PSI score
+        psi_contribution_percent:
+            the ratio between the PSI score of a given category over the total PSI score
+            of the categorical variable. If there is a drift, the test provides all the
+            categories that have a PSI contribution over than this ratio.
+
+    Returns:
+        actual_slices_size:
+            Length of rows with given categorical feature in actual slice
+        reference_slices_size:
+            Length of rows with given categorical feature in reference slice
+        metric:
+            The total psi score between the actual and reference datasets
+        passed:
+            TRUE if total_psi <= threshold
+    """
+    if slicing_function:
+        test_name = "test_drift_psi"
+        actual_dataset = actual_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
+        reference_dataset = reference_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
+
+    actual_series, reference_series = _extract_series(actual_dataset,
+                                                      reference_dataset,
+                                                      column_name, "category")
 
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_series)],
-                reference_slices_size=[len(reference_series)],
-                passed=passed,
-                metric=result.pvalue,
-                messages=messages,
-            )
-        )
-
-    def test_drift_earth_movers_distance(
-        self,
-        reference_ds: GiskardDataset,
-        actual_ds: GiskardDataset,
-        column_name: str,
-        threshold: float = 0.2,
-    ) -> SingleTestResult:
-        """
-        Test if the earth movers distance between the actual and reference datasets is
-        below the threshold for a given numerical feature
-
-        Example : The test is passed when the earth movers distance of the numerical
-         variable between the actual and reference datasets is lower than 0.1.
-         It means that we cannot assume drift for this variable.
-
-        Args:
-            actual_ds(GiskardDataset):
-                Actual dataset to compute the test
-            reference_ds(GiskardDataset):
-                Reference dataset to compute the test
-            column_name(str):
-                Name of column with numerical feature
-            threshold:
-                Threshold for earth movers distance
-
-        Returns:
-            actual_slices_size:
-                Length of rows with given numerical feature in actual slice
-            reference_slices_size:
-                Length of rows with given numerical feature in reference slice
-            metric:
-                The earth movers distance
-            passed:
-                TRUE if metric <= threshold
-        """
-        actual_series, reference_series = self._extract_series(
-            actual_ds, reference_ds, column_name, "numeric"
-        )
-
-        metric = self._calculate_earth_movers_distance(actual_series, reference_series)
+    messages, passed, total_psi = _test_series_drift_psi(
+        actual_series,
+        reference_series,
+        "data",
+        max_categories,
+        psi_contribution_percent,
+        threshold,
+    )
 
-        passed = metric <= threshold
+    return TestResult(
+        actual_slices_size=[len(actual_series)],
+        reference_slices_size=[len(reference_series)],
+        passed=passed,
+        metric=total_psi,
+        messages=messages,
+    )
+
+
+@test(name='Categorical drift (Chi-squared)')
+def test_drift_chi_square(actual_dataset: Dataset, reference_dataset: Dataset, column_name: str,
+                          slicing_function: SlicingFunction = None, threshold: float = 0.05,
+                          max_categories: int = 20, chi_square_contribution_percent: float = 0.2) -> TestResult:
+    """
+    Test if the p-value of the chi square test between the actual and reference datasets is
+    above the threshold for a given categorical feature
+
+    Example : The test is passed when the pvalue of the chi square test of the categorical variable between
+     reference and actual sets is higher than 0.05. It means that chi square test cannot be rejected at 5% level
+     and that we cannot assume drift for this variable.
+
+    Args:
+        actual_dataset(Dataset):
+            Actual dataset used to compute the test
+        reference_dataset(Dataset):
+            Reference dataset used to compute the test
+        column_name(str):
+            Name of column with categorical feature
+        slicing_function(Optional[SlicingFunction]):
+          Slicing function to be applied on both actual and reference datasets
+        threshold(Optional[float]):
+            Threshold for p-value of chi-square
+        max_categories:
+            the maximum categories to compute the chi square
+        chi_square_contribution_percent:
+            the ratio between the Chi-Square value of a given category over the total Chi-Square
+            value of the categorical variable. If there is a drift, the test provides all the
+            categories that have a PSI contribution over than this ratio.
+
+    Returns:
+        actual_slices_size:
+            Length of rows with given categorical feature in actual slice
+        reference_slices_size:
+            Length of rows with given categorical feature in reference slice
+        metric:
+            The pvalue of chi square test
+        passed:
+            TRUE if metric > threshold
+    """
+    if slicing_function:
+        test_name = "test_drift_chi_square"
+        actual_dataset = actual_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
+        reference_dataset = reference_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
+
+    actual_series, reference_series = _extract_series(actual_dataset,
+                                                      reference_dataset,
+                                                      column_name, "category")
 
-        messages: Union[typing.List[TestMessage], None] = None
+    messages, p_value, passed = _test_series_drift_chi(
+        actual_series,
+        reference_series,
+        "data",
+        chi_square_contribution_percent,
+        max_categories,
+        threshold,
+    )
 
-        if not passed:
-            messages = [
-                TestMessage(
-                    type=TestMessageType.ERROR,
-                    text=f"The data is drifting (metric is equal to {np.round(metric, 9)} and is below the test risk level {threshold}) ",
-                )
-            ]
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_series)],
-                reference_slices_size=[len(reference_series)],
-                passed=True if threshold is None else passed,
-                metric=metric,
-                messages=messages,
+    return TestResult(
+        actual_slices_size=[len(actual_series)],
+        reference_slices_size=[len(reference_series)],
+        passed=passed,
+        metric=p_value,
+        messages=messages,
+    )
+
+
+@test(name='Numerical drift (Kolmogorov-Smirnov)')
+def test_drift_ks(actual_dataset: Dataset, reference_dataset: Dataset, column_name: str,
+                  slicing_function: SlicingFunction = None,
+                  threshold: float = 0.05) -> TestResult:
+    """
+    Test if the pvalue of the KS test between the actual and reference datasets is above
+    the threshold for a given numerical feature
+
+    Example : The test is passed when the pvalue of the KS test of the numerical variable
+    between the actual and reference datasets is higher than 0.05. It means that the KS test
+    cannot be rejected at 5% level and that we cannot assume drift for this variable.
+
+    Args:
+        actual_dataset(Dataset):
+           Actual dataset used to compute the test
+        reference_dataset(Dataset):
+            Reference dataset used to compute the test
+        column_name(str):
+            Name of column with numerical feature
+        slicing_function(Optional[SlicingFunction]):
+          Slicing function to be applied on both actual and reference datasets
+        threshold(Optional[float]):
+            Threshold for p-value of KS test
+
+    Returns:
+        actual_slices_size:
+            Length of rows with given numerical feature in actual slice
+        reference_slices_size:
+            Length of rows with given numerical feature in reference slice
+        metric:
+            The pvalue of KS test
+        passed:
+            TRUE if metric >= threshold
+    """
+    if slicing_function:
+        test_name = "test_drift_ks"
+        actual_dataset = actual_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
+        reference_dataset = reference_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
+
+    actual_series, reference_series = _extract_series(actual_dataset,
+                                                      reference_dataset,
+                                                      column_name, "numeric")
+
+    result = _calculate_ks(actual_series, reference_series)
+
+    passed = bool(result.pvalue >= threshold)
+
+    messages = _generate_message_ks(passed, result, threshold, "data")
+
+    return TestResult(
+        actual_slices_size=[len(actual_series)],
+        reference_slices_size=[len(reference_series)],
+        passed=passed,
+        metric=result.pvalue,
+        messages=messages
+    )
+
+
+@test(name='Numerical drift (Earth mover\'s distance)')
+def test_drift_earth_movers_distance(actual_dataset: Dataset, reference_dataset: Dataset, column_name: str,
+                                     slicing_function: SlicingFunction = None, threshold: float = 0.2) -> TestResult:
+    """
+    Test if the earth movers distance between the actual and reference datasets is
+    below the threshold for a given numerical feature
+
+    Example : The test is passed when the earth movers distance of the numerical
+     variable between the actual and reference datasets is lower than 0.1.
+     It means that we cannot assume drift for this variable.
+
+    Args:
+        actual_dataset(Dataset):
+            Actual dataset used to compute the test
+        reference_dataset(Dataset):
+            Reference dataset used to compute the test
+        column_name(str):
+            Name of column with numerical feature
+        slicing_function(Optional[SlicingFunction]):
+            Slicing function to be applied on both actual and reference datasets
+        threshold(Optional[float]):
+            Threshold for earth movers distance
+
+    Returns:
+        actual_slices_size:
+            Length of rows with given numerical feature in actual slice
+        reference_slices_size:
+            Length of rows with given numerical feature in reference slice
+        metric:
+            The earth movers distance
+        passed:
+            TRUE if metric <= threshold
+    """
+    if slicing_function:
+        test_name = "test_drift_earth_movers_distance"
+        actual_dataset = actual_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
+        reference_dataset = reference_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
+
+    actual_series, reference_series = _extract_series(actual_dataset,
+                                                      reference_dataset,
+                                                      column_name, "numeric")
+
+    metric = _calculate_earth_movers_distance(actual_series, reference_series)
+
+    passed = bool(metric <= threshold)
+
+    messages: Optional[List[TestMessage]] = None
+
+    if not passed:
+        messages = [
+            TestMessage(
+                type=TestMessageLevel.ERROR,
+                text=f"The data is drifting (metric is equal to {np.round(metric, 9)} and is below the test risk level {threshold}) ",
             )
-        )
+        ]
+    return TestResult(
+        actual_slices_size=[len(actual_series)],
+        reference_slices_size=[len(reference_series)],
+        passed=True if threshold is None else passed,
+        metric=metric,
+        messages=messages,
+    )
+
+
+@test(name='Label drift (PSI)')
+def test_drift_prediction_psi(model: BaseModel, actual_dataset: Dataset, reference_dataset: Dataset,
+                              slicing_function: SlicingFunction = None, max_categories: int = 10,
+                              threshold: float = 0.2, psi_contribution_percent: float = 0.2):
+    """
+    Test if the PSI score between the reference and actual datasets is below the threshold
+    for the classification labels predictions
+
+    Example : The test is passed when the  PSI score of classification labels prediction
+    for females between reference and actual sets is below 0.2
+
+    Args:
+        model(BaseModel):
+            Model used to compute the test
+        actual_dataset(Dataset):
+            Actual dataset used to compute the test
+        reference_dataset(Dataset):
+            Reference dataset used to compute the test
+        slicing_function(Optional[SlicingFunction]):
+            Slicing function to be applied on both actual and reference datasets
+        threshold(Optional[float]):
+            Threshold value for PSI
+        max_categories:
+            The maximum categories to compute the PSI score
+        psi_contribution_percent:
+            The ratio between the PSI score of a given category over the total PSI score
+            of the categorical variable. If there is a drift, the test provides all the
+            categories that have a PSI contribution over than this ratio.
+
+    Returns:
+        actual_slices_size:
+            Length of actual slice tested
+        reference_slices_size:
+            Length of reference slice tested
+        passed:
+            TRUE if metric <= threshold
+        metric:
+            Total PSI value
+        messages:
+            Psi result message
+    """
+    if slicing_function:
+        test_name = "test_drift_prediction_psi"
+        actual_dataset = actual_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
+        reference_dataset = reference_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
+
+    prediction_reference = pd.Series(model.predict(reference_dataset).prediction)
+    prediction_actual = pd.Series(model.predict(actual_dataset).prediction)
+    messages, passed, total_psi = _test_series_drift_psi(
+        prediction_actual,
+        prediction_reference,
+        "prediction",
+        max_categories,
+        psi_contribution_percent,
+        threshold,
+    )
 
-    def test_drift_prediction_psi(
-        self,
-        reference_slice: GiskardDataset,
-        actual_slice: GiskardDataset,
-        model: GiskardModel,
-        max_categories: int = 10,
-        threshold: float = 0.2,
-        psi_contribution_percent: float = 0.2,
-    ):
-        """
-        Test if the PSI score between the reference and actual datasets is below the threshold
-        for the classification labels predictions
-
-        Example : The test is passed when the  PSI score of classification labels prediction
-        for females between reference and actual sets is below 0.2
-
-        Args:
-            actual_slice(GiskardDataset):
-                Slice of the actual dataset
-            reference_slice(GiskardDataset):
-                Slice of the reference dataset
-            model(GiskardModel):
-                Model used to compute the test
-            threshold(float):
-                Threshold value for PSI
-            max_categories:
-                The maximum categories to compute the PSI score
-            psi_contribution_percent:
-                The ratio between the PSI score of a given category over the total PSI score
-                of the categorical variable. If there is a drift, the test provides all the
-                categories that have a PSI contribution over than this ratio.
-
-        Returns:
-            actual_slices_size:
-                Length of actual slice tested
-            reference_slices_size:
-                Length of reference slice tested
-            passed:
-                TRUE if metric <= threshold
-            metric:
-                Total PSI value
-            messages:
-                Psi result message
-        """
-        actual_slice.df.reset_index(drop=True, inplace=True)
-        reference_slice.df.reset_index(drop=True, inplace=True)
-        prediction_reference = pd.Series(model.run_predict(reference_slice).prediction)
-        prediction_actual = pd.Series(model.run_predict(actual_slice).prediction)
-        messages, passed, total_psi = self._test_series_drift_psi(
-            prediction_actual,
-            prediction_reference,
-            "prediction",
-            max_categories,
-            psi_contribution_percent,
-            threshold,
-        )
+    return TestResult(
+        actual_slices_size=[len(actual_dataset)],
+        reference_slices_size=[len(reference_dataset)],
+        passed=passed,
+        metric=total_psi,
+        messages=messages,
+    )
 
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_slice)],
-                reference_slices_size=[len(reference_slice)],
-                passed=passed,
-                metric=total_psi,
-                messages=messages,
-            )
-        )
 
-    def _test_series_drift_psi(
-        self,
+def _test_series_drift_psi(
         actual_series,
         reference_series,
         test_data,
         max_categories,
         psi_contribution_percent,
         threshold,
-    ):
-        total_psi, output_data = self._calculate_drift_psi(
-            actual_series, reference_series, max_categories
-        )
-        passed = True if threshold is None else total_psi <= threshold
-        main_drifting_modalities_bool = output_data["Psi"] > psi_contribution_percent * total_psi
-        messages = self._generate_message_modalities(
-            main_drifting_modalities_bool, output_data, test_data
-        )
-        return messages, passed, total_psi
-
-    @staticmethod
-    def _generate_message_modalities(main_drifting_modalities_bool, output_data, test_data):
-        modalities_list = output_data[main_drifting_modalities_bool]["Modality"].tolist()
-        filtered_modalities = [
-            w for w in modalities_list if not re.match(DriftTests.other_modalities_pattern, w)
+):
+    total_psi, output_data = _calculate_drift_psi(actual_series, reference_series, max_categories)
+    passed = True if threshold is None else bool(total_psi <= threshold)
+    main_drifting_modalities_bool = output_data["Psi"] > psi_contribution_percent * total_psi
+    messages = _generate_message_modalities(main_drifting_modalities_bool, output_data, test_data)
+    return messages, passed, total_psi
+
+
+def _generate_message_modalities(main_drifting_modalities_bool, output_data, test_data):
+    modalities_list = output_data[main_drifting_modalities_bool]["Modality"].tolist()
+    filtered_modalities = [w for w in modalities_list if not re.match(other_modalities_pattern, w)]
+    messages: Optional[List[TestMessage]] = None
+    if filtered_modalities:
+        messages = [
+            TestMessage(
+                type=TestMessageLevel.ERROR,
+                text=f"The {test_data} is drifting for the following modalities: {','.join(filtered_modalities)}",
+            )
         ]
-        messages: Union[typing.List[TestMessage], None] = None
-        if filtered_modalities:
-            messages = [
-                TestMessage(
-                    type=TestMessageType.ERROR,
-                    text=f"The {test_data} is drifting for the following modalities: {','.join(filtered_modalities)}",
-                )
-            ]
-        return messages
-
-    def test_drift_prediction_chi_square(
-        self,
-        reference_slice: GiskardDataset,
-        actual_slice: GiskardDataset,
-        model: GiskardModel,
-        max_categories: int = 10,
-        threshold: float = 0.05,
-        chi_square_contribution_percent: float = 0.2,
-    ):
-        """
-        Test if the Chi Square value between the reference and actual datasets is below the threshold
-        for the classification labels predictions for a given slice
-
-        Example : The test is passed when the  Chi Square value of classification labels prediction
-        for females between reference and actual sets is below 0.05
-
-        Args:
-            actual_slice(GiskardDataset):
-                Slice of the actual dataset
-            reference_slice(GiskardDataset):
-                Slice of the reference dataset
-            model(GiskardModel):
-                Model used to compute the test
-            threshold(float):
-                Threshold value of p-value of Chi-Square
-            max_categories:
-                the maximum categories to compute the PSI score
-            chi_square_contribution_percent:
-                the ratio between the Chi-Square value of a given category over the total Chi-Square
-                value of the categorical variable. If there is a drift, the test provides all the
-                categories that have a PSI contribution over than this ratio.
-
-        Returns:
-            actual_slices_size:
-                Length of actual slice tested
-            reference_slices_size:
-                Length of reference slice tested
-            passed:
-                TRUE if metric > threshold
-            metric:
-                Calculated p-value of Chi_square
-            messages:
-                Message describing if prediction is drifting or not
-        """
-        actual_slice.df.reset_index(drop=True, inplace=True)
-        reference_slice.df.reset_index(drop=True, inplace=True)
-        prediction_reference = pd.Series(model.run_predict(reference_slice).prediction)
-        prediction_actual = pd.Series(model.run_predict(actual_slice).prediction)
-
-        messages, p_value, passed = self._test_series_drift_chi(
-            prediction_actual,
-            prediction_reference,
-            "prediction",
-            chi_square_contribution_percent,
-            max_categories,
-            threshold,
-        )
+    return messages
 
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_slice)],
-                reference_slices_size=[len(reference_slice)],
-                passed=passed,
-                metric=p_value,
-                messages=messages,
-            )
-        )
 
-    def _test_series_drift_chi(
-        self,
+@test(name='Label drift (Chi-squared)')
+def test_drift_prediction_chi_square(model: BaseModel, actual_dataset: Dataset, reference_dataset: Dataset,
+                                     slicing_function: SlicingFunction = None, max_categories: int = 10,
+                                     threshold: float = 0.05, chi_square_contribution_percent: float = 0.2):
+    """
+    Test if the Chi Square value between the reference and actual datasets is below the threshold
+    for the classification labels predictions for a given slice
+
+    Example : The test is passed when the  Chi Square value of classification labels prediction
+    for females between reference and actual sets is below 0.05
+
+    Args:
+        model(BaseModel):
+            Model used to compute the test
+        actual_dataset(Dataset):
+            Actual dataset used to compute the test
+        reference_dataset(Dataset):
+            Reference dataset used to compute the test
+        slicing_function(Optional[SlicingFunction]):
+            Slicing function to be applied on both actual and reference datasets
+        threshold(Optional[float]):
+            Threshold value of p-value of Chi-Square
+        max_categories:
+            the maximum categories to compute the PSI score
+        chi_square_contribution_percent:
+            the ratio between the Chi-Square value of a given category over the total Chi-Square
+            value of the categorical variable. If there is a drift, the test provides all the
+            categories that have a PSI contribution over than this ratio.
+
+    Returns:
+        actual_slices_size:
+            Length of actual slice tested
+        reference_slices_size:
+            Length of reference slice tested
+        passed:
+            TRUE if metric > threshold
+        metric:
+            Calculated p-value of Chi_square
+        messages:
+            Message describing if prediction is drifting or not
+    """
+    if slicing_function:
+        test_name = "test_drift_prediction_chi_square"
+        actual_dataset = actual_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
+        reference_dataset = reference_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
+
+    prediction_reference = pd.Series(model.predict(reference_dataset).prediction)
+    prediction_actual = pd.Series(model.predict(actual_dataset).prediction)
+
+    messages, p_value, passed = _test_series_drift_chi(
+        prediction_actual,
+        prediction_reference,
+        "prediction",
+        chi_square_contribution_percent,
+        max_categories,
+        threshold,
+    )
+
+    return TestResult(
+        actual_slices_size=[len(actual_dataset)],
+        reference_slices_size=[len(reference_dataset)],
+        passed=passed,
+        metric=p_value,
+        messages=messages,
+    )
+
+
+def _test_series_drift_chi(
         actual_series,
         reference_series,
         test_data,
         chi_square_contribution_percent,
         max_categories,
         threshold,
-    ):
-        chi_square, p_value, output_data = self._calculate_chi_square(
-            actual_series, reference_series, max_categories
-        )
-        passed = p_value > threshold
-        main_drifting_modalities_bool = (
-            output_data["Chi_square"] > chi_square_contribution_percent * chi_square
-        )
-        messages = self._generate_message_modalities(
-            main_drifting_modalities_bool, output_data, test_data
-        )
-        return messages, p_value, passed
-
-    def test_drift_prediction_ks(
-        self,
-        reference_slice: GiskardDataset,
-        actual_slice: GiskardDataset,
-        model: GiskardModel,
-        classification_label=None,
-        threshold=None,
-    ) -> SingleTestResult:
-        """
-        Test if the pvalue of the KS test for prediction between the reference and actual datasets for
-         a given subpopulation is above the threshold
-
-        Example : The test is passed when the pvalue of the KS test for the prediction for females
-         between reference and actual dataset is higher than 0.05. It means that the KS test cannot be
-         rejected at 5% level and that we cannot assume drift for this variable.
-
-        Args:
-            actual_slice(GiskardDataset):
-                Slice of the actual dataset
-            reference_slice(GiskardDataset):
-                Slice of the reference dataset
-            model(GiskardModel):
-                Model used to compute the test
-            threshold(float):
-                Threshold for p-value of Kolmogorov-Smirnov test
-            classification_label(str):
-                One specific label value from the target column for classification model
-
-        Returns:
-            actual_slices_size:
-                Length of actual slice tested
-            reference_slices_size:
-                Length of reference slice tested
-            passed:
-                TRUE if metric >= threshold
-            metric:
-                The calculated p-value Kolmogorov-Smirnov test
-            messages:
-                Kolmogorov-Smirnov result message
-        """
-        actual_slice.df.reset_index(drop=True, inplace=True)
-        reference_slice.df.reset_index(drop=True, inplace=True)
-
-        assert (
-            model.model_type != "classification"
-            or classification_label in model.classification_labels
-        ), f'"{classification_label}" is not part of model labels: {",".join(model.classification_labels)}'
-
-        prediction_reference = (
-            pd.Series(
-                model.run_predict(reference_slice).all_predictions[classification_label].values
+):
+    chi_square, p_value, output_data = _calculate_chi_square(actual_series, reference_series, max_categories)
+    passed = bool(p_value > threshold)
+    main_drifting_modalities_bool = output_data["Chi_square"] > chi_square_contribution_percent * chi_square
+    messages = _generate_message_modalities(main_drifting_modalities_bool, output_data, test_data)
+    return messages, p_value, passed
+
+
+@test(name='Classification Probability drift (Kolmogorov-Smirnov)', tags=['classification'])
+@validate_classification_label
+def test_drift_prediction_ks(model: BaseModel, actual_dataset: Dataset, reference_dataset: Dataset,
+                             slicing_function: SlicingFunction = None, classification_label: str = None,
+                             threshold: float = None) -> TestResult:
+    """
+    Test if the pvalue of the KS test for prediction between the reference and actual datasets for
+     a given subpopulation is above the threshold
+
+    Example : The test is passed when the pvalue of the KS test for the prediction for females
+     between reference and actual dataset is higher than 0.05. It means that the KS test cannot be
+     rejected at 5% level and that we cannot assume drift for this variable.
+
+    Args:
+        model(BaseModel):
+            Model used to compute the test
+        actual_dataset(Dataset):
+            Actual dataset used to compute the test
+        reference_dataset(Dataset):
+            Reference dataset used to compute the test
+        slicing_function(Optional[SlicingFunction]):
+            Slicing function to be applied on both actual and reference datasets
+        threshold(Optional[float]):
+            Threshold for p-value of Kolmogorov-Smirnov test
+        classification_label(Optional[str]):
+            One specific label value from the target column for classification model
+
+    Returns:
+        actual_slices_size:
+            Length of actual slice tested
+        reference_slices_size:
+            Length of reference slice tested
+        passed:
+            TRUE if metric >= threshold
+        metric:
+            The calculated p-value Kolmogorov-Smirnov test
+        messages:
+            Kolmogorov-Smirnov result message
+    """
+    if slicing_function:
+        test_name = "test_drift_prediction_ks"
+        actual_dataset = actual_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
+        reference_dataset = reference_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
+
+    prediction_reference = (
+        pd.Series(model.predict(reference_dataset).all_predictions[classification_label].values)
+        if model.is_classification
+        else pd.Series(model.predict(reference_dataset).prediction)
+    )
+    prediction_actual = (
+        pd.Series(model.predict(actual_dataset).all_predictions[classification_label].values)
+        if model.is_classification
+        else pd.Series(model.predict(actual_dataset).prediction)
+    )
+
+    result: Ks_2sampResult = _calculate_ks(prediction_reference, prediction_actual)
+
+    passed = True if threshold is None else bool(result.pvalue >= threshold)
+
+    messages = _generate_message_ks(passed, result, threshold, "prediction")
+
+    return TestResult(
+        actual_slices_size=[len(actual_dataset)],
+        reference_slices_size=[len(reference_dataset)],
+        passed=passed,
+        metric=result.pvalue,
+        messages=messages,
+    )
+
+
+def _generate_message_ks(passed, result, threshold, data_type):
+    messages: Optional[List[TestMessage]] = None
+    if not passed:
+        messages = [
+            TestMessage(
+                type=TestMessageLevel.ERROR,
+                text=f"The {data_type} is drifting (p-value is equal to {np.round(result.pvalue, 9)} "
+                     f"and is below the test risk level {threshold}) ",
             )
-            if model.model_type == "classification"
-            else pd.Series(model.run_predict(reference_slice).prediction)
-        )
-        prediction_actual = (
-            pd.Series(model.run_predict(actual_slice).all_predictions[classification_label].values)
-            if model.model_type == "classification"
-            else pd.Series(model.run_predict(actual_slice).prediction)
-        )
-
-        result: Ks_2sampResult = self._calculate_ks(prediction_reference, prediction_actual)
-
-        passed = True if threshold is None else result.pvalue >= threshold
+        ]
+    return messages
 
-        messages = self._generate_message_ks(passed, result, threshold, "prediction")
 
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_slice)],
-                reference_slices_size=[len(reference_slice)],
-                passed=passed,
-                metric=result.pvalue,
-                messages=messages,
+@test(name='Classification Probability drift (Earth mover\'s distance)', tags=['classification'])
+@validate_classification_label
+def test_drift_prediction_earth_movers_distance(model: BaseModel, actual_dataset: Dataset, reference_dataset: Dataset,
+                                                slicing_function: SlicingFunction = None,
+                                                classification_label: str = None, threshold: float = 0.2) -> TestResult:
+    """
+    Test if the Earth Mover’s Distance value between the reference and actual datasets is
+    below the threshold for the classification labels predictions for classification
+    model and prediction for regression models
+
+    Example :
+    Classification : The test is passed when the  Earth Mover’s Distance value of classification
+    labels probabilities for females between reference and actual sets is below 0.2
+
+    Regression : The test is passed when the  Earth Mover’s Distance value of prediction
+    for females between reference and actual sets is below 0.2
+
+    Args:
+        model(BaseModel):
+            uploaded model
+        actual_dataset(Dataset):
+            Actual dataset used to compute the test
+        reference_dataset(Dataset):
+            Reference dataset used to compute the test
+        slicing_function(Optional[SlicingFunction]):
+            Slicing function to be applied on both actual and reference datasets
+        classification_label(Optional[str]):
+            one specific label value from the target column for classification model
+        threshold(Optional[float]):
+            threshold for earth mover's distance
+
+    Returns:
+        passed:
+            TRUE if metric <= threshold
+        metric:
+            Earth Mover's Distance value
+
+    """
+    if slicing_function:
+        test_name = "test_drift_prediction_earth_movers_distance"
+        actual_dataset = actual_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
+        reference_dataset = reference_dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
+
+    prediction_reference = (
+        model.predict(reference_dataset).all_predictions[classification_label].values
+        if model.is_classification
+        else model.predict(reference_dataset).prediction
+    )
+    prediction_actual = (
+        model.predict(actual_dataset).all_predictions[classification_label].values
+        if model.is_classification
+        else model.predict(actual_dataset).prediction
+    )
+
+    metric = _calculate_earth_movers_distance(prediction_reference, prediction_actual)
+
+    passed = True if threshold is None else bool(metric <= threshold)
+    messages: Optional[typing.List[TestMessage]] = None
+
+    if not passed:
+        messages = [
+            TestMessage(
+                type=TestMessageLevel.ERROR,
+                text=f"The prediction is drifting (metric is equal to {np.round(metric, 9)} "
+                     f"and is above the test risk level {threshold}) ",
             )
-        )
-
-    @staticmethod
-    def _generate_message_ks(passed, result, threshold, data_type):
-        messages: Union[typing.List[TestMessage], None] = None
-        if not passed:
-            messages = [
-                TestMessage(
-                    type=TestMessageType.ERROR,
-                    text=f"The {data_type} is drifting (p-value is equal to {np.round(result.pvalue, 9)} "
-                    f"and is below the test risk level {threshold}) ",
-                )
-            ]
-        return messages
-
-    def test_drift_prediction_earth_movers_distance(
-        self,
-        reference_slice: GiskardDataset,
-        actual_slice: GiskardDataset,
-        model: GiskardModel,
-        classification_label=None,
-        threshold=0.2,
-    ) -> SingleTestResult:
-        """
-        Test if the Earth Mover’s Distance value between the reference and actual datasets is
-        below the threshold for the classification labels predictions for classification
-        model and prediction for regression models
-
-        Example :
-        Classification : The test is passed when the  Earth Mover’s Distance value of classification
-        labels probabilities for females between reference and actual sets is below 0.2
-
-        Regression : The test is passed when the  Earth Mover’s Distance value of prediction
-        for females between reference and actual sets is below 0.2
-
-        Args:
-            reference_slice(GiskardDataset):
-                slice of the reference dataset
-            actual_slice(GiskardDataset):
-                slice of the actual dataset
-            model(GiskardModel):
-                uploaded model
-            classification_label:
-                one specific label value from the target column for classification model
-            threshold:
-                threshold for earth mover's distance
-
-        Returns:
-            passed:
-                TRUE if metric <= threshold
-            metric:
-                Earth Mover's Distance value
-
-        """
-        actual_slice.df.reset_index(drop=True, inplace=True)
-        reference_slice.df.reset_index(drop=True, inplace=True)
-
-        prediction_reference = (
-            model.run_predict(reference_slice).all_predictions[classification_label].values
-            if model.model_type == "classification"
-            else model.run_predict(reference_slice).prediction
-        )
-        prediction_actual = (
-            model.run_predict(actual_slice).all_predictions[classification_label].values
-            if model.model_type == "classification"
-            else model.run_predict(actual_slice).prediction
-        )
-
-        metric = self._calculate_earth_movers_distance(prediction_reference, prediction_actual)
-
-        passed = True if threshold is None else metric <= threshold
-        messages: Union[typing.List[TestMessage], None] = None
+        ]
 
-        if not passed:
-            messages = [
-                TestMessage(
-                    type=TestMessageType.ERROR,
-                    text=f"The prediction is drifting (metric is equal to {np.round(metric, 9)} "
-                    f"and is above the test risk level {threshold}) ",
-                )
-            ]
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_slice)],
-                reference_slices_size=[len(reference_slice)],
-                passed=True if threshold is None else metric <= threshold,
-                metric=metric,
-                messages=messages,
-            )
-        )
+    return TestResult(
+        actual_slices_size=[len(actual_dataset)],
+        reference_slices_size=[len(reference_dataset)],
+        passed=bool(True if threshold is None else metric <= threshold),
+        metric=metric,
+        messages=messages,
+    )
```

### Comparing `giskard-1.9.1/giskard/ml_worker/testing/metamorphic_tests.py` & `giskard-2.0.0b1/giskard/testing/tests/metamorphic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,759 +1,766 @@
 import pandas as pd
 
-from giskard.ml_worker.core.giskard_dataset import GiskardDataset
-from giskard.ml_worker.core.model import GiskardModel
-from giskard.ml_worker.generated.ml_worker_pb2 import SingleTestResult, TestMessage, TestMessageType
-from giskard.ml_worker.testing.abstract_test_collection import AbstractTestCollection
-from giskard.ml_worker.testing.utils import apply_perturbation_inplace
-from giskard.ml_worker.utils.logging import timer
+from giskard import test
+from giskard.core.core import SupportedModelTypes
+from giskard.datasets.base import Dataset
+from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction
+from giskard.ml_worker.testing.registry.transformation_function import TransformationFunction
 from giskard.ml_worker.testing.stat_utils import equivalence_t_test, paired_t_test
 from giskard.ml_worker.testing.stat_utils import equivalence_wilcoxon, paired_wilcoxon
-from giskard.ml_worker.testing.utils import Direction
-
-
-class MetamorphicTests(AbstractTestCollection):
-    @staticmethod
-    def _predict_numeric_result(
-        ds: GiskardDataset, model: GiskardModel, output_proba=True, classification_label=None
-    ):
-        if model.model_type == "regression" or not output_proba:
-            return model.run_predict(ds).raw_prediction
-        elif model.model_type == "classification" and classification_label is not None:
-            return model.run_predict(ds).all_predictions[classification_label].values
-        elif model.model_type == "classification":
-            return model.run_predict(ds).probabilities
-
-    @staticmethod
-    def _prediction_ratio(prediction, perturbed_prediction):
-        return (
-            abs(perturbed_prediction - prediction) / prediction
-            if prediction != 0
-            else abs(perturbed_prediction)
-        )
-
-    @staticmethod
-    def _perturb_and_predict(
-        ds: GiskardDataset,
-        model: GiskardModel,
-        perturbation_dict,
-        output_proba=True,
-        classification_label=None,
-    ):
-        results_df = pd.DataFrame()
-        results_df["prediction"] = MetamorphicTests._predict_numeric_result(
-            ds, model, output_proba, classification_label
-        )
-        modified_rows = apply_perturbation_inplace(ds.df, perturbation_dict)
-        if len(modified_rows):
-            ds.df = ds.df.iloc[modified_rows]
-            results_df = results_df.iloc[modified_rows]
-            results_df["perturbed_prediction"] = MetamorphicTests._predict_numeric_result(
-                ds, model, output_proba, classification_label
-            )
-        else:
-            results_df["perturbed_prediction"] = results_df["prediction"]
-        return results_df, len(modified_rows)
-
-    @timer("Compare and predict the data")
-    def _compare_prediction(self, results_df, prediction_task, direction, output_sensitivity=None):
-        if direction == Direction.Invariant:
-            if prediction_task == "classification":
-                passed_idx = results_df.loc[
-                    results_df["prediction"] == results_df["perturbed_prediction"]
-                ].index.values
-
-            elif prediction_task == "regression":
-                results_df["predict_difference_ratio"] = results_df.apply(
-                    lambda x: self._prediction_ratio(x["prediction"], x["perturbed_prediction"]),
-                    axis=1,
-                )
-                passed_idx = results_df.loc[
-                    results_df["predict_difference_ratio"] < output_sensitivity
-                ].index.values
-
-        elif direction == Direction.Increasing:
-            passed_idx = results_df.loc[
-                results_df["prediction"] < results_df["perturbed_prediction"]
-            ].index.values
-
-        elif direction == Direction.Decreasing:
-            passed_idx = results_df.loc[
-                results_df["prediction"] > results_df["perturbed_prediction"]
-            ].index.values
-
-        failed_idx = results_df.loc[~results_df.index.isin(passed_idx)].index.values
-        return passed_idx, failed_idx
-
-    def _compare_probabilities_t_test(
-        self, result_df, direction, window_size=0.1, critical_quantile=0.05
-    ):
-
-        if direction == Direction.Invariant:
-            p_value = equivalence_t_test(
-                result_df["prediction"],
-                result_df["perturbed_prediction"],
-                window_size=window_size,
-                critical_quantile=critical_quantile,
-            )[1]
-
-        elif direction == Direction.Increasing:
-            p_value = paired_t_test(
-                result_df["prediction"],
-                result_df["perturbed_prediction"],
-                alternative="less",
-                critical_quantile=critical_quantile,
-            )[1]
-
-        elif direction == Direction.Decreasing:
-            p_value = paired_t_test(
-                result_df["prediction"],
-                result_df["perturbed_prediction"],
-                alternative="greater",
-                critical_quantile=critical_quantile,
-            )[1]
-
-        return p_value
-
-    def _compare_probabilities_wilcoxon(
-        self, result_df, direction, window_size=0.2, critical_quantile=0.05
-    ):
-
-        if direction == Direction.Invariant:
-            p_value = equivalence_wilcoxon(
-                result_df["prediction"],
-                result_df["perturbed_prediction"],
-                window_size=window_size,
-                critical_quantile=critical_quantile,
-            )[1]
-
-        elif direction == Direction.Increasing:
-            p_value = paired_wilcoxon(
-                result_df["prediction"],
-                result_df["perturbed_prediction"],
-                alternative="less",
-                critical_quantile=critical_quantile,
-            )[1]
-
-        elif direction == Direction.Decreasing:
-            p_value = paired_wilcoxon(
-                result_df["prediction"],
-                result_df["perturbed_prediction"],
-                alternative="greater",
-                critical_quantile=critical_quantile,
-            )[1]
-
-        return p_value
-
-    def _test_metamorphic(
-        self,
-        direction: Direction,
-        actual_slice: GiskardDataset,
-        model,
-        perturbation_dict,
-        threshold: float,
-        classification_label=None,
-        output_sensitivity=None,
-        output_proba=True,
-    ) -> SingleTestResult:
-        actual_slice.df.reset_index(drop=True, inplace=True)
-
-        results_df, modified_rows_count = self._perturb_and_predict(
-            actual_slice,
-            model,
-            perturbation_dict,
-            classification_label=classification_label,
-            output_proba=output_proba,
-        )
-
-        passed_idx, failed_idx = self._compare_prediction(
-            results_df, model.model_type, direction, output_sensitivity
-        )
-        passed_ratio = len(passed_idx) / modified_rows_count if modified_rows_count != 0 else 1
-
-        messages = [
-            TestMessage(
-                type=TestMessageType.INFO, text=f"{modified_rows_count} rows were perturbed"
-            )
-        ]
-
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_slice)],
-                metric=passed_ratio,
-                passed=passed_ratio > threshold,
-                messages=messages,
-            )
-        )
-
-    def test_metamorphic_invariance(
-        self, df: GiskardDataset, model, perturbation_dict, threshold=0.5, output_sensitivity=None
-    ) -> SingleTestResult:
-        """
-        Summary: Tests if the model prediction is invariant when the feature values are perturbed
-
-        Description: -
-        For classification: Test if the predicted classification label remains the same after
-        feature values perturbation.
-        For regression: Check whether the predicted output remains the same at the output_sensibility
-        level after feature values perturbation.
-
-        The test is passed when the ratio of invariant rows is higher than the threshold
-
-        Example : The test is passed when, after switching gender from male to female,
-        more than 50%(threshold 0.5) of males have unchanged outputs
-
-        Args:
-            df(GiskardDataset):
-              Dataset used to compute the test
-            model(GiskardModel):
-              Model used to compute the test
-            perturbation_dict(dict):
-              Dictionary of the perturbations. It provides the perturbed features as key
-              and a perturbation lambda function as value
-            window_size(float):
-              Threshold of the ratio of invariant rows
-            output_sensitivity(float):
-                Optional. The threshold for ratio between the difference between perturbed prediction and actual prediction over
-                the actual prediction for a regression model. We consider there is a prediction difference for
-                regression if the ratio is above the output_sensitivity of 0.1
-
-        Returns:
-            actual_slices_size:
-              Length of actual_slice tested
-            message:
-              Test result message
-            metric:
-              The ratio of unchanged rows over the perturbed rows
-            passed:
-              TRUE if metric > threshold
-        """
-
-        return self._test_metamorphic(
-            direction=Direction.Invariant,
-            actual_slice=df,
-            model=model,
-            perturbation_dict=perturbation_dict,
-            threshold=threshold,
-            output_sensitivity=output_sensitivity,
-            output_proba=False,
-        )
-
-    def test_metamorphic_increasing(
-        self, df: GiskardDataset, model, perturbation_dict, threshold=0.5, classification_label=None
-    ):
-        """
-        Summary: Tests if the model probability increases when the feature values are perturbed
-
-        Description: -
-        - For classification: Test if the model probability of a given classification_label is
-        increasing after feature values perturbation.
-
-        - For regression: Test if the model prediction is increasing after feature values perturbation.
-
-        The test is passed when the percentage of rows that are increasing is higher than the threshold
-
-        Example : For a credit scoring model, the test is passed when a decrease of wage by 10%,
-         default probability is increasing for more than 50% of people in the dataset
-
-        Args:
-            df(GiskardDataset):
-              Dataset used to compute the test
-            model(GiskardModel):
-              Model used to compute the test
-            perturbation_dict(dict):
-              Dictionary of the perturbations. It provides the perturbed features as key
-              and a perturbation lambda function as value
-            window_size(float):
-              Threshold of the ratio of increasing rows
-            classification_label(str):
-              Optional.One specific label value from the target column
-
-        Returns:
-            actual_slices_size:
-              Length of actual_slice tested
-            message:
-              Test result message
-            metric:
-              The ratio of increasing rows over the perturbed rows
-            passed:
-              TRUE if metric > threshold
-        """
-        assert (
-            model.model_type != "classification"
-            or str(classification_label) in model.classification_labels
-        ), f'"{classification_label}" is not part of model labels: {",".join(model.classification_labels)}'
-
-        return self._test_metamorphic(
-            direction=Direction.Increasing,
-            actual_slice=df,
-            model=model,
-            perturbation_dict=perturbation_dict,
-            classification_label=classification_label,
-            threshold=threshold,
-        )
+from giskard.ml_worker.testing.test_result import TestResult, TestMessage, TestMessageLevel
+from giskard.ml_worker.testing.utils import Direction, validate_classification_label
+from giskard.ml_worker.testing.utils import check_slice_not_empty
+from giskard.ml_worker.utils.logging import timer
+from giskard.models.base import BaseModel
+from giskard.models.utils import fix_seed
 
-    def test_metamorphic_decreasing(
-        self, df: GiskardDataset, model, perturbation_dict, threshold=0.5, classification_label=None
-    ):
-        """
-        Summary: Tests if the model probability decreases when the feature values are perturbed
 
-        Description: -
-        - For classification: Test if the model probability of a given classification_label is
-        decreasing after feature values perturbation.
+def _predict_numeric_result(model: BaseModel, ds: Dataset, output_proba=True, classification_label=None):
+    if model.is_regression or not output_proba:
+        return model.predict(ds).raw_prediction
+    elif model.is_classification and classification_label is not None:
+        return model.predict(ds).all_predictions[classification_label].values
+    elif model.is_classification:
+        return model.predict(ds).probabilities
 
-        - For regression: Test if the model prediction is decreasing after feature values perturbation.
 
-        The test is passed when the percentage of rows that are decreasing is higher than the threshold
+def _prediction_ratio(prediction, perturbed_prediction):
+    return abs(perturbed_prediction - prediction) / prediction if prediction != 0 else abs(perturbed_prediction)
 
-        Example : For a credit scoring model, the test is passed when an increase of wage by 10%,
-         default probability is decreasing for more than 50% of people in the dataset
 
-        Args:
-            df(GiskardDataset):
-              Dataset used to compute the test
-            model(GiskardModel):
-              Model used to compute the test
-            perturbation_dict(dict):
-              Dictionary of the perturbations. It provides the perturbed features as key
-              and a perturbation lambda function as value
-            threshold(float):
-              Threshold of the ratio of decreasing rows
-            classification_label(str):
-              Optional. One specific label value from the target column
-
-        Returns:
-            actual_slices_size:
-              Length of actual_slice tested
-            message:
-              Test result message
-            metric:
-              The ratio of decreasing rows over the perturbed rows
-            passed:
-              TRUE if metric > threshold
-        """
-
-        assert (
-            model.model_type != "classification"
-            or classification_label in model.classification_labels
-        ), f'"{classification_label}" is not part of model labels: {",".join(model.classification_labels)}'
-
-        return self._test_metamorphic(
-            direction=Direction.Decreasing,
-            actual_slice=df,
-            model=model,
-            perturbation_dict=perturbation_dict,
-            classification_label=classification_label,
-            threshold=threshold,
-        )
-
-    def _test_metamorphic_t_test(
-        self,
-        direction: Direction,
-        actual_slice: GiskardDataset,
-        model,
-        perturbation_dict,
-        window_size: float,
-        critical_quantile: float,
-        classification_label=None,
+@timer("Perturb and predict data")
+def _perturb_and_predict(
+        model: BaseModel,
+        ds: Dataset,
+        transformation_function: TransformationFunction,
         output_proba=True,
-    ) -> SingleTestResult:
+        classification_label=None,
+):
+    fix_seed()
 
-        actual_slice.df.reset_index(drop=True, inplace=True)
+    results_df = pd.DataFrame(
+        {
+            "prediction": _predict_numeric_result(model, ds, output_proba, classification_label),
+        },
+        index=ds.df.index,
+    )
+
+    perturbed_ds = ds.transform(transformation_function)
+    results_df["perturbed_prediction"] = _predict_numeric_result(
+        model, perturbed_ds, output_proba, classification_label
+    )
+    modified_idx = ds.df.compare(perturbed_ds.df).index
+
+    return results_df.loc[modified_idx], len(modified_idx)
+
+
+@timer("Compare and predict the data")
+def _compare_prediction(results_df, prediction_task, direction, output_sensitivity=None):
+    if direction == Direction.Invariant:
+        if prediction_task == SupportedModelTypes.CLASSIFICATION:
+            passed_idx = results_df.loc[results_df["prediction"] == results_df["perturbed_prediction"]].index.values
+
+        elif prediction_task == SupportedModelTypes.REGRESSION:
+            results_df["predict_difference_ratio"] = results_df.apply(
+                lambda x: _prediction_ratio(x["prediction"], x["perturbed_prediction"]),
+                axis=1,
+            )
+            passed_idx = results_df.loc[results_df["predict_difference_ratio"] < output_sensitivity].index.values
+        else:
+            raise ValueError(f"Invalid prediction task: {prediction_task}")
 
-        result_df, modified_rows_count = self._perturb_and_predict(
-            actual_slice,
-            model,
-            perturbation_dict,
-            output_proba=output_proba,
-            classification_label=classification_label,
-        )
+    elif direction == Direction.Increasing:
+        passed_idx = results_df.loc[results_df["prediction"] < results_df["perturbed_prediction"]].index.values
 
-        p_value = self._compare_probabilities_t_test(
-            result_df, direction, window_size, critical_quantile
-        )
+    elif direction == Direction.Decreasing:
+        passed_idx = results_df.loc[results_df["prediction"] > results_df["perturbed_prediction"]].index.values
+    else:
+        raise ValueError(f"Invalid direction: {direction}")
 
-        messages = [
-            TestMessage(
-                type=TestMessageType.INFO, text=f"{modified_rows_count} rows were perturbed"
-            )
-        ]
+    failed_idx = results_df.loc[~results_df.index.isin(passed_idx)].index.values
+    return passed_idx, failed_idx
 
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_slice)],
-                metric=p_value,
-                passed=p_value < critical_quantile,
-                messages=messages,
-            )
-        )
 
-    def test_metamorphic_decreasing_t_test(
-        self,
-        df: GiskardDataset,
-        model,
-        perturbation_dict,
-        critical_quantile=0.05,
-        classification_label=None,
-    ):
-        """
-        Summary: Tests if the model probability decreases when the feature values are perturbed
-
-        Description: Calculate the t-test on TWO RELATED samples. Sample (A) is the original probability predictions
-        while sample (B) is the probabilities after perturbation of one or more of the features.
-        This test computes the decreasing test to study if mean(B) < mean(A)
-        The test is passed when the p-value of the t-test between (A) and (B) is below the critical quantile
-
-        Example: For a credit scoring model, the test is passed when a decrease of wage by 10%,
-                 causes a statistically significant probability decrease.
-
-        Args:
-            df(GiskardDataset):
-                Dataset used to compute the test
-            model(GiskardModel):
-                Model used to compute the test
-            perturbation_dict(dict):
-                Dictionary of the perturbations. It provides the perturbed features as key
-                and a perturbation lambda function as value
-            critical_quantile(float):
-                Critical quantile above which the null hypothesis cannot be rejected
-
-        Returns:
-            actual_slices_size:
-                Length of actual_slice tested
-            message:
-                Test result message
-            metric:
-                The t-test in terms of p-value between unchanged rows over the perturbed rows
-            passed:
-                TRUE if the p-value of the t-test between (A) and (B) is below the critical value
-        """
-
-        assert (
-            model.model_type != "classification"
-            or str(classification_label) in model.classification_labels
-        ), f'"{classification_label}" is not part of model labels: {",".join(model.classification_labels)}'
-
-        return self._test_metamorphic_t_test(
-            direction=Direction.Decreasing,
-            actual_slice=df,
-            model=model,
-            perturbation_dict=perturbation_dict,
-            classification_label=classification_label,
-            window_size=float("nan"),
+def _compare_probabilities_t_test(result_df, direction, window_size=0.1, critical_quantile=0.05):
+    if direction == Direction.Invariant:
+        p_value = equivalence_t_test(
+            result_df["prediction"],
+            result_df["perturbed_prediction"],
+            window_size=window_size,
             critical_quantile=critical_quantile,
-        )
+        )[1]
 
-    def test_metamorphic_increasing_t_test(
-        self,
-        df: GiskardDataset,
-        model,
-        perturbation_dict,
-        critical_quantile=0.05,
-        classification_label=None,
-    ):
-        """
-        Summary: Tests if the model probability increases when the feature values are perturbed
-
-        Description: Calculate the t-test on TWO RELATED samples. Sample (A) is the original probability predictions
-        while sample (B) is the probabilities after perturbation of one or more of the features.
-        This test computes the increasing test to study if mean(A) < mean(B)
-        The test is passed when the p-value of the t-test between (A) and (B) is below the critical quantile
-
-        Example: For a credit scoring model, the test is passed when a decrease of wage by 10%,
-                 causes a statistically significant probability increase.
-
-        Args:
-            df(GiskardDataset):
-                Dataset used to compute the test
-            model(GiskardModel):
-                Model used to compute the test
-            perturbation_dict(dict):
-                Dictionary of the perturbations. It provides the perturbed features as key
-                and a perturbation lambda function as value
-            critical_quantile(float):
-                Critical quantile above which the null hypothesis cannot be rejected
-
-        Returns:
-            actual_slices_size:
-                Length of actual_slice tested
-            message:
-                Test result message
-            metric:
-                The t-test in terms of p-value between unchanged rows over the perturbed rows
-            passed:
-                TRUE if the p-value of the t-test between (A) and (B) is below the critical value
-        """
-
-        assert (
-            model.model_type != "classification"
-            or str(classification_label) in model.classification_labels
-        ), f'"{classification_label}" is not part of model labels: {",".join(model.classification_labels)}'
-
-        return self._test_metamorphic_t_test(
-            direction=Direction.Increasing,
-            actual_slice=df,
-            model=model,
-            perturbation_dict=perturbation_dict,
-            classification_label=classification_label,
-            window_size=float("nan"),
+    elif direction == Direction.Increasing:
+        p_value = paired_t_test(
+            result_df["prediction"],
+            result_df["perturbed_prediction"],
+            alternative="less",
             critical_quantile=critical_quantile,
-        )
+        )[1]
 
-    def test_metamorphic_invariance_t_test(
-        self,
-        df: GiskardDataset,
-        model,
-        perturbation_dict,
-        window_size: float,
-        critical_quantile: float,
-    ) -> SingleTestResult:
-        """
-        Summary: Tests if the model predictions are statistically invariant when the feature values are perturbed.
-
-        Description: Calculate the t-test on TWO RELATED samples. Sample (A) is the original probability predictions
-        while sample (B) is the probabilities after perturbation of one or more of the features.
-        This test computes the equivalence test to show that mean(B) - window_size/2 < mean(A) < mean(B) + window_size/2
-        The test is passed when the following tests pass:
-          - the p-value of the t-test between (A) and (B)+window_size/2 is below the critical quantile
-          - the p-value of the t-test between (B)-window_size/2 and (A) is below the critical quantile
-
-        Example: The test is passed when, after switching gender from male to female,
-        the probability distributions remains statistically invariant. In other words, the test is passed if the mean of the
-        perturbed sample is statistically within a window determined by the user.
-
-        Args:
-              df(GiskardDataset):
-                  Dataset used to compute the test
-              model(GiskardModel):
-                  Model used to compute the test
-              perturbation_dict(dict):
-                  Dictionary of the perturbations. It provides the perturbed features as key
-                  and a perturbation lambda function as value
-              window_size(float):
-                  Probability window in which the mean of the perturbed sample can be in
-              critical_quantile(float):
-                  Critical quantile above which the null hypothesis cannot be rejected
-
-        Returns:
-              actual_slices_size:
-                  Length of actual_slice tested
-              message:
-                  Test result message
-              metric:
-                  The t-test in terms of p-value between unchanged rows over the perturbed rows
-              passed:
-                  TRUE if the p-value of the t-test between (A) and (B)+window_size/2 < critical_quantile && the p-value of the t-test between (B)-window_size/2 and (A) < critical_quantile
-        """
-
-        return self._test_metamorphic_t_test(
-            direction=Direction.Invariant,
-            actual_slice=df,
-            model=model,
-            perturbation_dict=perturbation_dict,
-            window_size=window_size,
+    elif direction == Direction.Decreasing:
+        p_value = paired_t_test(
+            result_df["prediction"],
+            result_df["perturbed_prediction"],
+            alternative="greater",
             critical_quantile=critical_quantile,
-        )
+        )[1]
 
-    def _test_metamorphic_wilcoxon(
-        self,
-        direction: Direction,
-        actual_slice: GiskardDataset,
-        model,
-        perturbation_dict,
-        window_size: float,
-        critical_quantile: float,
-        classification_label=None,
-        output_proba=True,
-    ) -> SingleTestResult:
+    return p_value
 
-        actual_slice.df.reset_index(drop=True, inplace=True)
 
-        result_df, modified_rows_count = self._perturb_and_predict(
-            actual_slice,
-            model,
-            perturbation_dict,
-            output_proba=output_proba,
-            classification_label=classification_label,
-        )
+def _compare_probabilities_wilcoxon(result_df, direction, window_size=0.2, critical_quantile=0.05):
+    if direction == Direction.Invariant:
+        p_value = equivalence_wilcoxon(
+            result_df["prediction"],
+            result_df["perturbed_prediction"],
+            window_size=window_size,
+            critical_quantile=critical_quantile,
+        )[1]
 
-        p_value = self._compare_probabilities_wilcoxon(
-            result_df, direction, window_size, critical_quantile
-        )
+    elif direction == Direction.Increasing:
+        p_value = paired_wilcoxon(
+            result_df["prediction"],
+            result_df["perturbed_prediction"],
+            alternative="less",
+            critical_quantile=critical_quantile,
+        )[1]
 
-        messages = [
-            TestMessage(
-                type=TestMessageType.INFO, text=f"{modified_rows_count} rows were perturbed"
-            )
-        ]
+    elif direction == Direction.Decreasing:
+        p_value = paired_wilcoxon(
+            result_df["prediction"],
+            result_df["perturbed_prediction"],
+            alternative="greater",
+            critical_quantile=critical_quantile,
+        )[1]
 
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_slice)],
-                metric=p_value,
-                passed=p_value < critical_quantile,
-                messages=messages,
-            )
-        )
+    return p_value
 
-    def test_metamorphic_decreasing_wilcoxon(
-        self,
-        df: GiskardDataset,
-        model,
-        perturbation_dict,
-        critical_quantile=0.05,
-        classification_label=None,
-    ):
-        """
-        Summary: Tests if the model probability decreases when the feature values are perturbed
-
-        Description: Calculate the Wilcoxon signed-rank test on TWO RELATED samples. Sample (A) is the original probability predictions
-        while sample (B) is the probabilities after perturbation of one or more of the features.
-        This test computes the decreasing test to study if mean(B) < mean(A)
-        The test is passed when the p-value of the Wilcoxon signed-rank test between (A) and (B) is below the critical quantile
-
-        Example: For a credit scoring model, the test is passed when a decrease of wage by 10%,
-                 causes a statistically significant probability decrease.
-
-        Args:
-            df(GiskardDataset):
-                Dataset used to compute the test
-            model(GiskardModel):
-                Model used to compute the test
-            perturbation_dict(dict):
-                Dictionary of the perturbations. It provides the perturbed features as key
-                and a perturbation lambda function as value
-            critical_quantile(float):
-                Critical quantile above which the null hypothesis cannot be rejected
-
-        Returns:
-            actual_slices_size:
-                Length of actual_slice tested
-            message:
-                Test result message
-            metric:
-                The Wilcoxon signed-rank test in terms of p-value between unchanged rows over the perturbed rows
-            passed:
-                TRUE if the p-value of the Wilcoxon signed-rank test between (A) and (B) is below the critical value
-        """
-
-        assert (
-            model.model_type != "classification"
-            or str(classification_label) in model.classification_labels
-        ), f'"{classification_label}" is not part of model labels: {",".join(model.classification_labels)}'
-
-        return self._test_metamorphic_wilcoxon(
-            direction=Direction.Decreasing,
-            actual_slice=df,
-            model=model,
-            perturbation_dict=perturbation_dict,
-            classification_label=classification_label,
-            window_size=float("nan"),
-            critical_quantile=critical_quantile,
-        )
 
-    def test_metamorphic_increasing_wilcoxon(
-        self,
-        df: GiskardDataset,
-        model,
-        perturbation_dict,
-        critical_quantile=0.05,
-        classification_label=None,
-    ):
-        """
-        Summary: Tests if the model probability increases when the feature values are perturbed
-
-        Description: Calculate the Wilcoxon signed-rank test on TWO RELATED samples. Sample (A) is the original probability predictions
-        while sample (B) is the probabilities after perturbation of one or more of the features.
-        This test computes the increasing test to study if mean(A) < mean(B)
-        The test is passed when the p-value of the Wilcoxon signed-rank test between (A) and (B) is below the critical quantile
-
-        Example: For a credit scoring model, the test is passed when a decrease of wage by 10%,
-                 causes a statistically significant probability increase.
-
-        Args:
-            df(GiskardDataset):
-                Dataset used to compute the test
-            model(GiskardModel):
-                Model used to compute the test
-            perturbation_dict(dict):
-                Dictionary of the perturbations. It provides the perturbed features as key
-                and a perturbation lambda function as value
-            critical_quantile(float):
-                Critical quantile above which the null hypothesis cannot be rejected
-
-        Returns:
-            actual_slices_size:
-                Length of actual_slice tested
-            message:
-                Test result message
-            metric:
-                The Wilcoxon signed-rank test in terms of p-value between unchanged rows over the perturbed rows
-            passed:
-                TRUE if the p-value of the Wilcoxon signed-rank test between (A) and (B) is below the critical value
-        """
-
-        assert (
-            model.model_type != "classification"
-            or str(classification_label) in model.classification_labels
-        ), f'"{classification_label}" is not part of model labels: {",".join(model.classification_labels)}'
-
-        return self._test_metamorphic_wilcoxon(
-            direction=Direction.Increasing,
-            actual_slice=df,
-            model=model,
-            perturbation_dict=perturbation_dict,
-            classification_label=classification_label,
-            window_size=float("nan"),
-            critical_quantile=critical_quantile,
-        )
+def _test_metamorphic(
+    model,
+    direction: Direction,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    threshold: float,
+    classification_label=None,
+    output_sensitivity=None,
+    output_proba=True,
+) -> TestResult:
+    results_df, modified_rows_count = _perturb_and_predict(
+        model, dataset, transformation_function, output_proba=output_proba, classification_label=classification_label
+    )
+
+    passed_idx, _ = _compare_prediction(results_df, model.meta.model_type, direction, output_sensitivity)
+    passed_ratio = len(passed_idx) / modified_rows_count if modified_rows_count != 0 else 1
+
+    messages = [TestMessage(type=TestMessageLevel.INFO, text=f"{modified_rows_count} rows were perturbed")]
+
+    return TestResult(
+        actual_slices_size=[len(dataset)],
+        metric=passed_ratio,
+        passed=bool(passed_ratio > threshold),
+        messages=messages,
+    )
+
+
+@test(name="Invariance (proportion)")
+def test_metamorphic_invariance(
+    model: BaseModel,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    slicing_function: SlicingFunction = None,
+    threshold: float = 0.5,
+    output_sensitivity: float = None,
+):
+    """
+    Summary: Tests if the model prediction is invariant when the feature values are perturbed
+
+    Description: -
+    For classification: Test if the predicted classification label remains the same after
+    feature values perturbation.
+    For regression: Check whether the predicted output remains the same at the output_sensibility
+    level after feature values perturbation.
+
+    The test is passed when the ratio of invariant rows is higher than the threshold
+
+    Example : The test is passed when, after switching gender from male to female,
+    more than 50%(threshold 0.5) of males have unchanged outputs
+
+    Args:
+        model(BaseModel):
+          Model used to compute the test
+        dataset(Dataset):
+          Dataset used to compute the test
+        transformation_function(TransformationFunction):
+          Function performing the perturbations to be applied on dataset.
+        slicing_function(Optional[SlicingFunction]):
+          Slicing function to be applied on dataset
+        output_sensitivity(Optional[float]):
+            Optional. The threshold for ratio between the difference between perturbed prediction and actual prediction over
+            the actual prediction for a regression model. We consider there is a prediction difference for
+            regression if the ratio is above the output_sensitivity of 0.1
+
+    Returns:
+        actual_slices_size:
+          Length of dataset tested
+        message:
+          Test result message
+        metric:
+          The ratio of unchanged rows over the perturbed rows
+        passed:
+          TRUE if metric > threshold
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_metamorphic_invariance")
+
+    return _test_metamorphic(
+        direction=Direction.Invariant,
+        dataset=dataset,
+        model=model,
+        transformation_function=transformation_function,
+        threshold=threshold,
+        output_sensitivity=output_sensitivity,
+        output_proba=False,
+    )
+
+
+@test(name="Increasing (proportion)")
+@validate_classification_label
+def test_metamorphic_increasing(
+    model: BaseModel,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    slicing_function: SlicingFunction = None,
+    threshold: float = 0.5,
+    classification_label: str = None,
+):
+    """
+    Summary: Tests if the model probability increases when the feature values are perturbed
+
+    Description: -
+    - For classification: Test if the model probability of a given classification_label is
+    increasing after feature values perturbation.
+
+    - For regression: Test if the model prediction is increasing after feature values perturbation.
+
+    The test is passed when the percentage of rows that are increasing is higher than the threshold
+
+    Example : For a credit scoring model, the test is passed when a decrease of wage by 10%,
+     default probability is increasing for more than 50% of people in the dataset
+
+    Args:
+        model(BaseModel):
+          Model used to compute the test
+        dataset(Dataset):
+          Dataset used to compute the test
+        transformation_function(TransformationFunction):
+          Function performing the perturbations to be applied on dataset.
+        slicing_function(Optional[SlicingFunction]):
+          Slicing function to be applied on dataset
+        classification_label(str):
+          Optional.One specific label value from the target column
+
+    Returns:
+        actual_slices_size:
+          Length of dataset tested
+        message:
+          Test result message
+        metric:
+          The ratio of increasing rows over the perturbed rows
+        passed:
+          TRUE if metric > threshold
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_metamorphic_increasing")
+
+    return _test_metamorphic(
+        direction=Direction.Increasing,
+        dataset=dataset,
+        model=model,
+        transformation_function=transformation_function,
+        classification_label=classification_label,
+        threshold=threshold,
+    )
+
+
+@test(name="Decreasing (proportion)")
+@validate_classification_label
+def test_metamorphic_decreasing(
+    model: BaseModel,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    slicing_function: SlicingFunction = None,
+    threshold: float = 0.5,
+    classification_label: str = None,
+):
+    """
+    Summary: Tests if the model probability decreases when the feature values are perturbed
+
+    Description: -
+    - For classification: Test if the model probability of a given classification_label is
+    decreasing after feature values perturbation.
+
+    - For regression: Test if the model prediction is decreasing after feature values perturbation.
+
+    The test is passed when the percentage of rows that are decreasing is higher than the threshold
+
+    Example : For a credit scoring model, the test is passed when an increase of wage by 10%,
+     default probability is decreasing for more than 50% of people in the dataset
+
+    Args:
+        model(BaseModel):
+          Model used to compute the test
+        dataset(Dataset):
+          Dataset used to compute the test
+        transformation_function(TransformationFunction):
+          Function performing the perturbations to be applied on dataset.
+        slicing_function(Optional[SlicingFunction]):
+          Slicing function to be applied on dataset
+        threshold(float):
+          Threshold of the ratio of decreasing rows
+        classification_label(str):
+          Optional. One specific label value from the target column
+
+    Returns:
+        actual_slices_size:
+          Length of dataset tested
+        message:
+          Test result message
+        metric:
+          The ratio of decreasing rows over the perturbed rows
+        passed:
+          TRUE if metric > threshold
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_metamorphic_decreasing")
+
+    return _test_metamorphic(
+        direction=Direction.Decreasing,
+        dataset=dataset,
+        model=model,
+        transformation_function=transformation_function,
+        classification_label=classification_label,
+        threshold=threshold,
+    )
+
+
+def _test_metamorphic_t_test(
+    direction: Direction,
+    model,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    window_size: float,
+    critical_quantile: float,
+    classification_label=None,
+    output_proba=True,
+) -> TestResult:
+    result_df, modified_rows_count = _perturb_and_predict(
+        model, dataset, transformation_function, output_proba=output_proba, classification_label=classification_label
+    )
+
+    p_value = _compare_probabilities_t_test(result_df, direction, window_size, critical_quantile)
+
+    messages = [TestMessage(type=TestMessageLevel.INFO, text=f"{modified_rows_count} rows were perturbed")]
+
+    return TestResult(
+        actual_slices_size=[len(dataset)],
+        metric=p_value,
+        passed=bool(p_value < critical_quantile),
+        messages=messages,
+    )
+
+
+@test(name="Decreasing (t-test)")
+@validate_classification_label
+def test_metamorphic_decreasing_t_test(
+    model: BaseModel,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    slicing_function: SlicingFunction = None,
+    critical_quantile: float = 0.05,
+    classification_label: str = None,
+):
+    """
+    Summary: Tests if the model probability decreases when the feature values are perturbed
+
+    Description: Calculate the t-test on TWO RELATED samples. Sample (A) is the original probability predictions
+    while sample (B) is the probabilities after perturbation of one or more of the features.
+    This test computes the decreasing test to study if mean(B) < mean(A)
+    The test is passed when the p-value of the t-test between (A) and (B) is below the critical quantile
+
+    Example: For a credit scoring model, the test is passed when a decrease of wage by 10%,
+             causes a statistically significant probability decrease.
+
+    Args:
+        model(BaseModel):
+            Model used to compute the test
+        dataset(Dataset):
+            Dataset used to compute the test
+        transformation_function(TransformationFunction):
+            Function performing the perturbations to be applied on dataset.
+        slicing_function(Optional[SlicingFunction]):
+          Slicing function to be applied on dataset
+        critical_quantile(Optional[float]):
+            Critical quantile above which the null hypothesis cannot be rejected
+
+    Returns:
+        actual_slices_size:
+            Length of dataset tested
+        message:
+            Test result message
+        metric:
+            The t-test in terms of p-value between unchanged rows over the perturbed rows
+        passed:
+            TRUE if the p-value of the t-test between (A) and (B) is below the critical value
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(
+            sliced_dataset=dataset, dataset_name="dataset", test_name="test_metamorphic_decreasing_t_test"
+        )
+
+    return _test_metamorphic_t_test(
+        direction=Direction.Decreasing,
+        dataset=dataset,
+        model=model,
+        transformation_function=transformation_function,
+        window_size=float("nan"),
+        critical_quantile=critical_quantile,
+        classification_label=classification_label,
+    )
+
+
+@test(name="Increasing (t-test)")
+@validate_classification_label
+def test_metamorphic_increasing_t_test(
+    model: BaseModel,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    slicing_function: SlicingFunction = None,
+    critical_quantile: float = 0.05,
+    classification_label: str = None,
+):
+    """
+    Summary: Tests if the model probability increases when the feature values are perturbed
+
+    Description: Calculate the t-test on TWO RELATED samples. Sample (A) is the original probability predictions
+    while sample (B) is the probabilities after perturbation of one or more of the features.
+    This test computes the increasing test to study if mean(A) < mean(B)
+    The test is passed when the p-value of the t-test between (A) and (B) is below the critical quantile
+
+    Example: For a credit scoring model, the test is passed when a decrease of wage by 10%,
+             causes a statistically significant probability increase.
+
+    Args:
+        model(BaseModel):
+            Model used to compute the test
+        dataset(Dataset):
+            Dataset used to compute the test
+        transformation_function(TransformationFunction):
+            Function performing the perturbations to be applied on dataset.
+        slicing_function(Optional[SlicingFunction]):
+          Slicing function to be applied on dataset
+        critical_quantile(Optional[float]):
+            Critical quantile above which the null hypothesis cannot be rejected
+
+    Returns:
+        actual_slices_size:
+            Length of dataset tested
+        message:
+            Test result message
+        metric:
+            The t-test in terms of p-value between unchanged rows over the perturbed rows
+        passed:
+            TRUE if the p-value of the t-test between (A) and (B) is below the critical value
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(
+            sliced_dataset=dataset, dataset_name="dataset", test_name="test_metamorphic_increasing_t_test"
+        )
+
+    return _test_metamorphic_t_test(
+        direction=Direction.Increasing,
+        dataset=dataset,
+        model=model,
+        transformation_function=transformation_function,
+        window_size=float("nan"),
+        critical_quantile=critical_quantile,
+        classification_label=classification_label,
+    )
+
+
+@test(name="Invariance (t-test)")
+def test_metamorphic_invariance_t_test(
+    model: BaseModel,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    slicing_function: SlicingFunction = None,
+    window_size: float = 0.2,
+    critical_quantile: float = 0.05,
+) -> TestResult:
+    """
+    Summary: Tests if the model predictions are statistically invariant when the feature values are perturbed.
+
+    Description: Calculate the t-test on TWO RELATED samples. Sample (A) is the original probability predictions
+    while sample (B) is the probabilities after perturbation of one or more of the features.
+    This test computes the equivalence test to show that mean(B) - window_size/2 < mean(A) < mean(B) + window_size/2
+    The test is passed when the following tests pass:
+      - the p-value of the t-test between (A) and (B)+window_size/2 is below the critical quantile
+      - the p-value of the t-test between (B)-window_size/2 and (A) is below the critical quantile
+
+    Example: The test is passed when, after switching gender from male to female,
+    the probability distributions remains statistically invariant. In other words, the test is passed if the mean of the
+    perturbed sample is statistically within a window determined by the user.
 
-    def test_metamorphic_invariance_wilcoxon(
-        self, df: GiskardDataset, model, perturbation_dict, window_size=0.2, critical_quantile=0.05
-    ) -> SingleTestResult:
-        """
-        Summary: Tests if the model predictions are statistically invariant when the feature values are perturbed.
-
-        Description: Calculate the Wilcoxon signed-rank test on TWO RELATED samples. Sample (A) is the original probability predictions
-        while sample (B) is the probabilities after perturbation of one or more of the features.
-        This test computes the equivalence test to show that mean(B) - window_size/2 < mean(A) < mean(B) + window_size/2
-        The test is passed when the following tests pass:
-        - the p-value of the t-test between (A) and (B)+window_size/2 is below the critical quantile
-        - the p-value of the t-test between (B)-window_size/2 and (A) is below the critical quantile
-
-        Example: The test is passed when, after switching gender from male to female,
-        the probability distributions remains statistically invariant. In other words, the test is passed if the mean of the
-        perturbed sample is statistically within a window determined by the user.
-
-        Args:
-            df(GiskardDataset):
-                Dataset used to compute the test
-            model(GiskardModel):
-                Model used to compute the test
-            perturbation_dict(dict):
-                Dictionary of the perturbations. It provides the perturbed features as key
-                and a perturbation lambda function as value
-            window_size(float):
-                Probability window in which the mean of the perturbed sample can be in
-            critical_quantile(float):
-                Critical quantile above which the null hypothesis cannot be rejected
-
-        Returns:
-            actual_slices_size:
-                Length of actual_slice tested
-            message:
-                Test result message
-            metric:
-                The t-test in terms of p-value between unchanged rows over the perturbed rows
-            passed:
-                TRUE if the p-value of the Wilcoxon signed-rank test between (A) and (B)+window_size/2 < critical_quantile && the p-value of the t-test between (B)-window_size/2 and (A) < critical_quantile
-        """
-
-        return self._test_metamorphic_wilcoxon(
-            direction=Direction.Invariant,
-            actual_slice=df,
-            model=model,
-            perturbation_dict=perturbation_dict,
-            window_size=window_size,
-            critical_quantile=critical_quantile,
-        )
+    Args:
+          model(BaseModel):
+              Model used to compute the test
+          dataset(Dataset):
+              Dataset used to compute the test
+          transformation_function(TransformationFunction):
+              Function performing the perturbations to be applied on dataset.
+          slicing_function(Optional[SlicingFunction]):
+              Slicing function to be applied on dataset
+          window_size(Optional[float]):
+              Probability window in which the mean of the perturbed sample can be in
+          critical_quantile(Optional[float]):
+              Critical quantile above which the null hypothesis cannot be rejected
+
+    Returns:
+          actual_slices_size:
+              Length of dataset tested
+          message:
+              Test result message
+          metric:
+              The t-test in terms of p-value between unchanged rows over the perturbed rows
+          passed:
+              TRUE if the p-value of the t-test between (A) and (B)+window_size/2 < critical_quantile && the p-value of the t-test between (B)-window_size/2 and (A) < critical_quantile
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(
+            sliced_dataset=dataset, dataset_name="dataset", test_name="test_metamorphic_invariance_t_test"
+        )
+
+    return _test_metamorphic_t_test(
+        direction=Direction.Invariant,
+        dataset=dataset,
+        model=model,
+        transformation_function=transformation_function,
+        window_size=window_size,
+        critical_quantile=critical_quantile,
+    )
+
+
+def _test_metamorphic_wilcoxon(
+    direction: Direction,
+    model,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    window_size: float,
+    critical_quantile: float,
+    classification_label=None,
+    output_proba=True,
+) -> TestResult:
+    result_df, modified_rows_count = _perturb_and_predict(
+        model, dataset, transformation_function, output_proba=output_proba, classification_label=classification_label
+    )
+
+    p_value = _compare_probabilities_wilcoxon(result_df, direction, window_size, critical_quantile)
+
+    messages = [TestMessage(type=TestMessageLevel.INFO, text=f"{modified_rows_count} rows were perturbed")]
+
+    return TestResult(
+        actual_slices_size=[len(dataset)],
+        metric=p_value,
+        passed=bool(p_value < critical_quantile),
+        messages=messages,
+    )
+
+
+@test(name="Decreasing (Wilcoxon)")
+@validate_classification_label
+def test_metamorphic_decreasing_wilcoxon(
+    model: BaseModel,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    slicing_function: SlicingFunction = None,
+    critical_quantile: float = 0.05,
+    classification_label: str = None,
+):
+    """
+    Summary: Tests if the model probability decreases when the feature values are perturbed
+
+    Description: Calculate the Wilcoxon signed-rank test on TWO RELATED samples. Sample (A) is the original probability predictions
+    while sample (B) is the probabilities after perturbation of one or more of the features.
+    This test computes the decreasing test to study if mean(B) < mean(A)
+    The test is passed when the p-value of the Wilcoxon signed-rank test between (A) and (B) is below the critical quantile
+
+    Example: For a credit scoring model, the test is passed when a decrease of wage by 10%,
+             causes a statistically significant probability decrease.
+
+    Args:
+        model(BaseModel):
+            Model used to compute the test
+        dataset(Dataset):
+            Dataset used to compute the test
+        transformation_function(TransformationFunction):
+            Function performing the perturbations to be applied on dataset.
+        slicing_function(Optional[SlicingFunction]):
+            Slicing function to be applied on dataset
+        critical_quantile(Optional[float]):
+            Critical quantile above which the null hypothesis cannot be rejected
+
+    Returns:
+        actual_slices_size:
+            Length of dataset tested
+        message:
+            Test result message
+        metric:
+            The Wilcoxon signed-rank test in terms of p-value between unchanged rows over the perturbed rows
+        passed:
+            TRUE if the p-value of the Wilcoxon signed-rank test between (A) and (B) is below the critical value
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(
+            sliced_dataset=dataset, dataset_name="dataset", test_name="test_metamorphic_decreasing_wilcoxon"
+        )
+
+    return _test_metamorphic_wilcoxon(
+        direction=Direction.Decreasing,
+        dataset=dataset,
+        model=model,
+        transformation_function=transformation_function,
+        classification_label=classification_label,
+        window_size=float("nan"),
+        critical_quantile=critical_quantile,
+    )
+
+
+@test(name="Increasing (Wilcoxon)")
+@validate_classification_label
+def test_metamorphic_increasing_wilcoxon(
+    model: BaseModel,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    slicing_function: SlicingFunction = None,
+    critical_quantile: float = 0.05,
+    classification_label: str = None,
+):
+    """
+    Summary: Tests if the model probability increases when the feature values are perturbed
+
+    Description: Calculate the Wilcoxon signed-rank test on TWO RELATED samples. Sample (A) is the original probability predictions
+    while sample (B) is the probabilities after perturbation of one or more of the features.
+    This test computes the increasing test to study if mean(A) < mean(B)
+    The test is passed when the p-value of the Wilcoxon signed-rank test between (A) and (B) is below the critical quantile
+
+    Example: For a credit scoring model, the test is passed when a decrease of wage by 10%,
+             causes a statistically significant probability increase.
+
+    Args:
+        model(BaseModel):
+            Model used to compute the test
+        dataset(Dataset):
+            Dataset used to compute the test
+        transformation_function(TransformationFunction):
+            Function performing the perturbations to be applied on dataset.
+        slicing_function(Optional[SlicingFunction]):
+            Slicing function to be applied on dataset
+        critical_quantile(Optional[float]):
+            Critical quantile above which the null hypothesis cannot be rejected
+
+    Returns:
+        actual_slices_size:
+            Length of dataset tested
+        message:
+            Test result message
+        metric:
+            The Wilcoxon signed-rank test in terms of p-value between unchanged rows over the perturbed rows
+        passed:
+            TRUE if the p-value of the Wilcoxon signed-rank test between (A) and (B) is below the critical value
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(
+            sliced_dataset=dataset, dataset_name="dataset", test_name="test_metamorphic_increasing_wilcoxon"
+        )
+
+    return _test_metamorphic_wilcoxon(
+        direction=Direction.Increasing,
+        dataset=dataset,
+        model=model,
+        transformation_function=transformation_function,
+        classification_label=classification_label,
+        window_size=float("nan"),
+        critical_quantile=critical_quantile,
+    )
+
+
+@test(name="Invariance (Wilcoxon)")
+def test_metamorphic_invariance_wilcoxon(
+    model: BaseModel,
+    dataset: Dataset,
+    transformation_function: TransformationFunction,
+    slicing_function: SlicingFunction = None,
+    window_size: float = 0.2,
+    critical_quantile: float = 0.05,
+) -> TestResult:
+    """
+    Summary: Tests if the model predictions are statistically invariant when the feature values are perturbed.
+
+    Description: Calculate the Wilcoxon signed-rank test on TWO RELATED samples. Sample (A) is the original probability predictions
+    while sample (B) is the probabilities after perturbation of one or more of the features.
+    This test computes the equivalence test to show that mean(B) - window_size/2 < mean(A) < mean(B) + window_size/2
+    The test is passed when the following tests pass:
+    - the p-value of the t-test between (A) and (B)+window_size/2 is below the critical quantile
+    - the p-value of the t-test between (B)-window_size/2 and (A) is below the critical quantile
+
+    Example: The test is passed when, after switching gender from male to female,
+    the probability distributions remains statistically invariant. In other words, the test is passed if the mean of the
+    perturbed sample is statistically within a window determined by the user.
+
+    Args:
+        model(BaseModel):
+            Model used to compute the test
+        dataset(Dataset):
+            Dataset used to compute the test
+        transformation_function(TransformationFunction):
+            Function performing the perturbations to be applied on dataset.
+        slicing_function(Optional[SlicingFunction]):
+            Slicing function to be applied on dataset
+        window_size(Optional[float]):
+            Probability window in which the mean of the perturbed sample can be in
+        critical_quantile(Optional[float]):
+            Critical quantile above which the null hypothesis cannot be rejected
+
+    Returns:
+        actual_slices_size:
+            Length of dataset tested
+        message:
+            Test result message
+        metric:
+            The t-test in terms of p-value between unchanged rows over the perturbed rows
+        passed:
+            TRUE if the p-value of the Wilcoxon signed-rank test between (A) and (B)+window_size/2 < critical_quantile && the p-value of the t-test between (B)-window_size/2 and (A) < critical_quantile
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(
+            sliced_dataset=dataset, dataset_name="dataset", test_name="test_metamorphic_invariance_wilcoxon"
+        )
+
+    return _test_metamorphic_wilcoxon(
+        direction=Direction.Invariant,
+        dataset=dataset,
+        model=model,
+        transformation_function=transformation_function,
+        window_size=window_size,
+        critical_quantile=critical_quantile,
+    )
```

### Comparing `giskard-1.9.1/giskard/ml_worker/testing/stat_utils.py` & `giskard-2.0.0b1/giskard/ml_worker/testing/stat_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,15 @@
     p_value < quantile ==> we support the alternative hypothesis
 
     less ==> alternative: mean(pop1) < mean(pop2)
     greater ==> alternative: mean(pop1) > mean(pop2)
     """
 
     if alternative not in ["less", "greater"]:
-        raise ValueError(
-            "Incorrect alternative hypothesis! It has to be one of the following: ['less', 'greater']"
-        )
+        raise ValueError("Incorrect alternative hypothesis! It has to be one of the following: ['less', 'greater']")
 
     if np.array_equal(population_1, population_2):
         p_value = 1.0
     else:
         _, p_value = stats.ttest_rel(population_1, population_2, alternative=alternative)
 
     return p_value <= critical_quantile, p_value
@@ -66,17 +64,15 @@
     p_value < quantile ==> we support the alternative hypothesis
 
     less ==> alternative: mean(pop1) < mean(pop2)
     greater ==> alternative: mean(pop1) > mean(pop2)
     """
 
     if alternative not in ["less", "greater"]:
-        raise ValueError(
-            "Incorrect alternative hypothesis! It has to be one of the following: ['less', 'greater']"
-        )
+        raise ValueError("Incorrect alternative hypothesis! It has to be one of the following: ['less', 'greater']")
 
     if np.array_equal(population_1, population_2):
         p_value = 1.0
     else:
         _, p_value = stats.wilcoxon(population_1, population_2, alternative=alternative)
 
     return p_value <= critical_quantile, p_value
```

### Comparing `giskard-1.9.1/giskard/ml_worker/testing/statistical_tests.py` & `giskard-2.0.0b1/giskard/testing/tests/statistic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,236 +1,228 @@
-import pandas as pd
+"""Statistical tests"""
 import numpy as np
-from typing import Callable
+import pandas as pd
+from typing import Optional, Iterable
+
+from giskard import test
+from giskard.datasets.base import Dataset
+from giskard.ml_worker.testing.test_result import TestResult, TestMessage, TestMessageLevel
+from giskard.ml_worker.testing.utils import validate_classification_label
+from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction
+from giskard.models.base import BaseModel
+from giskard.ml_worker.testing.utils import check_slice_not_empty
+
+
+@test(name="Right Label", tags=["heuristic", "classification"])
+@validate_classification_label
+def test_right_label(model: BaseModel, dataset: Dataset, classification_label: str,
+                     slicing_function: SlicingFunction = None, threshold: float = 0.5) -> TestResult:
+    """
+    Summary: Test if the model returns the right classification label for a slice
+
+    Description: The test is passed when the percentage of rows returning the right
+    classification label is higher than the threshold in a given slice
+
+    Example: For a credit scoring model, the test is passed when more than 50%
+    of people with high-salaries are classified as “non default”
+
+
+    Args:
+      model(BaseModel):
+          Model used to compute the test
+      dataset(Dataset):
+          Dataset used to compute the test
+      classification_label(str):
+          Classification label you want to test
+      slicing_function(Optional[SlicingFunction]):
+          Slicing function to be applied on the dataset
+      threshold(Optional[float]):
+          Threshold for the percentage of passed rows
+
+    Returns:
+      actual_slices_size:
+          Length of dataset tested
+      metrics:
+          The ratio of rows with the right classification label over the total of rows in the slice
+      passed:
+          TRUE if passed_ratio > threshold
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_right_label")
+
+    prediction_results = model.predict(dataset).prediction
+
+    passed_idx = dataset.df.loc[prediction_results == classification_label].index.values
+
+    passed_ratio = len(passed_idx) / len(dataset)
+    return TestResult(
+        actual_slices_size=[len(dataset)],
+        metric=passed_ratio,
+        passed=bool(passed_ratio > threshold),
+    )
+
+
+@test(name="Output in range", tags=["heuristic", "classification", "regression"])
+@validate_classification_label
+def test_output_in_range(model: BaseModel, dataset: Dataset, slicing_function: SlicingFunction = None,
+                         classification_label: str = None, min_range: float = 0.3, max_range: float = 0.7,
+                         threshold: float = 0.5) -> TestResult:
+    """
+    Summary: Test if the model output belongs to the right range for a slice
+
+    Description: - The test is passed when the ratio of rows in the right range inside the
+    slice is higher than the threshold.
+
+    For classification: Test if the predicted probability for a given classification label
+    belongs to the right range for a dataset slice
+
+    For regression : Test if the predicted output belongs to the right range for a dataset slice
+
+    Example :
+    For Classification: For a credit scoring model, the test is passed when more than 50% of
+    people with high wage have a probability of defaulting between 0 and 0.1
+
+    For Regression : The predicted Sale Price of a house in the city falls in a particular range
+
+
+    Args:
+        model(BaseModel):
+            Model used to compute the test
+        dataset(Dataset):
+            Dataset used to compute the test
+        slicing_function(Optional[SlicingFunction]):
+            Slicing function to be applied on the dataset
+        classification_label(Optional[str]):
+            Optional. Classification label you want to test
+        min_range(Optional[float]):
+            Minimum probability of occurrence of classification label
+        max_range(Optional[float]):
+            Maximum probability of occurrence of classification label
+        threshold(Optional[float]):
+            Threshold for the percentage of passed rows
+
+    Returns:
+        actual_slices_size:
+            Length of dataset tested
+        metrics:
+            The proportion of rows in the right range inside the slice
+        passed:
+            TRUE if metric > threshold
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_output_in_range")
+
+    results_df = pd.DataFrame()
+
+    prediction_results = model.predict(dataset)
+
+    if model.is_regression:
+        results_df["output"] = prediction_results.raw_prediction
+
+    elif model.is_classification:
+        results_df["output"] = prediction_results.all_predictions[classification_label]
+
+    else:
+        raise ValueError(f"Prediction task is not supported: {model.meta.model_type}")
+
+    passed_idx = dataset.df.loc[
+        (results_df["output"] <= max_range) & (results_df["output"] >= min_range)
+        ].index.values
+
+    passed_ratio = len(passed_idx) / len(dataset)
+
+    return TestResult(
+        actual_slices_size=[len(dataset)],
+        metric=passed_ratio,
+        passed=bool(passed_ratio >= threshold),
+    )
+
+
+@test(name="Disparate impact", tags=["heuristic", "classification"])
+def test_disparate_impact(model: BaseModel, dataset: Dataset, protected_slicing_function: SlicingFunction,
+                          unprotected_slicing_function: SlicingFunction, positive_outcome: Iterable,
+                          slicing_function: SlicingFunction = None, min_threshold: float = 0.8,
+                          max_threshold: float = 1.25) -> TestResult:
+    """
+    Summary: Tests if the model is biased more towards an unprotected slice of the dataset over a protected slice.
+    Note that this test reflects only a possible bias in the model while being agnostic to any biaas in the dataset
+    it trained on. The Disparate Impact (DI) is only valid for classification models and is computed as the ratio
+    between the average count of correct predictions for the protected slice over the unprotected one given a
+    certain positive_outcome.
+
+    Description: Calculate the Disparate Impact between a protected and unprotected slice of a dataset. Otherwise
+    known as the "80 percent" rule, the Disparate Impact determines if a model was having an "adverse impact" on a
+    protected (or minority in some cases) group.
+
+    Example: The rule was originally based on the rates at which job applicants were hired. For example, if XYZ
+    Company hired 50 percent of the men applying for work in a predominantly male occupation while hiring only 20
+    percent of the female applicants, one could look at the ratio of those two hiring rates to judge whether there
+    might be a discrimination problem. The ratio of 20:50 means that the rate of hiring for female applicants is
+    only 40 percent of the rate of hiring for male applicants. That is, 20 divided by 50 equals
+    0.40, which is equivalent to 40 percent. Clearly, 40 percent is well below the 80 percent that was arbitrarily
+    set as an acceptable difference in hiring rates. Therefore, in this example, XYZ Company could have been called
+    upon to prove that there was a legitimate reason for hiring men at a rate so much higher than the rate of hiring
+    women.
 
-from giskard.ml_worker.core.giskard_dataset import GiskardDataset
-from giskard.ml_worker.core.model import GiskardModel
-from giskard.ml_worker.generated.ml_worker_pb2 import SingleTestResult, TestMessage, TestMessageType
-from giskard.ml_worker.testing.abstract_test_collection import AbstractTestCollection
-
-
-class StatisticalTests(AbstractTestCollection):
-    def test_right_label(
-            self,
-            actual_slice: GiskardDataset,
-            model: GiskardModel,
-            classification_label: str,
-            threshold=0.5,
-    ) -> SingleTestResult:
-        """
-        Summary: Test if the model returns the right classification label for a slice
-
-        Description: The test is passed when the percentage of rows returning the right
-        classification label is higher than the threshold in a given slice
-
-        Example: For a credit scoring model, the test is passed when more than 50%
-        of people with high-salaries are classified as “non default”
-
-        Args:
-           actual_slice(GiskardDataset):
-              Slice of the  actual dataset
-          model(GiskardModel):
+    Args:
+          model(BaseModel):
               Model used to compute the test
-          classification_label(str):
-              Classification label you want to test
-          threshold(float):
-              Threshold for the percentage of passed rows
-
-        Returns:
-          actual_slices_size:
-              Length of actual_slice tested
-          metrics:
-              The ratio of rows with the right classification label over the total of rows in the slice
+          dataset(Dataset):
+              Dataset used to compute the test
+          protected_slicing_function(SlicingFunction):
+              Slicing function that defines the protected group from the full dataset given
+          unprotected_slicing_function(SlicingFunction):
+              Slicing function that defines the unprotected group from the full dataset given
+          positive_outcome(str or float):
+              The target value that is considered a positive outcome in the dataset
+          slicing_function(Optional[SlicingFunction]):
+              Slicing function to be applied on the dataset
+          min_threshold(Optional[float]):
+              Threshold below which the DI test is considered to fail, by default 0.8
+          max_threshold(Optional[float]):
+              Threshold above which the DI test is considered to fail, by default 1.25
+
+    Returns:
+          metric:
+              The disparate impact ratio
           passed:
-              TRUE if passed_ratio > threshold
-        """
-        actual_slice.df.reset_index(drop=True, inplace=True)
-        prediction_results = model.run_predict(actual_slice).prediction
-        assert (
-                classification_label in model.classification_labels
-        ), f'"{classification_label}" is not part of model labels: {",".join(model.classification_labels)}'
-
-        passed_idx = actual_slice.df.loc[prediction_results == classification_label].index.values
-
-        passed_ratio = len(passed_idx) / len(actual_slice)
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_slice)],
-                metric=passed_ratio,
-                passed=passed_ratio > threshold,
-            )
+              TRUE if the disparate impact ratio > min_threshold && disparate impact ratio < max_threshold
+    """
+    if slicing_function:
+        dataset = dataset.slice(slicing_function)
+        check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_disparate_impact")
+
+    if positive_outcome not in list(model.meta.classification_labels):
+        raise ValueError(
+            f"The positive outcome chosen {positive_outcome} is not part of the dataset target values {list(model.meta.classification_labels)}."
         )
 
-    def test_output_in_range(
-            self,
-            actual_slice: GiskardDataset,
-            model: GiskardModel,
-            classification_label=None,
-            min_range: float = 0.3,
-            max_range: float = 0.7,
-            threshold=0.5,
-    ) -> SingleTestResult:
-        """
-        Summary: Test if the model output belongs to the right range for a slice
-
-        Description: - The test is passed when the ratio of rows in the right range inside the
-        slice is higher than the threshold.
-
-         For classification: Test if the predicted probability for a given classification label
-         belongs to the right range for a dataset slice
-
-        For regression : Test if the predicted output belongs to the right range for a dataset slice
-
-        Example :
-        For Classification: For a credit scoring model, the test is passed when more than 50% of
-        people with high wage have a probability of defaulting between 0 and 0.1
-
-        For Regression : The predicted Sale Price of a house in the city falls in a particular range
-        Args:
-            actual_slice(GiskardDataset):
-                Slice of the actual dataset
-            model(GiskardModel):
-                Model used to compute the test
-            classification_label(str):
-                Optional. Classification label you want to test
-            min_range(float):
-                Minimum probability of occurrence of classification label
-            max_range(float):
-                Maximum probability of occurrence of classification label
-            threshold(float):
-                Threshold for the percentage of passed rows
-
-        Returns:
-            actual_slices_size:
-                Length of actual_slice tested
-            metrics:
-                The proportion of rows in the right range inside the slice
-            passed:
-                TRUE if metric > threshold
-        """
-        results_df = pd.DataFrame()
-        actual_slice.df.reset_index(drop=True, inplace=True)
-
-        prediction_results = model.run_predict(actual_slice)
-
-        if model.model_type == "regression":
-            results_df["output"] = prediction_results.raw_prediction
-
-        elif model.model_type == "classification":
-            assert (
-                    classification_label in model.classification_labels
-            ), f'"{classification_label}" is not part of model labels: {",".join(model.classification_labels)}'
-            results_df["output"] = prediction_results.all_predictions[classification_label]
-
-        else:
-            raise ValueError(f"Prediction task is not supported: {model.model_type}")
-
-        passed_idx = actual_slice.df.loc[
-            (results_df["output"] <= max_range) & (results_df["output"] >= min_range)
-            ].index.values
-
-        passed_ratio = len(passed_idx) / len(actual_slice)
-
-        return self.save_results(
-            SingleTestResult(
-                actual_slices_size=[len(actual_slice)],
-                metric=passed_ratio,
-                passed=passed_ratio >= threshold,
-            )
+    protected_ds = dataset.slice(protected_slicing_function)
+    unprotected_ds = dataset.slice(unprotected_slicing_function)
+
+    if protected_ds.df.equals(unprotected_ds.df):
+        raise ValueError(
+            "The protected and unprotected datasets are equal. Please check that you chose different slices."
         )
 
-    def test_disparate_impact(
-            self,
-            gsk_dataset: GiskardDataset,
-            protected_slice: Callable[[pd.DataFrame], pd.DataFrame],
-            unprotected_slice: Callable[[pd.DataFrame], pd.DataFrame],
-            model: GiskardModel,
-            positive_outcome,
-            min_threshold=0.8,
-            max_threshold=1.25,
-    ) -> SingleTestResult:
-
-        """
-        Summary: Tests if the model is biased more towards an unprotected slice of the dataset over a protected slice.
-        Note that this test reflects only a possible bias in the model while being agnostic to any bias in the dataset
-        it trained on. The Disparate Impact (DI) is only valid for classification models and is computed as the ratio
-        between the average count of correct predictions for the protected_slice over the unprotected_slice given a
-        certain positive_outcome.
-
-        Description: Calculate the Disparate Impact between a protected and unprotected slice of a dataset. Otherwise
-        known as the "80 percent" rule, the Disparate Impact determines if a model was having an "adverse impact" on a
-        protected (or minority in some cases) group.
-
-        Example: The rule was originally based on the rates at which job applicants were hired. For example, if XYZ
-        Company hired 50 percent of the men applying for work in a predominantly male occupation while hiring only 20
-        percent of the female applicants, one could look at the ratio of those two hiring rates to judge whether there
-        might be a discrimination problem. The ratio of 20:50 means that the rate of hiring for female applicants is
-        only 40 percent of the rate of hiring for male applicants. That is, 20 divided by 50 equals
-        0.40, which is equivalent to 40 percent. Clearly, 40 percent is well below the 80 percent that was arbitrarily
-        set as an acceptable difference in hiring rates. Therefore, in this example, XYZ Company could have been called
-        upon to prove that there was a legitimate reason for hiring men at a rate so much higher than the rate of hiring
-        women.
-
-        Args:
-              gsk_dataset(GiskardDataset):
-                  Dataset used to compute the test
-              protected_slice(Callable):
-                  Slice that defines the protected group from the full dataset given
-              unprotected_slice(Callable):
-                  Slice that defines the unprotected group from the full dataset given
-              model(GiskardModel):
-                  Model used to compute the test
-              positive_outcome(str or float):
-                  The target value that is considered a positive outcome in the dataset
-              min_threshold(float):
-                  Threshold below which the DI test is considered to fail, by default 0.8
-              max_threshold(float):
-                  Threshold above which the DI test is considered to fail, by default 1.25
-
-        Returns:
-              metric:
-                  The disparate impact ratio
-              passed:
-                  TRUE if the disparate impact ratio > min_threshold && disparate impact ratio < max_threshold
-        """
-
-        if positive_outcome not in gsk_dataset.df[gsk_dataset.target].values:
-            raise ValueError(
-                f"The positive outcome chosen {positive_outcome} is not part of the dataset columns {gsk_dataset.columns}."
-            )
-
-        gsk_dataset.df.reset_index(drop=True, inplace=True)
-        protected_ds = gsk_dataset.slice(protected_slice)
-        unprotected_ds = gsk_dataset.slice(unprotected_slice)
-
-        if protected_ds.df.equals(unprotected_ds.df):
-            raise ValueError(
-                "The protected and unprotected datasets are equal. Please check that you chose different slices."
-            )
+    positive_idx = list(model.meta.classification_labels).index(positive_outcome)
 
-        positive_idx = list(model.classification_labels).index(positive_outcome)
+    protected_predictions = np.squeeze(model.predict(protected_ds).raw_prediction == positive_idx)
+    unprotected_predictions = np.squeeze(model.predict(unprotected_ds).raw_prediction == positive_idx)
 
-        protected_predictions = np.squeeze(
-            model.run_predict(protected_ds).raw_prediction == positive_idx
-        )
-        unprotected_predictions = np.squeeze(
-            model.run_predict(unprotected_ds).raw_prediction == positive_idx
+    protected_proba = np.count_nonzero(protected_predictions) / len(protected_ds.df)
+    unprotected_proba = np.count_nonzero(unprotected_predictions) / len(unprotected_ds.df)
+    disparate_impact_score = protected_proba / unprotected_proba
+
+    messages = [
+        TestMessage(
+            type=TestMessageLevel.INFO, text=f"min_threshold = {min_threshold}, max_threshold = {max_threshold}"
         )
+    ]
 
-        protected_proba = np.count_nonzero(protected_predictions) / len(protected_ds.df)
-        unprotected_proba = np.count_nonzero(unprotected_predictions) / len(unprotected_ds.df)
-        disparate_impact_score = protected_proba / unprotected_proba
-
-        messages = [
-            TestMessage(
-                type=TestMessageType.INFO,
-                text=f"min_threshold = {min_threshold}, max_threshold = {max_threshold}",
-            )
-        ]
-
-        return self.save_results(
-            SingleTestResult(
-                metric=disparate_impact_score,
-                passed=(disparate_impact_score > min_threshold) * (disparate_impact_score < max_threshold),
-                messages=messages,
-            )
-        )
+    return TestResult(
+        metric=disparate_impact_score,
+        passed=bool((disparate_impact_score > min_threshold) * (disparate_impact_score < max_threshold)),
+        messages=messages,
+    )
```

### Comparing `giskard-1.9.1/giskard/ml_worker/utils/error_interceptor.py` & `giskard-2.0.0b1/giskard/ml_worker/utils/request_interceptor.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,51 +16,49 @@
 from giskard.ml_worker.exceptions.IllegalArgumentError import CodedError
 from giskard.ml_worker.generated.ml_worker_pb2 import MLWorkerErrorInfo
 
 MESSAGE_TYPE = Union[Message, Iterable[Message]]
 
 logger = logging.getLogger(__name__)
 
-pool = ThreadPoolExecutor()
+pool = ThreadPoolExecutor(thread_name_prefix="ml_worker_thread")
 
 
-class ErrorInterceptor(grpc.aio.ServerInterceptor):
+class MLWorkerRequestInterceptor(grpc.aio.ServerInterceptor):
     @staticmethod
-    async def terminate_with_exception(
-        error_code: StatusCode, e: Exception, context: ServicerContext
-    ):
+    async def terminate_with_exception(error_code: StatusCode, e: Exception, context: ServicerContext):
         detail = any_pb2.Any()
         detail.Pack(
             MLWorkerErrorInfo(
                 stack=traceback.format_exc(),
                 error=str(e),
             )
         )
         code, _ = error_code.value
         rich_status = Status(code=code, message=e.__class__.__name__, details=[detail])
         await context.abort_with_status(rpc_status.to_status(rich_status))
 
     async def intercept_service(
-        self,
-        continuation: Callable[[grpc.HandlerCallDetails], Awaitable[grpc.RpcMethodHandler]],
-        handler_call_details: grpc.HandlerCallDetails,
+            self,
+            continuation: Callable[[grpc.HandlerCallDetails], Awaitable[grpc.RpcMethodHandler]],
+            handler_call_details: grpc.HandlerCallDetails,
     ) -> grpc.RpcMethodHandler:
         def _wrapper(behavior):
             @functools.wraps(behavior)
             async def wrapper(request, context: aio.ServicerContext):
                 try:
                     loop = asyncio.get_running_loop()
                     res = await loop.run_in_executor(pool, behavior, request, context)
                     return res
                 except CodedError as e:
                     logger.exception(e)
-                    await ErrorInterceptor.terminate_with_exception(e.code, e, context)
+                    await MLWorkerRequestInterceptor.terminate_with_exception(e.code, e, context)
                 except Exception as e:
                     logger.exception(e)
-                    await ErrorInterceptor.terminate_with_exception(StatusCode.INTERNAL, e, context)
+                    await MLWorkerRequestInterceptor.terminate_with_exception(StatusCode.INTERNAL, e, context)
 
             return wrapper
 
         handler = await continuation(handler_call_details)
         if handler and (handler.request_streaming or handler.response_streaming):
             return handler
```

### Comparing `giskard-1.9.1/giskard/ml_worker/utils/logging.py` & `giskard-2.0.0b1/giskard/ml_worker/utils/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 def configure_logging():
     stdout_handler = logging.StreamHandler(stream=sys.stdout)
     logging.getLogger("shap").setLevel(logging.WARNING)
+    logging.getLogger("pyngrok").setLevel(logging.ERROR)
+    logging.getLogger("giskard").setLevel(logging.WARNING)
     logging.basicConfig(
         level=settings.loglevel,
         format="%(asctime)s pid:%(process)d %(threadName)s %(name)-12s %(levelname)-8s %(message)s",
         handlers=[stdout_handler],
     )
```

### Comparing `giskard-1.9.1/giskard/settings.py` & `giskard-2.0.0b1/giskard/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     home: str = "~/giskard-home"
     port: int = 50051
     host: str = "localhost"
     max_workers: int = 10
     max_send_message_length_mb: int = 1024
     max_receive_message_length_mb: int = 1024
     loglevel = "INFO"
+    cache_dir: str = "cache"
+    disable_analytics = False
 
     class Config:
         env_prefix = "GSK_"
 
     @property
     def home_dir(self) -> Path:
         return Path(expand_env_var(self.home))
```

### Comparing `giskard-1.9.1/pyproject.toml` & `giskard-2.0.0b1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,111 @@
-# Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
-requires = ["poetry_core>=1.2.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["setuptools>=61", "wheel", "grpcio-tools", "protobuf<=3.20.3"]
+build-backend = "setuptools.build_meta"
 
-[tool.poetry.scripts]
+[[tool.pdm.source]]
+type = "find_links"
+url = "https://download.pytorch.org/whl/cpu/torch_stable.html"
+name = "torch"
+
+
+
+[tool.pdm.scripts]
+proto = "setup.py grpc"
+# add "-n auto" to the pytest command to parallelize the execution
+test.cmd = "pytest -n auto -c pyproject.toml --cov=giskard tests --cov-report=xml"
+test.env = { GSK_DISABLE_ANALYTICS = "True"}
+lint = "flake8 giskard tests"
+doc = "python -m sphinx_autobuild docs docs/_build/html"
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "typing-extensions>=4.5.0",
+    "black>=23.3.0",
+    "bandit>=1.7.4",
+    "darglint>=1.8.1",
+    "flake8>=3.9.2",
+    "jupyter>=1.0.0",
+    "jupyterlab>=3.4.2",
+    "pre-commit>=2.19.0",
+    "pydocstyle>=6.1.1",
+    "pylint>=2.13.9",
+    "pyupgrade>=2.32.1",
+    "safety>=1.10.3",
+    "mypy>=0.982",
+    "deptry>=0.5.13",
+    "httpretty>=1.1.4",
+    "isort[colors]>=5.12.0",
+    "pip>=23.1.2",
+    "langchain>=0.0.187",
+    "nltk>=3.8.1",
+    "xgboost>=1.7.5",
+    "lightgbm>=3.3.5",
+    "imbalanced-learn>=0.10.1",
+    "pytest-xdist>=3.3.1",
+]
+proto = [
+    "grpcio-tools>=1.46.3",
+    "mypy-protobuf>=3.2.0",
+    "mypy-extensions>=0.4.3",
+]
+test = [
+    "pytest-cov>=4.0.0",
+    "pytest>=7.1.2",
+    "catboost>=1.1.1",
+    "requests-mock>=1.10.0",
+    "tensorflow-hub>=0.12.0",
+    "transformers>=4.27.4",
+    "torch>=2.0.0",
+    "torchdata>=0.6.0",
+    "torchtext>=0.15.1",
+    "portalocker>=2.0.0",
+    "scikit-learn==1.0.2",
+    "tensorflow-macos>=2.8.0, <2.10; sys_platform == 'darwin' and platform_machine == 'arm64'",
+    "tensorflow>=2.8.0, <2.10; sys_platform != 'darwin' or platform_machine != 'arm64'",
+    "tensorflow-text>=2.8.0, <2.10; sys_platform != 'darwin' or platform_machine != 'arm64'",
+]
+doc = [
+    "furo>=2023.5.20",
+    "myst-parser>=1.0.0",
+    "sphinx-autobuild>=2021.3.14",
+    "sphinx>=6.1.3",
+    "sphinxcontrib-napoleon>=0.7",
+    "sphinx-autoapi>=2.1.0",
+    "sphinx-rtd-theme>=1.2.0",
+    "sphinx-tabs>=3.4.1",
+    "sphinx-design>=0.4.1",
+    "sphinx-copybutton>=0.5.2",
+    "sphinx-click>=4.4.0",
+    "nbsphinx>=0.9.2",
+]
+
+[tool.setuptools.packages.find]
+include = ["giskard*"]
+exclude = ["docs*", "tests*"]
+
+[tool.setuptools.package-data]
+giskard = ["**/*.html", "**/*.css", "**/*.js", "**/*.json", "**/*titanic.csv"]
+
+[project.scripts]
 giskard = "giskard.cli:cli"
 
-[tool.poetry]
+[project.urls]
+repository = "https://github.com/Giskard-AI/giskard"
+homepage = "https://giskard-ai"
+
+[project]
 name = "giskard"
-version = "1.9.1"
-description = "Inspect your AI models visually, find bugs, give feedback 🕵️‍♀️ 💬"
 readme = "README.md"
-authors = ["Giskard AI <hello@giskard.ai>"]
-license = "Apache Software License 2.0"
-repository = "https://github.com/Giskard-AI/python-client"
-homepage = "https://github.com/Giskard-AI/python-client"
-include = ["giskard/ml_worker/generated/*"]
-
-# Keywords description https://python-poetry.org/docs/pyproject/#keywords
+license = { text = "Apache Software License 2.0" }
+version = "2.0.0b1"
+description = "Inspect your AI models visually, find bugs, give feedback 🕵️‍♀️ 💬"
+authors = [
+    { name = "Giskard AI", email = "hello@giskard.ai" },
+]
 keywords = [
     "Artificial Intelligence",
     "Machine Learning",
     "Quality",
     "MLOps"
 ]
 
@@ -29,81 +113,72 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
+requires-python = ">=3.8.1,<3.12"
+dependencies = [
+    "cloudpickle>=1.1.1",
+    "zstandard>=0.10.0 ",
+    "mlflow-skinny>=2",
+    "numpy>=1.22.0,<1.24.0", # shap doesn't work with numpy>1.24.0: module 'numpy' has no attribute 'int'
+    "scikit-learn>=1.0",
+    "scipy",
+    "mixpanel>=4.4.0",
+    "requests>=2.19",
+    "pydantic>=1.7",
+    "tqdm>=4.42.0",
+    "setuptools>=39.1.0,<68.0.0",
+    "pandas>=1.3.4,<2",
+    "xxhash>=3.2.0",
+    "langdetect>=1.0.9",
+    "chardet", # text metadata
+    "jinja2>=3", # scan template (temporary)
+    "requests-toolbelt>=0.9.1",
+]
 
-
-[tool.poetry.dependencies]
-python = ">=3.7.5,<3.11"
-cloudpickle = "^2.1.0"
-importlib_metadata = { version = "^4.11.4" }
-numpy = ">=1.21.6,<1.22.0"
-pandas = "^1.3.5"
-pydantic = "^1.10.2"
-requests-toolbelt = "^0.9.1"
-scikit-learn = ">=1.0.0,<1.1.0"
-mixpanel = "^4.10.0"
-beautifulsoup4 = "^4.11.1"
-eli5 = "^0.13.0"
-grpcio = "^1.46.3, <= 1.51.1"
-grpcio-status = "^1.46.3, <= 1.51.1"
-protobuf = "^3.9.2"
-tenacity = "^8.1.0"
-python-daemon = "^2.3.1"
-click = "^8.1.3"
-lockfile = "^0.12.2"
-psutil = "^5.9.2"
-requests = "^2.28.1"
-tqdm = "^4.64.1"
-setuptools = ">=65.4.1,<68.0.0"
-zstandard = "0.20.0"
-scipy = ">=1.7.2,<1.8"
-shap = "^0.41.0"
-ipython = "^7.0.0"
-
-[tool.poetry.group.dev.dependencies]
-typing-extensions = "^4.1.0"
-black = "^22.8.0"
-bandit = "^1.7.4"
-darglint = "^1.8.1"
-flake8 = "^3.9.2"
-isort = { extras = ["colors"], version = "^5.10.1" }
-jupyter = "^1.0.0"
-jupyterlab = "^3.4.2"
-pre-commit = "^2.19.0"
-pydocstyle = "^6.1.1"
-pylint = "^2.13.9"
-pyupgrade = "^2.32.1"
-safety = "^1.10.3"
-grpcio-tools = "^1.46.3"
-mypy-protobuf = "^3.2.0"
-mypy-extensions = "^0.4.3"
-mypy = "^0.982"
-deptry = "^0.5.13"
-httpretty = "^1.1.4"
-
-[tool.poetry.group.test.dependencies]
-pytest-cov = "^3.0.0"
-pytest = "^7.1.2"
-catboost = "^1.1"
+[project.optional-dependencies]
+llm = [
+    "transformers",
+    "torch",
+    "langchain",
+    "datasets",
+    "evaluate",
+    "rouge_score",
+]
+server = [
+    "tenacity>=4.11.0",
+    "psutil>=5.4.6",
+    "click>=7.0",
+    "docker>=6.0.0",
+    "shap>=0.41.0",
+    "eli5>=0.12.0",
+    "ipython", # eli5.show_prediction doesn't work without ipython
+    "grpcio>=1.39.0,<=1.51.1",
+    "grpcio-status>=1.16.0,<=1.51.1",
+    "lockfile>=0.12.2",
+    "protobuf<=3.20.3",
+    "python-daemon>=2.2.2,<3",
+    "pycryptodome>=3.6.1",
+    "pyngrok>=6.0.0",
+]
 
 [tool.black]
 # https://github.com/psf/black
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310']
 line-length = 120
 color = true
+skip-string-normalization = true
 
 exclude = '''
 /(
     \.git
     | \.hg
     | \.mypy_cache
     | \.tox
@@ -116,28 +191,28 @@
     | venv
     | giskard/ml_worker/generated
 )/
 '''
 
 [tool.isort]
 # https://github.com/timothycrosley/isort/
-py_version = 37
+py_version = 38
 line_length = 100
 
 known_typing = ["typing", "types", "typing_extensions", "mypy", "mypy_extensions"]
 sections = ["FUTURE", "TYPING", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 include_trailing_comma = true
 profile = "black"
 multi_line_output = 3
 indent = 4
 color_output = true
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
-python_version = 3.7
+python_version = 3.8
 pretty = true
 show_traceback = true
 color_output = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 plugins = ["pydantic.mypy"]
@@ -155,24 +230,19 @@
 warn_no_return = false
 warn_redundant_casts = true
 warn_return_any = false
 warn_unreachable = true
 warn_unused_configs = false
 warn_unused_ignores = false
 
-
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 # Directories that are not visited by pytest collector:
 norecursedirs = ["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
 doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
 # Extra options:
 addopts = [
     "--strict-markers",
     "--tb=short",
     "--doctest-modules",
     "--doctest-continue-on-failure",
 ]
-
-[virtualenvs]
-create = true
-in-project = true
```

### Comparing `giskard-1.9.1/PKG-INFO` & `giskard-2.0.0b1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,29 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 1.9.1
+Version: 2.0.0b1
 Summary: Inspect your AI models visually, find bugs, give feedback 🕵️‍♀️ 💬
-Home-page: https://github.com/Giskard-AI/python-client
+Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
+Project-URL: repository, https://github.com/Giskard-AI/giskard
+Project-URL: homepage, https://giskard-ai
 Keywords: Artificial Intelligence,Machine Learning,Quality,MLOps
-Author: Giskard AI
-Author-email: hello@giskard.ai
-Requires-Python: >=3.7.5,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: cloudpickle (>=2.1.0,<3.0.0)
-Requires-Dist: eli5 (>=0.13.0,<0.14.0)
-Requires-Dist: grpcio (>=1.46.3,<=1.51.1)
-Requires-Dist: grpcio-status (>=1.46.3,<=1.51.1)
-Requires-Dist: importlib_metadata (>=4.11.4,<5.0.0)
-Requires-Dist: ipython (>=7.0.0,<8.0.0)
-Requires-Dist: lockfile (>=0.12.2,<0.13.0)
-Requires-Dist: mixpanel (>=4.10.0,<5.0.0)
-Requires-Dist: numpy (>=1.21.6,<1.22.0)
-Requires-Dist: pandas (>=1.3.5,<2.0.0)
-Requires-Dist: protobuf (>=3.9.2,<4.0.0)
-Requires-Dist: psutil (>=5.9.2,<6.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: python-daemon (>=2.3.1,<3.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
-Requires-Dist: scikit-learn (>=1.0.0,<1.1.0)
-Requires-Dist: scipy (>=1.7.2,<1.8)
-Requires-Dist: setuptools (>=65.4.1,<68.0.0)
-Requires-Dist: shap (>=0.41.0,<0.42.0)
-Requires-Dist: tenacity (>=8.1.0,<9.0.0)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: zstandard (==0.20.0)
-Project-URL: Repository, https://github.com/Giskard-AI/python-client
+Requires-Python: <3.12,>=3.8.1
 Description-Content-Type: text/markdown
+Provides-Extra: llm
+Provides-Extra: server
 
 # Giskard Client
 
 <div align="center">
 
 [![Python Version](https://img.shields.io/pypi/pyversions/python-client.svg)](https://pypi.org/project/python-client/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/Giskard-AI/python-client/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
@@ -408,8 +378,7 @@
   howpublished = {\url{https://github.com/Giskard-AI/python-client
 }
 ```
 
 ## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
 
 This project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)
-
```

