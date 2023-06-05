# Comparing `tmp/dapr-1.9.0rc4.tar.gz` & `tmp/dapr-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-1.9.0rc4.tar", last modified: Wed Feb 15 22:45:17 2023, max compression
+gzip compressed data, was "dist/dapr-1.9.1.tar", last modified: Tue Mar 21 16:28:37 2023, max compression
```

## Comparing `dapr-1.9.0rc4.tar` & `dapr-1.9.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/actor_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/actor/client/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/client/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/actor/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/_call_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/_method_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/_reminder_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/_state_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/_timer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/_type_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/method_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/reentrancy_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/remindable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/state_change.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/actor/runtime/state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/clients/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/grpc/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/grpc/_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    28997 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/grpc/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/grpc/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    47859 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/grpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/clients/http/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/http/dapr_actor_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/clients/http/dapr_invocation_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/conf/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/proto/common/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/proto/common/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/common/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/common/v1/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/common/v1/common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/proto/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/proto/runtime/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/runtime/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/runtime/v1/appcallback_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    71113 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/runtime/v1/dapr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    57502 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/proto/runtime/v1/dapr_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/serializers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr/version/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/dapr/version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/dapr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-02-15 22:45:17.000000 dapr-1.9.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-02-15 22:45:07.000000 dapr-1.9.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-03-21 16:28:22.000000 dapr-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-21 16:28:37.000000 dapr-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-03-21 16:28:22.000000 dapr-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/actor_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/actor/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/client/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/actor/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/_call_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/_method_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/_reminder_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/_state_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/_timer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/_type_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/method_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/reentrancy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/remindable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/state_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/actor/runtime/state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/clients/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/grpc/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/grpc/_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28997 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/grpc/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/grpc/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47859 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/grpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/clients/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/http/dapr_actor_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/clients/http/dapr_invocation_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/conf/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/proto/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/proto/common/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/common/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/common/v1/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/common/v1/common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/proto/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/proto/runtime/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/runtime/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/runtime/v1/appcallback_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71113 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/runtime/v1/dapr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57502 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/proto/runtime/v1/dapr_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/serializers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-21 16:28:22.000000 dapr-1.9.1/dapr/version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-21 16:28:36.000000 dapr-1.9.1/dapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-21 16:28:37.000000 dapr-1.9.1/dapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:28:36.000000 dapr-1.9.1/dapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:28:36.000000 dapr-1.9.1/dapr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-21 16:28:36.000000 dapr-1.9.1/dapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-21 16:28:36.000000 dapr-1.9.1/dapr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-21 16:28:37.000000 dapr-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-21 16:28:22.000000 dapr-1.9.1/setup.py
```

### Comparing `dapr-1.9.0rc4/LICENSE` & `dapr-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/PKG-INFO` & `dapr-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr
-Version: 1.9.0rc4
+Version: 1.9.1
 Summary: The official release of Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-1.9.0rc4/README.md` & `dapr-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/__init__.py` & `dapr-1.9.1/dapr/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/actor_interface.py` & `dapr-1.9.1/dapr/actor/actor_interface.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/client/__init__.py` & `dapr-1.9.1/dapr/actor/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/client/proxy.py` & `dapr-1.9.1/dapr/actor/client/proxy.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/id.py` & `dapr-1.9.1/dapr/actor/id.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/__init__.py` & `dapr-1.9.1/dapr/actor/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/_call_type.py` & `dapr-1.9.1/dapr/actor/runtime/_call_type.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/_method_context.py` & `dapr-1.9.1/dapr/actor/runtime/_method_context.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/_reminder_data.py` & `dapr-1.9.1/dapr/actor/runtime/_reminder_data.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/_state_provider.py` & `dapr-1.9.1/dapr/actor/runtime/_state_provider.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/_timer_data.py` & `dapr-1.9.1/dapr/actor/runtime/_timer_data.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/_type_information.py` & `dapr-1.9.1/dapr/actor/runtime/_type_information.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/_type_utils.py` & `dapr-1.9.1/dapr/actor/runtime/_type_utils.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/actor.py` & `dapr-1.9.1/dapr/actor/runtime/actor.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/config.py` & `dapr-1.9.1/dapr/actor/runtime/config.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/context.py` & `dapr-1.9.1/dapr/actor/runtime/context.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/manager.py` & `dapr-1.9.1/dapr/actor/runtime/manager.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/method_dispatcher.py` & `dapr-1.9.1/dapr/actor/runtime/method_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/reentrancy_context.py` & `dapr-1.9.1/dapr/actor/runtime/reentrancy_context.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/remindable.py` & `dapr-1.9.1/dapr/actor/runtime/remindable.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/runtime.py` & `dapr-1.9.1/dapr/actor/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/state_change.py` & `dapr-1.9.1/dapr/actor/runtime/state_change.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/actor/runtime/state_manager.py` & `dapr-1.9.1/dapr/actor/runtime/state_manager.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/__init__.py` & `dapr-1.9.1/dapr/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/base.py` & `dapr-1.9.1/dapr/clients/base.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/exceptions.py` & `dapr-1.9.1/dapr/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/grpc/__init__.py` & `dapr-1.9.1/dapr/clients/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/grpc/_helpers.py` & `dapr-1.9.1/dapr/clients/grpc/_helpers.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/grpc/_request.py` & `dapr-1.9.1/dapr/clients/grpc/_request.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/grpc/_response.py` & `dapr-1.9.1/dapr/clients/grpc/_response.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/grpc/_state.py` & `dapr-1.9.1/dapr/clients/grpc/_state.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/grpc/client.py` & `dapr-1.9.1/dapr/clients/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/http/__init__.py` & `dapr-1.9.1/dapr/clients/http/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/http/client.py` & `dapr-1.9.1/dapr/clients/http/client.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/http/dapr_actor_http_client.py` & `dapr-1.9.1/dapr/clients/http/dapr_actor_http_client.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/clients/http/dapr_invocation_http_client.py` & `dapr-1.9.1/dapr/clients/http/dapr_invocation_http_client.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/conf/__init__.py` & `dapr-1.9.1/dapr/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/conf/global_settings.py` & `dapr-1.9.1/dapr/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/__init__.py` & `dapr-1.9.1/dapr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/common/__init__.py` & `dapr-1.9.1/dapr/proto/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/common/v1/__init__.py` & `dapr-1.9.1/dapr/proto/common/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/common/v1/common_pb2.py` & `dapr-1.9.1/dapr/proto/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/runtime/__init__.py` & `dapr-1.9.1/dapr/proto/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/runtime/v1/__init__.py` & `dapr-1.9.1/dapr/proto/runtime/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/runtime/v1/appcallback_pb2.py` & `dapr-1.9.1/dapr/proto/runtime/v1/appcallback_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/runtime/v1/appcallback_pb2_grpc.py` & `dapr-1.9.1/dapr/proto/runtime/v1/appcallback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/runtime/v1/dapr_pb2.py` & `dapr-1.9.1/dapr/proto/runtime/v1/dapr_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/proto/runtime/v1/dapr_pb2_grpc.py` & `dapr-1.9.1/dapr/proto/runtime/v1/dapr_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/serializers/__init__.py` & `dapr-1.9.1/dapr/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/serializers/base.py` & `dapr-1.9.1/dapr/serializers/base.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/serializers/json.py` & `dapr-1.9.1/dapr/serializers/json.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/serializers/util.py` & `dapr-1.9.1/dapr/serializers/util.py`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/dapr/version/version.py` & `dapr-1.9.1/dapr/version/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__version__ = "1.9.0rc4"
+__version__ = "1.9.1"
```

### Comparing `dapr-1.9.0rc4/dapr.egg-info/PKG-INFO` & `dapr-1.9.1/dapr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr
-Version: 1.9.0rc4
+Version: 1.9.1
 Summary: The official release of Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-1.9.0rc4/dapr.egg-info/SOURCES.txt` & `dapr-1.9.1/dapr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dapr-1.9.0rc4/setup.cfg` & `dapr-1.9.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 include_package_data = True
 zip_safe = False
 install_requires = 
 	protobuf >= 3.17.3, < 4.22
 	grpcio >= 1.37.0
 	aiohttp >= 3.6.2
 	python-dateutil >= 2.8.1
+	typing-extensions>=4.4.0
 
 [options.packages.find]
 include = 
 	dapr
 	dapr.*
 exclude = 
 	ext
```

### Comparing `dapr-1.9.0rc4/setup.py` & `dapr-1.9.1/setup.py`

 * *Files identical despite different names*

