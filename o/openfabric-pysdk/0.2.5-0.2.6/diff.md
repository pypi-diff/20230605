# Comparing `tmp/openfabric_pysdk-0.2.5.tar.gz` & `tmp/openfabric_pysdk-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfabric_pysdk-0.2.5.tar", max compression
+gzip compressed data, was "openfabric_pysdk-0.2.6.tar", max compression
```

## Comparing `openfabric_pysdk-0.2.5.tar` & `openfabric_pysdk-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,76 @@
--rw-r--r--   0        0        0        0 2022-09-07 14:53:56.463341 openfabric_pysdk-0.2.5/README.md
--rw-r--r--   0        0        0        1 2023-03-14 13:31:02.159674 openfabric_pysdk-0.2.5/openfabric_pysdk/__init__.py
--rw-r--r--   0        0        0     5973 2023-04-14 19:33:07.463488 openfabric_pysdk-0.2.5/openfabric_pysdk/application.py
--rw-r--r--   0        0        0     3600 2023-03-30 07:45:52.768103 openfabric_pysdk-0.2.5/openfabric_pysdk/benchmark.py
--rw-r--r--   0        0        0      412 2023-03-14 13:25:56.167968 openfabric_pysdk-0.2.5/openfabric_pysdk/config.py
--rw-r--r--   0        0        0     5578 2023-04-11 19:44:10.159542 openfabric_pysdk-0.2.5/openfabric_pysdk/context.py
--rw-r--r--   0        0        0     7445 2023-04-14 07:07:30.349151 openfabric_pysdk-0.2.5/openfabric_pysdk/engine.py
--rw-r--r--   0        0        0     1993 2023-03-29 16:17:55.309405 openfabric_pysdk-0.2.5/openfabric_pysdk/loader.py
--rw-r--r--   0        0        0     1847 2023-04-14 19:08:23.089026 openfabric_pysdk-0.2.5/openfabric_pysdk/starter.py
--rw-r--r--   0        0        0     4463 2023-03-30 07:45:52.763114 openfabric_pysdk-0.2.5/openfabric_pysdk/store.py
--rw-r--r--   0        0        0     3114 2023-03-30 07:45:52.756404 openfabric_pysdk-0.2.5/openfabric_pysdk/task.py
--rw-r--r--   0        0        0    13433 2023-03-29 17:29:12.865670 openfabric_pysdk-0.2.5/openfabric_pysdk/templates/index.html
--rw-r--r--   0        0        0     3927 2023-04-14 19:55:42.380807 openfabric_pysdk-0.2.5/openfabric_pysdk/toolset.py
--rw-r--r--   0        0        0        0 2022-09-07 14:53:56.464562 openfabric_pysdk-0.2.5/openfabric_pysdk/transport/__init__.py
--rw-r--r--   0        0        0     2609 2023-03-15 16:39:57.524646 openfabric_pysdk-0.2.5/openfabric_pysdk/transport/queue.py
--rw-r--r--   0        0        0     1077 2023-04-14 07:05:53.611228 openfabric_pysdk-0.2.5/openfabric_pysdk/transport/rest.py
--rw-r--r--   0        0        0     6224 2023-04-14 19:04:51.739451 openfabric_pysdk-0.2.5/openfabric_pysdk/transport/socket.py
--rw-r--r--   0        0        0     2404 2023-04-14 20:26:38.835024 openfabric_pysdk-0.2.5/openfabric_pysdk/utility.py
--rw-r--r--   0        0        0      914 2023-04-20 14:46:51.646435 openfabric_pysdk-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 openfabric_pysdk-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-07 14:53:56.463341 openfabric_pysdk-0.2.6/README.md
+-rw-r--r--   0        0        0        1 2023-03-14 13:31:02.159674 openfabric_pysdk-0.2.6/openfabric_pysdk/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-30 07:33:24.749243 openfabric_pysdk-0.2.6/openfabric_pysdk/app/__init__.py
+-rw-r--r--   0        0        0     1900 2023-04-30 08:34:09.493462 openfabric_pysdk-0.2.6/openfabric_pysdk/app/app.py
+-rw-r--r--   0        0        0       67 2023-04-30 07:33:24.750402 openfabric_pysdk-0.2.6/openfabric_pysdk/benchmark/__init__.py
+-rw-r--r--   0        0        0     3606 2023-04-30 07:33:24.751474 openfabric_pysdk-0.2.6/openfabric_pysdk/benchmark/time_benchmark.py
+-rw-r--r--   0        0        0      282 2023-04-30 07:33:24.751836 openfabric_pysdk-0.2.6/openfabric_pysdk/context/__init__.py
+-rw-r--r--   0        0        0      178 2023-04-30 07:33:24.752888 openfabric_pysdk-0.2.6/openfabric_pysdk/context/bar.py
+-rw-r--r--   0        0        0      477 2023-04-30 07:33:24.753204 openfabric_pysdk-0.2.6/openfabric_pysdk/context/bar_schema.py
+-rw-r--r--   0        0        0     1224 2023-04-30 07:33:24.753644 openfabric_pysdk-0.2.6/openfabric_pysdk/context/message.py
+-rw-r--r--   0        0        0      599 2023-04-30 07:33:24.754167 openfabric_pysdk-0.2.6/openfabric_pysdk/context/message_schema.py
+-rw-r--r--   0        0        0     3281 2023-05-20 05:27:06.114491 openfabric_pysdk-0.2.6/openfabric_pysdk/context/ray.py
+-rw-r--r--   0        0        0      863 2023-05-20 05:27:06.114733 openfabric_pysdk-0.2.6/openfabric_pysdk/context/ray_schema.py
+-rw-r--r--   0        0        0      861 2023-04-30 07:33:24.755605 openfabric_pysdk-0.2.6/openfabric_pysdk/context/state.py
+-rw-r--r--   0        0        0      313 2023-04-30 07:33:24.755983 openfabric_pysdk-0.2.6/openfabric_pysdk/context/state_schema.py
+-rw-r--r--   0        0        0       84 2023-04-30 07:33:24.757497 openfabric_pysdk-0.2.6/openfabric_pysdk/engine/__init__.py
+-rw-r--r--   0        0        0     3893 2023-05-21 17:16:05.359357 openfabric_pysdk-0.2.6/openfabric_pysdk/engine/background_engine.py
+-rw-r--r--   0        0        0     4150 2023-05-20 05:27:06.115241 openfabric_pysdk-0.2.6/openfabric_pysdk/engine/foreground_engine.py
+-rw-r--r--   0        0        0       62 2023-04-30 07:33:24.758547 openfabric_pysdk-0.2.6/openfabric_pysdk/execution/__init__.py
+-rw-r--r--   0        0        0     4745 2023-04-30 07:33:24.758717 openfabric_pysdk-0.2.6/openfabric_pysdk/execution/container.py
+-rw-r--r--   0        0        0      522 2023-04-30 07:33:24.760682 openfabric_pysdk-0.2.6/openfabric_pysdk/execution/profile.py
+-rw-r--r--   0        0        0       49 2023-04-30 07:33:24.761730 openfabric_pysdk-0.2.6/openfabric_pysdk/fields/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-30 07:33:24.762486 openfabric_pysdk-0.2.6/openfabric_pysdk/flask/__init__.py
+-rw-r--r--   0        0        0      435 2023-05-21 17:16:05.359646 openfabric_pysdk-0.2.6/openfabric_pysdk/flask/core/__init__.py
+-rw-r--r--   0        0        0      423 2023-04-30 07:33:24.764277 openfabric_pysdk-0.2.6/openfabric_pysdk/flask/rest/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-30 07:33:24.764893 openfabric_pysdk-0.2.6/openfabric_pysdk/flask/socket/__init__.py
+-rw-r--r--   0        0        0      339 2023-04-30 07:33:24.765183 openfabric_pysdk-0.2.6/openfabric_pysdk/flask/socket/socketio_client.py
+-rw-r--r--   0        0        0      703 2023-04-30 07:33:24.765747 openfabric_pysdk-0.2.6/openfabric_pysdk/flask/socket/socketio_server.py
+-rw-r--r--   0        0        0       25 2023-05-20 05:27:06.115444 openfabric_pysdk-0.2.6/openfabric_pysdk/helper/__init__.py
+-rwxr-xr-x   0        0        0    16557 2023-05-20 05:27:06.115781 openfabric_pysdk-0.2.6/openfabric_pysdk/helper/proxy.py
+-rw-r--r--   0        0        0      664 2023-04-30 07:33:24.766303 openfabric_pysdk-0.2.6/openfabric_pysdk/loader/__init__.py
+-rw-r--r--   0        0        0      411 2023-04-30 07:33:24.766884 openfabric_pysdk-0.2.6/openfabric_pysdk/loader/config.py
+-rw-r--r--   0        0        0      208 2023-04-30 07:33:24.767395 openfabric_pysdk-0.2.6/openfabric_pysdk/service/__init__.py
+-rw-r--r--   0        0        0     1840 2023-04-30 08:25:56.833777 openfabric_pysdk-0.2.6/openfabric_pysdk/service/config_service.py
+-rw-r--r--   0        0        0     1443 2023-04-30 07:33:24.768243 openfabric_pysdk-0.2.6/openfabric_pysdk/service/remote_service.py
+-rw-r--r--   0        0        0     1007 2023-04-30 07:33:24.768766 openfabric_pysdk-0.2.6/openfabric_pysdk/service/rest_service.py
+-rw-r--r--   0        0        0     2199 2023-05-21 17:16:05.359939 openfabric_pysdk-0.2.6/openfabric_pysdk/service/socket_service.py
+-rw-r--r--   0        0        0     1477 2023-04-30 07:33:24.769946 openfabric_pysdk-0.2.6/openfabric_pysdk/service/swagger_service.py
+-rw-r--r--   0        0        0     1436 2023-04-30 07:33:24.770568 openfabric_pysdk-0.2.6/openfabric_pysdk/starter.py
+-rw-r--r--   0        0        0       75 2023-04-30 07:33:24.770993 openfabric_pysdk-0.2.6/openfabric_pysdk/store/__init__.py
+-rw-r--r--   0        0        0     2375 2023-04-30 07:33:24.771468 openfabric_pysdk-0.2.6/openfabric_pysdk/store/kvdb.py
+-rw-r--r--   0        0        0     1438 2023-04-30 07:33:24.771791 openfabric_pysdk-0.2.6/openfabric_pysdk/store/lru.py
+-rw-r--r--   0        0        0     2140 2023-04-30 07:33:24.772057 openfabric_pysdk-0.2.6/openfabric_pysdk/store/store.py
+-rw-r--r--   0        0        0     3114 2023-03-30 07:45:52.756404 openfabric_pysdk-0.2.6/openfabric_pysdk/task.py
+-rw-r--r--   0        0        0       52 2023-04-30 07:33:24.772326 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-30 07:33:24.772612 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/resource_descriptor.py
+-rw-r--r--   0        0        0        1 2023-04-30 07:33:24.772728 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/__init__.py
+-rw-r--r--   0        0        0      230 2023-04-30 07:33:24.773153 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/local/__init__.py
+-rw-r--r--   0        0        0      933 2023-04-30 07:33:24.774425 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/local/benchmark_api.py
+-rw-r--r--   0        0        0     1674 2023-04-30 07:33:24.775125 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/local/config_api.py
+-rw-r--r--   0        0        0     1128 2023-04-30 07:33:24.775494 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/local/execution_api.py
+-rw-r--r--   0        0        0     1040 2023-04-30 07:33:24.775745 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/local/manifest_api.py
+-rw-r--r--   0        0        0     2793 2023-05-20 05:27:06.116305 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/local/queue_api.py
+-rw-r--r--   0        0        0      256 2023-05-20 05:27:06.116771 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/remote/__init__.py
+-rw-r--r--   0        0        0      943 2023-04-30 07:33:24.776948 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/remote/benchmark_api.py
+-rw-r--r--   0        0        0     1864 2023-04-30 07:33:24.777581 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/remote/config_api.py
+-rw-r--r--   0        0        0     1015 2023-04-30 07:33:24.778047 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/remote/execution_api.py
+-rw-r--r--   0        0        0      966 2023-04-30 07:33:24.778209 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/remote/manifest_api.py
+-rw-r--r--   0        0        0     3036 2023-04-30 07:33:24.778366 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/remote/queue_api.py
+-rw-r--r--   0        0        0      135 2023-04-30 07:33:24.778771 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/schema/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-30 07:33:24.779464 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/schema/benchmark_schema.py
+-rw-r--r--   0        0        0      852 2023-04-30 07:33:24.779824 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/schema/manifest_schema.py
+-rw-r--r--   0        0        0      453 2023-04-30 07:33:24.780025 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/schema/uid_schema.py
+-rw-r--r--   0        0        0        0 2023-04-30 07:33:24.780094 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/socket/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-30 07:33:24.780365 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/socket/local/__init__.py
+-rw-r--r--   0        0        0     7662 2023-05-20 09:34:54.443872 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/socket/local/execution_socket.py
+-rw-r--r--   0        0        0       71 2023-05-20 05:27:06.117732 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/socket/remote/__init__.py
+-rw-r--r--   0        0        0     3954 2023-04-30 07:33:24.780960 openfabric_pysdk-0.2.6/openfabric_pysdk/transport/socket/remote/execution_socket.py
+-rw-r--r--   0        0        0      138 2023-04-30 07:33:24.781197 openfabric_pysdk-0.2.6/openfabric_pysdk/utility/__init__.py
+-rw-r--r--   0        0        0      679 2023-04-30 07:33:24.781459 openfabric_pysdk-0.2.6/openfabric_pysdk/utility/change_util.py
+-rw-r--r--   0        0        0     1473 2023-04-30 07:33:24.781730 openfabric_pysdk-0.2.6/openfabric_pysdk/utility/loader_util.py
+-rw-r--r--   0        0        0      345 2023-04-30 07:33:24.782179 openfabric_pysdk-0.2.6/openfabric_pysdk/utility/schema_util.py
+-rw-r--r--   0        0        0      890 2023-04-30 07:33:24.782442 openfabric_pysdk-0.2.6/openfabric_pysdk/utility/zip_util.py
+-rw-r--r--   0        0        0    13433 2023-04-30 07:33:24.783125 openfabric_pysdk-0.2.6/openfabric_pysdk/view/index.html
+-rw-r--r--   0        0        0      941 2023-06-05 14:36:39.987714 openfabric_pysdk-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 openfabric_pysdk-0.2.6/PKG-INFO
```

### Comparing `openfabric_pysdk-0.2.5/openfabric_pysdk/benchmark.py` & `openfabric_pysdk-0.2.6/openfabric_pysdk/benchmark/time_benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,20 +69,20 @@
     global _stats
     stats = _stats.get(name, None)
     if stats is None:
         logging.debug(f'Openfabric - timing_name="{name}", avg=never_recorded')
     else:
         count = len(stats)
         logging.debug(f'Openfabric - timing_name="{name}", '
-                     f'avg={stats.mean():.4g} '
-                     f'count={count} '
-                     f'stddev={stats.stddev() if count > 1 else float("NaN"):.4g} '
-                     f'min={stats.minimum():.4g} '
-                     f'max={stats.maximum():.4g} '
-                     )
+                      f'avg={stats.mean():.4g} '
+                      f'count={count} '
+                      f'stddev={stats.stddev() if count > 1 else float("NaN"):.4g} '
+                      f'min={stats.minimum():.4g} '
+                      f'max={stats.maximum():.4g} '
+                      )
 
 
 def clear_timings() -> None:
     global _stats
     _stats.clear()
```

### Comparing `openfabric_pysdk-0.2.5/openfabric_pysdk/loader.py` & `openfabric_pysdk-0.2.6/openfabric_pysdk/utility/loader_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import importlib
 from pydoc import locate
 
+from openfabric_pysdk.loader.config import execution
 from openfabric_pysdk.benchmark import MeasureBlockTime
-from openfabric_pysdk.config import execution
 
 
 #######################################################
 # Class loader utility class
 #######################################################
-class Loader:
+class LoaderUtil:
 
     @staticmethod
     def import_class(name):
         return locate(name.__module__ + "." + name.__name__)
 
     @staticmethod
     def get_class(name):
@@ -36,26 +36,7 @@
             function = function_config['function']
             package = function_config['package']
             if function is None or package is None:
                 return None
             module = importlib.import_module(package)
             # print(module.__name__ + "." + function)
             return locate(module.__name__ + "." + function)
-
-
-# Output concept
-InputClass = Loader.get_class("input_class")
-InputSchema = Loader.get_class("input_schema")
-
-# Output concept
-OutputClass = Loader.get_class("output_class")
-OutputSchema = Loader.get_class("output_schema")
-
-# Config concept
-ConfigClass = Loader.get_class("config_class")
-ConfigSchema = Loader.get_class("config_schema")
-
-# Execution callback function
-execution_callback_function = Loader.get_function("main_callback")
-
-# Config callback function
-config_callback_function = Loader.get_function("config_callback")
```

### Comparing `openfabric_pysdk-0.2.5/openfabric_pysdk/task.py` & `openfabric_pysdk-0.2.6/openfabric_pysdk/task.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.5/openfabric_pysdk/templates/index.html` & `openfabric_pysdk-0.2.6/openfabric_pysdk/view/index.html`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.5/openfabric_pysdk/transport/rest.py` & `openfabric_pysdk-0.2.6/openfabric_pysdk/transport/rest/local/execution_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import uuid
 
-from flask_apispec import marshal_with, doc, use_kwargs
-from flask_apispec.views import MethodResource
-from flask_restful import Resource
-
 from openfabric_pysdk.engine import foreground
+from openfabric_pysdk.flask.rest import *
 from openfabric_pysdk.loader import *
-from openfabric_pysdk.context import State
+from openfabric_pysdk.transport import ResourceDescriptor
 
 
 #######################################################
 #  Execution API
 #######################################################
-class ExecutionRestApi(MethodResource, Resource):
-    __state: State = None
+class ExecutionApi(MethodResource, Resource):
+    __descriptor: ResourceDescriptor = None
 
     # ------------------------------------------------------------------------
-    def __init__(self, state: State = None):
-        self.__state = state
+    def __init__(self, descriptor: ResourceDescriptor = None):
+        self.__descriptor = descriptor
 
-    @doc(description="Execute app and get response", tags=["Execution"])
+    # ------------------------------------------------------------------------
+    @doc(description="Execute execution and get response", tags=["Execution"])
     @use_kwargs(InputSchema, location='json')
-    @marshal_with(OutputSchema)  # marshalling
+    @marshal_with(OutputSchema)
     def post(self, *args) -> OutputClass:
         sid = uuid.uuid4().hex
         data = InputSchema().dump(list(args) if InputSchema().many is True else args[0])
-        qid = foreground.prepare(data, sid=sid, state=self.__state)
+        app = self.__descriptor.app
+        qid = foreground.prepare(app, data, sid=sid)
         return foreground.process(qid)
```

### Comparing `openfabric_pysdk-0.2.5/pyproject.toml` & `openfabric_pysdk-0.2.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openfabric-pysdk"
-version = "0.2.5"
+version = "0.2.6"
 description = "Openfabric Python SDK"
 authors = ["Andrei Tara <andrei@openfabric.ai>"]
 readme = "README.md"
 homepage = "https://openfabric.ai"
 repository = "https://github.com/Openfabric/openfabic-pysdk"
 keywords = ["openfabric", "SDK", "IoAI"]
 classifiers = [
@@ -23,14 +23,15 @@
 pickleDB = "^0.9.2"
 runstats = "^2.0.0"
 tqdm = "^4.62.3"
 Werkzeug = "2.0.3"
 marshmallow-enum = "^1.5.1"
 gevent = "^22.10.2"
 gevent-websocket = "^0.10.1"
+socketio-client = "^0.7.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openfabric_pysdk-0.2.5/PKG-INFO` & `openfabric_pysdk-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfabric-pysdk
-Version: 0.2.5
+Version: 0.2.6
 Summary: Openfabric Python SDK
 Home-page: https://openfabric.ai
 Keywords: openfabric,SDK,IoAI
 Author: Andrei Tara
 Author-email: andrei@openfabric.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -22,12 +22,13 @@
 Requires-Dist: Werkzeug (==2.0.3)
 Requires-Dist: flask-apispec (==0.11.0)
 Requires-Dist: gevent (>=22.10.2,<23.0.0)
 Requires-Dist: gevent-websocket (>=0.10.1,<0.11.0)
 Requires-Dist: marshmallow-enum (>=1.5.1,<2.0.0)
 Requires-Dist: pickleDB (>=0.9.2,<0.10.0)
 Requires-Dist: runstats (>=2.0.0,<3.0.0)
+Requires-Dist: socketio-client (>=0.7.2,<0.8.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Repository, https://github.com/Openfabric/openfabic-pysdk
 Description-Content-Type: text/markdown
```

