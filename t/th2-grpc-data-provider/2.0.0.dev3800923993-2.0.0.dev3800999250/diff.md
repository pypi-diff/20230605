# Comparing `tmp/th2_grpc_data_provider-2.0.0.dev3800923993.tar.gz` & `tmp/th2_grpc_data_provider-2.0.0.dev3800999250.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_data_provider-2.0.0.dev3800923993.tar", last modified: Thu Dec 29 13:41:26 2022, max compression
+gzip compressed data, was "dist/th2_grpc_data_provider-2.0.0.dev3800999250.tar", last modified: Thu Dec 29 13:57:48 2022, max compression
```

## Comparing `th2_grpc_data_provider-2.0.0.dev3800923993.tar` & `th2_grpc_data_provider-2.0.0.dev3800999250.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2359 2022-12-29 13:40:45.000000 th2_grpc_data_provider-2.0.0.dev3800923993/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-12-29 13:40:45.000000 th2_grpc_data_provider-2.0.0.dev3800923993/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2022-12-29 13:40:45.000000 th2_grpc_data_provider-2.0.0.dev3800923993/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11521 2022-12-29 13:40:45.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider.proto
--rw-r--r--   0 runner    (1001) docker     (122)    13838 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    40405 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    26015 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2096 2022-12-29 13:41:07.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider_service.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2022-12-29 13:40:45.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_data_provider.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4444 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_data_provider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     8667 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_data_provider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     4941 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_data_provider_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2022-12-29 13:41:07.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_provider_service_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      823 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2022-12-29 13:41:26.000000 th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2359 2022-12-29 13:57:05.000000 th2_grpc_data_provider-2.0.0.dev3800999250/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2022-12-29 13:57:06.000000 th2_grpc_data_provider-2.0.0.dev3800999250/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2022-12-29 13:57:05.000000 th2_grpc_data_provider-2.0.0.dev3800999250/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12903 2022-12-29 13:57:05.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    16338 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48461 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    27923 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2249 2022-12-29 13:57:28.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2022-12-29 13:57:05.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_data_provider.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4444 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_data_provider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8667 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_data_provider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     4941 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_data_provider_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2022-12-29 13:57:28.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_provider_service_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2022-12-29 13:57:48.000000 th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider.egg-info/top_level.txt
```

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/PKG-INFO` & `th2_grpc_data_provider-2.0.0.dev3800999250/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_data_provider
-Version: 2.0.0.dev3800923993
+Version: 2.0.0.dev3800999250
 Summary: th2_grpc_data_provider
 Home-page: https://github.com/th2-net/th2-data-provider
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC generator template library
```

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/README.md` & `th2_grpc_data_provider-2.0.0.dev3800999250/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/setup.py` & `th2_grpc_data_provider-2.0.0.dev3800999250/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider.proto` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider.proto`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,18 @@
   rpc searchMessages (MessageSearchRequest) returns (stream MessageSearchResponse) {
   }
 
   /* creates an event or an event metadata stream that matches the filter. */
   rpc searchEvents (EventSearchRequest) returns (stream EventSearchResponse) {
   }
 
+  rpc loadCradleMessageGroups (CradleMessageGroupsRequest) returns (CradleMessageGroupsResponse) {
+
+  }
+
   /*
   Searches for messages groups in specified timestamp
    */
   rpc searchMessageGroups (MessageGroupsSearchRequest) returns (stream MessageSearchResponse){
   }
 
   /* returns available message filters */
@@ -84,24 +88,61 @@
   }
 
   /* checks if the specified message matches the filter */
   rpc matchMessage (MessageMatchRequest) returns (MatchResponse) {
   }
 }
 
+message CradleMessageGroupsRequest {
+  google.protobuf.Timestamp start_timestamp = 1;
+  google.protobuf.Timestamp end_timestamp = 2;
+  repeated Group message_group = 3;
+  string external_user_queue = 4;
+  google.protobuf.BoolValue sort = 6;
+}
+
 // The scope for events to request
 message EventScope {
   string name = 1;
 }
 
 message BookId {
   // Name of the book to request data from
   string name = 1;
 }
 
+message MessageStreamInfo {
+  // string group TODO: this field isn't required because session_alias is unique for Cradle
+  string session_alias = 1;
+  Direction direction = 2;
+
+  int64 number_of_messages = 3;
+  google.protobuf.Timestamp max_timestamp = 4;
+  google.protobuf.Timestamp min_timestamp = 5;
+  int64 max_sequence = 6;
+  int64 min_sequence = 7;
+}
+
+message MessageIntervalInfo {
+  google.protobuf.Timestamp start_timestamp = 1;
+  google.protobuf.Timestamp end_timestamp = 2;
+
+  repeated MessageStreamInfo messages_info = 3;
+}
+
+message CradleMessageGroupsResponse {
+  oneof kind {
+      MessageIntervalInfo message_interval_info = 1;
+  }
+}
+
+message Group {
+  string name = 1;
+}
+
 message MessageGroupsSearchRequest {
   message Group {
     string name = 1;
   }
   google.protobuf.Timestamp start_timestamp = 1;
   google.protobuf.Timestamp end_timestamp = 2;
   BookId book_id = 7;
@@ -282,14 +323,25 @@
 
   repeated Filter filter = 8; // List of message search filters. (See 'search/sse/message' HTTP method https://github.com/th2-net/th2-rpt-data-provider)
   google.protobuf.BoolValue attached_events = 9; // If true, it will additionally load attachedEventsIds. Set by default to false.
   repeated string response_formats = 10; // List of possible response formats (e.g. PARSED or BASE_64)
   BookId book_id = 11;
 }
 
+message MessageGroupsSearchResponse {
+  oneof data {
+    MessageGroupCollectionResponse collection = 1; //TODO: move to MessageSearchResponse
+    MessageStreamPointers message_stream_pointers = 2;
+  }
+}
+
+message MessageGroupCollectionResponse {
+  repeated MessageGroupResponse messages = 1;
+}
+
 message MessageSearchResponse {
   oneof data {
     MessageGroupResponse message = 1;
     MessageStreamPointers message_stream_pointers = 2;
   }
 }
```

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider_pb2.py` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,90 +13,104 @@
 
 from th2_grpc_common import common_pb2 as th2__grpc__common_dot_common__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*th2_grpc_data_provider/data_provider.proto\x12\x11th2.data_provider\x1a\x1cth2_grpc_common/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x1a\n\nEventScope\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x16\n\x06\x42ookId\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xe2\x02\n\x1aMessageGroupsSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x07\x62ook_id\x18\x07 \x01(\x0b\x32\x19.th2.data_provider.BookId\x12J\n\rmessage_group\x18\x03 \x03(\x0b\x32\x33.th2.data_provider.MessageGroupsSearchRequest.Group\x12(\n\x04sort\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x10\n\x08raw_only\x18\x05 \x01(\x08\x12\x11\n\tkeep_open\x18\x06 \x01(\x08\x1a\x15\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\"C\n\x15MessageStreamsRequest\x12*\n\x07\x62ook_id\x18\x01 \x01(\x0b\x32\x19.th2.data_provider.BookId\"\x17\n\x15MessageFiltersRequest\"\x15\n\x13\x45ventFiltersRequest\"\xe3\x02\n\rEventResponse\x12\x1a\n\x08\x65vent_id\x18\x01 \x01(\x0b\x32\x08.EventID\x12!\n\x0fparent_event_id\x18\x02 \x01(\x0b\x32\x08.EventID\x12\x1a\n\x08\x62\x61tch_id\x18\x03 \x01(\x0b\x32\x08.EventID\x12\x12\n\nis_batched\x18\x04 \x01(\x08\x12\x33\n\x0fstart_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x06status\x18\x07 \x01(\x0e\x32\x0c.EventStatus\x12\x12\n\nevent_name\x18\x08 \x01(\t\x12\x12\n\nevent_type\x18\t \x01(\t\x12\x0c\n\x04\x62ody\x18\n \x01(\x0c\x12\'\n\x13\x61ttached_message_id\x18\x0b \x03(\x0b\x32\n.MessageID\"\xc9\x01\n\rEventMetadata\x12\x1a\n\x08\x65vent_id\x18\x01 \x01(\x0b\x32\x08.EventID\x12!\n\x0fparent_event_id\x18\x02 \x01(\x0b\x32\x08.EventID\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x06status\x18\x04 \x01(\x0e\x32\x0c.EventStatus\x12\x12\n\nevent_name\x18\x05 \x01(\t\x12\x12\n\nevent_type\x18\x06 \x01(\t\"(\n\x10\x42ulkEventRequest\x12\x14\n\x02id\x18\x01 \x03(\x0b\x32\x08.EventID\"D\n\x11\x42ulkEventResponse\x12/\n\x05\x65vent\x18\x01 \x03(\x0b\x32 .th2.data_provider.EventResponse\"<\n\x10MessageGroupItem\x12\x19\n\x07message\x18\x01 \x01(\x0b\x32\x08.Message\x12\r\n\x05match\x18\x02 \x01(\x08\"\xfd\x01\n\x14MessageGroupResponse\x12\x1e\n\nmessage_id\x18\x01 \x01(\x0b\x32\n.MessageID\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x08\x62ody_raw\x18\x03 \x01(\x0c\x42\x02\x18\x01\x12 \n\x0braw_message\x18\x06 \x01(\x0b\x32\x0b.RawMessage\x12#\n\x11\x61ttached_event_id\x18\x04 \x03(\x0b\x32\x08.EventID\x12\x39\n\x0cmessage_item\x18\x05 \x03(\x0b\x32#.th2.data_provider.MessageGroupItem\"G\n\x11\x46ilterInfoRequest\x12\x32\n\x0b\x66ilter_name\x18\x01 \x01(\x0b\x32\x1d.th2.data_provider.FilterName\"\x1a\n\nFilterName\x12\x0c\n\x04name\x18\x01 \x01(\t\"I\n\x13\x46ilterNamesResponse\x12\x32\n\x0b\x66ilter_name\x18\x01 \x03(\x0b\x32\x1d.th2.data_provider.FilterName\"\x90\x01\n\x0f\x46ilterParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x34\n\x04type\x18\x02 \x01(\x0e\x32&.th2.data_provider.FilterParameterType\x12+\n\rdefault_value\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x0c\n\x04hint\x18\x04 \x01(\t\"\x86\x01\n\x12\x46ilterInfoResponse\x12+\n\x04name\x18\x01 \x01(\x0b\x32\x1d.th2.data_provider.FilterName\x12\x0c\n\x04hint\x18\x02 \x01(\t\x12\x35\n\tparameter\x18\x03 \x03(\x0b\x32\".th2.data_provider.FilterParameter\"`\n\x13MessageMatchRequest\x12\x1e\n\nmessage_id\x18\x01 \x01(\x0b\x32\n.MessageID\x12)\n\x06\x66ilter\x18\x02 \x03(\x0b\x32\x19.th2.data_provider.Filter\"Z\n\x11\x45ventMatchRequest\x12\x1a\n\x08\x65vent_id\x18\x01 \x01(\x0b\x32\x08.EventID\x12)\n\x06\x66ilter\x18\x02 \x03(\x0b\x32\x19.th2.data_provider.Filter\"\x1e\n\rMatchResponse\x12\r\n\x05match\x18\x01 \x01(\x08\"h\n\x06\x46ilter\x12+\n\x04name\x18\x01 \x01(\x0b\x32\x1d.th2.data_provider.FilterName\x12\x10\n\x08negative\x18\x02 \x01(\x08\x12\r\n\x05value\x18\x03 \x03(\t\x12\x10\n\x08\x63onjunct\x18\x04 \x01(\x08\"\x87\x05\n\x12\x45ventSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x0cparent_event\x18\x03 \x01(\x0b\x32\x08.EventID\x12\x39\n\x10search_direction\x18\x04 \x01(\x0e\x32\x1f.th2.data_provider.TimeRelation\x12 \n\x0eresume_from_id\x18\x05 \x01(\x0b\x32\x08.EventID\x12\x37\n\x12result_count_limit\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12-\n\tkeep_open\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x10limit_for_parent\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\x31\n\rmetadata_only\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x11\x61ttached_messages\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12)\n\x06\x66ilter\x18\x0b \x03(\x0b\x32\x19.th2.data_provider.Filter\x12*\n\x07\x62ook_id\x18\x0c \x01(\x0b\x32\x19.th2.data_provider.BookId\x12,\n\x05scope\x18\r \x01(\x0b\x32\x1d.th2.data_provider.EventScope\"\xd3\x01\n\x13\x45ventSearchResponse\x12\x31\n\x05\x65vent\x18\x01 \x01(\x0b\x32 .th2.data_provider.EventResponseH\x00\x12:\n\x0e\x65vent_metadata\x18\x02 \x01(\x0b\x32 .th2.data_provider.EventMetadataH\x00\x12\x45\n\x14\x65vent_stream_pointer\x18\x03 \x01(\x0b\x32%.th2.data_provider.EventStreamPointerH\x00\x42\x06\n\x04\x64\x61ta\"W\n\x12\x45ventStreamPointer\x12\x13\n\x0bhas_started\x18\x01 \x01(\x08\x12\x11\n\thas_ended\x18\x02 \x01(\x08\x12\x19\n\x07last_id\x18\x03 \x01(\x0b\x32\x08.EventID\"\xba\x04\n\x14MessageSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x10search_direction\x18\x03 \x01(\x0e\x32\x1f.th2.data_provider.TimeRelation\x12\x37\n\x12result_count_limit\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x30\n\x06stream\x18\x05 \x03(\x0b\x32 .th2.data_provider.MessageStream\x12-\n\tkeep_open\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0estream_pointer\x18\x07 \x03(\x0b\x32\'.th2.data_provider.MessageStreamPointer\x12)\n\x06\x66ilter\x18\x08 \x03(\x0b\x32\x19.th2.data_provider.Filter\x12\x33\n\x0f\x61ttached_events\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x18\n\x10response_formats\x18\n \x03(\t\x12*\n\x07\x62ook_id\x18\x0b \x01(\x0b\x32\x19.th2.data_provider.BookId\"\xa8\x01\n\x15MessageSearchResponse\x12:\n\x07message\x18\x01 \x01(\x0b\x32\'.th2.data_provider.MessageGroupResponseH\x00\x12K\n\x17message_stream_pointers\x18\x02 \x01(\x0b\x32(.th2.data_provider.MessageStreamPointersH\x00\x42\x06\n\x04\x64\x61ta\"`\n\x15MessageStreamPointers\x12G\n\x16message_stream_pointer\x18\x01 \x03(\x0b\x32\'.th2.data_provider.MessageStreamPointer\"\x95\x01\n\x14MessageStreamPointer\x12\x38\n\x0emessage_stream\x18\x01 \x01(\x0b\x32 .th2.data_provider.MessageStream\x12\x13\n\x0bhas_started\x18\x02 \x01(\x08\x12\x11\n\thas_ended\x18\x03 \x01(\x08\x12\x1b\n\x07last_id\x18\x04 \x01(\x0b\x32\n.MessageID\"<\n\rMessageStream\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\tdirection\x18\x02 \x01(\x0e\x32\n.Direction\"R\n\x16MessageStreamsResponse\x12\x38\n\x0emessage_stream\x18\x01 \x03(\x0b\x32 .th2.data_provider.MessageStream\"\x0e\n\x0c\x42ooksRequest\"<\n\rBooksResponse\x12+\n\x08\x62ook_ids\x18\x01 \x03(\x0b\x32\x19.th2.data_provider.BookId*K\n\x13\x46ilterParameterType\x12\n\n\x06NUMBER\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\n\n\x06STRING\x10\x02\x12\x0f\n\x0bSTRING_LIST\x10\x03*&\n\x0cTimeRelation\x12\x08\n\x04NEXT\x10\x00\x12\x0c\n\x08PREVIOUS\x10\x01\x32\xb4\n\n\x0c\x44\x61taProvider\x12\x38\n\x08getEvent\x12\x08.EventID\x1a .th2.data_provider.EventResponse\"\x00\x12X\n\tgetEvents\x12#.th2.data_provider.BulkEventRequest\x1a$.th2.data_provider.BulkEventResponse\"\x00\x12\x43\n\ngetMessage\x12\n.MessageID\x1a\'.th2.data_provider.MessageGroupResponse\"\x00\x12j\n\x11getMessageStreams\x12(.th2.data_provider.MessageStreamsRequest\x1a).th2.data_provider.MessageStreamsResponse\"\x00\x12O\n\x08getBooks\x12\x1f.th2.data_provider.BooksRequest\x1a .th2.data_provider.BooksResponse\"\x00\x12g\n\x0esearchMessages\x12\'.th2.data_provider.MessageSearchRequest\x1a(.th2.data_provider.MessageSearchResponse\"\x00\x30\x01\x12\x61\n\x0csearchEvents\x12%.th2.data_provider.EventSearchRequest\x1a&.th2.data_provider.EventSearchResponse\"\x00\x30\x01\x12r\n\x13searchMessageGroups\x12-.th2.data_provider.MessageGroupsSearchRequest\x1a(.th2.data_provider.MessageSearchResponse\"\x00\x30\x01\x12h\n\x12getMessagesFilters\x12(.th2.data_provider.MessageFiltersRequest\x1a&.th2.data_provider.FilterNamesResponse\"\x00\x12\x64\n\x10getEventsFilters\x12&.th2.data_provider.EventFiltersRequest\x1a&.th2.data_provider.FilterNamesResponse\"\x00\x12\x63\n\x12getEventFilterInfo\x12$.th2.data_provider.FilterInfoRequest\x1a%.th2.data_provider.FilterInfoResponse\"\x00\x12\x65\n\x14getMessageFilterInfo\x12$.th2.data_provider.FilterInfoRequest\x1a%.th2.data_provider.FilterInfoResponse\"\x00\x12V\n\nmatchEvent\x12$.th2.data_provider.EventMatchRequest\x1a .th2.data_provider.MatchResponse\"\x00\x12Z\n\x0cmatchMessage\x12&.th2.data_provider.MessageMatchRequest\x1a .th2.data_provider.MatchResponse\"\x00\x42&\n\"com.exactpro.th2.dataprovider.grpcP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*th2_grpc_data_provider/data_provider.proto\x12\x11th2.data_provider\x1a\x1cth2_grpc_common/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xfc\x01\n\x1a\x43radleMessageGroupsRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\rmessage_group\x18\x03 \x03(\x0b\x32\x18.th2.data_provider.Group\x12\x1b\n\x13\x65xternal_user_queue\x18\x04 \x01(\t\x12(\n\x04sort\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\x1a\n\nEventScope\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x16\n\x06\x42ookId\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xf7\x01\n\x11MessageStreamInfo\x12\x15\n\rsession_alias\x18\x01 \x01(\t\x12\x1d\n\tdirection\x18\x02 \x01(\x0e\x32\n.Direction\x12\x1a\n\x12number_of_messages\x18\x03 \x01(\x03\x12\x31\n\rmax_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rmin_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0cmax_sequence\x18\x06 \x01(\x03\x12\x14\n\x0cmin_sequence\x18\x07 \x01(\x03\"\xba\x01\n\x13MessageIntervalInfo\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\rmessages_info\x18\x03 \x03(\x0b\x32$.th2.data_provider.MessageStreamInfo\"n\n\x1b\x43radleMessageGroupsResponse\x12G\n\x15message_interval_info\x18\x01 \x01(\x0b\x32&.th2.data_provider.MessageIntervalInfoH\x00\x42\x06\n\x04kind\"\x15\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xe2\x02\n\x1aMessageGroupsSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x07\x62ook_id\x18\x07 \x01(\x0b\x32\x19.th2.data_provider.BookId\x12J\n\rmessage_group\x18\x03 \x03(\x0b\x32\x33.th2.data_provider.MessageGroupsSearchRequest.Group\x12(\n\x04sort\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x10\n\x08raw_only\x18\x05 \x01(\x08\x12\x11\n\tkeep_open\x18\x06 \x01(\x08\x1a\x15\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\"C\n\x15MessageStreamsRequest\x12*\n\x07\x62ook_id\x18\x01 \x01(\x0b\x32\x19.th2.data_provider.BookId\"\x17\n\x15MessageFiltersRequest\"\x15\n\x13\x45ventFiltersRequest\"\xe3\x02\n\rEventResponse\x12\x1a\n\x08\x65vent_id\x18\x01 \x01(\x0b\x32\x08.EventID\x12!\n\x0fparent_event_id\x18\x02 \x01(\x0b\x32\x08.EventID\x12\x1a\n\x08\x62\x61tch_id\x18\x03 \x01(\x0b\x32\x08.EventID\x12\x12\n\nis_batched\x18\x04 \x01(\x08\x12\x33\n\x0fstart_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x06status\x18\x07 \x01(\x0e\x32\x0c.EventStatus\x12\x12\n\nevent_name\x18\x08 \x01(\t\x12\x12\n\nevent_type\x18\t \x01(\t\x12\x0c\n\x04\x62ody\x18\n \x01(\x0c\x12\'\n\x13\x61ttached_message_id\x18\x0b \x03(\x0b\x32\n.MessageID\"\xc9\x01\n\rEventMetadata\x12\x1a\n\x08\x65vent_id\x18\x01 \x01(\x0b\x32\x08.EventID\x12!\n\x0fparent_event_id\x18\x02 \x01(\x0b\x32\x08.EventID\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x06status\x18\x04 \x01(\x0e\x32\x0c.EventStatus\x12\x12\n\nevent_name\x18\x05 \x01(\t\x12\x12\n\nevent_type\x18\x06 \x01(\t\"(\n\x10\x42ulkEventRequest\x12\x14\n\x02id\x18\x01 \x03(\x0b\x32\x08.EventID\"D\n\x11\x42ulkEventResponse\x12/\n\x05\x65vent\x18\x01 \x03(\x0b\x32 .th2.data_provider.EventResponse\"<\n\x10MessageGroupItem\x12\x19\n\x07message\x18\x01 \x01(\x0b\x32\x08.Message\x12\r\n\x05match\x18\x02 \x01(\x08\"\xfd\x01\n\x14MessageGroupResponse\x12\x1e\n\nmessage_id\x18\x01 \x01(\x0b\x32\n.MessageID\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x08\x62ody_raw\x18\x03 \x01(\x0c\x42\x02\x18\x01\x12 \n\x0braw_message\x18\x06 \x01(\x0b\x32\x0b.RawMessage\x12#\n\x11\x61ttached_event_id\x18\x04 \x03(\x0b\x32\x08.EventID\x12\x39\n\x0cmessage_item\x18\x05 \x03(\x0b\x32#.th2.data_provider.MessageGroupItem\"G\n\x11\x46ilterInfoRequest\x12\x32\n\x0b\x66ilter_name\x18\x01 \x01(\x0b\x32\x1d.th2.data_provider.FilterName\"\x1a\n\nFilterName\x12\x0c\n\x04name\x18\x01 \x01(\t\"I\n\x13\x46ilterNamesResponse\x12\x32\n\x0b\x66ilter_name\x18\x01 \x03(\x0b\x32\x1d.th2.data_provider.FilterName\"\x90\x01\n\x0f\x46ilterParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x34\n\x04type\x18\x02 \x01(\x0e\x32&.th2.data_provider.FilterParameterType\x12+\n\rdefault_value\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x0c\n\x04hint\x18\x04 \x01(\t\"\x86\x01\n\x12\x46ilterInfoResponse\x12+\n\x04name\x18\x01 \x01(\x0b\x32\x1d.th2.data_provider.FilterName\x12\x0c\n\x04hint\x18\x02 \x01(\t\x12\x35\n\tparameter\x18\x03 \x03(\x0b\x32\".th2.data_provider.FilterParameter\"`\n\x13MessageMatchRequest\x12\x1e\n\nmessage_id\x18\x01 \x01(\x0b\x32\n.MessageID\x12)\n\x06\x66ilter\x18\x02 \x03(\x0b\x32\x19.th2.data_provider.Filter\"Z\n\x11\x45ventMatchRequest\x12\x1a\n\x08\x65vent_id\x18\x01 \x01(\x0b\x32\x08.EventID\x12)\n\x06\x66ilter\x18\x02 \x03(\x0b\x32\x19.th2.data_provider.Filter\"\x1e\n\rMatchResponse\x12\r\n\x05match\x18\x01 \x01(\x08\"h\n\x06\x46ilter\x12+\n\x04name\x18\x01 \x01(\x0b\x32\x1d.th2.data_provider.FilterName\x12\x10\n\x08negative\x18\x02 \x01(\x08\x12\r\n\x05value\x18\x03 \x03(\t\x12\x10\n\x08\x63onjunct\x18\x04 \x01(\x08\"\x87\x05\n\x12\x45ventSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x0cparent_event\x18\x03 \x01(\x0b\x32\x08.EventID\x12\x39\n\x10search_direction\x18\x04 \x01(\x0e\x32\x1f.th2.data_provider.TimeRelation\x12 \n\x0eresume_from_id\x18\x05 \x01(\x0b\x32\x08.EventID\x12\x37\n\x12result_count_limit\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12-\n\tkeep_open\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x10limit_for_parent\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\x31\n\rmetadata_only\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x11\x61ttached_messages\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12)\n\x06\x66ilter\x18\x0b \x03(\x0b\x32\x19.th2.data_provider.Filter\x12*\n\x07\x62ook_id\x18\x0c \x01(\x0b\x32\x19.th2.data_provider.BookId\x12,\n\x05scope\x18\r \x01(\x0b\x32\x1d.th2.data_provider.EventScope\"\xd3\x01\n\x13\x45ventSearchResponse\x12\x31\n\x05\x65vent\x18\x01 \x01(\x0b\x32 .th2.data_provider.EventResponseH\x00\x12:\n\x0e\x65vent_metadata\x18\x02 \x01(\x0b\x32 .th2.data_provider.EventMetadataH\x00\x12\x45\n\x14\x65vent_stream_pointer\x18\x03 \x01(\x0b\x32%.th2.data_provider.EventStreamPointerH\x00\x42\x06\n\x04\x64\x61ta\"W\n\x12\x45ventStreamPointer\x12\x13\n\x0bhas_started\x18\x01 \x01(\x08\x12\x11\n\thas_ended\x18\x02 \x01(\x08\x12\x19\n\x07last_id\x18\x03 \x01(\x0b\x32\x08.EventID\"\xba\x04\n\x14MessageSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x10search_direction\x18\x03 \x01(\x0e\x32\x1f.th2.data_provider.TimeRelation\x12\x37\n\x12result_count_limit\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x30\n\x06stream\x18\x05 \x03(\x0b\x32 .th2.data_provider.MessageStream\x12-\n\tkeep_open\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0estream_pointer\x18\x07 \x03(\x0b\x32\'.th2.data_provider.MessageStreamPointer\x12)\n\x06\x66ilter\x18\x08 \x03(\x0b\x32\x19.th2.data_provider.Filter\x12\x33\n\x0f\x61ttached_events\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x18\n\x10response_formats\x18\n \x03(\t\x12*\n\x07\x62ook_id\x18\x0b \x01(\x0b\x32\x19.th2.data_provider.BookId\"\xbb\x01\n\x1bMessageGroupsSearchResponse\x12G\n\ncollection\x18\x01 \x01(\x0b\x32\x31.th2.data_provider.MessageGroupCollectionResponseH\x00\x12K\n\x17message_stream_pointers\x18\x02 \x01(\x0b\x32(.th2.data_provider.MessageStreamPointersH\x00\x42\x06\n\x04\x64\x61ta\"[\n\x1eMessageGroupCollectionResponse\x12\x39\n\x08messages\x18\x01 \x03(\x0b\x32\'.th2.data_provider.MessageGroupResponse\"\xa8\x01\n\x15MessageSearchResponse\x12:\n\x07message\x18\x01 \x01(\x0b\x32\'.th2.data_provider.MessageGroupResponseH\x00\x12K\n\x17message_stream_pointers\x18\x02 \x01(\x0b\x32(.th2.data_provider.MessageStreamPointersH\x00\x42\x06\n\x04\x64\x61ta\"`\n\x15MessageStreamPointers\x12G\n\x16message_stream_pointer\x18\x01 \x03(\x0b\x32\'.th2.data_provider.MessageStreamPointer\"\x95\x01\n\x14MessageStreamPointer\x12\x38\n\x0emessage_stream\x18\x01 \x01(\x0b\x32 .th2.data_provider.MessageStream\x12\x13\n\x0bhas_started\x18\x02 \x01(\x08\x12\x11\n\thas_ended\x18\x03 \x01(\x08\x12\x1b\n\x07last_id\x18\x04 \x01(\x0b\x32\n.MessageID\"<\n\rMessageStream\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\tdirection\x18\x02 \x01(\x0e\x32\n.Direction\"R\n\x16MessageStreamsResponse\x12\x38\n\x0emessage_stream\x18\x01 \x03(\x0b\x32 .th2.data_provider.MessageStream\"\x0e\n\x0c\x42ooksRequest\"<\n\rBooksResponse\x12+\n\x08\x62ook_ids\x18\x01 \x03(\x0b\x32\x19.th2.data_provider.BookId*K\n\x13\x46ilterParameterType\x12\n\n\x06NUMBER\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\n\n\x06STRING\x10\x02\x12\x0f\n\x0bSTRING_LIST\x10\x03*&\n\x0cTimeRelation\x12\x08\n\x04NEXT\x10\x00\x12\x0c\n\x08PREVIOUS\x10\x01\x32\xb0\x0b\n\x0c\x44\x61taProvider\x12\x38\n\x08getEvent\x12\x08.EventID\x1a .th2.data_provider.EventResponse\"\x00\x12X\n\tgetEvents\x12#.th2.data_provider.BulkEventRequest\x1a$.th2.data_provider.BulkEventResponse\"\x00\x12\x43\n\ngetMessage\x12\n.MessageID\x1a\'.th2.data_provider.MessageGroupResponse\"\x00\x12j\n\x11getMessageStreams\x12(.th2.data_provider.MessageStreamsRequest\x1a).th2.data_provider.MessageStreamsResponse\"\x00\x12O\n\x08getBooks\x12\x1f.th2.data_provider.BooksRequest\x1a .th2.data_provider.BooksResponse\"\x00\x12g\n\x0esearchMessages\x12\'.th2.data_provider.MessageSearchRequest\x1a(.th2.data_provider.MessageSearchResponse\"\x00\x30\x01\x12\x61\n\x0csearchEvents\x12%.th2.data_provider.EventSearchRequest\x1a&.th2.data_provider.EventSearchResponse\"\x00\x30\x01\x12z\n\x17loadCradleMessageGroups\x12-.th2.data_provider.CradleMessageGroupsRequest\x1a..th2.data_provider.CradleMessageGroupsResponse\"\x00\x12r\n\x13searchMessageGroups\x12-.th2.data_provider.MessageGroupsSearchRequest\x1a(.th2.data_provider.MessageSearchResponse\"\x00\x30\x01\x12h\n\x12getMessagesFilters\x12(.th2.data_provider.MessageFiltersRequest\x1a&.th2.data_provider.FilterNamesResponse\"\x00\x12\x64\n\x10getEventsFilters\x12&.th2.data_provider.EventFiltersRequest\x1a&.th2.data_provider.FilterNamesResponse\"\x00\x12\x63\n\x12getEventFilterInfo\x12$.th2.data_provider.FilterInfoRequest\x1a%.th2.data_provider.FilterInfoResponse\"\x00\x12\x65\n\x14getMessageFilterInfo\x12$.th2.data_provider.FilterInfoRequest\x1a%.th2.data_provider.FilterInfoResponse\"\x00\x12V\n\nmatchEvent\x12$.th2.data_provider.EventMatchRequest\x1a .th2.data_provider.MatchResponse\"\x00\x12Z\n\x0cmatchMessage\x12&.th2.data_provider.MessageMatchRequest\x1a .th2.data_provider.MatchResponse\"\x00\x42&\n\"com.exactpro.th2.dataprovider.grpcP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'th2_grpc_data_provider.data_provider_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\"com.exactpro.th2.dataprovider.grpcP\001'
   _MESSAGEGROUPRESPONSE.fields_by_name['body_raw']._options = None
   _MESSAGEGROUPRESPONSE.fields_by_name['body_raw']._serialized_options = b'\030\001'
-  _FILTERPARAMETERTYPE._serialized_start=4664
-  _FILTERPARAMETERTYPE._serialized_end=4739
-  _TIMERELATION._serialized_start=4741
-  _TIMERELATION._serialized_end=4779
-  _EVENTSCOPE._serialized_start=187
-  _EVENTSCOPE._serialized_end=213
-  _BOOKID._serialized_start=215
-  _BOOKID._serialized_end=237
-  _MESSAGEGROUPSSEARCHREQUEST._serialized_start=240
-  _MESSAGEGROUPSSEARCHREQUEST._serialized_end=594
-  _MESSAGEGROUPSSEARCHREQUEST_GROUP._serialized_start=573
-  _MESSAGEGROUPSSEARCHREQUEST_GROUP._serialized_end=594
-  _MESSAGESTREAMSREQUEST._serialized_start=596
-  _MESSAGESTREAMSREQUEST._serialized_end=663
-  _MESSAGEFILTERSREQUEST._serialized_start=665
-  _MESSAGEFILTERSREQUEST._serialized_end=688
-  _EVENTFILTERSREQUEST._serialized_start=690
-  _EVENTFILTERSREQUEST._serialized_end=711
-  _EVENTRESPONSE._serialized_start=714
-  _EVENTRESPONSE._serialized_end=1069
-  _EVENTMETADATA._serialized_start=1072
-  _EVENTMETADATA._serialized_end=1273
-  _BULKEVENTREQUEST._serialized_start=1275
-  _BULKEVENTREQUEST._serialized_end=1315
-  _BULKEVENTRESPONSE._serialized_start=1317
-  _BULKEVENTRESPONSE._serialized_end=1385
-  _MESSAGEGROUPITEM._serialized_start=1387
-  _MESSAGEGROUPITEM._serialized_end=1447
-  _MESSAGEGROUPRESPONSE._serialized_start=1450
-  _MESSAGEGROUPRESPONSE._serialized_end=1703
-  _FILTERINFOREQUEST._serialized_start=1705
-  _FILTERINFOREQUEST._serialized_end=1776
-  _FILTERNAME._serialized_start=1778
-  _FILTERNAME._serialized_end=1804
-  _FILTERNAMESRESPONSE._serialized_start=1806
-  _FILTERNAMESRESPONSE._serialized_end=1879
-  _FILTERPARAMETER._serialized_start=1882
-  _FILTERPARAMETER._serialized_end=2026
-  _FILTERINFORESPONSE._serialized_start=2029
-  _FILTERINFORESPONSE._serialized_end=2163
-  _MESSAGEMATCHREQUEST._serialized_start=2165
-  _MESSAGEMATCHREQUEST._serialized_end=2261
-  _EVENTMATCHREQUEST._serialized_start=2263
-  _EVENTMATCHREQUEST._serialized_end=2353
-  _MATCHRESPONSE._serialized_start=2355
-  _MATCHRESPONSE._serialized_end=2385
-  _FILTER._serialized_start=2387
-  _FILTER._serialized_end=2491
-  _EVENTSEARCHREQUEST._serialized_start=2494
-  _EVENTSEARCHREQUEST._serialized_end=3141
-  _EVENTSEARCHRESPONSE._serialized_start=3144
-  _EVENTSEARCHRESPONSE._serialized_end=3355
-  _EVENTSTREAMPOINTER._serialized_start=3357
-  _EVENTSTREAMPOINTER._serialized_end=3444
-  _MESSAGESEARCHREQUEST._serialized_start=3447
-  _MESSAGESEARCHREQUEST._serialized_end=4017
-  _MESSAGESEARCHRESPONSE._serialized_start=4020
-  _MESSAGESEARCHRESPONSE._serialized_end=4188
-  _MESSAGESTREAMPOINTERS._serialized_start=4190
-  _MESSAGESTREAMPOINTERS._serialized_end=4286
-  _MESSAGESTREAMPOINTER._serialized_start=4289
-  _MESSAGESTREAMPOINTER._serialized_end=4438
-  _MESSAGESTREAM._serialized_start=4440
-  _MESSAGESTREAM._serialized_end=4500
-  _MESSAGESTREAMSRESPONSE._serialized_start=4502
-  _MESSAGESTREAMSRESPONSE._serialized_end=4584
-  _BOOKSREQUEST._serialized_start=4586
-  _BOOKSREQUEST._serialized_end=4600
-  _BOOKSRESPONSE._serialized_start=4602
-  _BOOKSRESPONSE._serialized_end=4662
-  _DATAPROVIDER._serialized_start=4782
-  _DATAPROVIDER._serialized_end=6114
+  _FILTERPARAMETERTYPE._serialized_start=5776
+  _FILTERPARAMETERTYPE._serialized_end=5851
+  _TIMERELATION._serialized_start=5853
+  _TIMERELATION._serialized_end=5891
+  _CRADLEMESSAGEGROUPSREQUEST._serialized_start=188
+  _CRADLEMESSAGEGROUPSREQUEST._serialized_end=440
+  _EVENTSCOPE._serialized_start=442
+  _EVENTSCOPE._serialized_end=468
+  _BOOKID._serialized_start=470
+  _BOOKID._serialized_end=492
+  _MESSAGESTREAMINFO._serialized_start=495
+  _MESSAGESTREAMINFO._serialized_end=742
+  _MESSAGEINTERVALINFO._serialized_start=745
+  _MESSAGEINTERVALINFO._serialized_end=931
+  _CRADLEMESSAGEGROUPSRESPONSE._serialized_start=933
+  _CRADLEMESSAGEGROUPSRESPONSE._serialized_end=1043
+  _GROUP._serialized_start=1045
+  _GROUP._serialized_end=1066
+  _MESSAGEGROUPSSEARCHREQUEST._serialized_start=1069
+  _MESSAGEGROUPSSEARCHREQUEST._serialized_end=1423
+  _MESSAGEGROUPSSEARCHREQUEST_GROUP._serialized_start=1045
+  _MESSAGEGROUPSSEARCHREQUEST_GROUP._serialized_end=1066
+  _MESSAGESTREAMSREQUEST._serialized_start=1425
+  _MESSAGESTREAMSREQUEST._serialized_end=1492
+  _MESSAGEFILTERSREQUEST._serialized_start=1494
+  _MESSAGEFILTERSREQUEST._serialized_end=1517
+  _EVENTFILTERSREQUEST._serialized_start=1519
+  _EVENTFILTERSREQUEST._serialized_end=1540
+  _EVENTRESPONSE._serialized_start=1543
+  _EVENTRESPONSE._serialized_end=1898
+  _EVENTMETADATA._serialized_start=1901
+  _EVENTMETADATA._serialized_end=2102
+  _BULKEVENTREQUEST._serialized_start=2104
+  _BULKEVENTREQUEST._serialized_end=2144
+  _BULKEVENTRESPONSE._serialized_start=2146
+  _BULKEVENTRESPONSE._serialized_end=2214
+  _MESSAGEGROUPITEM._serialized_start=2216
+  _MESSAGEGROUPITEM._serialized_end=2276
+  _MESSAGEGROUPRESPONSE._serialized_start=2279
+  _MESSAGEGROUPRESPONSE._serialized_end=2532
+  _FILTERINFOREQUEST._serialized_start=2534
+  _FILTERINFOREQUEST._serialized_end=2605
+  _FILTERNAME._serialized_start=2607
+  _FILTERNAME._serialized_end=2633
+  _FILTERNAMESRESPONSE._serialized_start=2635
+  _FILTERNAMESRESPONSE._serialized_end=2708
+  _FILTERPARAMETER._serialized_start=2711
+  _FILTERPARAMETER._serialized_end=2855
+  _FILTERINFORESPONSE._serialized_start=2858
+  _FILTERINFORESPONSE._serialized_end=2992
+  _MESSAGEMATCHREQUEST._serialized_start=2994
+  _MESSAGEMATCHREQUEST._serialized_end=3090
+  _EVENTMATCHREQUEST._serialized_start=3092
+  _EVENTMATCHREQUEST._serialized_end=3182
+  _MATCHRESPONSE._serialized_start=3184
+  _MATCHRESPONSE._serialized_end=3214
+  _FILTER._serialized_start=3216
+  _FILTER._serialized_end=3320
+  _EVENTSEARCHREQUEST._serialized_start=3323
+  _EVENTSEARCHREQUEST._serialized_end=3970
+  _EVENTSEARCHRESPONSE._serialized_start=3973
+  _EVENTSEARCHRESPONSE._serialized_end=4184
+  _EVENTSTREAMPOINTER._serialized_start=4186
+  _EVENTSTREAMPOINTER._serialized_end=4273
+  _MESSAGESEARCHREQUEST._serialized_start=4276
+  _MESSAGESEARCHREQUEST._serialized_end=4846
+  _MESSAGEGROUPSSEARCHRESPONSE._serialized_start=4849
+  _MESSAGEGROUPSSEARCHRESPONSE._serialized_end=5036
+  _MESSAGEGROUPCOLLECTIONRESPONSE._serialized_start=5038
+  _MESSAGEGROUPCOLLECTIONRESPONSE._serialized_end=5129
+  _MESSAGESEARCHRESPONSE._serialized_start=5132
+  _MESSAGESEARCHRESPONSE._serialized_end=5300
+  _MESSAGESTREAMPOINTERS._serialized_start=5302
+  _MESSAGESTREAMPOINTERS._serialized_end=5398
+  _MESSAGESTREAMPOINTER._serialized_start=5401
+  _MESSAGESTREAMPOINTER._serialized_end=5550
+  _MESSAGESTREAM._serialized_start=5552
+  _MESSAGESTREAM._serialized_end=5612
+  _MESSAGESTREAMSRESPONSE._serialized_start=5614
+  _MESSAGESTREAMSRESPONSE._serialized_end=5696
+  _BOOKSREQUEST._serialized_start=5698
+  _BOOKSREQUEST._serialized_end=5712
+  _BOOKSRESPONSE._serialized_start=5714
+  _BOOKSRESPONSE._serialized_end=5774
+  _DATAPROVIDER._serialized_start=5894
+  _DATAPROVIDER._serialized_end=7350
 # @@protoc_insertion_point(module_scope)
```

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider_pb2.pyi` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -46,14 +46,42 @@
     pass
 
 NEXT: TimeRelation.ValueType  # 0
 PREVIOUS: TimeRelation.ValueType  # 1
 global___TimeRelation = TimeRelation
 
 
+class CradleMessageGroupsRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    START_TIMESTAMP_FIELD_NUMBER: builtins.int
+    END_TIMESTAMP_FIELD_NUMBER: builtins.int
+    MESSAGE_GROUP_FIELD_NUMBER: builtins.int
+    EXTERNAL_USER_QUEUE_FIELD_NUMBER: builtins.int
+    SORT_FIELD_NUMBER: builtins.int
+    @property
+    def start_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def end_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def message_group(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Group]: ...
+    external_user_queue: typing.Text
+    @property
+    def sort(self) -> google.protobuf.wrappers_pb2.BoolValue: ...
+    def __init__(self,
+        *,
+        start_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
+        end_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
+        message_group: typing.Optional[typing.Iterable[global___Group]] = ...,
+        external_user_queue: typing.Text = ...,
+        sort: typing.Optional[google.protobuf.wrappers_pb2.BoolValue] = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["end_timestamp",b"end_timestamp","sort",b"sort","start_timestamp",b"start_timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["end_timestamp",b"end_timestamp","external_user_queue",b"external_user_queue","message_group",b"message_group","sort",b"sort","start_timestamp",b"start_timestamp"]) -> None: ...
+global___CradleMessageGroupsRequest = CradleMessageGroupsRequest
+
 class EventScope(google.protobuf.message.Message):
     """The scope for events to request"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     NAME_FIELD_NUMBER: builtins.int
     name: typing.Text
     def __init__(self,
         *,
@@ -71,14 +99,94 @@
     def __init__(self,
         *,
         name: typing.Text = ...,
         ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 global___BookId = BookId
 
+class MessageStreamInfo(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    SESSION_ALIAS_FIELD_NUMBER: builtins.int
+    DIRECTION_FIELD_NUMBER: builtins.int
+    NUMBER_OF_MESSAGES_FIELD_NUMBER: builtins.int
+    MAX_TIMESTAMP_FIELD_NUMBER: builtins.int
+    MIN_TIMESTAMP_FIELD_NUMBER: builtins.int
+    MAX_SEQUENCE_FIELD_NUMBER: builtins.int
+    MIN_SEQUENCE_FIELD_NUMBER: builtins.int
+    session_alias: typing.Text
+    """string group TODO: this field isn't required because session_alias is unique for Cradle"""
+
+    direction: th2_grpc_common.common_pb2.Direction.ValueType
+    number_of_messages: builtins.int
+    @property
+    def max_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def min_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    max_sequence: builtins.int
+    min_sequence: builtins.int
+    def __init__(self,
+        *,
+        session_alias: typing.Text = ...,
+        direction: th2_grpc_common.common_pb2.Direction.ValueType = ...,
+        number_of_messages: builtins.int = ...,
+        max_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
+        min_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
+        max_sequence: builtins.int = ...,
+        min_sequence: builtins.int = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["max_timestamp",b"max_timestamp","min_timestamp",b"min_timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["direction",b"direction","max_sequence",b"max_sequence","max_timestamp",b"max_timestamp","min_sequence",b"min_sequence","min_timestamp",b"min_timestamp","number_of_messages",b"number_of_messages","session_alias",b"session_alias"]) -> None: ...
+global___MessageStreamInfo = MessageStreamInfo
+
+class MessageIntervalInfo(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    START_TIMESTAMP_FIELD_NUMBER: builtins.int
+    END_TIMESTAMP_FIELD_NUMBER: builtins.int
+    MESSAGES_INFO_FIELD_NUMBER: builtins.int
+    @property
+    def start_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def end_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def messages_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MessageStreamInfo]: ...
+    def __init__(self,
+        *,
+        start_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
+        end_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
+        messages_info: typing.Optional[typing.Iterable[global___MessageStreamInfo]] = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["end_timestamp",b"end_timestamp","start_timestamp",b"start_timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["end_timestamp",b"end_timestamp","messages_info",b"messages_info","start_timestamp",b"start_timestamp"]) -> None: ...
+global___MessageIntervalInfo = MessageIntervalInfo
+
+class CradleMessageGroupsResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    MESSAGE_INTERVAL_INFO_FIELD_NUMBER: builtins.int
+    @property
+    def message_interval_info(self) -> global___MessageIntervalInfo: ...
+    def __init__(self,
+        *,
+        message_interval_info: typing.Optional[global___MessageIntervalInfo] = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["kind",b"kind","message_interval_info",b"message_interval_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["kind",b"kind","message_interval_info",b"message_interval_info"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind",b"kind"]) -> typing.Optional[typing_extensions.Literal["message_interval_info"]]: ...
+global___CradleMessageGroupsResponse = CradleMessageGroupsResponse
+
+class Group(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    NAME_FIELD_NUMBER: builtins.int
+    name: typing.Text
+    def __init__(self,
+        *,
+        name: typing.Text = ...,
+        ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
+global___Group = Group
+
 class MessageGroupsSearchRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     class Group(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
         NAME_FIELD_NUMBER: builtins.int
         name: typing.Text
         def __init__(self,
@@ -670,14 +778,46 @@
         response_formats: typing.Optional[typing.Iterable[typing.Text]] = ...,
         book_id: typing.Optional[global___BookId] = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["attached_events",b"attached_events","book_id",b"book_id","end_timestamp",b"end_timestamp","keep_open",b"keep_open","result_count_limit",b"result_count_limit","start_timestamp",b"start_timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["attached_events",b"attached_events","book_id",b"book_id","end_timestamp",b"end_timestamp","filter",b"filter","keep_open",b"keep_open","response_formats",b"response_formats","result_count_limit",b"result_count_limit","search_direction",b"search_direction","start_timestamp",b"start_timestamp","stream",b"stream","stream_pointer",b"stream_pointer"]) -> None: ...
 global___MessageSearchRequest = MessageSearchRequest
 
+class MessageGroupsSearchResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    COLLECTION_FIELD_NUMBER: builtins.int
+    MESSAGE_STREAM_POINTERS_FIELD_NUMBER: builtins.int
+    @property
+    def collection(self) -> global___MessageGroupCollectionResponse:
+        """TODO: move to MessageSearchResponse"""
+        pass
+    @property
+    def message_stream_pointers(self) -> global___MessageStreamPointers: ...
+    def __init__(self,
+        *,
+        collection: typing.Optional[global___MessageGroupCollectionResponse] = ...,
+        message_stream_pointers: typing.Optional[global___MessageStreamPointers] = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["collection",b"collection","data",b"data","message_stream_pointers",b"message_stream_pointers"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["collection",b"collection","data",b"data","message_stream_pointers",b"message_stream_pointers"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["data",b"data"]) -> typing.Optional[typing_extensions.Literal["collection","message_stream_pointers"]]: ...
+global___MessageGroupsSearchResponse = MessageGroupsSearchResponse
+
+class MessageGroupCollectionResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    MESSAGES_FIELD_NUMBER: builtins.int
+    @property
+    def messages(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MessageGroupResponse]: ...
+    def __init__(self,
+        *,
+        messages: typing.Optional[typing.Iterable[global___MessageGroupResponse]] = ...,
+        ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["messages",b"messages"]) -> None: ...
+global___MessageGroupCollectionResponse = MessageGroupCollectionResponse
+
 class MessageSearchResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     MESSAGE_FIELD_NUMBER: builtins.int
     MESSAGE_STREAM_POINTERS_FIELD_NUMBER: builtins.int
     @property
     def message(self) -> global___MessageGroupResponse: ...
     @property
```

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider_pb2_grpc.py` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,19 @@
                 response_deserializer=th2__grpc__data__provider_dot_data__provider__pb2.MessageSearchResponse.FromString,
                 )
         self.searchEvents = channel.unary_stream(
                 '/th2.data_provider.DataProvider/searchEvents',
                 request_serializer=th2__grpc__data__provider_dot_data__provider__pb2.EventSearchRequest.SerializeToString,
                 response_deserializer=th2__grpc__data__provider_dot_data__provider__pb2.EventSearchResponse.FromString,
                 )
+        self.loadCradleMessageGroups = channel.unary_unary(
+                '/th2.data_provider.DataProvider/loadCradleMessageGroups',
+                request_serializer=th2__grpc__data__provider_dot_data__provider__pb2.CradleMessageGroupsRequest.SerializeToString,
+                response_deserializer=th2__grpc__data__provider_dot_data__provider__pb2.CradleMessageGroupsResponse.FromString,
+                )
         self.searchMessageGroups = channel.unary_stream(
                 '/th2.data_provider.DataProvider/searchMessageGroups',
                 request_serializer=th2__grpc__data__provider_dot_data__provider__pb2.MessageGroupsSearchRequest.SerializeToString,
                 response_deserializer=th2__grpc__data__provider_dot_data__provider__pb2.MessageSearchResponse.FromString,
                 )
         self.getMessagesFilters = channel.unary_unary(
                 '/th2.data_provider.DataProvider/getMessagesFilters',
@@ -135,14 +140,20 @@
     def searchEvents(self, request, context):
         """creates an event or an event metadata stream that matches the filter. 
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def loadCradleMessageGroups(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def searchMessageGroups(self, request, context):
         """
         Searches for messages groups in specified timestamp
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
@@ -223,14 +234,19 @@
                     response_serializer=th2__grpc__data__provider_dot_data__provider__pb2.MessageSearchResponse.SerializeToString,
             ),
             'searchEvents': grpc.unary_stream_rpc_method_handler(
                     servicer.searchEvents,
                     request_deserializer=th2__grpc__data__provider_dot_data__provider__pb2.EventSearchRequest.FromString,
                     response_serializer=th2__grpc__data__provider_dot_data__provider__pb2.EventSearchResponse.SerializeToString,
             ),
+            'loadCradleMessageGroups': grpc.unary_unary_rpc_method_handler(
+                    servicer.loadCradleMessageGroups,
+                    request_deserializer=th2__grpc__data__provider_dot_data__provider__pb2.CradleMessageGroupsRequest.FromString,
+                    response_serializer=th2__grpc__data__provider_dot_data__provider__pb2.CradleMessageGroupsResponse.SerializeToString,
+            ),
             'searchMessageGroups': grpc.unary_stream_rpc_method_handler(
                     servicer.searchMessageGroups,
                     request_deserializer=th2__grpc__data__provider_dot_data__provider__pb2.MessageGroupsSearchRequest.FromString,
                     response_serializer=th2__grpc__data__provider_dot_data__provider__pb2.MessageSearchResponse.SerializeToString,
             ),
             'getMessagesFilters': grpc.unary_unary_rpc_method_handler(
                     servicer.getMessagesFilters,
@@ -388,14 +404,31 @@
         return grpc.experimental.unary_stream(request, target, '/th2.data_provider.DataProvider/searchEvents',
             th2__grpc__data__provider_dot_data__provider__pb2.EventSearchRequest.SerializeToString,
             th2__grpc__data__provider_dot_data__provider__pb2.EventSearchResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def loadCradleMessageGroups(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/th2.data_provider.DataProvider/loadCradleMessageGroups',
+            th2__grpc__data__provider_dot_data__provider__pb2.CradleMessageGroupsRequest.SerializeToString,
+            th2__grpc__data__provider_dot_data__provider__pb2.CradleMessageGroupsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def searchMessageGroups(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/data_provider_service.py` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/data_provider_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
     def searchMessages(self, request, timeout=None):
         return self.connector.create_request('searchMessages', request, timeout)
 
     def searchEvents(self, request, timeout=None):
         return self.connector.create_request('searchEvents', request, timeout)
 
+    def loadCradleMessageGroups(self, request, timeout=None):
+        return self.connector.create_request('loadCradleMessageGroups', request, timeout)
+
     def searchMessageGroups(self, request, timeout=None):
         return self.connector.create_request('searchMessageGroups', request, timeout)
 
     def getMessagesFilters(self, request, timeout=None):
         return self.connector.create_request('getMessagesFilters', request, timeout)
 
     def getEventsFilters(self, request, timeout=None):
```

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_data_provider.proto` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_data_provider.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_data_provider_pb2.py` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_data_provider_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_data_provider_pb2.pyi` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_data_provider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_data_provider_pb2_grpc.py` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_data_provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider/queue_provider_service_service.py` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider/queue_provider_service_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider.egg-info/PKG-INFO` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-data-provider
-Version: 2.0.0.dev3800923993
+Version: 2.0.0.dev3800999250
 Summary: th2_grpc_data_provider
 Home-page: https://github.com/th2-net/th2-data-provider
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC generator template library
```

### Comparing `th2_grpc_data_provider-2.0.0.dev3800923993/th2_grpc_data_provider.egg-info/SOURCES.txt` & `th2_grpc_data_provider-2.0.0.dev3800999250/th2_grpc_data_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

