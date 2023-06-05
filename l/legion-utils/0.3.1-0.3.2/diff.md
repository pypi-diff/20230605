# Comparing `tmp/legion-utils-0.3.1.tar.gz` & `tmp/legion-utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legion-utils-0.3.1.tar", last modified: Tue Apr 25 23:43:30 2023, max compression
+gzip compressed data, was "legion-utils-0.3.2.tar", last modified: Mon Jun  5 00:05:53 2023, max compression
```

## Comparing `legion-utils-0.3.1.tar` & `legion-utils-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34500 2022-11-16 02:41:58.357856 legion-utils-0.3.1/LICENSE
--rw-r--r--   0        0        0     2573 2022-11-16 02:41:58.357856 legion-utils-0.3.1/README.md
--rw-r--r--   0        0        0      671 2022-11-16 02:41:58.357856 legion-utils-0.3.1/legion_utils/__init__.py
--rw-r--r--   0        0        0    14781 2023-04-25 23:43:26.225395 legion-utils-0.3.1/legion_utils/core.py
--rw-r--r--   0        0        0        0 2023-04-25 23:43:26.225395 legion-utils-0.3.1/legion_utils/py.typed
--rw-r--r--   0        0        0      893 2023-04-25 23:43:26.225395 legion-utils-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-16 02:41:58.357856 legion-utils-0.3.1/tests/integration/__init__.py
--rw-r--r--   0        0        0      454 2023-04-17 01:19:20.049718 legion-utils-0.3.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     5565 2023-04-17 01:27:37.589477 legion-utils-0.3.1/tests/integration/test_alert.py
--rw-r--r--   0        0        0     2104 2023-04-17 01:25:04.130604 legion-utils-0.3.1/tests/integration/utils.py
--rw-r--r--   0        0        0        0 2022-11-16 02:41:58.357856 legion-utils-0.3.1/tests/unit/__init__.py
--rw-r--r--   0        0        0    20103 2023-04-25 23:43:26.225395 legion-utils-0.3.1/tests/unit/test_alert_data.py
--rw-r--r--   0        0        0     2834 1970-01-01 00:00:00.000000 legion-utils-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-12-29 00:46:20.302885 legion-utils-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2573 2022-12-29 00:46:20.302885 legion-utils-0.3.2/README.md
+-rw-r--r--   0        0        0      671 2022-12-29 00:46:20.302885 legion-utils-0.3.2/legion_utils/__init__.py
+-rw-r--r--   0        0        0    14784 2023-06-04 23:41:12.396781 legion-utils-0.3.2/legion_utils/core.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:24:10.869550 legion-utils-0.3.2/legion_utils/py.typed
+-rw-r--r--   0        0        0      893 2023-06-05 00:00:51.230722 legion-utils-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-29 00:46:20.302885 legion-utils-0.3.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-18 03:25:48.977120 legion-utils-0.3.2/tests/integration/conftest.py
+-rw-r--r--   0        0        0     5490 2023-06-04 23:40:09.545912 legion-utils-0.3.2/tests/integration/test_alert.py
+-rw-r--r--   0        0        0     2104 2023-04-18 03:25:48.981120 legion-utils-0.3.2/tests/integration/utils.py
+-rw-r--r--   0        0        0        0 2022-12-29 00:46:20.302885 legion-utils-0.3.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0    20130 2023-06-04 23:56:39.727194 legion-utils-0.3.2/tests/unit/test_alert_data.py
+-rw-r--r--   0        0        0     2834 1970-01-01 00:00:00.000000 legion-utils-0.3.2/PKG-INFO
```

### Comparing `legion-utils-0.3.1/LICENSE` & `legion-utils-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `legion-utils-0.3.1/README.md` & `legion-utils-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `legion-utils-0.3.1/legion_utils/__init__.py` & `legion-utils-0.3.2/legion_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `legion-utils-0.3.1/legion_utils/core.py` & `legion-utils-0.3.2/legion_utils/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
     if description is not None:
         _contents["description"] = description
     if alert_key is not None:
         _contents["alert_key"] = alert_key
     _contents.update(contents)
     route += f".{priority.name.lower()}"
     Topic(exchange=exchange, config=config).broadcast(
-        Message(contents=_contents), routing_key=route
+        Message.of(contents=_contents), routing_key=route
     )
 
 
 @typechecked
 def broadcast_info(
     exchange: str,
     route: str,
```

### Comparing `legion-utils-0.3.1/pyproject.toml` & `legion-utils-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "legion-utils"
-version = "0.3.1"
+version = "0.3.2"
 description = "Utilities for Legion Reporters and Monitors"
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
-    "robotnikmq>=0.7.0",
+    "robotnikmq>=0.7.1",
 ]
 requires-python = ">=3.8.3,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "GPL-3.0-or-later"
```

### Comparing `legion-utils-0.3.1/tests/integration/test_alert.py` & `legion-utils-0.3.2/tests/integration/test_alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 def broadcast_receive(config: RobotnikConfig, pub: Callable, sub: Callable):
     msg_received = Event()
 
     def subscriber():
         for msg in Subscriber(
             [ExchangeBinding(META_QUEUE, "#")],
             config=config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         ).consume():
             sub(msg)
             msg_received.set()
 
     sub_proc = Process(target=subscriber)
     sub_proc.start()
     sleep(0.2)
```

### Comparing `legion-utils-0.3.1/tests/integration/utils.py` & `legion-utils-0.3.2/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `legion-utils-0.3.1/tests/unit/test_alert_data.py` & `legion-utils-0.3.2/tests/unit/test_alert_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,130 +349,130 @@
         assert alert.ttl == exp_ttl
         assert alert.key == exp_key
         assert alert.description == exp_desc
         assert alert.msg_src == HOSTNAME
 
 
 def test_alert_msg_of():
-    msg = Message(
+    msg = Message.of(
         {
             "alert_key": "[stuff]",
             "ttl": 60,
             "description": "Testing stuff",
             "priority": Priority.ERROR,
             "stuff": "stuff",
         }
     )
     alert = AlertMsg.of(msg)
     assert alert.contents["stuff"] == "stuff"
 
 
 def test_alert_msg_of_no_key():
-    msg = Message(
+    msg = Message.of(
         {
             "ttl": 60,
             "description": "Testing stuff",
             "priority": Priority.ERROR,
             "stuff": "stuff",
         }
     )
     with raises(ValueError):
         AlertMsg.of(msg)
         assert False
 
 
 def test_alert_msg_of_no_description():
-    msg = Message(
+    msg = Message.of(
         {
             "alert_key": "[stuff]",
             "ttl": 60,
             "priority": Priority.ERROR,
             "stuff": "stuff",
         }
     )
     with raises(ValueError):
         AlertMsg.of(msg)
         assert False
 
 
 def test_alert_msg_of_no_priority():
-    msg = Message(
+    msg = Message.of(
         {
             "alert_key": "[stuff]",
             "ttl": 60,
             "description": "Testing stuff",
             "stuff": "stuff",
         }
     )
     with raises(ValueError):
         AlertMsg.of(msg)
         assert False
 
 
 def test_alert_msg_of_no_ttl():
-    msg = Message(
+    msg = Message.of(
         {
             "alert_key": "[stuff]",
             "description": "Testing stuff",
             "priority": Priority.ERROR,
             "stuff": "stuff",
         }
     )
     with raises(ValueError):
         AlertMsg.of(msg)
         assert False
 
 
 def test_alert_msg_of_invalid_priority():
-    msg = Message(
+    msg = Message.of(
         {
             "alert_key": "[stuff]",
             "ttl": 60,
             "description": "Testing stuff",
             "priority": "Priority.ERROR",
             "stuff": "stuff",
         }
     )
     with raises(ValueError):
         AlertMsg.of(msg)
         assert False
 
 
 def test_alert_msg_of_int_priority():
-    msg = Message(
+    msg = Message.of(
         {
             "alert_key": "[stuff]",
             "ttl": 60,
             "description": "Testing stuff",
             "priority": 3,
             "stuff": "stuff",
         }
     )
     alert = AlertMsg.of(msg)
     assert alert.contents["stuff"] == "stuff"
     assert alert.priority == Priority.ERROR
 
 
 def test_alert_msg_of_invalid_ttl():
-    msg = Message(
+    msg = Message.of(
         {
             "alert_key": "[stuff]",
             "ttl": "27",
             "description": "Testing stuff",
             "priority": Priority.ERROR,
             "stuff": "stuff",
         }
     )
     with raises(ValueError):
         AlertMsg.of(msg)
         assert False
 
 
 def test_alert_msg_of_negative_ttl():
-    msg = Message(
+    msg = Message.of(
         {
             "alert_key": "[stuff]",
             "ttl": -1,
             "description": "Testing stuff",
             "priority": Priority.ERROR,
             "stuff": "stuff",
         }
```

### Comparing `legion-utils-0.3.1/PKG-INFO` & `legion-utils-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legion-utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utilities for Legion Reporters and Monitors
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
 Requires-Python: >=3.8.3,<4.0
 Description-Content-Type: text/markdown
 
 # Legion Utils
```

