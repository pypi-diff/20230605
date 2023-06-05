# Comparing `tmp/momento-1.5.1.tar.gz` & `tmp/momento-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento-1.5.1.tar", max compression
+gzip compressed data, was "momento-1.5.2.tar", max compression
```

## Comparing `momento-1.5.1.tar` & `momento-1.5.2.tar`

### file list

```diff
@@ -1,105 +1,106 @@
--rw-r--r--   0        0        0    11357 2023-06-01 19:37:54.047194 momento-1.5.1/LICENSE
--rw-r--r--   0        0        0     4142 2023-06-01 19:37:54.047194 momento-1.5.1/README.md
--rw-r--r--   0        0        0     3778 2023-06-01 19:38:09.799399 momento-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      619 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/__init__.py
--rw-r--r--   0        0        0       86 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/auth/__init__.py
--rw-r--r--   0        0        0     2868 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/auth/credential_provider.py
--rw-r--r--   0        0        0     2003 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/auth/momento_endpoint_resolver.py
--rw-r--r--   0        0        0    43756 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/cache_client.py
--rw-r--r--   0        0        0    44407 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/cache_client_async.py
--rw-r--r--   0        0        0      176 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/config/__init__.py
--rw-r--r--   0        0        0     3250 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/config/configuration.py
--rw-r--r--   0        0        0     4290 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/config/configurations.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/config/transport/__init__.py
--rw-r--r--   0        0        0      314 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/config/transport/grpc_configuration.py
--rw-r--r--   0        0        0     2358 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/config/transport/transport_strategy.py
--rw-r--r--   0        0        0     1503 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/errors/__init__.py
--rw-r--r--   0        0        0     3991 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/errors/error_converter.py
--rw-r--r--   0        0        0     2329 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/errors/error_details.py
--rw-r--r--   0        0        0     8799 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/errors/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/__init__.py
--rw-r--r--   0        0        0      360 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/_utilities/__init__.py
--rw-r--r--   0        0        0     4735 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/_utilities/_data_validation.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/aio/__init__.py
--rw-r--r--   0        0        0     4377 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/aio/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1856 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/aio/_retry_interceptor.py
--rw-r--r--   0        0        0     5794 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/aio/_scs_control_client.py
--rw-r--r--   0        0        0    47746 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/aio/_scs_data_client.py
--rw-r--r--   0        0        0     3332 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/aio/_scs_grpc_manager.py
--rw-r--r--   0        0        0      123 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/aio/_utilities.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/synchronous/__init__.py
--rw-r--r--   0        0        0     3714 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/synchronous/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1829 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/synchronous/_retry_interceptor.py
--rw-r--r--   0        0        0     5700 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/synchronous/_scs_control_client.py
--rw-r--r--   0        0        0    47366 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/synchronous/_scs_data_client.py
--rw-r--r--   0        0        0     2562 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/synchronous/_scs_grpc_manager.py
--rw-r--r--   0        0        0      159 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/internal/synchronous/_utilities.py
--rw-r--r--   0        0        0     2790 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/logs.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/py.typed
--rw-r--r--   0        0        0      154 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/requests/__init__.py
--rw-r--r--   0        0        0     3800 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/requests/collection_ttl.py
--rw-r--r--   0        0        0       91 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/requests/sort_order.py
--rw-r--r--   0        0        0     6841 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/cache/__init__.py
--rw-r--r--   0        0        0     1758 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/cache/create.py
--rw-r--r--   0        0        0     1405 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/cache/delete.py
--rw-r--r--   0        0        0      849 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/cache/flush.py
--rw-r--r--   0        0        0     2275 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/cache/list.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/signing_key/__init__.py
--rw-r--r--   0        0        0     1764 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/signing_key/create.py
--rw-r--r--   0        0        0     2479 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/signing_key/list.py
--rw-r--r--   0        0        0      979 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/control/signing_key/revoke.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/dictionary/__init__.py
--rw-r--r--   0        0        0     2047 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/dictionary/fetch.py
--rw-r--r--   0        0        0     1678 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/dictionary/get_field.py
--rw-r--r--   0        0        0     3320 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/dictionary/get_fields.py
--rw-r--r--   0        0        0     1050 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/dictionary/increment.py
--rw-r--r--   0        0        0      945 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/dictionary/remove_field.py
--rw-r--r--   0        0        0      953 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/dictionary/remove_fields.py
--rw-r--r--   0        0        0      921 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/dictionary/set_field.py
--rw-r--r--   0        0        0      929 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/dictionary/set_fields.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/__init__.py
--rw-r--r--   0        0        0     1052 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/concatenate_back.py
--rw-r--r--   0        0        0     1060 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/concatenate_front.py
--rw-r--r--   0        0        0     1402 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/fetch.py
--rw-r--r--   0        0        0     1070 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/length.py
--rw-r--r--   0        0        0     1189 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/pop_back.py
--rw-r--r--   0        0        0     1199 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/pop_front.py
--rw-r--r--   0        0        0      977 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/push_back.py
--rw-r--r--   0        0        0      985 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/push_front.py
--rw-r--r--   0        0        0      874 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/list/remove_value.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/scalar/__init__.py
--rw-r--r--   0        0        0      823 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/scalar/delete.py
--rw-r--r--   0        0        0     1155 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/scalar/get.py
--rw-r--r--   0        0        0     1141 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/scalar/increment.py
--rw-r--r--   0        0        0      799 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/scalar/set.py
--rw-r--r--   0        0        0     1056 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/scalar/set_if_not_exists.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/set/__init__.py
--rw-r--r--   0        0        0      870 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/set/add_element.py
--rw-r--r--   0        0        0      880 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/set/add_elements.py
--rw-r--r--   0        0        0     1452 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/set/fetch.py
--rw-r--r--   0        0        0      896 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/set/remove_element.py
--rw-r--r--   0        0        0      906 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/set/remove_elements.py
--rw-r--r--   0        0        0        0 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/fetch.py
--rw-r--r--   0        0        0     1205 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/get_rank.py
--rw-r--r--   0        0        0     1581 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/get_score.py
--rw-r--r--   0        0        0     2323 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/get_scores.py
--rw-r--r--   0        0        0     1046 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/increment.py
--rw-r--r--   0        0        0      944 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/put_element.py
--rw-r--r--   0        0        0      952 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/put_elements.py
--rw-r--r--   0        0        0      971 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/remove_element.py
--rw-r--r--   0        0        0      979 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/data/sorted_set/remove_elements.py
--rw-r--r--   0        0        0     1460 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/mixins.py
--rw-r--r--   0        0        0     4724 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/responses/response.py
--rw-r--r--   0        0        0      423 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/retry/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/retry/default_eligibility_strategy.py
--rw-r--r--   0        0        0      216 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/retry/eligibility_strategy.py
--rw-r--r--   0        0        0     2181 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/retry/fixed_count_retry_strategy.py
--rw-r--r--   0        0        0      251 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/retry/retry_strategy.py
--rw-r--r--   0        0        0      291 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/retry/retryable_props.py
--rw-r--r--   0        0        0     1722 2023-06-01 19:37:54.051194 momento-1.5.1/src/momento/typing.py
--rw-r--r--   0        0        0     5563 1970-01-01 00:00:00.000000 momento-1.5.1/setup.py
--rw-r--r--   0        0        0     5415 1970-01-01 00:00:00.000000 momento-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-05 16:42:27.604468 momento-1.5.2/LICENSE
+-rw-r--r--   0        0        0     4142 2023-06-05 16:42:27.604468 momento-1.5.2/README.md
+-rw-r--r--   0        0        0     3805 2023-06-05 16:42:51.981947 momento-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      619 2023-06-05 16:42:27.604468 momento-1.5.2/src/momento/__init__.py
+-rw-r--r--   0        0        0       86 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/auth/__init__.py
+-rw-r--r--   0        0        0     2868 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/auth/credential_provider.py
+-rw-r--r--   0        0        0     2003 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/auth/momento_endpoint_resolver.py
+-rw-r--r--   0        0        0    43756 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/cache_client.py
+-rw-r--r--   0        0        0    44407 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/cache_client_async.py
+-rw-r--r--   0        0        0      176 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/__init__.py
+-rw-r--r--   0        0        0     3250 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/configuration.py
+-rw-r--r--   0        0        0     4290 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/configurations.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/transport/__init__.py
+-rw-r--r--   0        0        0      314 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/transport/grpc_configuration.py
+-rw-r--r--   0        0        0     2358 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/transport/transport_strategy.py
+-rw-r--r--   0        0        0     1503 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/errors/__init__.py
+-rw-r--r--   0        0        0     3991 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/errors/error_converter.py
+-rw-r--r--   0        0        0     2329 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/errors/error_details.py
+-rw-r--r--   0        0        0     8799 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/errors/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/_utilities/__init__.py
+-rw-r--r--   0        0        0     4735 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/_utilities/_data_validation.py
+-rw-r--r--   0        0        0      531 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/_utilities/_momento_version.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/__init__.py
+-rw-r--r--   0        0        0     4377 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1856 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_retry_interceptor.py
+-rw-r--r--   0        0        0     5794 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_scs_control_client.py
+-rw-r--r--   0        0        0    47746 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_scs_data_client.py
+-rw-r--r--   0        0        0     3206 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      123 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_utilities.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/__init__.py
+-rw-r--r--   0        0        0     3714 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1829 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_retry_interceptor.py
+-rw-r--r--   0        0        0     5700 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_scs_control_client.py
+-rw-r--r--   0        0        0    47366 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_scs_data_client.py
+-rw-r--r--   0        0        0     2436 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      159 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_utilities.py
+-rw-r--r--   0        0        0     2790 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/logs.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/py.typed
+-rw-r--r--   0        0        0      154 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/requests/__init__.py
+-rw-r--r--   0        0        0     3800 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/requests/collection_ttl.py
+-rw-r--r--   0        0        0       91 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/requests/sort_order.py
+-rw-r--r--   0        0        0     6841 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/__init__.py
+-rw-r--r--   0        0        0     1758 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/create.py
+-rw-r--r--   0        0        0     1405 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/delete.py
+-rw-r--r--   0        0        0      849 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/flush.py
+-rw-r--r--   0        0        0     2275 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/list.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/signing_key/__init__.py
+-rw-r--r--   0        0        0     1764 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/signing_key/create.py
+-rw-r--r--   0        0        0     2479 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/signing_key/list.py
+-rw-r--r--   0        0        0      979 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/signing_key/revoke.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/__init__.py
+-rw-r--r--   0        0        0     2047 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/fetch.py
+-rw-r--r--   0        0        0     1678 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/get_field.py
+-rw-r--r--   0        0        0     3320 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/get_fields.py
+-rw-r--r--   0        0        0     1050 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/increment.py
+-rw-r--r--   0        0        0      945 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/remove_field.py
+-rw-r--r--   0        0        0      953 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/remove_fields.py
+-rw-r--r--   0        0        0      921 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/set_field.py
+-rw-r--r--   0        0        0      929 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/set_fields.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/__init__.py
+-rw-r--r--   0        0        0     1052 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/concatenate_back.py
+-rw-r--r--   0        0        0     1060 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/concatenate_front.py
+-rw-r--r--   0        0        0     1402 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/fetch.py
+-rw-r--r--   0        0        0     1070 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/length.py
+-rw-r--r--   0        0        0     1189 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/pop_back.py
+-rw-r--r--   0        0        0     1199 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/pop_front.py
+-rw-r--r--   0        0        0      977 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/push_back.py
+-rw-r--r--   0        0        0      985 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/push_front.py
+-rw-r--r--   0        0        0      874 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/remove_value.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/delete.py
+-rw-r--r--   0        0        0     1155 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/get.py
+-rw-r--r--   0        0        0     1141 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/increment.py
+-rw-r--r--   0        0        0      799 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/set.py
+-rw-r--r--   0        0        0     1056 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/set_if_not_exists.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/__init__.py
+-rw-r--r--   0        0        0      870 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/add_element.py
+-rw-r--r--   0        0        0      880 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/add_elements.py
+-rw-r--r--   0        0        0     1452 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/fetch.py
+-rw-r--r--   0        0        0      896 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/remove_element.py
+-rw-r--r--   0        0        0      906 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/remove_elements.py
+-rw-r--r--   0        0        0        0 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/fetch.py
+-rw-r--r--   0        0        0     1205 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/get_rank.py
+-rw-r--r--   0        0        0     1581 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/get_score.py
+-rw-r--r--   0        0        0     2323 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/get_scores.py
+-rw-r--r--   0        0        0     1046 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/increment.py
+-rw-r--r--   0        0        0      944 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/put_element.py
+-rw-r--r--   0        0        0      952 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/put_elements.py
+-rw-r--r--   0        0        0      971 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/remove_element.py
+-rw-r--r--   0        0        0      979 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/remove_elements.py
+-rw-r--r--   0        0        0     1460 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/mixins.py
+-rw-r--r--   0        0        0     4724 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/response.py
+-rw-r--r--   0        0        0      423 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/default_eligibility_strategy.py
+-rw-r--r--   0        0        0      216 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/eligibility_strategy.py
+-rw-r--r--   0        0        0     2181 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/fixed_count_retry_strategy.py
+-rw-r--r--   0        0        0      251 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/retry_strategy.py
+-rw-r--r--   0        0        0      291 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/retryable_props.py
+-rw-r--r--   0        0        0     1722 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/typing.py
+-rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 momento-1.5.2/setup.py
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 momento-1.5.2/PKG-INFO
```

### Comparing `momento-1.5.1/LICENSE` & `momento-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/README.md` & `momento-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/pyproject.toml` & `momento-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momento"
-version = "1.5.1"
+version = "1.5.2"
 
 authors = ["Momento <hello@momentohq.com>"]
 description = "SDK for Momento"
 
 license = "Apache-2.0"
 
 documentation = "https://docs.momentohq.com/"
@@ -31,15 +31,15 @@
 python = "^3.7"
 
 momento-wire-types = "^0.64"
 grpcio = "^1.46.0"
 # note if you bump this presigned url test need be updated
 pyjwt = "^2.4.0"
 # Need a lower bound of 4 to be compatible with python 3.7 flake8
-importlib-metadata = ">=4"
+importlib-metadata = { version=">=4", python="<3.8" }
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
 pytest-asyncio = "^0.19.0"
 pytest-describe = "^2.0.1"
 pytest-sugar = "^0.9.5"
```

### Comparing `momento-1.5.1/src/momento/__init__.py` & `momento-1.5.2/src/momento/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/auth/credential_provider.py` & `momento-1.5.2/src/momento/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/auth/momento_endpoint_resolver.py` & `momento-1.5.2/src/momento/auth/momento_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/cache_client.py` & `momento-1.5.2/src/momento/cache_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/cache_client_async.py` & `momento-1.5.2/src/momento/cache_client_async.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/config/configuration.py` & `momento-1.5.2/src/momento/config/configuration.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/config/configurations.py` & `momento-1.5.2/src/momento/config/configurations.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/config/transport/transport_strategy.py` & `momento-1.5.2/src/momento/config/transport/transport_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/errors/__init__.py` & `momento-1.5.2/src/momento/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/errors/error_converter.py` & `momento-1.5.2/src/momento/errors/error_converter.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/errors/error_details.py` & `momento-1.5.2/src/momento/errors/error_details.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/errors/exceptions.py` & `momento-1.5.2/src/momento/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/_utilities/_data_validation.py` & `momento-1.5.2/src/momento/internal/_utilities/_data_validation.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/aio/_add_header_client_interceptor.py` & `momento-1.5.2/src/momento/internal/aio/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/aio/_retry_interceptor.py` & `momento-1.5.2/src/momento/internal/aio/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/aio/_scs_control_client.py` & `momento-1.5.2/src/momento/internal/aio/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/aio/_scs_data_client.py` & `momento-1.5.2/src/momento/internal/aio/_scs_data_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/aio/_scs_grpc_manager.py` & `momento-1.5.2/src/momento/internal/aio/_scs_grpc_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import grpc
-import importlib_metadata
 from momento_wire_types import cacheclient_pb2_grpc as cache_client
 from momento_wire_types import controlclient_pb2_grpc as control_client
 
 from momento.auth import CredentialProvider
 from momento.config import Configuration
+from momento.internal._utilities import momento_version
 from momento.retry import RetryStrategy
 
 from ._add_header_client_interceptor import AddHeaderClientInterceptor, Header
 from ._retry_interceptor import RetryInterceptor
 
 
 class _ControlGrpcManager:
     """Internal gRPC control mananger."""
 
-    version = importlib_metadata.Distribution.from_name("momento").version  # type: ignore[no-untyped-call]
+    version = momento_version
 
     def __init__(self, configuration: Configuration, credential_provider: CredentialProvider):
         self._secure_channel = grpc.aio.secure_channel(
             target=credential_provider.control_endpoint,
             credentials=grpc.ssl_channel_credentials(),
             interceptors=_interceptors(credential_provider.auth_token, configuration.get_retry_strategy()),
         )
@@ -31,15 +31,15 @@
     def async_stub(self) -> control_client.ScsControlStub:
         return control_client.ScsControlStub(self._secure_channel)  # type: ignore[no-untyped-call]
 
 
 class _DataGrpcManager:
     """Internal gRPC data mananger."""
 
-    version = importlib_metadata.Distribution.from_name("momento").version  # type: ignore[no-untyped-call]
+    version = momento_version
 
     def __init__(self, configuration: Configuration, credential_provider: CredentialProvider):
         self._secure_channel = grpc.aio.secure_channel(
             target=credential_provider.cache_endpoint,
             credentials=grpc.ssl_channel_credentials(),
             interceptors=_interceptors(credential_provider.auth_token, configuration.get_retry_strategy()),
             # Here is where you would pass override configuration to the underlying C gRPC layer.
```

### Comparing `momento-1.5.1/src/momento/internal/synchronous/_add_header_client_interceptor.py` & `momento-1.5.2/src/momento/internal/synchronous/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/synchronous/_retry_interceptor.py` & `momento-1.5.2/src/momento/internal/synchronous/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/synchronous/_scs_control_client.py` & `momento-1.5.2/src/momento/internal/synchronous/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/synchronous/_scs_data_client.py` & `momento-1.5.2/src/momento/internal/synchronous/_scs_data_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/internal/synchronous/_scs_grpc_manager.py` & `momento-1.5.2/src/momento/internal/synchronous/_scs_grpc_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import grpc
-import importlib_metadata
 from momento_wire_types import cacheclient_pb2_grpc as cache_client
 from momento_wire_types import controlclient_pb2_grpc as control_client
 
 from momento.auth import CredentialProvider
 from momento.config import Configuration
+from momento.internal._utilities import momento_version
 from momento.internal.synchronous._add_header_client_interceptor import (
     AddHeaderClientInterceptor,
     Header,
 )
 from momento.internal.synchronous._retry_interceptor import RetryInterceptor
 from momento.retry import RetryStrategy
 
 
 class _ControlGrpcManager:
     """Internal gRPC control mananger."""
 
-    version = importlib_metadata.Distribution.from_name("momento").version  # type: ignore[no-untyped-call]
+    version = momento_version
 
     def __init__(self, configuration: Configuration, credential_provider: CredentialProvider):
         self._secure_channel = grpc.secure_channel(
             target=credential_provider.control_endpoint, credentials=grpc.ssl_channel_credentials()
         )
         intercept_channel = grpc.intercept_channel(
             self._secure_channel, *_interceptors(credential_provider.auth_token, configuration.get_retry_strategy())
@@ -35,15 +35,15 @@
     def stub(self) -> control_client.ScsControlStub:
         return self._stub
 
 
 class _DataGrpcManager:
     """Internal gRPC data mananger."""
 
-    version = importlib_metadata.Distribution.from_name("momento").version  # type: ignore[no-untyped-call]
+    version = momento_version
 
     def __init__(self, configuration: Configuration, credential_provider: CredentialProvider):
         self._secure_channel = grpc.secure_channel(
             target=credential_provider.cache_endpoint,
             credentials=grpc.ssl_channel_credentials(),
         )
         intercept_channel = grpc.intercept_channel(
```

### Comparing `momento-1.5.1/src/momento/logs.py` & `momento-1.5.2/src/momento/logs.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/requests/collection_ttl.py` & `momento-1.5.2/src/momento/requests/collection_ttl.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/__init__.py` & `momento-1.5.2/src/momento/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/control/cache/create.py` & `momento-1.5.2/src/momento/responses/control/cache/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/control/cache/delete.py` & `momento-1.5.2/src/momento/responses/control/cache/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/control/cache/flush.py` & `momento-1.5.2/src/momento/responses/control/cache/flush.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/control/cache/list.py` & `momento-1.5.2/src/momento/responses/control/cache/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/control/signing_key/create.py` & `momento-1.5.2/src/momento/responses/control/signing_key/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/control/signing_key/list.py` & `momento-1.5.2/src/momento/responses/control/signing_key/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/control/signing_key/revoke.py` & `momento-1.5.2/src/momento/responses/control/signing_key/revoke.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/dictionary/fetch.py` & `momento-1.5.2/src/momento/responses/data/dictionary/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/dictionary/get_field.py` & `momento-1.5.2/src/momento/responses/data/dictionary/get_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/dictionary/get_fields.py` & `momento-1.5.2/src/momento/responses/data/dictionary/get_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/dictionary/increment.py` & `momento-1.5.2/src/momento/responses/data/dictionary/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/dictionary/remove_field.py` & `momento-1.5.2/src/momento/responses/data/dictionary/remove_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/dictionary/remove_fields.py` & `momento-1.5.2/src/momento/responses/data/dictionary/remove_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/dictionary/set_field.py` & `momento-1.5.2/src/momento/responses/data/dictionary/set_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/dictionary/set_fields.py` & `momento-1.5.2/src/momento/responses/data/dictionary/set_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/list/concatenate_back.py` & `momento-1.5.2/src/momento/responses/data/list/concatenate_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/list/concatenate_front.py` & `momento-1.5.2/src/momento/responses/data/list/concatenate_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/list/fetch.py` & `momento-1.5.2/src/momento/responses/data/list/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/list/length.py` & `momento-1.5.2/src/momento/responses/data/list/length.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/list/pop_back.py` & `momento-1.5.2/src/momento/responses/data/list/pop_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/list/pop_front.py` & `momento-1.5.2/src/momento/responses/data/list/pop_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/list/push_back.py` & `momento-1.5.2/src/momento/responses/data/list/push_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/list/push_front.py` & `momento-1.5.2/src/momento/responses/data/list/push_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/list/remove_value.py` & `momento-1.5.2/src/momento/responses/data/list/remove_value.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/scalar/delete.py` & `momento-1.5.2/src/momento/responses/data/scalar/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/scalar/get.py` & `momento-1.5.2/src/momento/responses/data/scalar/get.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/scalar/increment.py` & `momento-1.5.2/src/momento/responses/data/scalar/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/scalar/set.py` & `momento-1.5.2/src/momento/responses/data/scalar/set.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/scalar/set_if_not_exists.py` & `momento-1.5.2/src/momento/responses/data/scalar/set_if_not_exists.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/set/add_element.py` & `momento-1.5.2/src/momento/responses/data/set/add_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/set/add_elements.py` & `momento-1.5.2/src/momento/responses/data/set/add_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/set/fetch.py` & `momento-1.5.2/src/momento/responses/data/set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/set/remove_element.py` & `momento-1.5.2/src/momento/responses/data/set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/set/remove_elements.py` & `momento-1.5.2/src/momento/responses/data/set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/sorted_set/fetch.py` & `momento-1.5.2/src/momento/responses/data/sorted_set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/sorted_set/get_rank.py` & `momento-1.5.2/src/momento/responses/data/sorted_set/get_rank.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/sorted_set/get_score.py` & `momento-1.5.2/src/momento/responses/data/sorted_set/get_score.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/sorted_set/get_scores.py` & `momento-1.5.2/src/momento/responses/data/sorted_set/get_scores.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/sorted_set/increment.py` & `momento-1.5.2/src/momento/responses/data/sorted_set/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/sorted_set/put_element.py` & `momento-1.5.2/src/momento/responses/data/sorted_set/put_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/sorted_set/put_elements.py` & `momento-1.5.2/src/momento/responses/data/sorted_set/put_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/sorted_set/remove_element.py` & `momento-1.5.2/src/momento/responses/data/sorted_set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/data/sorted_set/remove_elements.py` & `momento-1.5.2/src/momento/responses/data/sorted_set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/mixins.py` & `momento-1.5.2/src/momento/responses/mixins.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/responses/response.py` & `momento-1.5.2/src/momento/responses/response.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/retry/default_eligibility_strategy.py` & `momento-1.5.2/src/momento/retry/default_eligibility_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/retry/fixed_count_retry_strategy.py` & `momento-1.5.2/src/momento/retry/fixed_count_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/src/momento/typing.py` & `momento-1.5.2/src/momento/typing.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.1/setup.py` & `momento-1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,33 @@
  'momento.retry']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['grpcio>=1.46.0,<2.0.0',
- 'importlib-metadata>=4',
  'momento-wire-types>=0.64,<0.65',
  'pyjwt>=2.4.0,<3.0.0']
 
+extras_require = \
+{':python_version < "3.8"': ['importlib-metadata>=4']}
+
 setup_kwargs = {
     'name': 'momento',
-    'version': '1.5.1',
+    'version': '1.5.2',
     'description': 'SDK for Momento',
     'long_description': '<head>\n  <meta name="Momento Python Client Library Documentation" content="Python client software development kit for Momento Cache">\n</head>\n<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n\n# Momento Python Client Library\n\nMomento Cache is a fast, simple, pay-as-you-go caching solution without any of the operational overhead\nrequired by traditional caching solutions.  This repo contains the source code for the Momento Python client library.\n\n* Website: [https://www.gomomento.com/](https://www.gomomento.com/)\n* Momento Documentation: [https://docs.momentohq.com/](https://docs.momentohq.com/)\n* Getting Started: [https://docs.momentohq.com/getting-started](https://docs.momentohq.com/getting-started)\n* Python SDK Documentation: [https://docs.momentohq.com/develop/sdks/python](https://docs.momentohq.com/develop/sdks/python)\n* Discuss: [Momento Discord](https://discord.gg/3HkAKjUZGq)\n\n## Packages\n\nThe Momento Python SDK package is available on pypi: [momento](https://pypi.org/project/momento/).\n\n## Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache, ListCaches\n\ncache_client = CacheClient(\n    Configurations.Laptop.v1(),\n    CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n    timedelta(seconds=60)\n)\n\ncreate_cache_response = cache_client.create_cache("cache")\nset_response = cache_client.set("cache", "my-key", "my-value")\nget_response = cache_client.get(_CACHE_NAME, _KEY)\nmatch get_response:\n    case CacheGet.Hit() as hit:\n        print(f"Got value: {hit.value_string}")\n    case _:\n        print(f"Response was not a hit: {get_response}")\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\ncache_client = CacheClient(\n    configuration=Configurations.Laptop.v1(),\n    credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n    default_ttl=timedelta(seconds=60)\n)\ncache_client.create_cache("cache")\ncache_client.set("cache", "myKey", "myValue")\nget_response = cache_client.get("cache", "myKey")\nif isinstance(get_response, CacheGet.Hit):\n    print(f"Got value: {get_response.value_string}")\n\n```\n\n## Getting Started and Documentation\n\nDocumentation is available on the [Momento Docs website](https://docs.momentohq.com).\n\n## Examples\n\nWorking example projects, with all required build configuration files, are available for both Python 3.10 and up\nand Python versions before 3.10:\n\n* [Python 3.10+ examples](./examples/py310)\n* [Pre-3.10 Python examples](./examples/prepy310)\n\n## Developing\n\nIf you are interested in contributing to the SDK, please see the [CONTRIBUTING](./CONTRIBUTING.md) docs.\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
     'author': 'Momento',
     'author_email': 'hello@momentohq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gomomento.com',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `momento-1.5.1/PKG-INFO` & `momento-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momento
-Version: 1.5.1
+Version: 1.5.2
 Summary: SDK for Momento
 Home-page: https://gomomento.com
 License: Apache-2.0
 Keywords: Momento,caching,key-value store,serverless
 Author: Momento
 Author-email: hello@momentohq.com
 Requires-Python: >=3.7,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Typing :: Typed
 Requires-Dist: grpcio (>=1.46.0,<2.0.0)
-Requires-Dist: importlib-metadata (>=4)
+Requires-Dist: importlib-metadata (>=4) ; python_version < "3.8"
 Requires-Dist: momento-wire-types (>=0.64,<0.65)
 Requires-Dist: pyjwt (>=2.4.0,<3.0.0)
 Project-URL: Documentation, https://docs.momentohq.com/
 Project-URL: Repository, https://github.com/momentohq/client-sdk-python
 Description-Content-Type: text/markdown
 
 <head>
```

