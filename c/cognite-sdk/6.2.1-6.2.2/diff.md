# Comparing `tmp/cognite_sdk-6.2.1.tar.gz` & `tmp/cognite_sdk-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.2.1.tar", max compression
+gzip compressed data, was "cognite_sdk-6.2.2.tar", max compression
```

## Comparing `cognite_sdk-6.2.1.tar` & `cognite_sdk-6.2.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0    11349 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/LICENSE
--rw-r--r--   0        0        0     3945 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/README.md
--rw-r--r--   0        0        0      503 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48450 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/assets.py
--rw-r--r--   0        0        0      573 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/data_modeling.py
--rw-r--r--   0        0        0    11025 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20644 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17419 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44319 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49915 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9297 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-05-26 06:54:28.807018 cognite_sdk-6.2.1/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     6483 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/spaces.py
--rw-r--r--   0        0        0     7909 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32111 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27928 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21012 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4638 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9570 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    37531 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/config.py
--rw-r--r--   0        0        0    18062 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/credentials.py
--rw-r--r--   0        0        0     8901 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34178 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-05-26 06:54:28.811019 cognite_sdk-6.2.1/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14299 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0     1753 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/spaces.py
--rw-r--r--   0        0        0    16814 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/py.typed
--rw-r--r--   0        0        0     8434 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7277 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-05-26 06:54:28.815019 cognite_sdk-6.2.1/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2133 2023-05-26 06:54:28.819018 cognite_sdk-6.2.1/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/README.md
+-rw-r--r--   0        0        0      503 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49083 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0      573 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/data_modeling.py
+-rw-r--r--   0        0        0    11025 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87459 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21276 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17320 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45329 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49915 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9466 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     6483 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/spaces.py
+-rw-r--r--   0        0        0     7909 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27887 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21811 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4589 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9525 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    37531 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      140 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/config.py
+-rw-r--r--   0        0        0    18062 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8901 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34178 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14299 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0     1753 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/spaces.py
+-rw-r--r--   0        0        0    16814 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/py.typed
+-rw-r--r--   0        0        0     8434 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7894 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7277 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2001 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2133 2023-06-05 09:54:54.654897 cognite_sdk-6.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.2.2/PKG-INFO
```

### Comparing `cognite_sdk-6.2.1/LICENSE` & `cognite_sdk-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/README.md` & `cognite_sdk-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/annotations.py` & `cognite_sdk-6.2.2/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/assets.py` & `cognite_sdk-6.2.2/cognite/client/_api/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,17 @@
             created_time (Union[Dict[str, int], TimestampRange]):  Range between two timestamps. Possible keys are `min` and `max`, with values given as time stamps in ms.
             last_updated_time (Union[Dict[str, int], TimestampRange]):  Range between two timestamps. Possible keys are `min` and `max`, with values given as time stamps in ms.
             root (bool): filtered assets are root assets or not
             external_id_prefix (str): Filter by this (case-sensitive) prefix for the external ID.
             aggregated_properties (Sequence[str]): Set of aggregated properties to include.
             limit (int, optional): Maximum number of assets to return. Defaults to return all items.
             partitions (int): Retrieve assets in parallel using this number of workers. Also requires `limit=None` to be passed.
+                To prevent unexpected problems and maximize read throughput, API documentation recommends at most use 10 partitions.
+                When using more than 10 partitions, actual throughout decreases.
+                In future releases of the APIs, CDF may reject requests with more than 10 partitions.
 
         Yields:
             Union[Asset, AssetList]: yields Asset one by one if chunk_size is not specified, else AssetList objects.
         """
         if aggregated_properties:
             aggregated_properties = [to_camel_case(s) for s in aggregated_properties]
 
@@ -250,14 +253,18 @@
             source (str): The source of this asset.
             created_time (Union[Dict[str, int], TimestampRange]):  Range between two timestamps. Possible keys are `min` and `max`, with values given as time stamps in ms.
             last_updated_time (Union[Dict[str, int], TimestampRange]):  Range between two timestamps. Possible keys are `min` and `max`, with values given as time stamps in ms.
             root (bool): filtered assets are root assets or not.
             external_id_prefix (str): Filter by this (case-sensitive) prefix for the external ID.
             aggregated_properties (Sequence[str]): Set of aggregated properties to include.
             partitions (int): Retrieve assets in parallel using this number of workers. Also requires `limit=None` to be passed.
+                To prevent unexpected problems and maximize read throughput, API documentation recommends at most use 10 partitions.
+                When using more than 10 partitions, actual throughout decreases.
+                In future releases of the APIs, CDF may reject requests with more than 10 partitions.
+
             limit (int, optional): Maximum number of assets to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
 
         Returns:
             AssetList: List of requested assets
 
         Examples:
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/data_modeling.py` & `cognite_sdk-6.2.2/cognite/client/_api/data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/data_sets.py` & `cognite_sdk-6.2.2/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.2.2/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/datapoints.py` & `cognite_sdk-6.2.2/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/diagrams.py` & `cognite_sdk-6.2.2/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.2.2/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/events.py` & `cognite_sdk-6.2.2/cognite/client/_api/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,17 @@
             source (str): The source of this event.
             created_time (Union[Dict[str, int], TimestampRange]):  Range between two timestamps. Possible keys are `min` and `max`, with values given as time stamps in ms.
             last_updated_time (Union[Dict[str, int], TimestampRange]):  Range between two timestamps. Possible keys are `min` and `max`, with values given as time stamps in ms.
             external_id_prefix (str): External Id provided by client. Should be unique within the project
             sort (Sequence[str]): Sort by array of selected fields. Ex: ["startTime:desc']. Default sort order is asc when ommitted. Filter accepts following field names: startTime, endTime, createdTime, lastUpdatedTime. We only support 1 field for now.
             limit (int, optional): Maximum number of events to return. Defaults to return all items.
             partitions (int): Retrieve assets in parallel using this number of workers. Also requires `limit=None` to be passed.
+                To prevent unexpected problems and maximize read throughput, API documentation recommends at most use 10 partitions.
+                When using more than 10 partitions, actual throughout decreases.
+                In future releases of the APIs, CDF may reject requests with more than 10 partitions.
 
         Yields:
             Union[Event, EventList]: yields Event one by one if chunk_size is not specified, else EventList objects.
         """
         asset_subtree_ids_processed = process_asset_subtree_ids(asset_subtree_ids, asset_subtree_external_ids)
         data_set_ids_processed = process_data_set_ids(data_set_ids, data_set_external_ids)
 
@@ -214,14 +217,17 @@
             data_set_external_ids (Sequence[str]): Return only events in the specified data set(s) with this external id / these external ids.
             source (str): The source of this event.
             created_time (Union[Dict[str, int], TimestampRange]):  Range between two timestamps. Possible keys are `min` and `max`, with values given as time stamps in ms.
             last_updated_time (Union[Dict[str, int], TimestampRange]):  Range between two timestamps. Possible keys are `min` and `max`, with values given as time stamps in ms.
             external_id_prefix (str): External Id provided by client. Should be unique within the project.
             sort (Sequence[str]): Sort by array of selected fields. Ex: ["startTime:desc']. Default sort order is asc when ommitted. Filter accepts following field names: startTime, endTime, createdTime, lastUpdatedTime. We only support 1 field for now.
             partitions (int): Retrieve events in parallel using this number of workers. Also requires `limit=None` to be passed.
+                To prevent unexpected problems and maximize read throughput, API documentation recommends at most use 10 partitions.
+                When using more than 10 partitions, actual throughout decreases.
+                In future releases of the APIs, CDF may reject requests with more than 10 partitions.
             limit (int, optional): Maximum number of events to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
 
         Returns:
             EventList: List of requested events
 
         Examples:
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.2.2/cognite/client/_api/extractionpipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,14 @@
             update_cls=ExtractionPipelineUpdate,
             items=item,
         )
 
 
 class ExtractionPipelineRunsAPI(APIClient):
     _RESOURCE_PATH = "/extpipes/runs"
-    _LIST_CLASS = ExtractionPipelineRunList
 
     def list(
         self,
         external_id: str,
         statuses: Sequence[str] = None,
         message_substring: str = None,
         created_time: Union[Dict[str, Any], TimestampRange] = None,
@@ -313,15 +312,14 @@
         """
         utils._auxiliary.assert_type(run, "run", [ExtractionPipelineRun, Sequence])
         return self._create_multiple(list_cls=ExtractionPipelineRunList, resource_cls=ExtractionPipelineRun, items=run)
 
 
 class ExtractionPipelineConfigsAPI(APIClient):
     _RESOURCE_PATH = "/extpipes/config"
-    _LIST_CLASS = ExtractionPipelineConfigRevisionList
 
     def retrieve(
         self, external_id: str, revision: Optional[int] = None, active_at_time: Optional[int] = None
     ) -> ExtractionPipelineConfig:
         """`Retrieve a specific configuration revision, or the latest by default <https://docs.cognite.com/api/v1/#tag/Extraction-Pipelines-Config/operation/getExtPipeConfigRevision>`
 
         By default the latest configuration revision is retrieved, or you can specify a timestamp or a revision number.
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/files.py` & `cognite_sdk-6.2.2/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/functions.py` & `cognite_sdk-6.2.2/cognite/client/_api/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     if identifier.is_singleton():
         return identifier[0]
     raise AssertionError("Exactly one of function_id and function_external_id must be specified")
 
 
 class FunctionsAPI(APIClient):
     _RESOURCE_PATH = "/functions"
-    _LIST_CLASS = FunctionList
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self.calls = FunctionCallsAPI(config, api_version, cognite_client)
         self.schedules = FunctionSchedulesAPI(config, api_version, cognite_client)
         # Variable used to guarantee all items are returned when list(limit) is None, inf or -1.
         self._LIST_LIMIT_CEILING = 10_000
@@ -279,15 +278,15 @@
             file_id=file_id,
             status=status,
             external_id_prefix=external_id_prefix,
             created_time=created_time,
         ).dump(camel_case=True)
         res = self._post(url_path=f"{self._RESOURCE_PATH}/list", json={"filter": filter, "limit": limit})
 
-        return self._LIST_CLASS._load(res.json()["items"], cognite_client=self._cognite_client)
+        return FunctionList._load(res.json()["items"], cognite_client=self._cognite_client)
 
     def retrieve(
         self, id: Optional[int] = None, external_id: Optional[str] = None
     ) -> Union[FunctionList, Function, None]:
         """`Retrieve a single function by id. <https://docs.cognite.com/api/v1/#operation/byIdsFunctions>`_
 
         Args:
@@ -654,15 +653,17 @@
 
 def _sanitize_filename(filename: str) -> str:
     # Forwardslash, '/', is not allowed in file names:
     return filename.replace("/", "-")
 
 
 class FunctionCallsAPI(APIClient):
-    _LIST_CLASS = FunctionCallList
+    _RESOURCE_PATH = "/functions/{}/calls"
+    _RESOURCE_PATH_RESPONSE = "/functions/{}/calls/{}/response"
+    _RESOURCE_PATH_LOGS = "/functions/{}/calls/{}/logs"
 
     def list(
         self,
         function_id: Optional[int] = None,
         function_external_id: Optional[str] = None,
         status: Optional[str] = None,
         schedule_id: Optional[int] = None,
@@ -701,15 +702,15 @@
 
         """
         identifier = _get_function_identifier(function_id, function_external_id)
         function_id = _get_function_internal_id(self._cognite_client, identifier)
         filter = FunctionCallsFilter(
             status=status, schedule_id=schedule_id, start_time=start_time, end_time=end_time
         ).dump(camel_case=True)
-        resource_path = f"/functions/{function_id}/calls"
+        resource_path = self._RESOURCE_PATH.format(function_id)
         return self._list(
             method="POST",
             resource_path=resource_path,
             filter=filter,
             limit=limit,
             resource_cls=FunctionCall,
             list_cls=FunctionCallList,
@@ -743,36 +744,36 @@
                 >>> func = c.functions.retrieve(id=1)
                 >>> call = func.retrieve_call(id=2)
 
         """
         identifier = _get_function_identifier(function_id, function_external_id)
         function_id = _get_function_internal_id(self._cognite_client, identifier)
 
-        resource_path = f"/functions/{function_id}/calls"
+        resource_path = self._RESOURCE_PATH.format(function_id)
         identifiers = IdentifierSequence.load(ids=call_id).as_singleton()
 
         return self._retrieve_multiple(
             resource_path=resource_path,
             identifiers=identifiers,
             resource_cls=FunctionCall,
             list_cls=FunctionCallList,
         )
 
     def get_response(
         self, call_id: int, function_id: Optional[int] = None, function_external_id: Optional[str] = None
-    ) -> Dict:
+    ) -> Optional[Dict]:
         """`Retrieve the response from a function call. <https://docs.cognite.com/api/v1/#operation/getFunctionCallResponse>`_
 
         Args:
             call_id (int): ID of the call.
             function_id (int, optional): ID of the function on which the call was made.
             function_external_id (str, optional): External ID of the function on which the call was made.
 
         Returns:
-            Response from the function call.
+            Dict[str, Any] | None: Response from the function call.
 
         Examples:
 
             Retrieve function call response by call ID::
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
@@ -784,17 +785,17 @@
                 >>> c = CogniteClient()
                 >>> call = c.functions.calls.retrieve(call_id=2, function_id=1)
                 >>> response = call.get_response()
 
         """
         identifier = _get_function_identifier(function_id, function_external_id)
         function_id = _get_function_internal_id(self._cognite_client, identifier)
-        url = f"/functions/{function_id}/calls/{call_id}/response"
-        res = self._get(url)
-        return res.json().get("response")
+
+        resource_path = self._RESOURCE_PATH_RESPONSE.format(function_id, call_id)
+        return self._get(resource_path).json().get("response")
 
     def get_logs(
         self, call_id: int, function_id: Optional[int] = None, function_external_id: Optional[str] = None
     ) -> FunctionCallLog:
         """`Retrieve logs for function call. <https://docs.cognite.com/api/v1/#operation/getFunctionCalls>`_
 
         Args:
@@ -820,37 +821,34 @@
                 >>> call = c.functions.calls.retrieve(call_id=2, function_id=1)
                 >>> logs = call.get_logs()
 
         """
         identifier = _get_function_identifier(function_id, function_external_id)
         function_id = _get_function_internal_id(self._cognite_client, identifier)
 
-        url = f"/functions/{function_id}/calls/{call_id}/logs"
-        res = self._get(url)
-        return FunctionCallLog._load(res.json()["items"])
+        resource_path = self._RESOURCE_PATH_LOGS.format(function_id, call_id)
+        return FunctionCallLog._load(self._get(resource_path).json()["items"])
 
 
 class FunctionSchedulesAPI(APIClient):
     _RESOURCE_PATH = "/functions/schedules"
-    _LIST_CLASS = FunctionSchedulesList
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self._LIST_LIMIT_CEILING = 10_000
 
     def retrieve(self, id: int) -> Union[FunctionSchedule, FunctionSchedulesList, None]:
         """`Retrieve a single function schedule by id. <https://docs.cognite.com/api/v1/#operation/byIdsFunctionSchedules>`_
 
         Args:
             id (int): ID
 
         Returns:
             Optional[FunctionSchedule]: Requested function schedule.
 
-
         Examples:
 
             Get function schedule by id::
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.functions.schedules.retrieve(id=1)
@@ -912,16 +910,17 @@
             function_id=function_id,
             function_external_id=function_external_id,
             created_time=created_time,
             cron_expression=cron_expression,
         ).dump(camel_case=True)
         res = self._post(url_path=f"{self._RESOURCE_PATH}/list", json={"filter": filter, "limit": limit})
 
-        return self._LIST_CLASS._load(res.json()["items"], cognite_client=self._cognite_client)
+        return FunctionSchedulesList._load(res.json()["items"], cognite_client=self._cognite_client)
 
+    # TODO: Major version 7, remove 'function_external_id' which only worked when using API-keys.
     def create(
         self,
         name: str,
         cron_expression: str,
         function_id: Optional[int] = None,
         function_external_id: Optional[str] = None,
         client_credentials: Union[Dict, ClientCredentials, None] = None,
@@ -929,49 +928,61 @@
         data: Optional[Dict] = None,
     ) -> FunctionSchedule:
         """`Create a schedule associated with a specific project. <https://docs.cognite.com/api/v1/#operation/postFunctionSchedules>`_
 
         Args:
             name (str): Name of the schedule.
             function_id (optional, int): Id of the function. This is required if the schedule is created with client_credentials.
-            function_external_id (optional, str): External id of the function. This is deprecated and cannot be used together with client_credentials.
+            function_external_id (optional, str): External id of the function. **NOTE**: This is deprecated and will be removed in a future major version.
             description (str): Description of the schedule.
             cron_expression (str): Cron expression.
             client_credentials: (optional, ClientCredentials, Dict): Instance of ClientCredentials or a dictionary containing client credentials:
                 client_id
                 client_secret
-            data (optional, Dict): Data to be passed to the scheduled run. **WARNING:** Secrets or other confidential information should not be passed via this argument. There is a dedicated `secrets` argument in FunctionsAPI.create() for this purpose.
+            data (optional, Dict): Data to be passed to the scheduled run.
 
         Returns:
             FunctionSchedule: Created function schedule.
 
+        Warning:
+            Do not pass secrets or other confidential information via the ``data`` argument. There is a dedicated
+            ``secrets`` argument in FunctionsAPI.create() for this purpose.
+
         Examples:
 
-            Create function schedule::
+            Create a function schedule that runs using specified client credentials (**recommended**)::
 
+                >>> import os
                 >>> from cognite.client import CogniteClient
                 >>> from cognite.client.data_classes import ClientCredentials
                 >>> c = CogniteClient()
                 >>> schedule = c.functions.schedules.create(
-                ...     name= "My schedule",
+                ...     name="My schedule",
                 ...     function_id=123,
                 ...     cron_expression="*/5 * * * *",
-                ...     client_credentials=ClientCredentials("my-client-id", "my-client-secret"),
-                ...     description="This schedule does magic stuff."
+                ...     client_credentials=ClientCredentials("my-client-id", os.environ["MY_CLIENT_SECRET"]),
+                ...     description="This schedule does magic stuff.",
+                ...     data={"magic": "stuff"},
                 ... )
 
-        """
-        _get_function_identifier(function_id, function_external_id)
+            You may also create a schedule that runs with your -current- credentials, i.e. the same credentials you used
+            to instantiate the ``CogniteClient`` (that you're using right now). **Note**: Unless you happen to already use
+            client credentials, *this is not a recommended way to create schedules*, as it will create an explicit dependency
+            on your user account, which it will run the function "on behalf of" (until the schedule is eventually removed)::
 
-        nonce = None
-        if client_credentials is not None:
-            if function_id is None:
-                raise ValueError("When passing 'client_credentials', 'function_id' must be set")
-            nonce = _create_session_and_return_nonce(self._cognite_client, client_credentials)
+                >>> schedule = c.functions.schedules.create(
+                ...     name="My schedule",
+                ...     function_id=456,
+                ...     cron_expression="*/5 * * * *",
+                ...     description="A schedule just used for some temporary testing.",
+                ... )
 
+        """
+        _get_function_identifier(function_id, function_external_id)
+        nonce = _create_session_and_return_nonce(self._cognite_client, client_credentials)
         body: Dict[str, List[Dict[str, Union[str, int, None, Dict]]]] = {
             "items": [
                 {
                     "name": name,
                     "description": description,
                     "functionId": function_id,
                     "functionExternalId": function_external_id,
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/geospatial.py` & `cognite_sdk-6.2.2/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/iam.py` & `cognite_sdk-6.2.2/cognite/client/_api/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,20 +168,27 @@
     def inspect(self) -> TokenInspection:
         """Inspect a token.
 
         Get details about which projects it belongs to and which capabilities are granted to it.
 
         Returns:
             TokenInspection: The object with token inspection details.
+
+        Example:
+
+            Inspect token::
+
+                >>> from cognite.client import CogniteClient
+                >>> c = CogniteClient()
+                >>> res = c.iam.token.inspect()
         """
         return TokenInspection._load(self._get("/api/v1/token/inspect").json())
 
 
 class SessionsAPI(APIClient):
-    _LIST_CLASS = SessionList
     _RESOURCE_PATH = "/sessions"
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self._LIST_LIMIT = 100
 
     def create(self, client_credentials: Optional[ClientCredentials] = None) -> CreatedSession:
@@ -211,20 +218,20 @@
 
         Returns:
             SessionList: List of revoked sessions. If the user does not have the sessionsAcl:LIST capability, then only the session IDs will be present in the response.
         """
         identifiers = IdentifierSequence.load(ids=id, external_ids=None)
         items = {"items": identifiers.as_dicts()}
 
-        return self._LIST_CLASS._load(self._post(self._RESOURCE_PATH + "/revoke", items).json()["items"])
+        return SessionList._load(self._post(self._RESOURCE_PATH + "/revoke", items).json()["items"])
 
     def list(self, status: Optional[str] = None) -> SessionList:
         """`List all sessions in the current project. <https://docs.cognite.com/api/v1/#operation/listSessions>`_
 
         Args:
             status (Optional[str]): If given, only sessions with the given status are returned.
 
         Returns:
             SessionList: a list of sessions in the current project.
         """
-        filter = {"status": status} if status else None
-        return self._list(list_cls=self._LIST_CLASS, resource_cls=Session, method="GET", filter=filter)
+        filter = {"status": status} if status is not None else None
+        return self._list(list_cls=SessionList, resource_cls=Session, method="GET", filter=filter)
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/labels.py` & `cognite_sdk-6.2.2/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/raw.py` & `cognite_sdk-6.2.2/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/relationships.py` & `cognite_sdk-6.2.2/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/sequences.py` & `cognite_sdk-6.2.2/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/spaces.py` & `cognite_sdk-6.2.2/cognite/client/_api/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.2.2/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/templates.py` & `cognite_sdk-6.2.2/cognite/client/_api/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,14 @@
         """
         resource_path = utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH, external_id)
         self._post(resource_path + "/delete", {"version": version})
 
 
 class TemplateInstancesAPI(APIClient):
     _RESOURCE_PATH = "/templategroups/{}/versions/{}/instances"
-    _LIST_CLASS = TemplateInstanceList
 
     def create(
         self, external_id: str, version: int, instances: Union[TemplateInstance, Sequence[TemplateInstance]]
     ) -> Union[TemplateInstance, TemplateInstanceList]:
         """`Create one or more template instances.`
 
         Args:
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/three_d.py` & `cognite_sdk-6.2.2/cognite/client/_api/three_d.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,15 +564,14 @@
         """
         path = utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH + "/{}", id)
         return self._get(path).content
 
 
 class ThreeDAssetMappingAPI(APIClient):
     _RESOURCE_PATH = "/3d/models/{}/revisions/{}/mappings"
-    _LIST_CLASS = ThreeDAssetMappingList
 
     def list(
         self,
         model_id: int,
         revision_id: int,
         node_id: int = None,
         asset_id: int = None,
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/time_series.py` & `cognite_sdk-6.2.2/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.2.2/cognite/client/_api/transformations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     "TransformationNotificationsAPI",
     "TransformationJobsAPI",
 ]
 
 
 class TransformationsAPI(APIClient):
     _RESOURCE_PATH = "/transformations"
-    _LIST_CLASS = TransformationList
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self.jobs = TransformationJobsAPI(config, api_version, cognite_client)
         self.schedules = TransformationSchedulesAPI(config, api_version, cognite_client)
         self.schema = TransformationSchemaAPI(config, api_version, cognite_client)
         self.notifications = TransformationNotificationsAPI(config, api_version, cognite_client)
@@ -56,15 +55,15 @@
 
         Examples:
 
             Create new transformations:
 
                 >>> from cognite.client import CogniteClient
                 >>> from cognite.client.data_classes import Transformation, TransformationDestination
-                >>> from cognite.client.data_classes.transformations.common import ViewInfo, EdgeType
+                >>> from cognite.client.data_classes.transformations.common import ViewInfo, EdgeType, DataModelInfo
                 >>> c = CogniteClient()
                 >>> transformations = [
                 >>>     Transformation(
                 >>>         name="transformation1",
                 >>>         destination=TransformationDestination.assets()
                 >>>     ),
                 >>>     Transformation(
@@ -82,14 +81,24 @@
                 >>>      destination=TransformationDestination.edges(view, "InstanceSpace")
                 >>>      ),
                 >>>      Transformation(
                 >>>      name="transformation5",
                 >>>      edge_type = EdgeType(space="TypeSpace", external_id="TypeExtId"),
                 >>>      destination=TransformationDestination.edges(edge_type,"InstanceSpace")
                 >>>      ),
+                >>>      Transformation(
+                >>>      name="transformation6",
+                >>>      data_model = DataModelInfo(space="modelSpace", external_id="modelExternalId",version="modelVersion",destination_type="viewExternalId"),
+                >>>      destination=TransformationDestination.instances(data_model,"InstanceSpace")
+                >>>      ),
+                >>>      Transformation(
+                >>>      name="transformation7",
+                >>>      data_model = DataModelInfo(space="modelSpace", external_id="modelExternalId",version="modelVersion",destination_type="viewExternalId", destination_relationship_from_type="connectionPropertyName"),
+                >>>      destination=TransformationDestination.instances(data_model,"InstanceSpace")
+                >>>      ),
                 >>> ]
                 >>> res = c.transformations.create(transformations)
 
         """
         if isinstance(transformation, Sequence):
             sessions: Dict[str, NonceCredentials] = {}
             transformation = [t.copy() for t in transformation]
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.2.2/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.2.2/cognite/client/_api/transformations/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from cognite.client.data_classes import TransformationNotification, TransformationNotificationList
 from cognite.client.data_classes.transformations.notifications import TransformationNotificationFilter
 from cognite.client.utils._identifier import IdentifierSequence
 
 
 class TransformationNotificationsAPI(APIClient):
     _RESOURCE_PATH = "/transformations/notifications"
-    _LIST_CLASS = TransformationNotificationList
 
     def create(
         self, notification: Union[TransformationNotification, Sequence[TransformationNotification]]
     ) -> Union[TransformationNotification, TransformationNotificationList]:
         """`Subscribe for notifications on the transformation errors. <https://docs.cognite.com/api/v1/#operation/createTransformationNotifications>`_
 
         Args:
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.2.2/cognite/client/_api/transformations/schedules.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
     from cognite.client.config import ClientConfig
 
 
 class TransformationSchedulesAPI(APIClient):
     _RESOURCE_PATH = "/transformations/schedules"
-    _LIST_CLASS = TransformationScheduleList
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self._CREATE_LIMIT = 5
         self._DELETE_LIMIT = 5
         self._UPDATE_LIMIT = 5
```

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.2.2/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api/vision.py` & `cognite_sdk-6.2.2/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_api_client.py` & `cognite_sdk-6.2.2/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_cognite_client.py` & `cognite_sdk-6.2.2/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_http_client.py` & `cognite_sdk-6.2.2/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.2.2/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.2.2/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.2.2/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/config.py` & `cognite_sdk-6.2.2/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/credentials.py` & `cognite_sdk-6.2.2/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/_base.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/assets.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/events.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/files.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/functions.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/iam.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/labels.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/raw.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/shared.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/spaces.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/templates.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/exceptions.py` & `cognite_sdk-6.2.2/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/testing.py` & `cognite_sdk-6.2.2/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/__init__.py` & `cognite_sdk-6.2.2/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.2.2/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.2.2/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_graph.py` & `cognite_sdk-6.2.2/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_identifier.py` & `cognite_sdk-6.2.2/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_logging.py` & `cognite_sdk-6.2.2/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.2.2/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.2.2/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.2.2/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_text.py` & `cognite_sdk-6.2.2/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_time.py` & `cognite_sdk-6.2.2/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_validation.py` & `cognite_sdk-6.2.2/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.2.2/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.1/pyproject.toml` & `cognite_sdk-6.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.2.1"
+version = "6.2.2"
 
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.2.1/PKG-INFO` & `cognite_sdk-6.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.2.1
+Version: 6.2.2
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.2.1 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.2.2 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

