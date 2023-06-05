# Comparing `tmp/voltha-protos-5.4.5.tar.gz` & `tmp/voltha-protos-5.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/voltha-protos-5.4.5.tar", last modified: Thu Jun  1 14:32:10 2023, max compression
+gzip compressed data, was "dist/voltha-protos-5.4.6.tar", last modified: Mon Jun  5 07:06:37 2023, max compression
```

## Comparing `voltha-protos-5.4.5.tar` & `voltha-protos-5.4.6.tar`

### file list

```diff
@@ -1,65 +1,69 @@
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/PKG-INFO
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     3151 2023-06-01 14:31:34.000000 voltha-protos-5.4.5/README.md
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1663 2023-06-01 14:31:34.000000 voltha-protos-5.4.5/setup.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       38 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/setup.cfg
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)       17 2023-06-01 14:31:34.000000 voltha-protos-5.4.5/MANIFEST.in
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/python/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/python/voltha_protos/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/ietf_interfaces_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19060 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/omci_alarm_db_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25293 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/inter_adapter_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    64403 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/events_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19758 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/ext_config_pb2.py
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-06-01 14:31:34.000000 voltha-protos-5.4.5/python/voltha_protos/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    59478 2023-06-01 14:31:59.000000 voltha-protos-5.4.5/python/voltha_protos/adapter_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13326 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/logical_device_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/core_adapter_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    48518 2023-06-01 14:32:03.000000 voltha-protos-5.4.5/python/voltha_protos/voltha_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/device_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   108159 2023-06-01 14:32:03.000000 voltha-protos-5.4.5/python/voltha_protos/voltha_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/omci_test_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4572 2023-06-01 14:31:59.000000 voltha-protos-5.4.5/python/voltha_protos/core_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/omci_mib_db_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4295 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/extensions_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16809 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/ietf_interfaces_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5050 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/omci_test_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/logical_device_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5344 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/onu_inter_adapter_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:31:59.000000 voltha-protos-5.4.5/python/voltha_protos/common_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:31:59.000000 voltha-protos-5.4.5/python/voltha_protos/adapter_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   421230 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/openflow_13_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   106603 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/device_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/ext_config_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    49438 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/core_adapter_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/inter_adapter_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40916 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/core_services_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4707 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/health_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    96862 2023-06-01 14:32:03.000000 voltha-protos-5.4.5/python/voltha_protos/tech_profile_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4435 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/olt_inter_adapter_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:31:59.000000 voltha-protos-5.4.5/python/voltha_protos/core_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/events_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16961 2023-06-01 14:31:59.000000 voltha-protos-5.4.5/python/voltha_protos/common_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19653 2023-06-01 14:31:59.000000 voltha-protos-5.4.5/python/voltha_protos/adapter_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13096 2023-06-01 14:32:00.000000 voltha-protos-5.4.5/python/voltha_protos/core_services_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/openflow_13_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8405 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9978 2023-06-01 14:31:59.000000 voltha-protos-5.4.5/python/voltha_protos/adapter_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   162370 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/extensions_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    52525 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/openolt_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2588 2023-06-01 14:32:01.000000 voltha-protos-5.4.5/python/voltha_protos/health_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18434 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/omci_mib_db_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11674 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   247532 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/openolt_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:03.000000 voltha-protos-5.4.5/python/voltha_protos/tech_profile_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-01 14:32:02.000000 voltha-protos-5.4.5/python/voltha_protos/omci_alarm_db_pb2_grpc.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/python/test/
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-06-01 14:31:34.000000 voltha-protos-5.4.5/python/test/__init__.py
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1007 2023-06-01 14:31:34.000000 voltha-protos-5.4.5/python/test/test_protos.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/python/voltha_protos.egg-info/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/python/voltha_protos.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/python/voltha_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2302 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/python/voltha_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       86 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/python/voltha_protos.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       19 2023-06-01 14:32:10.000000 voltha-protos-5.4.5/python/voltha_protos.egg-info/top_level.txt
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        6 2023-06-01 14:31:34.000000 voltha-protos-5.4.5/VERSION
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/PKG-INFO
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     3151 2023-06-05 07:06:03.000000 voltha-protos-5.4.6/README.md
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1663 2023-06-05 07:06:03.000000 voltha-protos-5.4.6/setup.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       38 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/setup.cfg
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)       17 2023-06-05 07:06:03.000000 voltha-protos-5.4.6/MANIFEST.in
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/python/
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/python/voltha_protos/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/ietf_interfaces_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19060 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/omci_alarm_db_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25293 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/inter_adapter_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    64403 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/events_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19758 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/ext_config_pb2.py
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-06-05 07:06:03.000000 voltha-protos-5.4.6/python/voltha_protos/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    59478 2023-06-05 07:06:26.000000 voltha-protos-5.4.6/python/voltha_protos/adapter_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13326 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/logical_device_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/core_adapter_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    51324 2023-06-05 07:06:30.000000 voltha-protos-5.4.6/python/voltha_protos/voltha_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/device_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   115088 2023-06-05 07:06:30.000000 voltha-protos-5.4.6/python/voltha_protos/voltha_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/omci_test_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4572 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/core_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/omci_mib_db_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4295 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/extensions_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16809 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/ietf_interfaces_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5050 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/omci_test_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/logical_device_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5344 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/onu_inter_adapter_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:26.000000 voltha-protos-5.4.6/python/voltha_protos/common_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:26.000000 voltha-protos-5.4.6/python/voltha_protos/adapter_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   421230 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/openflow_13_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:30.000000 voltha-protos-5.4.6/python/voltha_protos/voip_system_profile_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   106603 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/device_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/ext_config_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    49438 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/core_adapter_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/inter_adapter_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    76610 2023-06-05 07:06:30.000000 voltha-protos-5.4.6/python/voltha_protos/voip_system_profile_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:30.000000 voltha-protos-5.4.6/python/voltha_protos/voip_user_profile_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40916 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/core_services_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4707 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/health_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    96862 2023-06-05 07:06:30.000000 voltha-protos-5.4.6/python/voltha_protos/tech_profile_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4435 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/olt_inter_adapter_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/core_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/events_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18104 2023-06-05 07:06:26.000000 voltha-protos-5.4.6/python/voltha_protos/common_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19653 2023-06-05 07:06:26.000000 voltha-protos-5.4.6/python/voltha_protos/adapter_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13096 2023-06-05 07:06:27.000000 voltha-protos-5.4.6/python/voltha_protos/core_services_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/openflow_13_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8405 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9978 2023-06-05 07:06:26.000000 voltha-protos-5.4.6/python/voltha_protos/adapter_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   162370 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/extensions_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    52525 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/openolt_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2588 2023-06-05 07:06:28.000000 voltha-protos-5.4.6/python/voltha_protos/health_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18434 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/omci_mib_db_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11674 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   247532 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/openolt_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:30.000000 voltha-protos-5.4.6/python/voltha_protos/tech_profile_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-06-05 07:06:29.000000 voltha-protos-5.4.6/python/voltha_protos/omci_alarm_db_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7988 2023-06-05 07:06:30.000000 voltha-protos-5.4.6/python/voltha_protos/voip_user_profile_pb2.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/python/test/
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-06-05 07:06:03.000000 voltha-protos-5.4.6/python/test/__init__.py
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1007 2023-06-05 07:06:03.000000 voltha-protos-5.4.6/python/test/test_protos.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/python/voltha_protos.egg-info/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/python/voltha_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/python/voltha_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2500 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/python/voltha_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       86 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/python/voltha_protos.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       19 2023-06-05 07:06:37.000000 voltha-protos-5.4.6/python/voltha_protos.egg-info/top_level.txt
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        6 2023-06-05 07:06:03.000000 voltha-protos-5.4.6/VERSION
```

### Comparing `voltha-protos-5.4.5/PKG-INFO` & `voltha-protos-5.4.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: voltha-protos
-Version: 5.4.5
+Version: 5.4.6
 Summary: Protobuf interface definitions
 Home-page: https://gerrit.opencord.org/gitweb?p=voltha-protos.git
 Author: VOLTHA project
 Author-email: voltha-dev@opencord.org
 License: Apache Software License
 Description: UNKNOWN
 Keywords: protobuf voltha
```

### Comparing `voltha-protos-5.4.5/README.md` & `voltha-protos-5.4.6/README.md`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/setup.py` & `voltha-protos-5.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/omci_alarm_db_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/omci_alarm_db_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/inter_adapter_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/inter_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/events_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/events_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/ext_config_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/ext_config_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/__init__.py` & `voltha-protos-5.4.6/python/voltha_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/adapter_service_pb2_grpc.py` & `voltha-protos-5.4.6/python/voltha_protos/adapter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/logical_device_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/logical_device_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/voltha_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/voltha_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,31 @@
 from voltha_protos import health_pb2 as voltha__protos_dot_health__pb2
 from voltha_protos import logical_device_pb2 as voltha__protos_dot_logical__device__pb2
 from voltha_protos import device_pb2 as voltha__protos_dot_device__pb2
 from voltha_protos import adapter_pb2 as voltha__protos_dot_adapter__pb2
 from voltha_protos import openflow_13_pb2 as voltha__protos_dot_openflow__13__pb2
 from voltha_protos import events_pb2 as voltha__protos_dot_events__pb2
 from voltha_protos import extensions_pb2 as voltha__protos_dot_extensions__pb2
+from voltha_protos import voip_system_profile_pb2 as voltha__protos_dot_voip__system__profile__pb2
+from voltha_protos import voip_user_profile_pb2 as voltha__protos_dot_voip__user__profile__pb2
 from voltha_protos import omci_mib_db_pb2 as voltha__protos_dot_omci__mib__db__pb2
 from voltha_protos import omci_alarm_db_pb2 as voltha__protos_dot_omci__alarm__db__pb2
 from voltha_protos import omci_test_pb2 as voltha__protos_dot_omci__test__pb2
 
 from voltha_protos.common_pb2 import *
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='voltha_protos/voltha.proto',
   package='voltha',
   syntax='proto3',
   serialized_options=b'\n\023org.opencord.volthaB\014VolthaProtosZ.github.com/opencord/voltha-protos/v5/go/voltha\252\002\026Opencord.Voltha.Voltha',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1avoltha_protos/voltha.proto\x12\x06voltha\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1avoltha_protos/common.proto\x1a\x1avoltha_protos/health.proto\x1a\"voltha_protos/logical_device.proto\x1a\x1avoltha_protos/device.proto\x1a\x1bvoltha_protos/adapter.proto\x1a\x1fvoltha_protos/openflow_13.proto\x1a\x1avoltha_protos/events.proto\x1a\x1evoltha_protos/extensions.proto\x1a\x1fvoltha_protos/omci_mib_db.proto\x1a!voltha_protos/omci_alarm_db.proto\x1a\x1dvoltha_protos/omci_test.proto\"I\n\x0c\x43oreInstance\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12$\n\x06health\x18\x02 \x01(\x0b\x32\x14.health.HealthStatus\"4\n\rCoreInstances\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.voltha.CoreInstance\"\xd5\x02\n\x06Voltha\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\"\n\x08\x61\x64\x61pters\x18\x02 \x03(\x0b\x32\x10.adapter.Adapter\x12\x36\n\x0flogical_devices\x18\x03 \x03(\x0b\x32\x1d.logical_device.LogicalDevice\x12\x1f\n\x07\x64\x65vices\x18\x04 \x03(\x0b\x32\x0e.device.Device\x12(\n\x0c\x64\x65vice_types\x18\x05 \x03(\x0b\x32\x12.device.DeviceType\x12)\n\revent_filters\x18\x07 \x03(\x0b\x32\x12.event.EventFilter\x12.\n\x11omci_mib_database\x18\x1c \x03(\x0b\x32\x13.omci.MibDeviceData\x12\x32\n\x13omci_alarm_database\x18\x1d \x03(\x0b\x32\x15.omci.AlarmDeviceDataJ\x04\x08\x06\x10\x07\x32\xc7\x33\n\rVolthaService\x12\x44\n\tGetVoltha\x12\x16.google.protobuf.Empty\x1a\x0e.voltha.Voltha\"\x0f\x82\xd3\xe4\x93\x02\t\x12\x07/api/v1\x12]\n\x11ListCoreInstances\x12\x16.google.protobuf.Empty\x1a\x15.voltha.CoreInstances\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/api/v1/instances\x12S\n\x0fGetCoreInstance\x12\n.common.ID\x1a\x14.voltha.CoreInstance\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/api/v1/instances/{id}\x12S\n\x0cListAdapters\x12\x16.google.protobuf.Empty\x1a\x11.adapter.Adapters\"\x18\x82\xd3\xe4\x93\x02\x12\x12\x10/api/v1/adapters\x12m\n\x12ListLogicalDevices\x12\x16.google.protobuf.Empty\x1a\x1e.logical_device.LogicalDevices\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/api/v1/logical_devices\x12\x63\n\x10GetLogicalDevice\x12\n.common.ID\x1a\x1d.logical_device.LogicalDevice\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/api/v1/logical_devices/{id}\x12n\n\x16ListLogicalDevicePorts\x12\n.common.ID\x1a\x1c.logical_device.LogicalPorts\"*\x82\xd3\xe4\x93\x02$\x12\"/api/v1/logical_devices/{id}/ports\x12\x88\x01\n\x14GetLogicalDevicePort\x12\x1d.logical_device.LogicalPortId\x1a\x1b.logical_device.LogicalPort\"4\x82\xd3\xe4\x93\x02.\x12,/api/v1/logical_devices/{id}/ports/{port_id}\x12\x8d\x01\n\x17\x45nableLogicalDevicePort\x12\x1d.logical_device.LogicalPortId\x1a\x16.google.protobuf.Empty\";\x82\xd3\xe4\x93\x02\x35\"3/api/v1/logical_devices/{id}/ports/{port_id}/enable\x12\x8f\x01\n\x18\x44isableLogicalDevicePort\x12\x1d.logical_device.LogicalPortId\x1a\x16.google.protobuf.Empty\"<\x82\xd3\xe4\x93\x02\x36\"4/api/v1/logical_devices/{id}/ports/{port_id}/disable\x12\x64\n\x16ListLogicalDeviceFlows\x12\n.common.ID\x1a\x12.openflow_13.Flows\"*\x82\xd3\xe4\x93\x02$\x12\"/api/v1/logical_devices/{id}/flows\x12\x83\x01\n\x1cUpdateLogicalDeviceFlowTable\x12\x1c.openflow_13.FlowTableUpdate\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'\"\"/api/v1/logical_devices/{id}/flows:\x01*\x12\x84\x01\n\x1dUpdateLogicalDeviceMeterTable\x12\x1b.openflow_13.MeterModUpdate\x1a\x16.google.protobuf.Empty\".\x82\xd3\xe4\x93\x02(\"#/api/v1/logical_devices/{id}/meters:\x01*\x12g\n\x17ListLogicalDeviceMeters\x12\n.common.ID\x1a\x13.openflow_13.Meters\"+\x82\xd3\xe4\x93\x02%\x12#/api/v1/logical_devices/{id}/meters\x12t\n\x1bListLogicalDeviceFlowGroups\x12\n.common.ID\x1a\x17.openflow_13.FlowGroups\"0\x82\xd3\xe4\x93\x02*\x12(/api/v1/logical_devices/{id}/flow_groups\x12\x93\x01\n!UpdateLogicalDeviceFlowGroupTable\x12!.openflow_13.FlowGroupTableUpdate\x1a\x16.google.protobuf.Empty\"3\x82\xd3\xe4\x93\x02-\"(/api/v1/logical_devices/{id}/flow_groups:\x01*\x12O\n\x0bListDevices\x12\x16.google.protobuf.Empty\x1a\x0f.device.Devices\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/api/v1/devices\x12O\n\rListDeviceIds\x12\x16.google.protobuf.Empty\x1a\x0b.common.IDs\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/api/v1/deviceids\x12U\n\x10ReconcileDevices\x12\x0b.common.IDs\x1a\x16.google.protobuf.Empty\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/api/v1/deviceids:\x01*\x12\x45\n\tGetDevice\x12\n.common.ID\x1a\x0e.device.Device\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/api/v1/devices/{id}\x12J\n\x0c\x43reateDevice\x12\x0e.device.Device\x1a\x0e.device.Device\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/api/v1/devices:\x01*\x12W\n\x0c\x45nableDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\"#\x82\xd3\xe4\x93\x02\x1d\"\x1b/api/v1/devices/{id}/enable\x12Y\n\rDisableDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\"$\x82\xd3\xe4\x93\x02\x1e\"\x1c/api/v1/devices/{id}/disable\x12W\n\x0cRebootDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\"#\x82\xd3\xe4\x93\x02\x1d\"\x1b/api/v1/devices/{id}/reboot\x12W\n\x0c\x44\x65leteDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\"#\x82\xd3\xe4\x93\x02\x1d*\x1b/api/v1/devices/{id}/delete\x12\x62\n\x11\x46orceDeleteDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\")\x82\xd3\xe4\x93\x02#*!/api/v1/devices/{id}/force_delete\x12x\n\rDownloadImage\x12\x15.device.ImageDownload\x1a\x15.common.OperationResp\"9\x88\x02\x01\x82\xd3\xe4\x93\x02\x30\"+/api/v1/devices/{id}/image_downloads/{name}:\x01*\x12\x85\x01\n\x16GetImageDownloadStatus\x12\x15.device.ImageDownload\x1a\x15.device.ImageDownload\"=\x88\x02\x01\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v1/devices/{id}/image_downloads/{name}/status\x12x\n\x10GetImageDownload\x12\x15.device.ImageDownload\x1a\x15.device.ImageDownload\"6\x88\x02\x01\x82\xd3\xe4\x93\x02-\x12+/api/v1/devices/{id}/image_downloads/{name}\x12i\n\x12ListImageDownloads\x12\n.common.ID\x1a\x16.device.ImageDownloads\"/\x88\x02\x01\x82\xd3\xe4\x93\x02&\x12$/api/v1/devices/{id}/image_downloads\x12{\n\x13\x43\x61ncelImageDownload\x12\x15.device.ImageDownload\x1a\x15.common.OperationResp\"6\x88\x02\x01\x82\xd3\xe4\x93\x02-*+/api/v1/devices/{id}/image_downloads/{name}\x12\x8b\x01\n\x13\x41\x63tivateImageUpdate\x12\x15.device.ImageDownload\x1a\x15.common.OperationResp\"F\x88\x02\x01\x82\xd3\xe4\x93\x02=\"8/api/v1/devices/{id}/image_downloads/{name}/image_update:\x01*\x12\x89\x01\n\x11RevertImageUpdate\x12\x15.device.ImageDownload\x1a\x15.common.OperationResp\"F\x88\x02\x01\x82\xd3\xe4\x93\x02=\"8/api/v1/devices/{id}/image_downloads/{name}/image_revert:\x01*\x12\x88\x01\n\x15\x44ownloadImageToDevice\x12\".device.DeviceImageDownloadRequest\x1a\x1b.device.DeviceImageResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/devices/images/download_images\x12w\n\x0eGetImageStatus\x12\x1a.device.DeviceImageRequest\x1a\x1b.device.DeviceImageResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/devices/images/images_status\x12\x89\x01\n\x19\x41\x62ortImageUpgradeToDevice\x12\x1a.device.DeviceImageRequest\x1a\x1b.device.DeviceImageResponse\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/devices/images/abort_upgrade_images\x12V\n\x0cGetOnuImages\x12\n.common.ID\x1a\x11.device.OnuImages\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/devices/{id}/onu_images\x12{\n\rActivateImage\x12\x1a.device.DeviceImageRequest\x1a\x1b.device.DeviceImageResponse\"1\x82\xd3\xe4\x93\x02+\"&/api/v1/devices/images/activate_images:\x01*\x12w\n\x0b\x43ommitImage\x12\x1a.device.DeviceImageRequest\x1a\x1b.device.DeviceImageResponse\"/\x82\xd3\xe4\x93\x02)\"$/api/v1/devices/images/commit_images:\x01*\x12P\n\x0fListDevicePorts\x12\n.common.ID\x1a\r.device.Ports\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/devices/{id}/ports\x12]\n\x13ListDevicePmConfigs\x12\n.common.ID\x1a\x11.device.PmConfigs\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/devices/{id}/pm_configs\x12n\n\x15UpdateDevicePmConfigs\x12\x11.device.PmConfigs\x1a\x16.google.protobuf.Empty\"*\x82\xd3\xe4\x93\x02$\"\x1f/api/v1/devices/{id}/pm_configs:\x01*\x12U\n\x0fListDeviceFlows\x12\n.common.ID\x1a\x12.openflow_13.Flows\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/devices/{id}/flows\x12\x65\n\x14ListDeviceFlowGroups\x12\n.common.ID\x1a\x17.openflow_13.FlowGroups\"(\x82\xd3\xe4\x93\x02\"\x12 /api/v1/devices/{id}/flow_groups\x12\\\n\x0fListDeviceTypes\x12\x16.google.protobuf.Empty\x1a\x13.device.DeviceTypes\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/api/v1/device_types\x12R\n\rGetDeviceType\x12\n.common.ID\x1a\x12.device.DeviceType\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/api/v1/device_types/{id}\x12\x46\n\x10StreamPacketsOut\x12\x16.openflow_13.PacketOut\x1a\x16.google.protobuf.Empty\"\x00(\x01\x12\x45\n\x10ReceivePacketsIn\x12\x16.google.protobuf.Empty\x1a\x15.openflow_13.PacketIn\"\x00\x30\x01\x12K\n\x13ReceiveChangeEvents\x12\x16.google.protobuf.Empty\x1a\x18.openflow_13.ChangeEvent\"\x00\x30\x01\x12]\n\x11\x43reateEventFilter\x12\x12.event.EventFilter\x1a\x12.event.EventFilter\" \x82\xd3\xe4\x93\x02\x1a\"\x15/api/v1/event_filters:\x01*\x12U\n\x0eGetEventFilter\x12\n.common.ID\x1a\x13.event.EventFilters\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/event_filters/{id}\x12\x62\n\x11UpdateEventFilter\x12\x12.event.EventFilter\x1a\x12.event.EventFilter\"%\x82\xd3\xe4\x93\x02\x1f\x1a\x1a/api/v1/event_filters/{id}:\x01*\x12\x63\n\x11\x44\x65leteEventFilter\x12\x12.event.EventFilter\x1a\x16.google.protobuf.Empty\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/api/v1/event_filters/{id}\x12^\n\x10ListEventFilters\x12\x16.google.protobuf.Empty\x1a\x13.event.EventFilters\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/api/v1/event_filters\x12L\n\tGetImages\x12\n.common.ID\x1a\x0e.device.Images\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v1/devices/{id}/images\x12X\n\x08SelfTest\x12\n.common.ID\x1a\x18.device.SelfTestResponse\"&\x82\xd3\xe4\x93\x02 \"\x1e/api/v1/devices/{id}/self_test\x12V\n\x10GetMibDeviceData\x12\n.common.ID\x1a\x13.omci.MibDeviceData\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/api/v1/openomci/{id}/mib\x12\\\n\x12GetAlarmDeviceData\x12\n.common.ID\x1a\x15.omci.AlarmDeviceData\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v1/openomci/{id}/alarm\x12s\n\rSimulateAlarm\x12\x1c.device.SimulateAlarmRequest\x1a\x15.common.OperationResp\"-\x82\xd3\xe4\x93\x02\'\"\"/api/v1/devices/{id}/simulate_larm:\x01*\x12M\n\nEnablePort\x12\x0c.device.Port\x1a\x16.google.protobuf.Empty\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/EnablePort:\x01*\x12O\n\x0b\x44isablePort\x12\x0c.device.Port\x1a\x16.google.protobuf.Empty\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/DisablePort:\x01*\x12^\n\x0bGetExtValue\x12\x19.extension.ValueSpecifier\x1a\x17.extension.ReturnValues\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/GetExtValue\x12W\n\x0bSetExtValue\x12\x13.extension.ValueSet\x1a\x16.google.protobuf.Empty\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/SetExtValue\x12\x64\n\x13StartOmciTestAction\x12\x15.omci.OmciTestRequest\x1a\x12.omci.TestResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v1/start_omci_test:\x01*Bl\n\x13org.opencord.volthaB\x0cVolthaProtosZ.github.com/opencord/voltha-protos/v5/go/voltha\xaa\x02\x16Opencord.Voltha.VolthaP\x02\x62\x06proto3'
+  serialized_pb=b'\n\x1avoltha_protos/voltha.proto\x12\x06voltha\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1avoltha_protos/common.proto\x1a\x1avoltha_protos/health.proto\x1a\"voltha_protos/logical_device.proto\x1a\x1avoltha_protos/device.proto\x1a\x1bvoltha_protos/adapter.proto\x1a\x1fvoltha_protos/openflow_13.proto\x1a\x1avoltha_protos/events.proto\x1a\x1evoltha_protos/extensions.proto\x1a\'voltha_protos/voip_system_profile.proto\x1a%voltha_protos/voip_user_profile.proto\x1a\x1fvoltha_protos/omci_mib_db.proto\x1a!voltha_protos/omci_alarm_db.proto\x1a\x1dvoltha_protos/omci_test.proto\"I\n\x0c\x43oreInstance\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12$\n\x06health\x18\x02 \x01(\x0b\x32\x14.health.HealthStatus\"4\n\rCoreInstances\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.voltha.CoreInstance\"\xd5\x02\n\x06Voltha\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\"\n\x08\x61\x64\x61pters\x18\x02 \x03(\x0b\x32\x10.adapter.Adapter\x12\x36\n\x0flogical_devices\x18\x03 \x03(\x0b\x32\x1d.logical_device.LogicalDevice\x12\x1f\n\x07\x64\x65vices\x18\x04 \x03(\x0b\x32\x0e.device.Device\x12(\n\x0c\x64\x65vice_types\x18\x05 \x03(\x0b\x32\x12.device.DeviceType\x12)\n\revent_filters\x18\x07 \x03(\x0b\x32\x12.event.EventFilter\x12.\n\x11omci_mib_database\x18\x1c \x03(\x0b\x32\x13.omci.MibDeviceData\x12\x32\n\x13omci_alarm_database\x18\x1d \x03(\x0b\x32\x15.omci.AlarmDeviceDataJ\x04\x08\x06\x10\x07\x32\xae\x37\n\rVolthaService\x12\x44\n\tGetVoltha\x12\x16.google.protobuf.Empty\x1a\x0e.voltha.Voltha\"\x0f\x82\xd3\xe4\x93\x02\t\x12\x07/api/v1\x12]\n\x11ListCoreInstances\x12\x16.google.protobuf.Empty\x1a\x15.voltha.CoreInstances\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/api/v1/instances\x12S\n\x0fGetCoreInstance\x12\n.common.ID\x1a\x14.voltha.CoreInstance\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/api/v1/instances/{id}\x12S\n\x0cListAdapters\x12\x16.google.protobuf.Empty\x1a\x11.adapter.Adapters\"\x18\x82\xd3\xe4\x93\x02\x12\x12\x10/api/v1/adapters\x12m\n\x12ListLogicalDevices\x12\x16.google.protobuf.Empty\x1a\x1e.logical_device.LogicalDevices\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/api/v1/logical_devices\x12\x63\n\x10GetLogicalDevice\x12\n.common.ID\x1a\x1d.logical_device.LogicalDevice\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/api/v1/logical_devices/{id}\x12n\n\x16ListLogicalDevicePorts\x12\n.common.ID\x1a\x1c.logical_device.LogicalPorts\"*\x82\xd3\xe4\x93\x02$\x12\"/api/v1/logical_devices/{id}/ports\x12\x88\x01\n\x14GetLogicalDevicePort\x12\x1d.logical_device.LogicalPortId\x1a\x1b.logical_device.LogicalPort\"4\x82\xd3\xe4\x93\x02.\x12,/api/v1/logical_devices/{id}/ports/{port_id}\x12\x8d\x01\n\x17\x45nableLogicalDevicePort\x12\x1d.logical_device.LogicalPortId\x1a\x16.google.protobuf.Empty\";\x82\xd3\xe4\x93\x02\x35\"3/api/v1/logical_devices/{id}/ports/{port_id}/enable\x12\x8f\x01\n\x18\x44isableLogicalDevicePort\x12\x1d.logical_device.LogicalPortId\x1a\x16.google.protobuf.Empty\"<\x82\xd3\xe4\x93\x02\x36\"4/api/v1/logical_devices/{id}/ports/{port_id}/disable\x12\x64\n\x16ListLogicalDeviceFlows\x12\n.common.ID\x1a\x12.openflow_13.Flows\"*\x82\xd3\xe4\x93\x02$\x12\"/api/v1/logical_devices/{id}/flows\x12\x83\x01\n\x1cUpdateLogicalDeviceFlowTable\x12\x1c.openflow_13.FlowTableUpdate\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'\"\"/api/v1/logical_devices/{id}/flows:\x01*\x12\x84\x01\n\x1dUpdateLogicalDeviceMeterTable\x12\x1b.openflow_13.MeterModUpdate\x1a\x16.google.protobuf.Empty\".\x82\xd3\xe4\x93\x02(\"#/api/v1/logical_devices/{id}/meters:\x01*\x12g\n\x17ListLogicalDeviceMeters\x12\n.common.ID\x1a\x13.openflow_13.Meters\"+\x82\xd3\xe4\x93\x02%\x12#/api/v1/logical_devices/{id}/meters\x12t\n\x1bListLogicalDeviceFlowGroups\x12\n.common.ID\x1a\x17.openflow_13.FlowGroups\"0\x82\xd3\xe4\x93\x02*\x12(/api/v1/logical_devices/{id}/flow_groups\x12\x93\x01\n!UpdateLogicalDeviceFlowGroupTable\x12!.openflow_13.FlowGroupTableUpdate\x1a\x16.google.protobuf.Empty\"3\x82\xd3\xe4\x93\x02-\"(/api/v1/logical_devices/{id}/flow_groups:\x01*\x12O\n\x0bListDevices\x12\x16.google.protobuf.Empty\x1a\x0f.device.Devices\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/api/v1/devices\x12O\n\rListDeviceIds\x12\x16.google.protobuf.Empty\x1a\x0b.common.IDs\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/api/v1/deviceids\x12U\n\x10ReconcileDevices\x12\x0b.common.IDs\x1a\x16.google.protobuf.Empty\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/api/v1/deviceids:\x01*\x12\x45\n\tGetDevice\x12\n.common.ID\x1a\x0e.device.Device\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/api/v1/devices/{id}\x12J\n\x0c\x43reateDevice\x12\x0e.device.Device\x1a\x0e.device.Device\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/api/v1/devices:\x01*\x12W\n\x0c\x45nableDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\"#\x82\xd3\xe4\x93\x02\x1d\"\x1b/api/v1/devices/{id}/enable\x12Y\n\rDisableDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\"$\x82\xd3\xe4\x93\x02\x1e\"\x1c/api/v1/devices/{id}/disable\x12W\n\x0cRebootDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\"#\x82\xd3\xe4\x93\x02\x1d\"\x1b/api/v1/devices/{id}/reboot\x12W\n\x0c\x44\x65leteDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\"#\x82\xd3\xe4\x93\x02\x1d*\x1b/api/v1/devices/{id}/delete\x12\x62\n\x11\x46orceDeleteDevice\x12\n.common.ID\x1a\x16.google.protobuf.Empty\")\x82\xd3\xe4\x93\x02#*!/api/v1/devices/{id}/force_delete\x12x\n\rDownloadImage\x12\x15.device.ImageDownload\x1a\x15.common.OperationResp\"9\x88\x02\x01\x82\xd3\xe4\x93\x02\x30\"+/api/v1/devices/{id}/image_downloads/{name}:\x01*\x12\x85\x01\n\x16GetImageDownloadStatus\x12\x15.device.ImageDownload\x1a\x15.device.ImageDownload\"=\x88\x02\x01\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v1/devices/{id}/image_downloads/{name}/status\x12x\n\x10GetImageDownload\x12\x15.device.ImageDownload\x1a\x15.device.ImageDownload\"6\x88\x02\x01\x82\xd3\xe4\x93\x02-\x12+/api/v1/devices/{id}/image_downloads/{name}\x12i\n\x12ListImageDownloads\x12\n.common.ID\x1a\x16.device.ImageDownloads\"/\x88\x02\x01\x82\xd3\xe4\x93\x02&\x12$/api/v1/devices/{id}/image_downloads\x12{\n\x13\x43\x61ncelImageDownload\x12\x15.device.ImageDownload\x1a\x15.common.OperationResp\"6\x88\x02\x01\x82\xd3\xe4\x93\x02-*+/api/v1/devices/{id}/image_downloads/{name}\x12\x8b\x01\n\x13\x41\x63tivateImageUpdate\x12\x15.device.ImageDownload\x1a\x15.common.OperationResp\"F\x88\x02\x01\x82\xd3\xe4\x93\x02=\"8/api/v1/devices/{id}/image_downloads/{name}/image_update:\x01*\x12\x89\x01\n\x11RevertImageUpdate\x12\x15.device.ImageDownload\x1a\x15.common.OperationResp\"F\x88\x02\x01\x82\xd3\xe4\x93\x02=\"8/api/v1/devices/{id}/image_downloads/{name}/image_revert:\x01*\x12\x88\x01\n\x15\x44ownloadImageToDevice\x12\".device.DeviceImageDownloadRequest\x1a\x1b.device.DeviceImageResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/devices/images/download_images\x12w\n\x0eGetImageStatus\x12\x1a.device.DeviceImageRequest\x1a\x1b.device.DeviceImageResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/devices/images/images_status\x12\x89\x01\n\x19\x41\x62ortImageUpgradeToDevice\x12\x1a.device.DeviceImageRequest\x1a\x1b.device.DeviceImageResponse\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/devices/images/abort_upgrade_images\x12V\n\x0cGetOnuImages\x12\n.common.ID\x1a\x11.device.OnuImages\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/devices/{id}/onu_images\x12{\n\rActivateImage\x12\x1a.device.DeviceImageRequest\x1a\x1b.device.DeviceImageResponse\"1\x82\xd3\xe4\x93\x02+\"&/api/v1/devices/images/activate_images:\x01*\x12w\n\x0b\x43ommitImage\x12\x1a.device.DeviceImageRequest\x1a\x1b.device.DeviceImageResponse\"/\x82\xd3\xe4\x93\x02)\"$/api/v1/devices/images/commit_images:\x01*\x12P\n\x0fListDevicePorts\x12\n.common.ID\x1a\r.device.Ports\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/devices/{id}/ports\x12]\n\x13ListDevicePmConfigs\x12\n.common.ID\x1a\x11.device.PmConfigs\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/devices/{id}/pm_configs\x12n\n\x15UpdateDevicePmConfigs\x12\x11.device.PmConfigs\x1a\x16.google.protobuf.Empty\"*\x82\xd3\xe4\x93\x02$\"\x1f/api/v1/devices/{id}/pm_configs:\x01*\x12U\n\x0fListDeviceFlows\x12\n.common.ID\x1a\x12.openflow_13.Flows\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/devices/{id}/flows\x12\x65\n\x14ListDeviceFlowGroups\x12\n.common.ID\x1a\x17.openflow_13.FlowGroups\"(\x82\xd3\xe4\x93\x02\"\x12 /api/v1/devices/{id}/flow_groups\x12\\\n\x0fListDeviceTypes\x12\x16.google.protobuf.Empty\x1a\x13.device.DeviceTypes\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/api/v1/device_types\x12R\n\rGetDeviceType\x12\n.common.ID\x1a\x12.device.DeviceType\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/api/v1/device_types/{id}\x12\x46\n\x10StreamPacketsOut\x12\x16.openflow_13.PacketOut\x1a\x16.google.protobuf.Empty\"\x00(\x01\x12\x45\n\x10ReceivePacketsIn\x12\x16.google.protobuf.Empty\x1a\x15.openflow_13.PacketIn\"\x00\x30\x01\x12K\n\x13ReceiveChangeEvents\x12\x16.google.protobuf.Empty\x1a\x18.openflow_13.ChangeEvent\"\x00\x30\x01\x12]\n\x11\x43reateEventFilter\x12\x12.event.EventFilter\x1a\x12.event.EventFilter\" \x82\xd3\xe4\x93\x02\x1a\"\x15/api/v1/event_filters:\x01*\x12U\n\x0eGetEventFilter\x12\n.common.ID\x1a\x13.event.EventFilters\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/event_filters/{id}\x12\x62\n\x11UpdateEventFilter\x12\x12.event.EventFilter\x1a\x12.event.EventFilter\"%\x82\xd3\xe4\x93\x02\x1f\x1a\x1a/api/v1/event_filters/{id}:\x01*\x12\x63\n\x11\x44\x65leteEventFilter\x12\x12.event.EventFilter\x1a\x16.google.protobuf.Empty\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/api/v1/event_filters/{id}\x12^\n\x10ListEventFilters\x12\x16.google.protobuf.Empty\x1a\x13.event.EventFilters\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/api/v1/event_filters\x12L\n\tGetImages\x12\n.common.ID\x1a\x0e.device.Images\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v1/devices/{id}/images\x12X\n\x08SelfTest\x12\n.common.ID\x1a\x18.device.SelfTestResponse\"&\x82\xd3\xe4\x93\x02 \"\x1e/api/v1/devices/{id}/self_test\x12V\n\x10GetMibDeviceData\x12\n.common.ID\x1a\x13.omci.MibDeviceData\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/api/v1/openomci/{id}/mib\x12\\\n\x12GetAlarmDeviceData\x12\n.common.ID\x1a\x15.omci.AlarmDeviceData\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v1/openomci/{id}/alarm\x12s\n\rSimulateAlarm\x12\x1c.device.SimulateAlarmRequest\x1a\x15.common.OperationResp\"-\x82\xd3\xe4\x93\x02\'\"\"/api/v1/devices/{id}/simulate_larm:\x01*\x12M\n\nEnablePort\x12\x0c.device.Port\x1a\x16.google.protobuf.Empty\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/EnablePort:\x01*\x12O\n\x0b\x44isablePort\x12\x0c.device.Port\x1a\x16.google.protobuf.Empty\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/DisablePort:\x01*\x12^\n\x0bGetExtValue\x12\x19.extension.ValueSpecifier\x1a\x17.extension.ReturnValues\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/GetExtValue\x12W\n\x0bSetExtValue\x12\x13.extension.ValueSet\x1a\x16.google.protobuf.Empty\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/SetExtValue\x12\x64\n\x13StartOmciTestAction\x12\x15.omci.OmciTestRequest\x1a\x12.omci.TestResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v1/start_omci_test:\x01*\x12\x85\x01\n\x14PutVoipSystemProfile\x12-.voip_system_profile.VoipSystemProfileRequest\x1a\x16.google.protobuf.Empty\"&\x82\xd3\xe4\x93\x02 \"\x1b/api/v1/voip_system_profile:\x01*\x12p\n\x17\x44\x65leteVoipSystemProfile\x12\x0b.common.Key\x1a\x16.google.protobuf.Empty\"0\x82\xd3\xe4\x93\x02**(/api/v1/voip_system_profile/{key}/delete\x12}\n\x12PutVoipUserProfile\x12).voip_user_profile.VoipUserProfileRequest\x1a\x16.google.protobuf.Empty\"$\x82\xd3\xe4\x93\x02\x1e\"\x19/api/v1/voip_user_profile:\x01*\x12l\n\x15\x44\x65leteVoipUserProfile\x12\x0b.common.Key\x1a\x16.google.protobuf.Empty\".\x82\xd3\xe4\x93\x02(*&/api/v1/voip_user_profile/{key}/deleteBl\n\x13org.opencord.volthaB\x0cVolthaProtosZ.github.com/opencord/voltha-protos/v5/go/voltha\xaa\x02\x16Opencord.Voltha.VolthaP\x02\x62\x06proto3'
   ,
-  dependencies=[google_dot_api_dot_annotations__pb2.DESCRIPTOR,google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,voltha__protos_dot_common__pb2.DESCRIPTOR,voltha__protos_dot_health__pb2.DESCRIPTOR,voltha__protos_dot_logical__device__pb2.DESCRIPTOR,voltha__protos_dot_device__pb2.DESCRIPTOR,voltha__protos_dot_adapter__pb2.DESCRIPTOR,voltha__protos_dot_openflow__13__pb2.DESCRIPTOR,voltha__protos_dot_events__pb2.DESCRIPTOR,voltha__protos_dot_extensions__pb2.DESCRIPTOR,voltha__protos_dot_omci__mib__db__pb2.DESCRIPTOR,voltha__protos_dot_omci__alarm__db__pb2.DESCRIPTOR,voltha__protos_dot_omci__test__pb2.DESCRIPTOR,],
+  dependencies=[google_dot_api_dot_annotations__pb2.DESCRIPTOR,google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,voltha__protos_dot_common__pb2.DESCRIPTOR,voltha__protos_dot_health__pb2.DESCRIPTOR,voltha__protos_dot_logical__device__pb2.DESCRIPTOR,voltha__protos_dot_device__pb2.DESCRIPTOR,voltha__protos_dot_adapter__pb2.DESCRIPTOR,voltha__protos_dot_openflow__13__pb2.DESCRIPTOR,voltha__protos_dot_events__pb2.DESCRIPTOR,voltha__protos_dot_extensions__pb2.DESCRIPTOR,voltha__protos_dot_voip__system__profile__pb2.DESCRIPTOR,voltha__protos_dot_voip__user__profile__pb2.DESCRIPTOR,voltha__protos_dot_omci__mib__db__pb2.DESCRIPTOR,voltha__protos_dot_omci__alarm__db__pb2.DESCRIPTOR,voltha__protos_dot_omci__test__pb2.DESCRIPTOR,],
   public_dependencies=[voltha__protos_dot_common__pb2.DESCRIPTOR,])
 
 
 
 
 _COREINSTANCE = _descriptor.Descriptor(
   name='CoreInstance',
@@ -71,16 +73,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=438,
-  serialized_end=511,
+  serialized_start=518,
+  serialized_end=591,
 )
 
 
 _COREINSTANCES = _descriptor.Descriptor(
   name='CoreInstances',
   full_name='voltha.CoreInstances',
   filename=None,
@@ -103,16 +105,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=513,
-  serialized_end=565,
+  serialized_start=593,
+  serialized_end=645,
 )
 
 
 _VOLTHA = _descriptor.Descriptor(
   name='Voltha',
   full_name='voltha.Voltha',
   filename=None,
@@ -184,16 +186,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=568,
-  serialized_end=909,
+  serialized_start=648,
+  serialized_end=989,
 )
 
 _COREINSTANCE.fields_by_name['health'].message_type = voltha__protos_dot_health__pb2._HEALTHSTATUS
 _COREINSTANCES.fields_by_name['items'].message_type = _COREINSTANCE
 _VOLTHA.fields_by_name['adapters'].message_type = voltha__protos_dot_adapter__pb2._ADAPTER
 _VOLTHA.fields_by_name['logical_devices'].message_type = voltha__protos_dot_logical__device__pb2._LOGICALDEVICE
 _VOLTHA.fields_by_name['devices'].message_type = voltha__protos_dot_device__pb2._DEVICE
@@ -233,16 +235,16 @@
 _VOLTHASERVICE = _descriptor.ServiceDescriptor(
   name='VolthaService',
   full_name='voltha.VolthaService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=912,
-  serialized_end=7511,
+  serialized_start=992,
+  serialized_end=8078,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetVoltha',
     full_name='voltha.VolthaService.GetVoltha',
     index=0,
     containing_service=None,
     input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
@@ -876,13 +878,53 @@
     index=63,
     containing_service=None,
     input_type=voltha__protos_dot_omci__test__pb2._OMCITESTREQUEST,
     output_type=voltha__protos_dot_omci__test__pb2._TESTRESPONSE,
     serialized_options=b'\202\323\344\223\002\034\"\027/api/v1/start_omci_test:\001*',
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='PutVoipSystemProfile',
+    full_name='voltha.VolthaService.PutVoipSystemProfile',
+    index=64,
+    containing_service=None,
+    input_type=voltha__protos_dot_voip__system__profile__pb2._VOIPSYSTEMPROFILEREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=b'\202\323\344\223\002 \"\033/api/v1/voip_system_profile:\001*',
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='DeleteVoipSystemProfile',
+    full_name='voltha.VolthaService.DeleteVoipSystemProfile',
+    index=65,
+    containing_service=None,
+    input_type=voltha__protos_dot_common__pb2._KEY,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=b'\202\323\344\223\002**(/api/v1/voip_system_profile/{key}/delete',
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='PutVoipUserProfile',
+    full_name='voltha.VolthaService.PutVoipUserProfile',
+    index=66,
+    containing_service=None,
+    input_type=voltha__protos_dot_voip__user__profile__pb2._VOIPUSERPROFILEREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=b'\202\323\344\223\002\036\"\031/api/v1/voip_user_profile:\001*',
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='DeleteVoipUserProfile',
+    full_name='voltha.VolthaService.DeleteVoipUserProfile',
+    index=67,
+    containing_service=None,
+    input_type=voltha__protos_dot_common__pb2._KEY,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=b'\202\323\344\223\002(*&/api/v1/voip_user_profile/{key}/delete',
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_VOLTHASERVICE)
 
 DESCRIPTOR.services_by_name['VolthaService'] = _VOLTHASERVICE
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `voltha-protos-5.4.5/python/voltha_protos/voltha_pb2_grpc.py` & `voltha-protos-5.4.6/python/voltha_protos/voltha_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from voltha_protos import events_pb2 as voltha__protos_dot_events__pb2
 from voltha_protos import extensions_pb2 as voltha__protos_dot_extensions__pb2
 from voltha_protos import logical_device_pb2 as voltha__protos_dot_logical__device__pb2
 from voltha_protos import omci_alarm_db_pb2 as voltha__protos_dot_omci__alarm__db__pb2
 from voltha_protos import omci_mib_db_pb2 as voltha__protos_dot_omci__mib__db__pb2
 from voltha_protos import omci_test_pb2 as voltha__protos_dot_omci__test__pb2
 from voltha_protos import openflow_13_pb2 as voltha__protos_dot_openflow__13__pb2
+from voltha_protos import voip_system_profile_pb2 as voltha__protos_dot_voip__system__profile__pb2
+from voltha_protos import voip_user_profile_pb2 as voltha__protos_dot_voip__user__profile__pb2
 from voltha_protos import voltha_pb2 as voltha__protos_dot_voltha__pb2
 
 
 class VolthaServiceStub(object):
     """
     Voltha APIs
 
@@ -344,14 +346,34 @@
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.StartOmciTestAction = channel.unary_unary(
                 '/voltha.VolthaService/StartOmciTestAction',
                 request_serializer=voltha__protos_dot_omci__test__pb2.OmciTestRequest.SerializeToString,
                 response_deserializer=voltha__protos_dot_omci__test__pb2.TestResponse.FromString,
                 )
+        self.PutVoipSystemProfile = channel.unary_unary(
+                '/voltha.VolthaService/PutVoipSystemProfile',
+                request_serializer=voltha__protos_dot_voip__system__profile__pb2.VoipSystemProfileRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.DeleteVoipSystemProfile = channel.unary_unary(
+                '/voltha.VolthaService/DeleteVoipSystemProfile',
+                request_serializer=voltha__protos_dot_common__pb2.Key.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.PutVoipUserProfile = channel.unary_unary(
+                '/voltha.VolthaService/PutVoipUserProfile',
+                request_serializer=voltha__protos_dot_voip__user__profile__pb2.VoipUserProfileRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.DeleteVoipUserProfile = channel.unary_unary(
+                '/voltha.VolthaService/DeleteVoipUserProfile',
+                request_serializer=voltha__protos_dot_common__pb2.Key.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
 
 
 class VolthaServiceServicer(object):
     """
     Voltha APIs
 
     """
@@ -832,14 +854,42 @@
     def StartOmciTestAction(self, request, context):
         """omci start and stop cli implementation
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def PutVoipSystemProfile(self, request, context):
+        """Saves or updates system wide configuration into voltha KV
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteVoipSystemProfile(self, request, context):
+        """Deletes the given profile from voltha KV
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def PutVoipUserProfile(self, request, context):
+        """Saves or updates a profile (VOIP) into voltha KV
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteVoipUserProfile(self, request, context):
+        """Deletes the given profile from voltha KV
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_VolthaServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetVoltha': grpc.unary_unary_rpc_method_handler(
                     servicer.GetVoltha,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=voltha__protos_dot_voltha__pb2.Voltha.SerializeToString,
@@ -1155,14 +1205,34 @@
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'StartOmciTestAction': grpc.unary_unary_rpc_method_handler(
                     servicer.StartOmciTestAction,
                     request_deserializer=voltha__protos_dot_omci__test__pb2.OmciTestRequest.FromString,
                     response_serializer=voltha__protos_dot_omci__test__pb2.TestResponse.SerializeToString,
             ),
+            'PutVoipSystemProfile': grpc.unary_unary_rpc_method_handler(
+                    servicer.PutVoipSystemProfile,
+                    request_deserializer=voltha__protos_dot_voip__system__profile__pb2.VoipSystemProfileRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'DeleteVoipSystemProfile': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteVoipSystemProfile,
+                    request_deserializer=voltha__protos_dot_common__pb2.Key.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'PutVoipUserProfile': grpc.unary_unary_rpc_method_handler(
+                    servicer.PutVoipUserProfile,
+                    request_deserializer=voltha__protos_dot_voip__user__profile__pb2.VoipUserProfileRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'DeleteVoipUserProfile': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteVoipUserProfile,
+                    request_deserializer=voltha__protos_dot_common__pb2.Key.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'voltha.VolthaService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -2255,7 +2325,75 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/voltha.VolthaService/StartOmciTestAction',
             voltha__protos_dot_omci__test__pb2.OmciTestRequest.SerializeToString,
             voltha__protos_dot_omci__test__pb2.TestResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def PutVoipSystemProfile(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/voltha.VolthaService/PutVoipSystemProfile',
+            voltha__protos_dot_voip__system__profile__pb2.VoipSystemProfileRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteVoipSystemProfile(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/voltha.VolthaService/DeleteVoipSystemProfile',
+            voltha__protos_dot_common__pb2.Key.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def PutVoipUserProfile(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/voltha.VolthaService/PutVoipUserProfile',
+            voltha__protos_dot_voip__user__profile__pb2.VoipUserProfileRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteVoipUserProfile(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/voltha.VolthaService/DeleteVoipUserProfile',
+            voltha__protos_dot_common__pb2.Key.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `voltha-protos-5.4.5/python/voltha_protos/core_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/core_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/extensions_pb2_grpc.py` & `voltha-protos-5.4.6/python/voltha_protos/extensions_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/ietf_interfaces_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/ietf_interfaces_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/omci_test_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/omci_test_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/onu_inter_adapter_service_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/onu_inter_adapter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/openflow_13_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/openflow_13_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/device_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/device_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/core_adapter_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/core_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/core_services_pb2_grpc.py` & `voltha-protos-5.4.6/python/voltha_protos/core_services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/health_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/health_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/tech_profile_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/tech_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/olt_inter_adapter_service_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/olt_inter_adapter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/common_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/common_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='voltha_protos/common.proto',
   package='common',
   syntax='proto3',
   serialized_options=b'\n\023org.opencord.volthaZ.github.com/opencord/voltha-protos/v5/go/common',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1avoltha_protos/common.proto\x12\x06\x63ommon\"\x10\n\x02ID\x12\n\n\x02id\x18\x01 \x01(\t\" \n\x03IDs\x12\x19\n\x05items\x18\x01 \x03(\x0b\x32\n.common.ID\"P\n\nConnection\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x13\n\x0b\x63ontextInfo\x18\x02 \x01(\t\x12\x1b\n\x13keep_alive_interval\x18\x03 \x01(\x03\"h\n\nAdminState\"Z\n\x05Types\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x12\n\x0ePREPROVISIONED\x10\x01\x12\x0b\n\x07\x45NABLED\x10\x02\x12\x0c\n\x08\x44ISABLED\x10\x03\x12\x15\n\x11\x44OWNLOADING_IMAGE\x10\x04\"\x9f\x01\n\nOperStatus\"\x90\x01\n\x05Types\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nDISCOVERED\x10\x01\x12\x0e\n\nACTIVATING\x10\x02\x12\x0b\n\x07TESTING\x10\x03\x12\n\n\x06\x41\x43TIVE\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0f\n\x0bRECONCILING\x10\x06\x12\x16\n\x12RECONCILING_FAILED\x10\x07\x12\x0c\n\x08REBOOTED\x10\x08\"E\n\rConnectStatus\"4\n\x05Types\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bUNREACHABLE\x10\x01\x12\r\n\tREACHABLE\x10\x02\"\xdc\x01\n\rOperationResp\x12\x37\n\x04\x63ode\x18\x01 \x01(\x0e\x32).common.OperationResp.OperationReturnCode\x12\x17\n\x0f\x61\x64\x64itional_info\x18\x02 \x01(\t\"y\n\x13OperationReturnCode\x12\x15\n\x11OPERATION_SUCCESS\x10\x00\x12\x15\n\x11OPERATION_FAILURE\x10\x01\x12\x19\n\x15OPERATION_UNSUPPORTED\x10\x02\x12\x19\n\x15OPERATION_IN_PROGRESS\x10\x03*\x1c\n\x0cTestModeKeys\x12\x0c\n\x08\x61pi_test\x10\x00\x42\x45\n\x13org.opencord.volthaZ.github.com/opencord/voltha-protos/v5/go/commonb\x06proto3'
+  serialized_pb=b'\n\x1avoltha_protos/common.proto\x12\x06\x63ommon\"\x12\n\x03Key\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x10\n\x02ID\x12\n\n\x02id\x18\x01 \x01(\t\" \n\x03IDs\x12\x19\n\x05items\x18\x01 \x03(\x0b\x32\n.common.ID\"P\n\nConnection\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x13\n\x0b\x63ontextInfo\x18\x02 \x01(\t\x12\x1b\n\x13keep_alive_interval\x18\x03 \x01(\x03\"h\n\nAdminState\"Z\n\x05Types\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x12\n\x0ePREPROVISIONED\x10\x01\x12\x0b\n\x07\x45NABLED\x10\x02\x12\x0c\n\x08\x44ISABLED\x10\x03\x12\x15\n\x11\x44OWNLOADING_IMAGE\x10\x04\"\x9f\x01\n\nOperStatus\"\x90\x01\n\x05Types\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nDISCOVERED\x10\x01\x12\x0e\n\nACTIVATING\x10\x02\x12\x0b\n\x07TESTING\x10\x03\x12\n\n\x06\x41\x43TIVE\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0f\n\x0bRECONCILING\x10\x06\x12\x16\n\x12RECONCILING_FAILED\x10\x07\x12\x0c\n\x08REBOOTED\x10\x08\"E\n\rConnectStatus\"4\n\x05Types\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bUNREACHABLE\x10\x01\x12\r\n\tREACHABLE\x10\x02\"\xdc\x01\n\rOperationResp\x12\x37\n\x04\x63ode\x18\x01 \x01(\x0e\x32).common.OperationResp.OperationReturnCode\x12\x17\n\x0f\x61\x64\x64itional_info\x18\x02 \x01(\t\"y\n\x13OperationReturnCode\x12\x15\n\x11OPERATION_SUCCESS\x10\x00\x12\x15\n\x11OPERATION_FAILURE\x10\x01\x12\x19\n\x15OPERATION_UNSUPPORTED\x10\x02\x12\x19\n\x15OPERATION_IN_PROGRESS\x10\x03*\x1c\n\x0cTestModeKeys\x12\x0c\n\x08\x61pi_test\x10\x00\x42\x45\n\x13org.opencord.volthaZ.github.com/opencord/voltha-protos/v5/go/commonb\x06proto3'
 )
 
 _TESTMODEKEYS = _descriptor.EnumDescriptor(
   name='TestModeKeys',
   full_name='common.TestModeKeys',
   filename=None,
   file=DESCRIPTOR,
@@ -34,16 +34,16 @@
       name='api_test', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=734,
-  serialized_end=762,
+  serialized_start=754,
+  serialized_end=782,
 )
 _sym_db.RegisterEnumDescriptor(_TESTMODEKEYS)
 
 TestModeKeys = enum_type_wrapper.EnumTypeWrapper(_TESTMODEKEYS)
 api_test = 0
 
 
@@ -78,16 +78,16 @@
       name='DOWNLOADING_IMAGE', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=186,
-  serialized_end=276,
+  serialized_start=206,
+  serialized_end=296,
 )
 _sym_db.RegisterEnumDescriptor(_ADMINSTATE_TYPES)
 
 _OPERSTATUS_TYPES = _descriptor.EnumDescriptor(
   name='Types',
   full_name='common.OperStatus.Types',
   filename=None,
@@ -138,16 +138,16 @@
       name='REBOOTED', index=8, number=8,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=294,
-  serialized_end=438,
+  serialized_start=314,
+  serialized_end=458,
 )
 _sym_db.RegisterEnumDescriptor(_OPERSTATUS_TYPES)
 
 _CONNECTSTATUS_TYPES = _descriptor.EnumDescriptor(
   name='Types',
   full_name='common.ConnectStatus.Types',
   filename=None,
@@ -168,16 +168,16 @@
       name='REACHABLE', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=457,
-  serialized_end=509,
+  serialized_start=477,
+  serialized_end=529,
 )
 _sym_db.RegisterEnumDescriptor(_CONNECTSTATUS_TYPES)
 
 _OPERATIONRESP_OPERATIONRETURNCODE = _descriptor.EnumDescriptor(
   name='OperationReturnCode',
   full_name='common.OperationResp.OperationReturnCode',
   filename=None,
@@ -203,20 +203,52 @@
       name='OPERATION_IN_PROGRESS', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=611,
-  serialized_end=732,
+  serialized_start=631,
+  serialized_end=752,
 )
 _sym_db.RegisterEnumDescriptor(_OPERATIONRESP_OPERATIONRETURNCODE)
 
 
+_KEY = _descriptor.Descriptor(
+  name='Key',
+  full_name='common.Key',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='common.Key.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=38,
+  serialized_end=56,
+)
+
+
 _ID = _descriptor.Descriptor(
   name='ID',
   full_name='common.ID',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -236,16 +268,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=38,
-  serialized_end=54,
+  serialized_start=58,
+  serialized_end=74,
 )
 
 
 _IDS = _descriptor.Descriptor(
   name='IDs',
   full_name='common.IDs',
   filename=None,
@@ -268,16 +300,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=56,
-  serialized_end=88,
+  serialized_start=76,
+  serialized_end=108,
 )
 
 
 _CONNECTION = _descriptor.Descriptor(
   name='Connection',
   full_name='common.Connection',
   filename=None,
@@ -314,16 +346,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=90,
-  serialized_end=170,
+  serialized_start=110,
+  serialized_end=190,
 )
 
 
 _ADMINSTATE = _descriptor.Descriptor(
   name='AdminState',
   full_name='common.AdminState',
   filename=None,
@@ -340,16 +372,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=172,
-  serialized_end=276,
+  serialized_start=192,
+  serialized_end=296,
 )
 
 
 _OPERSTATUS = _descriptor.Descriptor(
   name='OperStatus',
   full_name='common.OperStatus',
   filename=None,
@@ -366,16 +398,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=279,
-  serialized_end=438,
+  serialized_start=299,
+  serialized_end=458,
 )
 
 
 _CONNECTSTATUS = _descriptor.Descriptor(
   name='ConnectStatus',
   full_name='common.ConnectStatus',
   filename=None,
@@ -392,16 +424,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=440,
-  serialized_end=509,
+  serialized_start=460,
+  serialized_end=529,
 )
 
 
 _OPERATIONRESP = _descriptor.Descriptor(
   name='OperationResp',
   full_name='common.OperationResp',
   filename=None,
@@ -432,34 +464,42 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=512,
-  serialized_end=732,
+  serialized_start=532,
+  serialized_end=752,
 )
 
 _IDS.fields_by_name['items'].message_type = _ID
 _ADMINSTATE_TYPES.containing_type = _ADMINSTATE
 _OPERSTATUS_TYPES.containing_type = _OPERSTATUS
 _CONNECTSTATUS_TYPES.containing_type = _CONNECTSTATUS
 _OPERATIONRESP.fields_by_name['code'].enum_type = _OPERATIONRESP_OPERATIONRETURNCODE
 _OPERATIONRESP_OPERATIONRETURNCODE.containing_type = _OPERATIONRESP
+DESCRIPTOR.message_types_by_name['Key'] = _KEY
 DESCRIPTOR.message_types_by_name['ID'] = _ID
 DESCRIPTOR.message_types_by_name['IDs'] = _IDS
 DESCRIPTOR.message_types_by_name['Connection'] = _CONNECTION
 DESCRIPTOR.message_types_by_name['AdminState'] = _ADMINSTATE
 DESCRIPTOR.message_types_by_name['OperStatus'] = _OPERSTATUS
 DESCRIPTOR.message_types_by_name['ConnectStatus'] = _CONNECTSTATUS
 DESCRIPTOR.message_types_by_name['OperationResp'] = _OPERATIONRESP
 DESCRIPTOR.enum_types_by_name['TestModeKeys'] = _TESTMODEKEYS
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
+Key = _reflection.GeneratedProtocolMessageType('Key', (_message.Message,), {
+  'DESCRIPTOR' : _KEY,
+  '__module__' : 'voltha_protos.common_pb2'
+  # @@protoc_insertion_point(class_scope:common.Key)
+  })
+_sym_db.RegisterMessage(Key)
+
 ID = _reflection.GeneratedProtocolMessageType('ID', (_message.Message,), {
   'DESCRIPTOR' : _ID,
   '__module__' : 'voltha_protos.common_pb2'
   # @@protoc_insertion_point(class_scope:common.ID)
   })
 _sym_db.RegisterMessage(ID)
```

### Comparing `voltha-protos-5.4.5/python/voltha_protos/adapter_service_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/adapter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/core_services_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/core_services_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py` & `voltha-protos-5.4.6/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/adapter_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/extensions_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/openolt_pb2_grpc.py` & `voltha-protos-5.4.6/python/voltha_protos/openolt_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/health_pb2_grpc.py` & `voltha-protos-5.4.6/python/voltha_protos/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/omci_mib_db_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/omci_mib_db_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py` & `voltha-protos-5.4.6/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos/openolt_pb2.py` & `voltha-protos-5.4.6/python/voltha_protos/openolt_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/test/__init__.py` & `voltha-protos-5.4.6/python/test/__init__.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/test/test_protos.py` & `voltha-protos-5.4.6/python/test/test_protos.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.5/python/voltha_protos.egg-info/PKG-INFO` & `voltha-protos-5.4.6/python/voltha_protos.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: voltha-protos
-Version: 5.4.5
+Version: 5.4.6
 Summary: Protobuf interface definitions
 Home-page: https://gerrit.opencord.org/gitweb?p=voltha-protos.git
 Author: VOLTHA project
 Author-email: voltha-dev@opencord.org
 License: Apache Software License
 Description: UNKNOWN
 Keywords: protobuf voltha
```

### Comparing `voltha-protos-5.4.5/python/voltha_protos.egg-info/SOURCES.txt` & `voltha-protos-5.4.6/python/voltha_protos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py
 python/voltha_protos/openflow_13_pb2.py
 python/voltha_protos/openflow_13_pb2_grpc.py
 python/voltha_protos/openolt_pb2.py
 python/voltha_protos/openolt_pb2_grpc.py
 python/voltha_protos/tech_profile_pb2.py
 python/voltha_protos/tech_profile_pb2_grpc.py
+python/voltha_protos/voip_system_profile_pb2.py
+python/voltha_protos/voip_system_profile_pb2_grpc.py
+python/voltha_protos/voip_user_profile_pb2.py
+python/voltha_protos/voip_user_profile_pb2_grpc.py
 python/voltha_protos/voltha_pb2.py
 python/voltha_protos/voltha_pb2_grpc.py
 python/voltha_protos.egg-info/PKG-INFO
 python/voltha_protos.egg-info/SOURCES.txt
 python/voltha_protos.egg-info/dependency_links.txt
 python/voltha_protos.egg-info/requires.txt
 python/voltha_protos.egg-info/top_level.txt
```

