# Comparing `tmp/classwork-0.0.3.tar.gz` & `tmp/classwork-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classwork-0.0.3.tar", max compression
+gzip compressed data, was "classwork-0.0.4.tar", max compression
```

## Comparing `classwork-0.0.3.tar` & `classwork-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-06-03 17:09:04.784909 classwork-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     4193 2023-06-03 16:54:31.476439 classwork-0.0.3/README.md
--rw-r--r--   0        0        0      161 2023-06-03 15:43:24.017838 classwork-0.0.3/classwork/__init__.py
--rw-r--r--   0        0        0    11060 2023-06-03 22:43:17.833105 classwork-0.0.3/classwork/main.py
--rw-r--r--   0        0        0     3086 2023-06-03 15:08:39.227871 classwork-0.0.3/classwork/utils.py
--rw-r--r--   0        0        0      451 2023-06-03 22:35:53.120516 classwork-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4922 1970-01-01 00:00:00.000000 classwork-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-03 17:09:04.784909 classwork-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     4193 2023-06-03 16:54:31.476439 classwork-0.0.4/README.md
+-rw-r--r--   0        0        0      161 2023-06-03 15:43:24.017838 classwork-0.0.4/classwork/__init__.py
+-rw-r--r--   0        0        0    11255 2023-06-04 22:42:29.676389 classwork-0.0.4/classwork/main.py
+-rw-r--r--   0        0        0     3190 2023-06-04 22:42:45.904413 classwork-0.0.4/classwork/utils.py
+-rw-r--r--   0        0        0      451 2023-06-04 22:46:14.677039 classwork-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4922 1970-01-01 00:00:00.000000 classwork-0.0.4/PKG-INFO
```

### Comparing `classwork-0.0.3/LICENSE.md` & `classwork-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.3/README.md` & `classwork-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.3/classwork/main.py` & `classwork-0.0.4/classwork/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import nats
 
 from time import perf_counter as pc
 from typ import json as safe_json
 from nats.aio.client import Client as NATS
 from nats.aio.errors import ErrNoServers, ErrTimeout
 
-from .utils import hash_str, precision_format_time, importing_script, sanitize_name, get_class_props, RaisingThread
+from .utils import hash_str, precision_format_time, importing_script, sanitize_name, get_class_props, RaisingThread, is_initialized
 
 app_name = "classwork"
 
 
 class ClassWork:
     def __init__(self, nats_url) -> None:
         self.nats_url = nats_url
@@ -203,14 +203,19 @@
 
             except Exception as e:
                 # print(e)
                 await asyncio.sleep(2)
                 pass
 
     async def register(self, name, worker_class):
+
+        # ensure worker class is initialized
+        if not is_initialized(worker_class):
+            raise Exception("worker_class must be initialized before registering it!")
+
         await self.__setup()
         # make & sanitize name
         name = sanitize_name(name)
         # make subjects
         subjects = [f"{name}.{prop}" for prop in get_class_props(worker_class)]
 
         # print(subjects)
```

### Comparing `classwork-0.0.3/classwork/utils.py` & `classwork-0.0.4/classwork/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,19 +78,25 @@
         as_int = int(re.split(r"[\.\+]", str(as_int / 32))[1][:-1])
 
     hashids = Hashids(salt=text)
     id = hashids.encode(as_int)
 
     return id
 
+
 class __c:
-    __ne__ = 1
+    def __init__(self) -> None:
+        pass
+
 
 default_props = dir(__c)
 
+def is_initialized(testClass):
+    return type(testClass) != type(__c)
+
 def get_class_props(cls):
     props = [
         p for p in dir(cls) if p not in default_props and callable(getattr(cls, p))
     ]
 
     return props
```

### Comparing `classwork-0.0.3/PKG-INFO` & `classwork-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classwork
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple Python module to help distribute you tasks across multiple brokers as microservices
 License: MIT
 Author: Anthony Mugendi
 Author-email: ngurumugz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

