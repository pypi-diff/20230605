# Comparing `tmp/nuclio_sdk-0.5.3.tar.gz` & `tmp/nuclio_sdk-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-moulhhhn/nuclio_sdk-0.5.3.tar", last modified: Wed May 17 14:34:20 2023, max compression
+gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-ttg06ebp/nuclio_sdk-0.5.4.tar", last modified: Mon Jun  5 11:07:45 2023, max compression
```

## Comparing `nuclio_sdk-0.5.3.tar` & `nuclio_sdk-0.5.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/mock_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/mock_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/setup.py
```

### Comparing `nuclio_sdk-0.5.3/LICENSE.txt` & `nuclio_sdk-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/PKG-INFO` & `nuclio_sdk-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclio_sdk
-Version: 0.5.3
+Version: 0.5.4
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.3/Pipfile` & `nuclio_sdk-0.5.4/Pipfile`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/Pipfile.lock` & `nuclio_sdk-0.5.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/__init__.py` & `nuclio_sdk-0.5.4/nuclio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/context.py` & `nuclio_sdk-0.5.4/nuclio_sdk/context.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/event.py` & `nuclio_sdk-0.5.4/nuclio_sdk/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         # serialize it if is a datetime object
         if isinstance(self.timestamp, datetime.datetime):
             obj["timestamp"] = str(self.timestamp)
 
         if isinstance(obj["body"], bytes):
             obj["body"] = base64.b64encode(obj["body"]).decode("ascii")
 
-        return json.dumps(obj)
+        return json.dumps(obj, default=str)
 
     def get_header(self, header_key):
         for key, value in self.headers.items():
             if key.lower() == header_key.lower():
                 return value
 
     @staticmethod
```

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/exceptions.py` & `nuclio_sdk-0.5.4/nuclio_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/helpers.py` & `nuclio_sdk-0.5.4/nuclio_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/json_encoder.py` & `nuclio_sdk-0.5.4/nuclio_sdk/json_encoder.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/logger.py` & `nuclio_sdk-0.5.4/nuclio_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/platform.py` & `nuclio_sdk-0.5.4/nuclio_sdk/platform.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
-import signal
 import http.client
 
 import nuclio_sdk
 import nuclio_sdk.helpers
 
 
 class Platform(object):
@@ -31,14 +30,15 @@
         self.kind = kind
         self.namespace = namespace
 
         # connection_provider is used for unit testing
         self._connection_provider = connection_provider or http.client.HTTPConnection
 
         self._control_callback = on_control_callback
+        self._termination_callback = None
 
     async def explicit_ack(self, qualified_offset):
         """
         Notifying the processor to ack on a qualified offset
 
         :param qualified_offset: the qualified offset to ack
         :type qualified_offset: QualifiedOffset
@@ -47,19 +47,23 @@
         if self._control_callback:
             await self._control_callback(message)
         else:
             raise Exception(
                 "Cannot send explicit ack since control callback was not initialized"
             )
 
-    def on_signal(self, callback, sig=signal.SIGTERM):
+    def set_termination_callback(self, callback):
         """
-        Syntactic sugar to bind an incoming system signal on user's callback
+        Register a callback to be called when the platform is terminating.
+        If already registered, the callback will be replaced.
+        When called, the callback will be called with zero arguments.
+
+        :param callback: the callback to call when terminating
         """
-        signal.signal(sig, callback)
+        self._termination_callback = callback
 
     def call_function(
         self, function_name, event, node=None, timeout=None, service_name_override=None
     ):
 
         # get connection from provider
         connection = self._connection_provider(
@@ -125,7 +129,15 @@
         if self.kind == "local":
             service_name = service_name_override or "nuclio-{0}-{1}".format(
                 self.namespace, function_name
             )
         else:
             service_name = service_name_override or "nuclio-{0}".format(function_name)
         return "{0}:8080".format(service_name)
+
+    def _on_signal(self):
+        """
+        When a signal is received, call the termination callback as a hook before exiting
+        If not set, the callback will be a no-op
+        """
+        if self._termination_callback:
+            self._termination_callback()
```

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/qualified_offset.py` & `nuclio_sdk-0.5.4/nuclio_sdk/qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/response.py` & `nuclio_sdk-0.5.4/nuclio_sdk/response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/test/__init__.py` & `nuclio_sdk-0.5.4/nuclio_sdk/test/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/test/mock_platform.py` & `nuclio_sdk-0.5.4/nuclio_sdk/test/mock_platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/test/test_case.py` & `nuclio_sdk-0.5.4/nuclio_sdk/test/test_case.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/test/test_event.py` & `nuclio_sdk-0.5.4/nuclio_sdk/test/test_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import datetime
 import json
 
 import nuclio_sdk.test
 import nuclio_sdk.helpers
 import nuclio_sdk.json_encoder
 
 
@@ -45,14 +45,21 @@
 
     def test_event_to_json_string_body(self):
         request_body = "str-body"
         event = nuclio_sdk.Event(body=request_body)
         serialized_event = self._deserialize_event(event)
         self.assertEqual(request_body, serialized_event.body)
 
+    def test_print_event(self):
+        """
+        Test that printing an event doesn't raise an exception
+        """
+        event = nuclio_sdk.Event(body=datetime.datetime(2022, 1, 1))
+        print(event)
+
     def _deserialize_event(self, event):
         raise NotImplementedError
 
 
 class TestEventMsgPack(nuclio_sdk.test.TestCase, TestEvent):
     def _deserialize_event(self, event):
         event_json = {k: v for k, v in json.loads(event.to_json()).items()}
```

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/test/test_logger.py` & `nuclio_sdk-0.5.4/nuclio_sdk/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/test/test_qualified_offset.py` & `nuclio_sdk-0.5.4/nuclio_sdk/test/test_qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk/test/test_response.py` & `nuclio_sdk-0.5.4/nuclio_sdk/test/test_response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk.egg-info/PKG-INFO` & `nuclio_sdk-0.5.4/nuclio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclio-sdk
-Version: 0.5.3
+Version: 0.5.4
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.3/nuclio_sdk.egg-info/SOURCES.txt` & `nuclio_sdk-0.5.4/nuclio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.3/setup.py` & `nuclio_sdk-0.5.4/setup.py`

 * *Files identical despite different names*

