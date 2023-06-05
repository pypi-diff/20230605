# Comparing `tmp/classwork-0.0.4.tar.gz` & `tmp/classwork-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classwork-0.0.4.tar", max compression
+gzip compressed data, was "classwork-0.0.5.tar", max compression
```

## Comparing `classwork-0.0.4.tar` & `classwork-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-06-03 17:09:04.784909 classwork-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     4193 2023-06-03 16:54:31.476439 classwork-0.0.4/README.md
--rw-r--r--   0        0        0      161 2023-06-03 15:43:24.017838 classwork-0.0.4/classwork/__init__.py
--rw-r--r--   0        0        0    11255 2023-06-04 22:42:29.676389 classwork-0.0.4/classwork/main.py
--rw-r--r--   0        0        0     3190 2023-06-04 22:42:45.904413 classwork-0.0.4/classwork/utils.py
--rw-r--r--   0        0        0      451 2023-06-04 22:46:14.677039 classwork-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4922 1970-01-01 00:00:00.000000 classwork-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-03 17:09:04.784909 classwork-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     4217 2023-06-04 23:24:45.976726 classwork-0.0.5/README.md
+-rw-r--r--   0        0        0      161 2023-06-03 15:43:24.017838 classwork-0.0.5/classwork/__init__.py
+-rw-r--r--   0        0        0    11825 2023-06-05 00:43:48.036265 classwork-0.0.5/classwork/main.py
+-rw-r--r--   0        0        0     3682 2023-06-05 00:42:29.366659 classwork-0.0.5/classwork/utils.py
+-rw-r--r--   0        0        0      473 2023-06-05 00:21:21.251984 classwork-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 classwork-0.0.5/PKG-INFO
```

### Comparing `classwork-0.0.4/LICENSE.md` & `classwork-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.4/README.md` & `classwork-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 # init ClassWork
 nats_url = "nats://127.0.0.1:4222"
 class_work = ClassWork(nats_url=nats_url)
 
 # Our callback function
 # This is where complete work gets reported
-def report_callback(report_card):
+async def report_callback(report_card):
     print("We have a report!")
     pprint(report_card)
 
 
 # We need this function to create our job schedules
 async def schedules():
     # Assign a job
@@ -96,15 +96,15 @@
 
 This code will create a *task* into NATS and the job workers (attentive students 😂) already listening will pick the task and run it, then publish their reports which is routed via NATS back to the scheduler (teacher?).
 
 Take note of the following:
 1. `class_work.assign` must be run in async mode. So we have wrapped it in an async method. You can also use `asyncio.run` directly.
 2. Naming your task is very important. This naming convection is unashamedly borrowed from [moleculer](https://moleculer.services/). In this case, your task is **"my_worker.add"**. This will route to any worker class registered with the **name** "my_worker" and method "add". 
 3. Because all this traffic is routed via NATS, your arguments must be JSON serializable. Even though we use [typ](https://github.com/vsapronov/typjson) to handle edge cases like `sets`, beware that there are limits to what you can pass in your arguments
-4. `report_callback` is called with a 'report' of your task. A report card 😊 will look like the one below:
+4. `report_callback` must be async. It is called with a 'report' of your task. A report card 😊 will look like the one below:
 
 
 ```
 We have a report!
 {'task': 'my_worker.add',
  'duration': {'latency': {'request': '4 ms and 356 µs',
                           'response': '5 s and 4 ms'},
```

### Comparing `classwork-0.0.4/classwork/main.py` & `classwork-0.0.5/classwork/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,31 @@
  This software is released under the MIT License.
  https://opensource.org/licenses/MIT
 """
 import json
 import asyncio
 import uuid
 import nats
-
+import sys
+import traceback
 from time import perf_counter as pc
 from typ import json as safe_json
 from nats.aio.client import Client as NATS
 from nats.aio.errors import ErrNoServers, ErrTimeout
 
-from .utils import hash_str, precision_format_time, importing_script, sanitize_name, get_class_props, RaisingThread, is_initialized
+from .utils import (
+    hash_str,
+    precision_format_time,
+    importing_script,
+    sanitize_name,
+    get_class_props,
+    RaisingThread,
+    is_initialized,
+    trace_report_error,
+)
 
 app_name = "classwork"
 
 
 class ClassWork:
     def __init__(self, nats_url) -> None:
         self.nats_url = nats_url
@@ -29,18 +39,17 @@
 
     async def __setup(self):
         mac_id = hex(uuid.getnode())
         exec_file = importing_script()
         hashid = hash_str(f"{exec_file}")
         self.id = f"{app_name}_{mac_id}_{str(hashid)}"
 
-    async def __connect(self):       
-        
+    async def __connect(self):
         # trace_caller()
-    
+
         # Setup pool of servers from a NATS cluster.
         options = {
             "servers": self.nats_url
             if isinstance(self.nats_url, list)
             else [self.nats_url]
         }
 
@@ -80,20 +89,21 @@
             nc = await nats.connect(**options)
         except ErrNoServers as e:
             # Could not connect to any server in the cluster.
             # print(e)
             return
 
         if nc.is_connected:
-            print(f" >> Connection to NATS server [{nc.connected_url.netloc}] established.")
+            print(
+                f" >> Connection to NATS server [{nc.connected_url.netloc}] established."
+            )
             self.nc = nc
             self.js = nc.jetstream()
 
             return self.nc, self.js
-        
 
     async def __add_stream(self, stream_name, subjects):
         # print(f"{stream_name=}, {subjects=}")
         # await self.__setup()
         # connect
         # nc, js = await self.__connect()
         streams = None
@@ -170,15 +180,14 @@
         except:
             pass
 
     def __get_messages_bg(self, subject, cb):
         asyncio.run(self.__get_messages(subject, cb))
 
     async def __get_messages(self, subject, cb):
-        
         # _, self.jss = await connect_client(self.nats_url)
         await self.__connect()
 
         psub = await self.js.pull_subscribe(subject, "psub")
 
         # Fetch and ack messagess from consumer.
         while True:
@@ -203,15 +212,14 @@
 
             except Exception as e:
                 # print(e)
                 await asyncio.sleep(2)
                 pass
 
     async def register(self, name, worker_class):
-
         # ensure worker class is initialized
         if not is_initialized(worker_class):
             raise Exception("worker_class must be initialized before registering it!")
 
         await self.__setup()
         # make & sanitize name
         name = sanitize_name(name)
@@ -221,54 +229,65 @@
         # print(subjects)
         # listen for any of these subjects
         # print(self.js)
         if not hasattr(self, "js"):
             await self.__connect()
 
         async def handle_message(msg):
-            subject = msg.subject
-            data = json.loads(msg.data.decode())
-            _, prop = subject.split(".")
-            func = getattr(worker_class, prop)
-
-            # calc latency
-            latency = pc() - data["call_start"]
-            # call worker method and pass args
-            response = await func(*data["args"])
-            # calculate total time
-            duration = pc() - data["call_start"] - latency
-
-            # compose payload
-            payload = {
-                "response": response,
-                "task": subject,
-                # "args": data["args"],
-                "req_id": data["req_id"],
-                "call_start": data["call_start"],
-                "duration": {
-                    "latency": {"request": latency},
-                    f"{subject}": precision_format_time(duration),
-                },
-            }
-
-            ack = await self.js.publish(
-                data["reply"], safe_json.dumps(payload).encode()
-            )
-
-            # acknowledge msg receipt
-            await msg.ack()
+            try:
+                subject = msg.subject
+                data = json.loads(msg.data.decode())
+                _, prop = subject.split(".")
+                func = getattr(worker_class, prop)
+
+                # print(data)
+                # calc latency
+                latency = pc() - data["call_start"]
+
+                try:
+                    # call worker method and pass args
+                    response = await func(*data["args"])
+                except Exception as e:
+                    trace_report_error()
+                    # probably exit?
+                    sys.exit()
+                # calculate total time
+                duration = pc() - data["call_start"] - latency
+
+                # compose payload
+                payload = {
+                    "response": response,
+                    "task": subject,
+                    # "args": data["args"],
+                    "req_id": data["req_id"],
+                    "call_start": data["call_start"],
+                    "duration": {
+                        "latency": {"request": latency},
+                        f"{subject}": precision_format_time(duration),
+                    },
+                }
+
+                ack = await self.js.publish(
+                    data["reply"], safe_json.dumps(payload).encode()
+                )
+
+                # acknowledge msg receipt
+                await msg.ack()
+
+            except:
+                traceback.print_exc()
+                sys.exit()
 
         for i, subject in enumerate(subjects):
             # make stream name
             stream_name = f"{app_name}_worker_" + hash_str(f"{name}_{subject}")
 
             # make stream
             await self.__add_stream(stream_name=stream_name, subjects=[subject])
-            
-            
+
             t = RaisingThread(
                 target=self.__get_messages_bg, args=[subject, handle_message]
             )
             t.start()
 
             # try:
             #     t.join()
@@ -300,48 +319,48 @@
         if not hasattr(self, "js"):
             await self.__connect()
 
         await self.__add_stream(stream_name=self.id, subjects=[self.id])
 
         ack = await self.js.publish(task, safe_json.dumps(payload).encode())
         # print(ack)
-        
+
         async def handle_message(msg):
-            
             try:
                 # print(msg)
                 if report_callback and callable(report_callback):
                     # subject = msg.subject
                     data = json.loads(msg.data.decode())
-                    
+
                     # data["duration"]["request_latency"]
                     data["duration"]["latency"]["response"] = precision_format_time(
                         pc()
                         - data["call_start"]
                         - data["duration"]["latency"]["request"]
                     )
-                    
-                    
+
                     # print( data["duration"]["latency"]["request"] )
 
                     data["duration"]["latency"]["request"] = precision_format_time(
                         data["duration"]["latency"]["request"]
                     )
 
                     del data["call_start"]
 
-                    report_callback(data)
+                    try:
+                        await report_callback(data)
+                    except Exception as e:
+                        trace_report_error("SCHEDULER/REPORT ERROR!")
+                        # exit
+                        sys.exit()
 
                     # acknowledge receipt
                     await msg.ack()
 
             except Exception as e:
                 # print(e)
                 raise e
 
-            
         t = RaisingThread(target=self.__get_messages_bg, args=[self.id, handle_message])
         t.start()
-        
-        
 
         # await __clear_streams()
```

### Comparing `classwork-0.0.4/classwork/utils.py` & `classwork-0.0.5/classwork/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,19 +4,21 @@
  This software is released under the MIT License.
  https://opensource.org/licenses/MIT
 """
 
 import os
 import sys
 import re
+import traceback
 import threading
 from hashids import Hashids
+from termcolor2 import c
 
-def precision_format_time(seconds, precision=2, last_sep = " and "):
 
+def precision_format_time(seconds, precision=2, last_sep=" and "):
     time_dict = {
         "hours": int(seconds // 3600),
         "minutes": int((seconds % 3600) // 60),
         "seconds": int(seconds % 60),
         "milliseconds": int((seconds % 1) * 1000),
         "microseconds": int((seconds % 0.001) * 1000000),
         "nanoseconds": int((seconds % 0.000001) * 1000000000),
@@ -38,40 +40,42 @@
         "nanoseconds": "ns",
         "picoseconds": "ps",
         "femtoseconds": "fs",
         "attoseconds": "as",
         "zeptoseconds": "zs",
         "yoctoseconds": "ys",
     }
-    
-    
-    time_arr = [f"{val} {time_units[unit]}" for unit, val in time_dict.items() if val>0][0:precision]
+
+    time_arr = [
+        f"{val} {time_units[unit]}" for unit, val in time_dict.items() if val > 0
+    ][0:precision]
 
     time_str = ""
-    
+
     for i, val in enumerate(time_arr):
-        time_str +=  val 
-        if i<len(time_arr)-1:
-            time_str += ", " if i<len(time_arr)-2 else last_sep 
-    
-    
+        time_str += val
+        if i < len(time_arr) - 1:
+            time_str += ", " if i < len(time_arr) - 2 else last_sep
+
     return time_str
 
+
 def importing_script():
     # get working directory
     dir = os.getcwd()
     # get script path as passed to python
     script = sys.argv[0]
     # if path is not absolute, then join with current dir
     importing_script = (
         os.path.join(dir, script) if not os.path.isabs(script) else script
     )
 
     return importing_script
 
+
 def hash_str(text, hash_length="short"):
     import hashlib
 
     a = hashlib.md5(bytes(text, encoding="utf-8"))
     b = a.hexdigest()
     as_int = int(b, 16)
     if hash_length == "short":
@@ -86,40 +90,60 @@
 class __c:
     def __init__(self) -> None:
         pass
 
 
 default_props = dir(__c)
 
+
 def is_initialized(testClass):
     return type(testClass) != type(__c)
 
+
 def get_class_props(cls):
     props = [
         p for p in dir(cls) if p not in default_props and callable(getattr(cls, p))
     ]
 
     return props
 
+
 def sanitize_name(name):
     return re.sub(r"[^\w]", "_", name)
 
+
 class RaisingThread(threading.Thread):
-  def run(self):
-    self._exc = None
-    try:
-      super().run()
-    except Exception as e:
-      self._exc = e
-
-  def join(self, timeout=None):
-    super().join(timeout=timeout)
-    
-    if self._exc:
-      raise self._exc
+    def run(self):
+        self._exc = None
+        try:
+            super().run()
+        except Exception as e:
+            self._exc = e
+
+    def join(self, timeout=None):
+        super().join(timeout=timeout)
+
+        if self._exc:
+            raise self._exc
+
 
 def trace_caller():
     try:
         raise Exception
     except Exception:
         frame = sys.exc_info()[2].tb_frame.f_back.f_back
-        print(" >> invoked by:", frame.f_code.co_name)
+        print(" >> invoked by:", frame.f_code.co_name)
+
+
+def trace_report_error(header="WORKER/TASK ERROR!"):
+    # format error in running function
+    e = traceback.format_exc()
+    # first we split by File tracebacks
+    e = e.split("File ")
+    # We discard index 1 as it points to this file
+    e.pop(1)
+
+    # Then we join back
+    e = "  File ".join(e)
+    # print error now
+    print(c(f"\n{header}").red.blink.bold.underline)
+    print(c(f"  {e}").red)
```

### Comparing `classwork-0.0.4/PKG-INFO` & `classwork-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: classwork
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple Python module to help distribute you tasks across multiple brokers as microservices
 License: MIT
 Author: Anthony Mugendi
 Author-email: ngurumugz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hashids (==1.3.1)
 Requires-Dist: nats-py (==2.2.0)
 Requires-Dist: numpy (==1.23.5)
+Requires-Dist: termcolor2 (>=0.0.3,<0.0.4)
 Requires-Dist: typjson (==0.0.32)
 Description-Content-Type: text/markdown
 
 <!--
  Copyright (c) 2023 Anthony Mugendi
  
  This software is released under the MIT License.
@@ -88,15 +89,15 @@
 
 # init ClassWork
 nats_url = "nats://127.0.0.1:4222"
 class_work = ClassWork(nats_url=nats_url)
 
 # Our callback function
 # This is where complete work gets reported
-def report_callback(report_card):
+async def report_callback(report_card):
     print("We have a report!")
     pprint(report_card)
 
 
 # We need this function to create our job schedules
 async def schedules():
     # Assign a job
@@ -116,15 +117,15 @@
 
 This code will create a *task* into NATS and the job workers (attentive students 😂) already listening will pick the task and run it, then publish their reports which is routed via NATS back to the scheduler (teacher?).
 
 Take note of the following:
 1. `class_work.assign` must be run in async mode. So we have wrapped it in an async method. You can also use `asyncio.run` directly.
 2. Naming your task is very important. This naming convection is unashamedly borrowed from [moleculer](https://moleculer.services/). In this case, your task is **"my_worker.add"**. This will route to any worker class registered with the **name** "my_worker" and method "add". 
 3. Because all this traffic is routed via NATS, your arguments must be JSON serializable. Even though we use [typ](https://github.com/vsapronov/typjson) to handle edge cases like `sets`, beware that there are limits to what you can pass in your arguments
-4. `report_callback` is called with a 'report' of your task. A report card 😊 will look like the one below:
+4. `report_callback` must be async. It is called with a 'report' of your task. A report card 😊 will look like the one below:
 
 
 ```
 We have a report!
 {'task': 'my_worker.add',
  'duration': {'latency': {'request': '4 ms and 356 µs',
                           'response': '5 s and 4 ms'},
```

