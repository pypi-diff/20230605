# Comparing `tmp/classwork-0.0.5.tar.gz` & `tmp/classwork-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classwork-0.0.5.tar", max compression
+gzip compressed data, was "classwork-0.0.6.tar", max compression
```

## Comparing `classwork-0.0.5.tar` & `classwork-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-06-03 17:09:04.784909 classwork-0.0.5/LICENSE.md
--rw-r--r--   0        0        0     4217 2023-06-04 23:24:45.976726 classwork-0.0.5/README.md
--rw-r--r--   0        0        0      161 2023-06-03 15:43:24.017838 classwork-0.0.5/classwork/__init__.py
--rw-r--r--   0        0        0    11825 2023-06-05 00:43:48.036265 classwork-0.0.5/classwork/main.py
--rw-r--r--   0        0        0     3682 2023-06-05 00:42:29.366659 classwork-0.0.5/classwork/utils.py
--rw-r--r--   0        0        0      473 2023-06-05 00:21:21.251984 classwork-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 classwork-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-03 17:09:04.784909 classwork-0.0.6/LICENSE.md
+-rw-r--r--   0        0        0     4534 2023-06-05 02:18:46.252572 classwork-0.0.6/README.md
+-rw-r--r--   0        0        0      161 2023-06-03 15:43:24.017838 classwork-0.0.6/classwork/__init__.py
+-rw-r--r--   0        0        0    12765 2023-06-05 02:11:06.603814 classwork-0.0.6/classwork/main.py
+-rw-r--r--   0        0        0     3700 2023-06-05 02:11:24.504052 classwork-0.0.6/classwork/utils.py
+-rw-r--r--   0        0        0      473 2023-06-05 01:11:15.309982 classwork-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5306 1970-01-01 00:00:00.000000 classwork-0.0.6/PKG-INFO
```

### Comparing `classwork-0.0.5/LICENSE.md` & `classwork-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.5/README.md` & `classwork-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -97,29 +97,29 @@
 This code will create a *task* into NATS and the job workers (attentive students 😂) already listening will pick the task and run it, then publish their reports which is routed via NATS back to the scheduler (teacher?).
 
 Take note of the following:
 1. `class_work.assign` must be run in async mode. So we have wrapped it in an async method. You can also use `asyncio.run` directly.
 2. Naming your task is very important. This naming convection is unashamedly borrowed from [moleculer](https://moleculer.services/). In this case, your task is **"my_worker.add"**. This will route to any worker class registered with the **name** "my_worker" and method "add". 
 3. Because all this traffic is routed via NATS, your arguments must be JSON serializable. Even though we use [typ](https://github.com/vsapronov/typjson) to handle edge cases like `sets`, beware that there are limits to what you can pass in your arguments
 4. `report_callback` must be async. It is called with a 'report' of your task. A report card 😊 will look like the one below:
-
+5. `args` can be passed as a list or dict. They will be treated as `*args` if list and `**kwargs` if dict.
 
 ```
 We have a report!
 {'task': 'my_worker.add',
  'duration': {'latency': {'request': '4 ms and 356 µs',
                           'response': '5 s and 4 ms'},
               'my_worker.add': '3 s and 1 ms'},
  'req_id': '8mYjJjM0kb5',
  'response': 3}
 ```
 
 ## Report Explanation
 - **duration:** is a high precision (down to yoctoseconds) report of the time taken.
-    - **latency:** shows the time taken to route your "task **request**" to the worker and "task **response**" back to the scheduler.
+    - **latency:** shows the time taken to route your "task **request**" to the worker and "task **response**" back to the scheduler. It is important to understand that since both worker and scheduler are disconnected, latency may also include delays of either to access the NATS network and thus does not specifically refer to network latency.
 - **req_id:** is a unique id assigned to each job
 - **response:** is the actual value returned by the worker
 
 
 ## Try it
 
 We have sample code in [scheduler.py](scheduler.py) and [worker.py](worker.py)
```

### Comparing `classwork-0.0.5/classwork/main.py` & `classwork-0.0.6/classwork/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 """
 import json
 import asyncio
 import uuid
 import nats
 import sys
 import traceback
+from termcolor2 import c
 from time import perf_counter as pc
 from typ import json as safe_json
 from nats.aio.client import Client as NATS
 from nats.aio.errors import ErrNoServers, ErrTimeout
 
 from .utils import (
     hash_str,
     precision_format_time,
     importing_script,
     sanitize_name,
     get_class_props,
     RaisingThread,
     is_initialized,
     trace_report_error,
+    isclass,
 )
 
 app_name = "classwork"
 
 
 class ClassWork:
     def __init__(self, nats_url) -> None:
@@ -90,15 +92,17 @@
         except ErrNoServers as e:
             # Could not connect to any server in the cluster.
             # print(e)
             return
 
         if nc.is_connected:
             print(
-                f" >> Connection to NATS server [{nc.connected_url.netloc}] established."
+                c(
+                    f" >> Connection to NATS server [{nc.connected_url.netloc}] established."
+                ).green.bold
             )
             self.nc = nc
             self.js = nc.jetstream()
 
             return self.nc, self.js
 
     async def __add_stream(self, stream_name, subjects):
@@ -212,15 +216,22 @@
 
             except Exception as e:
                 # print(e)
                 await asyncio.sleep(2)
                 pass
 
     async def register(self, name, worker_class):
+        # validate values
+        if not isinstance(name, str):
+            raise TypeError(f"name must be a string")
+
         # ensure worker class is initialized
+        if not isclass(worker_class):
+            raise TypeError("worker_class must be a class")
+
         if not is_initialized(worker_class):
             raise Exception("worker_class must be initialized before registering it!")
 
         await self.__setup()
         # make & sanitize name
         name = sanitize_name(name)
         # make subjects
@@ -241,15 +252,21 @@
 
                 # print(data)
                 # calc latency
                 latency = pc() - data["call_start"]
 
                 try:
                     # call worker method and pass args
-                    response = await func(*data["args"])
+                    if isinstance(data["args"], dict):
+                        # **kwargs
+                        response = await func(**data["args"])
+                    elif isinstance(data["args"], list):
+                        # *args                #
+                        response = await func(*data["args"])
+
                 except Exception as e:
                     trace_report_error()
                     # probably exit?
                     sys.exit()
                 # calculate total time
                 duration = pc() - data["call_start"] - latency
 
@@ -258,15 +275,15 @@
                     "response": response,
                     "task": subject,
                     # "args": data["args"],
                     "req_id": data["req_id"],
                     "call_start": data["call_start"],
                     "duration": {
                         "latency": {"request": latency},
-                        f"{subject}": precision_format_time(duration),
+                        f"{subject}": duration,
                     },
                 }
 
                 ack = await self.js.publish(
                     data["reply"], safe_json.dumps(payload).encode()
                 )
 
@@ -292,14 +309,24 @@
             # try:
             #     t.join()
             # except Exception as e:
             #     print(e)
             #     raise e
 
     async def assign(self, task, args, report_callback):
+        # validate values
+        if not isinstance(task, str):
+            raise TypeError(f"task must be a string")
+
+        if not isinstance(args, (list, dict)):
+            raise TypeError(f"args must be a list or dict")
+
+        if not callable(report_callback):
+            raise TypeError(f"report_callback must be a callable method")
+
         await self.__setup()
 
         # make req_id
         req_id = str(pc())
         req_id = "{}_{}_{}_{}".format(
             self.id, req_id, task, "".join(list(map(str, args)))
         )
@@ -332,35 +359,36 @@
                     data = json.loads(msg.data.decode())
 
                     # data["duration"]["request_latency"]
                     data["duration"]["latency"]["response"] = precision_format_time(
                         pc()
                         - data["call_start"]
                         - data["duration"]["latency"]["request"]
+                        - data["duration"][task]
                     )
 
-                    # print( data["duration"]["latency"]["request"] )
+                    data["duration"][task] = precision_format_time(
+                        data["duration"][task]
+                    )
 
                     data["duration"]["latency"]["request"] = precision_format_time(
                         data["duration"]["latency"]["request"]
                     )
 
                     del data["call_start"]
 
                     try:
                         await report_callback(data)
                     except Exception as e:
                         trace_report_error("SCHEDULER/REPORT ERROR!")
-                        # exit
-                        sys.exit()
 
                     # acknowledge receipt
                     await msg.ack()
 
             except Exception as e:
-                # print(e)
+                print(e)
                 raise e
 
         t = RaisingThread(target=self.__get_messages_bg, args=[self.id, handle_message])
         t.start()
 
         # await __clear_streams()
```

### Comparing `classwork-0.0.5/classwork/utils.py` & `classwork-0.0.6/classwork/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import os
 import sys
 import re
 import traceback
 import threading
 from hashids import Hashids
 from termcolor2 import c
+from pprint import pprint
 
 
 def precision_format_time(seconds, precision=2, last_sep=" and "):
     time_dict = {
         "hours": int(seconds // 3600),
         "minutes": int((seconds % 3600) // 60),
         "seconds": int(seconds % 60),
@@ -91,16 +92,21 @@
     def __init__(self) -> None:
         pass
 
 
 default_props = dir(__c)
 
 
-def is_initialized(testClass):
-    return type(testClass) != type(__c)
+# check if a class is initialized
+def is_initialized(cls):
+    return isclass(cls) and type(cls) != type(__c)
+
+
+def isclass(var):
+    return str(type(var)).startswith("<class")
 
 
 def get_class_props(cls):
     props = [
         p for p in dir(cls) if p not in default_props and callable(getattr(cls, p))
     ]
 
@@ -133,17 +139,13 @@
         frame = sys.exc_info()[2].tb_frame.f_back.f_back
         print(" >> invoked by:", frame.f_code.co_name)
 
 
 def trace_report_error(header="WORKER/TASK ERROR!"):
     # format error in running function
     e = traceback.format_exc()
-    # first we split by File tracebacks
-    e = e.split("File ")
-    # We discard index 1 as it points to this file
-    e.pop(1)
 
-    # Then we join back
-    e = "  File ".join(e)
+    ee = re.sub(r"[\w\W]+?in handle_message[^\)]+\)\n", "", e)
+
     # print error now
     print(c(f"\n{header}").red.blink.bold.underline)
-    print(c(f"  {e}").red)
+    print(c(f"  {ee}").red)
```

### Comparing `classwork-0.0.5/PKG-INFO` & `classwork-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classwork
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple Python module to help distribute you tasks across multiple brokers as microservices
 License: MIT
 Author: Anthony Mugendi
 Author-email: ngurumugz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -118,29 +118,29 @@
 This code will create a *task* into NATS and the job workers (attentive students 😂) already listening will pick the task and run it, then publish their reports which is routed via NATS back to the scheduler (teacher?).
 
 Take note of the following:
 1. `class_work.assign` must be run in async mode. So we have wrapped it in an async method. You can also use `asyncio.run` directly.
 2. Naming your task is very important. This naming convection is unashamedly borrowed from [moleculer](https://moleculer.services/). In this case, your task is **"my_worker.add"**. This will route to any worker class registered with the **name** "my_worker" and method "add". 
 3. Because all this traffic is routed via NATS, your arguments must be JSON serializable. Even though we use [typ](https://github.com/vsapronov/typjson) to handle edge cases like `sets`, beware that there are limits to what you can pass in your arguments
 4. `report_callback` must be async. It is called with a 'report' of your task. A report card 😊 will look like the one below:
-
+5. `args` can be passed as a list or dict. They will be treated as `*args` if list and `**kwargs` if dict.
 
 ```
 We have a report!
 {'task': 'my_worker.add',
  'duration': {'latency': {'request': '4 ms and 356 µs',
                           'response': '5 s and 4 ms'},
               'my_worker.add': '3 s and 1 ms'},
  'req_id': '8mYjJjM0kb5',
  'response': 3}
 ```
 
 ## Report Explanation
 - **duration:** is a high precision (down to yoctoseconds) report of the time taken.
-    - **latency:** shows the time taken to route your "task **request**" to the worker and "task **response**" back to the scheduler.
+    - **latency:** shows the time taken to route your "task **request**" to the worker and "task **response**" back to the scheduler. It is important to understand that since both worker and scheduler are disconnected, latency may also include delays of either to access the NATS network and thus does not specifically refer to network latency.
 - **req_id:** is a unique id assigned to each job
 - **response:** is the actual value returned by the worker
 
 
 ## Try it
 
 We have sample code in [scheduler.py](scheduler.py) and [worker.py](worker.py)
```

